# Comparing `tmp/monsda-1.2.6.tar.gz` & `tmp/monsda-1.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "monsda-1.2.6.tar", last modified: Wed May 22 12:27:33 2024, max compression
+gzip compressed data, was "monsda-1.2.7.tar", last modified: Mon Jun  3 08:00:03 2024, max compression
```

## Comparing `monsda-1.2.6.tar` & `monsda-1.2.7.tar`

### file list

```diff
@@ -1,265 +1,265 @@
-drwxr-xr-x   0 fall      (1000) fall      (1000)        0 2024-05-22 12:27:33.704138 monsda-1.2.6/
--rw-r--r--   0 fall      (1000) fall      (1000)    35149 2024-03-04 09:35:20.000000 monsda-1.2.6/LICENSE
--rw-r--r--   0 fall      (1000) fall      (1000)       49 2024-03-04 09:35:20.000000 monsda-1.2.6/MANIFEST.in
-drwxr-xr-x   0 fall      (1000) fall      (1000)        0 2024-05-22 12:27:33.684138 monsda-1.2.6/MONSDA/
--rwxr-xr-x   0 fall      (1000) fall      (1000)    70162 2024-03-25 16:31:46.000000 monsda-1.2.6/MONSDA/Configurator.py
--rw-r--r--   0 fall      (1000) fall      (1000)     5763 2024-03-04 09:35:20.000000 monsda-1.2.6/MONSDA/Deprecated.py
--rwxr-xr-x   0 fall      (1000) fall      (1000)     2581 2024-03-04 09:35:20.000000 monsda-1.2.6/MONSDA/Logger.py
--rw-r--r--   0 fall      (1000) fall      (1000)    37733 2024-03-25 16:31:46.000000 monsda-1.2.6/MONSDA/Params.py
--rwxr-xr-x   0 fall      (1000) fall      (1000)    34812 2024-03-28 08:34:24.000000 monsda-1.2.6/MONSDA/RunMONSDA.py
--rw-r--r--   0 fall      (1000) fall      (1000)    18515 2024-03-25 16:31:46.000000 monsda-1.2.6/MONSDA/Utils.py
--rwxr-xr-x   0 fall      (1000) fall      (1000)   171767 2024-03-25 16:31:46.000000 monsda-1.2.6/MONSDA/Workflows.py
--rw-r--r--   0 fall      (1000) fall      (1000)       73 2024-03-04 09:35:20.000000 monsda-1.2.6/MONSDA/__init__.py
--rw-r--r--   0 fall      (1000) fall      (1000)       32 2024-03-04 09:35:20.000000 monsda-1.2.6/MONSDA/__main__.py
--rw-r--r--   0 fall      (1000) fall      (1000)      497 2024-05-22 12:27:33.704138 monsda-1.2.6/MONSDA/_version.py
-drwxr-xr-x   0 fall      (1000) fall      (1000)        0 2024-05-22 12:27:33.685138 monsda-1.2.6/MONSDA/lib/
--rw-r--r--   0 fall      (1000) fall      (1000)     2357 2024-03-04 09:35:20.000000 monsda-1.2.6/MONSDA/lib/Collection.groovy
-drwxr-xr-x   0 fall      (1000) fall      (1000)        0 2024-05-22 12:27:33.703138 monsda-1.2.6/MONSDA.egg-info/
--rw-r--r--   0 fall      (1000) fall      (1000)    47451 2024-05-22 12:27:33.000000 monsda-1.2.6/MONSDA.egg-info/PKG-INFO
--rw-r--r--   0 fall      (1000) fall      (1000)     6004 2024-05-22 12:27:33.000000 monsda-1.2.6/MONSDA.egg-info/SOURCES.txt
--rw-r--r--   0 fall      (1000) fall      (1000)        1 2024-05-22 12:27:33.000000 monsda-1.2.6/MONSDA.egg-info/dependency_links.txt
--rw-r--r--   0 fall      (1000) fall      (1000)       93 2024-05-22 12:27:33.000000 monsda-1.2.6/MONSDA.egg-info/entry_points.txt
--rw-r--r--   0 fall      (1000) fall      (1000)        1 2024-03-19 14:46:42.000000 monsda-1.2.6/MONSDA.egg-info/not-zip-safe
--rw-r--r--   0 fall      (1000) fall      (1000)       89 2024-05-22 12:27:33.000000 monsda-1.2.6/MONSDA.egg-info/requires.txt
--rw-r--r--   0 fall      (1000) fall      (1000)        7 2024-05-22 12:27:33.000000 monsda-1.2.6/MONSDA.egg-info/top_level.txt
--rw-r--r--   0 fall      (1000) fall      (1000)    47451 2024-05-22 12:27:33.704138 monsda-1.2.6/PKG-INFO
--rw-r--r--   0 fall      (1000) fall      (1000)     6058 2024-03-04 09:43:25.000000 monsda-1.2.6/README.md
-drwxr-xr-x   0 fall      (1000) fall      (1000)        0 2024-05-22 12:27:33.686138 monsda-1.2.6/configs/
--rw-r--r--   0 fall      (1000) fall      (1000)    24464 2024-05-22 12:17:56.000000 monsda-1.2.6/configs/template.json
--rw-r--r--   0 fall      (1000) fall      (1000)    14131 2024-03-04 09:43:25.000000 monsda-1.2.6/configs/template_base_commented.json
--rw-r--r--   0 fall      (1000) fall      (1000)     9007 2024-05-22 12:17:56.000000 monsda-1.2.6/configs/template_clean.json
--rw-r--r--   0 fall      (1000) fall      (1000)    19963 2024-05-22 12:17:56.000000 monsda-1.2.6/configs/tutorial_exhaustive.json
--rw-r--r--   0 fall      (1000) fall      (1000)    13787 2024-05-22 12:17:56.000000 monsda-1.2.6/configs/tutorial_postprocess.json
--rw-r--r--   0 fall      (1000) fall      (1000)     1171 2024-05-22 12:17:56.000000 monsda-1.2.6/configs/tutorial_quick.json
--rw-r--r--   0 fall      (1000) fall      (1000)     8919 2024-05-22 12:17:56.000000 monsda-1.2.6/configs/tutorial_toolmix.json
-drwxr-xr-x   0 fall      (1000) fall      (1000)        0 2024-05-22 12:27:33.689138 monsda-1.2.6/envs/
--rw-r--r--   0 fall      (1000) fall      (1000)     5071 2024-03-04 09:35:20.000000 monsda-1.2.6/envs/LoveSonesonPatro.yaml
--rw-r--r--   0 fall      (1000) fall      (1000)      259 2024-03-04 09:35:20.000000 monsda-1.2.6/envs/base.yaml
--rw-r--r--   0 fall      (1000) fall      (1000)      114 2024-03-04 09:35:20.000000 monsda-1.2.6/envs/bbduk.yaml
--rw-r--r--   0 fall      (1000) fall      (1000)      114 2024-03-04 09:35:20.000000 monsda-1.2.6/envs/bbmap.yaml
--rw-r--r--   0 fall      (1000) fall      (1000)      210 2024-03-04 09:35:20.000000 monsda-1.2.6/envs/bedtools.yaml
--rw-r--r--   0 fall      (1000) fall      (1000)      132 2024-03-04 09:35:20.000000 monsda-1.2.6/envs/bwa.yaml
--rw-r--r--   0 fall      (1000) fall      (1000)      136 2024-03-04 09:35:20.000000 monsda-1.2.6/envs/bwa2.yaml
--rw-r--r--   0 fall      (1000) fall      (1000)      159 2024-03-04 09:35:20.000000 monsda-1.2.6/envs/bwameth.yaml
--rw-r--r--   0 fall      (1000) fall      (1000)      122 2024-03-04 09:35:20.000000 monsda-1.2.6/envs/ciri2.yaml
--rw-r--r--   0 fall      (1000) fall      (1000)      356 2024-03-04 09:35:20.000000 monsda-1.2.6/envs/countreads.yaml
--rw-r--r--   0 fall      (1000) fall      (1000)      359 2024-03-04 09:35:20.000000 monsda-1.2.6/envs/countreads_de.yaml
--rw-r--r--   0 fall      (1000) fall      (1000)      118 2024-03-04 09:35:20.000000 monsda-1.2.6/envs/cutadapt.yaml
--rw-r--r--   0 fall      (1000) fall      (1000)     4345 2024-03-04 09:35:20.000000 monsda-1.2.6/envs/deseq2_DE.yaml
--rw-r--r--   0 fall      (1000) fall      (1000)     3328 2024-03-04 09:35:20.000000 monsda-1.2.6/envs/dexseq_DEU.yaml
--rw-r--r--   0 fall      (1000) fall      (1000)     3200 2024-03-04 09:35:20.000000 monsda-1.2.6/envs/dexseq_DTU.yaml
--rw-r--r--   0 fall      (1000) fall      (1000)      347 2024-03-04 09:35:20.000000 monsda-1.2.6/envs/diego_DAS.yaml
--rw-r--r--   0 fall      (1000) fall      (1000)      120 2024-03-04 09:35:20.000000 monsda-1.2.6/envs/dorado.yaml
--rw-r--r--   0 fall      (1000) fall      (1000)     2948 2024-03-04 09:35:20.000000 monsda-1.2.6/envs/drimseq_DTU.yaml
--rw-r--r--   0 fall      (1000) fall      (1000)     1465 2024-03-04 09:35:20.000000 monsda-1.2.6/envs/edger_DAS.yaml
--rw-r--r--   0 fall      (1000) fall      (1000)     2758 2024-03-04 09:35:20.000000 monsda-1.2.6/envs/edger_DE.yaml
--rw-r--r--   0 fall      (1000) fall      (1000)     1465 2024-03-04 09:35:20.000000 monsda-1.2.6/envs/edger_DEU.yaml
--rw-r--r--   0 fall      (1000) fall      (1000)       91 2024-04-16 12:14:02.000000 monsda-1.2.6/envs/fastqc.yaml
--rw-r--r--   0 fall      (1000) fall      (1000)      290 2024-03-04 09:35:20.000000 monsda-1.2.6/envs/guppy.yaml
--rw-r--r--   0 fall      (1000) fall      (1000)      190 2024-03-04 09:35:20.000000 monsda-1.2.6/envs/hisat2.yaml
--rw-r--r--   0 fall      (1000) fall      (1000)      149 2024-03-04 09:35:20.000000 monsda-1.2.6/envs/index.yaml
--rw-r--r--   0 fall      (1000) fall      (1000)     3195 2024-03-04 09:35:20.000000 monsda-1.2.6/envs/isoformswitchanalyzer.yaml
--rw-r--r--   0 fall      (1000) fall      (1000)      153 2024-03-04 09:35:20.000000 monsda-1.2.6/envs/macs.yaml
--rw-r--r--   0 fall      (1000) fall      (1000)      139 2024-03-04 09:35:20.000000 monsda-1.2.6/envs/minimap.yaml
--rw-r--r--   0 fall      (1000) fall      (1000)      632 2024-05-22 12:25:05.000000 monsda-1.2.6/envs/monsda.yaml
--rw-r--r--   0 fall      (1000) fall      (1000)     6213 2024-03-04 09:35:20.000000 monsda-1.2.6/envs/peaks.yaml
--rw-r--r--   0 fall      (1000) fall      (1000)     1525 2024-03-04 09:35:20.000000 monsda-1.2.6/envs/perl.yaml
--rw-r--r--   0 fall      (1000) fall      (1000)      129 2024-03-04 09:35:20.000000 monsda-1.2.6/envs/picard.yaml
--rw-r--r--   0 fall      (1000) fall      (1000)      142 2024-03-04 09:35:20.000000 monsda-1.2.6/envs/piranha.yaml
--rw-r--r--   0 fall      (1000) fall      (1000)       91 2024-04-16 12:14:02.000000 monsda-1.2.6/envs/qc.yaml
--rw-r--r--   0 fall      (1000) fall      (1000)      103 2024-03-04 09:35:20.000000 monsda-1.2.6/envs/salmon.yaml
--rw-r--r--   0 fall      (1000) fall      (1000)      131 2024-03-04 09:35:20.000000 monsda-1.2.6/envs/samtools.yaml
--rw-r--r--   0 fall      (1000) fall      (1000)      213 2024-03-04 09:35:20.000000 monsda-1.2.6/envs/scyphy.yaml
--rw-r--r--   0 fall      (1000) fall      (1000)      151 2024-03-04 09:35:20.000000 monsda-1.2.6/envs/segemehl.yaml
--rw-r--r--   0 fall      (1000) fall      (1000)      145 2024-03-04 09:35:20.000000 monsda-1.2.6/envs/segemehl3.yaml
--rw-r--r--   0 fall      (1000) fall      (1000)      158 2024-03-04 09:35:20.000000 monsda-1.2.6/envs/sra.yaml
--rw-r--r--   0 fall      (1000) fall      (1000)      121 2024-03-04 09:35:20.000000 monsda-1.2.6/envs/star.yaml
--rw-r--r--   0 fall      (1000) fall      (1000)      562 2024-03-04 09:35:20.000000 monsda-1.2.6/envs/summary.yaml
--rw-r--r--   0 fall      (1000) fall      (1000)      123 2024-03-04 09:35:20.000000 monsda-1.2.6/envs/trimgalore.yaml
--rw-r--r--   0 fall      (1000) fall      (1000)      235 2024-03-04 09:35:20.000000 monsda-1.2.6/envs/trimm.yaml
--rw-r--r--   0 fall      (1000) fall      (1000)      161 2024-03-04 09:35:20.000000 monsda-1.2.6/envs/trimmomatic.yaml
--rw-r--r--   0 fall      (1000) fall      (1000)      159 2024-03-04 09:35:20.000000 monsda-1.2.6/envs/trnascan.yaml
--rw-r--r--   0 fall      (1000) fall      (1000)      228 2024-03-04 09:35:20.000000 monsda-1.2.6/envs/ucsc.yaml
--rw-r--r--   0 fall      (1000) fall      (1000)      150 2024-03-04 09:35:20.000000 monsda-1.2.6/envs/umitools.yaml
--rw-r--r--   0 fall      (1000) fall      (1000)      106 2024-03-04 09:35:20.000000 monsda-1.2.6/envs/zip.yaml
-drwxr-xr-x   0 fall      (1000) fall      (1000)        0 2024-05-22 12:27:33.689138 monsda-1.2.6/profile_nextflow/
--rw-r--r--   0 fall      (1000) fall      (1000)      217 2024-03-27 11:17:58.000000 monsda-1.2.6/profile_nextflow/nextflow.config
-drwxr-xr-x   0 fall      (1000) fall      (1000)        0 2024-05-22 12:27:33.690138 monsda-1.2.6/profile_snakemake/
--rw-r--r--   0 fall      (1000) fall      (1000)      344 2024-03-04 09:35:20.000000 monsda-1.2.6/profile_snakemake/cluster_config.yaml
--rw-r--r--   0 fall      (1000) fall      (1000)      277 2024-03-04 09:35:20.000000 monsda-1.2.6/profile_snakemake/config.yaml
--rwxr-xr-x   0 fall      (1000) fall      (1000)       51 2024-03-04 09:35:20.000000 monsda-1.2.6/profile_snakemake/slurm-jobscript.sh
--rwxr-xr-x   0 fall      (1000) fall      (1000)     1826 2024-03-04 09:35:20.000000 monsda-1.2.6/profile_snakemake/slurm-status.py
--rwxr-xr-x   0 fall      (1000) fall      (1000)    10397 2024-03-04 09:35:20.000000 monsda-1.2.6/profile_snakemake/slurm-submit-advanced.py
--rwxr-xr-x   0 fall      (1000) fall      (1000)     1880 2024-03-04 09:35:20.000000 monsda-1.2.6/profile_snakemake/slurm-submit.py
--rw-r--r--   0 fall      (1000) fall      (1000)    10495 2024-03-04 09:35:20.000000 monsda-1.2.6/profile_snakemake/slurm_utils.py
--rw-r--r--   0 fall      (1000) fall      (1000)     1303 2024-03-28 12:07:30.000000 monsda-1.2.6/pyproject.toml
-drwxr-xr-x   0 fall      (1000) fall      (1000)        0 2024-05-22 12:27:33.683138 monsda-1.2.6/scripts/
-drwxr-xr-x   0 fall      (1000) fall      (1000)        0 2024-05-22 12:27:33.692138 monsda-1.2.6/scripts/Analysis/
--rwxr-xr-x   0 fall      (1000) fall      (1000)     2882 2024-03-04 09:35:20.000000 monsda-1.2.6/scripts/Analysis/AddStructure.py
--rwxr-xr-x   0 fall      (1000) fall      (1000)     3647 2024-03-04 09:35:20.000000 monsda-1.2.6/scripts/Analysis/Cluster2tRNA.py
--rwxr-xr-x   0 fall      (1000) fall      (1000)    12627 2024-03-04 09:35:20.000000 monsda-1.2.6/scripts/Analysis/CollectBamStat.py
--rwxr-xr-x   0 fall      (1000) fall      (1000)    25757 2024-03-04 09:35:20.000000 monsda-1.2.6/scripts/Analysis/CountEnds.py
--rwxr-xr-x   0 fall      (1000) fall      (1000)      490 2024-03-04 09:35:20.000000 monsda-1.2.6/scripts/Analysis/CountFastqEnds.pl
-drwxr-xr-x   0 fall      (1000) fall      (1000)        0 2024-05-22 12:27:33.692138 monsda-1.2.6/scripts/Analysis/DAS/
--rwxr-xr-x   0 fall      (1000) fall      (1000)    27615 2024-03-04 09:35:20.000000 monsda-1.2.6/scripts/Analysis/DAS/DIEGO.py
--rwxr-xr-x   0 fall      (1000) fall      (1000)    12133 2024-03-04 09:35:20.000000 monsda-1.2.6/scripts/Analysis/DAS/EDGER.R
--rwxr-xr-x   0 fall      (1000) fall      (1000)     2108 2024-03-04 09:35:20.000000 monsda-1.2.6/scripts/Analysis/DAS/FeatureCounts2DIEGO.pl
--rwxr-xr-x   0 fall      (1000) fall      (1000)    13715 2024-03-04 09:35:20.000000 monsda-1.2.6/scripts/Analysis/DAS/FeatureCounts2DIEGO.py
--rwxr-xr-x   0 fall      (1000) fall      (1000)     4720 2024-03-04 09:35:20.000000 monsda-1.2.6/scripts/Analysis/DAS/diego_contrast_files.py
-drwxr-xr-x   0 fall      (1000) fall      (1000)        0 2024-05-22 12:27:33.692138 monsda-1.2.6/scripts/Analysis/DE/
--rwxr-xr-x   0 fall      (1000) fall      (1000)    15681 2024-03-04 09:35:20.000000 monsda-1.2.6/scripts/Analysis/DE/DESEQ2.R
--rwxr-xr-x   0 fall      (1000) fall      (1000)    16168 2024-03-04 09:35:20.000000 monsda-1.2.6/scripts/Analysis/DE/EDGER.R
-drwxr-xr-x   0 fall      (1000) fall      (1000)        0 2024-05-22 12:27:33.692138 monsda-1.2.6/scripts/Analysis/DEU/
--rwxr-xr-x   0 fall      (1000) fall      (1000)     9059 2024-03-04 09:35:20.000000 monsda-1.2.6/scripts/Analysis/DEU/DEXSEQ.R
--rwxr-xr-x   0 fall      (1000) fall      (1000)     9938 2024-03-04 09:35:20.000000 monsda-1.2.6/scripts/Analysis/DEU/EDGER.R
--rwxr-xr-x   0 fall      (1000) fall      (1000)     9611 2024-03-04 09:35:20.000000 monsda-1.2.6/scripts/Analysis/DEU/prepare_deu_annotation.py
-drwxr-xr-x   0 fall      (1000) fall      (1000)        0 2024-05-22 12:27:33.693138 monsda-1.2.6/scripts/Analysis/DTU/
--rwxr-xr-x   0 fall      (1000) fall      (1000)     7268 2024-03-04 09:35:20.000000 monsda-1.2.6/scripts/Analysis/DTU/DEXSEQ.R
--rwxr-xr-x   0 fall      (1000) fall      (1000)    14986 2024-03-04 09:35:20.000000 monsda-1.2.6/scripts/Analysis/DTU/DRIMSEQ.R
--rwxr-xr-x   0 fall      (1000) fall      (1000)     3421 2024-03-04 09:35:20.000000 monsda-1.2.6/scripts/Analysis/FindPeaks.pl
--rwxr-xr-x   0 fall      (1000) fall      (1000)     2737 2024-03-04 09:35:20.000000 monsda-1.2.6/scripts/Analysis/GOA.R
--rwxr-xr-x   0 fall      (1000) fall      (1000)    14628 2024-03-04 09:35:20.000000 monsda-1.2.6/scripts/Analysis/GenerateTrackDb.py
--rwxr-xr-x   0 fall      (1000) fall      (1000)      426 2024-03-04 09:35:20.000000 monsda-1.2.6/scripts/Analysis/GettRNAExpression.sh
--rwxr-xr-x   0 fall      (1000) fall      (1000)     5106 2024-03-04 09:35:20.000000 monsda-1.2.6/scripts/Analysis/NormalizePeaks.pl
--rwxr-xr-x   0 fall      (1000) fall      (1000)     5174 2024-03-04 09:35:20.000000 monsda-1.2.6/scripts/Analysis/PlBed2Bedgraph.pl
--rwxr-xr-x   0 fall      (1000) fall      (1000)     2228 2024-03-04 09:35:20.000000 monsda-1.2.6/scripts/Analysis/PreprocessPeaks.pl
--rwxr-xr-x   0 fall      (1000) fall      (1000)     8094 2024-03-04 09:35:20.000000 monsda-1.2.6/scripts/Analysis/RemoveSoftClip.py
--rwxr-xr-x   0 fall      (1000) fall      (1000)    11489 2024-03-04 09:35:20.000000 monsda-1.2.6/scripts/Analysis/RmdCreator.py
-drwxr-xr-x   0 fall      (1000) fall      (1000)        0 2024-05-22 12:27:33.693138 monsda-1.2.6/scripts/Analysis/SUMMARY/
--rwxr-xr-x   0 fall      (1000) fall      (1000)      408 2024-03-04 09:35:20.000000 monsda-1.2.6/scripts/Analysis/SUMMARY/header_summary.Rmd
--rwxr-xr-x   0 fall      (1000) fall      (1000)    13324 2024-03-04 09:35:20.000000 monsda-1.2.6/scripts/Analysis/build_DEU_table.py
--rwxr-xr-x   0 fall      (1000) fall      (1000)    10925 2024-03-04 09:35:20.000000 monsda-1.2.6/scripts/Analysis/build_DTU_table.py
--rwxr-xr-x   0 fall      (1000) fall      (1000)    14005 2024-03-04 09:35:20.000000 monsda-1.2.6/scripts/Analysis/build_count_table.py
--rwxr-xr-x   0 fall      (1000) fall      (1000)    11421 2024-03-04 09:35:20.000000 monsda-1.2.6/scripts/Analysis/build_salmon_table.py
-drwxr-xr-x   0 fall      (1000) fall      (1000)        0 2024-05-22 12:27:33.693138 monsda-1.2.6/scripts/Preprocessing/
--rwxr-xr-x   0 fall      (1000) fall      (1000)      237 2024-03-04 09:35:20.000000 monsda-1.2.6/scripts/Preprocessing/indexfa.sh
-drwxr-xr-x   0 fall      (1000) fall      (1000)        0 2024-05-22 12:27:33.694138 monsda-1.2.6/scripts/Shells/
--rw-r--r--   0 fall      (1000) fall      (1000)     1754 2024-03-04 09:35:20.000000 monsda-1.2.6/scripts/Shells/MergeExpression_Cufflinks.sh
--rw-r--r--   0 fall      (1000) fall      (1000)     1620 2024-03-04 09:35:20.000000 monsda-1.2.6/scripts/Shells/MergeExpression_RNAcounter.sh
--rw-r--r--   0 fall      (1000) fall      (1000)     1517 2024-03-04 09:35:20.000000 monsda-1.2.6/scripts/Shells/MergeGeneExpression_Cufflinks.sh
--rwxr-xr-x   0 fall      (1000) fall      (1000)      670 2024-03-25 16:31:46.000000 monsda-1.2.6/scripts/Shells/NonUniqueBam_woPicard.sh
--rwxr-xr-x   0 fall      (1000) fall      (1000)      565 2024-03-15 07:51:51.000000 monsda-1.2.6/scripts/Shells/NonUniqueBam_woPicard.sh~
--rwxr-xr-x   0 fall      (1000) fall      (1000)      460 2024-03-04 09:35:20.000000 monsda-1.2.6/scripts/Shells/Sam2Bam.sh
--rwxr-xr-x   0 fall      (1000) fall      (1000)      440 2024-03-04 09:35:20.000000 monsda-1.2.6/scripts/Shells/Sam2Bed.sh
--rwxr-xr-x   0 fall      (1000) fall      (1000)      966 2024-04-16 12:14:02.000000 monsda-1.2.6/scripts/Shells/UniqueBam_woPicard.sh
--rwxr-xr-x   0 fall      (1000) fall      (1000)      551 2024-03-15 07:50:55.000000 monsda-1.2.6/scripts/Shells/UniqueBam_woPicard.sh~
--rwxr-xr-x   0 fall      (1000) fall      (1000)     1628 2024-04-16 12:14:02.000000 monsda-1.2.6/scripts/Shells/UniqueSam_woPicard.sh
--rwxr-xr-x   0 fall      (1000) fall      (1000)      536 2024-03-04 09:35:20.000000 monsda-1.2.6/scripts/Shells/printEnds.sh
--rwxr-xr-x   0 fall      (1000) fall      (1000)      342 2024-03-04 09:35:20.000000 monsda-1.2.6/scripts/Shells/printFQEnds.sh
-drwxr-xr-x   0 fall      (1000) fall      (1000)        0 2024-05-22 12:27:33.694138 monsda-1.2.6/scripts/Universal/
--rwxr-xr-x   0 fall      (1000) fall      (1000)     8806 2024-03-28 12:04:17.000000 monsda-1.2.6/scripts/Universal/AnnotateBed.pl
--rwxr-xr-x   0 fall      (1000) fall      (1000)     5046 2024-03-04 09:35:20.000000 monsda-1.2.6/scripts/Universal/Bed2Bedgraph.pl
--rwxr-xr-x   0 fall      (1000) fall      (1000)     8118 2024-03-04 09:35:20.000000 monsda-1.2.6/scripts/Universal/ExtendBed.pl
--rw-r--r--   0 fall      (1000) fall      (1000)     2303 2024-03-04 09:35:20.000000 monsda-1.2.6/scripts/Universal/countCCA.pl
--rw-r--r--   0 fall      (1000) fall      (1000)      710 2024-03-04 09:35:20.000000 monsda-1.2.6/scripts/Universal/sam2fastq.pl
-drwxr-xr-x   0 fall      (1000) fall      (1000)        0 2024-05-22 12:27:33.694138 monsda-1.2.6/scripts/lib/
--rwxr-xr-x   0 fall      (1000) fall      (1000)    67149 2024-03-04 09:35:20.000000 monsda-1.2.6/scripts/lib/Collection.pm
--rwxr-xr-x   0 fall      (1000) fall      (1000)     3227 2024-03-04 09:35:20.000000 monsda-1.2.6/scripts/lib/Logger.py
--rw-r--r--   0 fall      (1000) fall      (1000)        0 2024-03-04 09:35:20.000000 monsda-1.2.6/scripts/lib/__init.py__
--rw-r--r--   0 fall      (1000) fall      (1000)     1099 2024-03-04 09:35:20.000000 monsda-1.2.6/scripts/lib/_lib.R
--rw-r--r--   0 fall      (1000) fall      (1000)      648 2024-05-22 12:27:33.704138 monsda-1.2.6/setup.cfg
--rw-r--r--   0 fall      (1000) fall      (1000)     3297 2024-03-26 16:29:05.000000 monsda-1.2.6/setup.py
-drwxr-xr-x   0 fall      (1000) fall      (1000)        0 2024-05-22 12:27:33.694138 monsda-1.2.6/tests/
--rwxr-xr-x   0 fall      (1000) fall      (1000)     3454 2024-03-25 16:31:46.000000 monsda-1.2.6/tests/test_functions.py
--rw-r--r--   0 fall      (1000) fall      (1000)    78254 2024-03-04 09:35:20.000000 monsda-1.2.6/versioneer.py
-drwxr-xr-x   0 fall      (1000) fall      (1000)        0 2024-05-22 12:27:33.703138 monsda-1.2.6/workflows/
--rw-r--r--   0 fall      (1000) fall      (1000)     7289 2024-03-04 09:35:20.000000 monsda-1.2.6/workflows/annotatebed.smk
--rw-r--r--   0 fall      (1000) fall      (1000)     2023 2024-03-04 09:35:20.000000 monsda-1.2.6/workflows/bbduk.nf
--rw-r--r--   0 fall      (1000) fall      (1000)     2713 2024-03-04 09:35:20.000000 monsda-1.2.6/workflows/bbduk.smk
--rw-r--r--   0 fall      (1000) fall      (1000)     3857 2024-03-04 09:35:20.000000 monsda-1.2.6/workflows/bwa.nf
--rw-r--r--   0 fall      (1000) fall      (1000)    14226 2024-03-04 09:35:20.000000 monsda-1.2.6/workflows/bwa.smk
--rw-r--r--   0 fall      (1000) fall      (1000)     3846 2024-03-04 09:35:20.000000 monsda-1.2.6/workflows/bwa2.nf
--rw-r--r--   0 fall      (1000) fall      (1000)     3499 2024-03-04 09:35:20.000000 monsda-1.2.6/workflows/bwa2.smk
--rw-r--r--   0 fall      (1000) fall      (1000)     4232 2024-03-04 09:35:20.000000 monsda-1.2.6/workflows/bwameth.nf
--rw-r--r--   0 fall      (1000) fall      (1000)     3360 2024-03-04 09:35:20.000000 monsda-1.2.6/workflows/bwameth.smk
--rw-r--r--   0 fall      (1000) fall      (1000)     2050 2024-03-04 09:35:20.000000 monsda-1.2.6/workflows/ciri2.nf
--rw-r--r--   0 fall      (1000) fall      (1000)     1816 2024-03-04 09:35:20.000000 monsda-1.2.6/workflows/ciri2.smk
--rw-r--r--   0 fall      (1000) fall      (1000)      507 2024-03-04 09:35:20.000000 monsda-1.2.6/workflows/collect.nf
--rw-r--r--   0 fall      (1000) fall      (1000)     9861 2024-03-04 09:35:20.000000 monsda-1.2.6/workflows/countreads.nf
--rw-r--r--   0 fall      (1000) fall      (1000)    15432 2024-03-04 09:35:20.000000 monsda-1.2.6/workflows/countreads.smk
--rw-r--r--   0 fall      (1000) fall      (1000)     2243 2024-03-04 09:35:20.000000 monsda-1.2.6/workflows/cutadapt.nf
--rw-r--r--   0 fall      (1000) fall      (1000)     2934 2024-03-04 09:35:20.000000 monsda-1.2.6/workflows/cutadapt.smk
--rw-r--r--   0 fall      (1000) fall      (1000)     7456 2024-03-04 09:35:20.000000 monsda-1.2.6/workflows/deseq2_DE.nf
--rw-r--r--   0 fall      (1000) fall      (1000)     7927 2024-03-04 09:35:20.000000 monsda-1.2.6/workflows/deseq2_DE.smk
--rw-r--r--   0 fall      (1000) fall      (1000)     9193 2024-03-04 09:35:20.000000 monsda-1.2.6/workflows/dexseq_DEU.nf
--rw-r--r--   0 fall      (1000) fall      (1000)     8476 2024-03-04 09:35:20.000000 monsda-1.2.6/workflows/dexseq_DEU.smk
--rw-r--r--   0 fall      (1000) fall      (1000)     8100 2024-03-04 09:35:20.000000 monsda-1.2.6/workflows/dexseq_DTU.nf
--rw-r--r--   0 fall      (1000) fall      (1000)    10062 2024-03-04 09:35:20.000000 monsda-1.2.6/workflows/dexseq_DTU.smk
--rw-r--r--   0 fall      (1000) fall      (1000)     9334 2024-03-04 09:35:20.000000 monsda-1.2.6/workflows/diego_DAS.nf
--rw-r--r--   0 fall      (1000) fall      (1000)     8157 2024-03-04 09:35:20.000000 monsda-1.2.6/workflows/diego_DAS.smk
--rw-r--r--   0 fall      (1000) fall      (1000)     1394 2024-03-04 09:35:20.000000 monsda-1.2.6/workflows/dorado.nf
--rw-r--r--   0 fall      (1000) fall      (1000)     1262 2024-03-04 09:35:20.000000 monsda-1.2.6/workflows/dorado.smk
--rw-r--r--   0 fall      (1000) fall      (1000)     8123 2024-03-04 09:35:20.000000 monsda-1.2.6/workflows/drimseq_DTU.nf
--rw-r--r--   0 fall      (1000) fall      (1000)    13421 2024-03-04 09:35:20.000000 monsda-1.2.6/workflows/drimseq_DTU.smk
--rw-r--r--   0 fall      (1000) fall      (1000)     7763 2024-03-04 09:35:20.000000 monsda-1.2.6/workflows/edger_DAS.nf
--rw-r--r--   0 fall      (1000) fall      (1000)     7887 2024-03-04 09:35:20.000000 monsda-1.2.6/workflows/edger_DAS.smk
--rw-r--r--   0 fall      (1000) fall      (1000)     7631 2024-03-04 09:35:20.000000 monsda-1.2.6/workflows/edger_DE.nf
--rw-r--r--   0 fall      (1000) fall      (1000)     7806 2024-03-04 09:35:20.000000 monsda-1.2.6/workflows/edger_DE.smk
--rw-r--r--   0 fall      (1000) fall      (1000)     7681 2024-03-04 09:35:20.000000 monsda-1.2.6/workflows/edger_DEU.nf
--rw-r--r--   0 fall      (1000) fall      (1000)     7668 2024-03-04 09:35:20.000000 monsda-1.2.6/workflows/edger_DEU.smk
--rw-r--r--   0 fall      (1000) fall      (1000)     3191 2024-03-04 09:35:20.000000 monsda-1.2.6/workflows/fastqc.nf
--rw-r--r--   0 fall      (1000) fall      (1000)     5830 2024-03-04 09:35:20.000000 monsda-1.2.6/workflows/fastqc.smk
--rw-r--r--   0 fall      (1000) fall      (1000)     2040 2024-03-04 09:35:20.000000 monsda-1.2.6/workflows/fastqc_dedup.nf
--rw-r--r--   0 fall      (1000) fall      (1000)     4596 2024-03-04 09:35:20.000000 monsda-1.2.6/workflows/fastqc_dedup.smk
--rw-r--r--   0 fall      (1000) fall      (1000)     2851 2024-03-04 09:35:20.000000 monsda-1.2.6/workflows/fastqc_dedup_trim.nf
--rw-r--r--   0 fall      (1000) fall      (1000)     5978 2024-03-04 09:35:20.000000 monsda-1.2.6/workflows/fastqc_dedup_trim.smk
--rw-r--r--   0 fall      (1000) fall      (1000)      860 2024-03-04 09:35:20.000000 monsda-1.2.6/workflows/fastqc_raw.nf
--rw-r--r--   0 fall      (1000) fall      (1000)     2901 2024-03-04 09:35:20.000000 monsda-1.2.6/workflows/fastqc_raw.smk
--rw-r--r--   0 fall      (1000) fall      (1000)     2069 2024-03-04 09:35:20.000000 monsda-1.2.6/workflows/fastqc_trim.nf
--rw-r--r--   0 fall      (1000) fall      (1000)     4661 2024-03-04 09:35:20.000000 monsda-1.2.6/workflows/fastqc_trim.smk
--rw-r--r--   0 fall      (1000) fall      (1000)       91 2024-03-04 09:35:20.000000 monsda-1.2.6/workflows/footer.nf
--rw-r--r--   0 fall      (1000) fall      (1000)       90 2024-03-04 09:35:20.000000 monsda-1.2.6/workflows/footer.smk
--rw-r--r--   0 fall      (1000) fall      (1000)     1788 2024-03-04 09:35:20.000000 monsda-1.2.6/workflows/guppy.nf
--rw-r--r--   0 fall      (1000) fall      (1000)     1661 2024-03-04 09:35:20.000000 monsda-1.2.6/workflows/guppy.smk
--rw-r--r--   0 fall      (1000) fall      (1000)     1609 2024-03-04 09:35:20.000000 monsda-1.2.6/workflows/header.nf
--rw-r--r--   0 fall      (1000) fall      (1000)    12190 2024-03-04 09:35:20.000000 monsda-1.2.6/workflows/header.smk
--rw-r--r--   0 fall      (1000) fall      (1000)     4459 2024-03-04 09:35:20.000000 monsda-1.2.6/workflows/hisat2.nf
--rw-r--r--   0 fall      (1000) fall      (1000)     4844 2024-03-04 09:35:20.000000 monsda-1.2.6/workflows/hisat2.smk
--rw-r--r--   0 fall      (1000) fall      (1000)     7366 2024-03-04 09:35:20.000000 monsda-1.2.6/workflows/macs.nf
--rw-r--r--   0 fall      (1000) fall      (1000)    14219 2024-03-04 09:35:20.000000 monsda-1.2.6/workflows/macs.smk
--rw-r--r--   0 fall      (1000) fall      (1000)     2372 2024-03-04 09:35:20.000000 monsda-1.2.6/workflows/manipulate_genome.nf
--rw-r--r--   0 fall      (1000) fall      (1000)     2359 2024-03-04 09:35:20.000000 monsda-1.2.6/workflows/manipulate_genome.smk
--rw-r--r--   0 fall      (1000) fall      (1000)     4247 2024-03-04 09:35:20.000000 monsda-1.2.6/workflows/mapping.nf
--rw-r--r--   0 fall      (1000) fall      (1000)     2698 2024-03-04 09:35:20.000000 monsda-1.2.6/workflows/mapping.smk
--rw-r--r--   0 fall      (1000) fall      (1000)     3854 2024-03-04 09:35:20.000000 monsda-1.2.6/workflows/minimap.nf
--rw-r--r--   0 fall      (1000) fall      (1000)     2968 2024-03-04 09:35:20.000000 monsda-1.2.6/workflows/minimap.smk
--rw-r--r--   0 fall      (1000) fall      (1000)     1022 2024-03-04 09:35:20.000000 monsda-1.2.6/workflows/multiqc.nf
--rw-r--r--   0 fall      (1000) fall      (1000)    10636 2024-03-04 09:35:20.000000 monsda-1.2.6/workflows/multiqc.smk
--rw-r--r--   0 fall      (1000) fall      (1000)     5667 2024-03-04 09:35:20.000000 monsda-1.2.6/workflows/notify.nf
--rw-r--r--   0 fall      (1000) fall      (1000)    11912 2024-03-04 09:35:20.000000 monsda-1.2.6/workflows/peaks.nf
--rw-r--r--   0 fall      (1000) fall      (1000)    21124 2024-03-04 09:35:20.000000 monsda-1.2.6/workflows/peaks.smk
--rw-r--r--   0 fall      (1000) fall      (1000)     1797 2024-03-04 09:35:20.000000 monsda-1.2.6/workflows/picard_dedup.nf
--rw-r--r--   0 fall      (1000) fall      (1000)     1250 2024-03-04 09:35:20.000000 monsda-1.2.6/workflows/picard_dedup.smk
--rw-r--r--   0 fall      (1000) fall      (1000)    12177 2024-03-04 09:35:20.000000 monsda-1.2.6/workflows/piranha.nf
--rw-r--r--   0 fall      (1000) fall      (1000)    20575 2024-03-04 09:35:20.000000 monsda-1.2.6/workflows/piranha.smk
--rw-r--r--   0 fall      (1000) fall      (1000)     1150 2024-03-04 09:35:20.000000 monsda-1.2.6/workflows/premultiqc.nf
--rw-r--r--   0 fall      (1000) fall      (1000)     1557 2024-03-04 09:35:20.000000 monsda-1.2.6/workflows/premultiqc.smk
--rw-r--r--   0 fall      (1000) fall      (1000)     5313 2024-03-04 09:35:20.000000 monsda-1.2.6/workflows/salmon.nf
--rw-r--r--   0 fall      (1000) fall      (1000)     3679 2024-03-04 09:35:20.000000 monsda-1.2.6/workflows/salmon.smk
--rw-r--r--   0 fall      (1000) fall      (1000)     4997 2024-03-04 09:35:20.000000 monsda-1.2.6/workflows/salmon_trim.smk
--rw-r--r--   0 fall      (1000) fall      (1000)    22666 2024-03-04 09:35:20.000000 monsda-1.2.6/workflows/scyphy.nf
--rw-r--r--   0 fall      (1000) fall      (1000)    32938 2024-03-04 09:35:20.000000 monsda-1.2.6/workflows/scyphy.smk
--rw-r--r--   0 fall      (1000) fall      (1000)     3881 2024-03-04 09:35:20.000000 monsda-1.2.6/workflows/segemehl.nf
--rw-r--r--   0 fall      (1000) fall      (1000)     3098 2024-03-04 09:35:20.000000 monsda-1.2.6/workflows/segemehl.smk
--rw-r--r--   0 fall      (1000) fall      (1000)     4378 2024-03-04 09:35:20.000000 monsda-1.2.6/workflows/segemehl3.nf
--rw-r--r--   0 fall      (1000) fall      (1000)     4699 2024-03-04 09:35:20.000000 monsda-1.2.6/workflows/segemehl3.smk
--rw-r--r--   0 fall      (1000) fall      (1000)     4613 2024-03-04 09:35:20.000000 monsda-1.2.6/workflows/segemehl3_bisulfite.nf
--rw-r--r--   0 fall      (1000) fall      (1000)     3695 2024-03-04 09:35:20.000000 monsda-1.2.6/workflows/segemehl3_bisulfite.smk
--rw-r--r--   0 fall      (1000) fall      (1000)     4681 2024-03-04 09:35:20.000000 monsda-1.2.6/workflows/segemehl_bisulfite.nf
--rw-r--r--   0 fall      (1000) fall      (1000)     3848 2024-03-04 09:35:20.000000 monsda-1.2.6/workflows/segemehl_bisulfite.smk
--rw-r--r--   0 fall      (1000) fall      (1000)     1719 2024-03-04 09:35:20.000000 monsda-1.2.6/workflows/simulatetrim.nf
--rw-r--r--   0 fall      (1000) fall      (1000)     1425 2024-03-04 09:35:20.000000 monsda-1.2.6/workflows/simulatetrim.smk
--rw-r--r--   0 fall      (1000) fall      (1000)     2017 2024-03-04 09:35:20.000000 monsda-1.2.6/workflows/sra.nf
--rw-r--r--   0 fall      (1000) fall      (1000)     3905 2024-03-04 09:35:20.000000 monsda-1.2.6/workflows/sra.smk
--rw-r--r--   0 fall      (1000) fall      (1000)     6531 2024-03-25 16:31:46.000000 monsda-1.2.6/workflows/star.nf
--rw-r--r--   0 fall      (1000) fall      (1000)     8723 2024-03-25 16:31:46.000000 monsda-1.2.6/workflows/star.smk
--rw-r--r--   0 fall      (1000) fall      (1000)     1190 2024-03-04 09:35:20.000000 monsda-1.2.6/workflows/summary.nf
--rw-r--r--   0 fall      (1000) fall      (1000)      857 2024-03-04 09:35:20.000000 monsda-1.2.6/workflows/summary.smk
--rw-r--r--   0 fall      (1000) fall      (1000)     2028 2024-03-04 09:35:20.000000 monsda-1.2.6/workflows/trimgalore.nf
--rw-r--r--   0 fall      (1000) fall      (1000)     3378 2024-03-04 09:35:20.000000 monsda-1.2.6/workflows/trimgalore.smk
--rw-r--r--   0 fall      (1000) fall      (1000)     7481 2024-03-04 09:35:20.000000 monsda-1.2.6/workflows/ucsc.nf
--rw-r--r--   0 fall      (1000) fall      (1000)     8139 2024-03-04 09:35:20.000000 monsda-1.2.6/workflows/ucsc.smk
--rw-r--r--   0 fall      (1000) fall      (1000)     4093 2024-03-04 09:35:20.000000 monsda-1.2.6/workflows/umitools.nf
--rw-r--r--   0 fall      (1000) fall      (1000)     7717 2024-03-04 09:35:20.000000 monsda-1.2.6/workflows/umitools.smk
--rw-r--r--   0 fall      (1000) fall      (1000)     1656 2024-03-04 09:35:20.000000 monsda-1.2.6/workflows/umitools_dedup.nf
--rw-r--r--   0 fall      (1000) fall      (1000)        1 2024-03-04 09:35:20.000000 monsda-1.2.6/workflows/unlock.smk
+drwxr-xr-x   0 fall      (1000) fall      (1000)        0 2024-06-03 08:00:03.110456 monsda-1.2.7/
+-rw-r--r--   0 fall      (1000) fall      (1000)    35149 2024-03-04 09:35:20.000000 monsda-1.2.7/LICENSE
+-rw-r--r--   0 fall      (1000) fall      (1000)       49 2024-03-04 09:35:20.000000 monsda-1.2.7/MANIFEST.in
+drwxr-xr-x   0 fall      (1000) fall      (1000)        0 2024-06-03 08:00:02.924458 monsda-1.2.7/MONSDA/
+-rwxr-xr-x   0 fall      (1000) fall      (1000)    70162 2024-03-25 16:31:46.000000 monsda-1.2.7/MONSDA/Configurator.py
+-rw-r--r--   0 fall      (1000) fall      (1000)     5763 2024-03-04 09:35:20.000000 monsda-1.2.7/MONSDA/Deprecated.py
+-rwxr-xr-x   0 fall      (1000) fall      (1000)     2581 2024-03-04 09:35:20.000000 monsda-1.2.7/MONSDA/Logger.py
+-rw-r--r--   0 fall      (1000) fall      (1000)    37733 2024-03-25 16:31:46.000000 monsda-1.2.7/MONSDA/Params.py
+-rwxr-xr-x   0 fall      (1000) fall      (1000)    34672 2024-05-31 09:53:46.000000 monsda-1.2.7/MONSDA/RunMONSDA.py
+-rw-r--r--   0 fall      (1000) fall      (1000)    18515 2024-03-25 16:31:46.000000 monsda-1.2.7/MONSDA/Utils.py
+-rwxr-xr-x   0 fall      (1000) fall      (1000)   171767 2024-03-25 16:31:46.000000 monsda-1.2.7/MONSDA/Workflows.py
+-rw-r--r--   0 fall      (1000) fall      (1000)       73 2024-03-04 09:35:20.000000 monsda-1.2.7/MONSDA/__init__.py
+-rw-r--r--   0 fall      (1000) fall      (1000)       32 2024-03-04 09:35:20.000000 monsda-1.2.7/MONSDA/__main__.py
+-rw-r--r--   0 fall      (1000) fall      (1000)      497 2024-06-03 08:00:03.114456 monsda-1.2.7/MONSDA/_version.py
+drwxr-xr-x   0 fall      (1000) fall      (1000)        0 2024-06-03 08:00:02.930458 monsda-1.2.7/MONSDA/lib/
+-rw-r--r--   0 fall      (1000) fall      (1000)     2357 2024-03-04 09:35:20.000000 monsda-1.2.7/MONSDA/lib/Collection.groovy
+drwxr-xr-x   0 fall      (1000) fall      (1000)        0 2024-06-03 08:00:03.106456 monsda-1.2.7/MONSDA.egg-info/
+-rw-r--r--   0 fall      (1000) fall      (1000)    47451 2024-06-03 08:00:02.000000 monsda-1.2.7/MONSDA.egg-info/PKG-INFO
+-rw-r--r--   0 fall      (1000) fall      (1000)     6004 2024-06-03 08:00:02.000000 monsda-1.2.7/MONSDA.egg-info/SOURCES.txt
+-rw-r--r--   0 fall      (1000) fall      (1000)        1 2024-06-03 08:00:02.000000 monsda-1.2.7/MONSDA.egg-info/dependency_links.txt
+-rw-r--r--   0 fall      (1000) fall      (1000)       93 2024-06-03 08:00:02.000000 monsda-1.2.7/MONSDA.egg-info/entry_points.txt
+-rw-r--r--   0 fall      (1000) fall      (1000)        1 2024-03-19 14:46:42.000000 monsda-1.2.7/MONSDA.egg-info/not-zip-safe
+-rw-r--r--   0 fall      (1000) fall      (1000)       89 2024-06-03 08:00:02.000000 monsda-1.2.7/MONSDA.egg-info/requires.txt
+-rw-r--r--   0 fall      (1000) fall      (1000)        7 2024-06-03 08:00:02.000000 monsda-1.2.7/MONSDA.egg-info/top_level.txt
+-rw-r--r--   0 fall      (1000) fall      (1000)    47451 2024-06-03 08:00:03.109455 monsda-1.2.7/PKG-INFO
+-rw-r--r--   0 fall      (1000) fall      (1000)     6058 2024-03-04 09:43:25.000000 monsda-1.2.7/README.md
+drwxr-xr-x   0 fall      (1000) fall      (1000)        0 2024-06-03 08:00:02.936458 monsda-1.2.7/configs/
+-rw-r--r--   0 fall      (1000) fall      (1000)    24464 2024-05-29 11:17:30.000000 monsda-1.2.7/configs/template.json
+-rw-r--r--   0 fall      (1000) fall      (1000)    14131 2024-03-04 09:43:25.000000 monsda-1.2.7/configs/template_base_commented.json
+-rw-r--r--   0 fall      (1000) fall      (1000)     9007 2024-05-29 11:17:30.000000 monsda-1.2.7/configs/template_clean.json
+-rw-r--r--   0 fall      (1000) fall      (1000)    19963 2024-05-29 11:17:30.000000 monsda-1.2.7/configs/tutorial_exhaustive.json
+-rw-r--r--   0 fall      (1000) fall      (1000)    13787 2024-05-29 11:17:30.000000 monsda-1.2.7/configs/tutorial_postprocess.json
+-rw-r--r--   0 fall      (1000) fall      (1000)     1171 2024-05-29 11:17:30.000000 monsda-1.2.7/configs/tutorial_quick.json
+-rw-r--r--   0 fall      (1000) fall      (1000)     8919 2024-05-29 11:17:30.000000 monsda-1.2.7/configs/tutorial_toolmix.json
+drwxr-xr-x   0 fall      (1000) fall      (1000)        0 2024-06-03 08:00:02.975457 monsda-1.2.7/envs/
+-rw-r--r--   0 fall      (1000) fall      (1000)     5071 2024-03-04 09:35:20.000000 monsda-1.2.7/envs/LoveSonesonPatro.yaml
+-rw-r--r--   0 fall      (1000) fall      (1000)      259 2024-03-04 09:35:20.000000 monsda-1.2.7/envs/base.yaml
+-rw-r--r--   0 fall      (1000) fall      (1000)      114 2024-03-04 09:35:20.000000 monsda-1.2.7/envs/bbduk.yaml
+-rw-r--r--   0 fall      (1000) fall      (1000)      114 2024-03-04 09:35:20.000000 monsda-1.2.7/envs/bbmap.yaml
+-rw-r--r--   0 fall      (1000) fall      (1000)      210 2024-03-04 09:35:20.000000 monsda-1.2.7/envs/bedtools.yaml
+-rw-r--r--   0 fall      (1000) fall      (1000)      132 2024-03-04 09:35:20.000000 monsda-1.2.7/envs/bwa.yaml
+-rw-r--r--   0 fall      (1000) fall      (1000)      136 2024-03-04 09:35:20.000000 monsda-1.2.7/envs/bwa2.yaml
+-rw-r--r--   0 fall      (1000) fall      (1000)      159 2024-03-04 09:35:20.000000 monsda-1.2.7/envs/bwameth.yaml
+-rw-r--r--   0 fall      (1000) fall      (1000)      122 2024-03-04 09:35:20.000000 monsda-1.2.7/envs/ciri2.yaml
+-rw-r--r--   0 fall      (1000) fall      (1000)      356 2024-03-04 09:35:20.000000 monsda-1.2.7/envs/countreads.yaml
+-rw-r--r--   0 fall      (1000) fall      (1000)      359 2024-03-04 09:35:20.000000 monsda-1.2.7/envs/countreads_de.yaml
+-rw-r--r--   0 fall      (1000) fall      (1000)      118 2024-03-04 09:35:20.000000 monsda-1.2.7/envs/cutadapt.yaml
+-rw-r--r--   0 fall      (1000) fall      (1000)     4373 2024-05-31 13:22:18.000000 monsda-1.2.7/envs/deseq2_DE.yaml
+-rw-r--r--   0 fall      (1000) fall      (1000)     3328 2024-03-04 09:35:20.000000 monsda-1.2.7/envs/dexseq_DEU.yaml
+-rw-r--r--   0 fall      (1000) fall      (1000)     3200 2024-03-04 09:35:20.000000 monsda-1.2.7/envs/dexseq_DTU.yaml
+-rw-r--r--   0 fall      (1000) fall      (1000)      347 2024-03-04 09:35:20.000000 monsda-1.2.7/envs/diego_DAS.yaml
+-rw-r--r--   0 fall      (1000) fall      (1000)      120 2024-03-04 09:35:20.000000 monsda-1.2.7/envs/dorado.yaml
+-rw-r--r--   0 fall      (1000) fall      (1000)     2948 2024-03-04 09:35:20.000000 monsda-1.2.7/envs/drimseq_DTU.yaml
+-rw-r--r--   0 fall      (1000) fall      (1000)     1465 2024-03-04 09:35:20.000000 monsda-1.2.7/envs/edger_DAS.yaml
+-rw-r--r--   0 fall      (1000) fall      (1000)     4396 2024-05-31 13:36:20.000000 monsda-1.2.7/envs/edger_DE.yaml
+-rw-r--r--   0 fall      (1000) fall      (1000)     1465 2024-03-04 09:35:20.000000 monsda-1.2.7/envs/edger_DEU.yaml
+-rw-r--r--   0 fall      (1000) fall      (1000)       91 2024-04-16 12:14:02.000000 monsda-1.2.7/envs/fastqc.yaml
+-rw-r--r--   0 fall      (1000) fall      (1000)      290 2024-03-04 09:35:20.000000 monsda-1.2.7/envs/guppy.yaml
+-rw-r--r--   0 fall      (1000) fall      (1000)      190 2024-03-04 09:35:20.000000 monsda-1.2.7/envs/hisat2.yaml
+-rw-r--r--   0 fall      (1000) fall      (1000)      149 2024-03-04 09:35:20.000000 monsda-1.2.7/envs/index.yaml
+-rw-r--r--   0 fall      (1000) fall      (1000)     3195 2024-03-04 09:35:20.000000 monsda-1.2.7/envs/isoformswitchanalyzer.yaml
+-rw-r--r--   0 fall      (1000) fall      (1000)      153 2024-03-04 09:35:20.000000 monsda-1.2.7/envs/macs.yaml
+-rw-r--r--   0 fall      (1000) fall      (1000)      139 2024-03-04 09:35:20.000000 monsda-1.2.7/envs/minimap.yaml
+-rw-r--r--   0 fall      (1000) fall      (1000)      632 2024-05-29 13:51:58.000000 monsda-1.2.7/envs/monsda.yaml
+-rw-r--r--   0 fall      (1000) fall      (1000)     6213 2024-03-04 09:35:20.000000 monsda-1.2.7/envs/peaks.yaml
+-rw-r--r--   0 fall      (1000) fall      (1000)     1525 2024-03-04 09:35:20.000000 monsda-1.2.7/envs/perl.yaml
+-rw-r--r--   0 fall      (1000) fall      (1000)      129 2024-03-04 09:35:20.000000 monsda-1.2.7/envs/picard.yaml
+-rw-r--r--   0 fall      (1000) fall      (1000)      142 2024-05-31 09:48:10.000000 monsda-1.2.7/envs/piranha.yaml
+-rw-r--r--   0 fall      (1000) fall      (1000)       91 2024-04-16 12:14:02.000000 monsda-1.2.7/envs/qc.yaml
+-rw-r--r--   0 fall      (1000) fall      (1000)      103 2024-03-04 09:35:20.000000 monsda-1.2.7/envs/salmon.yaml
+-rw-r--r--   0 fall      (1000) fall      (1000)      131 2024-03-04 09:35:20.000000 monsda-1.2.7/envs/samtools.yaml
+-rw-r--r--   0 fall      (1000) fall      (1000)      213 2024-03-04 09:35:20.000000 monsda-1.2.7/envs/scyphy.yaml
+-rw-r--r--   0 fall      (1000) fall      (1000)      151 2024-03-04 09:35:20.000000 monsda-1.2.7/envs/segemehl.yaml
+-rw-r--r--   0 fall      (1000) fall      (1000)      145 2024-03-04 09:35:20.000000 monsda-1.2.7/envs/segemehl3.yaml
+-rw-r--r--   0 fall      (1000) fall      (1000)      158 2024-03-04 09:35:20.000000 monsda-1.2.7/envs/sra.yaml
+-rw-r--r--   0 fall      (1000) fall      (1000)      121 2024-03-04 09:35:20.000000 monsda-1.2.7/envs/star.yaml
+-rw-r--r--   0 fall      (1000) fall      (1000)      562 2024-03-04 09:35:20.000000 monsda-1.2.7/envs/summary.yaml
+-rw-r--r--   0 fall      (1000) fall      (1000)      123 2024-03-04 09:35:20.000000 monsda-1.2.7/envs/trimgalore.yaml
+-rw-r--r--   0 fall      (1000) fall      (1000)      235 2024-03-04 09:35:20.000000 monsda-1.2.7/envs/trimm.yaml
+-rw-r--r--   0 fall      (1000) fall      (1000)      161 2024-03-04 09:35:20.000000 monsda-1.2.7/envs/trimmomatic.yaml
+-rw-r--r--   0 fall      (1000) fall      (1000)      159 2024-03-04 09:35:20.000000 monsda-1.2.7/envs/trnascan.yaml
+-rw-r--r--   0 fall      (1000) fall      (1000)      228 2024-03-04 09:35:20.000000 monsda-1.2.7/envs/ucsc.yaml
+-rw-r--r--   0 fall      (1000) fall      (1000)      150 2024-03-04 09:35:20.000000 monsda-1.2.7/envs/umitools.yaml
+-rw-r--r--   0 fall      (1000) fall      (1000)      106 2024-03-04 09:35:20.000000 monsda-1.2.7/envs/zip.yaml
+drwxr-xr-x   0 fall      (1000) fall      (1000)        0 2024-06-03 08:00:02.976457 monsda-1.2.7/profile_nextflow/
+-rw-r--r--   0 fall      (1000) fall      (1000)      217 2024-03-27 11:17:58.000000 monsda-1.2.7/profile_nextflow/nextflow.config
+drwxr-xr-x   0 fall      (1000) fall      (1000)        0 2024-06-03 08:00:02.983457 monsda-1.2.7/profile_snakemake/
+-rw-r--r--   0 fall      (1000) fall      (1000)      344 2024-03-04 09:35:20.000000 monsda-1.2.7/profile_snakemake/cluster_config.yaml
+-rw-r--r--   0 fall      (1000) fall      (1000)      277 2024-03-04 09:35:20.000000 monsda-1.2.7/profile_snakemake/config.yaml
+-rwxr-xr-x   0 fall      (1000) fall      (1000)       51 2024-03-04 09:35:20.000000 monsda-1.2.7/profile_snakemake/slurm-jobscript.sh
+-rwxr-xr-x   0 fall      (1000) fall      (1000)     1826 2024-03-04 09:35:20.000000 monsda-1.2.7/profile_snakemake/slurm-status.py
+-rwxr-xr-x   0 fall      (1000) fall      (1000)    10397 2024-03-04 09:35:20.000000 monsda-1.2.7/profile_snakemake/slurm-submit-advanced.py
+-rwxr-xr-x   0 fall      (1000) fall      (1000)     1880 2024-03-04 09:35:20.000000 monsda-1.2.7/profile_snakemake/slurm-submit.py
+-rw-r--r--   0 fall      (1000) fall      (1000)    10495 2024-03-04 09:35:20.000000 monsda-1.2.7/profile_snakemake/slurm_utils.py
+-rw-r--r--   0 fall      (1000) fall      (1000)     1303 2024-03-28 12:07:30.000000 monsda-1.2.7/pyproject.toml
+drwxr-xr-x   0 fall      (1000) fall      (1000)        0 2024-06-03 08:00:02.907458 monsda-1.2.7/scripts/
+drwxr-xr-x   0 fall      (1000) fall      (1000)        0 2024-06-03 08:00:02.999457 monsda-1.2.7/scripts/Analysis/
+-rwxr-xr-x   0 fall      (1000) fall      (1000)     2882 2024-03-04 09:35:20.000000 monsda-1.2.7/scripts/Analysis/AddStructure.py
+-rwxr-xr-x   0 fall      (1000) fall      (1000)     3647 2024-03-04 09:35:20.000000 monsda-1.2.7/scripts/Analysis/Cluster2tRNA.py
+-rwxr-xr-x   0 fall      (1000) fall      (1000)    12627 2024-03-04 09:35:20.000000 monsda-1.2.7/scripts/Analysis/CollectBamStat.py
+-rwxr-xr-x   0 fall      (1000) fall      (1000)    25757 2024-03-04 09:35:20.000000 monsda-1.2.7/scripts/Analysis/CountEnds.py
+-rwxr-xr-x   0 fall      (1000) fall      (1000)      490 2024-03-04 09:35:20.000000 monsda-1.2.7/scripts/Analysis/CountFastqEnds.pl
+drwxr-xr-x   0 fall      (1000) fall      (1000)        0 2024-06-03 08:00:03.002457 monsda-1.2.7/scripts/Analysis/DAS/
+-rwxr-xr-x   0 fall      (1000) fall      (1000)    27615 2024-03-04 09:35:20.000000 monsda-1.2.7/scripts/Analysis/DAS/DIEGO.py
+-rwxr-xr-x   0 fall      (1000) fall      (1000)    12133 2024-03-04 09:35:20.000000 monsda-1.2.7/scripts/Analysis/DAS/EDGER.R
+-rwxr-xr-x   0 fall      (1000) fall      (1000)     2108 2024-03-04 09:35:20.000000 monsda-1.2.7/scripts/Analysis/DAS/FeatureCounts2DIEGO.pl
+-rwxr-xr-x   0 fall      (1000) fall      (1000)    13715 2024-03-04 09:35:20.000000 monsda-1.2.7/scripts/Analysis/DAS/FeatureCounts2DIEGO.py
+-rwxr-xr-x   0 fall      (1000) fall      (1000)     4720 2024-03-04 09:35:20.000000 monsda-1.2.7/scripts/Analysis/DAS/diego_contrast_files.py
+drwxr-xr-x   0 fall      (1000) fall      (1000)        0 2024-06-03 08:00:03.004457 monsda-1.2.7/scripts/Analysis/DE/
+-rwxr-xr-x   0 fall      (1000) fall      (1000)    17576 2024-06-03 07:58:25.000000 monsda-1.2.7/scripts/Analysis/DE/DESEQ2.R
+-rwxr-xr-x   0 fall      (1000) fall      (1000)    18169 2024-06-03 07:58:24.000000 monsda-1.2.7/scripts/Analysis/DE/EDGER.R
+drwxr-xr-x   0 fall      (1000) fall      (1000)        0 2024-06-03 08:00:03.007457 monsda-1.2.7/scripts/Analysis/DEU/
+-rwxr-xr-x   0 fall      (1000) fall      (1000)     9059 2024-03-04 09:35:20.000000 monsda-1.2.7/scripts/Analysis/DEU/DEXSEQ.R
+-rwxr-xr-x   0 fall      (1000) fall      (1000)     9938 2024-03-04 09:35:20.000000 monsda-1.2.7/scripts/Analysis/DEU/EDGER.R
+-rwxr-xr-x   0 fall      (1000) fall      (1000)     9611 2024-03-04 09:35:20.000000 monsda-1.2.7/scripts/Analysis/DEU/prepare_deu_annotation.py
+drwxr-xr-x   0 fall      (1000) fall      (1000)        0 2024-06-03 08:00:03.008457 monsda-1.2.7/scripts/Analysis/DTU/
+-rwxr-xr-x   0 fall      (1000) fall      (1000)     7268 2024-03-04 09:35:20.000000 monsda-1.2.7/scripts/Analysis/DTU/DEXSEQ.R
+-rwxr-xr-x   0 fall      (1000) fall      (1000)    14986 2024-03-04 09:35:20.000000 monsda-1.2.7/scripts/Analysis/DTU/DRIMSEQ.R
+-rwxr-xr-x   0 fall      (1000) fall      (1000)     3421 2024-03-04 09:35:20.000000 monsda-1.2.7/scripts/Analysis/FindPeaks.pl
+-rwxr-xr-x   0 fall      (1000) fall      (1000)     2737 2024-03-04 09:35:20.000000 monsda-1.2.7/scripts/Analysis/GOA.R
+-rwxr-xr-x   0 fall      (1000) fall      (1000)    14628 2024-03-04 09:35:20.000000 monsda-1.2.7/scripts/Analysis/GenerateTrackDb.py
+-rwxr-xr-x   0 fall      (1000) fall      (1000)      426 2024-03-04 09:35:20.000000 monsda-1.2.7/scripts/Analysis/GettRNAExpression.sh
+-rwxr-xr-x   0 fall      (1000) fall      (1000)     5106 2024-03-04 09:35:20.000000 monsda-1.2.7/scripts/Analysis/NormalizePeaks.pl
+-rwxr-xr-x   0 fall      (1000) fall      (1000)     5174 2024-03-04 09:35:20.000000 monsda-1.2.7/scripts/Analysis/PlBed2Bedgraph.pl
+-rwxr-xr-x   0 fall      (1000) fall      (1000)     2228 2024-03-04 09:35:20.000000 monsda-1.2.7/scripts/Analysis/PreprocessPeaks.pl
+-rwxr-xr-x   0 fall      (1000) fall      (1000)     8094 2024-03-04 09:35:20.000000 monsda-1.2.7/scripts/Analysis/RemoveSoftClip.py
+-rwxr-xr-x   0 fall      (1000) fall      (1000)    11489 2024-03-04 09:35:20.000000 monsda-1.2.7/scripts/Analysis/RmdCreator.py
+drwxr-xr-x   0 fall      (1000) fall      (1000)        0 2024-06-03 08:00:03.009457 monsda-1.2.7/scripts/Analysis/SUMMARY/
+-rwxr-xr-x   0 fall      (1000) fall      (1000)      408 2024-03-04 09:35:20.000000 monsda-1.2.7/scripts/Analysis/SUMMARY/header_summary.Rmd
+-rwxr-xr-x   0 fall      (1000) fall      (1000)    13324 2024-03-04 09:35:20.000000 monsda-1.2.7/scripts/Analysis/build_DEU_table.py
+-rwxr-xr-x   0 fall      (1000) fall      (1000)    10925 2024-03-04 09:35:20.000000 monsda-1.2.7/scripts/Analysis/build_DTU_table.py
+-rwxr-xr-x   0 fall      (1000) fall      (1000)    14005 2024-03-04 09:35:20.000000 monsda-1.2.7/scripts/Analysis/build_count_table.py
+-rwxr-xr-x   0 fall      (1000) fall      (1000)    11421 2024-03-04 09:35:20.000000 monsda-1.2.7/scripts/Analysis/build_salmon_table.py
+drwxr-xr-x   0 fall      (1000) fall      (1000)        0 2024-06-03 08:00:03.010457 monsda-1.2.7/scripts/Preprocessing/
+-rwxr-xr-x   0 fall      (1000) fall      (1000)      237 2024-03-04 09:35:20.000000 monsda-1.2.7/scripts/Preprocessing/indexfa.sh
+drwxr-xr-x   0 fall      (1000) fall      (1000)        0 2024-06-03 08:00:03.017457 monsda-1.2.7/scripts/Shells/
+-rw-r--r--   0 fall      (1000) fall      (1000)     1754 2024-03-04 09:35:20.000000 monsda-1.2.7/scripts/Shells/MergeExpression_Cufflinks.sh
+-rw-r--r--   0 fall      (1000) fall      (1000)     1620 2024-03-04 09:35:20.000000 monsda-1.2.7/scripts/Shells/MergeExpression_RNAcounter.sh
+-rw-r--r--   0 fall      (1000) fall      (1000)     1517 2024-03-04 09:35:20.000000 monsda-1.2.7/scripts/Shells/MergeGeneExpression_Cufflinks.sh
+-rwxr-xr-x   0 fall      (1000) fall      (1000)      670 2024-03-25 16:31:46.000000 monsda-1.2.7/scripts/Shells/NonUniqueBam_woPicard.sh
+-rwxr-xr-x   0 fall      (1000) fall      (1000)      565 2024-03-15 07:51:51.000000 monsda-1.2.7/scripts/Shells/NonUniqueBam_woPicard.sh~
+-rwxr-xr-x   0 fall      (1000) fall      (1000)      460 2024-03-04 09:35:20.000000 monsda-1.2.7/scripts/Shells/Sam2Bam.sh
+-rwxr-xr-x   0 fall      (1000) fall      (1000)      440 2024-03-04 09:35:20.000000 monsda-1.2.7/scripts/Shells/Sam2Bed.sh
+-rwxr-xr-x   0 fall      (1000) fall      (1000)      966 2024-04-16 12:14:02.000000 monsda-1.2.7/scripts/Shells/UniqueBam_woPicard.sh
+-rwxr-xr-x   0 fall      (1000) fall      (1000)      551 2024-03-15 07:50:55.000000 monsda-1.2.7/scripts/Shells/UniqueBam_woPicard.sh~
+-rwxr-xr-x   0 fall      (1000) fall      (1000)     1628 2024-04-16 12:14:02.000000 monsda-1.2.7/scripts/Shells/UniqueSam_woPicard.sh
+-rwxr-xr-x   0 fall      (1000) fall      (1000)      536 2024-03-04 09:35:20.000000 monsda-1.2.7/scripts/Shells/printEnds.sh
+-rwxr-xr-x   0 fall      (1000) fall      (1000)      342 2024-03-04 09:35:20.000000 monsda-1.2.7/scripts/Shells/printFQEnds.sh
+drwxr-xr-x   0 fall      (1000) fall      (1000)        0 2024-06-03 08:00:03.021457 monsda-1.2.7/scripts/Universal/
+-rwxr-xr-x   0 fall      (1000) fall      (1000)     8806 2024-03-28 12:04:17.000000 monsda-1.2.7/scripts/Universal/AnnotateBed.pl
+-rwxr-xr-x   0 fall      (1000) fall      (1000)     5046 2024-03-04 09:35:20.000000 monsda-1.2.7/scripts/Universal/Bed2Bedgraph.pl
+-rwxr-xr-x   0 fall      (1000) fall      (1000)     8118 2024-03-04 09:35:20.000000 monsda-1.2.7/scripts/Universal/ExtendBed.pl
+-rw-r--r--   0 fall      (1000) fall      (1000)     2303 2024-03-04 09:35:20.000000 monsda-1.2.7/scripts/Universal/countCCA.pl
+-rw-r--r--   0 fall      (1000) fall      (1000)      710 2024-03-04 09:35:20.000000 monsda-1.2.7/scripts/Universal/sam2fastq.pl
+drwxr-xr-x   0 fall      (1000) fall      (1000)        0 2024-06-03 08:00:03.024457 monsda-1.2.7/scripts/lib/
+-rwxr-xr-x   0 fall      (1000) fall      (1000)    67149 2024-03-04 09:35:20.000000 monsda-1.2.7/scripts/lib/Collection.pm
+-rwxr-xr-x   0 fall      (1000) fall      (1000)     3227 2024-03-04 09:35:20.000000 monsda-1.2.7/scripts/lib/Logger.py
+-rw-r--r--   0 fall      (1000) fall      (1000)        0 2024-03-04 09:35:20.000000 monsda-1.2.7/scripts/lib/__init.py__
+-rw-r--r--   0 fall      (1000) fall      (1000)     1565 2024-06-03 07:27:29.000000 monsda-1.2.7/scripts/lib/_lib.R
+-rw-r--r--   0 fall      (1000) fall      (1000)      648 2024-06-03 08:00:03.113455 monsda-1.2.7/setup.cfg
+-rw-r--r--   0 fall      (1000) fall      (1000)     3297 2024-03-26 16:29:05.000000 monsda-1.2.7/setup.py
+drwxr-xr-x   0 fall      (1000) fall      (1000)        0 2024-06-03 08:00:03.025457 monsda-1.2.7/tests/
+-rwxr-xr-x   0 fall      (1000) fall      (1000)     3454 2024-03-25 16:31:46.000000 monsda-1.2.7/tests/test_functions.py
+-rw-r--r--   0 fall      (1000) fall      (1000)    78254 2024-03-04 09:35:20.000000 monsda-1.2.7/versioneer.py
+drwxr-xr-x   0 fall      (1000) fall      (1000)        0 2024-06-03 08:00:03.103456 monsda-1.2.7/workflows/
+-rw-r--r--   0 fall      (1000) fall      (1000)     7289 2024-03-04 09:35:20.000000 monsda-1.2.7/workflows/annotatebed.smk
+-rw-r--r--   0 fall      (1000) fall      (1000)     2023 2024-03-04 09:35:20.000000 monsda-1.2.7/workflows/bbduk.nf
+-rw-r--r--   0 fall      (1000) fall      (1000)     2713 2024-03-04 09:35:20.000000 monsda-1.2.7/workflows/bbduk.smk
+-rw-r--r--   0 fall      (1000) fall      (1000)     3857 2024-03-04 09:35:20.000000 monsda-1.2.7/workflows/bwa.nf
+-rw-r--r--   0 fall      (1000) fall      (1000)    14226 2024-03-04 09:35:20.000000 monsda-1.2.7/workflows/bwa.smk
+-rw-r--r--   0 fall      (1000) fall      (1000)     3846 2024-03-04 09:35:20.000000 monsda-1.2.7/workflows/bwa2.nf
+-rw-r--r--   0 fall      (1000) fall      (1000)     3499 2024-03-04 09:35:20.000000 monsda-1.2.7/workflows/bwa2.smk
+-rw-r--r--   0 fall      (1000) fall      (1000)     4232 2024-03-04 09:35:20.000000 monsda-1.2.7/workflows/bwameth.nf
+-rw-r--r--   0 fall      (1000) fall      (1000)     3360 2024-03-04 09:35:20.000000 monsda-1.2.7/workflows/bwameth.smk
+-rw-r--r--   0 fall      (1000) fall      (1000)     2050 2024-03-04 09:35:20.000000 monsda-1.2.7/workflows/ciri2.nf
+-rw-r--r--   0 fall      (1000) fall      (1000)     1816 2024-03-04 09:35:20.000000 monsda-1.2.7/workflows/ciri2.smk
+-rw-r--r--   0 fall      (1000) fall      (1000)      507 2024-03-04 09:35:20.000000 monsda-1.2.7/workflows/collect.nf
+-rw-r--r--   0 fall      (1000) fall      (1000)     9861 2024-03-04 09:35:20.000000 monsda-1.2.7/workflows/countreads.nf
+-rw-r--r--   0 fall      (1000) fall      (1000)    15432 2024-03-04 09:35:20.000000 monsda-1.2.7/workflows/countreads.smk
+-rw-r--r--   0 fall      (1000) fall      (1000)     2243 2024-03-04 09:35:20.000000 monsda-1.2.7/workflows/cutadapt.nf
+-rw-r--r--   0 fall      (1000) fall      (1000)     2934 2024-03-04 09:35:20.000000 monsda-1.2.7/workflows/cutadapt.smk
+-rw-r--r--   0 fall      (1000) fall      (1000)     7456 2024-03-04 09:35:20.000000 monsda-1.2.7/workflows/deseq2_DE.nf
+-rw-r--r--   0 fall      (1000) fall      (1000)     8187 2024-05-31 13:11:49.000000 monsda-1.2.7/workflows/deseq2_DE.smk
+-rw-r--r--   0 fall      (1000) fall      (1000)     9193 2024-03-04 09:35:20.000000 monsda-1.2.7/workflows/dexseq_DEU.nf
+-rw-r--r--   0 fall      (1000) fall      (1000)     8476 2024-03-04 09:35:20.000000 monsda-1.2.7/workflows/dexseq_DEU.smk
+-rw-r--r--   0 fall      (1000) fall      (1000)     8100 2024-03-04 09:35:20.000000 monsda-1.2.7/workflows/dexseq_DTU.nf
+-rw-r--r--   0 fall      (1000) fall      (1000)    10062 2024-03-04 09:35:20.000000 monsda-1.2.7/workflows/dexseq_DTU.smk
+-rw-r--r--   0 fall      (1000) fall      (1000)     9334 2024-03-04 09:35:20.000000 monsda-1.2.7/workflows/diego_DAS.nf
+-rw-r--r--   0 fall      (1000) fall      (1000)     8157 2024-03-04 09:35:20.000000 monsda-1.2.7/workflows/diego_DAS.smk
+-rw-r--r--   0 fall      (1000) fall      (1000)     1394 2024-03-04 09:35:20.000000 monsda-1.2.7/workflows/dorado.nf
+-rw-r--r--   0 fall      (1000) fall      (1000)     1262 2024-03-04 09:35:20.000000 monsda-1.2.7/workflows/dorado.smk
+-rw-r--r--   0 fall      (1000) fall      (1000)     8123 2024-03-04 09:35:20.000000 monsda-1.2.7/workflows/drimseq_DTU.nf
+-rw-r--r--   0 fall      (1000) fall      (1000)    13421 2024-03-04 09:35:20.000000 monsda-1.2.7/workflows/drimseq_DTU.smk
+-rw-r--r--   0 fall      (1000) fall      (1000)     7763 2024-03-04 09:35:20.000000 monsda-1.2.7/workflows/edger_DAS.nf
+-rw-r--r--   0 fall      (1000) fall      (1000)     7887 2024-03-04 09:35:20.000000 monsda-1.2.7/workflows/edger_DAS.smk
+-rw-r--r--   0 fall      (1000) fall      (1000)     7631 2024-03-04 09:35:20.000000 monsda-1.2.7/workflows/edger_DE.nf
+-rw-r--r--   0 fall      (1000) fall      (1000)     8052 2024-05-31 13:12:10.000000 monsda-1.2.7/workflows/edger_DE.smk
+-rw-r--r--   0 fall      (1000) fall      (1000)     7681 2024-03-04 09:35:20.000000 monsda-1.2.7/workflows/edger_DEU.nf
+-rw-r--r--   0 fall      (1000) fall      (1000)     7668 2024-03-04 09:35:20.000000 monsda-1.2.7/workflows/edger_DEU.smk
+-rw-r--r--   0 fall      (1000) fall      (1000)     3191 2024-03-04 09:35:20.000000 monsda-1.2.7/workflows/fastqc.nf
+-rw-r--r--   0 fall      (1000) fall      (1000)     5830 2024-03-04 09:35:20.000000 monsda-1.2.7/workflows/fastqc.smk
+-rw-r--r--   0 fall      (1000) fall      (1000)     2040 2024-03-04 09:35:20.000000 monsda-1.2.7/workflows/fastqc_dedup.nf
+-rw-r--r--   0 fall      (1000) fall      (1000)     4596 2024-03-04 09:35:20.000000 monsda-1.2.7/workflows/fastqc_dedup.smk
+-rw-r--r--   0 fall      (1000) fall      (1000)     2851 2024-03-04 09:35:20.000000 monsda-1.2.7/workflows/fastqc_dedup_trim.nf
+-rw-r--r--   0 fall      (1000) fall      (1000)     5978 2024-03-04 09:35:20.000000 monsda-1.2.7/workflows/fastqc_dedup_trim.smk
+-rw-r--r--   0 fall      (1000) fall      (1000)      860 2024-03-04 09:35:20.000000 monsda-1.2.7/workflows/fastqc_raw.nf
+-rw-r--r--   0 fall      (1000) fall      (1000)     2901 2024-03-04 09:35:20.000000 monsda-1.2.7/workflows/fastqc_raw.smk
+-rw-r--r--   0 fall      (1000) fall      (1000)     2069 2024-03-04 09:35:20.000000 monsda-1.2.7/workflows/fastqc_trim.nf
+-rw-r--r--   0 fall      (1000) fall      (1000)     4661 2024-03-04 09:35:20.000000 monsda-1.2.7/workflows/fastqc_trim.smk
+-rw-r--r--   0 fall      (1000) fall      (1000)       91 2024-03-04 09:35:20.000000 monsda-1.2.7/workflows/footer.nf
+-rw-r--r--   0 fall      (1000) fall      (1000)       90 2024-03-04 09:35:20.000000 monsda-1.2.7/workflows/footer.smk
+-rw-r--r--   0 fall      (1000) fall      (1000)     1788 2024-03-04 09:35:20.000000 monsda-1.2.7/workflows/guppy.nf
+-rw-r--r--   0 fall      (1000) fall      (1000)     1661 2024-03-04 09:35:20.000000 monsda-1.2.7/workflows/guppy.smk
+-rw-r--r--   0 fall      (1000) fall      (1000)     1609 2024-03-04 09:35:20.000000 monsda-1.2.7/workflows/header.nf
+-rw-r--r--   0 fall      (1000) fall      (1000)    12190 2024-03-04 09:35:20.000000 monsda-1.2.7/workflows/header.smk
+-rw-r--r--   0 fall      (1000) fall      (1000)     4459 2024-03-04 09:35:20.000000 monsda-1.2.7/workflows/hisat2.nf
+-rw-r--r--   0 fall      (1000) fall      (1000)     4844 2024-03-04 09:35:20.000000 monsda-1.2.7/workflows/hisat2.smk
+-rw-r--r--   0 fall      (1000) fall      (1000)     7366 2024-03-04 09:35:20.000000 monsda-1.2.7/workflows/macs.nf
+-rw-r--r--   0 fall      (1000) fall      (1000)    14219 2024-03-04 09:35:20.000000 monsda-1.2.7/workflows/macs.smk
+-rw-r--r--   0 fall      (1000) fall      (1000)     2372 2024-03-04 09:35:20.000000 monsda-1.2.7/workflows/manipulate_genome.nf
+-rw-r--r--   0 fall      (1000) fall      (1000)     2359 2024-03-04 09:35:20.000000 monsda-1.2.7/workflows/manipulate_genome.smk
+-rw-r--r--   0 fall      (1000) fall      (1000)     4247 2024-03-04 09:35:20.000000 monsda-1.2.7/workflows/mapping.nf
+-rw-r--r--   0 fall      (1000) fall      (1000)     2698 2024-03-04 09:35:20.000000 monsda-1.2.7/workflows/mapping.smk
+-rw-r--r--   0 fall      (1000) fall      (1000)     3854 2024-03-04 09:35:20.000000 monsda-1.2.7/workflows/minimap.nf
+-rw-r--r--   0 fall      (1000) fall      (1000)     2968 2024-03-04 09:35:20.000000 monsda-1.2.7/workflows/minimap.smk
+-rw-r--r--   0 fall      (1000) fall      (1000)     1022 2024-03-04 09:35:20.000000 monsda-1.2.7/workflows/multiqc.nf
+-rw-r--r--   0 fall      (1000) fall      (1000)    10636 2024-03-04 09:35:20.000000 monsda-1.2.7/workflows/multiqc.smk
+-rw-r--r--   0 fall      (1000) fall      (1000)     5667 2024-03-04 09:35:20.000000 monsda-1.2.7/workflows/notify.nf
+-rw-r--r--   0 fall      (1000) fall      (1000)    11912 2024-03-04 09:35:20.000000 monsda-1.2.7/workflows/peaks.nf
+-rw-r--r--   0 fall      (1000) fall      (1000)    21080 2024-05-29 11:14:58.000000 monsda-1.2.7/workflows/peaks.smk
+-rw-r--r--   0 fall      (1000) fall      (1000)     1797 2024-03-04 09:35:20.000000 monsda-1.2.7/workflows/picard_dedup.nf
+-rw-r--r--   0 fall      (1000) fall      (1000)     1250 2024-03-04 09:35:20.000000 monsda-1.2.7/workflows/picard_dedup.smk
+-rw-r--r--   0 fall      (1000) fall      (1000)    12177 2024-03-04 09:35:20.000000 monsda-1.2.7/workflows/piranha.nf
+-rw-r--r--   0 fall      (1000) fall      (1000)    20531 2024-05-29 11:15:15.000000 monsda-1.2.7/workflows/piranha.smk
+-rw-r--r--   0 fall      (1000) fall      (1000)     1150 2024-03-04 09:35:20.000000 monsda-1.2.7/workflows/premultiqc.nf
+-rw-r--r--   0 fall      (1000) fall      (1000)     1557 2024-03-04 09:35:20.000000 monsda-1.2.7/workflows/premultiqc.smk
+-rw-r--r--   0 fall      (1000) fall      (1000)     5313 2024-03-04 09:35:20.000000 monsda-1.2.7/workflows/salmon.nf
+-rw-r--r--   0 fall      (1000) fall      (1000)     3679 2024-03-04 09:35:20.000000 monsda-1.2.7/workflows/salmon.smk
+-rw-r--r--   0 fall      (1000) fall      (1000)     4997 2024-03-04 09:35:20.000000 monsda-1.2.7/workflows/salmon_trim.smk
+-rw-r--r--   0 fall      (1000) fall      (1000)    22666 2024-03-04 09:35:20.000000 monsda-1.2.7/workflows/scyphy.nf
+-rw-r--r--   0 fall      (1000) fall      (1000)    32938 2024-03-04 09:35:20.000000 monsda-1.2.7/workflows/scyphy.smk
+-rw-r--r--   0 fall      (1000) fall      (1000)     3881 2024-03-04 09:35:20.000000 monsda-1.2.7/workflows/segemehl.nf
+-rw-r--r--   0 fall      (1000) fall      (1000)     3098 2024-03-04 09:35:20.000000 monsda-1.2.7/workflows/segemehl.smk
+-rw-r--r--   0 fall      (1000) fall      (1000)     4378 2024-03-04 09:35:20.000000 monsda-1.2.7/workflows/segemehl3.nf
+-rw-r--r--   0 fall      (1000) fall      (1000)     4699 2024-03-04 09:35:20.000000 monsda-1.2.7/workflows/segemehl3.smk
+-rw-r--r--   0 fall      (1000) fall      (1000)     4613 2024-03-04 09:35:20.000000 monsda-1.2.7/workflows/segemehl3_bisulfite.nf
+-rw-r--r--   0 fall      (1000) fall      (1000)     3695 2024-03-04 09:35:20.000000 monsda-1.2.7/workflows/segemehl3_bisulfite.smk
+-rw-r--r--   0 fall      (1000) fall      (1000)     4681 2024-03-04 09:35:20.000000 monsda-1.2.7/workflows/segemehl_bisulfite.nf
+-rw-r--r--   0 fall      (1000) fall      (1000)     3848 2024-03-04 09:35:20.000000 monsda-1.2.7/workflows/segemehl_bisulfite.smk
+-rw-r--r--   0 fall      (1000) fall      (1000)     1719 2024-03-04 09:35:20.000000 monsda-1.2.7/workflows/simulatetrim.nf
+-rw-r--r--   0 fall      (1000) fall      (1000)     1425 2024-03-04 09:35:20.000000 monsda-1.2.7/workflows/simulatetrim.smk
+-rw-r--r--   0 fall      (1000) fall      (1000)     2017 2024-03-04 09:35:20.000000 monsda-1.2.7/workflows/sra.nf
+-rw-r--r--   0 fall      (1000) fall      (1000)     3905 2024-03-04 09:35:20.000000 monsda-1.2.7/workflows/sra.smk
+-rw-r--r--   0 fall      (1000) fall      (1000)     6531 2024-03-25 16:31:46.000000 monsda-1.2.7/workflows/star.nf
+-rw-r--r--   0 fall      (1000) fall      (1000)     8723 2024-03-25 16:31:46.000000 monsda-1.2.7/workflows/star.smk
+-rw-r--r--   0 fall      (1000) fall      (1000)     1190 2024-03-04 09:35:20.000000 monsda-1.2.7/workflows/summary.nf
+-rw-r--r--   0 fall      (1000) fall      (1000)      857 2024-03-04 09:35:20.000000 monsda-1.2.7/workflows/summary.smk
+-rw-r--r--   0 fall      (1000) fall      (1000)     2028 2024-03-04 09:35:20.000000 monsda-1.2.7/workflows/trimgalore.nf
+-rw-r--r--   0 fall      (1000) fall      (1000)     3378 2024-03-04 09:35:20.000000 monsda-1.2.7/workflows/trimgalore.smk
+-rw-r--r--   0 fall      (1000) fall      (1000)     7481 2024-03-04 09:35:20.000000 monsda-1.2.7/workflows/ucsc.nf
+-rw-r--r--   0 fall      (1000) fall      (1000)     8139 2024-03-04 09:35:20.000000 monsda-1.2.7/workflows/ucsc.smk
+-rw-r--r--   0 fall      (1000) fall      (1000)     4093 2024-03-04 09:35:20.000000 monsda-1.2.7/workflows/umitools.nf
+-rw-r--r--   0 fall      (1000) fall      (1000)     7717 2024-03-04 09:35:20.000000 monsda-1.2.7/workflows/umitools.smk
+-rw-r--r--   0 fall      (1000) fall      (1000)     1656 2024-03-04 09:35:20.000000 monsda-1.2.7/workflows/umitools_dedup.nf
+-rw-r--r--   0 fall      (1000) fall      (1000)        1 2024-03-04 09:35:20.000000 monsda-1.2.7/workflows/unlock.smk
```

### Comparing `monsda-1.2.6/LICENSE` & `monsda-1.2.7/LICENSE`

 * *Files identical despite different names*

### Comparing `monsda-1.2.6/MONSDA/Configurator.py` & `monsda-1.2.7/MONSDA/Configurator.py`

 * *Files identical despite different names*

### Comparing `monsda-1.2.6/MONSDA/Deprecated.py` & `monsda-1.2.7/MONSDA/Deprecated.py`

 * *Files identical despite different names*

### Comparing `monsda-1.2.6/MONSDA/Logger.py` & `monsda-1.2.7/MONSDA/Logger.py`

 * *Files identical despite different names*

### Comparing `monsda-1.2.6/MONSDA/Params.py` & `monsda-1.2.7/MONSDA/Params.py`

 * *Files identical despite different names*

### Comparing `monsda-1.2.6/MONSDA/RunMONSDA.py` & `monsda-1.2.7/MONSDA/RunMONSDA.py`

 * *Files 2% similar despite different names*

```diff
@@ -295,15 +295,15 @@
                     jobstorun = list()
 
                     for job in jobs:
                         smko, confo = job
                         rest = " ".join(argslist)
 
                         jobstorun.append(
-                            f"snakemake -j {threads} --software-deployment-method conda -s {smko} --configfile {confo} --directory {workdir} --printshellcmds --show-failed-logs {rest}"
+                            f"snakemake -j {threads} -s {smko} --configfile {confo} --directory {workdir} --printshellcmds --show-failed-logs {rest}"
                         )
 
                     for job in jobstorun:
                         with open("JOBS" + os.sep + scriptname + ".commands", "a") as j:
                             j.write(job + os.linesep)
                         if not save:
                             log.info(logid + "RUNNING " + str(job))
