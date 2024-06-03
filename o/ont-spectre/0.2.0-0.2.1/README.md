# Comparing `tmp/ont-spectre-0.2.0.tar.gz` & `tmp/ont_spectre-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ont-spectre-0.2.0.tar", last modified: Wed Apr  3 10:53:21 2024, max compression
+gzip compressed data, was "ont_spectre-0.2.1.tar", last modified: Mon Jun  3 12:17:26 2024, max compression
```

## Comparing `ont-spectre-0.2.0.tar` & `ont_spectre-0.2.1.tar`

### file list

```diff
@@ -1,56 +1,49 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 10:53:21.280399 ont-spectre-0.2.0/
--rw-rw-rw-   0 root         (0) root         (0)    14378 2024-04-03 10:50:01.000000 ont-spectre-0.2.0/LICENSE.md
--rw-rw-rw-   0 root         (0) root         (0)       89 2024-04-03 10:50:01.000000 ont-spectre-0.2.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2923 2024-04-03 10:53:21.280399 ont-spectre-0.2.0/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     2437 2024-04-03 10:50:01.000000 ont-spectre-0.2.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 10:53:21.280399 ont-spectre-0.2.0/ont_spectre.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2923 2024-04-03 10:53:21.000000 ont-spectre-0.2.0/ont_spectre.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1330 2024-04-03 10:53:21.000000 ont-spectre-0.2.0/ont_spectre.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-03 10:53:21.000000 ont-spectre-0.2.0/ont_spectre.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       50 2024-04-03 10:53:21.000000 ont-spectre-0.2.0/ont_spectre.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-03 10:53:21.000000 ont-spectre-0.2.0/ont_spectre.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       90 2024-04-03 10:53:21.000000 ont-spectre-0.2.0/ont_spectre.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2024-04-03 10:53:21.000000 ont-spectre-0.2.0/ont_spectre.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)       89 2024-04-03 10:50:01.000000 ont-spectre-0.2.0/requirements.txt
--rw-r--r--   0 root         (0) root         (0)       38 2024-04-03 10:53:21.280399 ont-spectre-0.2.0/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     2054 2024-04-03 10:50:01.000000 ont-spectre-0.2.0/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 10:53:21.228395 ont-spectre-0.2.0/spectre/
--rw-rw-rw-   0 root         (0) root         (0)       22 2024-04-03 10:50:01.000000 ont-spectre-0.2.0/spectre/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 10:53:21.232395 ont-spectre-0.2.0/spectre/analysis/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-03 10:50:01.000000 ont-spectre-0.2.0/spectre/analysis/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    35027 2024-04-03 10:50:01.000000 ont-spectre-0.2.0/spectre/analysis/analysis.py
--rw-rw-rw-   0 root         (0) root         (0)     6283 2024-04-03 10:50:01.000000 ont-spectre-0.2.0/spectre/analysis/call_cnv_AF.py
--rw-rw-rw-   0 root         (0) root         (0)     4279 2024-04-03 10:50:01.000000 ont-spectre-0.2.0/spectre/analysis/call_cnv_coverage.py
--rw-rw-rw-   0 root         (0) root         (0)     4022 2024-04-03 10:50:01.000000 ont-spectre-0.2.0/spectre/analysis/cnv_candidate.py
--rw-rw-rw-   0 root         (0) root         (0)    22029 2024-04-03 10:50:01.000000 ont-spectre-0.2.0/spectre/analysis/cnv_metrics.py
--rw-rw-rw-   0 root         (0) root         (0)     1490 2024-04-03 10:50:01.000000 ont-spectre-0.2.0/spectre/analysis/coverage_stats.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 10:53:21.256397 ont-spectre-0.2.0/spectre/data/
--rw-rw-rw-   0 root         (0) root         (0)    45118 2024-04-03 10:50:01.000000 ont-spectre-0.2.0/spectre/data/black_list_bins_0.01_merged.bed
--rw-rw-rw-   0 root         (0) root         (0)    39045 2024-04-03 10:50:01.000000 ont-spectre-0.2.0/spectre/data/black_list_bins_0.02_merged.bed
--rw-rw-rw-   0 root         (0) root         (0)    77227 2024-04-03 10:50:01.000000 ont-spectre-0.2.0/spectre/data/black_list_bins_0.03_merged.bed
--rw-rw-rw-   0 root         (0) root         (0)     2057 2024-04-03 10:50:01.000000 ont-spectre-0.2.0/spectre/data/grch37_blacklist_normal.bed
--rw-rw-rw-   0 root         (0) root         (0)     3212 2024-04-03 10:50:01.000000 ont-spectre-0.2.0/spectre/data/grch37_blacklist_plus.bed
--rw-rw-rw-   0 root         (0) root         (0)     2543 2024-04-03 10:50:01.000000 ont-spectre-0.2.0/spectre/data/grch37_blacklist_spectre.bed
--rw-rw-rw-   0 root         (0) root         (0)     4672 2024-04-03 10:50:01.000000 ont-spectre-0.2.0/spectre/data/grch38_blacklist.bed
--rw-rw-rw-   0 root         (0) root         (0)      199 2024-04-03 10:50:01.000000 ont-spectre-0.2.0/spectre/data/grch38_y.txt
--rw-rw-rw-   0 root         (0) root         (0)    23894 2024-04-03 10:50:01.000000 ont-spectre-0.2.0/spectre/data/metadata_GRCh38_no_alt.mdr
--rw-rw-rw-   0 root         (0) root         (0)    26684 2024-04-03 10:50:01.000000 ont-spectre-0.2.0/spectre/main.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 10:53:21.276399 ont-spectre-0.2.0/spectre/plots/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-03 10:50:01.000000 ont-spectre-0.2.0/spectre/plots/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4194 2024-04-03 10:50:01.000000 ont-spectre-0.2.0/spectre/plots/plot.py
--rw-rw-rw-   0 root         (0) root         (0)     6569 2024-04-03 10:50:01.000000 ont-spectre-0.2.0/spectre/spectreCNV.py
--rw-rw-rw-   0 root         (0) root         (0)    11195 2024-04-03 10:50:01.000000 ont-spectre-0.2.0/spectre/spectreCNVPopulation.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 10:53:21.276399 ont-spectre-0.2.0/spectre/util/
--rw-rw-rw-   0 root         (0) root         (0)     1505 2024-04-03 10:50:01.000000 ont-spectre-0.2.0/spectre/util/OSUtil.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-03 10:50:01.000000 ont-spectre-0.2.0/spectre/util/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1251 2024-04-03 10:50:01.000000 ont-spectre-0.2.0/spectre/util/cnv_id.py
--rw-rw-rw-   0 root         (0) root         (0)     1990 2024-04-03 10:50:01.000000 ont-spectre-0.2.0/spectre/util/dataAnalyzer.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 10:53:21.280399 ont-spectre-0.2.0/spectre/util/metadata/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-03 10:50:01.000000 ont-spectre-0.2.0/spectre/util/metadata/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     7403 2024-04-03 10:50:01.000000 ont-spectre-0.2.0/spectre/util/metadata/metadataCollector.py
--rw-rw-rw-   0 root         (0) root         (0)     2115 2024-04-03 10:50:01.000000 ont-spectre-0.2.0/spectre/util/mosdepthReader.py
--rw-rw-rw-   0 root         (0) root         (0)     9857 2024-04-03 10:50:01.000000 ont-spectre-0.2.0/spectre/util/outputWriter.py
--rw-rw-rw-   0 root         (0) root         (0)    11029 2024-04-03 10:50:01.000000 ont-spectre-0.2.0/spectre/util/vcf_parser.py
--rw-rw-rw-   0 root         (0) root         (0)     1088 2024-04-03 10:50:01.000000 ont-spectre-0.2.0/spectre-license.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 10:53:21.280399 ont-spectre-0.2.0/tests/
--rw-rw-rw-   0 root         (0) root         (0)       91 2024-04-03 10:50:01.000000 ont-spectre-0.2.0/tests/test_main.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-06-03 12:17:26.902572 ont_spectre-0.2.1/
+-rw-rw-rw-   0 root         (0) root         (0)    14378 2024-06-03 12:14:18.000000 ont_spectre-0.2.1/LICENSE.md
+-rw-rw-rw-   0 root         (0) root         (0)       89 2024-06-03 12:14:18.000000 ont_spectre-0.2.1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     1523 2024-06-03 12:17:26.898571 ont_spectre-0.2.1/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     1027 2024-06-03 12:14:18.000000 ont_spectre-0.2.1/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-06-03 12:17:26.898571 ont_spectre-0.2.1/ont_spectre.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1523 2024-06-03 12:17:26.000000 ont_spectre-0.2.1/ont_spectre.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1044 2024-06-03 12:17:26.000000 ont_spectre-0.2.1/ont_spectre.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-06-03 12:17:26.000000 ont_spectre-0.2.1/ont_spectre.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       50 2024-06-03 12:17:26.000000 ont_spectre-0.2.1/ont_spectre.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-06-03 12:17:26.000000 ont_spectre-0.2.1/ont_spectre.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       99 2024-06-03 12:17:26.000000 ont_spectre-0.2.1/ont_spectre.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2024-06-03 12:17:26.000000 ont_spectre-0.2.1/ont_spectre.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)       98 2024-06-03 12:14:18.000000 ont_spectre-0.2.1/requirements.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2024-06-03 12:17:26.902572 ont_spectre-0.2.1/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     2054 2024-06-03 12:14:18.000000 ont_spectre-0.2.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-06-03 12:17:26.894571 ont_spectre-0.2.1/spectre/
+-rw-rw-rw-   0 root         (0) root         (0)       22 2024-06-03 12:14:18.000000 ont_spectre-0.2.1/spectre/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-06-03 12:17:26.898571 ont_spectre-0.2.1/spectre/analysis/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-06-03 12:14:18.000000 ont_spectre-0.2.1/spectre/analysis/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    35100 2024-06-03 12:14:18.000000 ont_spectre-0.2.1/spectre/analysis/analysis.py
+-rw-rw-rw-   0 root         (0) root         (0)     6283 2024-06-03 12:14:18.000000 ont_spectre-0.2.1/spectre/analysis/call_cnv_AF.py
+-rw-rw-rw-   0 root         (0) root         (0)     4279 2024-06-03 12:14:18.000000 ont_spectre-0.2.1/spectre/analysis/call_cnv_coverage.py
+-rw-rw-rw-   0 root         (0) root         (0)     4022 2024-06-03 12:14:18.000000 ont_spectre-0.2.1/spectre/analysis/cnv_candidate.py
+-rw-rw-rw-   0 root         (0) root         (0)    22029 2024-06-03 12:14:18.000000 ont_spectre-0.2.1/spectre/analysis/cnv_metrics.py
+-rw-rw-rw-   0 root         (0) root         (0)     1490 2024-06-03 12:14:18.000000 ont_spectre-0.2.1/spectre/analysis/coverage_stats.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-06-03 12:17:26.898571 ont_spectre-0.2.1/spectre/data/
+-rw-rw-rw-   0 root         (0) root         (0)   147419 2024-06-03 12:14:18.000000 ont_spectre-0.2.1/spectre/data/grch38_blacklist_0.3.bed
+-rw-rw-rw-   0 root         (0) root         (0)    45241 2024-06-03 12:14:18.000000 ont_spectre-0.2.1/spectre/data/grch38_metadata.mdr
+-rw-rw-rw-   0 root         (0) root         (0)    27956 2024-06-03 12:14:18.000000 ont_spectre-0.2.1/spectre/main.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-06-03 12:17:26.898571 ont_spectre-0.2.1/spectre/plots/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-06-03 12:14:18.000000 ont_spectre-0.2.1/spectre/plots/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4194 2024-06-03 12:14:18.000000 ont_spectre-0.2.1/spectre/plots/plot.py
+-rw-rw-rw-   0 root         (0) root         (0)     6569 2024-06-03 12:14:18.000000 ont_spectre-0.2.1/spectre/spectreCNV.py
+-rw-rw-rw-   0 root         (0) root         (0)    11195 2024-06-03 12:14:18.000000 ont_spectre-0.2.1/spectre/spectreCNVPopulation.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-06-03 12:17:26.898571 ont_spectre-0.2.1/spectre/util/
+-rw-rw-rw-   0 root         (0) root         (0)     1505 2024-06-03 12:14:18.000000 ont_spectre-0.2.1/spectre/util/OSUtil.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-06-03 12:14:18.000000 ont_spectre-0.2.1/spectre/util/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1251 2024-06-03 12:14:18.000000 ont_spectre-0.2.1/spectre/util/cnv_id.py
+-rw-rw-rw-   0 root         (0) root         (0)     1990 2024-06-03 12:14:18.000000 ont_spectre-0.2.1/spectre/util/dataAnalyzer.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-06-03 12:17:26.898571 ont_spectre-0.2.1/spectre/util/metadata/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-06-03 12:14:18.000000 ont_spectre-0.2.1/spectre/util/metadata/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     7194 2024-06-03 12:14:18.000000 ont_spectre-0.2.1/spectre/util/metadata/metadataCollector.py
+-rw-rw-rw-   0 root         (0) root         (0)     2115 2024-06-03 12:14:18.000000 ont_spectre-0.2.1/spectre/util/mosdepthReader.py
+-rw-rw-rw-   0 root         (0) root         (0)    10043 2024-06-03 12:14:18.000000 ont_spectre-0.2.1/spectre/util/outputWriter.py
+-rw-rw-rw-   0 root         (0) root         (0)    11029 2024-06-03 12:14:18.000000 ont_spectre-0.2.1/spectre/util/vcf_parser.py
+-rw-rw-rw-   0 root         (0) root         (0)     1088 2024-06-03 12:14:18.000000 ont_spectre-0.2.1/spectre-license.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-06-03 12:17:26.898571 ont_spectre-0.2.1/tests/
+-rw-rw-rw-   0 root         (0) root         (0)       91 2024-06-03 12:14:18.000000 ont_spectre-0.2.1/tests/test_main.py
```

### Comparing `ont-spectre-0.2.0/LICENSE.md` & `ont_spectre-0.2.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `ont-spectre-0.2.0/PKG-INFO` & `ont_spectre-0.2.1/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,92 +1,59 @@
 Metadata-Version: 2.1
 Name: ont-spectre
-Version: 0.2.0
+Version: 0.2.1
 Summary: Oxford Nanopore Technologies Plc. fork of Spectre CNV caller
 Home-page: https://github.com/epi2me-labs/ont-spectre
 Author: epi2melabs
 Author-email: epi2melabs@nanoporetech.com
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
-Requires-Dist: pysam==0.21.0
-Requires-Dist: numpy==1.24.3
-Requires-Dist: pandas==2.0.1
-Requires-Dist: matplotlib==3.7.1
-Requires-Dist: scipy==1.10.1
-Requires-Dist: polars==0.19.15
+Requires-Dist: pysam>=0.22.0
+Requires-Dist: numpy>=1.24.3
+Requires-Dist: pandas>=2.0.1
+Requires-Dist: matplotlib>=3.7.1
+Requires-Dist: scipy>=1.10.1
+Requires-Dist: polars[pyarrow]>=0.19.15
 
 
 ![Spectre](./logo.png)
 # Spectre - Long read CNV caller
 
-## Required programs (conda)
+## Installation
+Recommended ways of installation are using pip or conda or pip package:
+```
+pip install ont-spectre
+```
+(or)
+```
+conda install nanoporetech::ont-spectre
+```
+
+## Run from sources
 
 Setup a conda environment for Spectre (copy and paste the following commands)
-```bash
-conda create -n spectre python=3.8.5 pysam==0.21.0 numpy==1.24.3 pandas==2.0.1 matplotlib==3.7.1 scipy==1.10.1 -y
-conda activate spectre
-```
-Alternatively, you can use pip for installing the packages stored in the requirements txt
 
 ```bash
 conda create -n spectre python=3.8.5 pip -y
 conda activate spectre
 pip install -r requirements.txt
 ```
-or install everything manually (check for package version in the requirements.txt file)
-
-|Program| Conda                               |
-|-------|-------------------------------------|
-| python3 | conda install python=3.8.5          |
-| pysam | conda install -c bioconda pysam=0.21.0     |
-| pandas| conda install -c anaconda pandas==2.0.1    |
-| numpy| conda install -c anaconda numpy==1.24.3     |
-| scipy| conda install -c anaconda scipy==1.10.1     |
-| matplotlib| conda install -c anaconda matplotlib==3.7.1 |
-
 
 ## How to run
 Spectre need as input:
 - The result of Mosdepth (directory)
 - Reference genome (can be bgzip compressed)
 - Window size used in Mosdepth (Make sure the binsize between Mosdepth and Spectre are matching. We suggest a binsize of 1000 base pairs.)
-
-Optional
 - VCF file containing SNV
 
 >INFO: Make sure to include "/" at the end if you are adding directory paths.
 
 
 ```bash
