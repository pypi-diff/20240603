# Comparing `tmp/inmoose-0.4.1.tar.gz` & `tmp/inmoose-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "inmoose-0.4.1.tar", last modified: Fri Mar 29 09:03:41 2024, max compression
+gzip compressed data, was "inmoose-0.5.0.tar", last modified: Mon Jun  3 13:32:44 2024, max compression
```

## Comparing `inmoose-0.4.1.tar` & `inmoose-0.5.0.tar`

### file list

```diff
@@ -1,208 +1,226 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 09:03:41.191398 inmoose-0.4.1/
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-03-29 09:03:34.000000 inmoose-0.4.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       70 2024-03-29 09:03:34.000000 inmoose-0.4.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     4256 2024-03-29 09:03:41.191398 inmoose-0.4.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3179 2024-03-29 09:03:34.000000 inmoose-0.4.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 09:03:41.119397 inmoose-0.4.1/inmoose/
--rw-r--r--   0 runner    (1001) docker     (127)      633 2024-03-29 09:03:34.000000 inmoose-0.4.1/inmoose/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 09:03:41.119397 inmoose-0.4.1/inmoose/common_cpp/
--rw-r--r--   0 runner    (1001) docker     (127)      962 2024-03-29 09:03:34.000000 inmoose-0.4.1/inmoose/common_cpp/common_cpp.pyx
--rw-r--r--   0 runner    (1001) docker     (127)     2836 2024-03-29 09:03:34.000000 inmoose-0.4.1/inmoose/common_cpp/matrix.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     9126 2024-03-29 09:03:34.000000 inmoose-0.4.1/inmoose/common_cpp/matrix.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 09:03:41.119397 inmoose-0.4.1/inmoose/consensus_clustering/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-29 09:03:34.000000 inmoose-0.4.1/inmoose/consensus_clustering/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    20310 2024-03-29 09:03:34.000000 inmoose-0.4.1/inmoose/consensus_clustering/consensus_clustering.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 09:03:41.115398 inmoose-0.4.1/inmoose/data/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 09:03:41.119397 inmoose-0.4.1/inmoose/data/airway/
--rw-r--r--   0 runner    (1001) docker     (127)      400 2024-03-29 09:03:34.000000 inmoose-0.4.1/inmoose/data/airway/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)  5154656 2024-03-29 09:03:34.000000 inmoose-0.4.1/inmoose/data/airway/airway.h5ad
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 09:03:41.155398 inmoose-0.4.1/inmoose/data/pasilla/
--rw-r--r--   0 runner    (1001) docker     (127) 13589253 2024-03-29 09:03:34.000000 inmoose-0.4.1/inmoose/data/pasilla/Dmel.BDGP5.25.62.DEXSeq.chr.gff
--rw-r--r--   0 runner    (1001) docker     (127)     1082 2024-03-29 09:03:34.000000 inmoose-0.4.1/inmoose/data/pasilla/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      552 2024-03-29 09:03:34.000000 inmoose-0.4.1/inmoose/data/pasilla/geneIDsinsubset.txt
--rw-r--r--   0 runner    (1001) docker     (127)   498373 2024-03-29 09:03:34.000000 inmoose-0.4.1/inmoose/data/pasilla/pasilla_gene_counts.tsv
--rw-r--r--   0 runner    (1001) docker     (127)      527 2024-03-29 09:03:34.000000 inmoose-0.4.1/inmoose/data/pasilla/pasilla_sample_annotation.csv
--rw-r--r--   0 runner    (1001) docker     (127)  1370030 2024-03-29 09:03:34.000000 inmoose-0.4.1/inmoose/data/pasilla/treated1fb.txt
--rw-r--r--   0 runner    (1001) docker     (127)  1359480 2024-03-29 09:03:34.000000 inmoose-0.4.1/inmoose/data/pasilla/treated2fb.txt
--rw-r--r--   0 runner    (1001) docker     (127)  1361730 2024-03-29 09:03:34.000000 inmoose-0.4.1/inmoose/data/pasilla/treated3fb.txt
--rw-r--r--   0 runner    (1001) docker     (127)  1363665 2024-03-29 09:03:34.000000 inmoose-0.4.1/inmoose/data/pasilla/untreated1fb.txt
--rw-r--r--   0 runner    (1001) docker     (127)  1371149 2024-03-29 09:03:34.000000 inmoose-0.4.1/inmoose/data/pasilla/untreated2fb.txt
--rw-r--r--   0 runner    (1001) docker     (127)  1358790 2024-03-29 09:03:34.000000 inmoose-0.4.1/inmoose/data/pasilla/untreated3fb.txt
--rw-r--r--   0 runner    (1001) docker     (127)  1359414 2024-03-29 09:03:34.000000 inmoose-0.4.1/inmoose/data/pasilla/untreated4fb.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 09:03:41.159398 inmoose-0.4.1/inmoose/deseq2/
--rw-r--r--   0 runner    (1001) docker     (127)    25647 2024-03-29 09:03:34.000000 inmoose-0.4.1/inmoose/deseq2/DESeqDataSet.py
--rw-r--r--   0 runner    (1001) docker     (127)     1725 2024-03-29 09:03:34.000000 inmoose-0.4.1/inmoose/deseq2/DESeqTransform.py
--rw-r--r--   0 runner    (1001) docker     (127)     3565 2024-03-29 09:03:34.000000 inmoose-0.4.1/inmoose/deseq2/Hmisc.py
--rw-r--r--   0 runner    (1001) docker     (127)      624 2024-03-29 09:03:34.000000 inmoose-0.4.1/inmoose/deseq2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    15132 2024-03-29 09:03:34.000000 inmoose-0.4.1/inmoose/deseq2/core.py
--rw-r--r--   0 runner    (1001) docker     (127)    35085 2024-03-29 09:03:34.000000 inmoose-0.4.1/inmoose/deseq2/deseq2_cpp.py
--rw-r--r--   0 runner    (1001) docker     (127)    36033 2024-03-29 09:03:34.000000 inmoose-0.4.1/inmoose/deseq2/dispersions.py
--rw-r--r--   0 runner    (1001) docker     (127)    10481 2024-03-29 09:03:34.000000 inmoose-0.4.1/inmoose/deseq2/estimateSizeFactors.py
--rw-r--r--   0 runner    (1001) docker     (127)    19848 2024-03-29 09:03:34.000000 inmoose-0.4.1/inmoose/deseq2/fitNbinomGLMs.py
--rw-r--r--   0 runner    (1001) docker     (127)     4538 2024-03-29 09:03:34.000000 inmoose-0.4.1/inmoose/deseq2/lrt.py
--rw-r--r--   0 runner    (1001) docker     (127)     3436 2024-03-29 09:03:34.000000 inmoose-0.4.1/inmoose/deseq2/misc.py
--rw-r--r--   0 runner    (1001) docker     (127)    10255 2024-03-29 09:03:34.000000 inmoose-0.4.1/inmoose/deseq2/outliers.py
--rw-r--r--   0 runner    (1001) docker     (127)     2908 2024-03-29 09:03:34.000000 inmoose-0.4.1/inmoose/deseq2/parallel.py
--rw-r--r--   0 runner    (1001) docker     (127)     8024 2024-03-29 09:03:34.000000 inmoose-0.4.1/inmoose/deseq2/plot.py
--rw-r--r--   0 runner    (1001) docker     (127)     5422 2024-03-29 09:03:34.000000 inmoose-0.4.1/inmoose/deseq2/prior.py
--rw-r--r--   0 runner    (1001) docker     (127)     4221 2024-03-29 09:03:34.000000 inmoose-0.4.1/inmoose/deseq2/replicates.py
--rw-r--r--   0 runner    (1001) docker     (127)    54356 2024-03-29 09:03:34.000000 inmoose-0.4.1/inmoose/deseq2/results.py
--rw-r--r--   0 runner    (1001) docker     (127)    12731 2024-03-29 09:03:34.000000 inmoose-0.4.1/inmoose/deseq2/vst.py
--rw-r--r--   0 runner    (1001) docker     (127)    21348 2024-03-29 09:03:34.000000 inmoose-0.4.1/inmoose/deseq2/wald.py
--rw-r--r--   0 runner    (1001) docker     (127)     4841 2024-03-29 09:03:34.000000 inmoose-0.4.1/inmoose/deseq2/weights.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 09:03:41.167398 inmoose-0.4.1/inmoose/edgepy/
--rw-r--r--   0 runner    (1001) docker     (127)     1158 2024-03-29 09:03:34.000000 inmoose-0.4.1/inmoose/edgepy/DGEExact.py
--rw-r--r--   0 runner    (1001) docker     (127)     2607 2024-03-29 09:03:34.000000 inmoose-0.4.1/inmoose/edgepy/DGEGLM.py
--rw-r--r--   0 runner    (1001) docker     (127)     1287 2024-03-29 09:03:34.000000 inmoose-0.4.1/inmoose/edgepy/DGELRT.py
--rw-r--r--   0 runner    (1001) docker     (127)     9278 2024-03-29 09:03:34.000000 inmoose-0.4.1/inmoose/edgepy/DGEList.py
--rw-r--r--   0 runner    (1001) docker     (127)     1331 2024-03-29 09:03:34.000000 inmoose-0.4.1/inmoose/edgepy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4236 2024-03-29 09:03:34.000000 inmoose-0.4.1/inmoose/edgepy/addPriorCount.py
--rw-r--r--   0 runner    (1001) docker     (127)     5473 2024-03-29 09:03:34.000000 inmoose-0.4.1/inmoose/edgepy/adjustedProfileLik.py
--rw-r--r--   0 runner    (1001) docker     (127)     7487 2024-03-29 09:03:34.000000 inmoose-0.4.1/inmoose/edgepy/aveLogCPM.py
--rw-r--r--   0 runner    (1001) docker     (127)     5042 2024-03-29 09:03:34.000000 inmoose-0.4.1/inmoose/edgepy/binomTest.py
--rw-r--r--   0 runner    (1001) docker     (127)     6135 2024-03-29 09:03:34.000000 inmoose-0.4.1/inmoose/edgepy/dispCoxReid.py
--rw-r--r--   0 runner    (1001) docker     (127)     7747 2024-03-29 09:03:34.000000 inmoose-0.4.1/inmoose/edgepy/dispCoxReidInterpolateTagwise.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 09:03:41.171398 inmoose-0.4.1/inmoose/edgepy/edgepy_cpp/
--rw-r--r--   0 runner    (1001) docker     (127)     6166 2024-03-29 09:03:34.000000 inmoose-0.4.1/inmoose/edgepy/edgepy_cpp/__init__.pxd
--rw-r--r--   0 runner    (1001) docker     (127)     3085 2024-03-29 09:03:34.000000 inmoose-0.4.1/inmoose/edgepy/edgepy_cpp/add_prior.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     1583 2024-03-29 09:03:34.000000 inmoose-0.4.1/inmoose/edgepy/edgepy_cpp/add_prior.h
--rw-r--r--   0 runner    (1001) docker     (127)     3110 2024-03-29 09:03:34.000000 inmoose-0.4.1/inmoose/edgepy/edgepy_cpp/add_prior_count.cpp
--rw-r--r--   0 runner    (1001) docker     (127)      869 2024-03-29 09:03:34.000000 inmoose-0.4.1/inmoose/edgepy/edgepy_cpp/add_prior_count.h
--rw-r--r--   0 runner    (1001) docker     (127)     5168 2024-03-29 09:03:34.000000 inmoose-0.4.1/inmoose/edgepy/edgepy_cpp/adj_coxreid.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     2568 2024-03-29 09:03:34.000000 inmoose-0.4.1/inmoose/edgepy/edgepy_cpp/ave_log_cpm.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     5065 2024-03-29 09:03:34.000000 inmoose-0.4.1/inmoose/edgepy/edgepy_cpp/compute_apl.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     3796 2024-03-29 09:03:34.000000 inmoose-0.4.1/inmoose/edgepy/edgepy_cpp/compute_nbdev.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     8270 2024-03-29 09:03:34.000000 inmoose-0.4.1/inmoose/edgepy/edgepy_cpp/edgepy_cpp.pyx
--rw-r--r--   0 runner    (1001) docker     (127)     3507 2024-03-29 09:03:34.000000 inmoose-0.4.1/inmoose/edgepy/edgepy_cpp/fit_levenberg.cpp
--rw-r--r--   0 runner    (1001) docker     (127)      955 2024-03-29 09:03:34.000000 inmoose-0.4.1/inmoose/edgepy/edgepy_cpp/fit_levenberg.h
--rw-r--r--   0 runner    (1001) docker     (127)     4692 2024-03-29 09:03:34.000000 inmoose-0.4.1/inmoose/edgepy/edgepy_cpp/fit_one_group.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     2371 2024-03-29 09:03:34.000000 inmoose-0.4.1/inmoose/edgepy/edgepy_cpp/get_one_way_fitted.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     2273 2024-03-29 09:03:34.000000 inmoose-0.4.1/inmoose/edgepy/edgepy_cpp/glm.h
--rw-r--r--   0 runner    (1001) docker     (127)    11007 2024-03-29 09:03:34.000000 inmoose-0.4.1/inmoose/edgepy/edgepy_cpp/glm_levenberg.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     2625 2024-03-29 09:03:34.000000 inmoose-0.4.1/inmoose/edgepy/edgepy_cpp/glm_one_group.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     6064 2024-03-29 09:03:34.000000 inmoose-0.4.1/inmoose/edgepy/edgepy_cpp/initialize_levenberg.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     1137 2024-03-29 09:03:34.000000 inmoose-0.4.1/inmoose/edgepy/edgepy_cpp/initialize_levenberg.h
--rw-r--r--   0 runner    (1001) docker     (127)     7061 2024-03-29 09:03:34.000000 inmoose-0.4.1/inmoose/edgepy/edgepy_cpp/interpolator.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     1308 2024-03-29 09:03:34.000000 inmoose-0.4.1/inmoose/edgepy/edgepy_cpp/interpolator.h
--rw-r--r--   0 runner    (1001) docker     (127)     1880 2024-03-29 09:03:34.000000 inmoose-0.4.1/inmoose/edgepy/edgepy_cpp/maximize_interpolant.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     5066 2024-03-29 09:03:34.000000 inmoose-0.4.1/inmoose/edgepy/edgepy_cpp/objects.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     1957 2024-03-29 09:03:34.000000 inmoose-0.4.1/inmoose/edgepy/edgepy_cpp/objects.h
--rw-r--r--   0 runner    (1001) docker     (127)     1801 2024-03-29 09:03:34.000000 inmoose-0.4.1/inmoose/edgepy/edgepy_cpp/utils.h
--rw-r--r--   0 runner    (1001) docker     (127)     5750 2024-03-29 09:03:34.000000 inmoose-0.4.1/inmoose/edgepy/estimateGLMCommonDisp.py
--rw-r--r--   0 runner    (1001) docker     (127)     7365 2024-03-29 09:03:34.000000 inmoose-0.4.1/inmoose/edgepy/estimateGLMTagwiseDisp.py
--rw-r--r--   0 runner    (1001) docker     (127)    10780 2024-03-29 09:03:34.000000 inmoose-0.4.1/inmoose/edgepy/exactTest.py
--rw-r--r--   0 runner    (1001) docker     (127)     3388 2024-03-29 09:03:34.000000 inmoose-0.4.1/inmoose/edgepy/exactTestBetaApprox.py
--rw-r--r--   0 runner    (1001) docker     (127)     5414 2024-03-29 09:03:34.000000 inmoose-0.4.1/inmoose/edgepy/exactTestByDeviance.py
--rw-r--r--   0 runner    (1001) docker     (127)     4539 2024-03-29 09:03:34.000000 inmoose-0.4.1/inmoose/edgepy/exactTestBySmallP.py
--rw-r--r--   0 runner    (1001) docker     (127)     4528 2024-03-29 09:03:34.000000 inmoose-0.4.1/inmoose/edgepy/exactTestDoubleTail.py
--rw-r--r--   0 runner    (1001) docker     (127)    17020 2024-03-29 09:03:34.000000 inmoose-0.4.1/inmoose/edgepy/glmFit.py
--rw-r--r--   0 runner    (1001) docker     (127)    15621 2024-03-29 09:03:34.000000 inmoose-0.4.1/inmoose/edgepy/glmQLFit.py
--rw-r--r--   0 runner    (1001) docker     (127)     5146 2024-03-29 09:03:34.000000 inmoose-0.4.1/inmoose/edgepy/makeCompressedMatrix.py
--rw-r--r--   0 runner    (1001) docker     (127)     2678 2024-03-29 09:03:34.000000 inmoose-0.4.1/inmoose/edgepy/maximizeInterpolant.py
--rw-r--r--   0 runner    (1001) docker     (127)     5852 2024-03-29 09:03:34.000000 inmoose-0.4.1/inmoose/edgepy/mglmLevenberg.py
--rw-r--r--   0 runner    (1001) docker     (127)     4863 2024-03-29 09:03:34.000000 inmoose-0.4.1/inmoose/edgepy/mglmOneGroup.py
--rw-r--r--   0 runner    (1001) docker     (127)     7924 2024-03-29 09:03:34.000000 inmoose-0.4.1/inmoose/edgepy/mglmOneWay.py
--rw-r--r--   0 runner    (1001) docker     (127)     2665 2024-03-29 09:03:34.000000 inmoose-0.4.1/inmoose/edgepy/movingAverageByCol.py
--rw-r--r--   0 runner    (1001) docker     (127)     4501 2024-03-29 09:03:34.000000 inmoose-0.4.1/inmoose/edgepy/nbinomDeviance.py
--rw-r--r--   0 runner    (1001) docker     (127)     4900 2024-03-29 09:03:34.000000 inmoose-0.4.1/inmoose/edgepy/predFC.py
--rw-r--r--   0 runner    (1001) docker     (127)     2752 2024-03-29 09:03:34.000000 inmoose-0.4.1/inmoose/edgepy/q2qnbinom.py
--rw-r--r--   0 runner    (1001) docker     (127)     2848 2024-03-29 09:03:34.000000 inmoose-0.4.1/inmoose/edgepy/residDF.py
--rw-r--r--   0 runner    (1001) docker     (127)     2659 2024-03-29 09:03:34.000000 inmoose-0.4.1/inmoose/edgepy/splitIntoGroups.py
--rw-r--r--   0 runner    (1001) docker     (127)     5006 2024-03-29 09:03:34.000000 inmoose-0.4.1/inmoose/edgepy/stats.py
--rw-r--r--   0 runner    (1001) docker     (127)     1773 2024-03-29 09:03:34.000000 inmoose-0.4.1/inmoose/edgepy/systematicSubset.py
--rw-r--r--   0 runner    (1001) docker     (127)     7307 2024-03-29 09:03:34.000000 inmoose-0.4.1/inmoose/edgepy/topTags.py
--rw-r--r--   0 runner    (1001) docker     (127)     1883 2024-03-29 09:03:34.000000 inmoose-0.4.1/inmoose/edgepy/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1911 2024-03-29 09:03:34.000000 inmoose-0.4.1/inmoose/edgepy/validDGEList.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 09:03:41.171398 inmoose-0.4.1/inmoose/limma/
--rw-r--r--   0 runner    (1001) docker     (127)       66 2024-03-29 09:03:34.000000 inmoose-0.4.1/inmoose/limma/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9206 2024-03-29 09:03:34.000000 inmoose-0.4.1/inmoose/limma/fitFDist.py
--rw-r--r--   0 runner    (1001) docker     (127)     5950 2024-03-29 09:03:34.000000 inmoose-0.4.1/inmoose/limma/squeezeVar.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 09:03:41.171398 inmoose-0.4.1/inmoose/pycombat/
--rw-r--r--   0 runner    (1001) docker     (127)       80 2024-03-29 09:03:34.000000 inmoose-0.4.1/inmoose/pycombat/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    17889 2024-03-29 09:03:34.000000 inmoose-0.4.1/inmoose/pycombat/covariates.py
--rw-r--r--   0 runner    (1001) docker     (127)     3366 2024-03-29 09:03:34.000000 inmoose-0.4.1/inmoose/pycombat/helper_seq.py
--rw-r--r--   0 runner    (1001) docker     (127)    22194 2024-03-29 09:03:34.000000 inmoose-0.4.1/inmoose/pycombat/pycombat_norm.py
--rw-r--r--   0 runner    (1001) docker     (127)     8912 2024-03-29 09:03:34.000000 inmoose-0.4.1/inmoose/pycombat/pycombat_seq.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 09:03:41.171398 inmoose-0.4.1/inmoose/sim/
--rw-r--r--   0 runner    (1001) docker     (127)       30 2024-03-29 09:03:34.000000 inmoose-0.4.1/inmoose/sim/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8408 2024-03-29 09:03:34.000000 inmoose-0.4.1/inmoose/sim/splat.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 09:03:41.171398 inmoose-0.4.1/inmoose/utils/
--rw-r--r--   0 runner    (1001) docker     (127)       98 2024-03-29 09:03:34.000000 inmoose-0.4.1/inmoose/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1118 2024-03-29 09:03:34.000000 inmoose-0.4.1/inmoose/utils/_stats.pyx
--rw-r--r--   0 runner    (1001) docker     (127)     1757 2024-03-29 09:03:34.000000 inmoose-0.4.1/inmoose/utils/factor.py
--rw-r--r--   0 runner    (1001) docker     (127)     5316 2024-03-29 09:03:34.000000 inmoose-0.4.1/inmoose/utils/stats.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 09:03:41.191398 inmoose-0.4.1/inmoose.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4256 2024-03-29 09:03:41.000000 inmoose-0.4.1/inmoose.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5789 2024-03-29 09:03:41.000000 inmoose-0.4.1/inmoose.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-29 09:03:41.000000 inmoose-0.4.1/inmoose.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      150 2024-03-29 09:03:41.000000 inmoose-0.4.1/inmoose.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)      223 2024-03-29 09:03:41.000000 inmoose-0.4.1/inmoose.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1050 2024-03-29 09:03:34.000000 inmoose-0.4.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-29 09:03:41.191398 inmoose-0.4.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     3157 2024-03-29 09:03:34.000000 inmoose-0.4.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 09:03:41.171398 inmoose-0.4.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-29 09:03:34.000000 inmoose-0.4.1/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 09:03:41.183398 inmoose-0.4.1/tests/consensus_clustering/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-29 09:03:34.000000 inmoose-0.4.1/tests/consensus_clustering/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)  6796249 2024-03-29 09:03:34.000000 inmoose-0.4.1/tests/consensus_clustering/mocked_data_consensus_clustering.csv
--rw-r--r--   0 runner    (1001) docker     (127)     3554 2024-03-29 09:03:34.000000 inmoose-0.4.1/tests/consensus_clustering/test_consensus_clustering.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 09:03:41.183398 inmoose-0.4.1/tests/data/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-29 09:03:34.000000 inmoose-0.4.1/tests/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      324 2024-03-29 09:03:34.000000 inmoose-0.4.1/tests/data/test_airway.py
--rw-r--r--   0 runner    (1001) docker     (127)      334 2024-03-29 09:03:34.000000 inmoose-0.4.1/tests/data/test_pasilla.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 09:03:41.187398 inmoose-0.4.1/tests/deseq2/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-29 09:03:34.000000 inmoose-0.4.1/tests/deseq2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2175 2024-03-29 09:03:34.000000 inmoose-0.4.1/tests/deseq2/test_DESeq.py
--rw-r--r--   0 runner    (1001) docker     (127)     2255 2024-03-29 09:03:34.000000 inmoose-0.4.1/tests/deseq2/test_DESeqDataSet.py
--rw-r--r--   0 runner    (1001) docker     (127)     1982 2024-03-29 09:03:34.000000 inmoose-0.4.1/tests/deseq2/test_LRT.py
--rw-r--r--   0 runner    (1001) docker     (127)      526 2024-03-29 09:03:34.000000 inmoose-0.4.1/tests/deseq2/test_QR.py
--rw-r--r--   0 runner    (1001) docker     (127)     1205 2024-03-29 09:03:34.000000 inmoose-0.4.1/tests/deseq2/test_addMLE.py
--rw-r--r--   0 runner    (1001) docker     (127)     2317 2024-03-29 09:03:34.000000 inmoose-0.4.1/tests/deseq2/test_betaFitting.py
--rw-r--r--   0 runner    (1001) docker     (127)      602 2024-03-29 09:03:34.000000 inmoose-0.4.1/tests/deseq2/test_collapse.py
--rw-r--r--   0 runner    (1001) docker     (127)     7523 2024-03-29 09:03:34.000000 inmoose-0.4.1/tests/deseq2/test_dispersions.py
--rw-r--r--   0 runner    (1001) docker     (127)      482 2024-03-29 09:03:34.000000 inmoose-0.4.1/tests/deseq2/test_fpkm.py
--rw-r--r--   0 runner    (1001) docker     (127)     1492 2024-03-29 09:03:34.000000 inmoose-0.4.1/tests/deseq2/test_interactions.py
--rw-r--r--   0 runner    (1001) docker     (127)     1162 2024-03-29 09:03:34.000000 inmoose-0.4.1/tests/deseq2/test_linear_mu.py
--rw-r--r--   0 runner    (1001) docker     (127)     1432 2024-03-29 09:03:34.000000 inmoose-0.4.1/tests/deseq2/test_methods.py
--rw-r--r--   0 runner    (1001) docker     (127)     2118 2024-03-29 09:03:34.000000 inmoose-0.4.1/tests/deseq2/test_model_matrix.py
--rw-r--r--   0 runner    (1001) docker     (127)     5298 2024-03-29 09:03:34.000000 inmoose-0.4.1/tests/deseq2/test_nbinomWald.py
--rw-r--r--   0 runner    (1001) docker     (127)     2137 2024-03-29 09:03:34.000000 inmoose-0.4.1/tests/deseq2/test_optim.py
--rw-r--r--   0 runner    (1001) docker     (127)     4172 2024-03-29 09:03:34.000000 inmoose-0.4.1/tests/deseq2/test_outlier.py
--rw-r--r--   0 runner    (1001) docker     (127)      125 2024-03-29 09:03:34.000000 inmoose-0.4.1/tests/deseq2/test_parallel.py
--rw-r--r--   0 runner    (1001) docker     (127)    11922 2024-03-29 09:03:34.000000 inmoose-0.4.1/tests/deseq2/test_results.py
--rw-r--r--   0 runner    (1001) docker     (127)     2896 2024-03-29 09:03:34.000000 inmoose-0.4.1/tests/deseq2/test_size_factor.py
--rw-r--r--   0 runner    (1001) docker     (127)      102 2024-03-29 09:03:34.000000 inmoose-0.4.1/tests/deseq2/test_unmix.py
--rw-r--r--   0 runner    (1001) docker     (127)    12870 2024-03-29 09:03:34.000000 inmoose-0.4.1/tests/deseq2/test_vst.py
--rw-r--r--   0 runner    (1001) docker     (127)     5196 2024-03-29 09:03:34.000000 inmoose-0.4.1/tests/deseq2/test_weights.py
--rw-r--r--   0 runner    (1001) docker     (127)     1531 2024-03-29 09:03:34.000000 inmoose-0.4.1/tests/deseq2/test_zero_zero.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 09:03:41.191398 inmoose-0.4.1/tests/edgepy/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-29 09:03:34.000000 inmoose-0.4.1/tests/edgepy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3816 2024-03-29 09:03:34.000000 inmoose-0.4.1/tests/edgepy/test_DGEList.py
--rw-r--r--   0 runner    (1001) docker     (127)     2239 2024-03-29 09:03:34.000000 inmoose-0.4.1/tests/edgepy/test_addPriorCount.py
--rw-r--r--   0 runner    (1001) docker     (127)     2009 2024-03-29 09:03:34.000000 inmoose-0.4.1/tests/edgepy/test_aveLogCPM.py
--rw-r--r--   0 runner    (1001) docker     (127)     1930 2024-03-29 09:03:34.000000 inmoose-0.4.1/tests/edgepy/test_compressMatrix.py
--rw-r--r--   0 runner    (1001) docker     (127)     8707 2024-03-29 09:03:34.000000 inmoose-0.4.1/tests/edgepy/test_dispersion.py
--rw-r--r--   0 runner    (1001) docker     (127)     9961 2024-03-29 09:03:34.000000 inmoose-0.4.1/tests/edgepy/test_exactTest.py
--rw-r--r--   0 runner    (1001) docker     (127)    17266 2024-03-29 09:03:34.000000 inmoose-0.4.1/tests/edgepy/test_glm.py
--rw-r--r--   0 runner    (1001) docker     (127)     1307 2024-03-29 09:03:34.000000 inmoose-0.4.1/tests/edgepy/test_lik.py
--rw-r--r--   0 runner    (1001) docker     (127)     9995 2024-03-29 09:03:34.000000 inmoose-0.4.1/tests/edgepy/test_mglm.py
--rw-r--r--   0 runner    (1001) docker     (127)     1913 2024-03-29 09:03:34.000000 inmoose-0.4.1/tests/edgepy/test_nbinomDeviance.py
--rw-r--r--   0 runner    (1001) docker     (127)      623 2024-03-29 09:03:34.000000 inmoose-0.4.1/tests/edgepy/test_objects.py
--rw-r--r--   0 runner    (1001) docker     (127)     1657 2024-03-29 09:03:34.000000 inmoose-0.4.1/tests/edgepy/test_predFC.py
--rw-r--r--   0 runner    (1001) docker     (127)     1031 2024-03-29 09:03:34.000000 inmoose-0.4.1/tests/edgepy/test_q2qnbinom.py
--rw-r--r--   0 runner    (1001) docker     (127)     1199 2024-03-29 09:03:34.000000 inmoose-0.4.1/tests/edgepy/test_stats.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 09:03:41.191398 inmoose-0.4.1/tests/limma/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-29 09:03:34.000000 inmoose-0.4.1/tests/limma/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      474 2024-03-29 09:03:34.000000 inmoose-0.4.1/tests/limma/test_fitFDist.py
--rw-r--r--   0 runner    (1001) docker     (127)     1449 2024-03-29 09:03:34.000000 inmoose-0.4.1/tests/limma/test_squeezeVar.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 09:03:41.191398 inmoose-0.4.1/tests/pycombat/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-29 09:03:34.000000 inmoose-0.4.1/tests/pycombat/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4827 2024-03-29 09:03:34.000000 inmoose-0.4.1/tests/pycombat/test_covariates.py
--rw-r--r--   0 runner    (1001) docker     (127)     5986 2024-03-29 09:03:34.000000 inmoose-0.4.1/tests/pycombat/test_pycombat.py
--rw-r--r--   0 runner    (1001) docker     (127)     9133 2024-03-29 09:03:34.000000 inmoose-0.4.1/tests/pycombat/test_pycombatseq.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 09:03:41.191398 inmoose-0.4.1/tests/sim/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-29 09:03:34.000000 inmoose-0.4.1/tests/sim/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      548 2024-03-29 09:03:34.000000 inmoose-0.4.1/tests/sim/test_splat.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 09:03:41.191398 inmoose-0.4.1/tests/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-29 09:03:34.000000 inmoose-0.4.1/tests/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1878 2024-03-29 09:03:34.000000 inmoose-0.4.1/tests/utils/test_factor.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 13:32:44.122455 inmoose-0.5.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-06-03 13:32:31.000000 inmoose-0.5.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       70 2024-06-03 13:32:31.000000 inmoose-0.5.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     4811 2024-06-03 13:32:44.122455 inmoose-0.5.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3734 2024-06-03 13:32:31.000000 inmoose-0.5.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 13:32:44.046455 inmoose-0.5.0/inmoose/
+-rw-r--r--   0 runner    (1001) docker     (127)      712 2024-06-03 13:32:31.000000 inmoose-0.5.0/inmoose/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 13:32:44.050455 inmoose-0.5.0/inmoose/common_cpp/
+-rw-r--r--   0 runner    (1001) docker     (127)      962 2024-06-03 13:32:31.000000 inmoose-0.5.0/inmoose/common_cpp/common_cpp.pyx
+-rw-r--r--   0 runner    (1001) docker     (127)     2836 2024-06-03 13:32:31.000000 inmoose-0.5.0/inmoose/common_cpp/matrix.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     9126 2024-06-03 13:32:31.000000 inmoose-0.5.0/inmoose/common_cpp/matrix.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 13:32:44.050455 inmoose-0.5.0/inmoose/consensus_clustering/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 13:32:31.000000 inmoose-0.5.0/inmoose/consensus_clustering/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20311 2024-06-03 13:32:31.000000 inmoose-0.5.0/inmoose/consensus_clustering/consensus_clustering.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 13:32:44.046455 inmoose-0.5.0/inmoose/data/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 13:32:44.050455 inmoose-0.5.0/inmoose/data/airway/
+-rw-r--r--   0 runner    (1001) docker     (127)      401 2024-06-03 13:32:31.000000 inmoose-0.5.0/inmoose/data/airway/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)  5154656 2024-06-03 13:32:31.000000 inmoose-0.5.0/inmoose/data/airway/airway.h5ad
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 13:32:44.082455 inmoose-0.5.0/inmoose/data/pasilla/
+-rw-r--r--   0 runner    (1001) docker     (127) 13589253 2024-06-03 13:32:31.000000 inmoose-0.5.0/inmoose/data/pasilla/Dmel.BDGP5.25.62.DEXSeq.chr.gff
+-rw-r--r--   0 runner    (1001) docker     (127)     1083 2024-06-03 13:32:31.000000 inmoose-0.5.0/inmoose/data/pasilla/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      552 2024-06-03 13:32:31.000000 inmoose-0.5.0/inmoose/data/pasilla/geneIDsinsubset.txt
+-rw-r--r--   0 runner    (1001) docker     (127)   498373 2024-06-03 13:32:31.000000 inmoose-0.5.0/inmoose/data/pasilla/pasilla_gene_counts.tsv
+-rw-r--r--   0 runner    (1001) docker     (127)      527 2024-06-03 13:32:31.000000 inmoose-0.5.0/inmoose/data/pasilla/pasilla_sample_annotation.csv
+-rw-r--r--   0 runner    (1001) docker     (127)  1370030 2024-06-03 13:32:31.000000 inmoose-0.5.0/inmoose/data/pasilla/treated1fb.txt
+-rw-r--r--   0 runner    (1001) docker     (127)  1359480 2024-06-03 13:32:31.000000 inmoose-0.5.0/inmoose/data/pasilla/treated2fb.txt
+-rw-r--r--   0 runner    (1001) docker     (127)  1361730 2024-06-03 13:32:31.000000 inmoose-0.5.0/inmoose/data/pasilla/treated3fb.txt
+-rw-r--r--   0 runner    (1001) docker     (127)  1363665 2024-06-03 13:32:31.000000 inmoose-0.5.0/inmoose/data/pasilla/untreated1fb.txt
+-rw-r--r--   0 runner    (1001) docker     (127)  1371149 2024-06-03 13:32:31.000000 inmoose-0.5.0/inmoose/data/pasilla/untreated2fb.txt
+-rw-r--r--   0 runner    (1001) docker     (127)  1358790 2024-06-03 13:32:31.000000 inmoose-0.5.0/inmoose/data/pasilla/untreated3fb.txt
+-rw-r--r--   0 runner    (1001) docker     (127)  1359414 2024-06-03 13:32:31.000000 inmoose-0.5.0/inmoose/data/pasilla/untreated4fb.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 13:32:44.090455 inmoose-0.5.0/inmoose/deseq2/
+-rw-r--r--   0 runner    (1001) docker     (127)    25648 2024-06-03 13:32:31.000000 inmoose-0.5.0/inmoose/deseq2/DESeqDataSet.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1725 2024-06-03 13:32:31.000000 inmoose-0.5.0/inmoose/deseq2/DESeqTransform.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3565 2024-06-03 13:32:31.000000 inmoose-0.5.0/inmoose/deseq2/Hmisc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1123 2024-06-03 13:32:31.000000 inmoose-0.5.0/inmoose/deseq2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15261 2024-06-03 13:32:31.000000 inmoose-0.5.0/inmoose/deseq2/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35060 2024-06-03 13:32:31.000000 inmoose-0.5.0/inmoose/deseq2/deseq2_cpp.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36066 2024-06-03 13:32:31.000000 inmoose-0.5.0/inmoose/deseq2/dispersions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10482 2024-06-03 13:32:31.000000 inmoose-0.5.0/inmoose/deseq2/estimateSizeFactors.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19849 2024-06-03 13:32:31.000000 inmoose-0.5.0/inmoose/deseq2/fitNbinomGLMs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4538 2024-06-03 13:32:31.000000 inmoose-0.5.0/inmoose/deseq2/lrt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3436 2024-06-03 13:32:31.000000 inmoose-0.5.0/inmoose/deseq2/misc.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10299 2024-06-03 13:32:31.000000 inmoose-0.5.0/inmoose/deseq2/outliers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2873 2024-06-03 13:32:31.000000 inmoose-0.5.0/inmoose/deseq2/parallel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8040 2024-06-03 13:32:31.000000 inmoose-0.5.0/inmoose/deseq2/plot.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5422 2024-06-03 13:32:31.000000 inmoose-0.5.0/inmoose/deseq2/prior.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4221 2024-06-03 13:32:31.000000 inmoose-0.5.0/inmoose/deseq2/replicates.py
+-rw-r--r--   0 runner    (1001) docker     (127)    54441 2024-06-03 13:32:31.000000 inmoose-0.5.0/inmoose/deseq2/results.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12875 2024-06-03 13:32:31.000000 inmoose-0.5.0/inmoose/deseq2/vst.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21333 2024-06-03 13:32:31.000000 inmoose-0.5.0/inmoose/deseq2/wald.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4842 2024-06-03 13:32:31.000000 inmoose-0.5.0/inmoose/deseq2/weights.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 13:32:44.094455 inmoose-0.5.0/inmoose/edgepy/
+-rw-r--r--   0 runner    (1001) docker     (127)     1158 2024-06-03 13:32:31.000000 inmoose-0.5.0/inmoose/edgepy/DGEExact.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2593 2024-06-03 13:32:31.000000 inmoose-0.5.0/inmoose/edgepy/DGEGLM.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1287 2024-06-03 13:32:31.000000 inmoose-0.5.0/inmoose/edgepy/DGELRT.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9307 2024-06-03 13:32:31.000000 inmoose-0.5.0/inmoose/edgepy/DGEList.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2044 2024-06-03 13:32:31.000000 inmoose-0.5.0/inmoose/edgepy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4237 2024-06-03 13:32:31.000000 inmoose-0.5.0/inmoose/edgepy/addPriorCount.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5474 2024-06-03 13:32:31.000000 inmoose-0.5.0/inmoose/edgepy/adjustedProfileLik.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7516 2024-06-03 13:32:31.000000 inmoose-0.5.0/inmoose/edgepy/aveLogCPM.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5042 2024-06-03 13:32:31.000000 inmoose-0.5.0/inmoose/edgepy/binomTest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6135 2024-06-03 13:32:31.000000 inmoose-0.5.0/inmoose/edgepy/dispCoxReid.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7748 2024-06-03 13:32:31.000000 inmoose-0.5.0/inmoose/edgepy/dispCoxReidInterpolateTagwise.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 13:32:44.098455 inmoose-0.5.0/inmoose/edgepy/edgepy_cpp/
+-rw-r--r--   0 runner    (1001) docker     (127)     6166 2024-06-03 13:32:31.000000 inmoose-0.5.0/inmoose/edgepy/edgepy_cpp/__init__.pxd
+-rw-r--r--   0 runner    (1001) docker     (127)     3085 2024-06-03 13:32:31.000000 inmoose-0.5.0/inmoose/edgepy/edgepy_cpp/add_prior.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1583 2024-06-03 13:32:31.000000 inmoose-0.5.0/inmoose/edgepy/edgepy_cpp/add_prior.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3110 2024-06-03 13:32:31.000000 inmoose-0.5.0/inmoose/edgepy/edgepy_cpp/add_prior_count.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)      869 2024-06-03 13:32:31.000000 inmoose-0.5.0/inmoose/edgepy/edgepy_cpp/add_prior_count.h
+-rw-r--r--   0 runner    (1001) docker     (127)     5168 2024-06-03 13:32:31.000000 inmoose-0.5.0/inmoose/edgepy/edgepy_cpp/adj_coxreid.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2568 2024-06-03 13:32:31.000000 inmoose-0.5.0/inmoose/edgepy/edgepy_cpp/ave_log_cpm.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     5065 2024-06-03 13:32:31.000000 inmoose-0.5.0/inmoose/edgepy/edgepy_cpp/compute_apl.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     3796 2024-06-03 13:32:31.000000 inmoose-0.5.0/inmoose/edgepy/edgepy_cpp/compute_nbdev.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     8270 2024-06-03 13:32:31.000000 inmoose-0.5.0/inmoose/edgepy/edgepy_cpp/edgepy_cpp.pyx
+-rw-r--r--   0 runner    (1001) docker     (127)     3507 2024-06-03 13:32:31.000000 inmoose-0.5.0/inmoose/edgepy/edgepy_cpp/fit_levenberg.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)      955 2024-06-03 13:32:31.000000 inmoose-0.5.0/inmoose/edgepy/edgepy_cpp/fit_levenberg.h
+-rw-r--r--   0 runner    (1001) docker     (127)     4692 2024-06-03 13:32:31.000000 inmoose-0.5.0/inmoose/edgepy/edgepy_cpp/fit_one_group.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2371 2024-06-03 13:32:31.000000 inmoose-0.5.0/inmoose/edgepy/edgepy_cpp/get_one_way_fitted.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2273 2024-06-03 13:32:31.000000 inmoose-0.5.0/inmoose/edgepy/edgepy_cpp/glm.h
+-rw-r--r--   0 runner    (1001) docker     (127)    11007 2024-06-03 13:32:31.000000 inmoose-0.5.0/inmoose/edgepy/edgepy_cpp/glm_levenberg.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2625 2024-06-03 13:32:31.000000 inmoose-0.5.0/inmoose/edgepy/edgepy_cpp/glm_one_group.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     6064 2024-06-03 13:32:31.000000 inmoose-0.5.0/inmoose/edgepy/edgepy_cpp/initialize_levenberg.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1137 2024-06-03 13:32:31.000000 inmoose-0.5.0/inmoose/edgepy/edgepy_cpp/initialize_levenberg.h
+-rw-r--r--   0 runner    (1001) docker     (127)     7061 2024-06-03 13:32:31.000000 inmoose-0.5.0/inmoose/edgepy/edgepy_cpp/interpolator.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1308 2024-06-03 13:32:31.000000 inmoose-0.5.0/inmoose/edgepy/edgepy_cpp/interpolator.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1880 2024-06-03 13:32:31.000000 inmoose-0.5.0/inmoose/edgepy/edgepy_cpp/maximize_interpolant.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     5066 2024-06-03 13:32:31.000000 inmoose-0.5.0/inmoose/edgepy/edgepy_cpp/objects.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1957 2024-06-03 13:32:31.000000 inmoose-0.5.0/inmoose/edgepy/edgepy_cpp/objects.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1801 2024-06-03 13:32:31.000000 inmoose-0.5.0/inmoose/edgepy/edgepy_cpp/utils.h
+-rw-r--r--   0 runner    (1001) docker     (127)     6004 2024-06-03 13:32:31.000000 inmoose-0.5.0/inmoose/edgepy/estimateGLMCommonDisp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7366 2024-06-03 13:32:31.000000 inmoose-0.5.0/inmoose/edgepy/estimateGLMTagwiseDisp.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10780 2024-06-03 13:32:31.000000 inmoose-0.5.0/inmoose/edgepy/exactTest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3388 2024-06-03 13:32:31.000000 inmoose-0.5.0/inmoose/edgepy/exactTestBetaApprox.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5414 2024-06-03 13:32:31.000000 inmoose-0.5.0/inmoose/edgepy/exactTestByDeviance.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4540 2024-06-03 13:32:31.000000 inmoose-0.5.0/inmoose/edgepy/exactTestBySmallP.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4582 2024-06-03 13:32:31.000000 inmoose-0.5.0/inmoose/edgepy/exactTestDoubleTail.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17019 2024-06-03 13:32:31.000000 inmoose-0.5.0/inmoose/edgepy/glmFit.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15621 2024-06-03 13:32:31.000000 inmoose-0.5.0/inmoose/edgepy/glmQLFit.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5146 2024-06-03 13:32:31.000000 inmoose-0.5.0/inmoose/edgepy/makeCompressedMatrix.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2678 2024-06-03 13:32:31.000000 inmoose-0.5.0/inmoose/edgepy/maximizeInterpolant.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5852 2024-06-03 13:32:31.000000 inmoose-0.5.0/inmoose/edgepy/mglmLevenberg.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4864 2024-06-03 13:32:31.000000 inmoose-0.5.0/inmoose/edgepy/mglmOneGroup.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7925 2024-06-03 13:32:31.000000 inmoose-0.5.0/inmoose/edgepy/mglmOneWay.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2666 2024-06-03 13:32:31.000000 inmoose-0.5.0/inmoose/edgepy/movingAverageByCol.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4502 2024-06-03 13:32:31.000000 inmoose-0.5.0/inmoose/edgepy/nbinomDeviance.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4901 2024-06-03 13:32:31.000000 inmoose-0.5.0/inmoose/edgepy/predFC.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2733 2024-06-03 13:32:31.000000 inmoose-0.5.0/inmoose/edgepy/q2qnbinom.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2848 2024-06-03 13:32:31.000000 inmoose-0.5.0/inmoose/edgepy/residDF.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2660 2024-06-03 13:32:31.000000 inmoose-0.5.0/inmoose/edgepy/splitIntoGroups.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5006 2024-06-03 13:32:31.000000 inmoose-0.5.0/inmoose/edgepy/stats.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1774 2024-06-03 13:32:31.000000 inmoose-0.5.0/inmoose/edgepy/systematicSubset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7308 2024-06-03 13:32:31.000000 inmoose-0.5.0/inmoose/edgepy/topTags.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1883 2024-06-03 13:32:31.000000 inmoose-0.5.0/inmoose/edgepy/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1954 2024-06-03 13:32:31.000000 inmoose-0.5.0/inmoose/edgepy/validDGEList.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 13:32:44.102455 inmoose-0.5.0/inmoose/limma/
+-rw-r--r--   0 runner    (1001) docker     (127)      761 2024-06-03 13:32:31.000000 inmoose-0.5.0/inmoose/limma/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10230 2024-06-03 13:32:31.000000 inmoose-0.5.0/inmoose/limma/contrasts.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10885 2024-06-03 13:32:31.000000 inmoose-0.5.0/inmoose/limma/decidetests.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3302 2024-06-03 13:32:31.000000 inmoose-0.5.0/inmoose/limma/dups.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18660 2024-06-03 13:32:31.000000 inmoose-0.5.0/inmoose/limma/ebayes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8311 2024-06-03 13:32:31.000000 inmoose-0.5.0/inmoose/limma/fitFDist.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16920 2024-06-03 13:32:31.000000 inmoose-0.5.0/inmoose/limma/lmfit.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6337 2024-06-03 13:32:31.000000 inmoose-0.5.0/inmoose/limma/marraylm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5950 2024-06-03 13:32:31.000000 inmoose-0.5.0/inmoose/limma/squeezeVar.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18587 2024-06-03 13:32:31.000000 inmoose-0.5.0/inmoose/limma/toptable.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 13:32:44.102455 inmoose-0.5.0/inmoose/pycombat/
+-rw-r--r--   0 runner    (1001) docker     (127)      113 2024-06-03 13:32:31.000000 inmoose-0.5.0/inmoose/pycombat/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17852 2024-06-03 13:32:31.000000 inmoose-0.5.0/inmoose/pycombat/covariates.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3366 2024-06-03 13:32:31.000000 inmoose-0.5.0/inmoose/pycombat/helper_seq.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22170 2024-06-03 13:32:31.000000 inmoose-0.5.0/inmoose/pycombat/pycombat_norm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8884 2024-06-03 13:32:31.000000 inmoose-0.5.0/inmoose/pycombat/pycombat_seq.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 13:32:44.102455 inmoose-0.5.0/inmoose/sim/
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-06-03 13:32:31.000000 inmoose-0.5.0/inmoose/sim/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8408 2024-06-03 13:32:31.000000 inmoose-0.5.0/inmoose/sim/splat.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 13:32:44.102455 inmoose-0.5.0/inmoose/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      474 2024-06-03 13:32:31.000000 inmoose-0.5.0/inmoose/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1118 2024-06-03 13:32:31.000000 inmoose-0.5.0/inmoose/utils/_stats.pyx
+-rw-r--r--   0 runner    (1001) docker     (127)     1738 2024-06-03 13:32:31.000000 inmoose-0.5.0/inmoose/utils/factor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1301 2024-06-03 13:32:31.000000 inmoose-0.5.0/inmoose/utils/linalg.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3977 2024-06-03 13:32:31.000000 inmoose-0.5.0/inmoose/utils/lm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8375 2024-06-03 13:32:31.000000 inmoose-0.5.0/inmoose/utils/splines.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5316 2024-06-03 13:32:31.000000 inmoose-0.5.0/inmoose/utils/stats.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 13:32:44.122455 inmoose-0.5.0/inmoose.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4811 2024-06-03 13:32:44.000000 inmoose-0.5.0/inmoose.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6255 2024-06-03 13:32:44.000000 inmoose-0.5.0/inmoose.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-03 13:32:44.000000 inmoose-0.5.0/inmoose.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      150 2024-06-03 13:32:44.000000 inmoose-0.5.0/inmoose.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      223 2024-06-03 13:32:44.000000 inmoose-0.5.0/inmoose.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1050 2024-06-03 13:32:31.000000 inmoose-0.5.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-06-03 13:32:44.122455 inmoose-0.5.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     3396 2024-06-03 13:32:31.000000 inmoose-0.5.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 13:32:44.102455 inmoose-0.5.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-03 13:32:31.000000 inmoose-0.5.0/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 13:32:44.114455 inmoose-0.5.0/tests/consensus_clustering/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 13:32:31.000000 inmoose-0.5.0/tests/consensus_clustering/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)  6796249 2024-06-03 13:32:31.000000 inmoose-0.5.0/tests/consensus_clustering/mocked_data_consensus_clustering.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     3556 2024-06-03 13:32:31.000000 inmoose-0.5.0/tests/consensus_clustering/test_consensus_clustering.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 13:32:44.114455 inmoose-0.5.0/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 13:32:31.000000 inmoose-0.5.0/tests/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      324 2024-06-03 13:32:31.000000 inmoose-0.5.0/tests/data/test_airway.py
+-rw-r--r--   0 runner    (1001) docker     (127)      334 2024-06-03 13:32:31.000000 inmoose-0.5.0/tests/data/test_pasilla.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 13:32:44.118455 inmoose-0.5.0/tests/deseq2/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 13:32:31.000000 inmoose-0.5.0/tests/deseq2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2176 2024-06-03 13:32:31.000000 inmoose-0.5.0/tests/deseq2/test_DESeq.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2256 2024-06-03 13:32:31.000000 inmoose-0.5.0/tests/deseq2/test_DESeqDataSet.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1982 2024-06-03 13:32:31.000000 inmoose-0.5.0/tests/deseq2/test_LRT.py
+-rw-r--r--   0 runner    (1001) docker     (127)      527 2024-06-03 13:32:31.000000 inmoose-0.5.0/tests/deseq2/test_QR.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1206 2024-06-03 13:32:31.000000 inmoose-0.5.0/tests/deseq2/test_addMLE.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2318 2024-06-03 13:32:31.000000 inmoose-0.5.0/tests/deseq2/test_betaFitting.py
+-rw-r--r--   0 runner    (1001) docker     (127)      603 2024-06-03 13:32:31.000000 inmoose-0.5.0/tests/deseq2/test_collapse.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7495 2024-06-03 13:32:31.000000 inmoose-0.5.0/tests/deseq2/test_dispersions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      483 2024-06-03 13:32:31.000000 inmoose-0.5.0/tests/deseq2/test_fpkm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1521 2024-06-03 13:32:31.000000 inmoose-0.5.0/tests/deseq2/test_interactions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1157 2024-06-03 13:32:31.000000 inmoose-0.5.0/tests/deseq2/test_linear_mu.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1433 2024-06-03 13:32:31.000000 inmoose-0.5.0/tests/deseq2/test_methods.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2121 2024-06-03 13:32:31.000000 inmoose-0.5.0/tests/deseq2/test_model_matrix.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5301 2024-06-03 13:32:31.000000 inmoose-0.5.0/tests/deseq2/test_nbinomWald.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2138 2024-06-03 13:32:31.000000 inmoose-0.5.0/tests/deseq2/test_optim.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4173 2024-06-03 13:32:31.000000 inmoose-0.5.0/tests/deseq2/test_outlier.py
+-rw-r--r--   0 runner    (1001) docker     (127)      125 2024-06-03 13:32:31.000000 inmoose-0.5.0/tests/deseq2/test_parallel.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11925 2024-06-03 13:32:31.000000 inmoose-0.5.0/tests/deseq2/test_results.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2897 2024-06-03 13:32:31.000000 inmoose-0.5.0/tests/deseq2/test_size_factor.py
+-rw-r--r--   0 runner    (1001) docker     (127)      102 2024-06-03 13:32:31.000000 inmoose-0.5.0/tests/deseq2/test_unmix.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12871 2024-06-03 13:32:31.000000 inmoose-0.5.0/tests/deseq2/test_vst.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5184 2024-06-03 13:32:31.000000 inmoose-0.5.0/tests/deseq2/test_weights.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1532 2024-06-03 13:32:31.000000 inmoose-0.5.0/tests/deseq2/test_zero_zero.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 13:32:44.118455 inmoose-0.5.0/tests/edgepy/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 13:32:31.000000 inmoose-0.5.0/tests/edgepy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3798 2024-06-03 13:32:31.000000 inmoose-0.5.0/tests/edgepy/test_DGEList.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2240 2024-06-03 13:32:31.000000 inmoose-0.5.0/tests/edgepy/test_addPriorCount.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2010 2024-06-03 13:32:31.000000 inmoose-0.5.0/tests/edgepy/test_aveLogCPM.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1931 2024-06-03 13:32:31.000000 inmoose-0.5.0/tests/edgepy/test_compressMatrix.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8708 2024-06-03 13:32:31.000000 inmoose-0.5.0/tests/edgepy/test_dispersion.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9962 2024-06-03 13:32:31.000000 inmoose-0.5.0/tests/edgepy/test_exactTest.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17267 2024-06-03 13:32:31.000000 inmoose-0.5.0/tests/edgepy/test_glm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1308 2024-06-03 13:32:31.000000 inmoose-0.5.0/tests/edgepy/test_lik.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9996 2024-06-03 13:32:31.000000 inmoose-0.5.0/tests/edgepy/test_mglm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1914 2024-06-03 13:32:31.000000 inmoose-0.5.0/tests/edgepy/test_nbinomDeviance.py
+-rw-r--r--   0 runner    (1001) docker     (127)      624 2024-06-03 13:32:31.000000 inmoose-0.5.0/tests/edgepy/test_objects.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1658 2024-06-03 13:32:31.000000 inmoose-0.5.0/tests/edgepy/test_predFC.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1001 2024-06-03 13:32:31.000000 inmoose-0.5.0/tests/edgepy/test_q2qnbinom.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1180 2024-06-03 13:32:31.000000 inmoose-0.5.0/tests/edgepy/test_stats.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 13:32:44.122455 inmoose-0.5.0/tests/limma/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 13:32:31.000000 inmoose-0.5.0/tests/limma/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      867 2024-06-03 13:32:31.000000 inmoose-0.5.0/tests/limma/test_contrasts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1220 2024-06-03 13:32:31.000000 inmoose-0.5.0/tests/limma/test_decidetests.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1882 2024-06-03 13:32:31.000000 inmoose-0.5.0/tests/limma/test_dups.py
+-rw-r--r--   0 runner    (1001) docker     (127)      440 2024-06-03 13:32:31.000000 inmoose-0.5.0/tests/limma/test_fitFDist.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26661 2024-06-03 13:32:31.000000 inmoose-0.5.0/tests/limma/test_lmFit.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1450 2024-06-03 13:32:31.000000 inmoose-0.5.0/tests/limma/test_squeezeVar.py
+-rw-r--r--   0 runner    (1001) docker     (127)      798 2024-06-03 13:32:31.000000 inmoose-0.5.0/tests/limma/test_tmixture.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 13:32:44.122455 inmoose-0.5.0/tests/pycombat/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 13:32:31.000000 inmoose-0.5.0/tests/pycombat/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4828 2024-06-03 13:32:31.000000 inmoose-0.5.0/tests/pycombat/test_covariates.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5857 2024-06-03 13:32:31.000000 inmoose-0.5.0/tests/pycombat/test_pycombat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9134 2024-06-03 13:32:31.000000 inmoose-0.5.0/tests/pycombat/test_pycombatseq.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 13:32:44.122455 inmoose-0.5.0/tests/sim/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 13:32:31.000000 inmoose-0.5.0/tests/sim/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      548 2024-06-03 13:32:31.000000 inmoose-0.5.0/tests/sim/test_splat.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 13:32:44.122455 inmoose-0.5.0/tests/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 13:32:31.000000 inmoose-0.5.0/tests/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1879 2024-06-03 13:32:31.000000 inmoose-0.5.0/tests/utils/test_factor.py
+-rw-r--r--   0 runner    (1001) docker     (127)      283 2024-06-03 13:32:31.000000 inmoose-0.5.0/tests/utils/test_linalg.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1480 2024-06-03 13:32:31.000000 inmoose-0.5.0/tests/utils/test_lm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1581 2024-06-03 13:32:31.000000 inmoose-0.5.0/tests/utils/test_splines.py
```

### Comparing `inmoose-0.4.1/LICENSE` & `inmoose-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `inmoose-0.4.1/PKG-INFO` & `inmoose-0.5.0/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: inmoose
-Version: 0.4.1
+Version: 0.5.0
 Summary: InMoose: the Integrated Multi Omic Open Source Environment
 Author-email: Maximilien Colange <maximilien@epigenelabs.com>, Léa Meunier <lea@epigenelabs.com>, Solène Weill <solene@epigenelabs.com>
 Project-URL: Source, https://github.com/epigenelabs/inmoose
 Project-URL: Documentation, https://inmoose.readthedocs.io/en/latest/
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
@@ -45,18 +45,18 @@
 
 Documentation is hosted on [readthedocs.org](https://inmoose.readthedocs.io/en/latest/).
 
 # Batch Effect Correction
 
 InMoose provides features to correct technical biases, also called batch
 effects, in transcriptomic data:
-- for microarray data, InMoose supersedes pyCombat [1], a Python 3
+- for microarray data, InMoose supersedes pyCombat [1], a Python3
   implementation of ComBat [2], one of the most widely used tool for batch effect
   correction on microarray data.
-- for RNASeq, InMoose features a port to Python3 of ComBat-Seq [3], one of the
+- for RNASeq data, InMoose features a port to Python3 of ComBat-Seq [3], one of the
   most widely used tool for batch effect correction on RNASeq data.
 
 To use these functions, simply import them and call them with default
 parameters:
 ```python
 from inmoose.pycombat import pycombat_norm, pycombat_seq
 