@@ -336,15 +336,15 @@
             jobstorun = list()
 
             for job in jobs:
                 smko, confo = job
                 rest = " ".join(argslist)
 
                 jobstorun.append(
-                    f"snakemake -j {threads} --software-deployment-method conda -s {smko} --configfile {confo} --directory {workdir} --printshellcmds --show-failed-logs {rest}"
+                    f"snakemake -j {threads} -s {smko} --configfile {confo} --directory {workdir} --printshellcmds --show-failed-logs {rest}"
                 )
 
             for job in jobstorun:
                 with open("JOBS" + os.sep + scriptname + ".commands", "a") as j:
                     j.write(job + os.linesep)
                     if not save:
                         log.info(logid + "RUNNING " + str(job))
@@ -382,15 +382,15 @@
                 )
                 jobstorun = list()
 
                 for job in jobs:
                     smko, confo = job
                     rest = " ".join(argslist)
                     jobstorun.append(
-                        f"snakemake -j {threads} --software-deployment-method conda -s {smko} --configfile {confo} --directory {workdir} --printshellcmds --show-failed-logs {rest}"
+                        f"snakemake -j {threads} -s {smko} --configfile {confo} --directory {workdir} --printshellcmds --show-failed-logs {rest}"
                     )
 
                 for job in jobstorun:
                     with open("JOBS" + os.sep + scriptname + ".commands", "a") as j:
                         j.write(job + os.linesep)
                         if not save:
                             log.info(logid + "RUNNING " + str(job))