-spectre.py CNVCaller \
+spectre CNVCaller \
   --bin-size 1000 \
   --coverage mosdepth/sampleid/ \
   --sample-id sampleid \
   --output-dir sampleid_output_directory_path/ \
   --reference reference.fasta.gz \
   --snv sampleid.vcf.gz
 ```
-### Run Spectre with multiple samples
-Run Spectre with multiple samples:
->INFO: This will start the population mode automatically.
-
-```bash
-spectre.py CNVCaller \
-  --bin-size 1000 \
-  --coverage mosdepth/sampleid-1/ mosdepth/sampleid-1/ \
-  --sample-id sampleid-1 sampleid-2 \
-  --output-dir sampleid_output_directory_path/ \
-  --reference reference.fasta.gz \
-  --snv sampleid.vcf.gz
-```
-
-### Population mode
-Run Spectre in population mode with two or more samples:
->INFO: Spectre produces an intermediate file (.spc) which contains all calculated CNVs from a given samples. They are 
-> located in the output folder of given sample.
-
-```bash
-spectre.py population \
-  --candidates /path/to/sample1.spc /path/to/sample2.spc \
-  --sample-id output_name \
-  --output-dir sampleid_output_directory_path/
-```
```

### Comparing `ont-spectre-0.2.0/README.md` & `ont_spectre-0.2.1/ont_spectre.egg-info/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,76 +1,59 @@
+Metadata-Version: 2.1
+Name: ont-spectre
+Version: 0.2.1
+Summary: Oxford Nanopore Technologies Plc. fork of Spectre CNV caller
+Home-page: https://github.com/epi2me-labs/ont-spectre
+Author: epi2melabs
+Author-email: epi2melabs@nanoporetech.com
+Description-Content-Type: text/markdown
+License-File: LICENSE.md
+Requires-Dist: pysam>=0.22.0
+Requires-Dist: numpy>=1.24.3
+Requires-Dist: pandas>=2.0.1
+Requires-Dist: matplotlib>=3.7.1
+Requires-Dist: scipy>=1.10.1
+Requires-Dist: polars[pyarrow]>=0.19.15
+
 
 ![Spectre](./logo.png)
 # Spectre - Long read CNV caller
 
-## Required programs (conda)
+## Installation
+Recommended ways of installation are using pip or conda or pip package:
+```
+pip install ont-spectre
+```
+(or)
+```
+conda install nanoporetech::ont-spectre
+```
+
+## Run from sources
 
 Setup a conda environment for Spectre (copy and paste the following commands)
-```bash
-conda create -n spectre python=3.8.5 pysam==0.21.0 numpy==1.24.3 pandas==2.0.1 matplotlib==3.7.1 scipy==1.10.1 -y
-conda activate spectre
-```
-Alternatively, you can use pip for installing the packages stored in the requirements txt
 
 ```bash
 conda create -n spectre python=3.8.5 pip -y
 conda activate spectre
 pip install -r requirements.txt
 ```
-or install everything manually (check for package version in the requirements.txt file)
-
-|Program| Conda                               |
-|-------|-------------------------------------|
-| python3 | conda install python=3.8.5          |
-| pysam | conda install -c bioconda pysam=0.21.0     |
-| pandas| conda install -c anaconda pandas==2.0.1    |
-| numpy| conda install -c anaconda numpy==1.24.3     |
-| scipy| conda install -c anaconda scipy==1.10.1     |
-| matplotlib| conda install -c anaconda matplotlib==3.7.1 |
-
 
 ## How to run
 Spectre need as input:
 - The result of Mosdepth (directory)
 - Reference genome (can be bgzip compressed)
 - Window size used in Mosdepth (Make sure the binsize between Mosdepth and Spectre are matching. We suggest a binsize of 1000 base pairs.)