@@ -66,14 +66,27 @@
 
 * `microarray_data`, `rnaseq_data`: the expression matrices, containing the
   information about the gene expression (rows) for each sample (columns).
 * `microarray_batches`, `rnaseq_batches`: list of batch indices, describing the
   batch for each sample. The list of batches should contain as many elements as
   the number of samples in the expression matrix.
 
+# Differential Expression Analysis
+
+InMoose provides features to analyse diffentially expressed genes in bulk
+transcriptomic data:
+- for microarray data, InMoose features a port of limma [4], the *de
+  facto* standard tool for differential expression analysis on microarray data.
+- for RNASeq data, InMoose features a ports to Python3 of edgeR [5] and DESeq2
+  [6], two of the most widely used tools for differential expression analysis on
+  RNASeq data.
+
+See the dedicated sections of the
+[documentation](https://inmoose.readthedocs.io/en/latest/).
+
 # Consensus clustering
 InMoose provides features to compute consensus clustering, a resampling based algorithm compatible with any clustering algorithms which class implementation is instantiated with parameter `n_clusters`, and possess a `fit_predict` method, which is invoked on data.
 Consensus clustering helps determining the best number of clusters to use and output confidence metrics and plots.
 
 
 To use these functions, import the consensusClustering class and a clustering algorithm class:
 ```python
```

### Comparing `inmoose-0.4.1/README.md` & `inmoose-0.5.0/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -17,18 +17,18 @@
 
 Documentation is hosted on [readthedocs.org](https://inmoose.readthedocs.io/en/latest/).
 
 # Batch Effect Correction
 
 InMoose provides features to correct technical biases, also called batch
 effects, in transcriptomic data:
-- for microarray data, InMoose supersedes pyCombat [1], a Python 3
+- for microarray data, InMoose supersedes pyCombat [1], a Python3
   implementation of ComBat [2], one of the most widely used tool for batch effect
   correction on microarray data.
-- for RNASeq, InMoose features a port to Python3 of ComBat-Seq [3], one of the
+- for RNASeq data, InMoose features a port to Python3 of ComBat-Seq [3], one of the
   most widely used tool for batch effect correction on RNASeq data.
 
 To use these functions, simply import them and call them with default
 parameters:
 ```python
 from inmoose.pycombat import pycombat_norm, pycombat_seq
 
@@ -38,14 +38,27 @@
 
 * `microarray_data`, `rnaseq_data`: the expression matrices, containing the
   information about the gene expression (rows) for each sample (columns).
 * `microarray_batches`, `rnaseq_batches`: list of batch indices, describing the
   batch for each sample. The list of batches should contain as many elements as
   the number of samples in the expression matrix.
 
+# Differential Expression Analysis
+
+InMoose provides features to analyse diffentially expressed genes in bulk
+transcriptomic data:
+- for microarray data, InMoose features a port of limma [4], the *de
+  facto* standard tool for differential expression analysis on microarray data.
+- for RNASeq data, InMoose features a ports to Python3 of edgeR [5] and DESeq2
+  [6], two of the most widely used tools for differential expression analysis on
+  RNASeq data.
+
+See the dedicated sections of the
+[documentation](https://inmoose.readthedocs.io/en/latest/).
+
 # Consensus clustering
 InMoose provides features to compute consensus clustering, a resampling based algorithm compatible with any clustering algorithms which class implementation is instantiated with parameter `n_clusters`, and possess a `fit_predict` method, which is invoked on data.
 Consensus clustering helps determining the best number of clusters to use and output confidence metrics and plots.
 
 
 To use these functions, import the consensusClustering class and a clustering algorithm class:
 ```python
```

### Comparing `inmoose-0.4.1/inmoose/__init__.py` & `inmoose-0.5.0/inmoose/__init__.py`

 * *Files 24% similar despite different names*

```diff
@@ -4,22 +4,22 @@
 
 # force RTLD_GLOBAL when loading common_cpp
 from sys import getdlopenflags, setdlopenflags
 from os import RTLD_GLOBAL
 
 default_dlopen_flags = getdlopenflags()
 setdlopenflags(default_dlopen_flags | RTLD_GLOBAL)
-from . import common_cpp
+from . import common_cpp as common_cpp
 
 setdlopenflags(default_dlopen_flags)
 del default_dlopen_flags
 
-from . import edgepy
-from . import pycombat
-from . import utils
-from . import consensus_clustering
-from . import deseq2
+from . import edgepy as edgepy
+from . import pycombat as pycombat
+from . import utils as utils
+from . import consensus_clustering as consensus_clustering
+from . import deseq2 as deseq2
 
 import logging
 
 logging.basicConfig(level=logging.INFO, format="[{levelname}] {message}", style="{")
 logging.captureWarnings(True)
```

### Comparing `inmoose-0.4.1/inmoose/common_cpp/common_cpp.pyx` & `inmoose-0.5.0/inmoose/common_cpp/common_cpp.pyx`

 * *Files identical despite different names*

### Comparing `inmoose-0.4.1/inmoose/common_cpp/matrix.cpp` & `inmoose-0.5.0/inmoose/common_cpp/matrix.cpp`

 * *Files identical despite different names*

### Comparing `inmoose-0.4.1/inmoose/common_cpp/matrix.h` & `inmoose-0.5.0/inmoose/common_cpp/matrix.h`

 * *Files identical despite different names*

### Comparing `inmoose-0.4.1/inmoose/consensus_clustering/consensus_clustering.py` & `inmoose-0.5.0/inmoose/consensus_clustering/consensus_clustering.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,21 +15,22 @@
 # You should have received a copy of the GNU General Public License
 # along with this program.  If not, see <https://www.gnu.org/licenses/>.
 # -----------------------------------------------------------------------------
 
 # This file is based on the file 'consensusClustering.py' of the repository
 # github.com/ZigaSajovic/Consensus_Clustering (as of July 30, 2021).
 
+import bisect
 import logging
-import numpy as np
 from itertools import combinations
-import bisect
-import seaborn as sn
+
 import matplotlib.pyplot as plt
+import numpy as np
 import pandas as pd
+import seaborn as sn
 
 
 class consensusClustering:
     """
     Implementation of Consensus clustering, following the paper https://link.springer.com/content/pdf/10.1023%2FA%3A1023949509487.pdf
 
     Arguments
```

### Comparing `inmoose-0.4.1/inmoose/data/airway/airway.h5ad` & `inmoose-0.5.0/inmoose/data/airway/airway.h5ad`

 * *Files identical despite different names*

### Comparing `inmoose-0.4.1/inmoose/data/pasilla/Dmel.BDGP5.25.62.DEXSeq.chr.gff` & `inmoose-0.5.0/inmoose/data/pasilla/Dmel.BDGP5.25.62.DEXSeq.chr.gff`

 * *Files identical despite different names*

### Comparing `inmoose-0.4.1/inmoose/data/pasilla/__init__.py` & `inmoose-0.5.0/inmoose/data/pasilla/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,16 +3,17 @@
     Retrieve the pasilla dataset as an :class:`AnnData` object
 
     The pasilla dataset is an RNA-Seq experiment on the effect of RNAi
     knockdown of Pasilla, the Drosophila melanogaster ortholog of mammalian
     NOVA1 and NOVA2, on the transcriptome [Brooks2011]_.
     """
     import importlib.resources
-    import pandas as pd
+
     import anndata as ad
+    import pandas as pd
 
     data_dir = importlib.resources.files("inmoose.data.pasilla")
     cts = pd.read_csv(
         data_dir.joinpath("pasilla_gene_counts.tsv"), sep="\t", index_col=0
     )
     anno = pd.read_csv(data_dir.joinpath("pasilla_sample_annotation.csv"), index_col=0)
```

### Comparing `inmoose-0.4.1/inmoose/data/pasilla/geneIDsinsubset.txt` & `inmoose-0.5.0/inmoose/data/pasilla/geneIDsinsubset.txt`

 * *Files identical despite different names*

### Comparing `inmoose-0.4.1/inmoose/data/pasilla/pasilla_gene_counts.tsv` & `inmoose-0.5.0/inmoose/data/pasilla/pasilla_gene_counts.tsv`

 * *Files identical despite different names*

### Comparing `inmoose-0.4.1/inmoose/data/pasilla/pasilla_sample_annotation.csv` & `inmoose-0.5.0/inmoose/data/pasilla/pasilla_sample_annotation.csv`

 * *Files identical despite different names*

### Comparing `inmoose-0.4.1/inmoose/data/pasilla/treated1fb.txt` & `inmoose-0.5.0/inmoose/data/pasilla/treated1fb.txt`

 * *Files identical despite different names*

### Comparing `inmoose-0.4.1/inmoose/data/pasilla/treated2fb.txt` & `inmoose-0.5.0/inmoose/data/pasilla/treated2fb.txt`

 * *Files identical despite different names*

### Comparing `inmoose-0.4.1/inmoose/data/pasilla/treated3fb.txt` & `inmoose-0.5.0/inmoose/data/pasilla/treated3fb.txt`

 * *Files identical despite different names*

### Comparing `inmoose-0.4.1/inmoose/data/pasilla/untreated1fb.txt` & `inmoose-0.5.0/inmoose/data/pasilla/untreated1fb.txt`

 * *Files identical despite different names*

### Comparing `inmoose-0.4.1/inmoose/data/pasilla/untreated2fb.txt` & `inmoose-0.5.0/inmoose/data/pasilla/untreated2fb.txt`

 * *Files identical despite different names*

### Comparing `inmoose-0.4.1/inmoose/data/pasilla/untreated3fb.txt` & `inmoose-0.5.0/inmoose/data/pasilla/untreated3fb.txt`

 * *Files identical despite different names*

### Comparing `inmoose-0.4.1/inmoose/data/pasilla/untreated4fb.txt` & `inmoose-0.5.0/inmoose/data/pasilla/untreated4fb.txt`

 * *Files identical despite different names*

### Comparing `inmoose-0.4.1/inmoose/deseq2/DESeqDataSet.py` & `inmoose-0.5.0/inmoose/deseq2/DESeqDataSet.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,16 +16,17 @@
 # along with this program.  If not, see <https://www.gnu.org/licenses/>.
 # -----------------------------------------------------------------------------
 
 # This file is based on the file 'R/AllClasses.R' and 'R/methods.R' of the
 # Bioconductor DESeq2 package (version 3.16).
 
 
-from collections import OrderedDict
 import logging
+from collections import OrderedDict
+
 import numpy as np
 import pandas as pd
 import patsy
 from anndata import AnnData
 from scipy.stats import median_abs_deviation as mad
 from scipy.stats import norm
 
@@ -95,16 +96,16 @@
     See Also
     --------
     .makeExampleDESeqDataSet
     """
 
     from .dispersions import estimateDispersions_dds as estimateDispersions
     from .estimateSizeFactors import estimateSizeFactors_dds as estimateSizeFactors
-    from .results import results_dds as results
     from .plot import plotDispEsts_dds as plotDispEsts
+    from .results import results_dds as results
 
     def __init__(self, countData, clinicalData=None, design=None, ignoreRank=False):
         """
         DESeqDataSet constructor
 
         Arguments
         ---------
```

### Comparing `inmoose-0.4.1/inmoose/deseq2/DESeqTransform.py` & `inmoose-0.5.0/inmoose/deseq2/DESeqTransform.py`

 * *Files identical despite different names*

### Comparing `inmoose-0.4.1/inmoose/deseq2/Hmisc.py` & `inmoose-0.5.0/inmoose/deseq2/Hmisc.py`

 * *Files identical despite different names*

### Comparing `inmoose-0.4.1/inmoose/deseq2/__init__.py` & `inmoose-0.5.0/inmoose/deseq2/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,17 +1,26 @@
-from .core import DESeq
-from .DESeqDataSet import DESeqDataSet, makeExampleDESeqDataSet
-from .DESeqTransform import DESeqTransform
+from .core import DESeq as DESeq
+from .DESeqDataSet import DESeqDataSet as DESeqDataSet
+from .DESeqDataSet import makeExampleDESeqDataSet as makeExampleDESeqDataSet
+from .DESeqTransform import DESeqTransform as DESeqTransform
 from .dispersions import (
-    estimateDispersionsGeneEst,
-    estimateDispersionsFit,
-    estimateDispersionsMAP,
-    estimateDispersionsPriorVar,
+    estimateDispersionsFit as estimateDispersionsFit,
 )
-from .estimateSizeFactors import estimateSizeFactorsForMatrix
-from .lrt import nbinomLRT
-from .outliers import replaceOutliers
-from .parallel import estimateMLEForBetaPriorVar
-from .prior import estimateBetaPriorVar
-from .replicates import collapseReplicates
-from .vst import varianceStabilizingTransformation
-from .wald import nbinomWaldTest
+from .dispersions import (
+    estimateDispersionsGeneEst as estimateDispersionsGeneEst,
+)
+from .dispersions import (
+    estimateDispersionsMAP as estimateDispersionsMAP,
+)
+from .dispersions import (
+    estimateDispersionsPriorVar as estimateDispersionsPriorVar,
+)
+from .estimateSizeFactors import (
+    estimateSizeFactorsForMatrix as estimateSizeFactorsForMatrix,
+)
+from .lrt import nbinomLRT as nbinomLRT
+from .outliers import replaceOutliers as replaceOutliers
+from .parallel import estimateMLEForBetaPriorVar as estimateMLEForBetaPriorVar
+from .prior import estimateBetaPriorVar as estimateBetaPriorVar
+from .replicates import collapseReplicates as collapseReplicates
+from .vst import varianceStabilizingTransformation as varianceStabilizingTransformation
+from .wald import nbinomWaldTest as nbinomWaldTest
```

### Comparing `inmoose-0.4.1/inmoose/deseq2/core.py` & `inmoose-0.5.0/inmoose/deseq2/core.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,14 +17,15 @@
 # -----------------------------------------------------------------------------
 
 # This file is based on the file 'R/core.R' of the Bioconductor DESeq2 package
 # (version 3.16).
 
 
 import logging
+
 import numpy as np
 import pandas as pd
 import patsy
 
 from .DESeqDataSet import DESeqDataSet, checkFullRank
 from .lrt import checkLRT, nbinomLRT
 from .misc import nOrMoreInCell
@@ -340,27 +341,30 @@
     else:  # if parallel
         if modelMatrixType is not None:
             if betaPrior and modelMatrixType != "expanded":
                 raise ValueError(
                     "parallelization not implemented for non-expanded matrix with beta priors"
                 )
 
-        obj = DESeqParallel(
-            obj,
-            test=test,
-            fitType=fitType,
-            betaPrior=betaPrior,
-            full=full,
-            reduced=reduced,
-            quiet=quiet,
-            modelMatrix=modelMatrix,
-            useT=useT,
-            minmu=minmu,
-            BPPARAM=BPPARAM,
+        raise NotImplementedError(
+            "parallelization is not implemented in inmoose for now"
         )
+        # obj = DESeqParallel(
+        #    obj,
+        #    test=test,
+        #    fitType=fitType,
+        #    betaPrior=betaPrior,
+        #    full=full,
+        #    reduced=reduced,
+        #    quiet=quiet,
+        #    modelMatrix=modelMatrix,
+        #    useT=useT,
+        #    minmu=minmu,
+        #    BPPARAM=BPPARAM,
+        # )
 
     # if there are sufficient replicates, then pass through to refitting function
     sufficientReps = nOrMoreInCell(obj.modelMatrix, minReplicatesForReplace).any()
     if sufficientReps:
         obj = refitWithoutOutliers(
             obj,
             test=test,
```

### Comparing `inmoose-0.4.1/inmoose/deseq2/deseq2_cpp.py` & `inmoose-0.5.0/inmoose/deseq2/deseq2_cpp.py`

 * *Files 0% similar despite different names*

```diff
@@ -25,17 +25,16 @@
 #
 # Note: the canonical, up-to-date DESeq2.cpp lives in the DESeq2 library, the
 # development branch of which can be viewed here:
 # https://github.com/mikelove/DESeq2/blob/master/src/DESeq2.cpp
 
 import numpy as np
 import pandas as pd
+from scipy.special import digamma, polygamma, xlog1py, xlogy
 from scipy.special import loggamma as lgamma
-from scipy.special import digamma, polygamma
-from scipy.special import xlog1py, xlogy
 
 from ..utils import dnbinom_mu
 
 
 def log_posterior(
     log_alpha,
     y,
@@ -1049,16 +1048,16 @@
     assert xtwxr_inv.shape == (y_n, x_p, x_p)
 
     hat_diagonals = np.zeros(y.shape)
     # this is equivalent to (for all j):
     #   hat_diagonals[:,j] = np.diag(xw[j] @ xtwxr_inv[j] @ xw[j].T)
     # but it avoids computing full matrix products just to retrieve the diags
     for k in range(x_p):
-        for l in range(x_p):
-            hat_diagonals[:, :] += (xw[:, :, k] * xw[:, :, l]).T * xtwxr_inv[:, k, l]
+        for m in range(x_p):
+            hat_diagonals[:, :] += (xw[:, :, k] * xw[:, :, m]).T * xtwxr_inv[:, k, m]
 
     # sigma is the covariance matrix for the betas
     sigma = xtwxr_inv @ x.T @ (x * w_vec.T[:, :, None]) @ xtwxr_inv
     assert sigma.shape == (y_n, x_p, x_p)
     contrast_num = contrast @ beta_mat.T
     contrast_denom = np.sqrt(contrast.T @ sigma @ contrast)
     beta_var_mat = np.diagonal(sigma, axis1=-2, axis2=-1)
```

### Comparing `inmoose-0.4.1/inmoose/deseq2/dispersions.py` & `inmoose-0.5.0/inmoose/deseq2/dispersions.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,26 +17,27 @@
 # -----------------------------------------------------------------------------
 
 # This file is based on the file 'R/core.R' of the Bioconductor DESeq2 package
 # (version 3.16).
 
 
 import logging
+
 import numpy as np
 import pandas as pd
+import statsmodels.api as sm
 from scipy.special import polygamma
 from scipy.stats import trim_mean
-import statsmodels.api as sm
 from statsmodels.tools.sm_exceptions import DomainWarning
 
 from ..utils import Factor
+from .deseq2_cpp import fitDispGridWrapper, fitDispWrapper
 from .fitNbinomGLMs import fitNbinomGLMs
-from .misc import checkFullRank, buildMatrixWithNACols, buildVectorWithNACols
+from .misc import buildMatrixWithNACols, buildVectorWithNACols, checkFullRank
 from .weights import getAndCheckWeights
-from .deseq2_cpp import fitDispWrapper, fitDispGridWrapper
 
 
 def estimateDispersions_dds(
     obj,
     fitType="parametric",
     maxit=100,
     useCR=True,
@@ -519,15 +520,18 @@
         # disps = objNZ.var["dispGeneEst"][useForFit],
         # minDisp = minDisp)
 
     if fitType == "mean":
         useForMean = objNZ.var["dispGeneEst"] > 10 * minDisp
         useForMean = useForMean & ~np.isnan(objNZ.var["dispGeneEst"])
         meanDisp = trim_mean(objNZ.var["dispGeneEst"][useForMean], 0.001)
-        dispFunction = lambda means: meanDisp
+
+        def dispFunction(means):
+            return meanDisp
+
         dispFunction.mean = meanDisp
 
     if fitType == "glmGamPoi":
         raise NotImplementedError()
 
     # store the dispersion function and attributes
     dispFunction.fitType = fitType
@@ -790,15 +794,15 @@
     """
     objNZ = obj[:, ~obj.var["allZero"]]
     aboveMinDisp = objNZ.var["dispGeneEst"] >= 100 * minDisp
     if modelMatrix is None:
         modelMatrix = objNZ.design
     # estimate the variance of the distribution of the
     # log dispersion estimates around the fitted value
-    dispResiduals = np.log(objNZ.var["dispGeneEst"]) - np.log(objNZ.var["dispFit"])
+    # dispResiduals = np.log(objNZ.var["dispGeneEst"]) - np.log(objNZ.var["dispFit"])
     if np.nansum(aboveMinDisp) == 0:
         raise ValueError("no data found which is greater than minDisp")
 
     varLogDispEsts = obj.dispersionFunction.varLogDispEsts
 
     m, p = modelMatrix.shape
 
@@ -938,10 +942,13 @@
         if np.sum(np.log(coefs / oldcoefs.values) ** 2) < 1e-6 and fit.converged:
             break
         iter_ = iter_ + 1
         if iter_ > 10:
             raise RuntimeError("dispersion fit did not converge")
 
     coefs.index = ["asymptDisp", "extraPois"]
-    ans = lambda q: coefs.iloc[0] + coefs.iloc[1] / q
+
+    def ans(q):
+        return coefs.iloc[0] + coefs.iloc[1] / q
+
     ans.coefficients = coefs
     return ans
```

### Comparing `inmoose-0.4.1/inmoose/deseq2/estimateSizeFactors.py` & `inmoose-0.5.0/inmoose/deseq2/estimateSizeFactors.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,14 +17,15 @@
 # -----------------------------------------------------------------------------
 
 # This file is based on the file 'R/core.R' of the Bioconductor DESeq2 package
 # (version 3.16).
 
 
 import logging
+
 import numpy as np
 
 
 def estimateSizeFactors_dds(
     obj,
     type_="ratio",
     locfunc=np.median,
```

### Comparing `inmoose-0.4.1/inmoose/deseq2/fitNbinomGLMs.py` & `inmoose-0.5.0/inmoose/deseq2/fitNbinomGLMs.py`

 * *Files 0% similar despite different names*

```diff
@@ -16,20 +16,21 @@
 # along with this program.  If not, see <https://www.gnu.org/licenses/>.
 # -----------------------------------------------------------------------------
 
 # This file is based on the file 'R/fitNbinomGLMs.R' of the Bioconductor DESeq2
 # package (version 3.16).
 
 
-from collections import OrderedDict
 import logging
+from collections import OrderedDict
+
 import numpy as np
 import pandas as pd
 import patsy
-from scipy.optimize import minimize, Bounds
+from scipy.optimize import Bounds, minimize
 
 from ..utils import dnbinom_mu, dnorm
 from .deseq2_cpp import fitBetaWrapper
 from .misc import renameModelMatrixColumns
 from .prior import estimateBetaPriorVar
 from .weights import getAndCheckWeights
```

### Comparing `inmoose-0.4.1/inmoose/deseq2/lrt.py` & `inmoose-0.5.0/inmoose/deseq2/lrt.py`

 * *Files identical despite different names*

### Comparing `inmoose-0.4.1/inmoose/deseq2/misc.py` & `inmoose-0.5.0/inmoose/deseq2/misc.py`

 * *Files identical despite different names*

### Comparing `inmoose-0.4.1/inmoose/deseq2/outliers.py` & `inmoose-0.5.0/inmoose/deseq2/outliers.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,21 +17,23 @@
 # -----------------------------------------------------------------------------
 
 # This file is based on the file 'R/core.R' of the Bioconductor DESeq2 package
 # (version 3.16).
 
 
 import logging
+
 import numpy as np
 import scipy.stats
 from scipy.stats import trim_mean
 
 from .dispersions import estimateDispersionsGeneEst, estimateDispersionsMAP
+from .lrt import nbinomLRT
 from .misc import nOrMoreInCell
-from .wald import nbinomWaldTest
+from .wald import nbinomWaldTest, recordMaxCooks
 
 
 def refitWithoutOutliers(
     obj,
     test,
     betaPrior,
     full,
```

### Comparing `inmoose-0.4.1/inmoose/deseq2/parallel.py` & `inmoose-0.5.0/inmoose/deseq2/parallel.py`

 * *Files 5% similar despite different names*

```diff
@@ -21,17 +21,17 @@
 
 
 import numpy as np
 import pandas as pd
 
 from .fitNbinomGLMs import fitNbinomGLMs
 from .misc import (
-    renameModelMatrixColumns,
     buildDataFrameWithNACols,
     buildMatrixWithNACols,
+    renameModelMatrixColumns,
 )
 
 
 def estimateMLEForBetaPriorVar(
     obj, maxit=100, useOptim=True, useQR=True, modelMatrixType=None
 ):
     """
@@ -60,15 +60,14 @@
         useOptim=useOptim,
         useQR=useQR,
         renameCols=(modelMatrixType == "standard"),
     )
     modelMatrix = fit["modelMatrix"]
     modelMatrixNames = modelMatrix.design_info.column_names
     H = fit["hat_diagonals"]
-    betaMatrix = fit["betaMatrix"]
 
     convertNames = renameModelMatrixColumns(obj.obs, objNZ.design)
     modelMatrixNames = [
         convertNames[x] if x in convertNames else x for x in modelMatrixNames
     ]
 
     mleBetaMatrix = fit["betaMatrix"]
```

### Comparing `inmoose-0.4.1/inmoose/deseq2/plot.py` & `inmoose-0.5.0/inmoose/deseq2/plot.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,17 +16,17 @@
 # along with this program.  If not, see <https://www.gnu.org/licenses/>.
 # -----------------------------------------------------------------------------
 
 # This file is based on the file 'R/plot.R' of the Bioconductor DESeq2 package
 # (version 3.16).
 
 
+import matplotlib.pyplot as plt
 import numpy as np
 import pandas as pd
-import matplotlib.pyplot as plt
 
 
 def plotDispEsts_dds(
     self,
     ymin=None,
     CV=False,
     genecol="black",
@@ -81,15 +81,17 @@
     sel = px > 0
     px = px[sel]
 
     # transformation of dispersion into CV or not
     if CV:
         f = np.sqrt
     else:
-        f = lambda x: x
+
+        def f(x):
+            return x
 
     py = f(self.var["dispGeneEst"][sel])
     if ymin is None:
         ymin = 10 ** np.floor(np.log10(np.nanmin(py[py > 0])) - 0.1)
 
     plt.scatter(px, np.maximum(py, ymin), s=cex, c=genecol, label="gene-est")
     if "x" in log:
```

### Comparing `inmoose-0.4.1/inmoose/deseq2/prior.py` & `inmoose-0.5.0/inmoose/deseq2/prior.py`

 * *Files identical despite different names*

### Comparing `inmoose-0.4.1/inmoose/deseq2/replicates.py` & `inmoose-0.5.0/inmoose/deseq2/replicates.py`

 * *Files identical despite different names*

### Comparing `inmoose-0.4.1/inmoose/deseq2/results.py` & `inmoose-0.5.0/inmoose/deseq2/results.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,19 +20,19 @@
 # package (version 3.16).
 
 
 import numpy as np
 import pandas as pd
 import patsy
 import scipy.stats
-from statsmodels.stats.multitest import multipletests
 from statsmodels.nonparametric.smoothers_lowess import lowess
+from statsmodels.stats.multitest import multipletests
 
-from ..utils import pnorm, pt
 from .. import __version__
+from ..utils import pnorm, pt
 from .deseq2_cpp import fitBeta
 from .misc import buildDataFrameWithNACols, getFactorName
 
 
 def p_adjust(*args, **kwargs):
     """
     Test results and p-value correction for multiple tests
@@ -408,15 +408,18 @@
         raise ValueError("listValues should contain a positive and a negative number")
     if obj.var.type.filter(["results"]).empty:
         raise ValueError("could not find results in obj. first run DESeq()")
     if test is None:
         test = obj.test
     elif test == "Wald" and obj.test == "LRT":
         # initially test was LRT, now need to add Wald statistics and p-values
-        obj = makeWaldTest(obj)
+        raise NotImplementedError(
+            "adding Wald statistics to LRT object is not implemented"
+        )
+        # obj = makeWaldTest(obj)
     elif test == "LRT" and obj.test == "Wald":
         raise ValueError(
             "the LRT requires the user to run nbinomLRT or DESeq(obj, test='LRT')"
         )
     if lfcThreshold == 0 and altHypothesis == "lessAbs":
         raise ValueError(
             "when testing altHypothesis='lessAbs', set the argument lfcThreshold to a positive value"
@@ -431,15 +434,15 @@
             raise ValueError(
                 "addMLE=True should be used by providing string vector of length 3 to 'contrast' instead of using 'name'"
             )
 
     if saveCols is not None:
         try:
             obj.var[saveCols]
-        except:
+        except KeyError:
             raise ValueError(f"invalid value for saveCols: {saveCols}")
 
     hasIntercept = patsy.INTERCEPT in obj.design.design_info.terms
     isExpanded = obj.modelMatrixType == "expanded"
     noInteraction = all(len(t.factors) < 2 for t in obj.design.design_info.terms)
     # if no intercept was used or an expanded model matrix was used,
     # and neither 'contrast' nor 'name' were specified,
@@ -469,17 +472,14 @@
         name = lastCoefName(obj)
     else:
         if not isinstance(name, str):
             raise ValueError("'name' should be a string")
 
     # done with input argument testing
 
-    WaldResults = f"WaldPvalue_{name}" in obj.obs
-    LRTResults = "LRTPValue" in obj.obs
-
     # this will be used in cleanContrast, and in the lfcThreshold chunks below
     useT = "tDegreesFreedom" in obj.var
 
     # if performing a contrast call the function cleanContrast()
     if contrast is not None:
         resNames = obj.resultsNames()
         # do some arg checking/cleaning
@@ -547,17 +547,21 @@
         # easier to read
         LFC = res.log2FoldChange
         SE = res.lfcSE
         T = lfcThreshold
 
         if useT:
             df = obj.var["tDegreesFreedom"]
-            pfunc = lambda q: pt(q, df=df, lower_tail=False)
+
+            def pfunc(q):
+                return pt(q, df=df, lower_tail=False)
         else:
-            pfunc = lambda q: pnorm(q, lower_tail=False)
+
+            def pfunc(q):
+                return pnorm(q, lower_tail=False)
 
         if altHypothesis == "greaterAbs":
             newStat = np.sign(LFC) * np.maximum((np.abs(LFC) - T) / SE, 0)
             newPvalue = np.minimum(1, 2 * pfunc((np.abs(LFC) - T) / SE))
         elif altHypothesis == "lessAbs":
             newStatAbove = np.maximum((T - LFC) / SE, 0)
             pvalueAbove = pfunc((T - LFC) / SE)
@@ -579,19 +583,19 @@
     m, p = obj.dispModelMatrix.shape
 
     if cooksCutoff is None or (isinstance(cooksCutoff, bool) and cooksCutoff):
         cooksCutoff = scipy.stats.f.ppf(0.99, p, m - p)
 
     # apply cutoff based on maximum Cook's distance
     # NB: cooksCutoff is not necessarily a Boolean
-    performCooksCutoff = not (cooksCutoff == False)
+    performCooksCutoff = not (cooksCutoff == False)  # noqa: E712
     if performCooksCutoff:
         cooksOutlier = obj.var["maxCooks"] > cooksCutoff
 
-        ### BEGIN heuristic to avoid filtering genes with low count outliers
+        # BEGIN heuristic to avoid filtering genes with low count outliers
         # as according to Cook's cutoff. only for two group designs.
         # do not filter if three or more counts are larger
         if np.any(cooksOutlier[~np.isnan(cooksOutlier)]):
             designVars = obj.design.design_info.factor_infos
             if len(designVars) == 1:
                 var = [v for v in designVars.values()][0]
                 if var.type == "categorical" and len(var.categories) == 2:
@@ -604,15 +608,15 @@
                     # if three or more counts larger than the outlier
                     # do not filter out the p-value for those genes
                     dontFilter = np.sum(outliers > outCount, axis=0) >= 3
                     # reset the outlier status for these genes
                     # NB: pandas 2.2 raises a warning here, but it should not. See
                     #     https://github.com/pandas-dev/pandas/issues/57338
                     cooksOutlier[cooksOutlier] &= ~dontFilter
-        ### END heuristic
+        # END heuristic
 
         res.loc[cooksOutlier, "pvalue"] = np.nan
 
     # if original baseMean was positive, but now zero due to replaced counts,
     # fill in results
     if "replace" in obj.var and np.nansum(obj.var["replace"]) > 0:
         nowZero = obj.var["replace"] & (obj.var["baseMean"] == 0)
```

### Comparing `inmoose-0.4.1/inmoose/deseq2/vst.py` & `inmoose-0.5.0/inmoose/deseq2/vst.py`

 * *Files 3% similar despite different names*

```diff
@@ -16,22 +16,23 @@
 # along with this program.  If not, see <https://www.gnu.org/licenses/>.
 # -----------------------------------------------------------------------------
 
 # This file is based on the file 'R/vst.R' Bioconductor DESeq2 package (version
 # 3.16).
 
 
-from anndata import AnnData
 import numpy as np
+from anndata import AnnData
+from scipy.interpolate import CubicSpline
 
 from . import (
     DESeqDataSet,
     DESeqTransform,
-    estimateDispersionsGeneEst,
     estimateDispersionsFit,
+    estimateDispersionsGeneEst,
 )
 
 
 def varianceStabilizingTransformation(obj, blind=True, fitType="parametric"):
     """
     Apply a variance stabilizing transformation (VST) to the count data
 
@@ -164,28 +165,31 @@
         raise ValueError(
             "call estimateDispersions before calling getVarianceStabilizedData"
         )
 
     ncounts = obj.counts(normalized=True)
     if obj.dispersionFunction.fitType == "parametric":
         coefs = obj.dispersionFunction.coefficients
-        vst_fn = lambda q: np.log(
-            (
-                1
-                + coefs["extraPois"]
-                + 2 * coefs["asymptDisp"] * q
-                + 2
-                * np.sqrt(
-                    coefs["asymptDisp"]
-                    * q
-                    * (1 + coefs["extraPois"] + coefs["asymptDisp"] * q)
+
+        def vst_fn(q):
+            return np.log(
+                (
+                    1
+                    + coefs["extraPois"]
+                    + 2 * coefs["asymptDisp"] * q
+                    + 2
+                    * np.sqrt(
+                        coefs["asymptDisp"]
+                        * q
+                        * (1 + coefs["extraPois"] + coefs["asymptDisp"] * q)
+                    )
                 )
-            )
-            / (4 * coefs["asymptDisp"])
-        ) / np.log(2)
+                / (4 * coefs["asymptDisp"])
+            ) / np.log(2)
+
         return vst_fn(ncounts)
 
     elif obj.dispersionFunction.fitType == "local":
         # non-parametric fit -> numerical integration
         if obj.sizeFactors is None:
             if obj.normalizationFactors is None:
                 raise ValueError(
@@ -196,37 +200,40 @@
             sf = obj.sizeFactors
         xg = np.sinh(np.linspace(np.arcsinh(0), np.arcsinh(ncounts.max()), num=1000))[
             1:
         ]
         xim = (1 / sf).mean()
         baseVarsAtGrid = obj.dispersionFunction(xg) * xg**2 + xim * xg
         integrand = 1 / np.sqrt(baseVarsAtGrid)
-        splf = splinefun(
+        splf = CubicSpline(
             np.arcsinh((xg[1:] + xg[:-1]) / 2),
             ((xg[1:] - xg[:-1]) * (integrand[1:] + integrand[:-1]) / 2).cumsum(),
         )
-        h1 = quantile(ncounts.mean(axis=1), 0.95)
-        h2 = quantile(ncounts.mean(axis=1), 0.999)
+        h1 = np.quantile(ncounts.mean(axis=1), 0.95)
+        h2 = np.quantile(ncounts.mean(axis=1), 0.999)
         eta = (np.log2(h2) - np.log2(h1)) / (
             splf(np.arcsinh(h2)) - splf(np.arcsinh(h1))
         )
         xi = np.log2(h1) - eta * splf(np.arcsinh(h1))
         tc = [
             eta * splf(np.arcsinh(ncounts[:, clm])) + xi
             for clm in obj.counts().var_names
         ]
         tc.rownames = obj.counts().rownames
         return tc
     elif obj.dispersionFunction.fitType == "mean":
         alpha = obj.dispersionFunction.mean
         # the following stabilizes NB counts with fixed dispersion alpha
         # and converges to log2(q) as q => infinity
-        vst_fn = lambda q: (
-            2 * np.arcsinh(np.sqrt(alpha * q)) - np.log(alpha) - np.log(4)
-        ) / np.log(2)
+
+        def vst_fn(q):
+            return (
+                2 * np.arcsinh(np.sqrt(alpha * q)) - np.log(alpha) - np.log(4)
+            ) / np.log(2)
+
         return vst_fn(ncounts)
     else:
         raise ValueError("fitType is not parametric, local or mean")
 
 
 def vst(obj, blind=True, nsub=1000, fitType="parametric"):
     """
```

### Comparing `inmoose-0.4.1/inmoose/deseq2/wald.py` & `inmoose-0.5.0/inmoose/deseq2/wald.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,21 +17,22 @@
 # -----------------------------------------------------------------------------
 
 # This file is based on the file 'R/core.R' of the Bioconductor DESeq2 package
 # (version 3.16).
 
 
 import logging
+
 import numpy as np
 import pandas as pd
 from scipy.stats import trim_mean
 
 from ..utils import Factor, pnorm, pt
-from .fitNbinomGLMs import fitNbinomGLMs, fitGLMsWithPrior
-from .misc import buildMatrixWithNACols, nOrMoreInCell, buildDataFrameWithNACols
+from .fitNbinomGLMs import fitGLMsWithPrior, fitNbinomGLMs
+from .misc import buildDataFrameWithNACols, buildMatrixWithNACols, nOrMoreInCell
 from .weights import getAndCheckWeights
 
 
 def nbinomWaldTest(
     obj,
     betaPrior=False,
     betaPriorVar=None,
@@ -190,15 +191,14 @@
     # only continue on the columns with non-zero means
     objNZ = obj[:, ~obj.var["allZero"]]
 
     # model matrix not provided...
     if modelMatrix is None:
         modelAsFormula = True
         termsOrder = np.array([len(t.factors) for t in obj.design.design_info.terms])
-        interactionPresent = (termsOrder > 1).any()
 
         # run some tests common to DESeq, nbinomWaldTest, nbinomLRT
         obj.designAndArgChecker(betaPrior)
 
         # what kind of model matrix to use
         if not isinstance(betaPrior, bool):
             raise ValueError("betaPrior must be a boolean")
@@ -299,17 +299,20 @@
     # store Cook's distance for each sample
     obj.layers["cooks"] = buildMatrixWithNACols(cooks, obj.var["allZero"])
 
     # add betas, standard errors and Wald p-values to the object
     modelMatrixNames = modelMatrix.design_info.column_names
     betaMatrix = fit["betaMatrix"]
     assert isinstance(betaMatrix, pd.DataFrame)
-    assert betaMatrix.shape == (
-        objNZ.n_vars,
-        len(modelMatrixNames),
+    assert (
+        betaMatrix.shape
+        == (
+            objNZ.n_vars,
+            len(modelMatrixNames),
+        )
     ), f"betaMatrix shape {betaMatrix.shape} is wrong, should be {(objNZ.n_vars, len(modelMatrixNames))}"
     betaMatrix.index = objNZ.var_names
     assert np.array_equal(betaMatrix.columns, modelMatrixNames)
     betaSE = fit["betaSE"]
     assert isinstance(betaSE, pd.DataFrame)
     assert (
         betaSE.shape == betaMatrix.shape
```

### Comparing `inmoose-0.4.1/inmoose/deseq2/weights.py` & `inmoose-0.5.0/inmoose/deseq2/weights.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,14 +17,15 @@
 # -----------------------------------------------------------------------------
 
 # This file is based on the file 'R/core.R' of the Bioconductor DESeq2 package
 # (version 3.16).
 
 
 import logging
+
 import numpy as np
 
 
 def getAndCheckWeights(obj, modelMatrix, weightThreshold=1e-2):
     """
     Check and retrive weights
```

### Comparing `inmoose-0.4.1/inmoose/edgepy/DGEExact.py` & `inmoose-0.5.0/inmoose/edgepy/DGEExact.py`

 * *Files identical despite different names*

### Comparing `inmoose-0.4.1/inmoose/edgepy/DGEGLM.py` & `inmoose-0.5.0/inmoose/edgepy/DGEGLM.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,16 +12,14 @@
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 
 # You should have received a copy of the GNU General Public License
 # along with this program.  If not, see <https://www.gnu.org/licenses/>.
 # -----------------------------------------------------------------------------
 
-import patsy
-
 
 class DGEGLM(object):
     """
     A simple class to store results of a GLM fit to each gene in  DGE dataset.
 
     Attributes
     ----------
```

### Comparing `inmoose-0.4.1/inmoose/edgepy/DGELRT.py` & `inmoose-0.5.0/inmoose/edgepy/DGELRT.py`

 * *Files identical despite different names*

### Comparing `inmoose-0.4.1/inmoose/edgepy/DGEList.py` & `inmoose-0.5.0/inmoose/edgepy/DGEList.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,19 +15,20 @@
 # You should have received a copy of the GNU General Public License
 # along with this program.  If not, see <https://www.gnu.org/licenses/>.
 # -----------------------------------------------------------------------------
 
 # This file is based on the file 'R/DGEList.R' of the Bioconductor edgeR package (version 3.38.4).
 
 import logging
+
 import numpy as np
 import pandas as pd
 
-from .edgepy_cpp import is_integer_array
 from ..utils import Factor
+from .edgepy_cpp import is_integer_array
 from .utils import _isAllZero
 
 
 class DGEList(object):
     """
     A class for storing read counts and associated information from digital
     gene expression or sequencing technologies.
@@ -162,15 +163,15 @@
                     "Number of rows in 'samples' must be equal to the number of columns in 'counts'"
                 )
 
         # Get group from samples if appropriate
         if (
             group is None
             and samples is not None
-            and (samples[group_col].values != None).all()
+            and (samples[group_col].values != None).all()  # noqa: E711
         ):
             group = samples[group_col].values
             samples = samples.drop(columns=[group_col])
 
         # Check group
         if group is None:
             group = np.ones(nlibs)
@@ -221,15 +222,15 @@
         By default, offset is constructed from the lib_size and norm_factors
         """
         if self.offset is not None:
             return self.offset
 
         lib_size = self.samples["lib_size"]
         norm_factors = self.samples["norm_factors"]
-        if (norm_factors.values != None).all():
+        if (norm_factors.values != None).all():  # noqa: E711
             lib_size = lib_size * norm_factors
         return np.log(lib_size)
 
     def getDispersion(self):
         """
         Get most complex dispersion values from DGEList object
         """
```

### Comparing `inmoose-0.4.1/inmoose/edgepy/addPriorCount.py` & `inmoose-0.5.0/inmoose/edgepy/addPriorCount.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,16 +16,17 @@
 # along with this program.  If not, see <https://www.gnu.org/licenses/>.
 # -----------------------------------------------------------------------------
 
 # This file is based on the file 'R/addPriorCount.R' of the Bioconductor edgeR package (version 3.38.4).
 
 
 import numpy as np
-from .makeCompressedMatrix import _compressOffsets, _compressPrior, makeCompressedMatrix
+
 from .edgepy_cpp import cxx_add_prior_count
+from .makeCompressedMatrix import _compressOffsets, _compressPrior, makeCompressedMatrix
 
 
 def addPriorCount(y, lib_size=None, offset=None, prior_count=1):
     """
     Add a library size-adjusted prior count to each observation.
 
     This function adds a positive prior count to each observation, often useful
```

### Comparing `inmoose-0.4.1/inmoose/edgepy/adjustedProfileLik.py` & `inmoose-0.5.0/inmoose/edgepy/adjustedProfileLik.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,21 +16,22 @@
 # along with this program.  If not, see <https://www.gnu.org/licenses/>.
 # -----------------------------------------------------------------------------
 
 # This file is based on the file 'R/adjustedProfileLik.R' of the Bioconductor edgeR package (version 3.38.4).
 
 
 import numpy as np
+
+from .edgepy_cpp import cxx_compute_apl
+from .glmFit import glmFit
 from .makeCompressedMatrix import (
-    _compressOffsets,
     _compressDispersions,
+    _compressOffsets,
     _compressWeights,
 )
-from .glmFit import glmFit
-from .edgepy_cpp import cxx_compute_apl
 
 
 def adjustedProfileLik(
     dispersion, y, design, offset, weights=None, adjust=True, start=None, get_coef=False
 ):
     """
     Compute adjusted profile log-likelihoods for the dispersion parameters of
```

### Comparing `inmoose-0.4.1/inmoose/edgepy/aveLogCPM.py` & `inmoose-0.5.0/inmoose/edgepy/aveLogCPM.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,25 +16,26 @@
 # along with this program.  If not, see <https://www.gnu.org/licenses/>.
 # -----------------------------------------------------------------------------
 
 # This file is based on the file 'R/aveLogCPM.R' of the Bioconductor edgeR package (version 3.38.4).
 
 
 from inspect import signature
+
 import numpy as np
 
-from .utils import _isAllZero
+from .edgepy_cpp import cxx_ave_log_cpm
 from .makeCompressedMatrix import (
     _compressDispersions,
-    _compressWeights,
     _compressOffsets,
     _compressPrior,
+    _compressWeights,
 )
 from .mglmOneGroup import mglmOneGroup
-from .edgepy_cpp import cxx_ave_log_cpm
+from .utils import _isAllZero
 
 
 def aveLogCPM_DGEList(self, normalized_lib_sizes=True, prior_count=2, dispersion=None):
     """
     Compute average log2 counts per million for each row of counts.
 
     See also
@@ -57,21 +58,21 @@
     Returns
     -------
     ndarray
         numeric vector giving :code:`log2(AveCPM)` for each row of :code:`y`
     """
     # Library sizes should be stored in y but are sometimes missing
     lib_size = self.samples["lib_size"]
-    if (lib_size.values == None).any():
+    if (lib_size.values == None).any():  # noqa: E711
         lib_size = self.counts.sum(axis=0)
 
     # Normalization factors should be stored in y but are sometimes missing
     if normalized_lib_sizes:
         nf = self.samples["norm_factors"]
-        if (nf.values != None).all():
+        if (nf.values != None).all():  # noqa: E711
             lib_size = lib_size * nf
 
     # Dispersion supplied as argument takes precedence over value in object
     # Should trended_dispersion or tagwise_dispersion be used instead of common_dispersion if available?
     if dispersion is None:
         dispersion = self.common_dispersion
```

### Comparing `inmoose-0.4.1/inmoose/edgepy/binomTest.py` & `inmoose-0.5.0/inmoose/edgepy/binomTest.py`

 * *Files identical despite different names*

### Comparing `inmoose-0.4.1/inmoose/edgepy/dispCoxReid.py` & `inmoose-0.5.0/inmoose/edgepy/dispCoxReid.py`

 * *Files identical despite different names*

### Comparing `inmoose-0.4.1/inmoose/edgepy/dispCoxReidInterpolateTagwise.py` & `inmoose-0.5.0/inmoose/edgepy/dispCoxReidInterpolateTagwise.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,17 +15,18 @@
 # You should have received a copy of the GNU General Public License
 # along with this program.  If not, see <https://www.gnu.org/licenses/>.
 # -----------------------------------------------------------------------------
 
 # This file is based on the file 'R/dispCoxReidInterpolateTagwise.R' of the Bioconductor edgeR package (version 3.38.4).
 
 
-import numpy as np
 from math import floor
 
+import numpy as np
+
 from .adjustedProfileLik import adjustedProfileLik
 from .aveLogCPM import aveLogCPM
 from .makeCompressedMatrix import _compressOffsets, _compressWeights
 from .maximizeInterpolant import maximizeInterpolant
 from .movingAverageByCol import movingAverageByCol
```

### Comparing `inmoose-0.4.1/inmoose/edgepy/edgepy_cpp/__init__.pxd` & `inmoose-0.5.0/inmoose/edgepy/edgepy_cpp/__init__.pxd`

 * *Files identical despite different names*

### Comparing `inmoose-0.4.1/inmoose/edgepy/edgepy_cpp/add_prior.cpp` & `inmoose-0.5.0/inmoose/edgepy/edgepy_cpp/add_prior.cpp`

 * *Files identical despite different names*

### Comparing `inmoose-0.4.1/inmoose/edgepy/edgepy_cpp/add_prior.h` & `inmoose-0.5.0/inmoose/edgepy/edgepy_cpp/add_prior.h`

 * *Files identical despite different names*

### Comparing `inmoose-0.4.1/inmoose/edgepy/edgepy_cpp/add_prior_count.cpp` & `inmoose-0.5.0/inmoose/edgepy/edgepy_cpp/add_prior_count.cpp`

 * *Files identical despite different names*

### Comparing `inmoose-0.4.1/inmoose/edgepy/edgepy_cpp/add_prior_count.h` & `inmoose-0.5.0/inmoose/edgepy/edgepy_cpp/add_prior_count.h`

 * *Files identical despite different names*

### Comparing `inmoose-0.4.1/inmoose/edgepy/edgepy_cpp/adj_coxreid.cpp` & `inmoose-0.5.0/inmoose/edgepy/edgepy_cpp/adj_coxreid.cpp`

 * *Files identical despite different names*

### Comparing `inmoose-0.4.1/inmoose/edgepy/edgepy_cpp/ave_log_cpm.cpp` & `inmoose-0.5.0/inmoose/edgepy/edgepy_cpp/ave_log_cpm.cpp`

 * *Files identical despite different names*

### Comparing `inmoose-0.4.1/inmoose/edgepy/edgepy_cpp/compute_apl.cpp` & `inmoose-0.5.0/inmoose/edgepy/edgepy_cpp/compute_apl.cpp`

 * *Files identical despite different names*

### Comparing `inmoose-0.4.1/inmoose/edgepy/edgepy_cpp/compute_nbdev.cpp` & `inmoose-0.5.0/inmoose/edgepy/edgepy_cpp/compute_nbdev.cpp`

 * *Files identical despite different names*

### Comparing `inmoose-0.4.1/inmoose/edgepy/edgepy_cpp/edgepy_cpp.pyx` & `inmoose-0.5.0/inmoose/edgepy/edgepy_cpp/edgepy_cpp.pyx`

 * *Files identical despite different names*

### Comparing `inmoose-0.4.1/inmoose/edgepy/edgepy_cpp/fit_levenberg.cpp` & `inmoose-0.5.0/inmoose/edgepy/edgepy_cpp/fit_levenberg.cpp`

 * *Files identical despite different names*

### Comparing `inmoose-0.4.1/inmoose/edgepy/edgepy_cpp/fit_levenberg.h` & `inmoose-0.5.0/inmoose/edgepy/edgepy_cpp/fit_levenberg.h`

 * *Files identical despite different names*

### Comparing `inmoose-0.4.1/inmoose/edgepy/edgepy_cpp/fit_one_group.cpp` & `inmoose-0.5.0/inmoose/edgepy/edgepy_cpp/fit_one_group.cpp`

 * *Files identical despite different names*

### Comparing `inmoose-0.4.1/inmoose/edgepy/edgepy_cpp/get_one_way_fitted.cpp` & `inmoose-0.5.0/inmoose/edgepy/edgepy_cpp/get_one_way_fitted.cpp`

 * *Files identical despite different names*

### Comparing `inmoose-0.4.1/inmoose/edgepy/edgepy_cpp/glm.h` & `inmoose-0.5.0/inmoose/edgepy/edgepy_cpp/glm.h`

 * *Files identical despite different names*

### Comparing `inmoose-0.4.1/inmoose/edgepy/edgepy_cpp/glm_levenberg.cpp` & `inmoose-0.5.0/inmoose/edgepy/edgepy_cpp/glm_levenberg.cpp`

 * *Files identical despite different names*

### Comparing `inmoose-0.4.1/inmoose/edgepy/edgepy_cpp/glm_one_group.cpp` & `inmoose-0.5.0/inmoose/edgepy/edgepy_cpp/glm_one_group.cpp`

 * *Files identical despite different names*

### Comparing `inmoose-0.4.1/inmoose/edgepy/edgepy_cpp/initialize_levenberg.cpp` & `inmoose-0.5.0/inmoose/edgepy/edgepy_cpp/initialize_levenberg.cpp`

 * *Files identical despite different names*

### Comparing `inmoose-0.4.1/inmoose/edgepy/edgepy_cpp/initialize_levenberg.h` & `inmoose-0.5.0/inmoose/edgepy/edgepy_cpp/initialize_levenberg.h`

 * *Files identical despite different names*

### Comparing `inmoose-0.4.1/inmoose/edgepy/edgepy_cpp/interpolator.cpp` & `inmoose-0.5.0/inmoose/edgepy/edgepy_cpp/interpolator.cpp`

 * *Files identical despite different names*

### Comparing `inmoose-0.4.1/inmoose/edgepy/edgepy_cpp/interpolator.h` & `inmoose-0.5.0/inmoose/edgepy/edgepy_cpp/interpolator.h`

 * *Files identical despite different names*

### Comparing `inmoose-0.4.1/inmoose/edgepy/edgepy_cpp/maximize_interpolant.cpp` & `inmoose-0.5.0/inmoose/edgepy/edgepy_cpp/maximize_interpolant.cpp`

 * *Files identical despite different names*

### Comparing `inmoose-0.4.1/inmoose/edgepy/edgepy_cpp/objects.cpp` & `inmoose-0.5.0/inmoose/edgepy/edgepy_cpp/objects.cpp`

 * *Files identical despite different names*

### Comparing `inmoose-0.4.1/inmoose/edgepy/edgepy_cpp/objects.h` & `inmoose-0.5.0/inmoose/edgepy/edgepy_cpp/objects.h`

 * *Files identical despite different names*

### Comparing `inmoose-0.4.1/inmoose/edgepy/edgepy_cpp/utils.h` & `inmoose-0.5.0/inmoose/edgepy/edgepy_cpp/utils.h`

 * *Files identical despite different names*

### Comparing `inmoose-0.4.1/inmoose/edgepy/estimateGLMCommonDisp.py` & `inmoose-0.5.0/inmoose/edgepy/estimateGLMCommonDisp.py`

 * *Files 3% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 # You should have received a copy of the GNU General Public License
 # along with this program.  If not, see <https://www.gnu.org/licenses/>.
 # -----------------------------------------------------------------------------
 
 # This file is based on the file 'R/estimateGLMCommonDisp.R' of the Bioconductor edgeR package (version 3.38.4).
 
 import logging
+
 import numpy as np
 
 from .aveLogCPM import aveLogCPM
 from .dispCoxReid import dispCoxReid
 from .validDGEList import validDGEList
 
 
@@ -157,20 +158,26 @@
             design=design,
             offset=offset,
             subset=subset,
             AveLogCPM=AveLogCPM,
             weights=weights,
         )
     elif method == "Pearson":
-        disp = dispPearson(
-            y, design=design, offset=offset, subset=subset, AveLogCPM=AveLogCPM
+        raise NotImplementedError(
+            "method 'Pearson' for dispersion estimation is not implemented"
         )
+        # disp = dispPearson(
+        #    y, design=design, offset=offset, subset=subset, AveLogCPM=AveLogCPM
+        # )
     elif method == "deviance":
-        disp = dispDeviance(
-            y, design=design, offset=offset, subset=subset, AveLogCPM=AveLogCPM
+        raise NotImplementedError(
+            "method 'deviance' for dispersion estimation is not implemented"
         )
+        # disp = dispDeviance(
+        #    y, design=design, offset=offset, subset=subset, AveLogCPM=AveLogCPM
+        # )
     else:
         raise ValueError(f"invalid method for dispersion evaluation: {method}")
 
     logging.debug(f"Disp = {round(disp, 5)}, BCV = {round(np.sqrt(disp), 4)}")
 
     return disp
```

### Comparing `inmoose-0.4.1/inmoose/edgepy/estimateGLMTagwiseDisp.py` & `inmoose-0.5.0/inmoose/edgepy/estimateGLMTagwiseDisp.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,14 +16,15 @@
 # along with this program.  If not, see <https://www.gnu.org/licenses/>.
 # -----------------------------------------------------------------------------
 
 # This file is based on the file 'R/estimateGLMTagwiseDisp.R' of the Bioconductor edgeR package (version 3.38.4).
 
 
 import logging
+
 import numpy as np
 
 from .aveLogCPM import aveLogCPM
 from .dispCoxReidInterpolateTagwise import dispCoxReidInterpolateTagwise
 
 
 def estimateGLMTagwiseDisp_DGEList(
```

### Comparing `inmoose-0.4.1/inmoose/edgepy/exactTest.py` & `inmoose-0.5.0/inmoose/edgepy/exactTest.py`

 * *Files identical despite different names*

### Comparing `inmoose-0.4.1/inmoose/edgepy/exactTestBetaApprox.py` & `inmoose-0.5.0/inmoose/edgepy/exactTestBetaApprox.py`

 * *Files identical despite different names*

### Comparing `inmoose-0.4.1/inmoose/edgepy/exactTestByDeviance.py` & `inmoose-0.5.0/inmoose/edgepy/exactTestByDeviance.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -18,16 +18,16 @@
 
 # This file is based on the file 'R/exactTestByDeviance.R' of the Bioconductor edgeR package (version 3.38.4).
 
 import numpy as np
 from scipy.stats import nbinom
 
 from .binomTest import binomTest
-from .exactTestDoubleTail import exactTestDoubleTail
 from .edgepy_cpp import compute_unit_nb_deviance
+from .exactTestDoubleTail import exactTestDoubleTail
 
 
 def exactTestByDeviance(y1, y2, dispersion=0.0):
     """
     Compute genewise *p*-values for differences in the means between two groups of negative-binomially distributed counts.
 
     This function uses the deviance goodness of fit statistics to define the
```

### Comparing `inmoose-0.4.1/inmoose/edgepy/exactTestBySmallP.py` & `inmoose-0.5.0/inmoose/edgepy/exactTestBySmallP.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 # You should have received a copy of the GNU General Public License
 # along with this program.  If not, see <https://www.gnu.org/licenses/>.
 # -----------------------------------------------------------------------------
 
 # This file is based on the file 'R/exactTestBySmallP.R' of the Bioconductor edgeR package (version 3.38.4).
 
 import numpy as np
+
 from ..utils import dnbinom_mu as dnbinom
 from .binomTest import binomTest
 from .exactTestDoubleTail import exactTestDoubleTail
 
 
 def exactTestBySmallP(y1, y2, dispersion=0):
     """
```

### Comparing `inmoose-0.4.1/inmoose/edgepy/exactTestDoubleTail.py` & `inmoose-0.5.0/inmoose/edgepy/exactTestDoubleTail.py`

 * *Files 8% similar despite different names*

```diff
@@ -15,16 +15,18 @@
 # You should have received a copy of the GNU General Public License
 # along with this program.  If not, see <https://www.gnu.org/licenses/>.
 # -----------------------------------------------------------------------------
 
 # This file is based on the file 'R/exactTestDoubleTail.R' of the Bioconductor edgeR package (version 3.38.4).
 
 import numpy as np
+
 from ..utils import dnbinom_mu as dnbinom
 from .binomTest import binomTest
+from .exactTestBetaApprox import exactTestBetaApprox
 
 
 def exactTestDoubleTail(y1, y2, dispersion=0, big_count=900):
     """
     Compute genewise *p*-values for differences in the means between two groups of negative-binomially distributed counts.
 
     This function computes two-sided *p*-values by doubling the smaller tail
```

### Comparing `inmoose-0.4.1/inmoose/edgepy/glmFit.py` & `inmoose-0.5.0/inmoose/edgepy/glmFit.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,26 +18,25 @@
 
 # This file is based on the file 'R/glmfit.R' of the Bioconductor edgeR package (version 3.38.4).
 
 
 import numpy as np
 import pandas as pd
 import scipy
+from patsy import DesignMatrix, dmatrix
 
 from ..utils import asfactor
 from .DGEGLM import DGEGLM
 from .DGELRT import DGELRT
 from .makeCompressedMatrix import _compressDispersions, _compressOffsets
 from .mglmLevenberg import mglmLevenberg
 from .mglmOneWay import designAsFactor, mglmOneWay
 from .nbinomDeviance import nbinomDeviance
 from .predFC import predFC
 
-from patsy import dmatrix, DesignMatrix
-
 
 def glmFit_DGEList(self, design=None, dispersion=None, prior_count=0.125, start=None):
     """
     Fit a negative binomial generalized log-linear model to the read counts for
     each gene. Conduct genewise statistical tests for a given coefficient or
     coefficient contrast.
```

### Comparing `inmoose-0.4.1/inmoose/edgepy/glmQLFit.py` & `inmoose-0.5.0/inmoose/edgepy/glmQLFit.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -18,19 +18,19 @@
 
 # This file is based on the files 'R/glmQLFTest.R' and 'src/R_check_poisson_bound.cpp' of the Bioconductor edgeR package (version 3.38.4).
 
 import numpy as np
 import patsy
 import scipy
 
+from ..limma import squeezeVar
 from .aveLogCPM import aveLogCPM
 from .DGEGLM import DGEGLM
 from .glmFit import glmFit, glmLRT
 from .residDF import _residDF
-from ..limma import squeezeVar
 
 
 def glmQLFit_DGEList(
     self,
     design=None,
     dispersion=None,
     abundance_trend=True,
```

### Comparing `inmoose-0.4.1/inmoose/edgepy/makeCompressedMatrix.py` & `inmoose-0.5.0/inmoose/edgepy/makeCompressedMatrix.py`

 * *Files identical despite different names*

### Comparing `inmoose-0.4.1/inmoose/edgepy/maximizeInterpolant.py` & `inmoose-0.5.0/inmoose/edgepy/maximizeInterpolant.py`

 * *Files identical despite different names*

### Comparing `inmoose-0.4.1/inmoose/edgepy/mglmLevenberg.py` & `inmoose-0.5.0/inmoose/edgepy/mglmLevenberg.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 # -----------------------------------------------------------------------------
 
 # This file is based on the file 'R/mglmLevenberg.R' of the Bioconductor edgeR package (version 3.38.4).
 
 
 import numpy as np
 
-from .edgepy_cpp import cxx_get_levenberg_start, cxx_fit_levenberg
+from .edgepy_cpp import cxx_fit_levenberg, cxx_get_levenberg_start
 from .makeCompressedMatrix import (
     _compressDispersions,
     _compressOffsets,
     _compressWeights,
 )
 from .utils import _isAllZero
```

### Comparing `inmoose-0.4.1/inmoose/edgepy/mglmOneGroup.py` & `inmoose-0.5.0/inmoose/edgepy/mglmOneGroup.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,23 +16,24 @@
 # along with this program.  If not, see <https://www.gnu.org/licenses/>.
 # -----------------------------------------------------------------------------
 
 # This file is based on the file 'R/mglmOneGroup.R' of the Bioconductor edgeR package (version 3.38.4).
 
 
 import logging
+
 import numpy as np
 
+from .edgepy_cpp import cxx_fit_one_group
 from .makeCompressedMatrix import (
     _compressDispersions,
     _compressOffsets,
     _compressWeights,
 )
 from .utils import _isAllZero
-from .edgepy_cpp import cxx_fit_one_group
 
 
 def mglmOneGroup(
     y,
     dispersion=0,
     offset=0,
     weights=None,
```

### Comparing `inmoose-0.4.1/inmoose/edgepy/mglmOneWay.py` & `inmoose-0.5.0/inmoose/edgepy/mglmOneWay.py`

 * *Files 0% similar despite different names*

```diff
@@ -16,23 +16,24 @@
 # along with this program.  If not, see <https://www.gnu.org/licenses/>.
 # -----------------------------------------------------------------------------
 
 # This file is based on the file 'R/mglmOneWay.R' of the Bioconductor edgeR package (version 3.38.4).
 
 
 import numpy as np
+from scipy.linalg import solve
+
 from ..utils import Factor, asfactor
+from .edgepy_cpp import cxx_get_one_way_fitted
 from .makeCompressedMatrix import (
-    _compressOffsets,
     _compressDispersions,
+    _compressOffsets,
     _compressWeights,
 )
 from .mglmOneGroup import mglmOneGroup
-from .edgepy_cpp import cxx_get_one_way_fitted
-from scipy.linalg import solve
 
 
 def designAsFactor(design):
     """
     Convert a general design matrix into a oneway layout if that is possible.
 
     This function determines how many distinct row values the design matrix is
```

### Comparing `inmoose-0.4.1/inmoose/edgepy/movingAverageByCol.py` & `inmoose-0.5.0/inmoose/edgepy/movingAverageByCol.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,17 +16,18 @@
 # along with this program.  If not, see <https://www.gnu.org/licenses/>.
 # -----------------------------------------------------------------------------
 
 # This file is based on the file 'R/movingAverageByCol.R' of the Bioconductor edgeR package (version 3.38.4).
 
 
 import logging
-import numpy as np
 from math import ceil, floor
 
+import numpy as np
+
 
 def movingAverageByCol(x, width=5, full_length=True):
     """
     Moving average smoother for matrix columns.
 
     Arguments
     ---------
```

### Comparing `inmoose-0.4.1/inmoose/edgepy/nbinomDeviance.py` & `inmoose-0.5.0/inmoose/edgepy/nbinomDeviance.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,16 +16,17 @@
 # along with this program.  If not, see <https://www.gnu.org/licenses/>.
 # -----------------------------------------------------------------------------
 
 # This file is based on the file 'R/nbinomDeviance.R' of the Bioconductor edgeR package (version 3.38.4).
 
 
 import numpy as np
+
+from .edgepy_cpp import cxx_compute_nbdev_nosum, cxx_compute_nbdev_sum
 from .makeCompressedMatrix import _compressDispersions, _compressWeights
-from .edgepy_cpp import cxx_compute_nbdev_sum, cxx_compute_nbdev_nosum
 
 
 def nbinomDeviance(y, mean, dispersion=0, weights=None):
     """
     Residual deviances for row-wise negative binomial GLMs.
 
     This function computes the total residual deviance for each row of :code:`y`,
```

### Comparing `inmoose-0.4.1/inmoose/edgepy/predFC.py` & `inmoose-0.5.0/inmoose/edgepy/predFC.py`

 * *Files 0% similar despite different names*

```diff
@@ -16,14 +16,15 @@
 # along with this program.  If not, see <https://www.gnu.org/licenses/>.
 # -----------------------------------------------------------------------------
 
 # This file is based on the file 'R/predFC.R' of the Bioconductor edgeR package (version 3.38.4).
 
 
 import logging
+
 import numpy as np
 
 from .addPriorCount import addPriorCount
 
 
 def predFC_DGEList(
     self, design, prior_count=0.125, offset=None, dispersion=None, weights=None
```

### Comparing `inmoose-0.4.1/inmoose/edgepy/q2qnbinom.py` & `inmoose-0.5.0/inmoose/edgepy/q2qnbinom.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,15 +14,14 @@
 
 # You should have received a copy of the GNU General Public License
 # along with this program.  If not, see <https://www.gnu.org/licenses/>.
 # -----------------------------------------------------------------------------
 
 # This file is based on the file 'R/q2qnbinom.R' of the Bioconductor edgeR package (version 3.38.4).
 
-import numpy as np
 from .edgepy_cpp import _q2qnbinom
 
 
 # the actual implementation in done in Cython
 # this Python wrapper allows to use optional and named arguments
 def q2qnbinom(x, input_mean, output_mean, dispersion=0):
     """
```

### Comparing `inmoose-0.4.1/inmoose/edgepy/residDF.py` & `inmoose-0.5.0/inmoose/edgepy/residDF.py`

 * *Files identical despite different names*

### Comparing `inmoose-0.4.1/inmoose/edgepy/splitIntoGroups.py` & `inmoose-0.5.0/inmoose/edgepy/splitIntoGroups.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,14 +16,15 @@
 # along with this program.  If not, see <https://www.gnu.org/licenses/>.
 # -----------------------------------------------------------------------------
 
 # This file is based on the file 'R/splitIntoGroups.R' of the Bioconductor edgeR package (version 3.38.4).
 
 
 import numpy as np
+
 from ..utils import asfactor
 
 
 def splitIntoGroups_DGEList(self):
     """
     Split the counts according to group
```

### Comparing `inmoose-0.4.1/inmoose/edgepy/stats.py` & `inmoose-0.5.0/inmoose/edgepy/stats.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 # along with this program.  If not, see <https://www.gnu.org/licenses/>.
 # -----------------------------------------------------------------------------
 
 # This file wraps scipy.stats functions into R-like functions.
 
 
 import numpy as np
-from scipy.stats import norm, gamma, nbinom
+from scipy.stats import gamma, nbinom, norm
 
 
 def rbinom(n, size, prob=None, mu=None, seed=None):
     if prob is None and mu is None:
         raise ValueError("exactly one of prob and mu must be provided")
     if prob is not None and mu is not None:
         raise ValueError("exactly one of prob and mu must be provided")
```

### Comparing `inmoose-0.4.1/inmoose/edgepy/systematicSubset.py` & `inmoose-0.5.0/inmoose/edgepy/systematicSubset.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,17 +15,18 @@
 # You should have received a copy of the GNU General Public License
 # along with this program.  If not, see <https://www.gnu.org/licenses/>.
 # -----------------------------------------------------------------------------
 
 # This file is based on the file 'R/systematicSubset.R' of the Bioconductor edgeR package (version 3.38.4).
 
 
-import numpy as np
 from math import floor
 
+import numpy as np
+
 
 def systematicSubset(n, order_by):
     """
     Take a systematic subset of indices stratified by a ranking variable
 
     Arguments
     ---------
```

### Comparing `inmoose-0.4.1/inmoose/edgepy/topTags.py` & `inmoose-0.5.0/inmoose/edgepy/topTags.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 # You should have received a copy of the GNU General Public License
 # along with this program.  If not, see <https://www.gnu.org/licenses/>.
 # -----------------------------------------------------------------------------
 
 # This file is based on the files 'R/topTags.R' of the Bioconductor edgeR package (version 3.38.4).
 
 import logging
+
 import numpy as np
 import pandas as pd
 from statsmodels.stats.multitest import multipletests
 
 from .DGEExact import DGEExact
```

### Comparing `inmoose-0.4.1/inmoose/edgepy/utils.py` & `inmoose-0.5.0/inmoose/edgepy/utils.py`

 * *Files identical despite different names*

### Comparing `inmoose-0.4.1/inmoose/edgepy/validDGEList.py` & `inmoose-0.5.0/inmoose/edgepy/validDGEList.py`

 * *Files 8% similar despite different names*

```diff
@@ -16,14 +16,15 @@
 # along with this program.  If not, see <https://www.gnu.org/licenses/>.
 # -----------------------------------------------------------------------------
 
 # This file is based on the file 'R/validDGEList.R' of the Bioconductor edgeR package (version 3.38.4).
 
 
 import numpy as np
+
 from ..utils import gl
 
 
 def validDGEList(y):
     """
     Check for standard components of DGEList object
 
@@ -39,15 +40,15 @@
     DGEList
         the input :code:`y`, with missing components added
     """
     if y.counts is None:
         raise RuntimeError("No count matrix")
     y.counts = np.asarray(y.counts, order="F")
     nlib = y.counts.shape[1]
-    if (y.samples.group.values == None).any():
+    if (y.samples.group.values == None).any():  # noqa: E711
         y.samples.group = gl(1, nlib)
-    if (y.samples.lib_size.values == None).any():
+    if (y.samples.lib_size.values == None).any():  # noqa: E711
         y.samples.lib_size = y.counts.sum(axis=0)
-    if (y.samples.norm_factors.values == None).any():
+    if (y.samples.norm_factors.values == None).any():  # noqa: E711
         y.samples.norm_factors = np.ones(nlib)
 
     return y
```

### Comparing `inmoose-0.4.1/inmoose/limma/fitFDist.py` & `inmoose-0.5.0/inmoose/limma/fitFDist.py`

 * *Files 10% similar despite different names*

```diff
@@ -15,18 +15,19 @@
 # You should have received a copy of the GNU General Public License
 # along with this program.  If not, see <https://www.gnu.org/licenses/>.
 # -----------------------------------------------------------------------------
 
 # This file is based on the file 'R/fitFDist.R' of the Bioconductor limma package (version 3.55.1).
 
 import logging
+
 import numpy as np
-import patsy
 from scipy.special import digamma, polygamma
-from scipy.linalg import lstsq, qr
+
+from ..utils import lm_fit, ns
 
 
 def fitFDist(x, df1, covariate=None):
     """
     Moment estimation of the parameters of a scaled F-distribution given one of the degrees of freedom.
 
     This function is called internally by :func:`eBayes` and :func:`squeezeVar`
@@ -146,43 +147,26 @@
     e = z - digamma(df1 / 2) + np.log(df1 / 2)
 
     if covariate is None:
         emean = e.mean()
         evar = np.sum((e - emean) ** 2 / (nok - 1))
     else:
         try:
-            # design = splines_ns(covariate, df=splinedf, intercept=True)
-            design = patsy.dmatrix("cr(covariate, df=splinedf)")
-        except:
+            design = ns(covariate, df=splinedf, include_intercept=True)
+        except:  # noqa: E722
             raise RuntimeError("Problem with covariate")
-        # fit = lm.fit(design,e)
-        coefficients, _, rank, _ = lstsq(design, e)
-        fitted_values = design @ coefficients
+        fit = lm_fit(design.basis, e)
         if notallok:
-            # design2 = predict(design, newx=covariate_notok)
-            (design2,) = patsy.build_design_matrices(
-                [design.design_info], {"covariate": covariate_notok}
-            )
+            design2 = design.predict(newx=covariate_notok)
             emean = np.zeros(n)
-            emean[ok] = fitted_values
-            emean[~ok] = design2 @ coefficients
+            emean[ok] = fit.fitted_values
+            emean[~ok] = design2.basis @ fit.coefficients
         else:
-            emean = fitted_values
-        # lstsq does not return the effects, so let us compute them manually
-        # Reminder: to solve AX = Y for X, we use QR decomposition of A
-        #   A = QR, where Q is orthogonal and R is upper triangular
-        # thus, AX = Y boils down to a triangular system RX = QtY
-        # Given a solution Z, it may not be exact (because the system was
-        # over-determined for example):
-        #   QtY = Qt(AZ + E) = RZ + QtE
-        # E = Y-AZ is the error, QtE is the effect
-        Q, R = qr(design, mode="full")
-        effects = Q.T @ (e - fitted_values)
-        # evar = (fit.effects[rank:] ** 2).mean()
-        evar = (effects[rank:] ** 2).mean()
+            emean = fit.fitted_values
+        evar = (fit.effects[fit.rank :] ** 2).mean()
 
     # Estimate scale and df2
     evar = evar - polygamma(1, df1 / 2).mean()
     if evar > 0:
         df2 = 2 * trigammaInverse(evar)
         s20 = np.exp(emean + digamma(df2 / 2) - np.log(df2 / 2))
     else:
```

### Comparing `inmoose-0.4.1/inmoose/limma/squeezeVar.py` & `inmoose-0.5.0/inmoose/limma/squeezeVar.py`

 * *Files identical despite different names*

### Comparing `inmoose-0.4.1/inmoose/pycombat/covariates.py` & `inmoose-0.5.0/inmoose/pycombat/covariates.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,17 +12,18 @@
 # GNU General Public License for more details.
 
 # You should have received a copy of the GNU General Public License
 # along with this program.  If not, see <https://www.gnu.org/licenses/>.
 # -----------------------------------------------------------------------------
 
 import logging
+
 import numpy as np
 import pandas as pd
-from patsy import dmatrix, DesignMatrix
+from patsy import DesignMatrix, dmatrix
 
 from ..utils import asfactor
 
 
 class VirtualCohortInput:
     """
     Attributes
@@ -288,17 +289,15 @@
         :class:`~inmoose.utils.factor.Factor`
             resulting batch identifiers
         :class:`patsy.DesignMatrix`
             resulting covariate Matrix
         """
         nan_covar_mod = self.covar_mod.isna()
         if na_cov_action == "raise":
-            name_nan_covar_mod = nan_covar_mod.loc[
-                :, nan_covar_mod.any() == True
-            ].columns
+            name_nan_covar_mod = nan_covar_mod.loc[:, nan_covar_mod.any()].columns
             raise ValueError(
                 f"{nan_covar_mod.sum().sum()} values are missing in covariates {', '.join(name_nan_covar_mod)}. Correct your covariates or use the cov_missing_value parameters"
             )
         elif na_cov_action == "remove":
             logging.warnings.warn(
                 f"{(nan_covar_mod.sum(axis=1)>0).sum()} samples with missing covariates in covar_mod. They are removed from the data. You may want to double check your covariates."
             )
```

### Comparing `inmoose-0.4.1/inmoose/pycombat/helper_seq.py` & `inmoose-0.5.0/inmoose/pycombat/helper_seq.py`

 * *Files identical despite different names*

### Comparing `inmoose-0.4.1/inmoose/pycombat/pycombat_norm.py` & `inmoose-0.5.0/inmoose/pycombat/pycombat_norm.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,22 +12,22 @@
 # GNU General Public License for more details.
 
 # You should have received a copy of the GNU General Public License
 # along with this program.  If not, see <https://www.gnu.org/licenses/>.
 # -----------------------------------------------------------------------------
 
 import logging
-import numpy as np
 from functools import partial
+
 import mpmath as mp
+import numpy as np
 import pandas as pd
 
 from .covariates import make_design_matrix
 
-
 # aprior and bprior are useful to compute "hyper-prior values"
 # -> prior parameters used to estimate the prior gamma distribution for multiplicative batch effect
 # aprior - calculates empirical hyper-prior values
 
 
 def compute_prior(prior, gamma_hat, mean_only):
     """[summary]
@@ -163,15 +163,15 @@
         n = len(x)
         j = [1] * n
         dat = np.repeat(x, len(np.transpose(g)), axis=1)
         resid2 = np.square(dat - g)
         sum2 = np.dot(np.transpose(resid2), j)
         # /begin{handling high precision computing}
         temp_2d = 2 * d
-        if precision == None:
+        if precision is None:
             LH = np.power(1 / (np.pi * temp_2d), n / 2) * np.exp(
                 np.negative(sum2) / (temp_2d)
             )
 
         else:  # only if precision parameter informed
             # increase the precision of the computing (if negative exponential too close to 0)
             mp.dps = precision
@@ -216,17 +216,15 @@
         t2 {matrix} --
         a_prior {float} -- aprior
         b_prior {float} -- bprior
 
     Returns:
         array list -- estimated adjusted additive and multiplicative batch effect
     """
-    if (
-        mean_only
-    ):  # if mean_only, no need for complex method: batch effect is immediately calculated
+    if mean_only:  # if mean_only, no need for complex method: batch effect is immediately calculated
         t2_n = np.multiply(t2[i], 1)
         t2_n_g_hat = np.multiply(t2_n, gamma_hat[i])
         gamma_star = postmean(
             gamma_bar[i], 1, t2_n, t2_n_g_hat
         )  # additive batch effect
         delta_star = [1] * len(s_data)  # multiplicative batch effect
     else:  # if not(mean_only) then use it_solve
@@ -280,15 +278,15 @@
 
     Arguments:
         mean_only {boolean} -- user's choice about mean_only
 
     Returns:
         ()
     """
-    if mean_only == True:
+    if mean_only:
         logging.info("Using mean only version")
 
 
 def calculate_mean_var(design, batches, ref, dat, n_batches, n_batch, n_array):
     """calculates the Normalisation factors
 
     Arguments:
```

### Comparing `inmoose-0.4.1/inmoose/pycombat/pycombat_seq.py` & `inmoose-0.5.0/inmoose/pycombat/pycombat_seq.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,21 +15,21 @@
 # You should have received a copy of the GNU General Public License
 # along with this program.  If not, see <https://www.gnu.org/licenses/>.
 # -----------------------------------------------------------------------------
 
 # This file is based on the file 'R/ComBat_seq.R' of the Bioconductor sva package (version 3.44.0).
 
 import logging
+
 import numpy as np
 import pandas as pd
 
 from ..edgepy import DGEList, estimateGLMCommonDisp, estimateGLMTagwiseDisp, glmFit
-from ..utils import asfactor
 from .covariates import make_design_matrix
-from .helper_seq import vec2mat, match_quantiles
+from .helper_seq import match_quantiles, vec2mat
 
 
 def pycombat_seq(
     counts,
     batch,
     covar_mod=None,
     shrink=False,
```

### Comparing `inmoose-0.4.1/inmoose/sim/splat.py` & `inmoose-0.5.0/inmoose/sim/splat.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,16 +18,16 @@
 """
 This module contains utilities to simulate RNASeq and single-cell RNASeq count
 data. It follows the Splat model, as described in https://genomebiology.biomedcentral.com/articles/10.1186/s13059-017-1305-0.
 Yet it is a completely independent implementation.
 """
 
 import numpy as np
-from scipy.stats import gamma, lognorm, chi2, poisson, bernoulli
 from scipy.special import expit
+from scipy.stats import bernoulli, chi2, gamma, lognorm, poisson
 
 
 def get_lognorm_factors(size, sel_prob, neg_prob, loc, scale, random_state):
     """
     Draw log-normal factors.
 
     Arguments
```

### Comparing `inmoose-0.4.1/inmoose/utils/_stats.pyx` & `inmoose-0.5.0/inmoose/utils/_stats.pyx`

 * *Files identical despite different names*

### Comparing `inmoose-0.4.1/inmoose/utils/factor.py` & `inmoose-0.5.0/inmoose/utils/factor.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,15 +12,14 @@
 # GNU General Public License for more details.
 
 # You should have received a copy of the GNU General Public License
 # along with this program.  If not, see <https://www.gnu.org/licenses/>.
 # -----------------------------------------------------------------------------
 
 
-import numpy as np
 from pandas import Categorical
 
 
 class Factor(Categorical):
     """
     A class to represent a factor, as in R.
```

### Comparing `inmoose-0.4.1/inmoose/utils/stats.py` & `inmoose-0.5.0/inmoose/utils/stats.py`

 * *Files identical despite different names*

### Comparing `inmoose-0.4.1/inmoose.egg-info/PKG-INFO` & `inmoose-0.5.0/inmoose.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: inmoose
-Version: 0.4.1
+Version: 0.5.0
 Summary: InMoose: the Integrated Multi Omic Open Source Environment
 Author-email: Maximilien Colange <maximilien@epigenelabs.com>, Léa Meunier <lea@epigenelabs.com>, Solène Weill <solene@epigenelabs.com>
 Project-URL: Source, https://github.com/epigenelabs/inmoose
 Project-URL: Documentation, https://inmoose.readthedocs.io/en/latest/
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
@@ -45,18 +45,18 @@
 
 Documentation is hosted on [readthedocs.org](https://inmoose.readthedocs.io/en/latest/).
 
 # Batch Effect Correction
 
 InMoose provides features to correct technical biases, also called batch
 effects, in transcriptomic data:
-- for microarray data, InMoose supersedes pyCombat [1], a Python 3
+- for microarray data, InMoose supersedes pyCombat [1], a Python3
   implementation of ComBat [2], one of the most widely used tool for batch effect
   correction on microarray data.
-- for RNASeq, InMoose features a port to Python3 of ComBat-Seq [3], one of the
+- for RNASeq data, InMoose features a port to Python3 of ComBat-Seq [3], one of the
   most widely used tool for batch effect correction on RNASeq data.
 
 To use these functions, simply import them and call them with default
 parameters:
 ```python
 from inmoose.pycombat import pycombat_norm, pycombat_seq
 
@@ -66,14 +66,27 @@
 
 * `microarray_data`, `rnaseq_data`: the expression matrices, containing the
   information about the gene expression (rows) for each sample (columns).
 * `microarray_batches`, `rnaseq_batches`: list of batch indices, describing the
   batch for each sample. The list of batches should contain as many elements as
   the number of samples in the expression matrix.
 
+# Differential Expression Analysis
+
+InMoose provides features to analyse diffentially expressed genes in bulk
+transcriptomic data:
+- for microarray data, InMoose features a port of limma [4], the *de
+  facto* standard tool for differential expression analysis on microarray data.
+- for RNASeq data, InMoose features a ports to Python3 of edgeR [5] and DESeq2
+  [6], two of the most widely used tools for differential expression analysis on
+  RNASeq data.
+
+See the dedicated sections of the
+[documentation](https://inmoose.readthedocs.io/en/latest/).
+
 # Consensus clustering
 InMoose provides features to compute consensus clustering, a resampling based algorithm compatible with any clustering algorithms which class implementation is instantiated with parameter `n_clusters`, and possess a `fit_predict` method, which is invoked on data.
 Consensus clustering helps determining the best number of clusters to use and output confidence metrics and plots.
 
 
 To use these functions, import the consensusClustering class and a clustering algorithm class:
 ```python
```

### Comparing `inmoose-0.4.1/inmoose.egg-info/SOURCES.txt` & `inmoose-0.5.0/inmoose.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -106,26 +106,36 @@
 inmoose/edgepy/edgepy_cpp/interpolator.cpp
 inmoose/edgepy/edgepy_cpp/interpolator.h
 inmoose/edgepy/edgepy_cpp/maximize_interpolant.cpp
 inmoose/edgepy/edgepy_cpp/objects.cpp
 inmoose/edgepy/edgepy_cpp/objects.h
 inmoose/edgepy/edgepy_cpp/utils.h
 inmoose/limma/__init__.py
+inmoose/limma/contrasts.py
+inmoose/limma/decidetests.py
+inmoose/limma/dups.py
+inmoose/limma/ebayes.py
 inmoose/limma/fitFDist.py
+inmoose/limma/lmfit.py
+inmoose/limma/marraylm.py
 inmoose/limma/squeezeVar.py
+inmoose/limma/toptable.py
 inmoose/pycombat/__init__.py
 inmoose/pycombat/covariates.py
 inmoose/pycombat/helper_seq.py
 inmoose/pycombat/pycombat_norm.py
 inmoose/pycombat/pycombat_seq.py
 inmoose/sim/__init__.py
 inmoose/sim/splat.py
 inmoose/utils/__init__.py
 inmoose/utils/_stats.pyx
 inmoose/utils/factor.py
+inmoose/utils/linalg.py
+inmoose/utils/lm.py
+inmoose/utils/splines.py
 inmoose/utils/stats.py
 tests/__init__.py
 tests/consensus_clustering/__init__.py
 tests/consensus_clustering/mocked_data_consensus_clustering.csv
 tests/consensus_clustering/test_consensus_clustering.py
 tests/data/__init__.py
 tests/data/test_airway.py
@@ -166,17 +176,25 @@
 tests/edgepy/test_mglm.py
 tests/edgepy/test_nbinomDeviance.py
 tests/edgepy/test_objects.py
 tests/edgepy/test_predFC.py
 tests/edgepy/test_q2qnbinom.py
 tests/edgepy/test_stats.py
 tests/limma/__init__.py
+tests/limma/test_contrasts.py
+tests/limma/test_decidetests.py
+tests/limma/test_dups.py
 tests/limma/test_fitFDist.py
+tests/limma/test_lmFit.py
 tests/limma/test_squeezeVar.py
+tests/limma/test_tmixture.py
 tests/pycombat/__init__.py
 tests/pycombat/test_covariates.py
 tests/pycombat/test_pycombat.py
 tests/pycombat/test_pycombatseq.py
 tests/sim/__init__.py
 tests/sim/test_splat.py
 tests/utils/__init__.py
-tests/utils/test_factor.py
+tests/utils/test_factor.py
+tests/utils/test_linalg.py
+tests/utils/test_lm.py
+tests/utils/test_splines.py
```

### Comparing `inmoose-0.4.1/pyproject.toml` & `inmoose-0.5.0/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "inmoose"
-version = "0.4.1"
+version = "0.5.0"
 description = "InMoose: the Integrated Multi Omic Open Source Environment"
 readme = "README.md"
 authors = [
   {name = "Maximilien Colange", email = "maximilien@epigenelabs.com"},
   {name = "Léa Meunier", email = "lea@epigenelabs.com"},
   {name = "Solène Weill", email = "solene@epigenelabs.com"},
 ]
```

### Comparing `inmoose-0.4.1/setup.py` & `inmoose-0.5.0/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,12 +1,24 @@
 import sys
+
 import numpy
 from setuptools import Extension, setup
+from setuptools.command.build_ext import build_ext
+
+
+class build_ext_cxx17(build_ext):
+    def build_extensions(self):
+        std_flag = (
+            "-std:c++17" if self.compiler.compiler_type == "msvc" else "-std=c++17"
+        )
+        for e in self.extensions:
+            e.extra_compile_args.append(std_flag)
+        super().build_extensions()
+
 
-cxx_compile_flags = ["-std=c++17"]
 macros = [("NPY_NO_DEPRECATED_API", "NPY_1_7_API_VERSION")]
 profiling = False
 linetrace = False
 if "--profile" in sys.argv:
     profiling = True
     linetrace = True
     macros += [("CYTHON_TRACE_NOGIL", "1")]
@@ -15,25 +27,23 @@
 common_cpp = Extension(
     "inmoose.common_cpp",
     [
         "inmoose/common_cpp/common_cpp.pyx",
         "inmoose/common_cpp/matrix.cpp",
     ],
     include_dirs=[numpy.get_include()],
-    extra_compile_args=cxx_compile_flags,
     define_macros=macros,
 )
 
 stats_cpp = Extension(
     "inmoose.utils.stats_cpp",
     [
         "inmoose/utils/_stats.pyx",
     ],
     include_dirs=[numpy.get_include()],
-    extra_compile_args=cxx_compile_flags,
     define_macros=macros,
 )
 
 edgepy_cpp = Extension(
     "inmoose.edgepy.edgepy_cpp",
     [
         "inmoose/edgepy/edgepy_cpp/edgepy_cpp.pyx",
@@ -43,20 +53,20 @@
         "inmoose/edgepy/edgepy_cpp/fit_levenberg.cpp",
         "inmoose/edgepy/edgepy_cpp/glm_levenberg.cpp",
         "inmoose/edgepy/edgepy_cpp/glm_one_group.cpp",
         "inmoose/edgepy/edgepy_cpp/interpolator.cpp",
         "inmoose/edgepy/edgepy_cpp/objects.cpp",
     ],
     include_dirs=[numpy.get_include(), "inmoose/common_cpp/"],
-    extra_compile_args=cxx_compile_flags,
     define_macros=macros,
 )
 
 
 setup(
+    cmdclass={"build_ext": build_ext_cxx17},
     packages=[
         "inmoose",
         "inmoose/consensus_clustering",
         "inmoose/data",
         "inmoose/data/airway",
         "inmoose/data/pasilla",
         "inmoose/pycombat",
```

### Comparing `inmoose-0.4.1/tests/consensus_clustering/mocked_data_consensus_clustering.csv` & `inmoose-0.5.0/tests/consensus_clustering/mocked_data_consensus_clustering.csv`

 * *Files identical despite different names*

### Comparing `inmoose-0.4.1/tests/consensus_clustering/test_consensus_clustering.py` & `inmoose-0.5.0/tests/consensus_clustering/test_consensus_clustering.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,16 @@
-import unittest
-from inmoose.consensus_clustering.consensus_clustering import consensusClustering
-from sklearn.cluster import AgglomerativeClustering
-import pandas as pd
-import numpy as np
 import importlib.resources
 import os
+import unittest
+
+import numpy as np
+import pandas as pd
+from sklearn.cluster import AgglomerativeClustering
+
+from inmoose.consensus_clustering.consensus_clustering import consensusClustering
 
 
 class test_consensusClustering(unittest.TestCase):
     def setUp(self) -> None:
         this_dir = importlib.resources.files(__package__)
         mock_file = this_dir.joinpath("mocked_data_consensus_clustering.csv")
```

### Comparing `inmoose-0.4.1/tests/deseq2/test_DESeq.py` & `inmoose-0.5.0/tests/deseq2/test_DESeq.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import unittest
+
 import patsy
 
-from inmoose.utils import Factor
 from inmoose.deseq2 import DESeq, makeExampleDESeqDataSet
+from inmoose.utils import Factor
 
 
 class Test(unittest.TestCase):
     def test_DESeq(self):
         """test that DESeq() gives correct errors"""
         dds = makeExampleDESeqDataSet(n=100, m=8)
         with self.assertRaisesRegex(
```

### Comparing `inmoose-0.4.1/tests/deseq2/test_DESeqDataSet.py` & `inmoose-0.5.0/tests/deseq2/test_DESeqDataSet.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import unittest
+
 import numpy as np
 from pandas.api.types import CategoricalDtype
 
 from inmoose.deseq2 import DESeqDataSet
 
 
 class Test(unittest.TestCase):
```

### Comparing `inmoose-0.4.1/tests/deseq2/test_LRT.py` & `inmoose-0.5.0/tests/deseq2/test_LRT.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import unittest
 
+from inmoose.deseq2 import DESeq, makeExampleDESeqDataSet, nbinomLRT
 from inmoose.utils import Factor
-from inmoose.deseq2 import makeExampleDESeqDataSet, DESeq, nbinomLRT
 
 
 class Test(unittest.TestCase):
     def test_LRT(self):
         """test that test='LRT' gives correct errors"""
         dds = makeExampleDESeqDataSet(n=100, m=4)
         dds.obs["group"] = Factor([1, 2, 1, 2])
```

### Comparing `inmoose-0.4.1/tests/deseq2/test_addMLE.py` & `inmoose-0.5.0/tests/deseq2/test_addMLE.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import unittest
+
 import numpy as np
 
+from inmoose.deseq2 import DESeq, makeExampleDESeqDataSet, nbinomWaldTest
 from inmoose.utils import Factor
-from inmoose.deseq2 import makeExampleDESeqDataSet, DESeq, nbinomWaldTest
 
 
 class Test(unittest.TestCase):
     def test_addMLE(self):
         """test that adding MLE works as expected"""
         dds = makeExampleDESeqDataSet(n=200, m=12, betaSD=1, seed=42)
         dds.obs["condition"] = Factor(np.repeat(["A", "B", "C"], 4))
```

### Comparing `inmoose-0.4.1/tests/deseq2/test_betaFitting.py` & `inmoose-0.5.0/tests/deseq2/test_betaFitting.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 import unittest
+
 import numpy as np
 import pandas as pd
 import scipy.stats
 from scipy.optimize import minimize
 
-from inmoose.utils import Factor, dnbinom_mu, dnorm
 from inmoose.deseq2 import DESeqDataSet
 from inmoose.deseq2.fitNbinomGLMs import fitNbinomGLMs
+from inmoose.utils import Factor, dnbinom_mu, dnorm
 
 
 class Test(unittest.TestCase):
     def test_betaFitting(self):
         """test that estimates of beta fit from various methods are equal"""
         m = 10
         y = scipy.stats.poisson.rvs(20, size=m, random_state=42)
```

### Comparing `inmoose-0.4.1/tests/deseq2/test_collapse.py` & `inmoose-0.5.0/tests/deseq2/test_collapse.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import unittest
+
 import numpy as np
 
-from inmoose.deseq2 import makeExampleDESeqDataSet, collapseReplicates
+from inmoose.deseq2 import collapseReplicates, makeExampleDESeqDataSet
 
 
 class Test(unittest.TestCase):
     def test_collapse(self):
         """test that collapse replicates works"""
         dds = makeExampleDESeqDataSet(n=10, m=8)
         dds.obs["sample"] = np.repeat([1, 2, 3, 4], 2)
```

### Comparing `inmoose-0.4.1/tests/deseq2/test_dispersions.py` & `inmoose-0.5.0/tests/deseq2/test_dispersions.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 import unittest
+
 import numpy as np
 import pandas as pd
 import patsy
 from scipy.optimize import minimize
-import scipy.stats
 
-from inmoose.utils import Factor, dnbinom_mu, dnorm
 from inmoose.deseq2 import (
-    DESeqDataSet,
-    makeExampleDESeqDataSet,
     DESeq,
-    estimateDispersionsGeneEst,
+    DESeqDataSet,
     estimateDispersionsFit,
+    estimateDispersionsGeneEst,
     estimateDispersionsMAP,
+    makeExampleDESeqDataSet,
 )
-from inmoose.deseq2.fitNbinomGLMs import fitNbinomGLMs
 from inmoose.deseq2.deseq2_cpp import fitDisp
+from inmoose.deseq2.fitNbinomGLMs import fitNbinomGLMs
+from inmoose.utils import Factor, dnbinom_mu, dnorm
 
 
 class Test(unittest.TestCase):
     def test_dispersion_errors(self):
         """test that expected errors are thrown during dispersion estimation"""
         dds = makeExampleDESeqDataSet(n=100, m=2)
         dds = dds.estimateSizeFactors()
@@ -178,15 +178,15 @@
         dispD2Num = num_2nd_deriv(logPost, dispRes["log_alpha"])
         self.assertTrue(np.allclose(dispD2DESeq, dispD2Num))
 
         # test fit alternative
         dds = makeExampleDESeqDataSet()
         dds = dds.estimateSizeFactors()
         # ddsLocal = dds.copy().estimateDispersions(fitType="local")
-        ddsMean = dds.copy().estimateDispersions(fitType="mean")
+        dds.copy().estimateDispersions(fitType="mean")
         ddsMed = estimateDispersionsGeneEst(dds.copy())
         useForMedian = ddsMed.var["dispGeneEst"] > 1e-7
         medianDisp = np.nanmedian(ddsMed.var["dispGeneEst"][useForMedian])
         ddsMed.setDispFunction(lambda x: medianDisp)
         ddsMed = estimateDispersionsMAP(ddsMed)
 
         # test iterative
```

### Comparing `inmoose-0.4.1/tests/deseq2/test_interactions.py` & `inmoose-0.5.0/tests/deseq2/test_interactions.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import unittest
+
 import numpy as np
 import patsy
 
+from inmoose.deseq2 import DESeq, makeExampleDESeqDataSet
 from inmoose.utils import Factor
-from inmoose.deseq2 import makeExampleDESeqDataSet, DESeq
 
 
 @unittest.skip("lfcShrink is not implemented")
 class Test(unittest.TestCase):
     def test_interation_errors(self):
         """test that interactions throw errors"""
         dds = makeExampleDESeqDataSet(n=100, m=8)
@@ -21,21 +22,21 @@
             ValueError, expected_regex="designs with interations"
         ):
             DESeq(dds, betaPrior=True)
 
         # also lfcShrink
         res = dds.results(name="conditionB.groupY")
         with self.assertRaises(NotImplementedError):
-            res = lfcShrink(dds, coef=4, res=res, type="normal")
+            res = lfcShrink(dds, coef=4, res=res, type="normal")  # noqa: F821
 
         res = dds.results(contrast=["condition", "B", "A"])
         with self.assertRaises(NotImplementedError):
-            res = lfcShrink(
+            res = lfcShrink(  # noqa: F821
                 dds, contrast=["condition", "B", "A"], res=res, type="normal"
             )
 
         # however, this is allowed
         dds2 = dds.copy()
         dds2.design = patsy.dmatrix("~ condition + group + condition:group", dds2.obs)
         dds2 = DESeq(dds2)
-        res2 = dds2.results(name="conditionB.groupY")
-        res2 = lfcShrink(dds2, coef=4, res=res, type="normal")
+        dds2.results(name="conditionB.groupY")
+        lfcShrink(dds2, coef=4, res=res, type="normal")  # noqa: F821
```

### Comparing `inmoose-0.4.1/tests/deseq2/test_linear_mu.py` & `inmoose-0.5.0/tests/deseq2/test_linear_mu.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 import unittest
+
 import numpy as np
 
 from inmoose.deseq2 import (
     DESeqDataSet,
-    makeExampleDESeqDataSet,
-    estimateDispersionsGeneEst,
     estimateDispersionsFit,
+    estimateDispersionsGeneEst,
     estimateDispersionsMAP,
+    makeExampleDESeqDataSet,
     nbinomWaldTest,
 )
 
 
 class Test(unittest.TestCase):
     def test_linear_mu(self):
         """test that the use of linear model for fitting mu works as expected"""
@@ -31,8 +32,8 @@
         mu2 = dds2.layers["mu"]
         cors = np.diag(np.corrcoef(mu1, mu2)[: mu1.shape[0], mu1.shape[1] :])
         self.assertTrue(np.all(cors > 1 - 1e-6))
 
         dds2 = estimateDispersionsFit(dds2, fitType="mean")
         dds2 = estimateDispersionsMAP(dds2)
         dds2 = nbinomWaldTest(dds2)
-        res = dds2.results()
+        dds2.results()
```

### Comparing `inmoose-0.4.1/tests/deseq2/test_methods.py` & `inmoose-0.5.0/tests/deseq2/test_methods.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import unittest
+
 import numpy as np
 import pandas as pd
 
-from inmoose.utils import Factor
 from inmoose.deseq2 import DESeqDataSet
+from inmoose.utils import Factor
 
 
 class Test(unittest.TestCase):
     def test_method_errors(self):
         """test that methods throw errors"""
         coldata = pd.DataFrame({"x": Factor(["A", "A", "B", "B"])})
         counts = np.arange(1, 17).reshape((4, 4))
```

### Comparing `inmoose-0.4.1/tests/deseq2/test_model_matrix.py` & `inmoose-0.5.0/tests/deseq2/test_model_matrix.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 import unittest
+
 import numpy as np
 import pandas as pd
 import patsy
 import scipy.stats
 
+from inmoose.deseq2 import DESeq, DESeqDataSet, makeExampleDESeqDataSet
 from inmoose.utils import Factor
-from inmoose.deseq2 import makeExampleDESeqDataSet, DESeq, DESeqDataSet
 
 
 class Test(unittest.TestCase):
     def test_model_matrix(self):
         """test that supplying custom model matrix works"""
         dds = makeExampleDESeqDataSet(n=100, m=18)
         dds.obs["group"] = Factor(np.repeat([1, 2, 3], [6, 6, 6]))
@@ -21,15 +22,15 @@
         dds = dds[:16]
 
         m1 = patsy.dmatrix("~ group*condition", dds.obs)
         m2 = m1[:, :8]
         m2.design_info = m1.design_info
         m1 = m2
         m1.design_info.column_name_indexes.popitem()
-        m0 = patsy.dmatrix("~ group + condition", dds.obs)
+        # m0 = patsy.dmatrix("~ group + condition", dds.obs)
 
         # TODO
         # dds = DESeq(dds, full=m1, reduced=m0, test="LRT")
         # dds.result()
         # dds.results(name="group2.conditionC", test="Wald")
         dds = dds.removeResults()
         dds = DESeq(dds, full=m1, test="Wald", betaPrior=False)
```

### Comparing `inmoose-0.4.1/tests/deseq2/test_nbinomWald.py` & `inmoose-0.5.0/tests/deseq2/test_nbinomWald.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 import unittest
+
 import numpy as np
 import patsy
 
-from inmoose.utils import Factor, pt
 from inmoose.deseq2 import (
-    makeExampleDESeqDataSet,
-    nbinomWaldTest,
-    nbinomLRT,
     DESeq,
-    estimateMLEForBetaPriorVar,
     estimateBetaPriorVar,
     estimateDispersionsGeneEst,
+    estimateMLEForBetaPriorVar,
+    makeExampleDESeqDataSet,
+    nbinomLRT,
+    nbinomWaldTest,
 )
+from inmoose.utils import Factor, pt
 
 
 class Test(unittest.TestCase):
     def test_nbinomWald_errors(self):
         """test that nbinomWald throws various errors and works with edge cases"""
         dds = makeExampleDESeqDataSet(n=100, m=4)
         with self.assertRaisesRegex(
@@ -28,15 +29,15 @@
             expected_regex="testing requires dispersion estimates, first call estimateDispersions()",
         ):
             nbinomLRT(dds)
 
         dds = dds.estimateSizeFactors()
         dds = dds.estimateDispersions()
         mm = patsy.dmatrix("~condition", dds.obs)
-        mm0 = patsy.dmatrix("~1", dds.obs)
+        # mm0 = patsy.dmatrix("~1", dds.obs)
         with self.assertRaisesRegex(
             ValueError,
             expected_regex="user-supplied model matrix with betaPrior=True requires supplying betaPriorVar",
         ):
             nbinomWaldTest(dds, betaPrior=True, modelMatrix=mm)
         # TODO
         # with self.assertRaisesRegex(ValueError, expected_regex="unused argument (betaPrior = TRUE)"):
```

### Comparing `inmoose-0.4.1/tests/deseq2/test_optim.py` & `inmoose-0.5.0/tests/deseq2/test_optim.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import unittest
+
 import numpy as np
 import patsy
 import scipy.stats
 
-from inmoose.deseq2 import makeExampleDESeqDataSet, DESeq
+from inmoose.deseq2 import DESeq, makeExampleDESeqDataSet
 from inmoose.deseq2.fitNbinomGLMs import fitNbinomGLMs
 
 
 class Test(unittest.TestCase):
     def test_optim(self):
         """test that optim gives same results"""
         dds = makeExampleDESeqDataSet(n=100, interceptMean=10, interceptSD=3, seed=51)
```

### Comparing `inmoose-0.4.1/tests/deseq2/test_outlier.py` & `inmoose-0.5.0/tests/deseq2/test_outlier.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import unittest
+
 import numpy as np
 from scipy.stats import f
 
-from inmoose.deseq2 import makeExampleDESeqDataSet, DESeq, replaceOutliers
+from inmoose.deseq2 import DESeq, makeExampleDESeqDataSet, replaceOutliers
 
 
 class Test(unittest.TestCase):
     def test_outlier_filtering_replacement(self):
         """test that outlier filtering and replacement works as expected"""
         dds = makeExampleDESeqDataSet(
             n=100, m=12, dispMeanRel=lambda x: 4 / x + 0.5, seed=42
```

### Comparing `inmoose-0.4.1/tests/deseq2/test_results.py` & `inmoose-0.5.0/tests/deseq2/test_results.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 import unittest
+
 import numpy as np
 
-from inmoose.utils import Factor
 from inmoose.deseq2 import DESeq, makeExampleDESeqDataSet
+from inmoose.utils import Factor
 
 
 class Test(unittest.TestCase):
     def test_results(self):
         """test that results work as expected and throw errors"""
-        ## test contrasts
+        # test contrasts
         dds = makeExampleDESeqDataSet(n=200, m=12, seed=42)
         dds.obs["condition"] = Factor(np.repeat([1, 2, 3], 4))
         dds.obs["group"] = Factor(np.repeat([[1, 2]], 6, axis=0).flatten())
         dds.obs["foo"] = np.repeat(["lo", "hi"], 6)
         dds.counts()[:, 0] = np.repeat([100, 200, 800], 4)
 
         dds.design = "~ group + condition"
@@ -308,12 +309,12 @@
         self.assertTrue(dds.var.description.filter("results").empty)
 
     @unittest.skip("not sure what to test")
     def test_results_custom_filters(self):
         """test that custom filters can be provided to results()"""
         dds = makeExampleDESeqDataSet(n=200, m=4, betaSD=np.repeat([0, 2], [150, 50]))
         dds = DESeq(dds)
-        res = dds.results()
-        method = "BH"
-        alpha = 0.1
+        _res = dds.results()
+        _method = "BH"
+        _alpha = 0.1
 
         raise NotImplementedError()
```

### Comparing `inmoose-0.4.1/tests/deseq2/test_size_factor.py` & `inmoose-0.5.0/tests/deseq2/test_size_factor.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 import unittest
+
 import numpy as np
 import pandas as pd
 import patsy
 
 from inmoose.deseq2 import (
-    estimateSizeFactorsForMatrix,
     DESeqDataSet,
+    estimateSizeFactorsForMatrix,
     makeExampleDESeqDataSet,
 )
 
 
 class Test(unittest.TestCase):
     def test_size_factor(self):
         """test that size factor works"""
```

### Comparing `inmoose-0.4.1/tests/deseq2/test_vst.py` & `inmoose-0.5.0/tests/deseq2/test_vst.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import unittest
+
 import numpy as np
 
 from inmoose.deseq2 import makeExampleDESeqDataSet, varianceStabilizingTransformation
 
 
 class Test(unittest.TestCase):
     def test_varianceStabilizingTransform(self):
```

### Comparing `inmoose-0.4.1/tests/deseq2/test_weights.py` & `inmoose-0.5.0/tests/deseq2/test_weights.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import unittest
+
 import numpy as np
 import pandas as pd
 
-from inmoose.utils import Factor
-from inmoose.deseq2 import makeExampleDESeqDataSet, DESeq, nbinomWaldTest
+from inmoose.deseq2 import DESeq, makeExampleDESeqDataSet, nbinomWaldTest
 from inmoose.deseq2.fitNbinomGLMs import fitNbinomGLMsOptim
+from inmoose.utils import Factor
 
 
 class Test(unittest.TestCase):
     def test_weights(self):
         """test that weights work"""
         dds = makeExampleDESeqDataSet(n=10, seed=42)
         w = np.ones(dds.shape)
@@ -111,15 +112,15 @@
         with self.assertWarnsRegex(
             UserWarning,
             expected_regex="for 1 genes, the weights as supplied won't allow parameter estimation",
         ):
             dds = DESeq(dds)
         self.assertTrue(dds.var["allZero"].iloc[0])
         self.assertTrue(dds.var["weightsFail"].iloc[0])
-        res = dds.results()
+        dds.results()
 
     @unittest.skip("not sure what is tested here")
     def test_weights_CR(self):
         """test that weights with and without CR term included"""
         alpha = 0.25
 
         def dmr(x):
@@ -135,8 +136,8 @@
         w[0:o, :] = 1e-6
         w[50 : (50 + o), :] = 1e-6
         dds.layers["weights"] = w
         dds.counts()[1:o, :] = 1
         dds.counts()[50 : (50 + o), :] = 1
         dds.sizeFactors = 1
         dds = dds.estimateDispersions(fitType="mean")
-        dds2 = dds.estimateDispersions(fitType="mean", useCR=False)
+        dds.estimateDispersions(fitType="mean", useCR=False)
```

### Comparing `inmoose-0.4.1/tests/deseq2/test_zero_zero.py` & `inmoose-0.5.0/tests/deseq2/test_zero_zero.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import unittest
+
 import numpy as np
 
-from inmoose.utils import Factor
 from inmoose.deseq2 import DESeq, makeExampleDESeqDataSet
+from inmoose.utils import Factor
 
 
 class zero_zero(unittest.TestCase):
     def test_zero_zero(self):
         """test that contrast of two groups with all zeros - LFC zeroed out"""
 
         # test comparison of two groups with all zeros
```

### Comparing `inmoose-0.4.1/tests/edgepy/test_DGEList.py` & `inmoose-0.5.0/tests/edgepy/test_DGEList.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 import unittest
+
 import numpy as np
 
 from inmoose.edgepy import DGEList, validDGEList
 
 
 class test_utils(unittest.TestCase):
     def test_isAllZero(self):
         from inmoose.edgepy.utils import _isAllZero
 
         self.assertEqual(_isAllZero(np.array([])), False)
         self.assertEqual(_isAllZero(np.array([0, 0, 0])), True)
         self.assertEqual(_isAllZero(np.array([2, 1, 0])), False)
-        arr = np.array([np.NaN, 0, -1, np.PINF, 1, np.NINF])
         with self.assertRaisesRegex(
             ValueError, expected_regex="NaN counts are not allowed"
         ):
             _isAllZero(np.array([1, 2, 3, np.NaN, 4, 5]))
         with self.assertRaisesRegex(
             ValueError, expected_regex="infinite counts are not allowed"
         ):
@@ -90,10 +90,10 @@
     def test_validDGEList(self):
         d = DGEList([[42]])
         d.counts = None
         with self.assertRaisesRegex(RuntimeError, expected_regex="No count matrix"):
             validDGEList(d)
         d = DGEList([[42]])
         d = validDGEList(d)
-        self.assertFalse((d.samples.group.values == None).any())
-        self.assertFalse((d.samples.lib_size.values == None).any())
-        self.assertFalse((d.samples.norm_factors.values == None).any())
+        self.assertFalse((d.samples.group.values == None).any())  # noqa: E711
+        self.assertFalse((d.samples.lib_size.values == None).any())  # noqa: E711
+        self.assertFalse((d.samples.norm_factors.values == None).any())  # noqa: E711
```

### Comparing `inmoose-0.4.1/tests/edgepy/test_addPriorCount.py` & `inmoose-0.5.0/tests/edgepy/test_addPriorCount.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import unittest
+
 import numpy as np
 
-from inmoose.utils import rnbinom
 from inmoose.edgepy import addPriorCount
+from inmoose.utils import rnbinom
 
 
 class test_addPriorCount(unittest.TestCase):
     def setUp(self):
         y = np.array(rnbinom(80, size=5, mu=20, seed=42)).reshape((20, 4))
         self.y = np.vstack(([0, 0, 0, 0], [0, 0, 2, 2], y))
```

### Comparing `inmoose-0.4.1/tests/edgepy/test_aveLogCPM.py` & `inmoose-0.5.0/tests/edgepy/test_aveLogCPM.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import unittest
+
 import numpy as np
 
+from inmoose.edgepy import DGEList, aveLogCPM
 from inmoose.utils import rnbinom
-from inmoose.edgepy import aveLogCPM, DGEList
 
 
 class test_aveLogCPM(unittest.TestCase):
     def setUp(self):
         y = np.array(rnbinom(80, size=5, mu=20, seed=42)).reshape((20, 4))
         y = np.vstack(([0, 0, 0, 0], [0, 0, 2, 2], y))
         group = np.array([1, 1, 2, 2])
```

### Comparing `inmoose-0.4.1/tests/edgepy/test_compressMatrix.py` & `inmoose-0.5.0/tests/edgepy/test_compressMatrix.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import unittest
+
 import numpy as np
 
 from inmoose.edgepy.makeCompressedMatrix import makeCompressedMatrix
 
 
 class Test(unittest.TestCase):
     def test_makeCompressedMatrix(self):
```

### Comparing `inmoose-0.4.1/tests/edgepy/test_dispersion.py` & `inmoose-0.5.0/tests/edgepy/test_dispersion.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 import unittest
+
 import numpy as np
 
-from inmoose.utils import rnbinom
 from inmoose.edgepy import (
     DGEList,
     dispCoxReid,
     maximizeInterpolant,
     movingAverageByCol,
     systematicSubset,
 )
+from inmoose.utils import rnbinom
 
 
 class test_dispersion(unittest.TestCase):
     def setUp(self):
         y = np.array(rnbinom(80, size=5, mu=20, seed=42)).reshape((20, 4))
         y = np.vstack(([0, 0, 0, 0], [0, 0, 2, 2], y))
         self.group = np.array([1, 1, 2, 2])
```

### Comparing `inmoose-0.4.1/tests/edgepy/test_exactTest.py` & `inmoose-0.5.0/tests/edgepy/test_exactTest.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import unittest
+
 import numpy as np
 import pandas as pd
 
+from inmoose.edgepy import DGEList, binomTest, exactTest, exactTestBetaApprox, topTags
 from inmoose.utils import rnbinom
-from inmoose.edgepy import DGEList, exactTest, binomTest, exactTestBetaApprox, topTags
 
 
 class Test(unittest.TestCase):
     def setUp(self):
         y = np.array(rnbinom(80, size=5, mu=20, seed=42)).reshape((20, 4))
         y = np.vstack(([0, 0, 0, 0], [0, 0, 2, 2], y))
         self.group = np.array([1, 2, 2, 2])
```

### Comparing `inmoose-0.4.1/tests/edgepy/test_glm.py` & `inmoose-0.5.0/tests/edgepy/test_glm.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import unittest
+
 import numpy as np
 import pandas as pd
 
-from inmoose.utils import rnbinom
 from inmoose.edgepy import DGEList, glmFit, glmLRT, glmQLFTest
+from inmoose.utils import rnbinom
 
 
 class test_DGEGLM(unittest.TestCase):
     def test_constructor(self):
         from inmoose.edgepy import DGEGLM
 
         d = DGEGLM((1, 2, 3, 4, 5))
```

### Comparing `inmoose-0.4.1/tests/edgepy/test_lik.py` & `inmoose-0.5.0/tests/edgepy/test_lik.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import unittest
+
 import numpy as np
 
-from inmoose.utils import rnbinom
 from inmoose.edgepy import DGEList, adjustedProfileLik
+from inmoose.utils import rnbinom
 
 
 class test_APL(unittest.TestCase):
     def setUp(self):
         y = np.array(rnbinom(80, size=5, mu=20, seed=42)).reshape((20, 4))
         y = np.vstack(([0, 0, 0, 0], [0, 0, 2, 2], y))
         self.group = np.array([1, 1, 2, 2])
```

### Comparing `inmoose-0.4.1/tests/edgepy/test_mglm.py` & `inmoose-0.5.0/tests/edgepy/test_mglm.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import unittest
+
 import numpy as np
 
+from inmoose.edgepy import designAsFactor, mglmLevenberg, mglmOneGroup, mglmOneWay
 from inmoose.utils import Factor, rnbinom
-from inmoose.edgepy import mglmLevenberg, mglmOneGroup, mglmOneWay, designAsFactor
 
 
 class test_mglm(unittest.TestCase):
     def setUp(self):
         y = np.array(rnbinom(80, size=5, mu=20, seed=42)).reshape((20, 4))
         self.y = np.vstack(([0, 0, 0, 0], [0, 0, 2, 2], y))
         self.group = np.array([1, 1, 2, 2])
```

### Comparing `inmoose-0.4.1/tests/edgepy/test_nbinomDeviance.py` & `inmoose-0.5.0/tests/edgepy/test_nbinomDeviance.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import unittest
+
 import numpy as np
 
-from inmoose.utils import rnbinom
 from inmoose.edgepy import nbinomDeviance
+from inmoose.utils import rnbinom
 
 
 class test_nbinomDeviance(unittest.TestCase):
     def setUp(self):
         y = np.array(rnbinom(80, size=5, mu=20, seed=42)).reshape((20, 4))
         self.y = np.vstack(([0, 0, 0, 0], [0, 0, 2, 2], y))
```

### Comparing `inmoose-0.4.1/tests/edgepy/test_objects.py` & `inmoose-0.5.0/tests/edgepy/test_objects.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import unittest
+
 import numpy as np
 
 from inmoose.edgepy import is_integer_array
 
 
 class test_objects(unittest.TestCase):
     def test_is_integer(self):
```

### Comparing `inmoose-0.4.1/tests/edgepy/test_predFC.py` & `inmoose-0.5.0/tests/edgepy/test_predFC.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import unittest
+
 import numpy as np
 
-from inmoose.utils import rnbinom
 from inmoose.edgepy import DGEList
+from inmoose.utils import rnbinom
 
 
 class test_predFC(unittest.TestCase):
     def setUp(self):
         y = np.array(rnbinom(80, size=5, mu=20, seed=42)).reshape((20, 4))
         y = np.vstack(([0, 0, 0, 0], [0, 0, 2, 2], y))
         self.group = np.array([1, 1, 2, 2])
```

### Comparing `inmoose-0.4.1/tests/edgepy/test_q2qnbinom.py` & `inmoose-0.5.0/tests/edgepy/test_q2qnbinom.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import unittest
+
 import numpy as np
-from scipy.stats import nbinom
 
 from inmoose.edgepy import q2qnbinom
 
 
 class Test(unittest.TestCase):
     def test_q2qnbinom(self):
         x = np.arange(20, dtype=float)
```

### Comparing `inmoose-0.4.1/tests/edgepy/test_stats.py` & `inmoose-0.5.0/tests/edgepy/test_stats.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 import unittest
-import numpy as np
 
 from inmoose.edgepy import pnbinom, qnbinom
 
 
 class test_nbinom(unittest.TestCase):
     def test_nbinom(self):
         for i in range(10):
```

### Comparing `inmoose-0.4.1/tests/limma/test_squeezeVar.py` & `inmoose-0.5.0/tests/limma/test_squeezeVar.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import unittest
+
 import numpy as np
 
 from inmoose.limma import squeezeVar
 
 
 class Test(unittest.TestCase):
     def test_squeezeVar(self):
```

### Comparing `inmoose-0.4.1/tests/pycombat/test_covariates.py` & `inmoose-0.5.0/tests/pycombat/test_covariates.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import unittest
+
 import numpy as np
 import pandas as pd
 import patsy
 
-from inmoose.pycombat.covariates import make_design_matrix, VirtualCohortInput
+from inmoose.pycombat.covariates import VirtualCohortInput, make_design_matrix
 
 
 class Test(unittest.TestCase):
     def test_VirtualCohortInput(self):
         counts = np.ones((100, 5))
         batch = np.array([1, 1, 2, 2, 2])
```

### Comparing `inmoose-0.4.1/tests/pycombat/test_pycombat.py` & `inmoose-0.5.0/tests/pycombat/test_pycombat.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,23 +1,25 @@
 import unittest
+
 import numpy as np
 import pandas as pd
 
+from inmoose.pycombat import pycombat_norm
 from inmoose.pycombat.covariates import make_design_matrix
-from inmoose.pycombat.pycombat_norm import check_mean_only
 from inmoose.pycombat.pycombat_norm import (
+    adjust_data,
+    calculate_mean_var,
+    calculate_stand_mean,
+    check_mean_only,
     compute_prior,
+    fit_model,
     postmean,
     postvar,
-    it_sol,
-    int_eprior,
+    standardise_data,
 )
-from inmoose.pycombat.pycombat_norm import calculate_mean_var, calculate_stand_mean
-from inmoose.pycombat.pycombat_norm import standardise_data, fit_model, adjust_data
-from inmoose.pycombat import pycombat_norm
 
 
 class test_pycombat(unittest.TestCase):
     @classmethod
     def setUpClass(self):
         matrix = np.transpose(
             [
```

### Comparing `inmoose-0.4.1/tests/pycombat/test_pycombatseq.py` & `inmoose-0.5.0/tests/pycombat/test_pycombatseq.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import unittest
+
 import numpy as np
 import pandas as pd
 
-from inmoose.utils import rnbinom
 from inmoose.pycombat import pycombat_seq
+from inmoose.utils import rnbinom
 
 
 class test_pycombatseq(unittest.TestCase):
     def setUp(self):
         y = np.array(rnbinom(100, size=5, mu=20, seed=42)).reshape((20, 5))
         self.y = np.vstack(([0, 0, 0, 0, 0], [0, 0, 2, 2, 2], y))
         self.batch = np.array([1, 1, 2, 2, 2])
```

### Comparing `inmoose-0.4.1/tests/sim/test_splat.py` & `inmoose-0.5.0/tests/sim/test_splat.py`

 * *Files identical despite different names*

### Comparing `inmoose-0.4.1/tests/utils/test_factor.py` & `inmoose-0.5.0/tests/utils/test_factor.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import unittest
+
 import numpy as np
 
-from inmoose.utils import Factor, gl, asfactor
+from inmoose.utils import Factor, asfactor, gl
 
 
 class test_factor(unittest.TestCase):
     def test_class(self):
         f = Factor([1, 1, 2, 3, 3])
         self.assertTrue(np.array_equal(f.__array__(), [1, 1, 2, 3, 3]))
         self.assertTrue(np.array_equal(f.categories, [1, 2, 3]))
```