@@ -412,15 +412,15 @@
                 )
                 jobstorun = list()
 
                 for job in jobs:
                     smko, confo = job
                     rest = " ".join(argslist)
                     jobstorun.append(
-                        f"snakemake -j {threads} --software-deployment-method conda -s {smko} --configfile {confo} --directory {workdir} --printshellcmds --show-failed-logs {rest}"
+                        f"snakemake -j {threads} -s {smko} --configfile {confo} --directory {workdir} --printshellcmds --show-failed-logs {rest}"
                     )
 
                 for job in jobstorun:
                     with open("JOBS" + os.sep + scriptname + ".commands", "a") as j:
                         j.write(job + os.linesep)
                         if not save:
                             log.info(logid + "RUNNING " + str(job))
```

### Comparing `monsda-1.2.6/MONSDA/Utils.py` & `monsda-1.2.7/MONSDA/Utils.py`

 * *Files identical despite different names*

### Comparing `monsda-1.2.6/MONSDA/Workflows.py` & `monsda-1.2.7/MONSDA/Workflows.py`

 * *Files identical despite different names*

### Comparing `monsda-1.2.6/MONSDA/lib/Collection.groovy` & `monsda-1.2.7/MONSDA/lib/Collection.groovy`

 * *Files identical despite different names*

### Comparing `monsda-1.2.6/MONSDA.egg-info/PKG-INFO` & `monsda-1.2.7/MONSDA.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: MONSDA
-Version: 1.2.6
+Version: 1.2.7
 Summary: MONSDA, Modular Organizer of Nextflow and Snakemake driven hts Data Analysis
 Home-page: https://github.com/jfallmann/MONSDA
 Author: Joerg Fallmann
 Author-email: Joerg Fallmann <fallmann.joerg@gmail.com>
 Maintainer-email: Joerg Fallmann <fallmann.joerg@gmail.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