-
-Optional
 - VCF file containing SNV
 
 >INFO: Make sure to include "/" at the end if you are adding directory paths.
 
 
 ```bash
-spectre.py CNVCaller \
+spectre CNVCaller \
   --bin-size 1000 \
   --coverage mosdepth/sampleid/ \
   --sample-id sampleid \
   --output-dir sampleid_output_directory_path/ \
   --reference reference.fasta.gz \
   --snv sampleid.vcf.gz
 ```
-### Run Spectre with multiple samples
-Run Spectre with multiple samples:
->INFO: This will start the population mode automatically.
-
-```bash
-spectre.py CNVCaller \
-  --bin-size 1000 \
-  --coverage mosdepth/sampleid-1/ mosdepth/sampleid-1/ \
-  --sample-id sampleid-1 sampleid-2 \
-  --output-dir sampleid_output_directory_path/ \
-  --reference reference.fasta.gz \
-  --snv sampleid.vcf.gz
-```
-
-### Population mode
-Run Spectre in population mode with two or more samples:
->INFO: Spectre produces an intermediate file (.spc) which contains all calculated CNVs from a given samples. They are 
-> located in the output folder of given sample.
-
-```bash
-spectre.py population \
-  --candidates /path/to/sample1.spc /path/to/sample2.spc \
-  --sample-id output_name \
-  --output-dir sampleid_output_directory_path/
-```
```

### Comparing `ont-spectre-0.2.0/setup.py` & `ont_spectre-0.2.1/setup.py`

 * *Files identical despite different names*

### Comparing `ont-spectre-0.2.0/spectre/analysis/analysis.py` & `ont_spectre-0.2.1/spectre/analysis/analysis.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,14 +17,15 @@
 from spectre.util import outputWriter
 from spectre.util import vcf_parser
 from spectre.util.dataAnalyzer import NormaldataAnalyser as NorAn
 from spectre.util.cnv_id import CNV_ID
 from spectre.util.OSUtil import OSUtil as OSUt
 
 MOSDEPTH_HEADER = ['chrom_', 'start_', 'end_', 'coverage_']
+MOSDEPTH_DTYPES = [pl.Utf8, pl.Int64, pl.Int64, pl.Float64]
 
 class CNVAnalysis(object):
     def __init__(self, coverage_file, coverage_mosdepth_data, bin_size, output_directory, outbed, outvcf, genome_info,
                  sample_id, metadata_ref, snv_file, only_chr_list="", ploidy=2,min_cnv_len=1000000, as_dev=False,
                  dev_params=None, debug_dir="", dist_proportion=0.25, threshhold_quantile=5):
         # input
         self.coverage_file = coverage_file
@@ -112,15 +113,21 @@
         self.logger.info("Parsing VCF to AF freqs file")
         vcf = vcf_parser.VCFSNVParser(self.min_chr_length, self.as_dev)
         vcf_df = pl.from_pandas(vcf.vcf_to_dataframe(self.snv_file))
         vcf_df = vcf_df.with_columns(pl.col('start_').apply(lambda x: x // self.bin_size * self.bin_size))
 
         af_good_bins_df = self.annotate_bins_df(vcf_df)
 
-        coverages_df = pl.read_csv(self.coverage_full_path, has_header=False, separator='\t', new_columns=MOSDEPTH_HEADER)
+        coverages_df = pl.read_csv(
+            self.coverage_full_path,
+            has_header=False,
+            separator='\t',
+            new_columns=MOSDEPTH_HEADER,
+            dtypes=MOSDEPTH_DTYPES
+        )
         coverages_df = coverages_df.join(af_good_bins_df, on=['chrom_', 'start_'], how='left')
         self.coverages_df = coverages_df.with_columns(pl.col("af_good").fill_null(False))
 
         self.coverages_df_diploid = self.coverages_df.filter(af_good=True)
 
     def detect_xy_chromosome_proidness(self, genome_median, coverage_lower_threshold):
         # Detecting chrY has some caverage
@@ -377,15 +384,14 @@
             while n_merges > 0:
                 merge_rounds += 1
                 self.logger.debug(f'Current merge cycle {merge_rounds}')
                 self.logger.info(f'n candidates in {chromosome_name}: {len(merged_candidates)}')
                 [n_merges, merged_candidates, dev_candidates_string] = self.cnv_candidate_merge(merged_candidates)
                 self.logger.debug([f'{c.start}-{c.end}, ({c.type},{c.size})' for c in merged_candidates])
 
-            self.logger.debug(f'dev_candidates_string: {dev_candidates_string}')
             self.logger.debug(f'Total merge rounds: {merge_rounds}')
 
             [n_merges, merged_candidates, _] = self.cnv_candidate_merge(cnv_candidates=merged_candidates,
                                                                         allow_over_blacklist_merging=True)
             self.logger.debug(f'Merged with final blacklist ignoring round: {n_merges}')
 
             candidates_cnv_list = self.clean_merged_candidates(merged_candidates)
```

### Comparing `ont-spectre-0.2.0/spectre/analysis/call_cnv_AF.py` & `ont_spectre-0.2.1/spectre/analysis/call_cnv_AF.py`

 * *Files identical despite different names*

### Comparing `ont-spectre-0.2.0/spectre/analysis/call_cnv_coverage.py` & `ont_spectre-0.2.1/spectre/analysis/call_cnv_coverage.py`

 * *Files identical despite different names*

### Comparing `ont-spectre-0.2.0/spectre/analysis/cnv_candidate.py` & `ont_spectre-0.2.1/spectre/analysis/cnv_candidate.py`

 * *Files identical despite different names*

### Comparing `ont-spectre-0.2.0/spectre/analysis/cnv_metrics.py` & `ont_spectre-0.2.1/spectre/analysis/cnv_metrics.py`

 * *Files identical despite different names*

### Comparing `ont-spectre-0.2.0/spectre/analysis/coverage_stats.py` & `ont_spectre-0.2.1/spectre/analysis/coverage_stats.py`

 * *Files identical despite different names*

### Comparing `ont-spectre-0.2.0/spectre/data/metadata_GRCh38_no_alt.mdr` & `ont_spectre-0.2.1/spectre/data/grch38_metadata.mdr`

 * *Files 25% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #####	Statistic report
 #####	Basepair statistic
 BPDEF	A	T	C	G	GC%	Total bp
-BPSTA	866420001	868918077	598683433	600854940	698124.4495789271	171823
+BPSTA	1732840002	1737836154	1197366866	1201709880	1396248.8991578542	343646
 #####	N-Sequence positions in given reference file
 NSDEF	From	To
 NSPOS	chr1	0	10000
 NSPOS	chr1	207000	258000
 NSPOS	chr1	297000	348000
 NSPOS	chr1	535000	586000
 NSPOS	chr1	2702000	2747000
@@ -780,7 +780,787 @@
 NSPOS	chrUn_KI270741v1	126000	127000
 NSPOS	chrUn_KI270741v1	127000	129000
 NSPOS	chrUn_KI270756v1	11000	12000
 NSPOS	chrUn_KI270757v1	10000	15000
 NSPOS	chrUn_KI270757v1	16000	21000
 NSPOS	chrUn_KI270757v1	44000	47000
 NSPOS	chrUn_GL000216v2	1000	2000
+NSPOS	1	0	10000
+NSPOS	1	207000	258000
+NSPOS	1	297000	348000
+NSPOS	1	535000	586000
+NSPOS	1	2702000	2747000
+NSPOS	1	12954000	13005000
+NSPOS	1	16799000	16850000
+NSPOS	1	29552000	29554000
+NSPOS	1	121757000	121758000
+NSPOS	1	121757000	121759000
+NSPOS	1	121768000	121769000
+NSPOS	1	121776000	121777000
+NSPOS	1	121778000	121780000
+NSPOS	1	121781000	121782000
+NSPOS	1	121792000	121793000
+NSPOS	1	121796000	121797000
+NSPOS	1	121799000	121800000
+NSPOS	1	121804000	121805000
+NSPOS	1	121807000	121808000
+NSPOS	1	121810000	121811000
+NSPOS	1	121813000	121814000
+NSPOS	1	121815000	121816000
+NSPOS	1	121823000	121824000
+NSPOS	1	121826000	121827000
+NSPOS	1	121829000	121830000
+NSPOS	1	121845000	121846000
+NSPOS	1	121851000	121852000
+NSPOS	1	121856000	121857000
+NSPOS	1	121867000	121868000
+NSPOS	1	121870000	121871000
+NSPOS	1	121873000	121874000
+NSPOS	1	121890000	121891000
+NSPOS	1	121893000	121894000
+NSPOS	1	121898000	121899000
+NSPOS	1	121902000	121903000
+NSPOS	1	121911000	121912000
+NSPOS	1	121914000	121915000
+NSPOS	1	121916000	121917000
+NSPOS	1	121923000	121924000
+NSPOS	1	121926000	121927000
+NSPOS	1	121930000	121931000
+NSPOS	1	121935000	121936000
+NSPOS	1	121940000	121941000
+NSPOS	1	121944000	121945000
+NSPOS	1	121946000	121948000
+NSPOS	1	121950000	121951000
+NSPOS	1	121953000	121954000
+NSPOS	1	121955000	121956000
+NSPOS	1	121958000	121959000
+NSPOS	1	121963000	121964000
+NSPOS	1	121965000	121966000
+NSPOS	1	121968000	121969000
+NSPOS	1	121972000	121973000
+NSPOS	1	121974000	121975000
+NSPOS	1	121976000	122027000
+NSPOS	1	122056000	122057000
+NSPOS	1	122102000	122104000
+NSPOS	1	122109000	122110000
+NSPOS	1	122125000	122126000
+NSPOS	1	122173000	122175000
+NSPOS	1	122224000	122225000
+NSPOS	1	122229000	122231000
+NSPOS	1	122237000	122238000
+NSPOS	1	122503000	122504000
+NSPOS	1	124785000	124786000
+NSPOS	1	124849000	124850000
+NSPOS	1	124932000	124933000
+NSPOS	1	124977000	124979000
+NSPOS	1	125013000	125014000
+NSPOS	1	125026000	125027000
+NSPOS	1	125029000	125030000
+NSPOS	1	125103000	125104000
+NSPOS	1	125130000	125132000
+NSPOS	1	125171000	125174000
+NSPOS	1	125184000	143185000
+NSPOS	1	223558000	223609000
+NSPOS	1	228558000	228609000
+NSPOS	2	0	10000
+NSPOS	2	16145000	16147000
+NSPOS	2	32867000	32869000
+NSPOS	2	32916000	32918000
+NSPOS	2	89330000	89531000
+NSPOS	2	89685000	89754000
+NSPOS	2	90402000	91403000
+NSPOS	2	92138000	92189000
+NSPOS	2	92270000	92272000
+NSPOS	2	92701000	92703000
+NSPOS	2	92879000	92880000
+NSPOS	2	93296000	93297000
+NSPOS	2	93465000	93466000
+NSPOS	2	93598000	93599000
+NSPOS	2	93694000	93695000
+NSPOS	2	93921000	93922000
+NSPOS	2	94014000	94015000
+NSPOS	2	94090000	94141000
+NSPOS	2	94293000	94497000
+NSPOS	2	97439000	97490000
+NSPOS	2	238903000	238905000
+NSPOS	3	0	10000
+NSPOS	3	90550000	90551000
+NSPOS	3	90565000	90569000
+NSPOS	3	90699000	90700000
+NSPOS	3	90722000	90773000
+NSPOS	3	91233000	91234000
+NSPOS	3	91247000	91248000
+NSPOS	3	91249000	91257000
+NSPOS	3	91257000	91261000
+NSPOS	3	91265000	91277000
+NSPOS	3	91282000	91283000
+NSPOS	3	91291000	91292000
+NSPOS	3	91345000	91346000
+NSPOS	3	91364000	91365000
+NSPOS	3	91438000	91439000
+NSPOS	3	91553000	91554000
+NSPOS	3	91891000	91892000
+NSPOS	3	93470000	93471000
+NSPOS	3	93655000	93706000
+NSPOS	4	0	10000
+NSPOS	4	1429000	1435000
+NSPOS	4	1435000	1442000
+NSPOS	4	8797000	8817000
+NSPOS	4	9272000	9323000
+NSPOS	4	31819000	31833000
+NSPOS	4	31835000	31836000
+NSPOS	4	32833000	32840000
+NSPOS	4	49336000	49487000
+NSPOS	4	49658000	49709000
+NSPOS	4	49711000	49713000
+NSPOS	4	50475000	50476000
+NSPOS	4	51107000	51108000
+NSPOS	4	51418000	51420000
+NSPOS	4	51743000	51794000
+NSPOS	4	58878000	58922000
+NSPOS	4	190123000	190174000
+NSPOS	5	0	10000
+NSPOS	5	17530000	17581000
+NSPOS	5	46435000	46486000
+NSPOS	5	46527000	46528000
+NSPOS	5	46546000	46547000
+NSPOS	5	46553000	46554000
+NSPOS	5	46563000	46565000
+NSPOS	5	46569000	46570000
+NSPOS	5	46624000	46625000
+NSPOS	5	46796000	46797000
+NSPOS	5	47032000	47033000
+NSPOS	5	47061000	47062000
+NSPOS	5	47069000	47074000
+NSPOS	5	47078000	47079000
+NSPOS	5	47079000	47083000
+NSPOS	5	47106000	47107000
+NSPOS	5	47153000	47154000
+NSPOS	5	47296000	47297000
+NSPOS	5	47300000	47307000
+NSPOS	5	47309000	49592000
+NSPOS	5	49592000	49600000
+NSPOS	5	49600000	49602000
+NSPOS	5	49603000	49610000
+NSPOS	5	49611000	49613000
+NSPOS	5	49618000	49622000
+NSPOS	5	49628000	49631000
+NSPOS	5	49633000	49642000
+NSPOS	5	49646000	49647000
+NSPOS	5	49650000	49657000
+NSPOS	5	49661000	49667000
+NSPOS	5	49667000	49668000
+NSPOS	5	49721000	49722000
+NSPOS	5	50059000	50110000
+NSPOS	5	139452000	139454000
+NSPOS	5	155760000	155762000
+NSPOS	6	0	60000
+NSPOS	6	58453000	58554000
+NSPOS	6	59439000	59440000
+NSPOS	6	59818000	59820000
+NSPOS	6	59829000	60230000
+NSPOS	6	61357000	61364000
+NSPOS	6	61370000	61372000
+NSPOS	6	61378000	61379000
+NSPOS	6	61381000	61382000
+NSPOS	6	61393000	61394000
+NSPOS	6	61398000	61399000
+NSPOS	6	95020000	95071000
+NSPOS	6	167591000	167642000
+NSPOS	7	0	10000
+NSPOS	7	237000	241000
+NSPOS	7	58119000	58170000
+NSPOS	7	58272000	58273000
+NSPOS	7	58356000	58357000
+NSPOS	7	58756000	58757000
+NSPOS	7	59509000	59510000
+NSPOS	7	60250000	60252000
+NSPOS	7	60828000	60879000
+NSPOS	7	61063000	61064000
+NSPOS	7	61327000	61378000
+NSPOS	7	61528000	61579000
+NSPOS	7	61964000	61968000
+NSPOS	7	61976000	62027000
+NSPOS	7	62456000	62507000
+NSPOS	7	143650000	143701000
+NSPOS	8	0	60000
+NSPOS	8	7617000	7668000
+NSPOS	8	12234000	12285000
+NSPOS	8	43983000	44034000
+NSPOS	8	44228000	44230000
+NSPOS	8	45196000	45197000
+NSPOS	8	45344000	45346000
+NSPOS	8	45500000	45501000
+NSPOS	8	45864000	45865000
+NSPOS	8	45877000	45928000
+NSPOS	8	85664000	85715000
+NSPOS	9	0	10000
+NSPOS	9	40529000	40530000
+NSPOS	9	40537000	40538000
+NSPOS	9	40547000	40548000
+NSPOS	9	40561000	40562000
+NSPOS	9	41225000	41230000
+NSPOS	9	41237000	41239000
+NSPOS	9	43222000	43237000
+NSPOS	9	43240000	43241000
+NSPOS	9	43254000	43255000
+NSPOS	9	43263000	43264000
+NSPOS	9	43268000	43269000
+NSPOS	9	43270000	43275000
+NSPOS	9	43276000	43277000
+NSPOS	9	43281000	43283000
+NSPOS	9	43332000	43334000
+NSPOS	9	43370000	43372000
+NSPOS	9	43377000	43383000
+NSPOS	9	43389000	43390000
+NSPOS	9	44851000	44852000
+NSPOS	9	45518000	60519000
+NSPOS	9	60688000	60739000
+NSPOS	9	60779000	60830000
+NSPOS	9	61003000	61054000
+NSPOS	9	61231000	61282000
+NSPOS	9	61468000	61519000
+NSPOS	9	61735000	61786000
+NSPOS	9	62149000	62250000
+NSPOS	9	62748000	62799000
+NSPOS	9	62958000	63009000
+NSPOS	9	63202000	63253000
+NSPOS	9	63492000	63543000
+NSPOS	9	63918000	63969000
+NSPOS	9	64135000	64186000
+NSPOS	9	64215000	64316000
+NSPOS	9	64998000	65049000
+NSPOS	9	65080000	65131000
+NSPOS	9	65325000	65376000
+NSPOS	9	65595000	65646000
+NSPOS	9	66391000	66592000
+NSPOS	9	67920000	68221000
+NSPOS	9	134183000	134186000
+NSPOS	10	0	10000
+NSPOS	10	38529000	38574000
+NSPOS	10	38906000	38912000
+NSPOS	10	38913000	38919000
+NSPOS	10	39229000	39231000
+NSPOS	10	39238000	39240000
+NSPOS	10	39254000	39255000
+NSPOS	10	39338000	39339000
+NSPOS	10	39341000	39342000
+NSPOS	10	39409000	39411000
+NSPOS	10	39479000	39480000
+NSPOS	10	39497000	39498000
+NSPOS	10	39570000	39571000
+NSPOS	10	39585000	39591000
+NSPOS	10	39593000	39598000
+NSPOS	10	39598000	39599000
+NSPOS	10	39602000	39607000
+NSPOS	10	39607000	39608000
+NSPOS	10	39613000	39616000
+NSPOS	10	39617000	39618000
+NSPOS	10	39622000	39626000
+NSPOS	10	39635000	39636000
+NSPOS	10	39636000	39687000
+NSPOS	10	39935000	39936000
+NSPOS	10	40493000	40494000
+NSPOS	10	40583000	40584000
+NSPOS	10	40722000	40723000
+NSPOS	10	40927000	40929000
+NSPOS	10	41497000	41498000
+NSPOS	10	41545000	41546000
+NSPOS	10	41593000	41694000
+NSPOS	10	41916000	42067000
+NSPOS	10	47780000	47871000
+NSPOS	10	124121000	124122000
+NSPOS	10	131597000	131598000
+NSPOS	10	133690000	133741000
+NSPOS	11	0	60000
+NSPOS	11	50821000	51079000
+NSPOS	11	51090000	51091000
+NSPOS	11	51120000	51121000
+NSPOS	11	51622000	51623000
+NSPOS	11	51945000	51946000
+NSPOS	11	52128000	52129000
+NSPOS	11	52368000	52370000
+NSPOS	11	53216000	53217000
+NSPOS	11	53531000	53532000
+NSPOS	11	53986000	53987000
+NSPOS	11	54342000	54343000
+NSPOS	11	54425000	54526000
+NSPOS	11	70955000	71056000
+NSPOS	11	87978000	88003000
+NSPOS	11	96566000	96567000
+NSPOS	12	0	10000
+NSPOS	12	7083000	7085000
+NSPOS	12	34719000	34770000
+NSPOS	12	34798000	34799000
+NSPOS	12	34816000	34817000
+NSPOS	12	34820000	34821000
+NSPOS	12	34822000	34830000
+NSPOS	12	34832000	34833000
+NSPOS	12	34835000	34836000
+NSPOS	12	34849000	34850000
+NSPOS	12	36673000	36674000
+NSPOS	12	36779000	36780000
+NSPOS	12	36797000	36798000
+NSPOS	12	36966000	36967000
+NSPOS	12	37185000	37236000
+NSPOS	12	37240000	37246000
+NSPOS	12	37255000	37258000
+NSPOS	12	37333000	37334000
+NSPOS	12	37334000	37335000
+NSPOS	12	37379000	37381000
+NSPOS	12	37460000	37461000
+NSPOS	12	123443000	123444000
+NSPOS	12	123476000	123477000
+NSPOS	12	132223000	132225000
+NSPOS	13	0	16000000
+NSPOS	13	16022000	16023000
+NSPOS	13	16110000	16111000
+NSPOS	13	16164000	16165000
+NSPOS	13	16228000	16229000
+NSPOS	13	16249000	16250000
+NSPOS	13	16256000	16257000
+NSPOS	13	16259000	16260000
+NSPOS	13	16282000	16283000
+NSPOS	13	17416000	17417000
+NSPOS	13	17416000	17417000
+NSPOS	13	17417000	17418000
+NSPOS	13	17418000	17419000
+NSPOS	13	18051000	18172000
+NSPOS	13	18358000	18409000
+NSPOS	13	86202000	86253000
+NSPOS	13	111703000	111754000
+NSPOS	13	111793000	111844000
+NSPOS	13	113673000	113724000
+NSPOS	14	0	16023000
+NSPOS	14	16053000	16055000
+NSPOS	14	16061000	16062000
+NSPOS	14	16086000	16090000
+NSPOS	14	16096000	16097000
+NSPOS	14	16105000	16114000
+NSPOS	14	16130000	16134000
+NSPOS	14	16140000	16401000
+NSPOS	14	16404000	18224000
+NSPOS	14	18712000	18863000
+NSPOS	14	19511000	19612000
+NSPOS	15	0	17000000
+NSPOS	15	17049000	17050000
+NSPOS	15	17076000	17077000
+NSPOS	15	17083000	17084000
+NSPOS	15	17498000	17500000
+NSPOS	15	17751000	17752000
+NSPOS	15	18341000	18342000
+NSPOS	15	18355000	18356000
+NSPOS	15	18979000	18980000
+NSPOS	15	19725000	19776000
+NSPOS	15	20689000	20730000
+NSPOS	15	21193000	21243000
+NSPOS	15	21778000	21829000
+NSPOS	15	22308000	22359000
+NSPOS	15	23226000	23277000
+NSPOS	15	84270000	84321000
+NSPOS	16	0	10000
+NSPOS	16	18436000	18487000
+NSPOS	16	33214000	33265000
+NSPOS	16	33392000	33443000
+NSPOS	16	34289000	34340000
+NSPOS	16	34521000	34572000
+NSPOS	16	34576000	34581000
+NSPOS	16	34584000	34585000
+NSPOS	16	36260000	36261000
+NSPOS	16	36261000	36312000
+NSPOS	16	36314000	36315000
+NSPOS	16	36334000	36335000
+NSPOS	16	36337000	36338000
+NSPOS	16	36669000	36670000
+NSPOS	16	37462000	37463000
+NSPOS	16	37946000	37947000
+NSPOS	16	37956000	37957000
+NSPOS	16	38265000	38266000
+NSPOS	16	38269000	38276000
+NSPOS	16	38280000	46381000
+NSPOS	17	0	60000
+NSPOS	17	448000	489000
+NSPOS	17	490000	492000
+NSPOS	17	21795000	21815000
+NSPOS	17	21860000	21861000
+NSPOS	17	21976000	21977000
+NSPOS	17	21983000	21984000
+NSPOS	17	21984000	21986000
+NSPOS	17	21992000	22043000
+NSPOS	17	22089000	22090000
+NSPOS	17	22763000	22814000
+NSPOS	17	23194000	23196000
+NSPOS	17	25684000	25685000
+NSPOS	17	25735000	25737000
+NSPOS	17	25919000	25921000
+NSPOS	17	26566000	26567000
+NSPOS	17	26569000	26571000
+NSPOS	17	26592000	26593000
+NSPOS	17	26616000	26617000
+NSPOS	17	26627000	26628000
+NSPOS	17	26638000	26639000
+NSPOS	17	26640000	26641000
+NSPOS	17	26643000	26644000
+NSPOS	17	26698000	26699000
+NSPOS	17	26720000	26722000
+NSPOS	17	26735000	26736000
+NSPOS	17	26805000	26806000
+NSPOS	17	26820000	26821000
+NSPOS	17	26859000	26861000
+NSPOS	17	26876000	26877000
+NSPOS	17	26880000	26881000
+NSPOS	17	26885000	26936000
+NSPOS	17	81742000	81793000
+NSPOS	17	81796000	81798000
+NSPOS	17	81798000	81800000
+NSPOS	18	0	10000
+NSPOS	18	15410000	15461000
+NSPOS	18	15535000	15536000
+NSPOS	18	15780000	15781000
+NSPOS	18	15788000	15792000
+NSPOS	18	15797000	15798000
+NSPOS	18	15914000	15915000
+NSPOS	18	16246000	16247000
+NSPOS	18	16431000	16432000
+NSPOS	18	16431000	16432000
+NSPOS	18	16769000	16770000
+NSPOS	18	16770000	16771000
+NSPOS	18	16770000	16771000
+NSPOS	18	16876000	16877000
+NSPOS	18	18504000	18505000
+NSPOS	18	19182000	19184000
+NSPOS	18	19347000	19348000
+NSPOS	18	20561000	20562000
+NSPOS	18	20564000	20572000
+NSPOS	18	20582000	20583000
+NSPOS	18	20603000	20604000
+NSPOS	18	20625000	20626000
+NSPOS	18	20641000	20642000
+NSPOS	18	20652000	20653000
+NSPOS	18	20687000	20688000
+NSPOS	18	20696000	20697000
+NSPOS	18	20736000	20737000
+NSPOS	18	20747000	20748000
+NSPOS	18	20751000	20752000
+NSPOS	18	20813000	20814000
+NSPOS	18	20830000	20832000
+NSPOS	18	20835000	20836000
+NSPOS	18	20839000	20840000
+NSPOS	18	20850000	20851000
+NSPOS	18	20861000	20912000
+NSPOS	18	46969000	47020000
+NSPOS	18	54536000	54538000
+NSPOS	18	80255000	80256000
+NSPOS	19	0	60000
+NSPOS	19	24448000	24892000
+NSPOS	19	24895000	24896000
+NSPOS	19	24898000	24905000
+NSPOS	19	24908000	27241000
+NSPOS	20	0	60000
+NSPOS	20	63000	64000
+NSPOS	20	66000	67000
+NSPOS	20	26348000	26349000
+NSPOS	20	26364000	26366000
+NSPOS	20	26382000	26383000
+NSPOS	20	26386000	26437000
+NSPOS	20	26442000	26443000
+NSPOS	20	26586000	26588000
+NSPOS	20	26590000	26597000
+NSPOS	20	26608000	26609000
+NSPOS	20	26634000	26635000
+NSPOS	20	26646000	26647000
+NSPOS	20	27295000	27296000
+NSPOS	20	27504000	27505000
+NSPOS	20	27518000	27519000
+NSPOS	20	27871000	27872000
+NSPOS	20	28180000	28181000
+NSPOS	20	28256000	28257000
+NSPOS	20	28317000	28318000
+NSPOS	20	28445000	28447000
+NSPOS	20	28494000	28495000
+NSPOS	20	28499000	28505000
+NSPOS	20	28508000	28509000
+NSPOS	20	28556000	28558000
+NSPOS	20	28646000	28647000
+NSPOS	20	28648000	28649000
+NSPOS	20	28650000	28651000
+NSPOS	20	28652000	28653000
+NSPOS	20	28654000	28655000
+NSPOS	20	28681000	28682000
+NSPOS	20	28688000	28689000
+NSPOS	20	28696000	28697000
+NSPOS	20	28697000	28698000
+NSPOS	20	28719000	28720000
+NSPOS	20	28728000	28729000
+NSPOS	20	28751000	28753000
+NSPOS	20	28754000	28755000
+NSPOS	20	28757000	28758000
+NSPOS	20	28790000	28791000
+NSPOS	20	28820000	28821000
+NSPOS	20	28843000	28860000
+NSPOS	20	28861000	28862000
+NSPOS	20	28867000	28869000
+NSPOS	20	28875000	28876000
+NSPOS	20	28889000	28890000
+NSPOS	20	28890000	28897000
+NSPOS	20	29125000	29126000
+NSPOS	20	29129000	29130000
+NSPOS	20	29140000	29141000
+NSPOS	20	29165000	29166000
+NSPOS	20	29204000	29205000
+NSPOS	20	29271000	29272000
+NSPOS	20	29307000	29308000
+NSPOS	20	29315000	29316000
+NSPOS	20	29362000	29363000
+NSPOS	20	29412000	29414000
+NSPOS	20	29447000	29448000
+NSPOS	20	29452000	29453000
+NSPOS	20	29538000	29539000
+NSPOS	20	29540000	29541000
+NSPOS	20	29556000	29557000
+NSPOS	20	29562000	29564000
+NSPOS	20	29564000	29566000
+NSPOS	20	29592000	29593000
+NSPOS	20	29651000	29652000
+NSPOS	20	29697000	29698000
+NSPOS	20	29884000	29885000
+NSPOS	20	29917000	29918000
+NSPOS	20	29978000	29979000
+NSPOS	20	30017000	30018000
+NSPOS	20	30030000	30031000
+NSPOS	20	30038000	30089000
+NSPOS	20	30425000	30457000
+NSPOS	20	30761000	30812000
+NSPOS	20	31001000	31052000
+NSPOS	20	31107000	31158000
+NSPOS	20	31159000	31162000
+NSPOS	20	36314000	36315000
+NSPOS	21	0	5010000
+NSPOS	21	5166000	5217000
+NSPOS	21	5393000	5444000
+NSPOS	21	5449000	5500000
+NSPOS	21	5627000	5678000
+NSPOS	21	5796000	5847000
+NSPOS	21	5916000	5967000
+NSPOS	21	6161000	6212000
+NSPOS	21	6377000	6428000
+NSPOS	21	6580000	6631000
+NSPOS	21	6739000	6790000
+NSPOS	21	6934000	6985000
+NSPOS	21	7149000	7200000
+NSPOS	21	7327000	7378000
+NSPOS	21	7500000	7551000
+NSPOS	21	7693000	7744000
+NSPOS	21	7865000	7916000
+NSPOS	21	8049000	8100000
+NSPOS	21	8260000	8311000
+NSPOS	21	8472000	8523000
+NSPOS	21	8706000	8757000
+NSPOS	21	8886000	8987000
+NSPOS	21	9196000	9247000
+NSPOS	21	9377000	9528000
+NSPOS	21	10169000	10270000
+NSPOS	21	10274000	10325000
+NSPOS	21	10814000	12966000
+NSPOS	21	31784000	31785000
+NSPOS	21	31785000	31786000
+NSPOS	21	38914000	38915000
+NSPOS	21	41584000	41585000
+NSPOS	21	42615000	42616000
+NSPOS	21	43212000	43263000
+NSPOS	21	43468000	43469000
+NSPOS	22	0	10510000
+NSPOS	22	10784000	10835000
+NSPOS	22	10874000	10925000
+NSPOS	22	10966000	11017000
+NSPOS	22	11068000	11119000
+NSPOS	22	11160000	11211000
+NSPOS	22	11378000	11429000
+NSPOS	22	11497000	11548000
+NSPOS	22	11631000	11682000
+NSPOS	22	11724000	11775000
+NSPOS	22	11977000	12028000
+NSPOS	22	12225000	12276000
+NSPOS	22	12438000	12489000
+NSPOS	22	12641000	12692000
+NSPOS	22	12726000	12777000
+NSPOS	22	12818000	12869000
+NSPOS	22	12904000	15155000
+NSPOS	22	16279000	16303000
+NSPOS	22	16304000	16306000
+NSPOS	22	16307000	16308000
+NSPOS	22	16310000	16311000
+NSPOS	22	16313000	16315000
+NSPOS	22	18239000	18340000
+NSPOS	22	18433000	18484000
+NSPOS	22	18659000	18710000
+NSPOS	22	49973000	49976000
+NSPOS	X	0	10000
+NSPOS	X	44000	95000
+NSPOS	X	133000	223000
+NSPOS	X	226000	227000
+NSPOS	X	1949000	2133000
+NSPOS	X	2137000	2138000
+NSPOS	X	37099000	37286000
+NSPOS	X	49348000	49529000
+NSPOS	X	50228000	50279000
+NSPOS	X	58555000	58606000
+NSPOS	X	58736000	58737000
+NSPOS	X	58804000	58805000
+NSPOS	X	58988000	58989000
+NSPOS	X	59064000	59065000
+NSPOS	X	59477000	59478000
+NSPOS	X	59487000	59488000
+NSPOS	X	59532000	59534000
+NSPOS	X	60550000	60551000
+NSPOS	X	61173000	61174000
+NSPOS	X	61212000	61213000
+NSPOS	X	62068000	62069000
+NSPOS	X	62107000	62108000
+NSPOS	X	62412000	62463000
+NSPOS	X	114281000	114332000
+NSPOS	X	115738000	115839000
+NSPOS	X	116557000	116596000
+NSPOS	X	120879000	120930000
+NSPOS	X	144425000	144476000
+NSPOS	Y	0	2782000
+NSPOS	Y	9046000	9056000
+NSPOS	Y	9057000	9108000
+NSPOS	Y	9111000	9113000
+NSPOS	Y	9114000	9117000
+NSPOS	Y	9403000	9454000
+NSPOS	Y	10266000	10317000
+NSPOS	Y	10544000	10595000
+NSPOS	Y	10633000	10646000
+NSPOS	Y	10649000	10652000
+NSPOS	Y	10669000	10671000
+NSPOS	Y	10674000	10677000
+NSPOS	Y	10679000	10683000
+NSPOS	Y	10691000	10692000
+NSPOS	Y	10694000	10745000
+NSPOS	Y	10747000	10748000
+NSPOS	Y	10809000	10811000
+NSPOS	Y	10816000	10818000
+NSPOS	Y	10852000	10856000
+NSPOS	Y	10871000	10872000
+NSPOS	Y	10890000	10892000
+NSPOS	Y	10896000	10899000
+NSPOS	Y	10908000	10910000
+NSPOS	Y	10922000	10924000
+NSPOS	Y	10956000	10958000
+NSPOS	Y	10961000	10963000
+NSPOS	Y	10965000	10968000
+NSPOS	Y	10969000	10971000
+NSPOS	Y	10986000	10987000
+NSPOS	Y	11002000	11004000
+NSPOS	Y	11012000	11014000
+NSPOS	Y	11016000	11018000
+NSPOS	Y	11023000	11025000
+NSPOS	Y	11028000	11030000
+NSPOS	Y	11036000	11038000
+NSPOS	Y	11592000	11643000
+NSPOS	Y	11647000	11648000
+NSPOS	Y	11653000	11654000
+NSPOS	Y	11660000	11663000
+NSPOS	Y	11663000	11665000
+NSPOS	Y	11669000	11671000
+NSPOS	Y	11671000	11672000
+NSPOS	Y	11673000	11675000
+NSPOS	Y	20207000	20258000
+NSPOS	Y	21739000	21742000
+NSPOS	Y	21747000	21749000
+NSPOS	Y	21750000	21751000
+NSPOS	Y	21789000	21806000
+NSPOS	Y	26673000	56674000
+NSPOS	Y	56771000	56822000
+NSPOS	16_KI270728v1_random	40000	91000
+NSPOS	16_KI270728v1_random	247000	298000
+NSPOS	16_KI270728v1_random	446000	497000
+NSPOS	16_KI270728v1_random	680000	731000
+NSPOS	16_KI270728v1_random	1367000	1418000
+NSPOS	16_KI270728v1_random	1625000	1676000
+NSPOS	17_KI270729v1_random	6000	11000
+NSPOS	17_KI270729v1_random	13000	21000
+NSPOS	17_KI270729v1_random	51000	52000
+NSPOS	17_KI270729v1_random	54000	55000
+NSPOS	17_KI270729v1_random	57000	58000
+NSPOS	17_KI270729v1_random	102000	103000
+NSPOS	17_KI270729v1_random	158000	159000
+NSPOS	17_KI270729v1_random	234000	235000
+NSPOS	17_KI270730v1_random	88000	91000
+NSPOS	17_KI270730v1_random	91000	92000
+NSPOS	17_KI270730v1_random	93000	96000
+NSPOS	17_KI270730v1_random	100000	102000
+NSPOS	17_KI270730v1_random	107000	108000
+NSPOS	17_KI270730v1_random	109000	110000
+NSPOS	22_KI270736v1_random	57000	59000
+NSPOS	22_KI270736v1_random	116000	117000
+NSPOS	22_KI270736v1_random	156000	157000
+NSPOS	22_KI270736v1_random	158000	162000
+NSPOS	22_KI270736v1_random	163000	167000
+NSPOS	22_KI270736v1_random	167000	171000
+NSPOS	22_KI270736v1_random	175000	180000
+NSPOS	22_KI270737v1_random	81000	82000
+NSPOS	22_KI270738v1_random	5000	7000
+NSPOS	22_KI270738v1_random	68000	69000
+NSPOS	22_KI270738v1_random	79000	80000
+NSPOS	22_KI270738v1_random	86000	87000
+NSPOS	22_KI270738v1_random	87000	88000
+NSPOS	22_KI270738v1_random	91000	94000
+NSPOS	22_KI270738v1_random	95000	96000
+NSPOS	22_KI270739v1_random	13000	15000
+NSPOS	22_KI270739v1_random	37000	39000
+NSPOS	22_KI270739v1_random	41000	42000
+NSPOS	Un_KI270322v1	2000	9000
+NSPOS	Un_KI270322v1	10000	20000
+NSPOS	Un_KI270311v1	1000	11000
+NSPOS	Un_KI270317v1	1000	37000
+NSPOS	Un_KI270442v1	3000	4000
+NSPOS	Un_KI270442v1	4000	10000
+NSPOS	Un_KI270442v1	11000	12000
+NSPOS	Un_KI270442v1	20000	23000
+NSPOS	Un_KI270442v1	51000	56000
+NSPOS	Un_KI270442v1	63000	68000
+NSPOS	Un_KI270442v1	72000	75000
+NSPOS	Un_KI270442v1	87000	88000
+NSPOS	Un_KI270442v1	100000	101000
+NSPOS	Un_KI270442v1	162000	164000
+NSPOS	Un_KI270442v1	175000	176000
+NSPOS	Un_KI270442v1	227000	229000
+NSPOS	Un_KI270442v1	333000	336000
+NSPOS	Un_KI270442v1	374000	375000
+NSPOS	Un_KI270442v1	384000	385000
+NSPOS	Un_KI270442v1	390000	391000
+NSPOS	Un_KI270435v1	48000	49000
+NSPOS	Un_KI270435v1	57000	58000
+NSPOS	Un_KI270435v1	84000	85000
+NSPOS	Un_KI270438v1	14000	20000
+NSPOS	Un_KI270438v1	23000	29000
+NSPOS	Un_KI270438v1	32000	44000
+NSPOS	Un_KI270438v1	49000	57000
+NSPOS	Un_KI270438v1	62000	64000
+NSPOS	Un_KI270438v1	64000	65000
+NSPOS	Un_KI270519v1	63000	64000
+NSPOS	Un_KI270519v1	97000	98000
+NSPOS	Un_KI270519v1	120000	121000
+NSPOS	Un_KI270519v1	123000	124000
+NSPOS	Un_KI270538v1	4000	15000
+NSPOS	Un_KI270538v1	34000	39000
+NSPOS	Un_KI270538v1	43000	54000
+NSPOS	Un_KI270538v1	60000	61000
+NSPOS	Un_KI270538v1	81000	84000
+NSPOS	Un_KI270538v1	84000	87000
+NSPOS	Un_KI270589v1	6000	10000
+NSPOS	Un_KI270589v1	25000	28000
+NSPOS	Un_KI270589v1	35000	38000
+NSPOS	Un_KI270589v1	39000	42000
+NSPOS	Un_KI270741v1	66000	67000
+NSPOS	Un_KI270741v1	103000	105000
+NSPOS	Un_KI270741v1	110000	111000
+NSPOS	Un_KI270741v1	118000	119000
+NSPOS	Un_KI270741v1	126000	127000
+NSPOS	Un_KI270741v1	127000	129000
+NSPOS	Un_KI270756v1	11000	12000
+NSPOS	Un_KI270757v1	10000	15000
+NSPOS	Un_KI270757v1	16000	21000
+NSPOS	Un_KI270757v1	44000	47000
+NSPOS	Un_GL000216v2	1000	2000
```

### Comparing `ont-spectre-0.2.0/spectre/main.py` & `ont_spectre-0.2.1/spectre/main.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import argparse
 import logging as logger
 from multiprocessing import Pool
 import os
 import sys
+import pkg_resources
 
 import pysam
 
 from spectre import spectreCNV, spectreCNVPopulation, __version__
 from spectre.util.metadata.metadataCollector import FastaRef
 
 
@@ -153,51 +154,62 @@
                        "chr_lengths_by_name": {}}
         for chr_name, chr_len in zip(genome_info_pysam.references, genome_info_pysam.lengths):
             genome_info["chr_lengths_by_name"][chr_name] = chr_len
         return genome_info
 
     def meta_data_extraction(self):
         # ----------- Metadata extraction from ref file  -----------
-        # self.metadata_args.as_dev  # Note: this is not used
         reference_fas = self.metadata_args.reference
         bin_size = self.metadata_args.bin_size
         output_dir = os.path.abspath(os.path.expanduser(self.metadata_args.out_dir))
         threshold = self.metadata_args.n_size
         # if "call_from_console" then the meta_data_report serves as output only, otherwise as both
         meta_data_report = self.metadata_args.metadata if not self.metadata_args.call_from_console \
             else f'{output_dir}/{self.metadata_args.metadata}'
         default_metadata_name = f'{output_dir}/metadata.mdr'  # default
         save_only = self.metadata_args.save_only
         fasta_metadata = FastaRef()
         blacklist_data_bed = self.metadata_args.black_list  # bed format
         self.logger.info("Extraction of metadata is activated")
 
-        # metadata parameter given?
         if meta_data_report != "":
-            meta_data_report = os.path.abspath(os.path.expanduser(meta_data_report))
+            metadata_resource_path = 'data/' + meta_data_report + '.mdr'
+            if pkg_resources.resource_exists(__name__, metadata_resource_path):
+                with pkg_resources.resource_stream(__name__, metadata_resource_path) as meta_data_report_stream:
+                    self.logger.info(f'Extracting metadata from resource: {metadata_resource_path}')
+                    metadata_result = fasta_metadata.extract_n_regions_from_report(meta_data_report_stream)
+            else:
+                path = os.path.abspath(os.path.expanduser(meta_data_report))
+                self.logger.info(f'Extracting metadata from file: {path}')
+                with open(path, 'rb') as f:
+                    metadata_result = fasta_metadata.extract_n_regions_from_report(f)
         else:
-            self.logger.info("Looking for default metadata.mdr")
             meta_data_report = os.path.abspath(os.path.expanduser(default_metadata_name))
-        # metadata file exists
-        if not os.path.exists(meta_data_report):
-            self.logger.info(f'Extracting metadata from {reference_fas}')
+            self.logger.info(f'Generating metadata based on reference: {reference_fas}')
+            self.logger.info(f'Writing metadata to file: {meta_data_report}')
             metadata_result = fasta_metadata.get_n_regions(filepath=reference_fas, report_output_dir=output_dir,
-                                                           out_file_name=meta_data_report, threshold=threshold,
-                                                           bin_size=bin_size, save_only=save_only)
-        else:
-            self.logger.info(f'Extracting metadata from {meta_data_report}')
-            metadata_result = fasta_metadata.extract_n_regions_from_report(meta_data_report)
+                                                            out_file_name=meta_data_report, threshold=threshold,
+                                                            bin_size=bin_size, save_only=save_only)
         if blacklist_data_bed != "":