```

### Comparing `monsda-1.2.6/MONSDA.egg-info/SOURCES.txt` & `monsda-1.2.7/MONSDA.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `monsda-1.2.6/PKG-INFO` & `monsda-1.2.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: MONSDA
-Version: 1.2.6
+Version: 1.2.7
 Summary: MONSDA, Modular Organizer of Nextflow and Snakemake driven hts Data Analysis
 Home-page: https://github.com/jfallmann/MONSDA
 Author: Joerg Fallmann
 Author-email: Joerg Fallmann <fallmann.joerg@gmail.com>
 Maintainer-email: Joerg Fallmann <fallmann.joerg@gmail.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
```

### Comparing `monsda-1.2.6/README.md` & `monsda-1.2.7/README.md`

 * *Files identical despite different names*

### Comparing `monsda-1.2.6/configs/template.json` & `monsda-1.2.7/configs/template.json`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 {
     "WORKFLOWS": "", #which workflows do you want to run "MAPPING, QC, DEDUP, TRIMMING, COUNTING, TRACKS, PEAKS, DE, DEU, DAS, DTU, CIRCS"
     "BINS": "", #where to find customscripts used in the workflow !!!ADVANCED USAGE ONLY!!!
     "MAXTHREADS": "20", #maximum number of cores to use, make sure this fits your needs