-            self.logger.debug("Using blacklist")
-            blacklist_results = fasta_metadata.extract_blacklisted_regions(blacklist_data_bed)
+            blacklisr_resource_path = 'data/' + blacklist_data_bed + '.bed'
+            if pkg_resources.resource_exists(__name__, blacklisr_resource_path):
+                with pkg_resources.resource_stream(__name__, blacklisr_resource_path) as blacklist_data_bed_stream:
+                    self.logger.info(f'Using blacklist from resource: {blacklisr_resource_path}')
+                    blacklist_results = fasta_metadata.extract_blacklisted_regions(blacklist_data_bed_stream)
+            else:
+                self.logger.info(f'Extracting blacklist from {blacklist_data_bed}')
+                path = os.path.abspath(os.path.expanduser(blacklist_data_bed))
+                with open(path, 'rb') as f:
+                    blacklist_results = fasta_metadata.extract_blacklisted_regions(f)
             metadata_result = fasta_metadata.merge_metadata(metadata_result, blacklist_results)
-        # return metadata object (dict) after writing to file?
-        if save_only:
-            pass
         else:
+            self.logger.info('No blacklist was provided')
+
+        # return metadata object (dict) after writing to file?
+        if not save_only:
             self.logger.debug("returned meta Object")
             return metadata_result
 
     def __set_genome_info(self, reference):
         pysam_genome = pysam.FastaFile(reference)
         self.genome = self.make_genome_info(pysam_genome)
         pysam_genome.close()
@@ -310,25 +322,27 @@
                 --bin-size     Bin/Window size (same as Mosdepth)
                 --coverage     Coverage directory from Mosdepth output. Expects the following files:
                                    <prefix>.mosdepth.summary.txt
                                    <prefix>.regions.bed.gz
                                    <prefix>.regions.bed.gz.csi
                                Can be one or more directories. Example:
                                     --coverage /path/dir1/ /path/dir2/
+                --snv          VCF file containing the SNV for the same sample CNV want to be called
                 --sample-id    Sample name/ID. Can be one or more ID. Example:
                                     --sample-id id1 id2
                 --output-dir   Output directory
                 --reference    Reference sequence used for mapping (for N removal)
             Optional, if missing it will be created
-                --metadata     Metadata file for Ns removal
+                --metadata     Metadata file for Ns removal or label of available file in package resources: grch38_metadata
             Optional
-                --blacklist    Blacklist in bed format for sites that will be ignored (Default = "")
+                --blacklist    Blacklist in bed format for sites that will be ignored
+                               or label of available blackslists in package resorces: grch38_blacklist_0.3
+                               (Default = "")
                 --only-chr     Comma separated list of chromosomes to use
                 --ploidy       Set the ploidy for the analysis, useful for sex chromosomes (Default = 2)