-    "VERSION": "1.2.6", #needs to be identical to the installed version for reproducibility reasons
+    "VERSION": "1.2.7", #needs to be identical to the installed version for reproducibility reasons
     "SETTINGS": {
         "id": {
             "condition": {
                 "setting": {
                     "SAMPLES": ["Sample_1","Sample_2"] # List of samples you whish to analyze; skip file ending, this names will be used for input/output files of various formats; if paired sequencing make sure the names have _R1/_R2 as identifiers of first/second in pair at the very end of the filename and only list one file without the _R1/_R2 extension, this will be appended automatically
                     "SEQUENCING": "single",  #or paired and stranded (rf,fr) info comma separated
                     "REFERENCE": "GENOMES/Dm6/dm6.fa.gz",  #default Referene Genome fa.gz file
```

### Comparing `monsda-1.2.6/configs/template_base_commented.json` & `monsda-1.2.7/configs/template_base_commented.json`

 * *Files identical despite different names*

### Comparing `monsda-1.2.6/configs/template_clean.json` & `monsda-1.2.7/configs/template_clean.json`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 {
   "WORKFLOWS": "",
   "BINS": "",
   "MAXTHREADS": "20",
-  "VERSION": "1.2.6",
+  "VERSION": "1.2.7",
   "SETTINGS": {
     "id": {
       "condition": {
         "SAMPLES": [
           "rep_1",
           "rep_2"
         ],
```

### Comparing `monsda-1.2.6/configs/tutorial_exhaustive.json` & `monsda-1.2.7/configs/tutorial_exhaustive.json`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 {
     "WORKFLOWS": "FETCH, QC, TRIMMING, MAPPING, DEDUP, TRACKS, PEAKS, DE, DEU, DAS, DTU, COUNTING",
-    "VERSION": "1.2.6",
+    "VERSION": "1.2.7",
     "BINS": "",
     "MAXTHREADS": "16",
     "SETTINGS": {
         "Ecoli": {
             "WT": {
                 "dummylevel": {
                     "SAMPLES": [
```

### Comparing `monsda-1.2.6/configs/tutorial_postprocess.json` & `monsda-1.2.7/configs/tutorial_postprocess.json`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 {
     "WORKFLOWS": "FETCH, QC, TRIMMING, MAPPING, DEDUP, TRACKS, PEAKS, DE, DEU, COUNTING",
-    "VERSION": "1.2.6",
+    "VERSION": "1.2.7",
     "BINS": "",
     "MAXTHREADS": "16",
     "SETTINGS": {
         "Ecoli": {
             "WT": {
                 "dummylevel": {
                     "SAMPLES": [
```

### Comparing `monsda-1.2.6/configs/tutorial_quick.json` & `monsda-1.2.7/configs/tutorial_quick.json`

 * *Files 10% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9285714285714286%*

 * *Differences: {"'VERSION'": "'1.2.7'"}*

```diff
@@ -37,10 +37,10 @@
             "REFERENCE": "GENOMES/Ecoli/ecoli.fa.gz",
             "SAMPLES": [
                 "SRR16324019"
             ],
             "SEQUENCING": "paired"
         }
     },
-    "VERSION": "1.2.6",
+    "VERSION": "1.2.7",
     "WORKFLOWS": "FETCH,MAPPING"
 }
```

### Comparing `monsda-1.2.6/configs/tutorial_toolmix.json` & `monsda-1.2.7/configs/tutorial_toolmix.json`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 {
     "WORKFLOWS": "FETCH, QC, TRIMMING, MAPPING, DEDUP",
-    "VERSION": "1.2.6",
+    "VERSION": "1.2.7",
     "BINS": "",
     "MAXTHREADS": "16",
     "SETTINGS": {
         "Ecoli": {
             "WT": {   
                 "dummylevel": {       
                     "SAMPLES": [
```

### Comparing `monsda-1.2.6/envs/LoveSonesonPatro.yaml` & `monsda-1.2.7/envs/LoveSonesonPatro.yaml`

 * *Files identical despite different names*

### Comparing `monsda-1.2.6/envs/deseq2_DE.yaml` & `monsda-1.2.7/envs/deseq2_DE.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 name: deseq2
 channels:
   - conda-forge
   - bioconda
   - defaults
-  - r
 dependencies:
   - bioconductor-annotate =1.70.0
   - bioconductor-annotationdbi =1.54.0
   - bioconductor-apeglm =1.14.0
   - bioconductor-aroma.light =3.22.0
   - bioconductor-biobase =2.52.0
   - bioconductor-biocfilecache =2.0.0
@@ -34,14 +33,15 @@
   - bioconductor-rhtslib =1.24.0
   - bioconductor-rsamtools =2.8.0
   - bioconductor-rtracklayer =1.52.0
   - bioconductor-ruvseq =1.26.0
   - bioconductor-s4vectors =0.30.0
   - bioconductor-shortread =1.50.0
   - bioconductor-summarizedexperiment =1.22.0
+  - bioconductor-enhancedvolcano 
   - bioconductor-xvector =0.32.0
   - bioconductor-zlibbioc =1.38.0
   - pigz =2.6
   - r-acepack =1.4.1
   - r-askpass =1.1
   - r-assertthat =0.2.1
   - r-backports =1.2.1
```

### Comparing `monsda-1.2.6/envs/dexseq_DEU.yaml` & `monsda-1.2.7/envs/dexseq_DEU.yaml`

 * *Files identical despite different names*

### Comparing `monsda-1.2.6/envs/dexseq_DTU.yaml` & `monsda-1.2.7/envs/dexseq_DTU.yaml`

 * *Files identical despite different names*

### Comparing `monsda-1.2.6/envs/drimseq_DTU.yaml` & `monsda-1.2.7/envs/drimseq_DTU.yaml`

 * *Files identical despite different names*

### Comparing `monsda-1.2.6/envs/edger_DAS.yaml` & `monsda-1.2.7/envs/edger_DAS.yaml`

 * *Files identical despite different names*

### Comparing `monsda-1.2.6/envs/edger_DEU.yaml` & `monsda-1.2.7/envs/edger_DEU.yaml`

 * *Files identical despite different names*

### Comparing `monsda-1.2.6/envs/isoformswitchanalyzer.yaml` & `monsda-1.2.7/envs/isoformswitchanalyzer.yaml`

 * *Files identical despite different names*

### Comparing `monsda-1.2.6/envs/monsda.yaml` & `monsda-1.2.7/envs/monsda.yaml`

 * *Files 15% similar despite different names*

```diff
@@ -3,25 +3,25 @@
   - conda-forge
   - bioconda
   - defaults
 dependencies:
   - biopython=1.83
   - grep >=3.4
   - isort=5.13.2
-  - monsda=1.2.6
+  - monsda=1.2.7
   - natsort=8.4.0
-  - nextflow=23.10.1
+  - nextflow=24.04.2
   - numpy=1.26.4
   - pandas=2.2.1
   - perl=5.34.0
   - pip>=24.0
   - python=3.12.2
   - pyyaml=6.0.1
   - scipy=1.12.0
-  - snakemake=8.11.3
+  - snakemake=8.12.0
   - snakemake-executor-plugin-slurm=0.5.0
   - snakemake-executor-plugin-cluster-generic=1.0.9
   - snakemake-interface-common=1.17.2
   - snakemake-interface-executor-plugins=9.1.1
   - snakemake-interface-report-plugins=1.0.0
   - snakemake-interface-storage-plugins=3.2.2
   - snakemake-storage-plugin-s3=0.2.11
```

### Comparing `monsda-1.2.6/envs/peaks.yaml` & `monsda-1.2.7/envs/peaks.yaml`

 * *Files identical despite different names*

### Comparing `monsda-1.2.6/envs/perl.yaml` & `monsda-1.2.7/envs/perl.yaml`

 * *Files identical despite different names*

### Comparing `monsda-1.2.6/envs/summary.yaml` & `monsda-1.2.7/envs/summary.yaml`

 * *Files identical despite different names*

### Comparing `monsda-1.2.6/profile_snakemake/slurm-status.py` & `monsda-1.2.7/profile_snakemake/slurm-status.py`

 * *Files identical despite different names*

### Comparing `monsda-1.2.6/profile_snakemake/slurm-submit-advanced.py` & `monsda-1.2.7/profile_snakemake/slurm-submit-advanced.py`

 * *Files identical despite different names*

### Comparing `monsda-1.2.6/profile_snakemake/slurm-submit.py` & `monsda-1.2.7/profile_snakemake/slurm-submit.py`

 * *Files identical despite different names*

### Comparing `monsda-1.2.6/profile_snakemake/slurm_utils.py` & `monsda-1.2.7/profile_snakemake/slurm_utils.py`

 * *Files identical despite different names*

### Comparing `monsda-1.2.6/pyproject.toml` & `monsda-1.2.7/pyproject.toml`

 * *Files identical despite different names*

### Comparing `monsda-1.2.6/scripts/Analysis/AddStructure.py` & `monsda-1.2.7/scripts/Analysis/AddStructure.py`

 * *Files identical despite different names*

### Comparing `monsda-1.2.6/scripts/Analysis/Cluster2tRNA.py` & `monsda-1.2.7/scripts/Analysis/Cluster2tRNA.py`

 * *Files identical despite different names*

### Comparing `monsda-1.2.6/scripts/Analysis/CollectBamStat.py` & `monsda-1.2.7/scripts/Analysis/CollectBamStat.py`

 * *Files identical despite different names*

### Comparing `monsda-1.2.6/scripts/Analysis/CountEnds.py` & `monsda-1.2.7/scripts/Analysis/CountEnds.py`

 * *Files identical despite different names*

### Comparing `monsda-1.2.6/scripts/Analysis/DAS/DIEGO.py` & `monsda-1.2.7/scripts/Analysis/DAS/DIEGO.py`

 * *Files identical despite different names*

### Comparing `monsda-1.2.6/scripts/Analysis/DAS/EDGER.R` & `monsda-1.2.7/scripts/Analysis/DAS/EDGER.R`

 * *Files identical despite different names*

### Comparing `monsda-1.2.6/scripts/Analysis/DAS/FeatureCounts2DIEGO.pl` & `monsda-1.2.7/scripts/Analysis/DAS/FeatureCounts2DIEGO.pl`

 * *Files identical despite different names*

### Comparing `monsda-1.2.6/scripts/Analysis/DAS/FeatureCounts2DIEGO.py` & `monsda-1.2.7/scripts/Analysis/DAS/FeatureCounts2DIEGO.py`

 * *Files identical despite different names*

### Comparing `monsda-1.2.6/scripts/Analysis/DAS/diego_contrast_files.py` & `monsda-1.2.7/scripts/Analysis/DAS/diego_contrast_files.py`

 * *Files identical despite different names*

### Comparing `monsda-1.2.6/scripts/Analysis/DE/DESEQ2.R` & `monsda-1.2.7/scripts/Analysis/DE/DESEQ2.R`

 * *Files 10% similar despite different names*

```diff
@@ -7,14 +7,15 @@
     require(ggrepel)
     require(ggplot2)
     require(rtracklayer)
     require(RUVSeq)
     require(dplyr)
     require(GenomeInfoDb)
     require(apeglm)
+    require(EnhancedVolcano)
 })
 
 options(echo = TRUE)
 
 ## ARGS
 args <- commandArgs(trailingOnly = TRUE)
 argsLen <- length(args)
@@ -181,19 +182,46 @@
         # add comp object to list for image
         comparison_objs[[contrast_name]] <- res
 
         # sort and output
         resOrdered <- res_shrink[order(res_shrink$log2FoldChange), ]
 
         # # Add gene names  (check how gene_id col is named )
-        resOrdered$Gene <- lapply(rownames(resOrdered), function(x) {
+        resOrdered$Gene <- unlist(lapply(rownames(resOrdered), function(x) {
             get_gene_name(x, gtf_gene)
-        })
+        }))
         resOrdered$Gene_ID <- rownames(resOrdered)
         resOrdered <- resOrdered[, c(7, 6, 1, 2, 3, 4, 5)]
+
+        # plotVolcano
+        pdf(
+            file = paste("Figures/DE", "DESEQ2", combi, contrast_name, "figure_Volcano.pdf", sep = "_"), width = 15, height = 10
+        )
+        print(EnhancedVolcano(resOrdered,
+            lab = rownames(resOrdered),
+            x = "log2FoldChange",
+            y = "padj",
+            title = paste0(contrast_name, "_p005_lfc15", sep = ""),
+            pCutoff = 0.05,
+            FCcutoff = 1.5,
+            pointSize = 3.0,
+            labSize = 5.0,
+            colAlpha = .3,
+            legendLabels = c(
+                "Not sig.", "Log (base 2) FC", "p-value",
+                "p-value & Log (base 2) FC"
+            ),
+            legendPosition = "right",
+            legendLabSize = 10,
+            legendIconSize = 5.0,
+            drawConnectors = TRUE,
+            widthConnectors = 0.75
+        ))
+        dev.off()
+
         resOrdered <- as.data.frame(apply(resOrdered, 2, as.character))
 
         # write the table to a tsv file
         write.table(as.data.frame(resOrdered), gzfile(paste("Tables/DE", "DESEQ2", combi, contrast_name, "table", "results.tsv.gz", sep = "_")), sep = "\t", row.names = FALSE, quote = F)
 
         # sort and output
         res <- resn[order(resn$log2FoldChange), ]
@@ -225,19 +253,45 @@
             listname <- paste(contrast_name, "_norm", sep = "")
             comparison_objs[[listname]] <- res
 
             # sort and output
             resOrdered <- res_shrink[order(res_shrink$log2FoldChange), ]
 
             # # Add gene names  (check how gene_id col is named )
-            resOrdered$Gene <- lapply(rownames(resOrdered), function(x) {
+            resOrdered$Gene <- unlist(lapply(rownames(resOrdered), function(x) {
                 get_gene_name(x, gtf_gene)
-            })
+            }))
             resOrdered$Gene_ID <- rownames(resOrdered)
             resOrdered <- resOrdered[, c(7, 6, 1, 2, 3, 4, 5)]
+
+            # plot Volcano
+            pdf(
+                file = paste("Figures/DE", "DESEQ2", combi, contrast_name, "figure_Volcano_norm.pdf", sep = "_"), width = 15, height = 10
+            )
+            print(EnhancedVolcano(resOrdered,
+                lab = rownames(resOrdered),
+                x = "log2FoldChange",
+                y = "padj",
+                title = paste0(contrast_name, "_p005_lfc15", sep = ""),
+                pCutoff = 0.05,
+                FCcutoff = 1.5,
+                pointSize = 3.0,
+                labSize = 5.0,
+                colAlpha = .3,
+                legendLabels = c(
+                    "Not sig.", "Log (base 2) FC", "p-value",
+                    "p-value & Log (base 2) FC"
+                ),
+                legendPosition = "right",
+                legendLabSize = 10,
+                legendIconSize = 5.0,
+                drawConnectors = TRUE,
+                widthConnectors = 0.75
+            ))
+            dev.off()
             resOrdered <- as.data.frame(apply(resOrdered, 2, as.character))
 
             # write the table to a tsv file
             write.table(as.data.frame(resOrdered), gzfile(paste("Tables/DE", "DESEQ2", combi, contrast_name, "table", "results_norm.tsv.gz", sep = "_")), sep = "\t", row.names = FALSE, quote = F)
 
 
             # sort and output
@@ -253,15 +307,14 @@
             write.table(as.data.frame(res), gzfile(paste("Tables/DE", "DESEQ2", combi, contrast_name, "table", "results_norm_noshrink.tsv.gz", sep = "_")), sep = "\t", row.names = FALSE, quote = F)
 
             # plotMA
             png(paste("Figures/DE", "DESEQ2", combi, contrast_name, "figure", "MA_norm.png", sep = "_"))
             DESeq2::plotMA(res)
             dev.off()
         }
-
         # cleanup
         rm(res, resOrdered)
         print(paste("cleanup done for ", contrast_name, sep = ""))
     })
 }
 
 #### Now plot and print over-all comparisons
```

### Comparing `monsda-1.2.6/scripts/Analysis/DE/EDGER.R` & `monsda-1.2.7/scripts/Analysis/DE/EDGER.R`

 * *Files 4% similar despite different names*

```diff
@@ -2,14 +2,15 @@
     require(utils)
     require(BiocParallel)
     require(edgeR)
     require(rtracklayer)
     require(RUVSeq)
     require(dplyr)
     require(GenomeInfoDb)
+    require(EnhancedVolcano)
 })
 
 options(echo = TRUE)
 
 ## ARGS
 args <- commandArgs(trailingOnly = TRUE)
 argsLen <- length(args)
@@ -238,20 +239,48 @@
         # qlf <- glmQLFTest(fit, contrast=contrast) ## glm quasi-likelihood-F-Test
         AvsB <- makeContrasts(TreatvsUntreat = paste("condition", A, sep = ""), levels = design)
         qlf <- glmQLFTest(fit, contrast = AvsB) ## glm quasi-likelihood-F-Test
         # add comp object to list for image
         comparison_objs[[contrast_name]] <- qlf
 
         # # Add gene names  (check how gene_id col is named )
-        qlf$table$Gene <- lapply(rownames(qlf$table), function(x) {
+        qlf$table$Gene <- unlist(lapply(rownames(qlf$table), function(x) {
             get_gene_name(x, gtf_gene)
-        })
+        }))
         qlf$table$Gene_ID <- rownames(qlf$table)
         res <- qlf$table[, c(6, 5, 2, 1, 3, 4)]
         res$FDR <- p.adjust(res$PValue, method = "BH")
+        rownames(res) <- res$Gene
+
+        # plotVolcano
+        pdf(
+            file = paste("Figures/DE", "EDGER", combi, contrast_name, "figure_Volcano.pdf", sep = "_"), width = 15, height = 10
+        )
+        print(EnhancedVolcano(res,
+            lab = rownames(res),
+            x = "logFC",
+            y = "FDR",
+            title = paste0(contrast_name, "_p005_lfc15", sep = ""),
+            pCutoff = 0.05,
+            FCcutoff = 1.5,
+            pointSize = 3.0,
+            labSize = 5.0,
+            colAlpha = .3,
+            legendLabels = c(
+                "Not sig.", "Log (base 2) FC", "p-value",
+                "p-value & Log (base 2) FC"
+            ),
+            legendPosition = "right",
+            legendLabSize = 10,
+            legendIconSize = 5.0,
+            drawConnectors = TRUE,
+            widthConnectors = 0.75
+        ))
+        dev.off()
+
         res <- as.data.frame(apply(res, 2, as.character))
 
         # create results table
         write.table(as.data.frame(res), gzfile(paste("Tables/DE", "EDGER", combi, contrast_name, "table", "results.tsv.gz", sep = "_")), sep = "\t", quote = F, row.names = FALSE)
 
         # create sorted results Tables
         tops <- topTags(qlf, n = nrow(qlf$table), sort.by = "logFC")
@@ -292,19 +321,48 @@
             # qlf <- glmQLFTest(fit, contrast=contrast) ## glm quasi-likelihood-F-Test
             AvsB <- makeContrasts(TreatvsUntreat = paste("condition", A, sep = ""), levels = design)
             qlf <- glmQLFTest(fit, contrast = AvsB) ## glm quasi-likelihood-F-Test
             # add comp object to list for image
             comparison_objs <- append(comparison_objs, qlf)
 
             # # Add gene names  (check how gene_id col is named )
-            qlf$table$Gene <- lapply(rownames(qlf$table), function(x) {
+            qlf$table$Gene <- unlist(lapply(rownames(qlf$table), function(x) {
                 get_gene_name(x, gtf_gene)
-            })
+            }))
             qlf$table$Gene_ID <- rownames(qlf$table)
             res <- qlf$table[, c(6, 5, 1, 2, 3, 4)]
+            res$FDR <- p.adjust(res$PValue, method = "BH")
+            rownames(res) <- res$Gene
+
+            # plotVolcano
+            pdf(
+                file = paste("Figures/DE", "EDGER", combi, contrast_name, "figure_Volcano_norm.pdf", sep = "_"), width = 15, height = 10
+            )
+            print(EnhancedVolcano(res,
+                lab = rownames(res),
+                x = as.numeric("logFC"),
+                y = as.numeric("FDR"),
+                title = paste0(contrast_name, "_p005_lfc15", sep = ""),
+                pCutoff = 0.05,
+                FCcutoff = 1.5,
+                pointSize = 3.0,
+                labSize = 5.0,
+                colAlpha = .3,
+                legendLabels = c(
+                    "Not sig.", "Log (base 2) FC", "p-value",
+                    "p-value & Log (base 2) FC"
+                ),
+                legendPosition = "right",
+                legendLabSize = 10,
+                legendIconSize = 5.0,
+                drawConnectors = TRUE,
+                widthConnectors = 0.75
+            ))
+            dev.off()
+
             res <- as.data.frame(apply(res, 2, as.character))
 
             # create results table
             write.table(as.data.frame(res), gzfile(paste("Tables/DE", "EDGER", combi, contrast_name, "table", "results_norm.tsv.gz", sep = "_")), sep = "\t", quote = F, row.names = FALSE)
 
             # create sorted results Tables
             tops <- topTags(qlf, n = nrow(qlf$table), sort.by = "logFC")
```

### Comparing `monsda-1.2.6/scripts/Analysis/DEU/DEXSEQ.R` & `monsda-1.2.7/scripts/Analysis/DEU/DEXSEQ.R`

 * *Files identical despite different names*

### Comparing `monsda-1.2.6/scripts/Analysis/DEU/EDGER.R` & `monsda-1.2.7/scripts/Analysis/DEU/EDGER.R`

 * *Files identical despite different names*

### Comparing `monsda-1.2.6/scripts/Analysis/DEU/prepare_deu_annotation.py` & `monsda-1.2.7/scripts/Analysis/DEU/prepare_deu_annotation.py`

 * *Files identical despite different names*

### Comparing `monsda-1.2.6/scripts/Analysis/DTU/DEXSEQ.R` & `monsda-1.2.7/scripts/Analysis/DTU/DEXSEQ.R`

 * *Files identical despite different names*

### Comparing `monsda-1.2.6/scripts/Analysis/DTU/DRIMSEQ.R` & `monsda-1.2.7/scripts/Analysis/DTU/DRIMSEQ.R`

 * *Files identical despite different names*

### Comparing `monsda-1.2.6/scripts/Analysis/FindPeaks.pl` & `monsda-1.2.7/scripts/Analysis/FindPeaks.pl`

 * *Files identical despite different names*

### Comparing `monsda-1.2.6/scripts/Analysis/GOA.R` & `monsda-1.2.7/scripts/Analysis/GOA.R`

 * *Files identical despite different names*

### Comparing `monsda-1.2.6/scripts/Analysis/GenerateTrackDb.py` & `monsda-1.2.7/scripts/Analysis/GenerateTrackDb.py`

 * *Files identical despite different names*

### Comparing `monsda-1.2.6/scripts/Analysis/NormalizePeaks.pl` & `monsda-1.2.7/scripts/Analysis/NormalizePeaks.pl`

 * *Files identical despite different names*

### Comparing `monsda-1.2.6/scripts/Analysis/PlBed2Bedgraph.pl` & `monsda-1.2.7/scripts/Analysis/PlBed2Bedgraph.pl`

 * *Files identical despite different names*

### Comparing `monsda-1.2.6/scripts/Analysis/PreprocessPeaks.pl` & `monsda-1.2.7/scripts/Analysis/PreprocessPeaks.pl`

 * *Files identical despite different names*

### Comparing `monsda-1.2.6/scripts/Analysis/RemoveSoftClip.py` & `monsda-1.2.7/scripts/Analysis/RemoveSoftClip.py`

 * *Files identical despite different names*

### Comparing `monsda-1.2.6/scripts/Analysis/RmdCreator.py` & `monsda-1.2.7/scripts/Analysis/RmdCreator.py`

 * *Files identical despite different names*

### Comparing `monsda-1.2.6/scripts/Analysis/build_DEU_table.py` & `monsda-1.2.7/scripts/Analysis/build_DEU_table.py`

 * *Files identical despite different names*

### Comparing `monsda-1.2.6/scripts/Analysis/build_DTU_table.py` & `monsda-1.2.7/scripts/Analysis/build_DTU_table.py`

 * *Files identical despite different names*

### Comparing `monsda-1.2.6/scripts/Analysis/build_count_table.py` & `monsda-1.2.7/scripts/Analysis/build_count_table.py`

 * *Files identical despite different names*

### Comparing `monsda-1.2.6/scripts/Analysis/build_salmon_table.py` & `monsda-1.2.7/scripts/Analysis/build_salmon_table.py`

 * *Files identical despite different names*

### Comparing `monsda-1.2.6/scripts/Shells/MergeExpression_Cufflinks.sh` & `monsda-1.2.7/scripts/Shells/MergeExpression_Cufflinks.sh`

 * *Files identical despite different names*

### Comparing `monsda-1.2.6/scripts/Shells/MergeExpression_RNAcounter.sh` & `monsda-1.2.7/scripts/Shells/MergeExpression_RNAcounter.sh`

 * *Files identical despite different names*

### Comparing `monsda-1.2.6/scripts/Shells/MergeGeneExpression_Cufflinks.sh` & `monsda-1.2.7/scripts/Shells/MergeGeneExpression_Cufflinks.sh`

 * *Files identical despite different names*

### Comparing `monsda-1.2.6/scripts/Shells/NonUniqueBam_woPicard.sh` & `monsda-1.2.7/scripts/Shells/NonUniqueBam_woPicard.sh`

 * *Files identical despite different names*

### Comparing `monsda-1.2.6/scripts/Shells/NonUniqueBam_woPicard.sh~` & `monsda-1.2.7/scripts/Shells/NonUniqueBam_woPicard.sh~`

 * *Files identical despite different names*

### Comparing `monsda-1.2.6/scripts/Shells/UniqueBam_woPicard.sh` & `monsda-1.2.7/scripts/Shells/UniqueBam_woPicard.sh`

 * *Files identical despite different names*

### Comparing `monsda-1.2.6/scripts/Shells/UniqueBam_woPicard.sh~` & `monsda-1.2.7/scripts/Shells/UniqueBam_woPicard.sh~`

 * *Files identical despite different names*

### Comparing `monsda-1.2.6/scripts/Shells/UniqueSam_woPicard.sh` & `monsda-1.2.7/scripts/Shells/UniqueSam_woPicard.sh`

 * *Files identical despite different names*

### Comparing `monsda-1.2.6/scripts/Shells/printEnds.sh` & `monsda-1.2.7/scripts/Shells/printEnds.sh`

 * *Files identical despite different names*

### Comparing `monsda-1.2.6/scripts/Universal/AnnotateBed.pl` & `monsda-1.2.7/scripts/Universal/AnnotateBed.pl`

 * *Files identical despite different names*

### Comparing `monsda-1.2.6/scripts/Universal/Bed2Bedgraph.pl` & `monsda-1.2.7/scripts/Universal/Bed2Bedgraph.pl`

 * *Files identical despite different names*

### Comparing `monsda-1.2.6/scripts/Universal/ExtendBed.pl` & `monsda-1.2.7/scripts/Universal/ExtendBed.pl`

 * *Files identical despite different names*

### Comparing `monsda-1.2.6/scripts/Universal/countCCA.pl` & `monsda-1.2.7/scripts/Universal/countCCA.pl`

 * *Files identical despite different names*

### Comparing `monsda-1.2.6/scripts/Universal/sam2fastq.pl` & `monsda-1.2.7/scripts/Universal/sam2fastq.pl`

 * *Files identical despite different names*

### Comparing `monsda-1.2.6/scripts/lib/Collection.pm` & `monsda-1.2.7/scripts/lib/Collection.pm`

 * *Files identical despite different names*

### Comparing `monsda-1.2.6/scripts/lib/Logger.py` & `monsda-1.2.7/scripts/lib/Logger.py`

 * *Files identical despite different names*

### Comparing `monsda-1.2.6/setup.cfg` & `monsda-1.2.7/setup.cfg`

 * *Files identical despite different names*

### Comparing `monsda-1.2.6/setup.py` & `monsda-1.2.7/setup.py`

 * *Files identical despite different names*

### Comparing `monsda-1.2.6/tests/test_functions.py` & `monsda-1.2.7/tests/test_functions.py`

 * *Files identical despite different names*

### Comparing `monsda-1.2.6/versioneer.py` & `monsda-1.2.7/versioneer.py`

 * *Files identical despite different names*

### Comparing `monsda-1.2.6/workflows/annotatebed.smk` & `monsda-1.2.7/workflows/annotatebed.smk`

 * *Files identical despite different names*

### Comparing `monsda-1.2.6/workflows/bbduk.nf` & `monsda-1.2.7/workflows/bbduk.nf`

 * *Files identical despite different names*

### Comparing `monsda-1.2.6/workflows/bbduk.smk` & `monsda-1.2.7/workflows/bbduk.smk`

 * *Files identical despite different names*

### Comparing `monsda-1.2.6/workflows/bwa.nf` & `monsda-1.2.7/workflows/bwa.nf`

 * *Files identical despite different names*

### Comparing `monsda-1.2.6/workflows/bwa.smk` & `monsda-1.2.7/workflows/bwa.smk`

 * *Files identical despite different names*

### Comparing `monsda-1.2.6/workflows/bwa2.nf` & `monsda-1.2.7/workflows/bwa2.nf`

 * *Files identical despite different names*

### Comparing `monsda-1.2.6/workflows/bwa2.smk` & `monsda-1.2.7/workflows/bwa2.smk`

 * *Files identical despite different names*

### Comparing `monsda-1.2.6/workflows/bwameth.nf` & `monsda-1.2.7/workflows/bwameth.nf`

 * *Files identical despite different names*

### Comparing `monsda-1.2.6/workflows/bwameth.smk` & `monsda-1.2.7/workflows/bwameth.smk`

 * *Files identical despite different names*

### Comparing `monsda-1.2.6/workflows/ciri2.nf` & `monsda-1.2.7/workflows/ciri2.nf`

 * *Files identical despite different names*

### Comparing `monsda-1.2.6/workflows/ciri2.smk` & `monsda-1.2.7/workflows/ciri2.smk`

 * *Files identical despite different names*

### Comparing `monsda-1.2.6/workflows/countreads.nf` & `monsda-1.2.7/workflows/countreads.nf`

 * *Files identical despite different names*

### Comparing `monsda-1.2.6/workflows/countreads.smk` & `monsda-1.2.7/workflows/countreads.smk`

 * *Files identical despite different names*

### Comparing `monsda-1.2.6/workflows/cutadapt.nf` & `monsda-1.2.7/workflows/cutadapt.nf`

 * *Files identical despite different names*

### Comparing `monsda-1.2.6/workflows/cutadapt.smk` & `monsda-1.2.7/workflows/cutadapt.smk`

 * *Files identical despite different names*

### Comparing `monsda-1.2.6/workflows/deseq2_DE.nf` & `monsda-1.2.7/workflows/deseq2_DE.nf`

 * *Files identical despite different names*

### Comparing `monsda-1.2.6/workflows/deseq2_DE.smk` & `monsda-1.2.7/workflows/deseq2_DE.smk`

 * *Files 1% similar despite different names*

```diff
@@ -7,27 +7,28 @@
 rule themall:
     input:  session = expand("DE/{combo}/DE_DESEQ2_{scombo}_SESSION.gz", combo=combo, scombo=scombo),
             pca  = expand("DE/{combo}/Figures/DE_DESEQ2_{scombo}_DataSet_figure_PCA.png", combo=combo, scombo=scombo),
             rld  = expand("DE/{combo}/Tables/DE_DESEQ2_{scombo}_DataSet_table_rld.tsv.gz", combo=combo, scombo=scombo),
             vsd  = expand("DE/{combo}/Tables/DE_DESEQ2_{scombo}_DataSet_table_vsd.tsv.gz", combo=combo, scombo=scombo),
             tbl  = expand("DE/{combo}/Tables/DE_DESEQ2_{scombo}_{comparison}_table_results.tsv.gz", combo=combo, comparison=compstr, scombo=scombo),
             plot = expand("DE/{combo}/Figures/DE_DESEQ2_{scombo}_{comparison}_figure_MA.png", combo=combo, comparison=compstr, scombo=scombo),
+            vulcan = expand("DE/{combo}/Figures/DE_DESEQ2_{scombo}_{comparison}_figure_Volcano.pdf", combo=combo, comparison=compstr, scombo=scombo),
             vst  = expand("DE/{combo}/Figures/DE_DESEQ2_{scombo}_DataSet_figure_VST-and-log2.png", combo=combo, scombo=scombo),
             heat = expand("DE/{combo}/Figures/DE_DESEQ2_{scombo}_DataSet_figure_heatmap{i}.png", combo=combo,i=[1,2,3,"-samplebysample"], scombo=scombo),
             heats = expand("DE/{combo}/Figures/DE_DESEQ2_{scombo}_DataSet_figure_heatmap-samplebysample.png", combo=combo,i=[1,2,3,"-samplebysample"], scombo=scombo),
             sig   = expand("DE/{combo}/Tables/Sig_DE_DESEQ2_{scombo}_{comparison}_table_results.tsv.gz", combo=combo, comparison=compstr, scombo=scombo),
             sig_d = expand("DE/{combo}/Tables/SigDOWN_DE_DESEQ2_{scombo}_{comparison}_table_results.tsv.gz", combo=combo, comparison=compstr, scombo=scombo),
             sig_u = expand("DE/{combo}/Tables/SigUP_DE_DESEQ2_{scombo}_{comparison}_table_results.tsv.gz", combo=combo, comparison=compstr, scombo=scombo),
             Rmd = expand("REPORTS/SUMMARY/RmdSnippets/{combo}.Rmd", combo=combo)
 
 rule featurecount_unique:
     input:  reads = expand("MAPPED/{scombo}/{{file}}_mapped_sorted_unique.bam", scombo=scombo)
     output: tmp   = temp("DE/{combo}/Featurecounts/{file}_tmp.counts"),
-            tmph = temp("DE/{combo}/Featurecounts/{file}_tmp.head.gz"),
-            tmpc = temp("DE/{combo}/Featurecounts/{file}_tmp.count.gz"),
+            tmph  = temp("DE/{combo}/Featurecounts/{file}_tmp.head.gz"),
+            tmpc  = temp("DE/{combo}/Featurecounts/{file}_tmp.count.gz"),
             cts   = "DE/{combo}/Featurecounts/{file}_mapped_sorted_unique.counts.gz"
     log:    "LOGS/DE/{combo}/{file}_featurecounts_deseq2_unique.log"
     conda:  ""+COUNTENV+".yaml"
     threads: MAXTHREAD
     params: countb = COUNTBIN,
             anno = ANNOTATION,
             cpara = lambda wildcards: tool_params(wildcards.file, None, config, "DE", DEENV.split('_')[0])['OPTIONS'].get('COUNT', ""),
@@ -47,22 +48,23 @@
              bins = BINS
     shell: "{params.bins}/Analysis/build_count_table.py {params.dereps} --table {output.tbl} --anno {output.anno} 2> {log}"
 
 rule run_deseq2:
     input:  cnt  = expand(rules.prepare_count_table.output.tbl, combo=combo, scombo=scombo),
             anno = expand(rules.prepare_count_table.output.anno, combo=combo, scombo=scombo),
     output: session = rules.themall.input.session,
-            pca  = rules.themall.input.pca,
-            rld  = rules.themall.input.rld,
-            vsd  = rules.themall.input.vsd,
-            tbl  = rules.themall.input.tbl,
-            plot = rules.themall.input.plot,
-            vst  = rules.themall.input.vst,
-            heat = rules.themall.input.heat,
-            heats = rules.themall.input.heats
+            pca    = rules.themall.input.pca,
+            rld    = rules.themall.input.rld,
+            vsd    = rules.themall.input.vsd,
+            tbl    = rules.themall.input.tbl,
+            plot   = rules.themall.input.plot,
+            vulcan = rules.themall.input.vulcan,
+            vst    = rules.themall.input.vst,
+            heat   = rules.themall.input.heat,
+            heats  = rules.themall.input.heats
     log:    expand("LOGS/DE/{combo}/run_deseq2.log", combo=combo)
     conda:  ""+DEENV+".yaml"
     threads: int(MAXTHREAD-1) if int(MAXTHREAD-1) >= 1 else 1
     params: bins = str.join(os.sep, [BINS, DEBIN]),
             outdir = 'DE/'+combo,
             compare = comparison,
             pcombo = scombo if scombo != '' else 'none',
@@ -84,14 +86,15 @@
 
 rule create_summary_snippet:
     input:  rules.run_deseq2.output.pca,
             rules.run_deseq2.output.rld,
             rules.run_deseq2.output.vsd,
             rules.run_deseq2.output.tbl,
             rules.run_deseq2.output.plot,
+            rules.run_deseq2.output.vulcan,
             rules.run_deseq2.output.vst,
             rules.run_deseq2.output.heat,
             rules.run_deseq2.output.heats,
             rules.themall.input.session
             # rules.filter_significant.output.sig,
             # rules.filter_significant.output.sig_d,
             # rules.filter_significant.output.sig_u
```

### Comparing `monsda-1.2.6/workflows/dexseq_DEU.nf` & `monsda-1.2.7/workflows/dexseq_DEU.nf`

 * *Files identical despite different names*

### Comparing `monsda-1.2.6/workflows/dexseq_DEU.smk` & `monsda-1.2.7/workflows/dexseq_DEU.smk`

 * *Files identical despite different names*

### Comparing `monsda-1.2.6/workflows/dexseq_DTU.nf` & `monsda-1.2.7/workflows/dexseq_DTU.nf`

 * *Files identical despite different names*

### Comparing `monsda-1.2.6/workflows/dexseq_DTU.smk` & `monsda-1.2.7/workflows/dexseq_DTU.smk`

 * *Files identical despite different names*

### Comparing `monsda-1.2.6/workflows/diego_DAS.nf` & `monsda-1.2.7/workflows/diego_DAS.nf`

 * *Files identical despite different names*

### Comparing `monsda-1.2.6/workflows/diego_DAS.smk` & `monsda-1.2.7/workflows/diego_DAS.smk`

 * *Files identical despite different names*

### Comparing `monsda-1.2.6/workflows/dorado.nf` & `monsda-1.2.7/workflows/dorado.nf`

 * *Files identical despite different names*

### Comparing `monsda-1.2.6/workflows/dorado.smk` & `monsda-1.2.7/workflows/dorado.smk`

 * *Files identical despite different names*

### Comparing `monsda-1.2.6/workflows/drimseq_DTU.nf` & `monsda-1.2.7/workflows/drimseq_DTU.nf`

 * *Files identical despite different names*

### Comparing `monsda-1.2.6/workflows/drimseq_DTU.smk` & `monsda-1.2.7/workflows/drimseq_DTU.smk`

 * *Files identical despite different names*

### Comparing `monsda-1.2.6/workflows/edger_DAS.nf` & `monsda-1.2.7/workflows/edger_DAS.nf`

 * *Files identical despite different names*

### Comparing `monsda-1.2.6/workflows/edger_DAS.smk` & `monsda-1.2.7/workflows/edger_DAS.smk`

 * *Files identical despite different names*

### Comparing `monsda-1.2.6/workflows/edger_DE.nf` & `monsda-1.2.7/workflows/edger_DE.nf`

 * *Files identical despite different names*

### Comparing `monsda-1.2.6/workflows/edger_DE.smk` & `monsda-1.2.7/workflows/edger_DE.smk`

 * *Files 3% similar despite different names*

```diff
@@ -6,27 +6,28 @@
 
 rule themall:
     input:  session = expand("DE/{combo}/DE_EDGER_{scombo}_SESSION.gz", combo=combo, scombo=scombo),
             allM    = expand("DE/{combo}/Figures/DE_EDGER_{scombo}_DataSet_figure_AllConditionsMDS.png", combo=combo, scombo=scombo),
             allBCV  = expand("DE/{combo}/Figures/DE_EDGER_{scombo}_DataSet_figure_AllConditionsBCV.png", combo=combo, scombo=scombo),
             allQLD  = expand("DE/{combo}/Figures/DE_EDGER_{scombo}_DataSet_figure_AllConditionsQLDisp.png", combo=combo, scombo=scombo),
             MDplot  = expand("DE/{combo}/Figures/DE_EDGER_{scombo}_{comparison}_figure_MD.png", combo=combo, comparison=compstr, scombo=scombo),
+            vulcan  = expand("DE/{combo}/Figures/DE_EDGER_{scombo}_{comparison}_figure_Volcano.pdf", combo=combo, comparison=compstr, scombo=scombo),
             allN    = expand("DE/{combo}/Tables/DE_EDGER_{scombo}_DataSet_table_AllConditionsNormalized.tsv.gz", combo=combo, scombo=scombo),
             res     = expand("DE/{combo}/Tables/DE_EDGER_{scombo}_{comparison}_table_results.tsv.gz", combo=combo, comparison = compstr, scombo=scombo),
             sort    = expand("DE/{combo}/Tables/DE_EDGER_{scombo}_{comparison}_table_results{sort}.tsv.gz", combo=combo, comparison=compstr, scombo=scombo, sort=["PValueSorted"]),
             sig     = expand("DE/{combo}/Tables/Sig_DE_EDGER_{scombo}_{comparison}_table_results.tsv.gz", combo=combo, comparison = compstr, scombo=scombo),
             sig_u   = expand("DE/{combo}/Tables/SigUP_DE_EDGER_{scombo}_{comparison}_table_results.tsv.gz", combo=combo, comparison = compstr, scombo=scombo),
             sig_d   = expand("DE/{combo}/Tables/SigDOWN_DE_EDGER_{scombo}_{comparison}_table_results.tsv.gz", combo=combo, comparison = compstr, scombo=scombo),
             Rmd     = expand("REPORTS/SUMMARY/RmdSnippets/{combo}.Rmd", combo=combo)
 
 rule featurecount_unique:
     input:  reads = expand("MAPPED/{scombo}/{{file}}_mapped_sorted_unique.bam", scombo=scombo)
     output: tmp   = temp("DE/{combo}/Featurecounts/{file}_tmp.counts"),
-            tmph = temp("DE/{combo}/Featurecounts/{file}_tmp.head.gz"),
-            tmpc = temp("DE/{combo}/Featurecounts/{file}_tmp.count.gz"),
+            tmph  = temp("DE/{combo}/Featurecounts/{file}_tmp.head.gz"),
+            tmpc  = temp("DE/{combo}/Featurecounts/{file}_tmp.count.gz"),
             cts   = "DE/{combo}/Featurecounts/{file}_mapped_sorted_unique.counts.gz"
     log:    "LOGS/DE/{combo}/{file}_featurecounts_edger_unique.log"
     conda:  ""+COUNTENV+".yaml"
     threads: MAXTHREAD
     params: countb = COUNTBIN,
             anno = ANNOTATION,
             cpara = lambda wildcards: tool_params(wildcards.file, None, config, "DE", DEENV.split('_')[0])['OPTIONS'].get('COUNT', ""),
@@ -43,21 +44,22 @@
     conda:   ""+DEENV+".yaml"
     threads: 1
     params:  dereps = lambda wildcards, input: get_reps(input.cnd, config, 'DE'),
              bins = BINS
     shell: "{params.bins}/Analysis/build_count_table.py {params.dereps} --table {output.tbl} --anno {output.anno} 2> {log}"
 
 rule run_edger:
-    input:  tbl = expand(rules.prepare_count_table.output.tbl, combo=combo, scombo=scombo),
+    input:  tbl  = expand(rules.prepare_count_table.output.tbl, combo=combo, scombo=scombo),
             anno = expand(rules.prepare_count_table.output.anno, combo=combo, scombo=scombo)
     output: session = rules.themall.input.session,
             allM    = rules.themall.input.allM,
             allBCV  = rules.themall.input.allBCV,
             allQLD  = rules.themall.input.allQLD,
             MDplot  = rules.themall.input.MDplot,
+            vulcan  = rules.themall.input.vulcan,
             allN    = rules.themall.input.allN,
             res     = rules.themall.input.res,
             sort    = rules.themall.input.sort
     log:    expand("LOGS/DE/{combo}/run_edger.log", combo=combo)
     conda:  ""+DEENV+".yaml"
     threads: int(MAXTHREAD-1) if int(MAXTHREAD-1) >= 1 else 1
     params: bins   = str.join(os.sep,[BINS, DEBIN]),
@@ -82,14 +84,15 @@
 
 
 rule create_summary_snippet:
     input:  rules.run_edger.output.allM,
             rules.run_edger.output.allBCV,
             rules.run_edger.output.allQLD,
             rules.run_edger.output.MDplot,
+            rules.run_edger.output.vulcan,
             rules.run_edger.output.allN,
             rules.run_edger.output.res,
             rules.run_edger.output.sort,
             rules.run_edger.output.session,
             rules.filter_significant.output.sig,
             rules.filter_significant.output.sig_d,
             rules.filter_significant.output.sig_u
```

### Comparing `monsda-1.2.6/workflows/edger_DEU.nf` & `monsda-1.2.7/workflows/edger_DEU.nf`

 * *Files identical despite different names*

### Comparing `monsda-1.2.6/workflows/edger_DEU.smk` & `monsda-1.2.7/workflows/edger_DEU.smk`

 * *Files identical despite different names*

### Comparing `monsda-1.2.6/workflows/fastqc.nf` & `monsda-1.2.7/workflows/fastqc.nf`

 * *Files identical despite different names*

### Comparing `monsda-1.2.6/workflows/fastqc.smk` & `monsda-1.2.7/workflows/fastqc.smk`

 * *Files identical despite different names*

### Comparing `monsda-1.2.6/workflows/fastqc_dedup.nf` & `monsda-1.2.7/workflows/fastqc_dedup.nf`

 * *Files identical despite different names*

### Comparing `monsda-1.2.6/workflows/fastqc_dedup.smk` & `monsda-1.2.7/workflows/fastqc_dedup.smk`

 * *Files identical despite different names*

### Comparing `monsda-1.2.6/workflows/fastqc_dedup_trim.nf` & `monsda-1.2.7/workflows/fastqc_dedup_trim.nf`

 * *Files identical despite different names*

### Comparing `monsda-1.2.6/workflows/fastqc_dedup_trim.smk` & `monsda-1.2.7/workflows/fastqc_dedup_trim.smk`

 * *Files identical despite different names*

### Comparing `monsda-1.2.6/workflows/fastqc_raw.nf` & `monsda-1.2.7/workflows/fastqc_raw.nf`

 * *Files identical despite different names*

### Comparing `monsda-1.2.6/workflows/fastqc_raw.smk` & `monsda-1.2.7/workflows/fastqc_raw.smk`

 * *Files identical despite different names*

### Comparing `monsda-1.2.6/workflows/fastqc_trim.nf` & `monsda-1.2.7/workflows/fastqc_trim.nf`

 * *Files identical despite different names*

### Comparing `monsda-1.2.6/workflows/fastqc_trim.smk` & `monsda-1.2.7/workflows/fastqc_trim.smk`

 * *Files identical despite different names*

### Comparing `monsda-1.2.6/workflows/guppy.nf` & `monsda-1.2.7/workflows/guppy.nf`

 * *Files identical despite different names*

### Comparing `monsda-1.2.6/workflows/guppy.smk` & `monsda-1.2.7/workflows/guppy.smk`

 * *Files identical despite different names*

### Comparing `monsda-1.2.6/workflows/header.nf` & `monsda-1.2.7/workflows/header.nf`

 * *Files identical despite different names*

### Comparing `monsda-1.2.6/workflows/header.smk` & `monsda-1.2.7/workflows/header.smk`

 * *Files identical despite different names*

### Comparing `monsda-1.2.6/workflows/hisat2.nf` & `monsda-1.2.7/workflows/hisat2.nf`

 * *Files identical despite different names*

### Comparing `monsda-1.2.6/workflows/hisat2.smk` & `monsda-1.2.7/workflows/hisat2.smk`

 * *Files identical despite different names*

### Comparing `monsda-1.2.6/workflows/macs.nf` & `monsda-1.2.7/workflows/macs.nf`

 * *Files identical despite different names*

### Comparing `monsda-1.2.6/workflows/macs.smk` & `monsda-1.2.7/workflows/macs.smk`

 * *Files identical despite different names*

### Comparing `monsda-1.2.6/workflows/manipulate_genome.nf` & `monsda-1.2.7/workflows/manipulate_genome.nf`

 * *Files identical despite different names*

### Comparing `monsda-1.2.6/workflows/manipulate_genome.smk` & `monsda-1.2.7/workflows/manipulate_genome.smk`

 * *Files identical despite different names*

### Comparing `monsda-1.2.6/workflows/mapping.nf` & `monsda-1.2.7/workflows/mapping.nf`

 * *Files identical despite different names*

### Comparing `monsda-1.2.6/workflows/mapping.smk` & `monsda-1.2.7/workflows/mapping.smk`

 * *Files identical despite different names*

### Comparing `monsda-1.2.6/workflows/minimap.nf` & `monsda-1.2.7/workflows/minimap.nf`

 * *Files identical despite different names*

### Comparing `monsda-1.2.6/workflows/minimap.smk` & `monsda-1.2.7/workflows/minimap.smk`

 * *Files identical despite different names*

### Comparing `monsda-1.2.6/workflows/multiqc.nf` & `monsda-1.2.7/workflows/multiqc.nf`

 * *Files identical despite different names*

### Comparing `monsda-1.2.6/workflows/multiqc.smk` & `monsda-1.2.7/workflows/multiqc.smk`

 * *Files identical despite different names*

### Comparing `monsda-1.2.6/workflows/notify.nf` & `monsda-1.2.7/workflows/notify.nf`

 * *Files identical despite different names*

### Comparing `monsda-1.2.6/workflows/peaks.nf` & `monsda-1.2.7/workflows/peaks.nf`

 * *Files identical despite different names*

### Comparing `monsda-1.2.6/workflows/peaks.smk` & `monsda-1.2.7/workflows/peaks.smk`

 * *Files 1% similar despite different names*

```diff
@@ -44,26 +44,26 @@
     checktype = ['sorted', 'unique'] if not rundedup else ['sorted', 'sorted_unique', 'sorted_dedup', 'sorted_unique_dedup']
     for type in checktype:
         checklist.append(os.path.isfile(os.path.abspath('BED/'+scombo+file+'_mapped_'+type+'.bed.gz')) and not os.path.islink(os.path.abspath('BED/'+scombo+file+'_mapped_'+type+'.bed.gz')))
 
 if not all(checklist):
     if not stranded or (stranded == 'fr' or stranded == 'ISF'):
         rule BamToBed:
-            input:  expand("MAPPED/{scombo}/{{file}}_mapped_{{type}}_nosoftclip.bam", scombo=scombo)
-            output: "BED/{scombo}/{file}_mapped_{type}_nosoftclip.bed.gz"
+            input:  expand("MAPPED/{scombo}/{{file}}_mapped_{{type}}.bam", scombo=scombo)
+            output: "BED/{scombo}/{file}_mapped_{type}.bed.gz"
             log:    "LOGS/PEAKS/{scombo}/{file}bam2bed_{type}.log"
             conda:  "bedtools.yaml"
             threads: 1
             params: sortmem = lambda wildcards, threads:  int(30/MAXTHREAD*threads)
             shell:  "bedtools bamtobed -split -i {input[0]} |sed 's/ /\_/g'|perl -wl -a -F\'\\t\' -n -e '$F[0] =~ s/\s/_/g;if($F[3]=~/\/2$/){{if ($F[5] eq \"+\"){{$F[5] = \"-\"}}elsif($F[5] eq \"-\"){{$F[5] = \"+\"}}}} print join(\"\t\",@F[0..$#F])' |sort -S {params.sortmem}% -T TMP -t$'\t' -k1,1 -k2,2n |gzip > {output[0]} 2> {log}"
 
     elif stranded and (stranded == 'rf' or stranded == 'ISR'):
         rule BamToBed:
-            input:  expand("MAPPED/{scombo}/{{file}}_mapped_{{type}}_nosoftclip.bam", scombo=scombo)
-            output: "BED/{scombo}/{file}_mapped_{type}_nosoftclip.bed.gz"
+            input:  expand("MAPPED/{scombo}/{{file}}_mapped_{{type}}.bam", scombo=scombo)
+            output: "BED/{scombo}/{file}_mapped_{type}.bed.gz"
             log:    "LOGS/PEAKS/{scombo}/{file}bam2bed_{type}.log"
             conda:  "bedtools.yaml"
             threads: 1
             params: sortmem = lambda wildcards, threads:  int(30/MAXTHREAD*threads)
             shell:  "bedtools bamtobed -split -i {input[0]} |sed 's/ /\_/g'|perl -wl -a -F\'\\t\' -n -e '$F[0] =~ s/\s/_/g;if($F[3]=~/\/1$/){{if ($F[5] eq \"+\"){{$F[5] = \"-\"}}elsif($F[5] eq \"-\"){{$F[5] = \"+\"}}}} print join(\"\t\",@F[0..$#F])' |sort -S {params.sortmem}% -T TMP -t$'\t' -k1,1 -k2,2n |gzip > {output[0]} 2> {log}"
 
 include: "manipulate_genome.smk"
```

### Comparing `monsda-1.2.6/workflows/picard_dedup.nf` & `monsda-1.2.7/workflows/picard_dedup.nf`

 * *Files identical despite different names*

### Comparing `monsda-1.2.6/workflows/picard_dedup.smk` & `monsda-1.2.7/workflows/picard_dedup.smk`

 * *Files identical despite different names*

### Comparing `monsda-1.2.6/workflows/piranha.nf` & `monsda-1.2.7/workflows/piranha.nf`

 * *Files identical despite different names*

### Comparing `monsda-1.2.6/workflows/piranha.smk` & `monsda-1.2.7/workflows/piranha.smk`

 * *Files 0% similar despite different names*

```diff
@@ -44,26 +44,26 @@
     checktype = ['sorted', 'unique'] if not rundedup else ['sorted', 'sorted_unique', 'sorted_dedup', 'sorted_unique_dedup']
     for type in checktype:
         checklist.append(os.path.isfile(os.path.abspath('BED/'+scombo+file+'_mapped_'+type+'.bed.gz')) and not os.path.islink(os.path.abspath('BED/'+scombo+file+'_mapped_'+type+'.bed.gz')))
 
 if not all(checklist):
     if not stranded or (stranded == 'fr' or stranded == 'ISF'):
         rule BamToBed:
-            input:  expand("MAPPED/{scombo}/{{file}}_mapped_{{type}}_nosoftclip.bam", scombo=scombo)
-            output: "BED/{scombo}/{file}_mapped_{type}_nosoftclip.bed.gz"
+            input:  expand("MAPPED/{scombo}/{{file}}_mapped_{{type}}.bam", scombo=scombo)
+            output: "BED/{scombo}/{file}_mapped_{type}.bed.gz"
             log:    "LOGS/PEAKS/{scombo}/{file}bam2bed_{type}.log"
             conda:  "bedtools.yaml"
             threads: 1
             params: sortmem = lambda wildcards, threads:  int(30/MAXTHREAD*threads)
             shell:  "bedtools bamtobed -split -i {input[0]} |sed 's/ /\_/g'|perl -wl -a -F\'\\t\' -n -e '$F[0] =~ s/\s/_/g;if($F[3]=~/\/2$/){{if ($F[5] eq \"+\"){{$F[5] = \"-\"}}elsif($F[5] eq \"-\"){{$F[5] = \"+\"}}}} print join(\"\t\",@F[0..$#F])' |sort -S {params.sortmem}% -T TMP -t$'\t' -k1,1 -k2,2n |gzip > {output[0]} 2> {log}"
 
     elif stranded and (stranded == 'rf' or stranded == 'ISR'):
         rule BamToBed:
-            input:  expand("MAPPED/{scombo}/{{file}}_mapped_{{type}}_nosoftclip.bam", scombo=scombo)
-            output: "BED/{scombo}/{file}_mapped_{type}_nosoftclip.bed.gz"
+            input:  expand("MAPPED/{scombo}/{{file}}_mapped_{{type}}.bam", scombo=scombo)
+            output: "BED/{scombo}/{file}_mapped_{type}.bed.gz"
             log:    "LOGS/PEAKS/{scombo}/{file}bam2bed_{type}.log"
             conda:  "bedtools.yaml"
             threads: 1
             params: sortmem = lambda wildcards, threads:  int(30/MAXTHREAD*threads)
             shell:  "bedtools bamtobed -split -i {input[0]} |sed 's/ /\_/g'|perl -wl -a -F\'\\t\' -n -e '$F[0] =~ s/\s/_/g;if($F[3]=~/\/1$/){{if ($F[5] eq \"+\"){{$F[5] = \"-\"}}elsif($F[5] eq \"-\"){{$F[5] = \"+\"}}}} print join(\"\t\",@F[0..$#F])' |sort -S {params.sortmem}% -T TMP -t$'\t' -k1,1 -k2,2n |gzip > {output[0]} 2> {log}"
 
 include: "manipulate_genome.smk"
```

### Comparing `monsda-1.2.6/workflows/premultiqc.nf` & `monsda-1.2.7/workflows/premultiqc.nf`

 * *Files identical despite different names*

### Comparing `monsda-1.2.6/workflows/premultiqc.smk` & `monsda-1.2.7/workflows/premultiqc.smk`

 * *Files identical despite different names*

### Comparing `monsda-1.2.6/workflows/salmon.nf` & `monsda-1.2.7/workflows/salmon.nf`

 * *Files identical despite different names*

### Comparing `monsda-1.2.6/workflows/salmon.smk` & `monsda-1.2.7/workflows/salmon.smk`

 * *Files identical despite different names*

### Comparing `monsda-1.2.6/workflows/salmon_trim.smk` & `monsda-1.2.7/workflows/salmon_trim.smk`

 * *Files identical despite different names*

### Comparing `monsda-1.2.6/workflows/scyphy.nf` & `monsda-1.2.7/workflows/scyphy.nf`

 * *Files identical despite different names*

### Comparing `monsda-1.2.6/workflows/scyphy.smk` & `monsda-1.2.7/workflows/scyphy.smk`

 * *Files identical despite different names*

### Comparing `monsda-1.2.6/workflows/segemehl.nf` & `monsda-1.2.7/workflows/segemehl.nf`

 * *Files identical despite different names*

### Comparing `monsda-1.2.6/workflows/segemehl.smk` & `monsda-1.2.7/workflows/segemehl.smk`

 * *Files identical despite different names*

### Comparing `monsda-1.2.6/workflows/segemehl3.nf` & `monsda-1.2.7/workflows/segemehl3.nf`

 * *Files identical despite different names*

### Comparing `monsda-1.2.6/workflows/segemehl3.smk` & `monsda-1.2.7/workflows/segemehl3.smk`

 * *Files identical despite different names*

### Comparing `monsda-1.2.6/workflows/segemehl3_bisulfite.nf` & `monsda-1.2.7/workflows/segemehl3_bisulfite.nf`

 * *Files identical despite different names*

### Comparing `monsda-1.2.6/workflows/segemehl3_bisulfite.smk` & `monsda-1.2.7/workflows/segemehl3_bisulfite.smk`

 * *Files identical despite different names*

### Comparing `monsda-1.2.6/workflows/segemehl_bisulfite.nf` & `monsda-1.2.7/workflows/segemehl_bisulfite.nf`

 * *Files identical despite different names*

### Comparing `monsda-1.2.6/workflows/segemehl_bisulfite.smk` & `monsda-1.2.7/workflows/segemehl_bisulfite.smk`

 * *Files identical despite different names*

### Comparing `monsda-1.2.6/workflows/simulatetrim.nf` & `monsda-1.2.7/workflows/simulatetrim.nf`

 * *Files identical despite different names*

### Comparing `monsda-1.2.6/workflows/simulatetrim.smk` & `monsda-1.2.7/workflows/simulatetrim.smk`

 * *Files identical despite different names*

### Comparing `monsda-1.2.6/workflows/sra.nf` & `monsda-1.2.7/workflows/sra.nf`

 * *Files identical despite different names*

### Comparing `monsda-1.2.6/workflows/sra.smk` & `monsda-1.2.7/workflows/sra.smk`

 * *Files identical despite different names*

### Comparing `monsda-1.2.6/workflows/star.nf` & `monsda-1.2.7/workflows/star.nf`

 * *Files identical despite different names*

### Comparing `monsda-1.2.6/workflows/star.smk` & `monsda-1.2.7/workflows/star.smk`

 * *Files identical despite different names*

### Comparing `monsda-1.2.6/workflows/summary.nf` & `monsda-1.2.7/workflows/summary.nf`

 * *Files identical despite different names*

### Comparing `monsda-1.2.6/workflows/summary.smk` & `monsda-1.2.7/workflows/summary.smk`

 * *Files identical despite different names*

### Comparing `monsda-1.2.6/workflows/trimgalore.nf` & `monsda-1.2.7/workflows/trimgalore.nf`

 * *Files identical despite different names*

### Comparing `monsda-1.2.6/workflows/trimgalore.smk` & `monsda-1.2.7/workflows/trimgalore.smk`

 * *Files identical despite different names*

### Comparing `monsda-1.2.6/workflows/ucsc.nf` & `monsda-1.2.7/workflows/ucsc.nf`

 * *Files identical despite different names*

### Comparing `monsda-1.2.6/workflows/ucsc.smk` & `monsda-1.2.7/workflows/ucsc.smk`

 * *Files identical despite different names*

### Comparing `monsda-1.2.6/workflows/umitools.nf` & `monsda-1.2.7/workflows/umitools.nf`

 * *Files identical despite different names*

### Comparing `monsda-1.2.6/workflows/umitools.smk` & `monsda-1.2.7/workflows/umitools.smk`

 * *Files identical despite different names*

### Comparing `monsda-1.2.6/workflows/umitools_dedup.nf` & `monsda-1.2.7/workflows/umitools_dedup.nf`

 * *Files identical despite different names*