-                --snv          VCF file containing the SNV for the same sample CNV want to be called
                 --n-size       Length of consecutive Ns (Default = 5)
                 --min_cnv_len  Minimum length of CNV (Default 1mb)
                 --population   Runs the population mode on all provided samples
                 --threads      Amount of threads (This will boost performance if multiple samples are provided)
 
 
         removeNs:
@@ -366,41 +380,41 @@
     subparser_version.add_argument('-0', '--0', action='store_true', required=False, dest='_0', default=False, help='')
 
     # ############################################################################################ #
     # CNV caller
     cnv_caller_help = "..."
     subparser_cnv_caller = subparsers.add_parser("CNVCaller", help=cnv_caller_help)
     # Required
-    subparser_cnv_caller.add_argument('-b', '--bin-size', type=int, required=True, dest='bin_size', default=500,
+    subparser_cnv_caller.add_argument('-b', '--bin-size', type=int, required=True, dest='bin_size', default=1000,
                                       help='..., default = 1kb')
     subparser_cnv_caller.add_argument('-c', '--coverage', type=str, required=True, dest='coverage_dir', default="",
                                       help='..., default = None', nargs='+')
     subparser_cnv_caller.add_argument('-s', '--sample-id', type=str, required=True, dest='sample_id', default="",
                                       help='..., default = None', nargs='+')
     subparser_cnv_caller.add_argument('-d', '--output-dir', type=str, required=True, dest='output_dir', default=".",
                                       help='..., default = None')
     subparser_cnv_caller.add_argument('-r', '--reference', type=str, required=True, dest='reference', default="",
                                       help='..., default = None')
+    subparser_cnv_caller.add_argument('-v', '--snv', type=str, required=True, dest='snv_file', default="",
+                                      help='...')
     # Optional, if missing will be created
     subparser_cnv_caller.add_argument('-m', '--metadata', type=str, required=False, dest='metadata', default="",
                                       help='..., default = None')
     # Optional
-    subparser_cnv_caller.add_argument('-v', '--snv', type=str, required=False, dest='snv_file', default="",
-                                      help='...')
     subparser_cnv_caller.add_argument('-l', '--blacklist', type=str, required=False, dest='black_list_file',
                                       default="",
                                       help='...')
     subparser_cnv_caller.add_argument('-o', '--only-chr', type=str, required=False, dest='only_chr_list', default="",
                                       help='...')
     subparser_cnv_caller.add_argument('-p', '--ploidy', type=int, required=False, dest='ploidy', default=2,
                                       help='..., default = 2')
     subparser_cnv_caller.add_argument('-n', '--n-size', type=int, required=False, dest='n_size', default=5,
                                       help='..., default = 5')
-    subparser_cnv_caller.add_argument('-mcl', '--min-cnv-len', type=int, required=False, dest='min_cnv_len', default=1000000,
-                                      help='..., default = 1000000')
+    subparser_cnv_caller.add_argument('-mcl', '--min-cnv-len', type=int, required=False, dest='min_cnv_len', default=80000,
+                                      help='..., default = 80000')
     subparser_cnv_caller.add_argument('-t', '--threads', type=int, required=False, dest='threads', default=1,
                                       help='..., default = 1')
     subparser_cnv_caller.add_argument('-i', '--population', action='store_true', required=False,
                                       dest='run_population_mode', default=False, help='...s, default = False')
 
     # Dev
     subparser_cnv_caller.add_argument('-0', '--dev', action='store_true', required=False, dest='as_dev', default=False,
@@ -412,21 +426,21 @@
     subparser_cnv_caller.add_argument('-03', '--lower-2n-threshold', type=float, required=False,
                                       dest='lower_2n_threshold', default=1.5, help='..., default = 2.5')
     subparser_cnv_caller.add_argument('-04', '--upper-2n-threshold', type=float, required=False,
                                       dest='upper_2n_threshold', default=2.5, help='..., default = 2.5')
     subparser_cnv_caller.add_argument('-05', '--cov-diff-threshold', type=float, required=False,
                                       dest='cov_diff_threshold', default=0.80, help='..., default = 0.80')
     subparser_cnv_caller.add_argument('-06', '--dist-proportion', type=float, required=False, dest='dist_proportion',
-                                      default=0.25, help='..., default = 0.25')
+                                      default=0.3, help='..., default = 0.3')
     subparser_cnv_caller.add_argument('-07', '--candidate-final-threshold', type=int, required=False,
                                       dest='candidate_final_threshold', default=100000,
                                       help='..., default = 100,000')  # 100kb
     subparser_cnv_caller.add_argument('-08', '--threshhold-quantile', type=float, required=False,
-                                      dest='threshhold_quantile', default=5,
-                                      help='..., default = 5')
+                                      dest='threshhold_quantile', default=10,
+                                      help='..., default = 10')
 
     # ############################################################################################ #
     # Metadata to remove Ns
     metadata_help = "..."
     subparser_metadata = subparsers.add_parser("removeNs", help=metadata_help)
     # Required
     subparser_metadata.add_argument('-r', '--reference', type=str, required=True, dest='reference', default="",
```

### Comparing `ont-spectre-0.2.0/spectre/plots/plot.py` & `ont_spectre-0.2.1/spectre/plots/plot.py`

 * *Files identical despite different names*

### Comparing `ont-spectre-0.2.0/spectre/spectreCNV.py` & `ont_spectre-0.2.1/spectre/spectreCNV.py`

 * *Files identical despite different names*

### Comparing `ont-spectre-0.2.0/spectre/spectreCNVPopulation.py` & `ont_spectre-0.2.1/spectre/spectreCNVPopulation.py`

 * *Files identical despite different names*

### Comparing `ont-spectre-0.2.0/spectre/util/OSUtil.py` & `ont_spectre-0.2.1/spectre/util/OSUtil.py`

 * *Files identical despite different names*

### Comparing `ont-spectre-0.2.0/spectre/util/cnv_id.py` & `ont_spectre-0.2.1/spectre/util/cnv_id.py`

 * *Files identical despite different names*

### Comparing `ont-spectre-0.2.0/spectre/util/dataAnalyzer.py` & `ont_spectre-0.2.1/spectre/util/dataAnalyzer.py`

 * *Files identical despite different names*

### Comparing `ont-spectre-0.2.0/spectre/util/metadata/metadataCollector.py` & `ont_spectre-0.2.1/spectre/util/metadata/metadataCollector.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 import gzip
 import logging as logger
-import mmap
 import os
 
 
 class FastaRef:
 
     def __init__(self, as_dev=False):
         # logger
@@ -109,51 +108,48 @@
                 self.static_report += "NSPOS\t" + str(chromosome) + "\t" + str(start) + "\t" + str(end) + "\n"
 
         # write statistic report to file
         self.logger.info("Writing report")
         self.__write_report(output_dir, filename)
 
     @classmethod
-    def extract_n_regions_from_report(cls, input_file: str) -> dict:
+    def extract_n_regions_from_report(cls, input_stream) -> dict:
         """
         Loads all N regions that previously have been extracted from the reference genome and stored in a .mdr file
-        :param input_file: /path/to/<file_name>.mdr
+        :param input_stream: A file-like object containing the data in binary format
         :return: dict with all N regions according to the chromosome
         """
         result = dict()
-        # assure abs paths
-        path = os.path.abspath(os.path.expanduser(input_file))
-        with open(path, "r") as fp:
-            # map file into memory
-            mm = mmap.mmap(fp.fileno(), 0, prot=mmap.PROT_READ)
-            for line in iter(mm.readline, b""):
-                # decode line and cut away last char from line (\n)
-                term = line.decode("utf-8")[:-1]
-                if term[:5].__eq__("NSPOS"):
-                    cells = term.strip().split("\t")
-                    if str(cells[1]) not in result:  # [1] = chromosome name
-                        result[str(cells[1])] = []
-                    result[str(cells[1])].append((cells[2], cells[3]))  # [2] start, [3] end
+        while line := input_stream.readline():
+            term = line.decode('utf-8').strip()  # decode from bytes to string and strip whitespace
+            if term[:5] == "NSPOS":
+                cells = term.split("\t")
+                chromosome = cells[1]
+                if chromosome not in result:
+                    result[chromosome] = []
+                result[chromosome].append((cells[2], cells[3]))  # [2] start, [3] end
         return result
 
     @classmethod
-    def extract_blacklisted_regions(cls, input_file: str) -> dict:
+    def extract_blacklisted_regions(cls, input_stream) -> dict:
+        """
+        Extract blacklisted regions from a given input stream.
+        :param input_stream: A file-like object containing the data in binary format.
+        :return: dict with blacklisted regions according to the chromosome.
+        """
         result = dict()
-        path = os.path.abspath(os.path.expanduser(input_file))
-        with open(path, "r") as fp:
-            mm = mmap.mmap(fp.fileno(), 0, prot=mmap.PROT_READ)
-            for line in iter(mm.readline, b""):
-                # decode line and cut away last char from line (\n)
-                term = line.decode("utf-8")[:-1]
-                chrom, start, end = term.split("\t")[:3]
-                if str(chrom) not in result:
-                    result[str(chrom)] = []
-                result[str(chrom)].append((start,end))
+        while line := input_stream.readline():
+            term = line.decode('utf-8').strip()  # Ensure line is decoded from bytes to str before splitting
+            chrom, start, end = term.split("\t")[:3]
+            if chrom not in result:
+                result[chrom] = []
+            result[chrom].append((start, end))
         return result
 
+
     @classmethod
     def merge_metadata(cls, m1:dict, m2:dict)->dict:
         """
         Merges two dictionaries with the structure str:list
         :param m1: dict m1 with structure str:list
         :param m2: dict m2 with structure str:list
         :return: merged dict with structure str:list
```

### Comparing `ont-spectre-0.2.0/spectre/util/mosdepthReader.py` & `ont_spectre-0.2.1/spectre/util/mosdepthReader.py`

 * *Files identical despite different names*

### Comparing `ont-spectre-0.2.0/spectre/util/outputWriter.py` & `ont_spectre-0.2.1/spectre/util/outputWriter.py`

 * *Files 2% similar despite different names*

```diff
@@ -30,15 +30,15 @@
         self.POS = 0
         self.ID = "."
         self.REF = "N"
         self.ALT = "."  # DEL/DUP
         self.QUAL = "."
         self.FILTER = "."
         self.INFO = "."
-        self.FORMAT = "GT:HO:GQ"
+        self.FORMAT = "GT:HO:GQ:CN"
         self.format_data = []
         self.sample_format_data = {}
         self.supp_vec = {}
 
     def format_vcf_line(self):
         sample_format_list = []
         if len(self.format_data) > 0:
@@ -92,14 +92,15 @@
         if population_mode:
             vcf_header += ['##INFO=<ID=SUPP_VEC,Number=1,Type=String,Description="Support vector">']
 
         # Add Format section
         vcf_header += ['##FORMAT=<ID=GT,Number=1,Type=String,Description="Genotype">',
                        '##FORMAT=<ID=HO,Number=2,Type=Float,Description="Homozygosity proportion">',
                        '##FORMAT=<ID=GQ,Number=1,Type=Integer,Description="Genotype quality">',
+                       '##FORMAT=<ID=CN,Number=1,Type=Integer,Description="Estimated copy number status">',
                        '##FORMAT=<ID=ID,Number=1,Type=String,Description="Population ID of supporting CNV calls">']
 
         if self.population_sample_ids:
             if population_mode:
                 s = f"##Spectre_population_samples={','.join(self.population_sample_ids)}"
             else:
                 s = f"##Spectre_sample={','.join(self.population_sample_ids)}"
@@ -132,15 +133,16 @@
                 vcf_line.INFO = f"END={each_candidate.end};SVLEN={each_candidate.size};SVTYPE={each_candidate.type};" \
                                 f"CN={each_candidate.cn_status}"
                 # checking if any other CNV through merging supported the given CNV
                 vcf_line.supp_vec = self.supp_vec.copy()
                 if not each_candidate.support_cnv_calls:
 
                     vcf_line.format_data = [each_candidate.gt, f'{round(each_candidate.het_score, 2)}',
-                                            f"{int(each_candidate.statistics['z-score']['sample_score'])}"]
+                                            f"{int(each_candidate.statistics['z-score']['sample_score'])}",
+                                            str(each_candidate.cn_status)]
                 else:
                     vcf_line.format_data = []
                     vcf_line.FORMAT += ":ID"  # ADD ID tag in format as everything that is following are IDs
                     vcf_line.supp_vec = dict(
                         [(str(sample_key), 0) for sample_key in each_candidate.support_cnv_calls.keys()])
                     for sample_key, sample_value in each_candidate.support_cnv_calls.items():
                         if sample_value:
```

### Comparing `ont-spectre-0.2.0/spectre/util/vcf_parser.py` & `ont_spectre-0.2.1/spectre/util/vcf_parser.py`

 * *Files identical despite different names*

### Comparing `ont-spectre-0.2.0/spectre-license.md` & `ont_spectre-0.2.1/spectre-license.md`

 * *Files identical despite different names*

