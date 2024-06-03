# Comparing `tmp/pesummary-1.2.0.tar.gz` & `tmp/pesummary-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pesummary-1.2.0.tar", last modified: Tue Feb 20 10:33:37 2024, max compression
+gzip compressed data, was "pesummary-1.3.0.tar", last modified: Mon Jun  3 08:12:48 2024, max compression
```

## Comparing `pesummary-1.2.0.tar` & `pesummary-1.3.0.tar`

### file list

```diff
@@ -1,454 +1,457 @@
-drwxr-xr-x   0 charlie    (501) staff       (20)        0 2024-02-20 10:33:37.700918 pesummary-1.2.0/
--rw-r--r--   0 charlie    (501) staff       (20)      318 2022-09-20 20:30:50.000000 pesummary-1.2.0/.AUTHORS
--rw-r--r--   0 charlie    (501) staff       (20)      259 2023-10-23 08:41:49.000000 pesummary-1.2.0/.flake8
--rw-r--r--   0 charlie    (501) staff       (20)      119 2022-09-20 20:30:50.000000 pesummary-1.2.0/.gitattributes
--rw-r--r--   0 charlie    (501) staff       (20)      646 2022-09-20 20:30:50.000000 pesummary-1.2.0/.gitignore
--rw-r--r--   0 charlie    (501) staff       (20)    13823 2024-02-20 10:30:45.000000 pesummary-1.2.0/.gitlab-ci.yml
--rw-r--r--   0 charlie    (501) staff       (20)      123 2022-09-20 20:30:50.000000 pesummary-1.2.0/.pre-commit-config.yaml
--rw-r--r--   0 charlie    (501) staff       (20)      392 2024-02-20 10:30:45.000000 pesummary-1.2.0/.readthedocs.yml
--rw-r--r--   0 charlie    (501) staff       (20)    41646 2023-04-23 23:35:41.000000 pesummary-1.2.0/CHANGELOG.md
--rw-r--r--   0 charlie    (501) staff       (20)     4818 2022-09-20 20:30:50.000000 pesummary-1.2.0/CONTRIBUTING.md
--rw-r--r--   0 charlie    (501) staff       (20)     1116 2023-04-23 23:35:41.000000 pesummary-1.2.0/LICENSE.md
--rw-r--r--   0 charlie    (501) staff       (20)      308 2022-09-20 20:30:50.000000 pesummary-1.2.0/MANIFEST.in
--rw-r--r--   0 charlie    (501) staff       (20)     4517 2024-02-20 10:33:37.700649 pesummary-1.2.0/PKG-INFO
--rw-r--r--   0 charlie    (501) staff       (20)     1481 2022-09-20 20:30:50.000000 pesummary-1.2.0/README.md
-drwxr-xr-x   0 charlie    (501) staff       (20)        0 2024-02-20 10:33:37.610414 pesummary-1.2.0/containers/
--rw-r--r--   0 charlie    (501) staff       (20)      977 2022-09-20 20:30:50.000000 pesummary-1.2.0/containers/Dockerfile-template
--rw-r--r--   0 charlie    (501) staff       (20)     1231 2023-04-23 23:35:41.000000 pesummary-1.2.0/containers/write_dockerfile.py
-drwxr-xr-x   0 charlie    (501) staff       (20)        0 2024-02-20 10:33:37.612591 pesummary-1.2.0/docs/
--rw-r--r--   0 charlie    (501) staff       (20)       46 2022-09-20 20:30:50.000000 pesummary-1.2.0/docs/.gitattributes
--rw-r--r--   0 charlie    (501) staff       (20)     1633 2022-09-20 20:30:50.000000 pesummary-1.2.0/docs/citing_pesummary.rst
-drwxr-xr-x   0 charlie    (501) staff       (20)        0 2024-02-20 10:33:37.612840 pesummary-1.2.0/docs/conf/
--rw-r--r--   0 charlie    (501) staff       (20)      693 2023-04-23 23:35:45.000000 pesummary-1.2.0/docs/conf/configuration.rst
--rw-r--r--   0 charlie    (501) staff       (20)     9118 2023-04-23 23:35:45.000000 pesummary-1.2.0/docs/conf.py
-drwxr-xr-x   0 charlie    (501) staff       (20)        0 2024-02-20 10:33:37.615348 pesummary-1.2.0/docs/core/
--rw-r--r--   0 charlie    (501) staff       (20)     1339 2022-09-20 20:30:50.000000 pesummary-1.2.0/docs/core/Array.rst
--rw-r--r--   0 charlie    (501) staff       (20)     2686 2022-09-20 20:30:50.000000 pesummary-1.2.0/docs/core/MCMCSamplesDict.rst
--rw-r--r--   0 charlie    (501) staff       (20)     5211 2022-09-20 20:30:50.000000 pesummary-1.2.0/docs/core/MultiAnalysisSamplesDict.rst
--rw-r--r--   0 charlie    (501) staff       (20)      391 2022-09-20 20:30:50.000000 pesummary-1.2.0/docs/core/ProbabilityDict.rst
--rw-r--r--   0 charlie    (501) staff       (20)      395 2022-09-20 20:30:50.000000 pesummary-1.2.0/docs/core/ProbabilityDict2D.rst
--rw-r--r--   0 charlie    (501) staff       (20)     3906 2022-09-20 20:30:50.000000 pesummary-1.2.0/docs/core/SamplesDict.rst
--rw-r--r--   0 charlie    (501) staff       (20)     2993 2022-09-20 20:30:50.000000 pesummary-1.2.0/docs/core/bounded_kdes.rst
-drwxr-xr-x   0 charlie    (501) staff       (20)        0 2024-02-20 10:33:37.616999 pesummary-1.2.0/docs/core/cli/
--rw-r--r--   0 charlie    (501) staff       (20)      778 2022-09-20 20:30:50.000000 pesummary-1.2.0/docs/core/cli/summaryclean.rst
--rw-r--r--   0 charlie    (501) staff       (20)      636 2022-09-20 20:30:50.000000 pesummary-1.2.0/docs/core/cli/summarycombine.rst
--rw-r--r--   0 charlie    (501) staff       (20)      643 2022-09-20 20:30:50.000000 pesummary-1.2.0/docs/core/cli/summarycombine_posteriors.rst
--rw-r--r--   0 charlie    (501) staff       (20)    15166 2022-09-20 20:30:50.000000 pesummary-1.2.0/docs/core/cli/summarycompare.rst
--rw-r--r--   0 charlie    (501) staff       (20)      366 2022-09-20 20:30:50.000000 pesummary-1.2.0/docs/core/cli/summaryextract.rst
--rw-r--r--   0 charlie    (501) staff       (20)      351 2022-09-20 20:30:50.000000 pesummary-1.2.0/docs/core/cli/summarymodify.rst
--rw-r--r--   0 charlie    (501) staff       (20)     3312 2023-04-23 23:35:45.000000 pesummary-1.2.0/docs/core/cli/summarypages.rst
--rw-r--r--   0 charlie    (501) staff       (20)      529 2022-09-20 20:30:50.000000 pesummary-1.2.0/docs/core/cli/summarypageslw.rst
--rw-r--r--   0 charlie    (501) staff       (20)     2815 2023-04-23 23:35:45.000000 pesummary-1.2.0/docs/core/cli/summarypublication.rst
--rw-r--r--   0 charlie    (501) staff       (20)      451 2022-09-20 20:30:50.000000 pesummary-1.2.0/docs/core/cli/summarysplit.rst
--rw-r--r--   0 charlie    (501) staff       (20)      239 2022-09-20 20:30:50.000000 pesummary-1.2.0/docs/core/cli/summaryversion.rst
-drwxr-xr-x   0 charlie    (501) staff       (20)        0 2024-02-20 10:33:37.617457 pesummary-1.2.0/docs/core/examples/
--rw-r--r--   0 charlie    (501) staff       (20)      130 2022-09-20 20:30:50.000000 pesummary-1.2.0/docs/core/examples/bounded_kde.png
--rw-r--r--   0 charlie    (501) staff       (20)      130 2022-09-20 20:30:50.000000 pesummary-1.2.0/docs/core/examples/bounded_kde_uniform.png
--rw-r--r--   0 charlie    (501) staff       (20)      130 2022-09-20 20:30:50.000000 pesummary-1.2.0/docs/core/examples/bounded_kdeplot.png
--rw-r--r--   0 charlie    (501) staff       (20)     3564 2022-09-20 20:30:50.000000 pesummary-1.2.0/docs/core/file_formats.rst
--rw-r--r--   0 charlie    (501) staff       (20)     1225 2022-09-20 20:30:50.000000 pesummary-1.2.0/docs/core/index.rst
--rw-r--r--   0 charlie    (501) staff       (20)     1079 2022-09-20 20:30:50.000000 pesummary-1.2.0/docs/core/pdf.rst
--rw-r--r--   0 charlie    (501) staff       (20)     4858 2023-04-23 23:35:45.000000 pesummary-1.2.0/docs/core/pesummary_file.rst
--rw-r--r--   0 charlie    (501) staff       (20)     4791 2022-09-20 20:30:50.000000 pesummary-1.2.0/docs/core/read.rst
--rw-r--r--   0 charlie    (501) staff       (20)      411 2023-04-23 23:35:45.000000 pesummary-1.2.0/docs/core/seaborn.rst
-drwxr-xr-x   0 charlie    (501) staff       (20)        0 2024-02-20 10:33:37.617622 pesummary-1.2.0/docs/core/tutorials/
-drwxr-xr-x   0 charlie    (501) staff       (20)        0 2024-02-20 10:33:37.618764 pesummary-1.2.0/docs/core/tutorials/examples/
--rw-r--r--   0 charlie    (501) staff       (20)      130 2022-09-20 20:30:50.000000 pesummary-1.2.0/docs/core/tutorials/examples/Histogram.png
--rw-r--r--   0 charlie    (501) staff       (20)      130 2022-09-20 20:30:50.000000 pesummary-1.2.0/docs/core/tutorials/examples/MultiAnalysisCorner.png
--rw-r--r--   0 charlie    (501) staff       (20)      130 2022-09-20 20:30:50.000000 pesummary-1.2.0/docs/core/tutorials/examples/MultiAnalysisHistogram.png
--rw-r--r--   0 charlie    (501) staff       (20)      131 2022-09-20 20:30:50.000000 pesummary-1.2.0/docs/core/tutorials/examples/MultiAnalysisReverseTriangle.png
--rw-r--r--   0 charlie    (501) staff       (20)      131 2022-09-20 20:30:50.000000 pesummary-1.2.0/docs/core/tutorials/examples/MultiAnalysisTriangle.png
--rw-r--r--   0 charlie    (501) staff       (20)      130 2022-09-20 20:30:50.000000 pesummary-1.2.0/docs/core/tutorials/examples/violin.png
--rw-r--r--   0 charlie    (501) staff       (20)     2839 2022-09-20 20:30:50.000000 pesummary-1.2.0/docs/core/tutorials/plotting_from_metafile.rst
--rw-r--r--   0 charlie    (501) staff       (20)     1746 2023-04-23 23:35:45.000000 pesummary-1.2.0/docs/core/write.rst
--rw-r--r--   0 charlie    (501) staff       (20)     1974 2024-02-20 10:30:45.000000 pesummary-1.2.0/docs/front.html.in
-drwxr-xr-x   0 charlie    (501) staff       (20)        0 2024-02-20 10:33:37.621796 pesummary-1.2.0/docs/gw/
--rw-r--r--   0 charlie    (501) staff       (20)     3666 2022-09-20 20:30:50.000000 pesummary-1.2.0/docs/gw/Conversion.rst
--rw-r--r--   0 charlie    (501) staff       (20)     1929 2023-04-23 23:35:45.000000 pesummary-1.2.0/docs/gw/SamplesDict.rst
--rw-r--r--   0 charlie    (501) staff       (20)     3249 2023-04-23 23:35:45.000000 pesummary-1.2.0/docs/gw/calibration.rst
--rw-r--r--   0 charlie    (501) staff       (20)     5891 2023-04-23 23:35:45.000000 pesummary-1.2.0/docs/gw/classification.rst
-drwxr-xr-x   0 charlie    (501) staff       (20)        0 2024-02-20 10:33:37.623526 pesummary-1.2.0/docs/gw/cli/
--rw-r--r--   0 charlie    (501) staff       (20)      186 2022-09-20 20:30:50.000000 pesummary-1.2.0/docs/gw/cli/executable_descriptions.rst
--rw-r--r--   0 charlie    (501) staff       (20)     1353 2022-09-20 20:30:50.000000 pesummary-1.2.0/docs/gw/cli/summaryclassification.rst
--rw-r--r--   0 charlie    (501) staff       (20)     1996 2022-09-20 20:30:50.000000 pesummary-1.2.0/docs/gw/cli/summarydetchar.rst
--rw-r--r--   0 charlie    (501) staff       (20)      616 2022-09-20 20:30:50.000000 pesummary-1.2.0/docs/gw/cli/summarygracedb.rst
--rw-r--r--   0 charlie    (501) staff       (20)      566 2022-09-20 20:30:50.000000 pesummary-1.2.0/docs/gw/cli/summarypipe.rst
--rw-r--r--   0 charlie    (501) staff       (20)     1433 2022-09-20 20:30:50.000000 pesummary-1.2.0/docs/gw/cli/summaryrecreate.rst
--rw-r--r--   0 charlie    (501) staff       (20)      682 2022-09-20 20:30:50.000000 pesummary-1.2.0/docs/gw/cli/summaryreview.rst
--rw-r--r--   0 charlie    (501) staff       (20)     2637 2022-09-20 20:30:50.000000 pesummary-1.2.0/docs/gw/cli/summarytgr.rst
-drwxr-xr-x   0 charlie    (501) staff       (20)        0 2024-02-20 10:33:37.624248 pesummary-1.2.0/docs/gw/examples/
--rw-r--r--   0 charlie    (501) staff       (20)      130 2022-09-20 20:30:50.000000 pesummary-1.2.0/docs/gw/examples/GW190412_violin.png
--rw-r--r--   0 charlie    (501) staff       (20)      130 2022-09-20 20:30:50.000000 pesummary-1.2.0/docs/gw/examples/bounded_violin.png
--rw-r--r--   0 charlie    (501) staff       (20)      130 2022-09-20 20:30:50.000000 pesummary-1.2.0/docs/gw/examples/gaussian_violin.png
--rw-r--r--   0 charlie    (501) staff       (20)      130 2022-09-20 20:30:50.000000 pesummary-1.2.0/docs/gw/examples/split_violin.png
--rw-r--r--   0 charlie    (501) staff       (20)     1317 2023-04-23 23:35:45.000000 pesummary-1.2.0/docs/gw/fetch.rst
--rw-r--r--   0 charlie    (501) staff       (20)     1674 2023-04-23 23:35:45.000000 pesummary-1.2.0/docs/gw/file_formats.rst
--rw-r--r--   0 charlie    (501) staff       (20)     3319 2022-09-20 20:30:50.000000 pesummary-1.2.0/docs/gw/index.rst
--rw-r--r--   0 charlie    (501) staff       (20)      238 2022-09-20 20:30:50.000000 pesummary-1.2.0/docs/gw/parameters.rst
--rw-r--r--   0 charlie    (501) staff       (20)     3462 2023-04-23 23:35:45.000000 pesummary-1.2.0/docs/gw/pesummary_file.rst
--rw-r--r--   0 charlie    (501) staff       (20)     2948 2022-09-20 20:30:50.000000 pesummary-1.2.0/docs/gw/psd.rst
--rw-r--r--   0 charlie    (501) staff       (20)     1791 2022-09-20 20:30:50.000000 pesummary-1.2.0/docs/gw/read.rst
--rw-r--r--   0 charlie    (501) staff       (20)     4759 2022-09-20 20:30:50.000000 pesummary-1.2.0/docs/gw/remnant_fits.rst
--rw-r--r--   0 charlie    (501) staff       (20)     2595 2022-09-20 20:30:50.000000 pesummary-1.2.0/docs/gw/strain.rst
-drwxr-xr-x   0 charlie    (501) staff       (20)        0 2024-02-20 10:33:37.626171 pesummary-1.2.0/docs/gw/summarypages/
-drwxr-xr-x   0 charlie    (501) staff       (20)        0 2024-02-20 10:33:37.627001 pesummary-1.2.0/docs/gw/summarypages/IMRPhenomPv3HM/
--rw-r--r--   0 charlie    (501) staff       (20)      692 2022-09-20 20:30:50.000000 pesummary-1.2.0/docs/gw/summarypages/IMRPhenomPv3HM/classification.rst
--rw-r--r--   0 charlie    (501) staff       (20)     1128 2022-09-20 20:30:50.000000 pesummary-1.2.0/docs/gw/summarypages/IMRPhenomPv3HM/corner.rst
-drwxr-xr-x   0 charlie    (501) staff       (20)        0 2024-02-20 10:33:37.627419 pesummary-1.2.0/docs/gw/summarypages/IMRPhenomPv3HM/examples/
--rw-r--r--   0 charlie    (501) staff       (20)      966 2022-09-20 20:30:50.000000 pesummary-1.2.0/docs/gw/summarypages/IMRPhenomPv3HM/examples/.gitattributes
--rw-r--r--   0 charlie    (501) staff       (20)      132 2022-09-20 20:30:50.000000 pesummary-1.2.0/docs/gw/summarypages/IMRPhenomPv3HM/examples/corner.mp4
--rw-r--r--   0 charlie    (501) staff       (20)      132 2022-09-20 20:30:50.000000 pesummary-1.2.0/docs/gw/summarypages/IMRPhenomPv3HM/examples/interactive_corner_source.html
--rw-r--r--   0 charlie    (501) staff       (20)      646 2022-09-20 20:30:50.000000 pesummary-1.2.0/docs/gw/summarypages/IMRPhenomPv3HM/home.rst
--rw-r--r--   0 charlie    (501) staff       (20)      976 2022-09-20 20:30:50.000000 pesummary-1.2.0/docs/gw/summarypages/IMRPhenomPv3HM/interactive.rst
--rw-r--r--   0 charlie    (501) staff       (20)     1785 2022-09-20 20:30:50.000000 pesummary-1.2.0/docs/gw/summarypages/IMRPhenomPv3HM/mass_1.rst
--rw-r--r--   0 charlie    (501) staff       (20)      391 2022-09-20 20:30:50.000000 pesummary-1.2.0/docs/gw/summarypages/about.rst
-drwxr-xr-x   0 charlie    (501) staff       (20)        0 2024-02-20 10:33:37.627988 pesummary-1.2.0/docs/gw/summarypages/comparison/
-drwxr-xr-x   0 charlie    (501) staff       (20)        0 2024-02-20 10:33:37.628142 pesummary-1.2.0/docs/gw/summarypages/comparison/examples/
--rw-r--r--   0 charlie    (501) staff       (20)   639556 2022-09-20 20:30:50.000000 pesummary-1.2.0/docs/gw/summarypages/comparison/examples/interactive_ridgeline.html
--rw-r--r--   0 charlie    (501) staff       (20)      615 2022-09-20 20:30:50.000000 pesummary-1.2.0/docs/gw/summarypages/comparison/home.rst
--rw-r--r--   0 charlie    (501) staff       (20)      912 2022-09-20 20:30:50.000000 pesummary-1.2.0/docs/gw/summarypages/comparison/interactive.rst
--rw-r--r--   0 charlie    (501) staff       (20)     2030 2022-09-20 20:30:50.000000 pesummary-1.2.0/docs/gw/summarypages/comparison/mass_1.rst
--rw-r--r--   0 charlie    (501) staff       (20)      549 2022-09-20 20:30:50.000000 pesummary-1.2.0/docs/gw/summarypages/downloads.rst
-drwxr-xr-x   0 charlie    (501) staff       (20)        0 2024-02-20 10:33:37.629587 pesummary-1.2.0/docs/gw/summarypages/examples/
--rw-r--r--   0 charlie    (501) staff       (20)      131 2022-09-20 20:30:50.000000 pesummary-1.2.0/docs/gw/summarypages/examples/watermark.png
--rw-r--r--   0 charlie    (501) staff       (20)      980 2022-09-20 20:30:50.000000 pesummary-1.2.0/docs/gw/summarypages/home.rst
--rw-r--r--   0 charlie    (501) staff       (20)      356 2022-09-20 20:30:50.000000 pesummary-1.2.0/docs/gw/summarypages/logging.rst
--rw-r--r--   0 charlie    (501) staff       (20)      504 2022-09-20 20:30:50.000000 pesummary-1.2.0/docs/gw/summarypages/publication.rst
--rw-r--r--   0 charlie    (501) staff       (20)     1166 2022-09-20 20:30:50.000000 pesummary-1.2.0/docs/gw/summarypages/version.rst
--rw-r--r--   0 charlie    (501) staff       (20)      502 2022-09-20 20:30:50.000000 pesummary-1.2.0/docs/gw/summarypages/watermark.rst
--rw-r--r--   0 charlie    (501) staff       (20)     4038 2022-09-20 20:30:50.000000 pesummary-1.2.0/docs/gw/tgr_file.rst
-drwxr-xr-x   0 charlie    (501) staff       (20)        0 2024-02-20 10:33:37.631359 pesummary-1.2.0/docs/gw/tutorials/
--rw-r--r--   0 charlie    (501) staff       (20)     1707 2023-04-23 23:35:45.000000 pesummary-1.2.0/docs/gw/tutorials/GWTC1_plots.rst
--rw-r--r--   0 charlie    (501) staff       (20)      967 2023-04-23 23:35:45.000000 pesummary-1.2.0/docs/gw/tutorials/comparing_public_data_files.rst
--rw-r--r--   0 charlie    (501) staff       (20)     9519 2022-09-20 20:30:50.000000 pesummary-1.2.0/docs/gw/tutorials/conversions_and_condor.rst
-drwxr-xr-x   0 charlie    (501) staff       (20)        0 2024-02-20 10:33:37.634171 pesummary-1.2.0/docs/gw/tutorials/examples/
--rw-r--r--   0 charlie    (501) staff       (20)      528 2022-09-20 20:30:50.000000 pesummary-1.2.0/docs/gw/tutorials/examples/.gitattributes
--rw-r--r--   0 charlie    (501) staff       (20)      130 2022-09-20 20:30:50.000000 pesummary-1.2.0/docs/gw/tutorials/examples/2d_contour_plot_luminosity_distance_and_chirp_mass.png
--rw-r--r--   0 charlie    (501) staff       (20)      130 2022-09-20 20:30:50.000000 pesummary-1.2.0/docs/gw/tutorials/examples/2d_contour_plot_mass_1_and_mass_2.png
--rw-r--r--   0 charlie    (501) staff       (20)      130 2022-09-20 20:30:50.000000 pesummary-1.2.0/docs/gw/tutorials/examples/2d_contour_plot_theta_jn_and_luminosity_distance.png
--rw-r--r--   0 charlie    (501) staff       (20)      131 2022-09-20 20:30:50.000000 pesummary-1.2.0/docs/gw/tutorials/examples/GW150914.png
--rw-r--r--   0 charlie    (501) staff       (20)      131 2022-09-20 20:30:50.000000 pesummary-1.2.0/docs/gw/tutorials/examples/GW190814.png
--rw-r--r--   0 charlie    (501) staff       (20)      130 2022-09-20 20:30:50.000000 pesummary-1.2.0/docs/gw/tutorials/examples/Histogram.png
--rw-r--r--   0 charlie    (501) staff       (20)      131 2022-09-20 20:30:50.000000 pesummary-1.2.0/docs/gw/tutorials/examples/MultiAnalysisCorner.png
--rw-r--r--   0 charlie    (501) staff       (20)      130 2022-09-20 20:30:50.000000 pesummary-1.2.0/docs/gw/tutorials/examples/MultiAnalysisHistogram.png
--rw-r--r--   0 charlie    (501) staff       (20)      131 2022-09-20 20:30:50.000000 pesummary-1.2.0/docs/gw/tutorials/examples/MultiAnalysisReverseTriangle.png
--rw-r--r--   0 charlie    (501) staff       (20)      131 2022-09-20 20:30:50.000000 pesummary-1.2.0/docs/gw/tutorials/examples/MultiAnalysisTriangle.png
--rw-r--r--   0 charlie    (501) staff       (20)      130 2022-09-20 20:30:50.000000 pesummary-1.2.0/docs/gw/tutorials/examples/PSD.png
--rw-r--r--   0 charlie    (501) staff       (20)      131 2022-09-20 20:30:50.000000 pesummary-1.2.0/docs/gw/tutorials/examples/comparison_for_GW150914.png
--rw-r--r--   0 charlie    (501) staff       (20)      130 2022-09-20 20:30:50.000000 pesummary-1.2.0/docs/gw/tutorials/examples/event_scatter_plot_total_mass_and_redshift.png
--rw-r--r--   0 charlie    (501) staff       (20)      130 2022-09-20 20:30:50.000000 pesummary-1.2.0/docs/gw/tutorials/examples/spin_disk.png
--rw-r--r--   0 charlie    (501) staff       (20)      130 2022-09-20 20:30:50.000000 pesummary-1.2.0/docs/gw/tutorials/examples/uncertainty_waveform_td.png
--rw-r--r--   0 charlie    (501) staff       (20)      130 2022-09-20 20:30:50.000000 pesummary-1.2.0/docs/gw/tutorials/examples/violin.png
--rw-r--r--   0 charlie    (501) staff       (20)      130 2022-09-20 20:30:50.000000 pesummary-1.2.0/docs/gw/tutorials/examples/violin_plot_mass_ratio.png
--rw-r--r--   0 charlie    (501) staff       (20)      130 2022-09-20 20:30:50.000000 pesummary-1.2.0/docs/gw/tutorials/examples/waveform_fd.png
--rw-r--r--   0 charlie    (501) staff       (20)      130 2022-09-20 20:30:50.000000 pesummary-1.2.0/docs/gw/tutorials/examples/waveform_td.png
--rw-r--r--   0 charlie    (501) staff       (20)     3997 2023-04-23 23:35:45.000000 pesummary-1.2.0/docs/gw/tutorials/interaction_with_ligo_skymap.rst
--rw-r--r--   0 charlie    (501) staff       (20)      801 2022-09-20 20:30:50.000000 pesummary-1.2.0/docs/gw/tutorials/make_your_own_page_from_metafile.rst
--rw-r--r--   0 charlie    (501) staff       (20)      811 2023-04-23 23:35:45.000000 pesummary-1.2.0/docs/gw/tutorials/plot_waveform_on_strain_data.rst
--rw-r--r--   0 charlie    (501) staff       (20)     3473 2022-09-20 20:30:50.000000 pesummary-1.2.0/docs/gw/tutorials/plotting_from_metafile.rst
--rw-r--r--   0 charlie    (501) staff       (20)      709 2023-04-23 23:35:45.000000 pesummary-1.2.0/docs/gw/tutorials/population_scatter_plot_GWTC-1.rst
--rw-r--r--   0 charlie    (501) staff       (20)      814 2022-09-20 20:30:50.000000 pesummary-1.2.0/docs/gw/tutorials/public_pages.rst
--rw-r--r--   0 charlie    (501) staff       (20)      690 2023-04-23 23:35:45.000000 pesummary-1.2.0/docs/gw/tutorials/release_notebook.rst
--rw-r--r--   0 charlie    (501) staff       (20)     1614 2023-04-23 23:35:45.000000 pesummary-1.2.0/docs/gw/tutorials/waveforms.rst
--rw-r--r--   0 charlie    (501) staff       (20)     4667 2022-09-20 20:30:50.000000 pesummary-1.2.0/docs/gw/violin.rst
--rw-r--r--   0 charlie    (501) staff       (20)     1891 2023-04-23 23:35:45.000000 pesummary-1.2.0/docs/index.rst
--rw-r--r--   0 charlie    (501) staff       (20)     2845 2023-04-23 23:35:41.000000 pesummary-1.2.0/docs/installation.rst
-drwxr-xr-x   0 charlie    (501) staff       (20)        0 2024-02-20 10:33:37.634298 pesummary-1.2.0/docs/io/
--rw-r--r--   0 charlie    (501) staff       (20)     3014 2023-04-23 23:35:45.000000 pesummary-1.2.0/docs/io/read.rst
--rw-r--r--   0 charlie    (501) staff       (20)      284 2024-02-20 10:30:45.000000 pesummary-1.2.0/docs/rtd-environment.yml
--rw-r--r--   0 charlie    (501) staff       (20)     2351 2022-09-20 20:30:50.000000 pesummary-1.2.0/docs/virtual_environment.rst
--rw-r--r--   0 charlie    (501) staff       (20)     2209 2022-09-20 20:30:50.000000 pesummary-1.2.0/docs/what_is_pesummary.rst
-drwxr-xr-x   0 charlie    (501) staff       (20)        0 2024-02-20 10:33:37.635028 pesummary-1.2.0/examples/
-drwxr-xr-x   0 charlie    (501) staff       (20)        0 2024-02-20 10:33:37.635701 pesummary-1.2.0/examples/core/
--rw-r--r--   0 charlie    (501) staff       (20)     1127 2022-09-20 20:30:50.000000 pesummary-1.2.0/examples/core/bounded_kdeplot.py
--rw-r--r--   0 charlie    (501) staff       (20)     1002 2022-09-20 20:30:50.000000 pesummary-1.2.0/examples/core/extract_information_from_pesummary_file.py
--rw-r--r--   0 charlie    (501) staff       (20)     3120 2022-09-20 20:30:50.000000 pesummary-1.2.0/examples/core/multiple_analysis_custom_read.py
--rw-r--r--   0 charlie    (501) staff       (20)     1490 2022-09-20 20:30:50.000000 pesummary-1.2.0/examples/core/pesummary_data_structure.txt
--rw-r--r--   0 charlie    (501) staff       (20)     2495 2022-09-20 20:30:50.000000 pesummary-1.2.0/examples/core/single_analysis_custom_read.py
--rw-r--r--   0 charlie    (501) staff       (20)     1711 2022-09-20 20:30:50.000000 pesummary-1.2.0/examples/custom_plot.py
--rw-r--r--   0 charlie    (501) staff       (20)     2174 2023-04-23 23:35:41.000000 pesummary-1.2.0/examples/extract_information_without_pesummary.py
-drwxr-xr-x   0 charlie    (501) staff       (20)        0 2024-02-20 10:33:37.638121 pesummary-1.2.0/examples/gw/
--rw-r--r--   0 charlie    (501) staff       (20)     1097 2022-09-20 20:30:50.000000 pesummary-1.2.0/examples/gw/GWTC-1_population_scatterplot.sh
--rw-r--r--   0 charlie    (501) staff       (20)     2624 2022-09-20 20:30:50.000000 pesummary-1.2.0/examples/gw/GWTC1_plots.sh
--rw-r--r--   0 charlie    (501) staff       (20)     1599 2022-09-20 20:30:50.000000 pesummary-1.2.0/examples/gw/compare_GW150914.py
--rw-r--r--   0 charlie    (501) staff       (20)      941 2022-09-20 20:30:50.000000 pesummary-1.2.0/examples/gw/extract_information_from_pesummary_file.py
--rw-r--r--   0 charlie    (501) staff       (20)     2709 2023-04-23 23:35:41.000000 pesummary-1.2.0/examples/gw/extract_information_from_pesummary_file_without_pesummary.py
--rw-r--r--   0 charlie    (501) staff       (20)      895 2022-09-20 20:30:50.000000 pesummary-1.2.0/examples/gw/fetch_open_data.py
--rw-r--r--   0 charlie    (501) staff       (20)      681 2023-04-23 23:35:41.000000 pesummary-1.2.0/examples/gw/fetch_open_strain.py
--rw-r--r--   0 charlie    (501) staff       (20)     1699 2022-09-20 20:30:50.000000 pesummary-1.2.0/examples/gw/latex.py
--rw-r--r--   0 charlie    (501) staff       (20)     1351 2023-04-23 23:35:41.000000 pesummary-1.2.0/examples/gw/ligo_skymap.py
--rwxr-xr-x   0 charlie    (501) staff       (20)      523 2022-09-20 20:30:50.000000 pesummary-1.2.0/examples/gw/make_public_release.py
--rw-r--r--   0 charlie    (501) staff       (20)     1390 2023-04-23 23:35:41.000000 pesummary-1.2.0/examples/gw/making_a_waveform_in_frequency_domain.py
--rw-r--r--   0 charlie    (501) staff       (20)     1281 2023-04-23 23:35:41.000000 pesummary-1.2.0/examples/gw/making_a_waveform_in_time_domain.py
--rw-r--r--   0 charlie    (501) staff       (20)      748 2023-04-23 23:35:41.000000 pesummary-1.2.0/examples/gw/making_a_waveform_in_time_domain_with_uncertainty.py
--rw-r--r--   0 charlie    (501) staff       (20)     2690 2022-09-20 20:30:50.000000 pesummary-1.2.0/examples/gw/pesummary_data_structure.txt
--rw-r--r--   0 charlie    (501) staff       (20)     1034 2022-09-20 20:30:50.000000 pesummary-1.2.0/examples/gw/plot_waveform_on_strain_data_GW150914.py
--rw-r--r--   0 charlie    (501) staff       (20)      775 2023-04-23 23:35:41.000000 pesummary-1.2.0/examples/gw/plot_waveform_on_strain_data_GW190814.py
--rw-r--r--   0 charlie    (501) staff       (20)     1641 2022-09-20 20:30:50.000000 pesummary-1.2.0/examples/gw/prior_conditioning.py
--rw-r--r--   0 charlie    (501) staff       (20)     1504 2023-04-23 23:35:41.000000 pesummary-1.2.0/examples/gw/violin_plots.py
--rw-r--r--   0 charlie    (501) staff       (20)      108 2022-09-20 20:30:50.000000 pesummary-1.2.0/examples/pesummary_core.ini
--rw-r--r--   0 charlie    (501) staff       (20)      282 2022-09-20 20:30:50.000000 pesummary-1.2.0/examples/pesummary_gw.ini
--rw-r--r--   0 charlie    (501) staff       (20)     1431 2023-04-23 23:35:41.000000 pesummary-1.2.0/examples/run_with_python.py
-drwxr-xr-x   0 charlie    (501) staff       (20)        0 2024-02-20 10:33:37.638695 pesummary-1.2.0/pesummary/
--rw-r--r--   0 charlie    (501) staff       (20)      309 2024-02-20 10:33:37.000000 pesummary-1.2.0/pesummary/.version
--rw-r--r--   0 charlie    (501) staff       (20)     1997 2022-09-20 20:30:50.000000 pesummary-1.2.0/pesummary/__init__.py
--rw-r--r--   0 charlie    (501) staff       (20)      411 2024-02-20 10:33:37.000000 pesummary-1.2.0/pesummary/_version.py
--rw-r--r--   0 charlie    (501) staff       (20)     5674 2022-09-20 20:30:50.000000 pesummary-1.2.0/pesummary/_version_helper.py
-drwxr-xr-x   0 charlie    (501) staff       (20)        0 2024-02-20 10:33:37.644448 pesummary-1.2.0/pesummary/cli/
--rw-r--r--   0 charlie    (501) staff       (20)       52 2022-09-20 20:30:50.000000 pesummary-1.2.0/pesummary/cli/__init__.py
--rw-r--r--   0 charlie    (501) staff       (20)     7587 2023-11-03 18:40:04.000000 pesummary-1.2.0/pesummary/cli/summaryclassification.py
--rw-r--r--   0 charlie    (501) staff       (20)     2508 2023-04-23 23:35:41.000000 pesummary-1.2.0/pesummary/cli/summaryclean.py
--rw-r--r--   0 charlie    (501) staff       (20)     1257 2023-04-23 23:35:41.000000 pesummary-1.2.0/pesummary/cli/summarycombine.py
--rw-r--r--   0 charlie    (501) staff       (20)     8223 2023-04-23 23:35:41.000000 pesummary-1.2.0/pesummary/cli/summarycombine_posteriors.py
--rw-r--r--   0 charlie    (501) staff       (20)    11646 2023-04-23 23:35:41.000000 pesummary-1.2.0/pesummary/cli/summarycompare.py
--rw-r--r--   0 charlie    (501) staff       (20)     3778 2023-04-23 23:35:41.000000 pesummary-1.2.0/pesummary/cli/summarydetchar.py
--rw-r--r--   0 charlie    (501) staff       (20)     2563 2023-04-23 23:35:41.000000 pesummary-1.2.0/pesummary/cli/summaryextract.py
--rw-r--r--   0 charlie    (501) staff       (20)     1434 2023-04-23 23:35:41.000000 pesummary-1.2.0/pesummary/cli/summarygracedb.py
--rw-r--r--   0 charlie    (501) staff       (20)     9659 2024-01-15 16:41:54.000000 pesummary-1.2.0/pesummary/cli/summaryjscompare.py
--rw-r--r--   0 charlie    (501) staff       (20)    24057 2023-04-23 23:35:41.000000 pesummary-1.2.0/pesummary/cli/summarymodify.py
--rw-r--r--   0 charlie    (501) staff       (20)    10894 2023-04-23 23:35:41.000000 pesummary-1.2.0/pesummary/cli/summarypages.py
--rw-r--r--   0 charlie    (501) staff       (20)     4097 2023-04-23 23:35:41.000000 pesummary-1.2.0/pesummary/cli/summarypageslw.py
--rw-r--r--   0 charlie    (501) staff       (20)    31078 2023-04-23 23:35:41.000000 pesummary-1.2.0/pesummary/cli/summarypipe.py
--rw-r--r--   0 charlie    (501) staff       (20)    13579 2024-01-15 16:41:54.000000 pesummary-1.2.0/pesummary/cli/summaryplots.py
--rw-r--r--   0 charlie    (501) staff       (20)    13547 2023-04-23 23:35:41.000000 pesummary-1.2.0/pesummary/cli/summarypublication.py
--rw-r--r--   0 charlie    (501) staff       (20)    10990 2023-04-23 23:35:41.000000 pesummary-1.2.0/pesummary/cli/summaryrecreate.py
--rw-r--r--   0 charlie    (501) staff       (20)    31084 2023-11-03 18:40:04.000000 pesummary-1.2.0/pesummary/cli/summaryreview.py
--rw-r--r--   0 charlie    (501) staff       (20)     6758 2023-04-23 23:35:41.000000 pesummary-1.2.0/pesummary/cli/summarysplit.py
--rw-r--r--   0 charlie    (501) staff       (20)    15650 2024-02-20 10:30:45.000000 pesummary-1.2.0/pesummary/cli/summarytest.py
--rw-r--r--   0 charlie    (501) staff       (20)     9472 2023-04-23 23:35:41.000000 pesummary-1.2.0/pesummary/cli/summarytgr.py
--rw-r--r--   0 charlie    (501) staff       (20)      386 2022-09-20 20:30:50.000000 pesummary-1.2.0/pesummary/cli/summaryversion.py
-drwxr-xr-x   0 charlie    (501) staff       (20)        0 2024-02-20 10:33:37.645281 pesummary-1.2.0/pesummary/conf/
--rw-r--r--   0 charlie    (501) staff       (20)       52 2022-09-20 20:30:50.000000 pesummary-1.2.0/pesummary/conf/__init__.py
--rw-r--r--   0 charlie    (501) staff       (20)     5198 2022-09-20 20:30:50.000000 pesummary-1.2.0/pesummary/conf/caption.py
--rw-r--r--   0 charlie    (501) staff       (20)     4489 2024-01-15 16:41:54.000000 pesummary-1.2.0/pesummary/conf/configuration.py
--rw-r--r--   0 charlie    (501) staff       (20)      422 2022-09-20 20:30:50.000000 pesummary-1.2.0/pesummary/conf/matplotlib_rcparams.sty
-drwxr-xr-x   0 charlie    (501) staff       (20)        0 2024-02-20 10:33:37.646022 pesummary-1.2.0/pesummary/core/
--rw-r--r--   0 charlie    (501) staff       (20)      109 2022-09-20 20:30:50.000000 pesummary-1.2.0/pesummary/core/__init__.py
-drwxr-xr-x   0 charlie    (501) staff       (20)        0 2024-02-20 10:33:37.647230 pesummary-1.2.0/pesummary/core/cli/
--rw-r--r--   0 charlie    (501) staff       (20)      109 2023-04-23 23:35:41.000000 pesummary-1.2.0/pesummary/core/cli/__init__.py
--rw-r--r--   0 charlie    (501) staff       (20)    10430 2023-04-23 23:35:41.000000 pesummary-1.2.0/pesummary/core/cli/actions.py
--rw-r--r--   0 charlie    (501) staff       (20)    83837 2024-01-15 16:41:54.000000 pesummary-1.2.0/pesummary/core/cli/inputs.py
--rw-r--r--   0 charlie    (501) staff       (20)    25359 2024-02-20 10:30:45.000000 pesummary-1.2.0/pesummary/core/cli/parser.py
-drwxr-xr-x   0 charlie    (501) staff       (20)        0 2024-02-20 10:33:37.648627 pesummary-1.2.0/pesummary/core/css/
--rw-r--r--   0 charlie    (501) staff       (20)      109 2022-09-20 20:30:50.000000 pesummary-1.2.0/pesummary/core/css/__init__.py
--rw-r--r--   0 charlie    (501) staff       (20)      178 2022-09-20 20:30:50.000000 pesummary-1.2.0/pesummary/core/css/font.css
--rw-r--r--   0 charlie    (501) staff       (20)     1601 2022-09-20 20:30:50.000000 pesummary-1.2.0/pesummary/core/css/image_styles.css
--rw-r--r--   0 charlie    (501) staff       (20)     1137 2022-09-20 20:30:50.000000 pesummary-1.2.0/pesummary/core/css/navbar.css
--rw-r--r--   0 charlie    (501) staff       (20)     1806 2022-09-20 20:30:50.000000 pesummary-1.2.0/pesummary/core/css/side_bar.css
--rw-r--r--   0 charlie    (501) staff       (20)      612 2022-09-20 20:30:50.000000 pesummary-1.2.0/pesummary/core/css/table.css
--rw-r--r--   0 charlie    (501) staff       (20)      879 2022-09-20 20:30:50.000000 pesummary-1.2.0/pesummary/core/css/toggle.css
--rw-r--r--   0 charlie    (501) staff       (20)      411 2022-09-20 20:30:50.000000 pesummary-1.2.0/pesummary/core/css/watermark.css
--rw-r--r--   0 charlie    (501) staff       (20)     6364 2024-02-20 10:30:45.000000 pesummary-1.2.0/pesummary/core/fetch.py
-drwxr-xr-x   0 charlie    (501) staff       (20)        0 2024-02-20 10:33:37.649696 pesummary-1.2.0/pesummary/core/file/
--rw-r--r--   0 charlie    (501) staff       (20)      109 2022-09-20 20:30:50.000000 pesummary-1.2.0/pesummary/core/file/__init__.py
-drwxr-xr-x   0 charlie    (501) staff       (20)        0 2024-02-20 10:33:37.652675 pesummary-1.2.0/pesummary/core/file/formats/
--rw-r--r--   0 charlie    (501) staff       (20)      109 2022-09-20 20:30:50.000000 pesummary-1.2.0/pesummary/core/file/formats/__init__.py
--rw-r--r--   0 charlie    (501) staff       (20)    39412 2024-02-20 10:30:45.000000 pesummary-1.2.0/pesummary/core/file/formats/base_read.py
--rw-r--r--   0 charlie    (501) staff       (20)    16259 2024-01-15 16:41:54.000000 pesummary-1.2.0/pesummary/core/file/formats/bilby.py
--rw-r--r--   0 charlie    (501) staff       (20)     2252 2022-09-20 20:30:50.000000 pesummary-1.2.0/pesummary/core/file/formats/csv.py
--rw-r--r--   0 charlie    (501) staff       (20)     2717 2023-04-23 23:35:41.000000 pesummary-1.2.0/pesummary/core/file/formats/dat.py
--rw-r--r--   0 charlie    (501) staff       (20)    10261 2023-04-23 23:35:41.000000 pesummary-1.2.0/pesummary/core/file/formats/default.py
--rw-r--r--   0 charlie    (501) staff       (20)     7086 2023-04-23 23:35:41.000000 pesummary-1.2.0/pesummary/core/file/formats/hdf5.py
--rw-r--r--   0 charlie    (501) staff       (20)     3282 2023-04-23 23:35:41.000000 pesummary-1.2.0/pesummary/core/file/formats/ini.py
--rw-r--r--   0 charlie    (501) staff       (20)     6841 2023-04-23 23:35:41.000000 pesummary-1.2.0/pesummary/core/file/formats/json.py
--rw-r--r--   0 charlie    (501) staff       (20)     3776 2022-09-20 20:30:50.000000 pesummary-1.2.0/pesummary/core/file/formats/numpy.py
--rw-r--r--   0 charlie    (501) staff       (20)    27079 2023-04-23 23:35:41.000000 pesummary-1.2.0/pesummary/core/file/formats/pesummary.py
--rw-r--r--   0 charlie    (501) staff       (20)     1288 2023-04-23 23:35:41.000000 pesummary-1.2.0/pesummary/core/file/formats/pickle.py
--rw-r--r--   0 charlie    (501) staff       (20)     6490 2023-04-23 23:35:41.000000 pesummary-1.2.0/pesummary/core/file/formats/sql.py
--rw-r--r--   0 charlie    (501) staff       (20)     1619 2023-04-23 23:35:41.000000 pesummary-1.2.0/pesummary/core/file/injection.py
--rw-r--r--   0 charlie    (501) staff       (20)     3756 2022-09-20 20:30:50.000000 pesummary-1.2.0/pesummary/core/file/mcmc.py
--rw-r--r--   0 charlie    (501) staff       (20)    26372 2023-04-23 23:35:41.000000 pesummary-1.2.0/pesummary/core/file/meta_file.py
--rw-r--r--   0 charlie    (501) staff       (20)     9009 2023-10-23 08:41:49.000000 pesummary-1.2.0/pesummary/core/file/read.py
--rw-r--r--   0 charlie    (501) staff       (20)     1942 2023-04-23 23:35:41.000000 pesummary-1.2.0/pesummary/core/finish.py
-drwxr-xr-x   0 charlie    (501) staff       (20)        0 2024-02-20 10:33:37.654485 pesummary-1.2.0/pesummary/core/js/
--rw-r--r--   0 charlie    (501) staff       (20)      109 2022-09-20 20:30:50.000000 pesummary-1.2.0/pesummary/core/js/__init__.py
--rw-r--r--   0 charlie    (501) staff       (20)     6956 2022-09-20 20:30:50.000000 pesummary-1.2.0/pesummary/core/js/combine_corner.js
--rw-r--r--   0 charlie    (501) staff       (20)     1007 2022-09-20 20:30:50.000000 pesummary-1.2.0/pesummary/core/js/expert.js
--rw-r--r--   0 charlie    (501) staff       (20)     4825 2022-09-20 20:30:50.000000 pesummary-1.2.0/pesummary/core/js/grab.js
--rw-r--r--   0 charlie    (501) staff       (20)     2272 2022-09-20 20:30:50.000000 pesummary-1.2.0/pesummary/core/js/html_to_csv.js
--rw-r--r--   0 charlie    (501) staff       (20)     1318 2022-09-20 20:30:50.000000 pesummary-1.2.0/pesummary/core/js/html_to_json.js
--rw-r--r--   0 charlie    (501) staff       (20)      705 2022-09-20 20:30:50.000000 pesummary-1.2.0/pesummary/core/js/html_to_shell.js
--rw-r--r--   0 charlie    (501) staff       (20)     1427 2022-09-20 20:30:50.000000 pesummary-1.2.0/pesummary/core/js/modal.js
--rw-r--r--   0 charlie    (501) staff       (20)     2361 2022-09-20 20:30:50.000000 pesummary-1.2.0/pesummary/core/js/multi_dropbar.js
--rw-r--r--   0 charlie    (501) staff       (20)     7471 2022-09-20 20:30:50.000000 pesummary-1.2.0/pesummary/core/js/multiple_posteriors.js
--rw-r--r--   0 charlie    (501) staff       (20)     2378 2022-09-20 20:30:50.000000 pesummary-1.2.0/pesummary/core/js/search.js
--rw-r--r--   0 charlie    (501) staff       (20)     1313 2022-09-20 20:30:50.000000 pesummary-1.2.0/pesummary/core/js/side_bar.js
-drwxr-xr-x   0 charlie    (501) staff       (20)        0 2024-02-20 10:33:37.654765 pesummary-1.2.0/pesummary/core/notebook/
--rw-r--r--   0 charlie    (501) staff       (20)      134 2022-09-20 20:30:50.000000 pesummary-1.2.0/pesummary/core/notebook/__init__.py
--rw-r--r--   0 charlie    (501) staff       (20)     6430 2022-09-20 20:30:50.000000 pesummary-1.2.0/pesummary/core/notebook/notebook.py
-drwxr-xr-x   0 charlie    (501) staff       (20)        0 2024-02-20 10:33:37.657190 pesummary-1.2.0/pesummary/core/plots/
--rw-r--r--   0 charlie    (501) staff       (20)      507 2022-09-20 20:30:50.000000 pesummary-1.2.0/pesummary/core/plots/__init__.py
--rw-r--r--   0 charlie    (501) staff       (20)     2901 2024-01-15 16:41:54.000000 pesummary-1.2.0/pesummary/core/plots/bounded_1d_kde.py
--rw-r--r--   0 charlie    (501) staff       (20)      566 2024-01-15 16:41:54.000000 pesummary-1.2.0/pesummary/core/plots/bounded_2d_kde.py
--rw-r--r--   0 charlie    (501) staff       (20)     8503 2023-04-23 23:35:41.000000 pesummary-1.2.0/pesummary/core/plots/corner.py
--rw-r--r--   0 charlie    (501) staff       (20)     2094 2022-09-20 20:30:50.000000 pesummary-1.2.0/pesummary/core/plots/figure.py
--rw-r--r--   0 charlie    (501) staff       (20)     7638 2023-04-23 23:35:41.000000 pesummary-1.2.0/pesummary/core/plots/interactive.py
--rw-r--r--   0 charlie    (501) staff       (20)     1841 2022-09-20 20:30:50.000000 pesummary-1.2.0/pesummary/core/plots/interpolate.py
--rw-r--r--   0 charlie    (501) staff       (20)      206 2022-09-20 20:30:50.000000 pesummary-1.2.0/pesummary/core/plots/latex_labels.py
--rw-r--r--   0 charlie    (501) staff       (20)    53281 2024-01-15 16:41:54.000000 pesummary-1.2.0/pesummary/core/plots/main.py
--rw-r--r--   0 charlie    (501) staff       (20)    32351 2024-02-20 10:30:45.000000 pesummary-1.2.0/pesummary/core/plots/plot.py
--rw-r--r--   0 charlie    (501) staff       (20)     2589 2022-09-20 20:30:50.000000 pesummary-1.2.0/pesummary/core/plots/population.py
--rw-r--r--   0 charlie    (501) staff       (20)    30619 2023-10-23 08:41:49.000000 pesummary-1.2.0/pesummary/core/plots/publication.py
-drwxr-xr-x   0 charlie    (501) staff       (20)        0 2024-02-20 10:33:37.658034 pesummary-1.2.0/pesummary/core/plots/seaborn/
--rw-r--r--   0 charlie    (501) staff       (20)      109 2022-09-20 20:30:50.000000 pesummary-1.2.0/pesummary/core/plots/seaborn/__init__.py
--rw-r--r--   0 charlie    (501) staff       (20)    15430 2022-09-20 20:30:50.000000 pesummary-1.2.0/pesummary/core/plots/seaborn/kde.py
--rw-r--r--   0 charlie    (501) staff       (20)    33098 2024-02-20 10:30:45.000000 pesummary-1.2.0/pesummary/core/plots/seaborn/violin.py
--rw-r--r--   0 charlie    (501) staff       (20)      748 2022-09-20 20:30:50.000000 pesummary-1.2.0/pesummary/core/reweight.py
-drwxr-xr-x   0 charlie    (501) staff       (20)        0 2024-02-20 10:33:37.659775 pesummary-1.2.0/pesummary/core/webpage/
--rw-r--r--   0 charlie    (501) staff       (20)     3038 2023-04-23 23:35:45.000000 pesummary-1.2.0/pesummary/core/webpage/base.py
--rw-r--r--   0 charlie    (501) staff       (20)      825 2023-04-23 23:35:45.000000 pesummary-1.2.0/pesummary/core/webpage/copyright.txt
--rw-r--r--   0 charlie    (501) staff       (20)    75259 2024-01-15 16:41:54.000000 pesummary-1.2.0/pesummary/core/webpage/main.py
--rw-r--r--   0 charlie    (501) staff       (20)     8151 2022-09-20 20:30:50.000000 pesummary-1.2.0/pesummary/core/webpage/tables.py
--rw-r--r--   0 charlie    (501) staff       (20)    53333 2024-01-15 16:41:54.000000 pesummary-1.2.0/pesummary/core/webpage/webpage.py
-drwxr-xr-x   0 charlie    (501) staff       (20)        0 2024-02-20 10:33:37.661824 pesummary-1.2.0/pesummary/gw/
--rw-r--r--   0 charlie    (501) staff       (20)      109 2022-09-20 20:30:50.000000 pesummary-1.2.0/pesummary/gw/__init__.py
--rw-r--r--   0 charlie    (501) staff       (20)    20204 2023-10-23 08:41:49.000000 pesummary-1.2.0/pesummary/gw/classification.py
-drwxr-xr-x   0 charlie    (501) staff       (20)        0 2024-02-20 10:33:37.662600 pesummary-1.2.0/pesummary/gw/cli/
--rw-r--r--   0 charlie    (501) staff       (20)      109 2023-04-23 23:35:41.000000 pesummary-1.2.0/pesummary/gw/cli/__init__.py
--rw-r--r--   0 charlie    (501) staff       (20)    64867 2024-01-15 16:41:54.000000 pesummary-1.2.0/pesummary/gw/cli/inputs.py
--rw-r--r--   0 charlie    (501) staff       (20)    21564 2023-04-23 23:35:41.000000 pesummary-1.2.0/pesummary/gw/cli/parser.py
-drwxr-xr-x   0 charlie    (501) staff       (20)        0 2024-02-20 10:33:37.665635 pesummary-1.2.0/pesummary/gw/conversions/
--rw-r--r--   0 charlie    (501) staff       (20)    95017 2024-02-20 10:30:45.000000 pesummary-1.2.0/pesummary/gw/conversions/__init__.py
--rw-r--r--   0 charlie    (501) staff       (20)     2299 2023-04-23 23:35:41.000000 pesummary-1.2.0/pesummary/gw/conversions/angles.py
--rw-r--r--   0 charlie    (501) staff       (20)     5839 2023-04-23 23:35:41.000000 pesummary-1.2.0/pesummary/gw/conversions/cosmology.py
--rw-r--r--   0 charlie    (501) staff       (20)    14034 2024-01-15 16:41:54.000000 pesummary-1.2.0/pesummary/gw/conversions/evolve.py
--rw-r--r--   0 charlie    (501) staff       (20)     3743 2022-09-20 20:30:50.000000 pesummary-1.2.0/pesummary/gw/conversions/mass.py
--rw-r--r--   0 charlie    (501) staff       (20)    31392 2022-09-20 20:30:50.000000 pesummary-1.2.0/pesummary/gw/conversions/nrutils.py
--rw-r--r--   0 charlie    (501) staff       (20)    27930 2023-04-23 23:35:41.000000 pesummary-1.2.0/pesummary/gw/conversions/remnant.py
--rw-r--r--   0 charlie    (501) staff       (20)    38522 2023-04-23 23:35:41.000000 pesummary-1.2.0/pesummary/gw/conversions/snr.py
--rw-r--r--   0 charlie    (501) staff       (20)     7953 2022-09-20 20:30:50.000000 pesummary-1.2.0/pesummary/gw/conversions/spins.py
--rw-r--r--   0 charlie    (501) staff       (20)    22067 2023-04-23 23:35:41.000000 pesummary-1.2.0/pesummary/gw/conversions/tgr.py
--rw-r--r--   0 charlie    (501) staff       (20)    13447 2023-10-23 08:41:49.000000 pesummary-1.2.0/pesummary/gw/conversions/tidal.py
--rw-r--r--   0 charlie    (501) staff       (20)      866 2022-09-20 20:30:50.000000 pesummary-1.2.0/pesummary/gw/conversions/time.py
--rw-r--r--   0 charlie    (501) staff       (20)      408 2022-09-20 20:30:50.000000 pesummary-1.2.0/pesummary/gw/conversions/utils.py
--rw-r--r--   0 charlie    (501) staff       (20)     1991 2022-09-20 20:30:50.000000 pesummary-1.2.0/pesummary/gw/cosmology.py
--rw-r--r--   0 charlie    (501) staff       (20)     6567 2024-02-20 10:30:45.000000 pesummary-1.2.0/pesummary/gw/fetch.py
-drwxr-xr-x   0 charlie    (501) staff       (20)        0 2024-02-20 10:33:37.671375 pesummary-1.2.0/pesummary/gw/file/
--rw-r--r--   0 charlie    (501) staff       (20)      750 2022-09-20 20:30:50.000000 pesummary-1.2.0/pesummary/gw/file/__init__.py
--rw-r--r--   0 charlie    (501) staff       (20)     7153 2023-04-23 23:35:41.000000 pesummary-1.2.0/pesummary/gw/file/calibration.py
--rw-r--r--   0 charlie    (501) staff       (20)      472 2022-09-20 20:30:50.000000 pesummary-1.2.0/pesummary/gw/file/conversions.py
-drwxr-xr-x   0 charlie    (501) staff       (20)        0 2024-02-20 10:33:37.673169 pesummary-1.2.0/pesummary/gw/file/formats/
--rw-r--r--   0 charlie    (501) staff       (20)     3495 2023-04-23 23:35:41.000000 pesummary-1.2.0/pesummary/gw/file/formats/GWTC1.py
--rw-r--r--   0 charlie    (501) staff       (20)      109 2022-09-20 20:30:50.000000 pesummary-1.2.0/pesummary/gw/file/formats/__init__.py
--rw-r--r--   0 charlie    (501) staff       (20)    25811 2023-04-23 23:35:41.000000 pesummary-1.2.0/pesummary/gw/file/formats/base_read.py
--rw-r--r--   0 charlie    (501) staff       (20)    11252 2024-02-20 10:30:45.000000 pesummary-1.2.0/pesummary/gw/file/formats/bilby.py
--rw-r--r--   0 charlie    (501) staff       (20)    10090 2023-04-23 23:35:41.000000 pesummary-1.2.0/pesummary/gw/file/formats/default.py
--rw-r--r--   0 charlie    (501) staff       (20)    20402 2023-04-23 23:35:41.000000 pesummary-1.2.0/pesummary/gw/file/formats/lalinference.py
--rw-r--r--   0 charlie    (501) staff       (20)    14349 2023-04-23 23:35:41.000000 pesummary-1.2.0/pesummary/gw/file/formats/pesummary.py
--rw-r--r--   0 charlie    (501) staff       (20)     1971 2022-09-20 20:30:50.000000 pesummary-1.2.0/pesummary/gw/file/formats/princeton.py
--rw-r--r--   0 charlie    (501) staff       (20)     1672 2023-04-23 23:35:41.000000 pesummary-1.2.0/pesummary/gw/file/formats/xml.py
--rw-r--r--   0 charlie    (501) staff       (20)     2095 2023-04-23 23:35:41.000000 pesummary-1.2.0/pesummary/gw/file/injection.py
--rw-r--r--   0 charlie    (501) staff       (20)    14137 2023-04-23 23:35:41.000000 pesummary-1.2.0/pesummary/gw/file/meta_file.py
--rw-r--r--   0 charlie    (501) staff       (20)    10521 2023-04-23 23:35:41.000000 pesummary-1.2.0/pesummary/gw/file/psd.py
--rw-r--r--   0 charlie    (501) staff       (20)     4126 2023-04-23 23:35:41.000000 pesummary-1.2.0/pesummary/gw/file/read.py
--rw-r--r--   0 charlie    (501) staff       (20)     4998 2022-09-20 20:30:50.000000 pesummary-1.2.0/pesummary/gw/file/skymap.py
--rw-r--r--   0 charlie    (501) staff       (20)    26901 2022-09-20 20:30:50.000000 pesummary-1.2.0/pesummary/gw/file/standard_names.py
--rw-r--r--   0 charlie    (501) staff       (20)     8572 2022-09-20 20:30:50.000000 pesummary-1.2.0/pesummary/gw/file/strain.py
--rw-r--r--   0 charlie    (501) staff       (20)     4556 2023-04-23 23:35:41.000000 pesummary-1.2.0/pesummary/gw/finish.py
--rw-r--r--   0 charlie    (501) staff       (20)     2048 2022-09-20 20:30:50.000000 pesummary-1.2.0/pesummary/gw/gracedb.py
-drwxr-xr-x   0 charlie    (501) staff       (20)        0 2024-02-20 10:33:37.673587 pesummary-1.2.0/pesummary/gw/notebook/
--rw-r--r--   0 charlie    (501) staff       (20)      151 2022-09-20 20:30:50.000000 pesummary-1.2.0/pesummary/gw/notebook/__init__.py
--rw-r--r--   0 charlie    (501) staff       (20)     1188 2022-09-20 20:30:50.000000 pesummary-1.2.0/pesummary/gw/notebook/notebook.py
--rw-r--r--   0 charlie    (501) staff       (20)     7067 2023-04-23 23:35:41.000000 pesummary-1.2.0/pesummary/gw/notebook/public.py
-drwxr-xr-x   0 charlie    (501) staff       (20)        0 2024-02-20 10:33:37.676143 pesummary-1.2.0/pesummary/gw/plots/
--rw-r--r--   0 charlie    (501) staff       (20)      109 2022-09-22 09:35:49.000000 pesummary-1.2.0/pesummary/gw/plots/__init__.py
--rw-r--r--   0 charlie    (501) staff       (20)     2666 2022-09-20 20:30:50.000000 pesummary-1.2.0/pesummary/gw/plots/bounds.py
--rw-r--r--   0 charlie    (501) staff       (20)     2244 2022-09-22 09:35:49.000000 pesummary-1.2.0/pesummary/gw/plots/cmap.py
--rw-r--r--   0 charlie    (501) staff       (20)     8714 2022-09-20 20:30:50.000000 pesummary-1.2.0/pesummary/gw/plots/cylon.csv
--rw-r--r--   0 charlie    (501) staff       (20)     9876 2023-04-23 23:35:45.000000 pesummary-1.2.0/pesummary/gw/plots/detchar.py
--rw-r--r--   0 charlie    (501) staff       (20)     7431 2022-09-20 20:30:50.000000 pesummary-1.2.0/pesummary/gw/plots/latex_labels.py
--rw-r--r--   0 charlie    (501) staff       (20)    49748 2024-02-20 10:30:45.000000 pesummary-1.2.0/pesummary/gw/plots/main.py
--rw-r--r--   0 charlie    (501) staff       (20)    54987 2024-02-20 10:30:45.000000 pesummary-1.2.0/pesummary/gw/plots/plot.py
--rw-r--r--   0 charlie    (501) staff       (20)     3204 2022-09-20 20:30:50.000000 pesummary-1.2.0/pesummary/gw/plots/public.py
--rw-r--r--   0 charlie    (501) staff       (20)    17311 2024-01-15 16:41:54.000000 pesummary-1.2.0/pesummary/gw/plots/publication.py
--rw-r--r--   0 charlie    (501) staff       (20)     6012 2022-09-20 20:30:50.000000 pesummary-1.2.0/pesummary/gw/plots/tgr.py
--rw-r--r--   0 charlie    (501) staff       (20)     5131 2023-04-23 23:35:41.000000 pesummary-1.2.0/pesummary/gw/pycbc.py
--rw-r--r--   0 charlie    (501) staff       (20)     3553 2023-04-23 23:35:41.000000 pesummary-1.2.0/pesummary/gw/reweight.py
--rw-r--r--   0 charlie    (501) staff       (20)    18863 2024-01-15 16:41:54.000000 pesummary-1.2.0/pesummary/gw/waveform.py
-drwxr-xr-x   0 charlie    (501) staff       (20)        0 2024-02-20 10:33:37.676869 pesummary-1.2.0/pesummary/gw/webpage/
--rw-r--r--   0 charlie    (501) staff       (20)      109 2022-09-20 20:30:50.000000 pesummary-1.2.0/pesummary/gw/webpage/__init__.py
--rw-r--r--   0 charlie    (501) staff       (20)    39087 2024-02-20 10:30:45.000000 pesummary-1.2.0/pesummary/gw/webpage/main.py
--rw-r--r--   0 charlie    (501) staff       (20)     7405 2022-09-20 20:30:50.000000 pesummary-1.2.0/pesummary/gw/webpage/public.py
--rw-r--r--   0 charlie    (501) staff       (20)    12756 2023-04-23 23:35:41.000000 pesummary-1.2.0/pesummary/gw/webpage/tgr.py
-drwxr-xr-x   0 charlie    (501) staff       (20)        0 2024-02-20 10:33:37.677345 pesummary-1.2.0/pesummary/io/
--rw-r--r--   0 charlie    (501) staff       (20)     1244 2022-09-20 20:30:50.000000 pesummary-1.2.0/pesummary/io/__init__.py
--rw-r--r--   0 charlie    (501) staff       (20)     3562 2022-09-20 20:30:50.000000 pesummary-1.2.0/pesummary/io/read.py
--rw-r--r--   0 charlie    (501) staff       (20)     4510 2022-09-20 20:30:50.000000 pesummary-1.2.0/pesummary/io/write.py
-drwxr-xr-x   0 charlie    (501) staff       (20)        0 2024-02-20 10:33:37.685848 pesummary-1.2.0/pesummary/tests/
--rw-r--r--   0 charlie    (501) staff       (20)      109 2022-09-20 20:30:50.000000 pesummary-1.2.0/pesummary/tests/__init__.py
--rw-r--r--   0 charlie    (501) staff       (20)      329 2023-04-23 23:35:41.000000 pesummary-1.2.0/pesummary/tests/_bilby.sh
--rw-r--r--   0 charlie    (501) staff       (20)     1949 2023-04-23 23:35:41.000000 pesummary-1.2.0/pesummary/tests/action_test.py
--rw-r--r--   0 charlie    (501) staff       (20)    18993 2024-02-20 10:30:45.000000 pesummary-1.2.0/pesummary/tests/base.py
--rw-r--r--   0 charlie    (501) staff       (20)      514 2023-04-23 23:35:41.000000 pesummary-1.2.0/pesummary/tests/bilby.sh
--rw-r--r--   0 charlie    (501) staff       (20)      656 2023-04-23 23:35:41.000000 pesummary-1.2.0/pesummary/tests/bilby_mcmc.sh
--rw-r--r--   0 charlie    (501) staff       (20)      933 2023-04-23 23:35:41.000000 pesummary-1.2.0/pesummary/tests/bilby_pipe.sh
--rw-r--r--   0 charlie    (501) staff       (20)     1907 2024-01-15 16:41:54.000000 pesummary-1.2.0/pesummary/tests/bounded_kde_test.py
--rw-r--r--   0 charlie    (501) staff       (20)     2703 2023-11-03 18:40:04.000000 pesummary-1.2.0/pesummary/tests/calibration_test.py
--rw-r--r--   0 charlie    (501) staff       (20)     7528 2024-02-20 10:30:45.000000 pesummary-1.2.0/pesummary/tests/classification_test.py
--rw-r--r--   0 charlie    (501) staff       (20)      430 2023-11-03 18:40:04.000000 pesummary-1.2.0/pesummary/tests/conftest.py
--rw-r--r--   0 charlie    (501) staff       (20)    47756 2024-02-20 10:30:45.000000 pesummary-1.2.0/pesummary/tests/conversion_test.py
--rw-r--r--   0 charlie    (501) staff       (20)     3026 2022-09-20 20:30:50.000000 pesummary-1.2.0/pesummary/tests/cosmology_test.py
--rw-r--r--   0 charlie    (501) staff       (20)       94 2022-09-20 20:30:50.000000 pesummary-1.2.0/pesummary/tests/example_config.ini
--rw-r--r--   0 charlie    (501) staff       (20)    90223 2024-02-20 10:30:45.000000 pesummary-1.2.0/pesummary/tests/executable_test.py
--rw-r--r--   0 charlie    (501) staff       (20)     1076 2022-09-20 20:30:50.000000 pesummary-1.2.0/pesummary/tests/executables.sh
--rw-r--r--   0 charlie    (501) staff       (20)     1626 2022-09-20 20:30:50.000000 pesummary-1.2.0/pesummary/tests/existing_file.py
--rw-r--r--   0 charlie    (501) staff       (20)     4676 2024-02-20 10:30:45.000000 pesummary-1.2.0/pesummary/tests/fetch_test.py
-drwxr-xr-x   0 charlie    (501) staff       (20)        0 2024-02-20 10:33:37.693898 pesummary-1.2.0/pesummary/tests/files/
--rw-r--r--   0 charlie    (501) staff       (20)       55 2022-09-20 20:30:50.000000 pesummary-1.2.0/pesummary/tests/files/.gitattributes
--rw-r--r--   0 charlie    (501) staff       (20)   843570 2022-09-20 20:30:50.000000 pesummary-1.2.0/pesummary/tests/files/calibration_envelope.txt
--rw-r--r--   0 charlie    (501) staff       (20)      545 2022-09-20 20:30:50.000000 pesummary-1.2.0/pesummary/tests/files/config_bilby.ini
--rw-r--r--   0 charlie    (501) staff       (20)     3576 2022-09-20 20:30:50.000000 pesummary-1.2.0/pesummary/tests/files/config_lalinference.ini
--rw-r--r--   0 charlie    (501) staff       (20)       19 2022-09-20 20:30:50.000000 pesummary-1.2.0/pesummary/tests/files/example.ini
--rw-r--r--   0 charlie    (501) staff       (20)   264597 2022-09-20 20:30:50.000000 pesummary-1.2.0/pesummary/tests/files/lal_pdf_for_summarytgr.dat.gz
--rw-r--r--   0 charlie    (501) staff       (20)    96127 2022-09-20 20:30:50.000000 pesummary-1.2.0/pesummary/tests/files/psd_file.txt
--rw-r--r--   0 charlie    (501) staff       (20)     1264 2023-11-03 18:40:04.000000 pesummary-1.2.0/pesummary/tests/finish_test.py
--rw-r--r--   0 charlie    (501) staff       (20)     1152 2022-09-20 20:30:50.000000 pesummary-1.2.0/pesummary/tests/imports.sh
--rw-r--r--   0 charlie    (501) staff       (20)     2470 2023-11-03 18:40:04.000000 pesummary-1.2.0/pesummary/tests/injection_test.py
--rw-r--r--   0 charlie    (501) staff       (20)    29256 2023-11-03 18:40:04.000000 pesummary-1.2.0/pesummary/tests/input_test.py
--rw-r--r--   0 charlie    (501) staff       (20)     1875 2022-09-20 20:30:50.000000 pesummary-1.2.0/pesummary/tests/lalinference.sh
--rw-r--r--   0 charlie    (501) staff       (20)     2461 2022-09-20 20:30:50.000000 pesummary-1.2.0/pesummary/tests/ligo_skymap_test.py
--rw-r--r--   0 charlie    (501) staff       (20)    12707 2022-09-20 20:30:50.000000 pesummary-1.2.0/pesummary/tests/main_injection.xml
--rw-r--r--   0 charlie    (501) staff       (20)       69 2022-09-20 20:30:50.000000 pesummary-1.2.0/pesummary/tests/main_input.ini
--rw-r--r--   0 charlie    (501) staff       (20)       33 2022-09-20 20:30:50.000000 pesummary-1.2.0/pesummary/tests/main_input_core.ini
--rw-r--r--   0 charlie    (501) staff       (20)    19886 2023-11-03 18:40:04.000000 pesummary-1.2.0/pesummary/tests/meta_file_test.py
--rw-r--r--   0 charlie    (501) staff       (20)     1501 2023-11-03 18:40:04.000000 pesummary-1.2.0/pesummary/tests/notebook_test.py
--rw-r--r--   0 charlie    (501) staff       (20)    20225 2023-11-03 18:40:04.000000 pesummary-1.2.0/pesummary/tests/plot_test.py
--rw-r--r--   0 charlie    (501) staff       (20)     4022 2023-11-03 18:40:04.000000 pesummary-1.2.0/pesummary/tests/psd_test.py
--rw-r--r--   0 charlie    (501) staff       (20)      667 2023-04-23 23:35:41.000000 pesummary-1.2.0/pesummary/tests/pycbc.sh
--rw-r--r--   0 charlie    (501) staff       (20)     4937 2023-11-03 18:40:04.000000 pesummary-1.2.0/pesummary/tests/pycbc_test.py
--rw-r--r--   0 charlie    (501) staff       (20)    75787 2023-11-03 18:40:04.000000 pesummary-1.2.0/pesummary/tests/read_test.py
--rw-r--r--   0 charlie    (501) staff       (20)     3482 2022-09-20 20:30:50.000000 pesummary-1.2.0/pesummary/tests/reweight_test.py
--rw-r--r--   0 charlie    (501) staff       (20)     3242 2022-09-20 20:30:50.000000 pesummary-1.2.0/pesummary/tests/strain_test.py
--rw-r--r--   0 charlie    (501) staff       (20)    10569 2024-02-20 10:30:45.000000 pesummary-1.2.0/pesummary/tests/summaryplots_test.py
--rw-r--r--   0 charlie    (501) staff       (20)    52125 2024-02-20 10:30:45.000000 pesummary-1.2.0/pesummary/tests/utils_test.py
--rw-r--r--   0 charlie    (501) staff       (20)     8486 2023-11-03 18:40:04.000000 pesummary-1.2.0/pesummary/tests/waveform_test.py
--rw-r--r--   0 charlie    (501) staff       (20)    11505 2024-01-15 16:41:54.000000 pesummary-1.2.0/pesummary/tests/webpage_test.py
--rw-r--r--   0 charlie    (501) staff       (20)    21589 2023-11-03 18:40:04.000000 pesummary-1.2.0/pesummary/tests/workflow_test.py
--rw-r--r--   0 charlie    (501) staff       (20)     7524 2023-11-03 18:40:04.000000 pesummary-1.2.0/pesummary/tests/write_test.py
-drwxr-xr-x   0 charlie    (501) staff       (20)        0 2024-02-20 10:33:37.697772 pesummary-1.2.0/pesummary/utils/
--rw-r--r--   0 charlie    (501) staff       (20)      240 2023-04-23 23:35:41.000000 pesummary-1.2.0/pesummary/utils/__init__.py
--rw-r--r--   0 charlie    (501) staff       (20)    10853 2024-02-20 10:30:45.000000 pesummary-1.2.0/pesummary/utils/array.py
--rw-r--r--   0 charlie    (501) staff       (20)     8888 2024-01-15 16:41:54.000000 pesummary-1.2.0/pesummary/utils/bounded_1d_kde.py
--rw-r--r--   0 charlie    (501) staff       (20)     3624 2024-01-15 16:41:54.000000 pesummary-1.2.0/pesummary/utils/bounded_2d_kde.py
--rw-r--r--   0 charlie    (501) staff       (20)     6015 2024-02-20 10:30:45.000000 pesummary-1.2.0/pesummary/utils/credible_interval.py
--rw-r--r--   0 charlie    (501) staff       (20)     9666 2023-10-23 08:41:49.000000 pesummary-1.2.0/pesummary/utils/decorators.py
--rw-r--r--   0 charlie    (501) staff       (20)     8392 2022-09-20 20:30:50.000000 pesummary-1.2.0/pesummary/utils/dict.py
--rw-r--r--   0 charlie    (501) staff       (20)      507 2022-09-20 20:30:50.000000 pesummary-1.2.0/pesummary/utils/exceptions.py
--rw-r--r--   0 charlie    (501) staff       (20)     2316 2024-01-15 16:41:54.000000 pesummary-1.2.0/pesummary/utils/kde_list.py
--rw-r--r--   0 charlie    (501) staff       (20)     2993 2022-09-20 20:30:50.000000 pesummary-1.2.0/pesummary/utils/list.py
--rw-r--r--   0 charlie    (501) staff       (20)     3187 2022-09-20 20:30:50.000000 pesummary-1.2.0/pesummary/utils/parameters.py
--rw-r--r--   0 charlie    (501) staff       (20)    16638 2024-01-19 09:12:30.000000 pesummary-1.2.0/pesummary/utils/pdf.py
--rw-r--r--   0 charlie    (501) staff       (20)     9255 2022-09-20 20:30:50.000000 pesummary-1.2.0/pesummary/utils/probability_dict.py
--rw-r--r--   0 charlie    (501) staff       (20)    76439 2024-02-20 10:30:45.000000 pesummary-1.2.0/pesummary/utils/samples_dict.py
--rw-r--r--   0 charlie    (501) staff       (20)     2991 2022-09-20 20:30:50.000000 pesummary-1.2.0/pesummary/utils/tqdm.py
--rw-r--r--   0 charlie    (501) staff       (20)    35507 2024-01-15 16:41:54.000000 pesummary-1.2.0/pesummary/utils/utils.py
-drwxr-xr-x   0 charlie    (501) staff       (20)        0 2024-02-20 10:33:37.698171 pesummary-1.2.0/pesummary.egg-info/
--rw-r--r--   0 charlie    (501) staff       (20)     4517 2024-02-20 10:33:37.000000 pesummary-1.2.0/pesummary.egg-info/PKG-INFO
--rw-r--r--   0 charlie    (501) staff       (20)    13466 2024-02-20 10:33:37.000000 pesummary-1.2.0/pesummary.egg-info/SOURCES.txt
--rw-r--r--   0 charlie    (501) staff       (20)        1 2024-02-20 10:33:37.000000 pesummary-1.2.0/pesummary.egg-info/dependency_links.txt
--rw-r--r--   0 charlie    (501) staff       (20)     1099 2024-02-20 10:33:37.000000 pesummary-1.2.0/pesummary.egg-info/entry_points.txt
--rw-r--r--   0 charlie    (501) staff       (20)      707 2024-02-20 10:33:37.000000 pesummary-1.2.0/pesummary.egg-info/requires.txt
--rw-r--r--   0 charlie    (501) staff       (20)       10 2024-02-20 10:33:37.000000 pesummary-1.2.0/pesummary.egg-info/top_level.txt
--rw-r--r--   0 charlie    (501) staff       (20)     4362 2024-02-20 10:30:45.000000 pesummary-1.2.0/pyproject.toml
--rw-r--r--   0 charlie    (501) staff       (20)       38 2024-02-20 10:33:37.700970 pesummary-1.2.0/setup.cfg
--rw-r--r--   0 charlie    (501) staff       (20)     1337 2022-09-20 20:30:50.000000 pesummary-1.2.0/setup.py
+drwxr-xr-x   0 charlie    (501) staff       (20)        0 2024-06-03 08:12:48.458527 pesummary-1.3.0/
+-rw-r--r--   0 charlie    (501) staff       (20)      318 2022-09-20 20:30:50.000000 pesummary-1.3.0/.AUTHORS
+-rw-r--r--   0 charlie    (501) staff       (20)      259 2023-10-23 08:41:49.000000 pesummary-1.3.0/.flake8
+-rw-r--r--   0 charlie    (501) staff       (20)      119 2022-09-20 20:30:50.000000 pesummary-1.3.0/.gitattributes
+-rw-r--r--   0 charlie    (501) staff       (20)      646 2022-09-20 20:30:50.000000 pesummary-1.3.0/.gitignore
+-rw-r--r--   0 charlie    (501) staff       (20)    13823 2024-02-20 10:30:45.000000 pesummary-1.3.0/.gitlab-ci.yml
+-rw-r--r--   0 charlie    (501) staff       (20)      123 2022-09-20 20:30:50.000000 pesummary-1.3.0/.pre-commit-config.yaml
+-rw-r--r--   0 charlie    (501) staff       (20)      490 2024-06-03 08:08:38.000000 pesummary-1.3.0/.readthedocs.yml
+-rw-r--r--   0 charlie    (501) staff       (20)    41646 2023-04-23 23:35:41.000000 pesummary-1.3.0/CHANGELOG.md
+-rw-r--r--   0 charlie    (501) staff       (20)     4818 2022-09-20 20:30:50.000000 pesummary-1.3.0/CONTRIBUTING.md
+-rw-r--r--   0 charlie    (501) staff       (20)     1116 2023-04-23 23:35:41.000000 pesummary-1.3.0/LICENSE.md
+-rw-r--r--   0 charlie    (501) staff       (20)      308 2022-09-20 20:30:50.000000 pesummary-1.3.0/MANIFEST.in
+-rw-r--r--   0 charlie    (501) staff       (20)     4562 2024-06-03 08:12:48.458276 pesummary-1.3.0/PKG-INFO
+-rw-r--r--   0 charlie    (501) staff       (20)     1481 2022-09-20 20:30:50.000000 pesummary-1.3.0/README.md
+drwxr-xr-x   0 charlie    (501) staff       (20)        0 2024-06-03 08:12:48.374002 pesummary-1.3.0/containers/
+-rw-r--r--   0 charlie    (501) staff       (20)      977 2022-09-20 20:30:50.000000 pesummary-1.3.0/containers/Dockerfile-template
+-rw-r--r--   0 charlie    (501) staff       (20)     1231 2023-04-23 23:35:41.000000 pesummary-1.3.0/containers/write_dockerfile.py
+drwxr-xr-x   0 charlie    (501) staff       (20)        0 2024-06-03 08:12:48.375803 pesummary-1.3.0/docs/
+-rw-r--r--   0 charlie    (501) staff       (20)       46 2022-09-20 20:30:50.000000 pesummary-1.3.0/docs/.gitattributes
+-rw-r--r--   0 charlie    (501) staff       (20)     1633 2022-09-20 20:30:50.000000 pesummary-1.3.0/docs/citing_pesummary.rst
+drwxr-xr-x   0 charlie    (501) staff       (20)        0 2024-06-03 08:12:48.376047 pesummary-1.3.0/docs/conf/
+-rw-r--r--   0 charlie    (501) staff       (20)      693 2023-04-23 23:35:45.000000 pesummary-1.3.0/docs/conf/configuration.rst
+-rw-r--r--   0 charlie    (501) staff       (20)     9118 2023-04-23 23:35:45.000000 pesummary-1.3.0/docs/conf.py
+drwxr-xr-x   0 charlie    (501) staff       (20)        0 2024-06-03 08:12:48.378397 pesummary-1.3.0/docs/core/
+-rw-r--r--   0 charlie    (501) staff       (20)     1339 2022-09-20 20:30:50.000000 pesummary-1.3.0/docs/core/Array.rst
+-rw-r--r--   0 charlie    (501) staff       (20)     2686 2022-09-20 20:30:50.000000 pesummary-1.3.0/docs/core/MCMCSamplesDict.rst
+-rw-r--r--   0 charlie    (501) staff       (20)     5211 2022-09-20 20:30:50.000000 pesummary-1.3.0/docs/core/MultiAnalysisSamplesDict.rst
+-rw-r--r--   0 charlie    (501) staff       (20)      391 2022-09-20 20:30:50.000000 pesummary-1.3.0/docs/core/ProbabilityDict.rst
+-rw-r--r--   0 charlie    (501) staff       (20)      395 2022-09-20 20:30:50.000000 pesummary-1.3.0/docs/core/ProbabilityDict2D.rst
+-rw-r--r--   0 charlie    (501) staff       (20)     3906 2022-09-20 20:30:50.000000 pesummary-1.3.0/docs/core/SamplesDict.rst
+-rw-r--r--   0 charlie    (501) staff       (20)     2993 2022-09-20 20:30:50.000000 pesummary-1.3.0/docs/core/bounded_kdes.rst
+drwxr-xr-x   0 charlie    (501) staff       (20)        0 2024-06-03 08:12:48.380111 pesummary-1.3.0/docs/core/cli/
+-rw-r--r--   0 charlie    (501) staff       (20)      778 2022-09-20 20:30:50.000000 pesummary-1.3.0/docs/core/cli/summaryclean.rst
+-rw-r--r--   0 charlie    (501) staff       (20)      636 2022-09-20 20:30:50.000000 pesummary-1.3.0/docs/core/cli/summarycombine.rst
+-rw-r--r--   0 charlie    (501) staff       (20)      643 2022-09-20 20:30:50.000000 pesummary-1.3.0/docs/core/cli/summarycombine_posteriors.rst
+-rw-r--r--   0 charlie    (501) staff       (20)    15166 2022-09-20 20:30:50.000000 pesummary-1.3.0/docs/core/cli/summarycompare.rst
+-rw-r--r--   0 charlie    (501) staff       (20)      366 2022-09-20 20:30:50.000000 pesummary-1.3.0/docs/core/cli/summaryextract.rst
+-rw-r--r--   0 charlie    (501) staff       (20)      351 2022-09-20 20:30:50.000000 pesummary-1.3.0/docs/core/cli/summarymodify.rst
+-rw-r--r--   0 charlie    (501) staff       (20)     3312 2023-04-23 23:35:45.000000 pesummary-1.3.0/docs/core/cli/summarypages.rst
+-rw-r--r--   0 charlie    (501) staff       (20)      529 2022-09-20 20:30:50.000000 pesummary-1.3.0/docs/core/cli/summarypageslw.rst
+-rw-r--r--   0 charlie    (501) staff       (20)     2815 2023-04-23 23:35:45.000000 pesummary-1.3.0/docs/core/cli/summarypublication.rst
+-rw-r--r--   0 charlie    (501) staff       (20)      451 2022-09-20 20:30:50.000000 pesummary-1.3.0/docs/core/cli/summarysplit.rst
+-rw-r--r--   0 charlie    (501) staff       (20)      239 2022-09-20 20:30:50.000000 pesummary-1.3.0/docs/core/cli/summaryversion.rst
+drwxr-xr-x   0 charlie    (501) staff       (20)        0 2024-06-03 08:12:48.380587 pesummary-1.3.0/docs/core/examples/
+-rw-r--r--   0 charlie    (501) staff       (20)      130 2022-09-20 20:30:50.000000 pesummary-1.3.0/docs/core/examples/bounded_kde.png
+-rw-r--r--   0 charlie    (501) staff       (20)      130 2022-09-20 20:30:50.000000 pesummary-1.3.0/docs/core/examples/bounded_kde_uniform.png
+-rw-r--r--   0 charlie    (501) staff       (20)      130 2022-09-20 20:30:50.000000 pesummary-1.3.0/docs/core/examples/bounded_kdeplot.png
+-rw-r--r--   0 charlie    (501) staff       (20)     3564 2022-09-20 20:30:50.000000 pesummary-1.3.0/docs/core/file_formats.rst
+-rw-r--r--   0 charlie    (501) staff       (20)     1225 2022-09-20 20:30:50.000000 pesummary-1.3.0/docs/core/index.rst
+-rw-r--r--   0 charlie    (501) staff       (20)     1079 2022-09-20 20:30:50.000000 pesummary-1.3.0/docs/core/pdf.rst
+-rw-r--r--   0 charlie    (501) staff       (20)     4858 2023-04-23 23:35:45.000000 pesummary-1.3.0/docs/core/pesummary_file.rst
+-rw-r--r--   0 charlie    (501) staff       (20)     4791 2022-09-20 20:30:50.000000 pesummary-1.3.0/docs/core/read.rst
+-rw-r--r--   0 charlie    (501) staff       (20)      411 2023-04-23 23:35:45.000000 pesummary-1.3.0/docs/core/seaborn.rst
+drwxr-xr-x   0 charlie    (501) staff       (20)        0 2024-06-03 08:12:48.380753 pesummary-1.3.0/docs/core/tutorials/
+drwxr-xr-x   0 charlie    (501) staff       (20)        0 2024-06-03 08:12:48.381753 pesummary-1.3.0/docs/core/tutorials/examples/
+-rw-r--r--   0 charlie    (501) staff       (20)      130 2022-09-20 20:30:50.000000 pesummary-1.3.0/docs/core/tutorials/examples/Histogram.png
+-rw-r--r--   0 charlie    (501) staff       (20)      130 2022-09-20 20:30:50.000000 pesummary-1.3.0/docs/core/tutorials/examples/MultiAnalysisCorner.png
+-rw-r--r--   0 charlie    (501) staff       (20)      130 2022-09-20 20:30:50.000000 pesummary-1.3.0/docs/core/tutorials/examples/MultiAnalysisHistogram.png
+-rw-r--r--   0 charlie    (501) staff       (20)      131 2022-09-20 20:30:50.000000 pesummary-1.3.0/docs/core/tutorials/examples/MultiAnalysisReverseTriangle.png
+-rw-r--r--   0 charlie    (501) staff       (20)      131 2022-09-20 20:30:50.000000 pesummary-1.3.0/docs/core/tutorials/examples/MultiAnalysisTriangle.png
+-rw-r--r--   0 charlie    (501) staff       (20)      130 2022-09-20 20:30:50.000000 pesummary-1.3.0/docs/core/tutorials/examples/violin.png
+-rw-r--r--   0 charlie    (501) staff       (20)     2839 2022-09-20 20:30:50.000000 pesummary-1.3.0/docs/core/tutorials/plotting_from_metafile.rst
+-rw-r--r--   0 charlie    (501) staff       (20)     1746 2023-04-23 23:35:45.000000 pesummary-1.3.0/docs/core/write.rst
+-rw-r--r--   0 charlie    (501) staff       (20)     1974 2024-02-20 10:30:45.000000 pesummary-1.3.0/docs/front.html.in
+drwxr-xr-x   0 charlie    (501) staff       (20)        0 2024-06-03 08:12:48.384424 pesummary-1.3.0/docs/gw/
+-rw-r--r--   0 charlie    (501) staff       (20)     3666 2022-09-20 20:30:50.000000 pesummary-1.3.0/docs/gw/Conversion.rst
+-rw-r--r--   0 charlie    (501) staff       (20)     1929 2023-04-23 23:35:45.000000 pesummary-1.3.0/docs/gw/SamplesDict.rst
+-rw-r--r--   0 charlie    (501) staff       (20)     3249 2023-04-23 23:35:45.000000 pesummary-1.3.0/docs/gw/calibration.rst
+-rw-r--r--   0 charlie    (501) staff       (20)     5891 2023-04-23 23:35:45.000000 pesummary-1.3.0/docs/gw/classification.rst
+drwxr-xr-x   0 charlie    (501) staff       (20)        0 2024-06-03 08:12:48.385609 pesummary-1.3.0/docs/gw/cli/
+-rw-r--r--   0 charlie    (501) staff       (20)      186 2022-09-20 20:30:50.000000 pesummary-1.3.0/docs/gw/cli/executable_descriptions.rst
+-rw-r--r--   0 charlie    (501) staff       (20)     1353 2022-09-20 20:30:50.000000 pesummary-1.3.0/docs/gw/cli/summaryclassification.rst
+-rw-r--r--   0 charlie    (501) staff       (20)     1996 2022-09-20 20:30:50.000000 pesummary-1.3.0/docs/gw/cli/summarydetchar.rst
+-rw-r--r--   0 charlie    (501) staff       (20)      616 2022-09-20 20:30:50.000000 pesummary-1.3.0/docs/gw/cli/summarygracedb.rst
+-rw-r--r--   0 charlie    (501) staff       (20)      566 2022-09-20 20:30:50.000000 pesummary-1.3.0/docs/gw/cli/summarypipe.rst
+-rw-r--r--   0 charlie    (501) staff       (20)     1433 2022-09-20 20:30:50.000000 pesummary-1.3.0/docs/gw/cli/summaryrecreate.rst
+-rw-r--r--   0 charlie    (501) staff       (20)      682 2022-09-20 20:30:50.000000 pesummary-1.3.0/docs/gw/cli/summaryreview.rst
+-rw-r--r--   0 charlie    (501) staff       (20)     2637 2022-09-20 20:30:50.000000 pesummary-1.3.0/docs/gw/cli/summarytgr.rst
+-rw-r--r--   0 charlie    (501) staff       (20)     2704 2024-06-03 08:08:38.000000 pesummary-1.3.0/docs/gw/corner.rst
+drwxr-xr-x   0 charlie    (501) staff       (20)        0 2024-06-03 08:12:48.387317 pesummary-1.3.0/docs/gw/examples/
+-rw-r--r--   0 charlie    (501) staff       (20)   173856 2024-06-03 08:08:40.000000 pesummary-1.3.0/docs/gw/examples/GW150914_corner.png
+-rw-r--r--   0 charlie    (501) staff       (20)      130 2022-09-20 20:30:50.000000 pesummary-1.3.0/docs/gw/examples/GW190412_violin.png
+-rw-r--r--   0 charlie    (501) staff       (20)      130 2022-09-20 20:30:50.000000 pesummary-1.3.0/docs/gw/examples/bounded_violin.png
+-rw-r--r--   0 charlie    (501) staff       (20)      130 2022-09-20 20:30:50.000000 pesummary-1.3.0/docs/gw/examples/gaussian_violin.png
+-rw-r--r--   0 charlie    (501) staff       (20)    49483 2024-06-03 08:08:41.000000 pesummary-1.3.0/docs/gw/examples/kde_corner.png
+-rw-r--r--   0 charlie    (501) staff       (20)      130 2022-09-20 20:30:50.000000 pesummary-1.3.0/docs/gw/examples/split_violin.png
+-rw-r--r--   0 charlie    (501) staff       (20)     1317 2023-04-23 23:35:45.000000 pesummary-1.3.0/docs/gw/fetch.rst
+-rw-r--r--   0 charlie    (501) staff       (20)     1674 2023-04-23 23:35:45.000000 pesummary-1.3.0/docs/gw/file_formats.rst
+-rw-r--r--   0 charlie    (501) staff       (20)     3330 2024-06-03 08:08:38.000000 pesummary-1.3.0/docs/gw/index.rst
+-rw-r--r--   0 charlie    (501) staff       (20)      238 2022-09-20 20:30:50.000000 pesummary-1.3.0/docs/gw/parameters.rst
+-rw-r--r--   0 charlie    (501) staff       (20)     3462 2023-04-23 23:35:45.000000 pesummary-1.3.0/docs/gw/pesummary_file.rst
+-rw-r--r--   0 charlie    (501) staff       (20)     2948 2022-09-20 20:30:50.000000 pesummary-1.3.0/docs/gw/psd.rst
+-rw-r--r--   0 charlie    (501) staff       (20)     1791 2022-09-20 20:30:50.000000 pesummary-1.3.0/docs/gw/read.rst
+-rw-r--r--   0 charlie    (501) staff       (20)     4759 2022-09-20 20:30:50.000000 pesummary-1.3.0/docs/gw/remnant_fits.rst
+-rw-r--r--   0 charlie    (501) staff       (20)     2595 2022-09-20 20:30:50.000000 pesummary-1.3.0/docs/gw/strain.rst
+drwxr-xr-x   0 charlie    (501) staff       (20)        0 2024-06-03 08:12:48.388473 pesummary-1.3.0/docs/gw/summarypages/
+drwxr-xr-x   0 charlie    (501) staff       (20)        0 2024-06-03 08:12:48.389148 pesummary-1.3.0/docs/gw/summarypages/IMRPhenomPv3HM/
+-rw-r--r--   0 charlie    (501) staff       (20)      692 2022-09-20 20:30:50.000000 pesummary-1.3.0/docs/gw/summarypages/IMRPhenomPv3HM/classification.rst
+-rw-r--r--   0 charlie    (501) staff       (20)     1128 2022-09-20 20:30:50.000000 pesummary-1.3.0/docs/gw/summarypages/IMRPhenomPv3HM/corner.rst
+drwxr-xr-x   0 charlie    (501) staff       (20)        0 2024-06-03 08:12:48.389558 pesummary-1.3.0/docs/gw/summarypages/IMRPhenomPv3HM/examples/
+-rw-r--r--   0 charlie    (501) staff       (20)      966 2022-09-20 20:30:50.000000 pesummary-1.3.0/docs/gw/summarypages/IMRPhenomPv3HM/examples/.gitattributes
+-rw-r--r--   0 charlie    (501) staff       (20)      132 2022-09-20 20:30:50.000000 pesummary-1.3.0/docs/gw/summarypages/IMRPhenomPv3HM/examples/corner.mp4
+-rw-r--r--   0 charlie    (501) staff       (20)      132 2022-09-20 20:30:50.000000 pesummary-1.3.0/docs/gw/summarypages/IMRPhenomPv3HM/examples/interactive_corner_source.html
+-rw-r--r--   0 charlie    (501) staff       (20)      646 2022-09-20 20:30:50.000000 pesummary-1.3.0/docs/gw/summarypages/IMRPhenomPv3HM/home.rst
+-rw-r--r--   0 charlie    (501) staff       (20)      976 2022-09-20 20:30:50.000000 pesummary-1.3.0/docs/gw/summarypages/IMRPhenomPv3HM/interactive.rst
+-rw-r--r--   0 charlie    (501) staff       (20)     1785 2022-09-20 20:30:50.000000 pesummary-1.3.0/docs/gw/summarypages/IMRPhenomPv3HM/mass_1.rst
+-rw-r--r--   0 charlie    (501) staff       (20)      391 2022-09-20 20:30:50.000000 pesummary-1.3.0/docs/gw/summarypages/about.rst
+drwxr-xr-x   0 charlie    (501) staff       (20)        0 2024-06-03 08:12:48.390049 pesummary-1.3.0/docs/gw/summarypages/comparison/
+drwxr-xr-x   0 charlie    (501) staff       (20)        0 2024-06-03 08:12:48.390206 pesummary-1.3.0/docs/gw/summarypages/comparison/examples/
+-rw-r--r--   0 charlie    (501) staff       (20)   639556 2022-09-20 20:30:50.000000 pesummary-1.3.0/docs/gw/summarypages/comparison/examples/interactive_ridgeline.html
+-rw-r--r--   0 charlie    (501) staff       (20)      615 2022-09-20 20:30:50.000000 pesummary-1.3.0/docs/gw/summarypages/comparison/home.rst
+-rw-r--r--   0 charlie    (501) staff       (20)      912 2022-09-20 20:30:50.000000 pesummary-1.3.0/docs/gw/summarypages/comparison/interactive.rst
+-rw-r--r--   0 charlie    (501) staff       (20)     2030 2022-09-20 20:30:50.000000 pesummary-1.3.0/docs/gw/summarypages/comparison/mass_1.rst
+-rw-r--r--   0 charlie    (501) staff       (20)      549 2022-09-20 20:30:50.000000 pesummary-1.3.0/docs/gw/summarypages/downloads.rst
+drwxr-xr-x   0 charlie    (501) staff       (20)        0 2024-06-03 08:12:48.391676 pesummary-1.3.0/docs/gw/summarypages/examples/
+-rw-r--r--   0 charlie    (501) staff       (20)      131 2022-09-20 20:30:50.000000 pesummary-1.3.0/docs/gw/summarypages/examples/watermark.png
+-rw-r--r--   0 charlie    (501) staff       (20)      980 2022-09-20 20:30:50.000000 pesummary-1.3.0/docs/gw/summarypages/home.rst
+-rw-r--r--   0 charlie    (501) staff       (20)      356 2022-09-20 20:30:50.000000 pesummary-1.3.0/docs/gw/summarypages/logging.rst
+-rw-r--r--   0 charlie    (501) staff       (20)      504 2022-09-20 20:30:50.000000 pesummary-1.3.0/docs/gw/summarypages/publication.rst
+-rw-r--r--   0 charlie    (501) staff       (20)     1166 2022-09-20 20:30:50.000000 pesummary-1.3.0/docs/gw/summarypages/version.rst
+-rw-r--r--   0 charlie    (501) staff       (20)      502 2022-09-20 20:30:50.000000 pesummary-1.3.0/docs/gw/summarypages/watermark.rst
+-rw-r--r--   0 charlie    (501) staff       (20)     4038 2022-09-20 20:30:50.000000 pesummary-1.3.0/docs/gw/tgr_file.rst
+drwxr-xr-x   0 charlie    (501) staff       (20)        0 2024-06-03 08:12:48.393466 pesummary-1.3.0/docs/gw/tutorials/
+-rw-r--r--   0 charlie    (501) staff       (20)     1707 2023-04-23 23:35:45.000000 pesummary-1.3.0/docs/gw/tutorials/GWTC1_plots.rst
+-rw-r--r--   0 charlie    (501) staff       (20)      967 2023-04-23 23:35:45.000000 pesummary-1.3.0/docs/gw/tutorials/comparing_public_data_files.rst
+-rw-r--r--   0 charlie    (501) staff       (20)     9519 2022-09-20 20:30:50.000000 pesummary-1.3.0/docs/gw/tutorials/conversions_and_condor.rst
+drwxr-xr-x   0 charlie    (501) staff       (20)        0 2024-06-03 08:12:48.396312 pesummary-1.3.0/docs/gw/tutorials/examples/
+-rw-r--r--   0 charlie    (501) staff       (20)      528 2022-09-20 20:30:50.000000 pesummary-1.3.0/docs/gw/tutorials/examples/.gitattributes
+-rw-r--r--   0 charlie    (501) staff       (20)      130 2022-09-20 20:30:50.000000 pesummary-1.3.0/docs/gw/tutorials/examples/2d_contour_plot_luminosity_distance_and_chirp_mass.png
+-rw-r--r--   0 charlie    (501) staff       (20)      130 2022-09-20 20:30:50.000000 pesummary-1.3.0/docs/gw/tutorials/examples/2d_contour_plot_mass_1_and_mass_2.png
+-rw-r--r--   0 charlie    (501) staff       (20)      130 2022-09-20 20:30:50.000000 pesummary-1.3.0/docs/gw/tutorials/examples/2d_contour_plot_theta_jn_and_luminosity_distance.png
+-rw-r--r--   0 charlie    (501) staff       (20)      131 2022-09-20 20:30:50.000000 pesummary-1.3.0/docs/gw/tutorials/examples/GW150914.png
+-rw-r--r--   0 charlie    (501) staff       (20)      131 2022-09-20 20:30:50.000000 pesummary-1.3.0/docs/gw/tutorials/examples/GW190814.png
+-rw-r--r--   0 charlie    (501) staff       (20)      130 2022-09-20 20:30:50.000000 pesummary-1.3.0/docs/gw/tutorials/examples/Histogram.png
+-rw-r--r--   0 charlie    (501) staff       (20)      131 2022-09-20 20:30:50.000000 pesummary-1.3.0/docs/gw/tutorials/examples/MultiAnalysisCorner.png
+-rw-r--r--   0 charlie    (501) staff       (20)      130 2022-09-20 20:30:50.000000 pesummary-1.3.0/docs/gw/tutorials/examples/MultiAnalysisHistogram.png
+-rw-r--r--   0 charlie    (501) staff       (20)      131 2022-09-20 20:30:50.000000 pesummary-1.3.0/docs/gw/tutorials/examples/MultiAnalysisReverseTriangle.png
+-rw-r--r--   0 charlie    (501) staff       (20)      131 2022-09-20 20:30:50.000000 pesummary-1.3.0/docs/gw/tutorials/examples/MultiAnalysisTriangle.png
+-rw-r--r--   0 charlie    (501) staff       (20)      130 2022-09-20 20:30:50.000000 pesummary-1.3.0/docs/gw/tutorials/examples/PSD.png
+-rw-r--r--   0 charlie    (501) staff       (20)      131 2022-09-20 20:30:50.000000 pesummary-1.3.0/docs/gw/tutorials/examples/comparison_for_GW150914.png
+-rw-r--r--   0 charlie    (501) staff       (20)      130 2022-09-20 20:30:50.000000 pesummary-1.3.0/docs/gw/tutorials/examples/event_scatter_plot_total_mass_and_redshift.png
+-rw-r--r--   0 charlie    (501) staff       (20)      130 2022-09-20 20:30:50.000000 pesummary-1.3.0/docs/gw/tutorials/examples/spin_disk.png
+-rw-r--r--   0 charlie    (501) staff       (20)      130 2022-09-20 20:30:50.000000 pesummary-1.3.0/docs/gw/tutorials/examples/uncertainty_waveform_td.png
+-rw-r--r--   0 charlie    (501) staff       (20)      130 2022-09-20 20:30:50.000000 pesummary-1.3.0/docs/gw/tutorials/examples/violin.png
+-rw-r--r--   0 charlie    (501) staff       (20)      130 2022-09-20 20:30:50.000000 pesummary-1.3.0/docs/gw/tutorials/examples/violin_plot_mass_ratio.png
+-rw-r--r--   0 charlie    (501) staff       (20)      130 2022-09-20 20:30:50.000000 pesummary-1.3.0/docs/gw/tutorials/examples/waveform_fd.png
+-rw-r--r--   0 charlie    (501) staff       (20)      130 2022-09-20 20:30:50.000000 pesummary-1.3.0/docs/gw/tutorials/examples/waveform_td.png
+-rw-r--r--   0 charlie    (501) staff       (20)     3997 2023-04-23 23:35:45.000000 pesummary-1.3.0/docs/gw/tutorials/interaction_with_ligo_skymap.rst
+-rw-r--r--   0 charlie    (501) staff       (20)      801 2022-09-20 20:30:50.000000 pesummary-1.3.0/docs/gw/tutorials/make_your_own_page_from_metafile.rst
+-rw-r--r--   0 charlie    (501) staff       (20)      811 2023-04-23 23:35:45.000000 pesummary-1.3.0/docs/gw/tutorials/plot_waveform_on_strain_data.rst
+-rw-r--r--   0 charlie    (501) staff       (20)     3473 2022-09-20 20:30:50.000000 pesummary-1.3.0/docs/gw/tutorials/plotting_from_metafile.rst
+-rw-r--r--   0 charlie    (501) staff       (20)      709 2023-04-23 23:35:45.000000 pesummary-1.3.0/docs/gw/tutorials/population_scatter_plot_GWTC-1.rst
+-rw-r--r--   0 charlie    (501) staff       (20)      814 2022-09-20 20:30:50.000000 pesummary-1.3.0/docs/gw/tutorials/public_pages.rst
+-rw-r--r--   0 charlie    (501) staff       (20)      690 2023-04-23 23:35:45.000000 pesummary-1.3.0/docs/gw/tutorials/release_notebook.rst
+-rw-r--r--   0 charlie    (501) staff       (20)     1614 2023-04-23 23:35:45.000000 pesummary-1.3.0/docs/gw/tutorials/waveforms.rst
+-rw-r--r--   0 charlie    (501) staff       (20)     4667 2022-09-20 20:30:50.000000 pesummary-1.3.0/docs/gw/violin.rst
+-rw-r--r--   0 charlie    (501) staff       (20)     1891 2023-04-23 23:35:45.000000 pesummary-1.3.0/docs/index.rst
+-rw-r--r--   0 charlie    (501) staff       (20)     2845 2023-04-23 23:35:41.000000 pesummary-1.3.0/docs/installation.rst
+drwxr-xr-x   0 charlie    (501) staff       (20)        0 2024-06-03 08:12:48.396443 pesummary-1.3.0/docs/io/
+-rw-r--r--   0 charlie    (501) staff       (20)     3014 2023-04-23 23:35:45.000000 pesummary-1.3.0/docs/io/read.rst
+-rw-r--r--   0 charlie    (501) staff       (20)     2351 2022-09-20 20:30:50.000000 pesummary-1.3.0/docs/virtual_environment.rst
+-rw-r--r--   0 charlie    (501) staff       (20)     2209 2022-09-20 20:30:50.000000 pesummary-1.3.0/docs/what_is_pesummary.rst
+drwxr-xr-x   0 charlie    (501) staff       (20)        0 2024-06-03 08:12:48.397218 pesummary-1.3.0/examples/
+drwxr-xr-x   0 charlie    (501) staff       (20)        0 2024-06-03 08:12:48.398122 pesummary-1.3.0/examples/core/
+-rw-r--r--   0 charlie    (501) staff       (20)     1127 2022-09-20 20:30:50.000000 pesummary-1.3.0/examples/core/bounded_kdeplot.py
+-rw-r--r--   0 charlie    (501) staff       (20)     1002 2022-09-20 20:30:50.000000 pesummary-1.3.0/examples/core/extract_information_from_pesummary_file.py
+-rw-r--r--   0 charlie    (501) staff       (20)     3120 2022-09-20 20:30:50.000000 pesummary-1.3.0/examples/core/multiple_analysis_custom_read.py
+-rw-r--r--   0 charlie    (501) staff       (20)     1490 2022-09-20 20:30:50.000000 pesummary-1.3.0/examples/core/pesummary_data_structure.txt
+-rw-r--r--   0 charlie    (501) staff       (20)     2495 2022-09-20 20:30:50.000000 pesummary-1.3.0/examples/core/single_analysis_custom_read.py
+-rw-r--r--   0 charlie    (501) staff       (20)     1711 2022-09-20 20:30:50.000000 pesummary-1.3.0/examples/custom_plot.py
+-rw-r--r--   0 charlie    (501) staff       (20)     2174 2023-04-23 23:35:41.000000 pesummary-1.3.0/examples/extract_information_without_pesummary.py
+drwxr-xr-x   0 charlie    (501) staff       (20)        0 2024-06-03 08:12:48.400667 pesummary-1.3.0/examples/gw/
+-rw-r--r--   0 charlie    (501) staff       (20)     1097 2022-09-20 20:30:50.000000 pesummary-1.3.0/examples/gw/GWTC-1_population_scatterplot.sh
+-rw-r--r--   0 charlie    (501) staff       (20)     2624 2022-09-20 20:30:50.000000 pesummary-1.3.0/examples/gw/GWTC1_plots.sh
+-rw-r--r--   0 charlie    (501) staff       (20)     1599 2022-09-20 20:30:50.000000 pesummary-1.3.0/examples/gw/compare_GW150914.py
+-rw-r--r--   0 charlie    (501) staff       (20)      941 2022-09-20 20:30:50.000000 pesummary-1.3.0/examples/gw/extract_information_from_pesummary_file.py
+-rw-r--r--   0 charlie    (501) staff       (20)     2709 2023-04-23 23:35:41.000000 pesummary-1.3.0/examples/gw/extract_information_from_pesummary_file_without_pesummary.py
+-rw-r--r--   0 charlie    (501) staff       (20)      895 2022-09-20 20:30:50.000000 pesummary-1.3.0/examples/gw/fetch_open_data.py
+-rw-r--r--   0 charlie    (501) staff       (20)      681 2023-04-23 23:35:41.000000 pesummary-1.3.0/examples/gw/fetch_open_strain.py
+-rw-r--r--   0 charlie    (501) staff       (20)     1699 2022-09-20 20:30:50.000000 pesummary-1.3.0/examples/gw/latex.py
+-rw-r--r--   0 charlie    (501) staff       (20)     1351 2023-04-23 23:35:41.000000 pesummary-1.3.0/examples/gw/ligo_skymap.py
+-rwxr-xr-x   0 charlie    (501) staff       (20)      523 2022-09-20 20:30:50.000000 pesummary-1.3.0/examples/gw/make_public_release.py
+-rw-r--r--   0 charlie    (501) staff       (20)     1390 2023-04-23 23:35:41.000000 pesummary-1.3.0/examples/gw/making_a_waveform_in_frequency_domain.py
+-rw-r--r--   0 charlie    (501) staff       (20)     1281 2023-04-23 23:35:41.000000 pesummary-1.3.0/examples/gw/making_a_waveform_in_time_domain.py
+-rw-r--r--   0 charlie    (501) staff       (20)      748 2023-04-23 23:35:41.000000 pesummary-1.3.0/examples/gw/making_a_waveform_in_time_domain_with_uncertainty.py
+-rw-r--r--   0 charlie    (501) staff       (20)     2690 2022-09-20 20:30:50.000000 pesummary-1.3.0/examples/gw/pesummary_data_structure.txt
+-rw-r--r--   0 charlie    (501) staff       (20)     1034 2022-09-20 20:30:50.000000 pesummary-1.3.0/examples/gw/plot_waveform_on_strain_data_GW150914.py
+-rw-r--r--   0 charlie    (501) staff       (20)      775 2023-04-23 23:35:41.000000 pesummary-1.3.0/examples/gw/plot_waveform_on_strain_data_GW190814.py
+-rw-r--r--   0 charlie    (501) staff       (20)     1641 2022-09-20 20:30:50.000000 pesummary-1.3.0/examples/gw/prior_conditioning.py
+-rw-r--r--   0 charlie    (501) staff       (20)     1504 2023-04-23 23:35:41.000000 pesummary-1.3.0/examples/gw/violin_plots.py
+-rw-r--r--   0 charlie    (501) staff       (20)      108 2022-09-20 20:30:50.000000 pesummary-1.3.0/examples/pesummary_core.ini
+-rw-r--r--   0 charlie    (501) staff       (20)      282 2022-09-20 20:30:50.000000 pesummary-1.3.0/examples/pesummary_gw.ini
+-rw-r--r--   0 charlie    (501) staff       (20)     1431 2023-04-23 23:35:41.000000 pesummary-1.3.0/examples/run_with_python.py
+drwxr-xr-x   0 charlie    (501) staff       (20)        0 2024-06-03 08:12:48.401264 pesummary-1.3.0/pesummary/
+-rw-r--r--   0 charlie    (501) staff       (20)      303 2024-06-03 08:12:48.000000 pesummary-1.3.0/pesummary/.version
+-rw-r--r--   0 charlie    (501) staff       (20)     1997 2022-09-20 20:30:50.000000 pesummary-1.3.0/pesummary/__init__.py
+-rw-r--r--   0 charlie    (501) staff       (20)      411 2024-06-03 08:12:48.000000 pesummary-1.3.0/pesummary/_version.py
+-rw-r--r--   0 charlie    (501) staff       (20)     5674 2022-09-20 20:30:50.000000 pesummary-1.3.0/pesummary/_version_helper.py
+drwxr-xr-x   0 charlie    (501) staff       (20)        0 2024-06-03 08:12:48.406577 pesummary-1.3.0/pesummary/cli/
+-rw-r--r--   0 charlie    (501) staff       (20)       52 2022-09-20 20:30:50.000000 pesummary-1.3.0/pesummary/cli/__init__.py
+-rw-r--r--   0 charlie    (501) staff       (20)     7587 2023-11-03 18:40:04.000000 pesummary-1.3.0/pesummary/cli/summaryclassification.py
+-rw-r--r--   0 charlie    (501) staff       (20)     2508 2023-04-23 23:35:41.000000 pesummary-1.3.0/pesummary/cli/summaryclean.py
+-rw-r--r--   0 charlie    (501) staff       (20)     1257 2023-04-23 23:35:41.000000 pesummary-1.3.0/pesummary/cli/summarycombine.py
+-rw-r--r--   0 charlie    (501) staff       (20)     8223 2023-04-23 23:35:41.000000 pesummary-1.3.0/pesummary/cli/summarycombine_posteriors.py
+-rw-r--r--   0 charlie    (501) staff       (20)    11646 2023-04-23 23:35:41.000000 pesummary-1.3.0/pesummary/cli/summarycompare.py
+-rw-r--r--   0 charlie    (501) staff       (20)     3778 2023-04-23 23:35:41.000000 pesummary-1.3.0/pesummary/cli/summarydetchar.py
+-rw-r--r--   0 charlie    (501) staff       (20)     2563 2023-04-23 23:35:41.000000 pesummary-1.3.0/pesummary/cli/summaryextract.py
+-rw-r--r--   0 charlie    (501) staff       (20)     1434 2023-04-23 23:35:41.000000 pesummary-1.3.0/pesummary/cli/summarygracedb.py
+-rw-r--r--   0 charlie    (501) staff       (20)     9659 2024-01-15 16:41:54.000000 pesummary-1.3.0/pesummary/cli/summaryjscompare.py
+-rw-r--r--   0 charlie    (501) staff       (20)    24057 2023-04-23 23:35:41.000000 pesummary-1.3.0/pesummary/cli/summarymodify.py
+-rw-r--r--   0 charlie    (501) staff       (20)    10894 2023-04-23 23:35:41.000000 pesummary-1.3.0/pesummary/cli/summarypages.py
+-rw-r--r--   0 charlie    (501) staff       (20)     4097 2023-04-23 23:35:41.000000 pesummary-1.3.0/pesummary/cli/summarypageslw.py
+-rw-r--r--   0 charlie    (501) staff       (20)    31078 2023-04-23 23:35:41.000000 pesummary-1.3.0/pesummary/cli/summarypipe.py
+-rw-r--r--   0 charlie    (501) staff       (20)    13579 2024-01-15 16:41:54.000000 pesummary-1.3.0/pesummary/cli/summaryplots.py
+-rw-r--r--   0 charlie    (501) staff       (20)    13547 2023-04-23 23:35:41.000000 pesummary-1.3.0/pesummary/cli/summarypublication.py
+-rw-r--r--   0 charlie    (501) staff       (20)    10990 2023-04-23 23:35:41.000000 pesummary-1.3.0/pesummary/cli/summaryrecreate.py
+-rw-r--r--   0 charlie    (501) staff       (20)    31084 2023-11-03 18:40:04.000000 pesummary-1.3.0/pesummary/cli/summaryreview.py
+-rw-r--r--   0 charlie    (501) staff       (20)     6758 2023-04-23 23:35:41.000000 pesummary-1.3.0/pesummary/cli/summarysplit.py
+-rw-r--r--   0 charlie    (501) staff       (20)    15650 2024-02-20 10:30:45.000000 pesummary-1.3.0/pesummary/cli/summarytest.py
+-rw-r--r--   0 charlie    (501) staff       (20)     9472 2023-04-23 23:35:41.000000 pesummary-1.3.0/pesummary/cli/summarytgr.py
+-rw-r--r--   0 charlie    (501) staff       (20)      386 2022-09-20 20:30:50.000000 pesummary-1.3.0/pesummary/cli/summaryversion.py
+drwxr-xr-x   0 charlie    (501) staff       (20)        0 2024-06-03 08:12:48.407374 pesummary-1.3.0/pesummary/conf/
+-rw-r--r--   0 charlie    (501) staff       (20)       52 2022-09-20 20:30:50.000000 pesummary-1.3.0/pesummary/conf/__init__.py
+-rw-r--r--   0 charlie    (501) staff       (20)     5198 2022-09-20 20:30:50.000000 pesummary-1.3.0/pesummary/conf/caption.py
+-rw-r--r--   0 charlie    (501) staff       (20)     4749 2024-06-03 08:08:38.000000 pesummary-1.3.0/pesummary/conf/configuration.py
+-rw-r--r--   0 charlie    (501) staff       (20)      422 2022-09-20 20:30:50.000000 pesummary-1.3.0/pesummary/conf/matplotlib_rcparams.sty
+drwxr-xr-x   0 charlie    (501) staff       (20)        0 2024-06-03 08:12:48.408079 pesummary-1.3.0/pesummary/core/
+-rw-r--r--   0 charlie    (501) staff       (20)      109 2022-09-20 20:30:50.000000 pesummary-1.3.0/pesummary/core/__init__.py
+drwxr-xr-x   0 charlie    (501) staff       (20)        0 2024-06-03 08:12:48.409759 pesummary-1.3.0/pesummary/core/cli/
+-rw-r--r--   0 charlie    (501) staff       (20)      109 2023-04-23 23:35:41.000000 pesummary-1.3.0/pesummary/core/cli/__init__.py
+-rw-r--r--   0 charlie    (501) staff       (20)    10430 2023-04-23 23:35:41.000000 pesummary-1.3.0/pesummary/core/cli/actions.py
+-rw-r--r--   0 charlie    (501) staff       (20)    83837 2024-01-15 16:41:54.000000 pesummary-1.3.0/pesummary/core/cli/inputs.py
+-rw-r--r--   0 charlie    (501) staff       (20)    25359 2024-02-20 10:30:45.000000 pesummary-1.3.0/pesummary/core/cli/parser.py
+drwxr-xr-x   0 charlie    (501) staff       (20)        0 2024-06-03 08:12:48.411295 pesummary-1.3.0/pesummary/core/css/
+-rw-r--r--   0 charlie    (501) staff       (20)      109 2022-09-20 20:30:50.000000 pesummary-1.3.0/pesummary/core/css/__init__.py
+-rw-r--r--   0 charlie    (501) staff       (20)      178 2022-09-20 20:30:50.000000 pesummary-1.3.0/pesummary/core/css/font.css
+-rw-r--r--   0 charlie    (501) staff       (20)     1601 2022-09-20 20:30:50.000000 pesummary-1.3.0/pesummary/core/css/image_styles.css
+-rw-r--r--   0 charlie    (501) staff       (20)     1137 2022-09-20 20:30:50.000000 pesummary-1.3.0/pesummary/core/css/navbar.css
+-rw-r--r--   0 charlie    (501) staff       (20)     1806 2022-09-20 20:30:50.000000 pesummary-1.3.0/pesummary/core/css/side_bar.css
+-rw-r--r--   0 charlie    (501) staff       (20)      612 2022-09-20 20:30:50.000000 pesummary-1.3.0/pesummary/core/css/table.css
+-rw-r--r--   0 charlie    (501) staff       (20)      879 2022-09-20 20:30:50.000000 pesummary-1.3.0/pesummary/core/css/toggle.css
+-rw-r--r--   0 charlie    (501) staff       (20)      411 2022-09-20 20:30:50.000000 pesummary-1.3.0/pesummary/core/css/watermark.css
+-rw-r--r--   0 charlie    (501) staff       (20)     6364 2024-02-20 10:30:45.000000 pesummary-1.3.0/pesummary/core/fetch.py
+drwxr-xr-x   0 charlie    (501) staff       (20)        0 2024-06-03 08:12:48.412331 pesummary-1.3.0/pesummary/core/file/
+-rw-r--r--   0 charlie    (501) staff       (20)      109 2022-09-20 20:30:50.000000 pesummary-1.3.0/pesummary/core/file/__init__.py
+drwxr-xr-x   0 charlie    (501) staff       (20)        0 2024-06-03 08:12:48.415168 pesummary-1.3.0/pesummary/core/file/formats/
+-rw-r--r--   0 charlie    (501) staff       (20)      109 2022-09-20 20:30:50.000000 pesummary-1.3.0/pesummary/core/file/formats/__init__.py
+-rw-r--r--   0 charlie    (501) staff       (20)    39412 2024-02-20 10:30:45.000000 pesummary-1.3.0/pesummary/core/file/formats/base_read.py
+-rw-r--r--   0 charlie    (501) staff       (20)    16259 2024-01-15 16:41:54.000000 pesummary-1.3.0/pesummary/core/file/formats/bilby.py
+-rw-r--r--   0 charlie    (501) staff       (20)     2252 2022-09-20 20:30:50.000000 pesummary-1.3.0/pesummary/core/file/formats/csv.py
+-rw-r--r--   0 charlie    (501) staff       (20)     2717 2023-04-23 23:35:41.000000 pesummary-1.3.0/pesummary/core/file/formats/dat.py
+-rw-r--r--   0 charlie    (501) staff       (20)    10261 2023-04-23 23:35:41.000000 pesummary-1.3.0/pesummary/core/file/formats/default.py
+-rw-r--r--   0 charlie    (501) staff       (20)     7086 2023-04-23 23:35:41.000000 pesummary-1.3.0/pesummary/core/file/formats/hdf5.py
+-rw-r--r--   0 charlie    (501) staff       (20)     3282 2023-04-23 23:35:41.000000 pesummary-1.3.0/pesummary/core/file/formats/ini.py
+-rw-r--r--   0 charlie    (501) staff       (20)     6841 2023-04-23 23:35:41.000000 pesummary-1.3.0/pesummary/core/file/formats/json.py
+-rw-r--r--   0 charlie    (501) staff       (20)     3776 2022-09-20 20:30:50.000000 pesummary-1.3.0/pesummary/core/file/formats/numpy.py
+-rw-r--r--   0 charlie    (501) staff       (20)    27079 2023-04-23 23:35:41.000000 pesummary-1.3.0/pesummary/core/file/formats/pesummary.py
+-rw-r--r--   0 charlie    (501) staff       (20)     1288 2023-04-23 23:35:41.000000 pesummary-1.3.0/pesummary/core/file/formats/pickle.py
+-rw-r--r--   0 charlie    (501) staff       (20)     6490 2023-04-23 23:35:41.000000 pesummary-1.3.0/pesummary/core/file/formats/sql.py
+-rw-r--r--   0 charlie    (501) staff       (20)     1619 2023-04-23 23:35:41.000000 pesummary-1.3.0/pesummary/core/file/injection.py
+-rw-r--r--   0 charlie    (501) staff       (20)     3756 2022-09-20 20:30:50.000000 pesummary-1.3.0/pesummary/core/file/mcmc.py
+-rw-r--r--   0 charlie    (501) staff       (20)    26372 2023-04-23 23:35:41.000000 pesummary-1.3.0/pesummary/core/file/meta_file.py
+-rw-r--r--   0 charlie    (501) staff       (20)     9009 2023-10-23 08:41:49.000000 pesummary-1.3.0/pesummary/core/file/read.py
+-rw-r--r--   0 charlie    (501) staff       (20)     1942 2023-04-23 23:35:41.000000 pesummary-1.3.0/pesummary/core/finish.py
+drwxr-xr-x   0 charlie    (501) staff       (20)        0 2024-06-03 08:12:48.416992 pesummary-1.3.0/pesummary/core/js/
+-rw-r--r--   0 charlie    (501) staff       (20)      109 2022-09-20 20:30:50.000000 pesummary-1.3.0/pesummary/core/js/__init__.py
+-rw-r--r--   0 charlie    (501) staff       (20)     6956 2022-09-20 20:30:50.000000 pesummary-1.3.0/pesummary/core/js/combine_corner.js
+-rw-r--r--   0 charlie    (501) staff       (20)     1007 2022-09-20 20:30:50.000000 pesummary-1.3.0/pesummary/core/js/expert.js
+-rw-r--r--   0 charlie    (501) staff       (20)     4825 2022-09-20 20:30:50.000000 pesummary-1.3.0/pesummary/core/js/grab.js
+-rw-r--r--   0 charlie    (501) staff       (20)     2272 2022-09-20 20:30:50.000000 pesummary-1.3.0/pesummary/core/js/html_to_csv.js
+-rw-r--r--   0 charlie    (501) staff       (20)     1318 2022-09-20 20:30:50.000000 pesummary-1.3.0/pesummary/core/js/html_to_json.js
+-rw-r--r--   0 charlie    (501) staff       (20)      705 2022-09-20 20:30:50.000000 pesummary-1.3.0/pesummary/core/js/html_to_shell.js
+-rw-r--r--   0 charlie    (501) staff       (20)     1427 2022-09-20 20:30:50.000000 pesummary-1.3.0/pesummary/core/js/modal.js
+-rw-r--r--   0 charlie    (501) staff       (20)     2361 2022-09-20 20:30:50.000000 pesummary-1.3.0/pesummary/core/js/multi_dropbar.js
+-rw-r--r--   0 charlie    (501) staff       (20)     7471 2022-09-20 20:30:50.000000 pesummary-1.3.0/pesummary/core/js/multiple_posteriors.js
+-rw-r--r--   0 charlie    (501) staff       (20)     2378 2022-09-20 20:30:50.000000 pesummary-1.3.0/pesummary/core/js/search.js
+-rw-r--r--   0 charlie    (501) staff       (20)     1313 2022-09-20 20:30:50.000000 pesummary-1.3.0/pesummary/core/js/side_bar.js
+drwxr-xr-x   0 charlie    (501) staff       (20)        0 2024-06-03 08:12:48.417247 pesummary-1.3.0/pesummary/core/notebook/
+-rw-r--r--   0 charlie    (501) staff       (20)      134 2022-09-20 20:30:50.000000 pesummary-1.3.0/pesummary/core/notebook/__init__.py
+-rw-r--r--   0 charlie    (501) staff       (20)     6430 2022-09-20 20:30:50.000000 pesummary-1.3.0/pesummary/core/notebook/notebook.py
+drwxr-xr-x   0 charlie    (501) staff       (20)        0 2024-06-03 08:12:48.419525 pesummary-1.3.0/pesummary/core/plots/
+-rw-r--r--   0 charlie    (501) staff       (20)      507 2022-09-20 20:30:50.000000 pesummary-1.3.0/pesummary/core/plots/__init__.py
+-rw-r--r--   0 charlie    (501) staff       (20)     2901 2024-01-15 16:41:54.000000 pesummary-1.3.0/pesummary/core/plots/bounded_1d_kde.py
+-rw-r--r--   0 charlie    (501) staff       (20)      566 2024-01-15 16:41:54.000000 pesummary-1.3.0/pesummary/core/plots/bounded_2d_kde.py
+-rw-r--r--   0 charlie    (501) staff       (20)    13733 2024-06-03 08:08:38.000000 pesummary-1.3.0/pesummary/core/plots/corner.py
+-rw-r--r--   0 charlie    (501) staff       (20)     2094 2022-09-20 20:30:50.000000 pesummary-1.3.0/pesummary/core/plots/figure.py
+-rw-r--r--   0 charlie    (501) staff       (20)     7638 2023-04-23 23:35:41.000000 pesummary-1.3.0/pesummary/core/plots/interactive.py
+-rw-r--r--   0 charlie    (501) staff       (20)     1841 2022-09-20 20:30:50.000000 pesummary-1.3.0/pesummary/core/plots/interpolate.py
+-rw-r--r--   0 charlie    (501) staff       (20)      206 2022-09-20 20:30:50.000000 pesummary-1.3.0/pesummary/core/plots/latex_labels.py
+-rw-r--r--   0 charlie    (501) staff       (20)    53281 2024-01-15 16:41:54.000000 pesummary-1.3.0/pesummary/core/plots/main.py
+-rw-r--r--   0 charlie    (501) staff       (20)    32398 2024-06-03 08:08:38.000000 pesummary-1.3.0/pesummary/core/plots/plot.py
+-rw-r--r--   0 charlie    (501) staff       (20)     2589 2022-09-20 20:30:50.000000 pesummary-1.3.0/pesummary/core/plots/population.py
+-rw-r--r--   0 charlie    (501) staff       (20)    30619 2023-10-23 08:41:49.000000 pesummary-1.3.0/pesummary/core/plots/publication.py
+drwxr-xr-x   0 charlie    (501) staff       (20)        0 2024-06-03 08:12:48.420307 pesummary-1.3.0/pesummary/core/plots/seaborn/
+-rw-r--r--   0 charlie    (501) staff       (20)      109 2022-09-20 20:30:50.000000 pesummary-1.3.0/pesummary/core/plots/seaborn/__init__.py
+-rw-r--r--   0 charlie    (501) staff       (20)    15430 2022-09-20 20:30:50.000000 pesummary-1.3.0/pesummary/core/plots/seaborn/kde.py
+-rw-r--r--   0 charlie    (501) staff       (20)    33098 2024-02-20 10:30:45.000000 pesummary-1.3.0/pesummary/core/plots/seaborn/violin.py
+-rw-r--r--   0 charlie    (501) staff       (20)      748 2022-09-20 20:30:50.000000 pesummary-1.3.0/pesummary/core/reweight.py
+drwxr-xr-x   0 charlie    (501) staff       (20)        0 2024-06-03 08:12:48.421998 pesummary-1.3.0/pesummary/core/webpage/
+-rw-r--r--   0 charlie    (501) staff       (20)     3038 2023-04-23 23:35:45.000000 pesummary-1.3.0/pesummary/core/webpage/base.py
+-rw-r--r--   0 charlie    (501) staff       (20)      825 2023-04-23 23:35:45.000000 pesummary-1.3.0/pesummary/core/webpage/copyright.txt
+-rw-r--r--   0 charlie    (501) staff       (20)    75259 2024-01-15 16:41:54.000000 pesummary-1.3.0/pesummary/core/webpage/main.py
+-rw-r--r--   0 charlie    (501) staff       (20)     8151 2022-09-20 20:30:50.000000 pesummary-1.3.0/pesummary/core/webpage/tables.py
+-rw-r--r--   0 charlie    (501) staff       (20)    53333 2024-01-15 16:41:54.000000 pesummary-1.3.0/pesummary/core/webpage/webpage.py
+drwxr-xr-x   0 charlie    (501) staff       (20)        0 2024-06-03 08:12:48.424195 pesummary-1.3.0/pesummary/gw/
+-rw-r--r--   0 charlie    (501) staff       (20)      109 2022-09-20 20:30:50.000000 pesummary-1.3.0/pesummary/gw/__init__.py
+-rw-r--r--   0 charlie    (501) staff       (20)    20204 2023-10-23 08:41:49.000000 pesummary-1.3.0/pesummary/gw/classification.py
+drwxr-xr-x   0 charlie    (501) staff       (20)        0 2024-06-03 08:12:48.425041 pesummary-1.3.0/pesummary/gw/cli/
+-rw-r--r--   0 charlie    (501) staff       (20)      109 2023-04-23 23:35:41.000000 pesummary-1.3.0/pesummary/gw/cli/__init__.py
+-rw-r--r--   0 charlie    (501) staff       (20)    66636 2024-06-03 08:08:38.000000 pesummary-1.3.0/pesummary/gw/cli/inputs.py
+-rw-r--r--   0 charlie    (501) staff       (20)    22445 2024-06-03 08:08:38.000000 pesummary-1.3.0/pesummary/gw/cli/parser.py
+drwxr-xr-x   0 charlie    (501) staff       (20)        0 2024-06-03 08:12:48.428541 pesummary-1.3.0/pesummary/gw/conversions/
+-rw-r--r--   0 charlie    (501) staff       (20)    96819 2024-06-03 08:08:38.000000 pesummary-1.3.0/pesummary/gw/conversions/__init__.py
+-rw-r--r--   0 charlie    (501) staff       (20)     2299 2023-04-23 23:35:41.000000 pesummary-1.3.0/pesummary/gw/conversions/angles.py
+-rw-r--r--   0 charlie    (501) staff       (20)     5839 2023-04-23 23:35:41.000000 pesummary-1.3.0/pesummary/gw/conversions/cosmology.py
+-rw-r--r--   0 charlie    (501) staff       (20)    14034 2024-01-15 16:41:54.000000 pesummary-1.3.0/pesummary/gw/conversions/evolve.py
+-rw-r--r--   0 charlie    (501) staff       (20)     3743 2022-09-20 20:30:50.000000 pesummary-1.3.0/pesummary/gw/conversions/mass.py
+-rw-r--r--   0 charlie    (501) staff       (20)    31392 2022-09-20 20:30:50.000000 pesummary-1.3.0/pesummary/gw/conversions/nrutils.py
+-rw-r--r--   0 charlie    (501) staff       (20)    35863 2024-06-03 08:08:38.000000 pesummary-1.3.0/pesummary/gw/conversions/remnant.py
+-rw-r--r--   0 charlie    (501) staff       (20)    38718 2024-06-03 08:08:38.000000 pesummary-1.3.0/pesummary/gw/conversions/snr.py
+-rw-r--r--   0 charlie    (501) staff       (20)     7953 2022-09-20 20:30:50.000000 pesummary-1.3.0/pesummary/gw/conversions/spins.py
+-rw-r--r--   0 charlie    (501) staff       (20)    22067 2023-04-23 23:35:41.000000 pesummary-1.3.0/pesummary/gw/conversions/tgr.py
+-rw-r--r--   0 charlie    (501) staff       (20)    13447 2023-10-23 08:41:49.000000 pesummary-1.3.0/pesummary/gw/conversions/tidal.py
+-rw-r--r--   0 charlie    (501) staff       (20)      866 2022-09-20 20:30:50.000000 pesummary-1.3.0/pesummary/gw/conversions/time.py
+-rw-r--r--   0 charlie    (501) staff       (20)      408 2022-09-20 20:30:50.000000 pesummary-1.3.0/pesummary/gw/conversions/utils.py
+-rw-r--r--   0 charlie    (501) staff       (20)     1991 2022-09-20 20:30:50.000000 pesummary-1.3.0/pesummary/gw/cosmology.py
+-rw-r--r--   0 charlie    (501) staff       (20)     6567 2024-02-20 10:30:45.000000 pesummary-1.3.0/pesummary/gw/fetch.py
+drwxr-xr-x   0 charlie    (501) staff       (20)        0 2024-06-03 08:12:48.430781 pesummary-1.3.0/pesummary/gw/file/
+-rw-r--r--   0 charlie    (501) staff       (20)      750 2022-09-20 20:30:50.000000 pesummary-1.3.0/pesummary/gw/file/__init__.py
+-rw-r--r--   0 charlie    (501) staff       (20)     7153 2023-04-23 23:35:41.000000 pesummary-1.3.0/pesummary/gw/file/calibration.py
+-rw-r--r--   0 charlie    (501) staff       (20)      472 2022-09-20 20:30:50.000000 pesummary-1.3.0/pesummary/gw/file/conversions.py
+drwxr-xr-x   0 charlie    (501) staff       (20)        0 2024-06-03 08:12:48.432340 pesummary-1.3.0/pesummary/gw/file/formats/
+-rw-r--r--   0 charlie    (501) staff       (20)     3495 2023-04-23 23:35:41.000000 pesummary-1.3.0/pesummary/gw/file/formats/GWTC1.py
+-rw-r--r--   0 charlie    (501) staff       (20)      109 2022-09-20 20:30:50.000000 pesummary-1.3.0/pesummary/gw/file/formats/__init__.py
+-rw-r--r--   0 charlie    (501) staff       (20)    25811 2023-04-23 23:35:41.000000 pesummary-1.3.0/pesummary/gw/file/formats/base_read.py
+-rw-r--r--   0 charlie    (501) staff       (20)    12022 2024-06-03 08:08:38.000000 pesummary-1.3.0/pesummary/gw/file/formats/bilby.py
+-rw-r--r--   0 charlie    (501) staff       (20)    10090 2023-04-23 23:35:41.000000 pesummary-1.3.0/pesummary/gw/file/formats/default.py
+-rw-r--r--   0 charlie    (501) staff       (20)    20402 2023-04-23 23:35:41.000000 pesummary-1.3.0/pesummary/gw/file/formats/lalinference.py
+-rw-r--r--   0 charlie    (501) staff       (20)    14349 2023-04-23 23:35:41.000000 pesummary-1.3.0/pesummary/gw/file/formats/pesummary.py
+-rw-r--r--   0 charlie    (501) staff       (20)     1971 2022-09-20 20:30:50.000000 pesummary-1.3.0/pesummary/gw/file/formats/princeton.py
+-rw-r--r--   0 charlie    (501) staff       (20)     2818 2024-06-03 08:08:38.000000 pesummary-1.3.0/pesummary/gw/file/formats/pycbc.py
+-rw-r--r--   0 charlie    (501) staff       (20)     1672 2023-04-23 23:35:41.000000 pesummary-1.3.0/pesummary/gw/file/formats/xml.py
+-rw-r--r--   0 charlie    (501) staff       (20)     2095 2023-04-23 23:35:41.000000 pesummary-1.3.0/pesummary/gw/file/injection.py
+-rw-r--r--   0 charlie    (501) staff       (20)    14137 2023-04-23 23:35:41.000000 pesummary-1.3.0/pesummary/gw/file/meta_file.py
+-rw-r--r--   0 charlie    (501) staff       (20)    11933 2024-06-03 08:08:38.000000 pesummary-1.3.0/pesummary/gw/file/psd.py
+-rw-r--r--   0 charlie    (501) staff       (20)     4545 2024-06-03 08:08:38.000000 pesummary-1.3.0/pesummary/gw/file/read.py
+-rw-r--r--   0 charlie    (501) staff       (20)     4998 2022-09-20 20:30:50.000000 pesummary-1.3.0/pesummary/gw/file/skymap.py
+-rw-r--r--   0 charlie    (501) staff       (20)    27419 2024-06-03 08:08:38.000000 pesummary-1.3.0/pesummary/gw/file/standard_names.py
+-rw-r--r--   0 charlie    (501) staff       (20)     8572 2022-09-20 20:30:50.000000 pesummary-1.3.0/pesummary/gw/file/strain.py
+-rw-r--r--   0 charlie    (501) staff       (20)     4556 2023-04-23 23:35:41.000000 pesummary-1.3.0/pesummary/gw/finish.py
+-rw-r--r--   0 charlie    (501) staff       (20)     2048 2022-09-20 20:30:50.000000 pesummary-1.3.0/pesummary/gw/gracedb.py
+drwxr-xr-x   0 charlie    (501) staff       (20)        0 2024-06-03 08:12:48.432883 pesummary-1.3.0/pesummary/gw/notebook/
+-rw-r--r--   0 charlie    (501) staff       (20)      151 2022-09-20 20:30:50.000000 pesummary-1.3.0/pesummary/gw/notebook/__init__.py
+-rw-r--r--   0 charlie    (501) staff       (20)     1188 2022-09-20 20:30:50.000000 pesummary-1.3.0/pesummary/gw/notebook/notebook.py
+-rw-r--r--   0 charlie    (501) staff       (20)     7067 2023-04-23 23:35:41.000000 pesummary-1.3.0/pesummary/gw/notebook/public.py
+drwxr-xr-x   0 charlie    (501) staff       (20)        0 2024-06-03 08:12:48.435248 pesummary-1.3.0/pesummary/gw/plots/
+-rw-r--r--   0 charlie    (501) staff       (20)      109 2022-09-22 09:35:49.000000 pesummary-1.3.0/pesummary/gw/plots/__init__.py
+-rw-r--r--   0 charlie    (501) staff       (20)     2666 2022-09-20 20:30:50.000000 pesummary-1.3.0/pesummary/gw/plots/bounds.py
+-rw-r--r--   0 charlie    (501) staff       (20)     2244 2022-09-22 09:35:49.000000 pesummary-1.3.0/pesummary/gw/plots/cmap.py
+-rw-r--r--   0 charlie    (501) staff       (20)     8714 2022-09-20 20:30:50.000000 pesummary-1.3.0/pesummary/gw/plots/cylon.csv
+-rw-r--r--   0 charlie    (501) staff       (20)     9876 2023-04-23 23:35:45.000000 pesummary-1.3.0/pesummary/gw/plots/detchar.py
+-rw-r--r--   0 charlie    (501) staff       (20)     7602 2024-06-03 08:08:38.000000 pesummary-1.3.0/pesummary/gw/plots/latex_labels.py
+-rw-r--r--   0 charlie    (501) staff       (20)    50441 2024-06-03 08:08:38.000000 pesummary-1.3.0/pesummary/gw/plots/main.py
+-rw-r--r--   0 charlie    (501) staff       (20)    51544 2024-06-03 08:08:38.000000 pesummary-1.3.0/pesummary/gw/plots/plot.py
+-rw-r--r--   0 charlie    (501) staff       (20)     3204 2022-09-20 20:30:50.000000 pesummary-1.3.0/pesummary/gw/plots/public.py
+-rw-r--r--   0 charlie    (501) staff       (20)    17311 2024-01-15 16:41:54.000000 pesummary-1.3.0/pesummary/gw/plots/publication.py
+-rw-r--r--   0 charlie    (501) staff       (20)     6012 2022-09-20 20:30:50.000000 pesummary-1.3.0/pesummary/gw/plots/tgr.py
+-rw-r--r--   0 charlie    (501) staff       (20)     5634 2024-06-03 08:08:38.000000 pesummary-1.3.0/pesummary/gw/pycbc.py
+-rw-r--r--   0 charlie    (501) staff       (20)     3553 2023-04-23 23:35:41.000000 pesummary-1.3.0/pesummary/gw/reweight.py
+-rw-r--r--   0 charlie    (501) staff       (20)    28491 2024-06-03 08:08:38.000000 pesummary-1.3.0/pesummary/gw/waveform.py
+drwxr-xr-x   0 charlie    (501) staff       (20)        0 2024-06-03 08:12:48.436008 pesummary-1.3.0/pesummary/gw/webpage/
+-rw-r--r--   0 charlie    (501) staff       (20)      109 2022-09-20 20:30:50.000000 pesummary-1.3.0/pesummary/gw/webpage/__init__.py
+-rw-r--r--   0 charlie    (501) staff       (20)    39389 2024-06-03 08:08:38.000000 pesummary-1.3.0/pesummary/gw/webpage/main.py
+-rw-r--r--   0 charlie    (501) staff       (20)     7405 2022-09-20 20:30:50.000000 pesummary-1.3.0/pesummary/gw/webpage/public.py
+-rw-r--r--   0 charlie    (501) staff       (20)    12756 2023-04-23 23:35:41.000000 pesummary-1.3.0/pesummary/gw/webpage/tgr.py
+drwxr-xr-x   0 charlie    (501) staff       (20)        0 2024-06-03 08:12:48.436581 pesummary-1.3.0/pesummary/io/
+-rw-r--r--   0 charlie    (501) staff       (20)     1244 2022-09-20 20:30:50.000000 pesummary-1.3.0/pesummary/io/__init__.py
+-rw-r--r--   0 charlie    (501) staff       (20)     3562 2022-09-20 20:30:50.000000 pesummary-1.3.0/pesummary/io/read.py
+-rw-r--r--   0 charlie    (501) staff       (20)     4510 2022-09-20 20:30:50.000000 pesummary-1.3.0/pesummary/io/write.py
+drwxr-xr-x   0 charlie    (501) staff       (20)        0 2024-06-03 08:12:48.447182 pesummary-1.3.0/pesummary/tests/
+-rw-r--r--   0 charlie    (501) staff       (20)      109 2022-09-20 20:30:50.000000 pesummary-1.3.0/pesummary/tests/__init__.py
+-rw-r--r--   0 charlie    (501) staff       (20)      329 2023-04-23 23:35:41.000000 pesummary-1.3.0/pesummary/tests/_bilby.sh
+-rw-r--r--   0 charlie    (501) staff       (20)     1949 2023-04-23 23:35:41.000000 pesummary-1.3.0/pesummary/tests/action_test.py
+-rw-r--r--   0 charlie    (501) staff       (20)    19441 2024-06-03 08:08:38.000000 pesummary-1.3.0/pesummary/tests/base.py
+-rw-r--r--   0 charlie    (501) staff       (20)      514 2023-04-23 23:35:41.000000 pesummary-1.3.0/pesummary/tests/bilby.sh
+-rw-r--r--   0 charlie    (501) staff       (20)      656 2023-04-23 23:35:41.000000 pesummary-1.3.0/pesummary/tests/bilby_mcmc.sh
+-rw-r--r--   0 charlie    (501) staff       (20)      933 2023-04-23 23:35:41.000000 pesummary-1.3.0/pesummary/tests/bilby_pipe.sh
+-rw-r--r--   0 charlie    (501) staff       (20)     1907 2024-01-15 16:41:54.000000 pesummary-1.3.0/pesummary/tests/bounded_kde_test.py
+-rw-r--r--   0 charlie    (501) staff       (20)     2703 2023-11-03 18:40:04.000000 pesummary-1.3.0/pesummary/tests/calibration_test.py
+-rw-r--r--   0 charlie    (501) staff       (20)     7528 2024-02-20 10:30:45.000000 pesummary-1.3.0/pesummary/tests/classification_test.py
+-rw-r--r--   0 charlie    (501) staff       (20)      430 2023-11-03 18:40:04.000000 pesummary-1.3.0/pesummary/tests/conftest.py
+-rw-r--r--   0 charlie    (501) staff       (20)    47756 2024-02-20 10:30:45.000000 pesummary-1.3.0/pesummary/tests/conversion_test.py
+-rw-r--r--   0 charlie    (501) staff       (20)     3026 2022-09-20 20:30:50.000000 pesummary-1.3.0/pesummary/tests/cosmology_test.py
+-rw-r--r--   0 charlie    (501) staff       (20)       94 2022-09-20 20:30:50.000000 pesummary-1.3.0/pesummary/tests/example_config.ini
+-rw-r--r--   0 charlie    (501) staff       (20)    90223 2024-02-20 10:30:45.000000 pesummary-1.3.0/pesummary/tests/executable_test.py
+-rw-r--r--   0 charlie    (501) staff       (20)     1076 2022-09-20 20:30:50.000000 pesummary-1.3.0/pesummary/tests/executables.sh
+-rw-r--r--   0 charlie    (501) staff       (20)     1626 2022-09-20 20:30:50.000000 pesummary-1.3.0/pesummary/tests/existing_file.py
+-rw-r--r--   0 charlie    (501) staff       (20)     4676 2024-02-20 10:30:45.000000 pesummary-1.3.0/pesummary/tests/fetch_test.py
+drwxr-xr-x   0 charlie    (501) staff       (20)        0 2024-06-03 08:12:48.450876 pesummary-1.3.0/pesummary/tests/files/
+-rw-r--r--   0 charlie    (501) staff       (20)       55 2022-09-20 20:30:50.000000 pesummary-1.3.0/pesummary/tests/files/.gitattributes
+-rw-r--r--   0 charlie    (501) staff       (20)   843570 2022-09-20 20:30:50.000000 pesummary-1.3.0/pesummary/tests/files/calibration_envelope.txt
+-rw-r--r--   0 charlie    (501) staff       (20)      545 2022-09-20 20:30:50.000000 pesummary-1.3.0/pesummary/tests/files/config_bilby.ini
+-rw-r--r--   0 charlie    (501) staff       (20)     3576 2022-09-20 20:30:50.000000 pesummary-1.3.0/pesummary/tests/files/config_lalinference.ini
+-rw-r--r--   0 charlie    (501) staff       (20)       19 2022-09-20 20:30:50.000000 pesummary-1.3.0/pesummary/tests/files/example.ini
+-rw-r--r--   0 charlie    (501) staff       (20)   264597 2022-09-20 20:30:50.000000 pesummary-1.3.0/pesummary/tests/files/lal_pdf_for_summarytgr.dat.gz
+-rw-r--r--   0 charlie    (501) staff       (20)    96127 2022-09-20 20:30:50.000000 pesummary-1.3.0/pesummary/tests/files/psd_file.txt
+-rw-r--r--   0 charlie    (501) staff       (20)     1264 2023-11-03 18:40:04.000000 pesummary-1.3.0/pesummary/tests/finish_test.py
+-rw-r--r--   0 charlie    (501) staff       (20)     1152 2022-09-20 20:30:50.000000 pesummary-1.3.0/pesummary/tests/imports.sh
+-rw-r--r--   0 charlie    (501) staff       (20)     2470 2023-11-03 18:40:04.000000 pesummary-1.3.0/pesummary/tests/injection_test.py
+-rw-r--r--   0 charlie    (501) staff       (20)    29256 2023-11-03 18:40:04.000000 pesummary-1.3.0/pesummary/tests/input_test.py
+-rw-r--r--   0 charlie    (501) staff       (20)     1875 2022-09-20 20:30:50.000000 pesummary-1.3.0/pesummary/tests/lalinference.sh
+-rw-r--r--   0 charlie    (501) staff       (20)     2461 2022-09-20 20:30:50.000000 pesummary-1.3.0/pesummary/tests/ligo_skymap_test.py
+-rw-r--r--   0 charlie    (501) staff       (20)    12707 2022-09-20 20:30:50.000000 pesummary-1.3.0/pesummary/tests/main_injection.xml
+-rw-r--r--   0 charlie    (501) staff       (20)       69 2022-09-20 20:30:50.000000 pesummary-1.3.0/pesummary/tests/main_input.ini
+-rw-r--r--   0 charlie    (501) staff       (20)       33 2022-09-20 20:30:50.000000 pesummary-1.3.0/pesummary/tests/main_input_core.ini
+-rw-r--r--   0 charlie    (501) staff       (20)    19886 2023-11-03 18:40:04.000000 pesummary-1.3.0/pesummary/tests/meta_file_test.py
+-rw-r--r--   0 charlie    (501) staff       (20)     1501 2023-11-03 18:40:04.000000 pesummary-1.3.0/pesummary/tests/notebook_test.py
+-rw-r--r--   0 charlie    (501) staff       (20)    20225 2023-11-03 18:40:04.000000 pesummary-1.3.0/pesummary/tests/plot_test.py
+-rw-r--r--   0 charlie    (501) staff       (20)     4804 2024-06-03 08:08:38.000000 pesummary-1.3.0/pesummary/tests/psd_test.py
+-rw-r--r--   0 charlie    (501) staff       (20)      665 2024-06-03 08:08:38.000000 pesummary-1.3.0/pesummary/tests/pycbc.sh
+-rw-r--r--   0 charlie    (501) staff       (20)     4937 2023-11-03 18:40:04.000000 pesummary-1.3.0/pesummary/tests/pycbc_test.py
+-rw-r--r--   0 charlie    (501) staff       (20)    75787 2023-11-03 18:40:04.000000 pesummary-1.3.0/pesummary/tests/read_test.py
+-rw-r--r--   0 charlie    (501) staff       (20)     3482 2022-09-20 20:30:50.000000 pesummary-1.3.0/pesummary/tests/reweight_test.py
+-rw-r--r--   0 charlie    (501) staff       (20)     3242 2022-09-20 20:30:50.000000 pesummary-1.3.0/pesummary/tests/strain_test.py
+-rw-r--r--   0 charlie    (501) staff       (20)    10603 2024-06-03 08:08:38.000000 pesummary-1.3.0/pesummary/tests/summaryplots_test.py
+-rw-r--r--   0 charlie    (501) staff       (20)    52125 2024-02-20 10:30:45.000000 pesummary-1.3.0/pesummary/tests/utils_test.py
+-rw-r--r--   0 charlie    (501) staff       (20)     8486 2023-11-03 18:40:04.000000 pesummary-1.3.0/pesummary/tests/waveform_test.py
+-rw-r--r--   0 charlie    (501) staff       (20)    11505 2024-01-15 16:41:54.000000 pesummary-1.3.0/pesummary/tests/webpage_test.py
+-rw-r--r--   0 charlie    (501) staff       (20)    21589 2023-11-03 18:40:04.000000 pesummary-1.3.0/pesummary/tests/workflow_test.py
+-rw-r--r--   0 charlie    (501) staff       (20)     7524 2023-11-03 18:40:04.000000 pesummary-1.3.0/pesummary/tests/write_test.py
+drwxr-xr-x   0 charlie    (501) staff       (20)        0 2024-06-03 08:12:48.455254 pesummary-1.3.0/pesummary/utils/
+-rw-r--r--   0 charlie    (501) staff       (20)      240 2023-04-23 23:35:41.000000 pesummary-1.3.0/pesummary/utils/__init__.py
+-rw-r--r--   0 charlie    (501) staff       (20)    10853 2024-02-20 10:30:45.000000 pesummary-1.3.0/pesummary/utils/array.py
+-rw-r--r--   0 charlie    (501) staff       (20)     8888 2024-01-15 16:41:54.000000 pesummary-1.3.0/pesummary/utils/bounded_1d_kde.py
+-rw-r--r--   0 charlie    (501) staff       (20)     3624 2024-01-15 16:41:54.000000 pesummary-1.3.0/pesummary/utils/bounded_2d_kde.py
+-rw-r--r--   0 charlie    (501) staff       (20)     6015 2024-02-20 10:30:45.000000 pesummary-1.3.0/pesummary/utils/credible_interval.py
+-rw-r--r--   0 charlie    (501) staff       (20)     9966 2024-06-03 08:08:38.000000 pesummary-1.3.0/pesummary/utils/decorators.py
+-rw-r--r--   0 charlie    (501) staff       (20)     8392 2022-09-20 20:30:50.000000 pesummary-1.3.0/pesummary/utils/dict.py
+-rw-r--r--   0 charlie    (501) staff       (20)      507 2022-09-20 20:30:50.000000 pesummary-1.3.0/pesummary/utils/exceptions.py
+-rw-r--r--   0 charlie    (501) staff       (20)     2316 2024-01-15 16:41:54.000000 pesummary-1.3.0/pesummary/utils/kde_list.py
+-rw-r--r--   0 charlie    (501) staff       (20)     2993 2022-09-20 20:30:50.000000 pesummary-1.3.0/pesummary/utils/list.py
+-rw-r--r--   0 charlie    (501) staff       (20)     3187 2022-09-20 20:30:50.000000 pesummary-1.3.0/pesummary/utils/parameters.py
+-rw-r--r--   0 charlie    (501) staff       (20)    16638 2024-01-19 09:12:30.000000 pesummary-1.3.0/pesummary/utils/pdf.py
+-rw-r--r--   0 charlie    (501) staff       (20)     9255 2022-09-20 20:30:50.000000 pesummary-1.3.0/pesummary/utils/probability_dict.py
+-rw-r--r--   0 charlie    (501) staff       (20)    76439 2024-02-20 10:30:45.000000 pesummary-1.3.0/pesummary/utils/samples_dict.py
+-rw-r--r--   0 charlie    (501) staff       (20)     2991 2022-09-20 20:30:50.000000 pesummary-1.3.0/pesummary/utils/tqdm.py
+-rw-r--r--   0 charlie    (501) staff       (20)    35507 2024-01-15 16:41:54.000000 pesummary-1.3.0/pesummary/utils/utils.py
+drwxr-xr-x   0 charlie    (501) staff       (20)        0 2024-06-03 08:12:48.455614 pesummary-1.3.0/pesummary.egg-info/
+-rw-r--r--   0 charlie    (501) staff       (20)     4562 2024-06-03 08:12:48.000000 pesummary-1.3.0/pesummary.egg-info/PKG-INFO
+-rw-r--r--   0 charlie    (501) staff       (20)    13564 2024-06-03 08:12:48.000000 pesummary-1.3.0/pesummary.egg-info/SOURCES.txt
+-rw-r--r--   0 charlie    (501) staff       (20)        1 2024-06-03 08:12:48.000000 pesummary-1.3.0/pesummary.egg-info/dependency_links.txt
+-rw-r--r--   0 charlie    (501) staff       (20)     1099 2024-06-03 08:12:48.000000 pesummary-1.3.0/pesummary.egg-info/entry_points.txt
+-rw-r--r--   0 charlie    (501) staff       (20)      720 2024-06-03 08:12:48.000000 pesummary-1.3.0/pesummary.egg-info/requires.txt
+-rw-r--r--   0 charlie    (501) staff       (20)       10 2024-06-03 08:12:48.000000 pesummary-1.3.0/pesummary.egg-info/top_level.txt
+-rw-r--r--   0 charlie    (501) staff       (20)     4430 2024-06-03 08:08:38.000000 pesummary-1.3.0/pyproject.toml
+-rw-r--r--   0 charlie    (501) staff       (20)       38 2024-06-03 08:12:48.458567 pesummary-1.3.0/setup.cfg
+-rw-r--r--   0 charlie    (501) staff       (20)     1337 2022-09-20 20:30:50.000000 pesummary-1.3.0/setup.py
```

### Comparing `pesummary-1.2.0/.gitignore` & `pesummary-1.3.0/.gitignore`

 * *Files identical despite different names*

### Comparing `pesummary-1.2.0/.gitlab-ci.yml` & `pesummary-1.3.0/.gitlab-ci.yml`

 * *Files identical despite different names*

### Comparing `pesummary-1.2.0/CHANGELOG.md` & `pesummary-1.3.0/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `pesummary-1.2.0/CONTRIBUTING.md` & `pesummary-1.3.0/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `pesummary-1.2.0/LICENSE.md` & `pesummary-1.3.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `pesummary-1.2.0/PKG-INFO` & `pesummary-1.3.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pesummary
-Version: 1.2.0
+Version: 1.3.0
 Summary: Python package to produce summary pages for Parameter estimation codes
 Author-email: Charlie Hoy <charlie.hoy@ligo.org>
 License: MIT
 Project-URL: Homepage, https://lscsoft.docs.ligo.org/pesummary
 Project-URL: Documentation, https://lscsoft.docs.ligo.org/pesummary/
 Project-URL: Issue Tracker, https://git.ligo.org/lscsoft/pesummary/-/issues/
 Project-URL: Source Code, https://git.ligo.org/lscsoft/pesummary.git
@@ -35,28 +35,29 @@
 Requires-Dist: statsmodels
 Requires-Dist: scipy>=1.8.0
 Requires-Dist: tables
 Requires-Dist: tqdm>=4.44.0
 Provides-Extra: docs
 Requires-Dist: ipykernel; extra == "docs"
 Requires-Dist: nbsphinx; extra == "docs"
+Requires-Dist: pycbc; extra == "docs"
 Requires-Dist: requests; extra == "docs"
 Requires-Dist: Sphinx!=5.0.0,>=4.0.0; extra == "docs"
 Requires-Dist: sphinx-argparse; extra == "docs"
 Requires-Dist: sphinx_rtd_theme; extra == "docs"
 Requires-Dist: sphinx-panels; extra == "docs"
 Requires-Dist: sphinxcontrib-programoutput; extra == "docs"
 Provides-Extra: lint
 Requires-Dist: flake8>=3.7.0; extra == "lint"
 Requires-Dist: flake8-bandit; extra == "lint"
 Provides-Extra: test
 Requires-Dist: astropy!=4.3.0,>=4.0; extra == "test"
 Requires-Dist: beautifulsoup4; extra == "test"
 Requires-Dist: bilby_pipe; extra == "test"
-Requires-Dist: coverage; extra == "test"
+Requires-Dist: coverage<=7.4.4; extra == "test"
 Requires-Dist: coverage-badge; extra == "test"
 Requires-Dist: cython>=0.28.5; extra == "test"
 Requires-Dist: markupsafe==2.0.1; extra == "test"
 Requires-Dist: pycbc>=2.0.3; extra == "test"
 Requires-Dist: pytest>=3.0.0; extra == "test"
 Requires-Dist: pytest-xdist; extra == "test"
 Requires-Dist: pytest-rerunfailures; extra == "test"
```

### Comparing `pesummary-1.2.0/README.md` & `pesummary-1.3.0/README.md`

 * *Files identical despite different names*

### Comparing `pesummary-1.2.0/containers/Dockerfile-template` & `pesummary-1.3.0/containers/Dockerfile-template`

 * *Files identical despite different names*

### Comparing `pesummary-1.2.0/containers/write_dockerfile.py` & `pesummary-1.3.0/containers/write_dockerfile.py`

 * *Files identical despite different names*

### Comparing `pesummary-1.2.0/docs/citing_pesummary.rst` & `pesummary-1.3.0/docs/citing_pesummary.rst`

 * *Files identical despite different names*

### Comparing `pesummary-1.2.0/docs/conf/configuration.rst` & `pesummary-1.3.0/docs/conf/configuration.rst`

 * *Files identical despite different names*

### Comparing `pesummary-1.2.0/docs/conf.py` & `pesummary-1.3.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `pesummary-1.2.0/docs/core/Array.rst` & `pesummary-1.3.0/docs/core/Array.rst`

 * *Files identical despite different names*

### Comparing `pesummary-1.2.0/docs/core/MCMCSamplesDict.rst` & `pesummary-1.3.0/docs/core/MCMCSamplesDict.rst`

 * *Files identical despite different names*

### Comparing `pesummary-1.2.0/docs/core/MultiAnalysisSamplesDict.rst` & `pesummary-1.3.0/docs/core/MultiAnalysisSamplesDict.rst`

 * *Files identical despite different names*

### Comparing `pesummary-1.2.0/docs/core/SamplesDict.rst` & `pesummary-1.3.0/docs/core/SamplesDict.rst`

 * *Files identical despite different names*

### Comparing `pesummary-1.2.0/docs/core/bounded_kdes.rst` & `pesummary-1.3.0/docs/core/bounded_kdes.rst`

 * *Files identical despite different names*

### Comparing `pesummary-1.2.0/docs/core/cli/summaryclean.rst` & `pesummary-1.3.0/docs/core/cli/summaryclean.rst`

 * *Files identical despite different names*

### Comparing `pesummary-1.2.0/docs/core/cli/summarycombine.rst` & `pesummary-1.3.0/docs/core/cli/summarycombine.rst`

 * *Files identical despite different names*

### Comparing `pesummary-1.2.0/docs/core/cli/summarycombine_posteriors.rst` & `pesummary-1.3.0/docs/core/cli/summarycombine_posteriors.rst`

 * *Files identical despite different names*

### Comparing `pesummary-1.2.0/docs/core/cli/summarycompare.rst` & `pesummary-1.3.0/docs/core/cli/summarycompare.rst`

 * *Files identical despite different names*

### Comparing `pesummary-1.2.0/docs/core/cli/summarypages.rst` & `pesummary-1.3.0/docs/core/cli/summarypages.rst`

 * *Files identical despite different names*

### Comparing `pesummary-1.2.0/docs/core/cli/summarypageslw.rst` & `pesummary-1.3.0/docs/core/cli/summarypageslw.rst`

 * *Files identical despite different names*

### Comparing `pesummary-1.2.0/docs/core/cli/summarypublication.rst` & `pesummary-1.3.0/docs/core/cli/summarypublication.rst`

 * *Files identical despite different names*

### Comparing `pesummary-1.2.0/docs/core/file_formats.rst` & `pesummary-1.3.0/docs/core/file_formats.rst`

 * *Files identical despite different names*

### Comparing `pesummary-1.2.0/docs/core/index.rst` & `pesummary-1.3.0/docs/core/index.rst`

 * *Files identical despite different names*

### Comparing `pesummary-1.2.0/docs/core/pdf.rst` & `pesummary-1.3.0/docs/core/pdf.rst`

 * *Files identical despite different names*

### Comparing `pesummary-1.2.0/docs/core/pesummary_file.rst` & `pesummary-1.3.0/docs/core/pesummary_file.rst`

 * *Files identical despite different names*

### Comparing `pesummary-1.2.0/docs/core/read.rst` & `pesummary-1.3.0/docs/core/read.rst`

 * *Files identical despite different names*

### Comparing `pesummary-1.2.0/docs/core/tutorials/plotting_from_metafile.rst` & `pesummary-1.3.0/docs/core/tutorials/plotting_from_metafile.rst`

 * *Files identical despite different names*

### Comparing `pesummary-1.2.0/docs/core/write.rst` & `pesummary-1.3.0/docs/core/write.rst`

 * *Files identical despite different names*

### Comparing `pesummary-1.2.0/docs/front.html.in` & `pesummary-1.3.0/docs/front.html.in`

 * *Files identical despite different names*

### Comparing `pesummary-1.2.0/docs/gw/Conversion.rst` & `pesummary-1.3.0/docs/gw/Conversion.rst`

 * *Files identical despite different names*

### Comparing `pesummary-1.2.0/docs/gw/SamplesDict.rst` & `pesummary-1.3.0/docs/gw/SamplesDict.rst`

 * *Files identical despite different names*

### Comparing `pesummary-1.2.0/docs/gw/calibration.rst` & `pesummary-1.3.0/docs/gw/calibration.rst`

 * *Files identical despite different names*

### Comparing `pesummary-1.2.0/docs/gw/classification.rst` & `pesummary-1.3.0/docs/gw/classification.rst`

 * *Files identical despite different names*

### Comparing `pesummary-1.2.0/docs/gw/cli/summaryclassification.rst` & `pesummary-1.3.0/docs/gw/cli/summaryclassification.rst`

 * *Files identical despite different names*

### Comparing `pesummary-1.2.0/docs/gw/cli/summarydetchar.rst` & `pesummary-1.3.0/docs/gw/cli/summarydetchar.rst`

 * *Files identical despite different names*

### Comparing `pesummary-1.2.0/docs/gw/cli/summarygracedb.rst` & `pesummary-1.3.0/docs/gw/cli/summarygracedb.rst`

 * *Files identical despite different names*

### Comparing `pesummary-1.2.0/docs/gw/cli/summarypipe.rst` & `pesummary-1.3.0/docs/gw/cli/summarypipe.rst`

 * *Files identical despite different names*

### Comparing `pesummary-1.2.0/docs/gw/cli/summaryrecreate.rst` & `pesummary-1.3.0/docs/gw/cli/summaryrecreate.rst`

 * *Files identical despite different names*

### Comparing `pesummary-1.2.0/docs/gw/cli/summaryreview.rst` & `pesummary-1.3.0/docs/gw/cli/summaryreview.rst`

 * *Files identical despite different names*

### Comparing `pesummary-1.2.0/docs/gw/cli/summarytgr.rst` & `pesummary-1.3.0/docs/gw/cli/summarytgr.rst`

 * *Files identical despite different names*

### Comparing `pesummary-1.2.0/docs/gw/fetch.rst` & `pesummary-1.3.0/docs/gw/fetch.rst`

 * *Files identical despite different names*

### Comparing `pesummary-1.2.0/docs/gw/file_formats.rst` & `pesummary-1.3.0/docs/gw/file_formats.rst`

 * *Files identical despite different names*

### Comparing `pesummary-1.2.0/docs/gw/index.rst` & `pesummary-1.3.0/docs/gw/index.rst`

 * *Files 4% similar despite different names*

```diff
@@ -91,14 +91,15 @@
 
 .. toctree::
     :maxdepth: 1
 
     ../core/seaborn
     ../core/bounded_kdes
     violin
+    corner
     tutorials/comparing_public_data_files
     tutorials/plotting_from_metafile
     tutorials/population_scatter_plot_GWTC-1
     tutorials/GWTC1_plots
     tutorials/interaction_with_ligo_skymap
     tutorials/plot_waveform_on_strain_data
```

### Comparing `pesummary-1.2.0/docs/gw/pesummary_file.rst` & `pesummary-1.3.0/docs/gw/pesummary_file.rst`

 * *Files identical despite different names*

### Comparing `pesummary-1.2.0/docs/gw/psd.rst` & `pesummary-1.3.0/docs/gw/psd.rst`

 * *Files identical despite different names*

### Comparing `pesummary-1.2.0/docs/gw/read.rst` & `pesummary-1.3.0/docs/gw/read.rst`

 * *Files identical despite different names*

### Comparing `pesummary-1.2.0/docs/gw/remnant_fits.rst` & `pesummary-1.3.0/docs/gw/remnant_fits.rst`

 * *Files identical despite different names*

### Comparing `pesummary-1.2.0/docs/gw/strain.rst` & `pesummary-1.3.0/docs/gw/strain.rst`

 * *Files identical despite different names*

### Comparing `pesummary-1.2.0/docs/gw/summarypages/IMRPhenomPv3HM/classification.rst` & `pesummary-1.3.0/docs/gw/summarypages/IMRPhenomPv3HM/classification.rst`

 * *Files identical despite different names*

### Comparing `pesummary-1.2.0/docs/gw/summarypages/IMRPhenomPv3HM/corner.rst` & `pesummary-1.3.0/docs/gw/summarypages/IMRPhenomPv3HM/corner.rst`

 * *Files identical despite different names*

### Comparing `pesummary-1.2.0/docs/gw/summarypages/IMRPhenomPv3HM/examples/.gitattributes` & `pesummary-1.3.0/docs/gw/summarypages/IMRPhenomPv3HM/examples/.gitattributes`

 * *Files identical despite different names*

### Comparing `pesummary-1.2.0/docs/gw/summarypages/IMRPhenomPv3HM/home.rst` & `pesummary-1.3.0/docs/gw/summarypages/IMRPhenomPv3HM/home.rst`

 * *Files identical despite different names*

### Comparing `pesummary-1.2.0/docs/gw/summarypages/IMRPhenomPv3HM/interactive.rst` & `pesummary-1.3.0/docs/gw/summarypages/IMRPhenomPv3HM/interactive.rst`

 * *Files identical despite different names*

### Comparing `pesummary-1.2.0/docs/gw/summarypages/IMRPhenomPv3HM/mass_1.rst` & `pesummary-1.3.0/docs/gw/summarypages/IMRPhenomPv3HM/mass_1.rst`

 * *Files identical despite different names*

### Comparing `pesummary-1.2.0/docs/gw/summarypages/comparison/examples/interactive_ridgeline.html` & `pesummary-1.3.0/docs/gw/summarypages/comparison/examples/interactive_ridgeline.html`

 * *Files identical despite different names*

### Comparing `pesummary-1.2.0/docs/gw/summarypages/comparison/home.rst` & `pesummary-1.3.0/docs/gw/summarypages/comparison/home.rst`

 * *Files identical despite different names*

### Comparing `pesummary-1.2.0/docs/gw/summarypages/comparison/interactive.rst` & `pesummary-1.3.0/docs/gw/summarypages/comparison/interactive.rst`

 * *Files identical despite different names*

### Comparing `pesummary-1.2.0/docs/gw/summarypages/comparison/mass_1.rst` & `pesummary-1.3.0/docs/gw/summarypages/comparison/mass_1.rst`

 * *Files identical despite different names*

### Comparing `pesummary-1.2.0/docs/gw/summarypages/downloads.rst` & `pesummary-1.3.0/docs/gw/summarypages/downloads.rst`

 * *Files identical despite different names*

### Comparing `pesummary-1.2.0/docs/gw/summarypages/home.rst` & `pesummary-1.3.0/docs/gw/summarypages/home.rst`

 * *Files identical despite different names*

### Comparing `pesummary-1.2.0/docs/gw/summarypages/version.rst` & `pesummary-1.3.0/docs/gw/summarypages/version.rst`

 * *Files identical despite different names*

### Comparing `pesummary-1.2.0/docs/gw/tgr_file.rst` & `pesummary-1.3.0/docs/gw/tgr_file.rst`

 * *Files identical despite different names*

### Comparing `pesummary-1.2.0/docs/gw/tutorials/GWTC1_plots.rst` & `pesummary-1.3.0/docs/gw/tutorials/GWTC1_plots.rst`

 * *Files identical despite different names*

### Comparing `pesummary-1.2.0/docs/gw/tutorials/comparing_public_data_files.rst` & `pesummary-1.3.0/docs/gw/tutorials/comparing_public_data_files.rst`

 * *Files identical despite different names*

### Comparing `pesummary-1.2.0/docs/gw/tutorials/conversions_and_condor.rst` & `pesummary-1.3.0/docs/gw/tutorials/conversions_and_condor.rst`

 * *Files identical despite different names*

### Comparing `pesummary-1.2.0/docs/gw/tutorials/examples/.gitattributes` & `pesummary-1.3.0/docs/gw/tutorials/examples/.gitattributes`

 * *Files identical despite different names*

### Comparing `pesummary-1.2.0/docs/gw/tutorials/interaction_with_ligo_skymap.rst` & `pesummary-1.3.0/docs/gw/tutorials/interaction_with_ligo_skymap.rst`

 * *Files identical despite different names*

### Comparing `pesummary-1.2.0/docs/gw/tutorials/make_your_own_page_from_metafile.rst` & `pesummary-1.3.0/docs/gw/tutorials/make_your_own_page_from_metafile.rst`

 * *Files identical despite different names*

### Comparing `pesummary-1.2.0/docs/gw/tutorials/plot_waveform_on_strain_data.rst` & `pesummary-1.3.0/docs/gw/tutorials/plot_waveform_on_strain_data.rst`

 * *Files identical despite different names*

### Comparing `pesummary-1.2.0/docs/gw/tutorials/plotting_from_metafile.rst` & `pesummary-1.3.0/docs/gw/tutorials/plotting_from_metafile.rst`

 * *Files identical despite different names*

### Comparing `pesummary-1.2.0/docs/gw/tutorials/population_scatter_plot_GWTC-1.rst` & `pesummary-1.3.0/docs/gw/tutorials/population_scatter_plot_GWTC-1.rst`

 * *Files identical despite different names*

### Comparing `pesummary-1.2.0/docs/gw/tutorials/public_pages.rst` & `pesummary-1.3.0/docs/gw/tutorials/public_pages.rst`

 * *Files identical despite different names*

### Comparing `pesummary-1.2.0/docs/gw/tutorials/release_notebook.rst` & `pesummary-1.3.0/docs/gw/tutorials/release_notebook.rst`

 * *Files identical despite different names*

### Comparing `pesummary-1.2.0/docs/gw/tutorials/waveforms.rst` & `pesummary-1.3.0/docs/gw/tutorials/waveforms.rst`

 * *Files identical despite different names*

### Comparing `pesummary-1.2.0/docs/gw/violin.rst` & `pesummary-1.3.0/docs/gw/violin.rst`

 * *Files identical despite different names*

### Comparing `pesummary-1.2.0/docs/index.rst` & `pesummary-1.3.0/docs/index.rst`

 * *Files identical despite different names*

### Comparing `pesummary-1.2.0/docs/installation.rst` & `pesummary-1.3.0/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `pesummary-1.2.0/docs/io/read.rst` & `pesummary-1.3.0/docs/io/read.rst`

 * *Files identical despite different names*

### Comparing `pesummary-1.2.0/docs/virtual_environment.rst` & `pesummary-1.3.0/docs/virtual_environment.rst`

 * *Files identical despite different names*

### Comparing `pesummary-1.2.0/docs/what_is_pesummary.rst` & `pesummary-1.3.0/docs/what_is_pesummary.rst`

 * *Files identical despite different names*

### Comparing `pesummary-1.2.0/examples/core/bounded_kdeplot.py` & `pesummary-1.3.0/examples/core/bounded_kdeplot.py`

 * *Files identical despite different names*

### Comparing `pesummary-1.2.0/examples/core/extract_information_from_pesummary_file.py` & `pesummary-1.3.0/examples/core/extract_information_from_pesummary_file.py`

 * *Files identical despite different names*

### Comparing `pesummary-1.2.0/examples/core/multiple_analysis_custom_read.py` & `pesummary-1.3.0/examples/core/multiple_analysis_custom_read.py`

 * *Files identical despite different names*

### Comparing `pesummary-1.2.0/examples/core/pesummary_data_structure.txt` & `pesummary-1.3.0/examples/core/pesummary_data_structure.txt`

 * *Files identical despite different names*

### Comparing `pesummary-1.2.0/examples/core/single_analysis_custom_read.py` & `pesummary-1.3.0/examples/core/single_analysis_custom_read.py`

 * *Files identical despite different names*

### Comparing `pesummary-1.2.0/examples/custom_plot.py` & `pesummary-1.3.0/examples/custom_plot.py`

 * *Files identical despite different names*

### Comparing `pesummary-1.2.0/examples/extract_information_without_pesummary.py` & `pesummary-1.3.0/examples/extract_information_without_pesummary.py`

 * *Files identical despite different names*

### Comparing `pesummary-1.2.0/examples/gw/GWTC-1_population_scatterplot.sh` & `pesummary-1.3.0/examples/gw/GWTC-1_population_scatterplot.sh`

 * *Files identical despite different names*

### Comparing `pesummary-1.2.0/examples/gw/GWTC1_plots.sh` & `pesummary-1.3.0/examples/gw/GWTC1_plots.sh`

 * *Files identical despite different names*

### Comparing `pesummary-1.2.0/examples/gw/compare_GW150914.py` & `pesummary-1.3.0/examples/gw/compare_GW150914.py`

 * *Files identical despite different names*

### Comparing `pesummary-1.2.0/examples/gw/extract_information_from_pesummary_file.py` & `pesummary-1.3.0/examples/gw/extract_information_from_pesummary_file.py`

 * *Files identical despite different names*

### Comparing `pesummary-1.2.0/examples/gw/extract_information_from_pesummary_file_without_pesummary.py` & `pesummary-1.3.0/examples/gw/extract_information_from_pesummary_file_without_pesummary.py`

 * *Files identical despite different names*

### Comparing `pesummary-1.2.0/examples/gw/fetch_open_data.py` & `pesummary-1.3.0/examples/gw/fetch_open_data.py`

 * *Files identical despite different names*

### Comparing `pesummary-1.2.0/examples/gw/fetch_open_strain.py` & `pesummary-1.3.0/examples/gw/fetch_open_strain.py`

 * *Files identical despite different names*

### Comparing `pesummary-1.2.0/examples/gw/latex.py` & `pesummary-1.3.0/examples/gw/latex.py`

 * *Files identical despite different names*

### Comparing `pesummary-1.2.0/examples/gw/ligo_skymap.py` & `pesummary-1.3.0/examples/gw/ligo_skymap.py`

 * *Files identical despite different names*

### Comparing `pesummary-1.2.0/examples/gw/make_public_release.py` & `pesummary-1.3.0/examples/gw/make_public_release.py`

 * *Files identical despite different names*

### Comparing `pesummary-1.2.0/examples/gw/making_a_waveform_in_frequency_domain.py` & `pesummary-1.3.0/examples/gw/making_a_waveform_in_frequency_domain.py`

 * *Files identical despite different names*

### Comparing `pesummary-1.2.0/examples/gw/making_a_waveform_in_time_domain.py` & `pesummary-1.3.0/examples/gw/making_a_waveform_in_time_domain.py`

 * *Files identical despite different names*

### Comparing `pesummary-1.2.0/examples/gw/making_a_waveform_in_time_domain_with_uncertainty.py` & `pesummary-1.3.0/examples/gw/making_a_waveform_in_time_domain_with_uncertainty.py`

 * *Files identical despite different names*

### Comparing `pesummary-1.2.0/examples/gw/pesummary_data_structure.txt` & `pesummary-1.3.0/examples/gw/pesummary_data_structure.txt`

 * *Files identical despite different names*

### Comparing `pesummary-1.2.0/examples/gw/plot_waveform_on_strain_data_GW150914.py` & `pesummary-1.3.0/examples/gw/plot_waveform_on_strain_data_GW150914.py`

 * *Files identical despite different names*

### Comparing `pesummary-1.2.0/examples/gw/plot_waveform_on_strain_data_GW190814.py` & `pesummary-1.3.0/examples/gw/plot_waveform_on_strain_data_GW190814.py`

 * *Files identical despite different names*

### Comparing `pesummary-1.2.0/examples/gw/prior_conditioning.py` & `pesummary-1.3.0/examples/gw/prior_conditioning.py`

 * *Files identical despite different names*

### Comparing `pesummary-1.2.0/examples/gw/violin_plots.py` & `pesummary-1.3.0/examples/gw/violin_plots.py`

 * *Files identical despite different names*

### Comparing `pesummary-1.2.0/examples/run_with_python.py` & `pesummary-1.3.0/examples/run_with_python.py`

 * *Files identical despite different names*

### Comparing `pesummary-1.2.0/pesummary/__init__.py` & `pesummary-1.3.0/pesummary/__init__.py`

 * *Files identical despite different names*

### Comparing `pesummary-1.2.0/pesummary/_version_helper.py` & `pesummary-1.3.0/pesummary/_version_helper.py`

 * *Files identical despite different names*

### Comparing `pesummary-1.2.0/pesummary/cli/summaryclassification.py` & `pesummary-1.3.0/pesummary/cli/summaryclassification.py`

 * *Files identical despite different names*

### Comparing `pesummary-1.2.0/pesummary/cli/summaryclean.py` & `pesummary-1.3.0/pesummary/cli/summaryclean.py`

 * *Files identical despite different names*

### Comparing `pesummary-1.2.0/pesummary/cli/summarycombine.py` & `pesummary-1.3.0/pesummary/cli/summarycombine.py`

 * *Files identical despite different names*

### Comparing `pesummary-1.2.0/pesummary/cli/summarycombine_posteriors.py` & `pesummary-1.3.0/pesummary/cli/summarycombine_posteriors.py`

 * *Files identical despite different names*

### Comparing `pesummary-1.2.0/pesummary/cli/summarycompare.py` & `pesummary-1.3.0/pesummary/cli/summarycompare.py`

 * *Files identical despite different names*

### Comparing `pesummary-1.2.0/pesummary/cli/summarydetchar.py` & `pesummary-1.3.0/pesummary/cli/summarydetchar.py`

 * *Files identical despite different names*

### Comparing `pesummary-1.2.0/pesummary/cli/summaryextract.py` & `pesummary-1.3.0/pesummary/cli/summaryextract.py`

 * *Files identical despite different names*

### Comparing `pesummary-1.2.0/pesummary/cli/summarygracedb.py` & `pesummary-1.3.0/pesummary/cli/summarygracedb.py`

 * *Files identical despite different names*

### Comparing `pesummary-1.2.0/pesummary/cli/summaryjscompare.py` & `pesummary-1.3.0/pesummary/cli/summaryjscompare.py`

 * *Files identical despite different names*

### Comparing `pesummary-1.2.0/pesummary/cli/summarymodify.py` & `pesummary-1.3.0/pesummary/cli/summarymodify.py`

 * *Files identical despite different names*

### Comparing `pesummary-1.2.0/pesummary/cli/summarypages.py` & `pesummary-1.3.0/pesummary/cli/summarypages.py`

 * *Files identical despite different names*

### Comparing `pesummary-1.2.0/pesummary/cli/summarypageslw.py` & `pesummary-1.3.0/pesummary/cli/summarypageslw.py`

 * *Files identical despite different names*

### Comparing `pesummary-1.2.0/pesummary/cli/summarypipe.py` & `pesummary-1.3.0/pesummary/cli/summarypipe.py`

 * *Files identical despite different names*

### Comparing `pesummary-1.2.0/pesummary/cli/summaryplots.py` & `pesummary-1.3.0/pesummary/cli/summaryplots.py`

 * *Files identical despite different names*

### Comparing `pesummary-1.2.0/pesummary/cli/summarypublication.py` & `pesummary-1.3.0/pesummary/cli/summarypublication.py`

 * *Files identical despite different names*

### Comparing `pesummary-1.2.0/pesummary/cli/summaryrecreate.py` & `pesummary-1.3.0/pesummary/cli/summaryrecreate.py`

 * *Files identical despite different names*

### Comparing `pesummary-1.2.0/pesummary/cli/summaryreview.py` & `pesummary-1.3.0/pesummary/cli/summaryreview.py`

 * *Files identical despite different names*

### Comparing `pesummary-1.2.0/pesummary/cli/summarysplit.py` & `pesummary-1.3.0/pesummary/cli/summarysplit.py`

 * *Files identical despite different names*

### Comparing `pesummary-1.2.0/pesummary/cli/summarytest.py` & `pesummary-1.3.0/pesummary/cli/summarytest.py`

 * *Files identical despite different names*

### Comparing `pesummary-1.2.0/pesummary/cli/summarytgr.py` & `pesummary-1.3.0/pesummary/cli/summarytgr.py`

 * *Files identical despite different names*

### Comparing `pesummary-1.2.0/pesummary/conf/caption.py` & `pesummary-1.3.0/pesummary/conf/caption.py`

 * *Files identical despite different names*

### Comparing `pesummary-1.2.0/pesummary/conf/configuration.py` & `pesummary-1.3.0/pesummary/conf/configuration.py`

 * *Files 5% similar despite different names*

```diff
@@ -114,17 +114,22 @@
 precessing_spins = ["spin_1x", "spin_1y", "spin_2x", "spin_2y"]
 # Parameters to use for GW extrinsic corner plot
 gw_extrinsic_corner_parameters = ["luminosity_distance", "psi", "ra", "dec"]
 
 # List of 2d plots to generate for GW analyses
 gw_2d_plots = [
     ["mass_1", "mass_2"], ["mass_1_source", "mass_2_source"], ["a_1", "a_2"],
-    ["mass_ratio", "chi_eff"], ["chi_p", "chi_eff"], ["cos_theta_jn", "chi_p"],
-    ["cos_theta_jn", "luminosity_distance"], ["chirp_mass", "luminosity_distance"],
-    ["lambda_1", "lambda_2"], ["mass_ratio", "lambda_tilde"]
+    ["total_mass", "chi_eff"], ["mass_ratio", "chi_eff"],
+    ["mass_ratio", "chi_p"], ["chi_p", "chi_eff"], ["cos_theta_jn", "chi_p"],
+    ["ra", "dec"], ["cos_theta_jn", "luminosity_distance"],
+    ["chirp_mass", "luminosity_distance"],
+    ["mass_ratio", "luminosity_distance"], ["lambda_1", "lambda_2"],
+    ["mass_ratio", "lambda_tilde"], ["ra", "geocent_time"],
+    ["dec", "geocent_time"], ["H1_L1_time_delay", "H1_V1_time_delay"],
+    ["H1_V1_time_delay", "L1_V1_time_delay"],
 ]
 
 # Cosmology to use when calculating redshift
 cosmology = "Planck15"
 
 # Analytic PSD to use for conversions when no PSD file is provided
 psd = "aLIGOZeroDetHighPower"
```

### Comparing `pesummary-1.2.0/pesummary/core/cli/actions.py` & `pesummary-1.3.0/pesummary/core/cli/actions.py`

 * *Files identical despite different names*

### Comparing `pesummary-1.2.0/pesummary/core/cli/inputs.py` & `pesummary-1.3.0/pesummary/core/cli/inputs.py`

 * *Files identical despite different names*

### Comparing `pesummary-1.2.0/pesummary/core/cli/parser.py` & `pesummary-1.3.0/pesummary/core/cli/parser.py`

 * *Files identical despite different names*

### Comparing `pesummary-1.2.0/pesummary/core/css/image_styles.css` & `pesummary-1.3.0/pesummary/core/css/image_styles.css`

 * *Files identical despite different names*

### Comparing `pesummary-1.2.0/pesummary/core/css/navbar.css` & `pesummary-1.3.0/pesummary/core/css/navbar.css`

 * *Files identical despite different names*

### Comparing `pesummary-1.2.0/pesummary/core/css/side_bar.css` & `pesummary-1.3.0/pesummary/core/css/side_bar.css`

 * *Files identical despite different names*

### Comparing `pesummary-1.2.0/pesummary/core/css/table.css` & `pesummary-1.3.0/pesummary/core/css/table.css`

 * *Files identical despite different names*

### Comparing `pesummary-1.2.0/pesummary/core/css/toggle.css` & `pesummary-1.3.0/pesummary/core/css/toggle.css`

 * *Files identical despite different names*

### Comparing `pesummary-1.2.0/pesummary/core/fetch.py` & `pesummary-1.3.0/pesummary/core/fetch.py`

 * *Files identical despite different names*

### Comparing `pesummary-1.2.0/pesummary/core/file/formats/base_read.py` & `pesummary-1.3.0/pesummary/core/file/formats/base_read.py`

 * *Files identical despite different names*

### Comparing `pesummary-1.2.0/pesummary/core/file/formats/bilby.py` & `pesummary-1.3.0/pesummary/core/file/formats/bilby.py`

 * *Files identical despite different names*

### Comparing `pesummary-1.2.0/pesummary/core/file/formats/csv.py` & `pesummary-1.3.0/pesummary/core/file/formats/csv.py`

 * *Files identical despite different names*

### Comparing `pesummary-1.2.0/pesummary/core/file/formats/dat.py` & `pesummary-1.3.0/pesummary/core/file/formats/dat.py`

 * *Files identical despite different names*

### Comparing `pesummary-1.2.0/pesummary/core/file/formats/default.py` & `pesummary-1.3.0/pesummary/core/file/formats/default.py`

 * *Files identical despite different names*

### Comparing `pesummary-1.2.0/pesummary/core/file/formats/hdf5.py` & `pesummary-1.3.0/pesummary/core/file/formats/hdf5.py`

 * *Files identical despite different names*

### Comparing `pesummary-1.2.0/pesummary/core/file/formats/ini.py` & `pesummary-1.3.0/pesummary/core/file/formats/ini.py`

 * *Files identical despite different names*

### Comparing `pesummary-1.2.0/pesummary/core/file/formats/json.py` & `pesummary-1.3.0/pesummary/core/file/formats/json.py`

 * *Files identical despite different names*

### Comparing `pesummary-1.2.0/pesummary/core/file/formats/numpy.py` & `pesummary-1.3.0/pesummary/core/file/formats/numpy.py`

 * *Files identical despite different names*

### Comparing `pesummary-1.2.0/pesummary/core/file/formats/pesummary.py` & `pesummary-1.3.0/pesummary/core/file/formats/pesummary.py`

 * *Files identical despite different names*

### Comparing `pesummary-1.2.0/pesummary/core/file/formats/pickle.py` & `pesummary-1.3.0/pesummary/core/file/formats/pickle.py`

 * *Files identical despite different names*

### Comparing `pesummary-1.2.0/pesummary/core/file/formats/sql.py` & `pesummary-1.3.0/pesummary/core/file/formats/sql.py`

 * *Files identical despite different names*

### Comparing `pesummary-1.2.0/pesummary/core/file/injection.py` & `pesummary-1.3.0/pesummary/core/file/injection.py`

 * *Files identical despite different names*

### Comparing `pesummary-1.2.0/pesummary/core/file/mcmc.py` & `pesummary-1.3.0/pesummary/core/file/mcmc.py`

 * *Files identical despite different names*

### Comparing `pesummary-1.2.0/pesummary/core/file/meta_file.py` & `pesummary-1.3.0/pesummary/core/file/meta_file.py`

 * *Files identical despite different names*

### Comparing `pesummary-1.2.0/pesummary/core/file/read.py` & `pesummary-1.3.0/pesummary/core/file/read.py`

 * *Files identical despite different names*

### Comparing `pesummary-1.2.0/pesummary/core/finish.py` & `pesummary-1.3.0/pesummary/core/finish.py`

 * *Files identical despite different names*

### Comparing `pesummary-1.2.0/pesummary/core/js/combine_corner.js` & `pesummary-1.3.0/pesummary/core/js/combine_corner.js`

 * *Files identical despite different names*

### Comparing `pesummary-1.2.0/pesummary/core/js/expert.js` & `pesummary-1.3.0/pesummary/core/js/expert.js`

 * *Files identical despite different names*

### Comparing `pesummary-1.2.0/pesummary/core/js/grab.js` & `pesummary-1.3.0/pesummary/core/js/grab.js`

 * *Files identical despite different names*

### Comparing `pesummary-1.2.0/pesummary/core/js/html_to_csv.js` & `pesummary-1.3.0/pesummary/core/js/html_to_csv.js`

 * *Files identical despite different names*

### Comparing `pesummary-1.2.0/pesummary/core/js/html_to_json.js` & `pesummary-1.3.0/pesummary/core/js/html_to_json.js`

 * *Files identical despite different names*

### Comparing `pesummary-1.2.0/pesummary/core/js/html_to_shell.js` & `pesummary-1.3.0/pesummary/core/js/html_to_shell.js`

 * *Files identical despite different names*

### Comparing `pesummary-1.2.0/pesummary/core/js/modal.js` & `pesummary-1.3.0/pesummary/core/js/modal.js`

 * *Files identical despite different names*

### Comparing `pesummary-1.2.0/pesummary/core/js/multi_dropbar.js` & `pesummary-1.3.0/pesummary/core/js/multi_dropbar.js`

 * *Files identical despite different names*

### Comparing `pesummary-1.2.0/pesummary/core/js/multiple_posteriors.js` & `pesummary-1.3.0/pesummary/core/js/multiple_posteriors.js`

 * *Files identical despite different names*

### Comparing `pesummary-1.2.0/pesummary/core/js/search.js` & `pesummary-1.3.0/pesummary/core/js/search.js`

 * *Files identical despite different names*

### Comparing `pesummary-1.2.0/pesummary/core/js/side_bar.js` & `pesummary-1.3.0/pesummary/core/js/side_bar.js`

 * *Files identical despite different names*

### Comparing `pesummary-1.2.0/pesummary/core/notebook/notebook.py` & `pesummary-1.3.0/pesummary/core/notebook/notebook.py`

 * *Files identical despite different names*

### Comparing `pesummary-1.2.0/pesummary/core/plots/bounded_1d_kde.py` & `pesummary-1.3.0/pesummary/core/plots/bounded_1d_kde.py`

 * *Files identical despite different names*

### Comparing `pesummary-1.2.0/pesummary/core/plots/bounded_2d_kde.py` & `pesummary-1.3.0/pesummary/core/plots/bounded_2d_kde.py`

 * *Files identical despite different names*

### Comparing `pesummary-1.2.0/pesummary/core/plots/figure.py` & `pesummary-1.3.0/pesummary/core/plots/figure.py`

 * *Files identical despite different names*

### Comparing `pesummary-1.2.0/pesummary/core/plots/interactive.py` & `pesummary-1.3.0/pesummary/core/plots/interactive.py`

 * *Files identical despite different names*

### Comparing `pesummary-1.2.0/pesummary/core/plots/interpolate.py` & `pesummary-1.3.0/pesummary/core/plots/interpolate.py`

 * *Files identical despite different names*

### Comparing `pesummary-1.2.0/pesummary/core/plots/main.py` & `pesummary-1.3.0/pesummary/core/plots/main.py`

 * *Files identical despite different names*

### Comparing `pesummary-1.2.0/pesummary/core/plots/plot.py` & `pesummary-1.3.0/pesummary/core/plots/plot.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 # Licensed under an MIT style license -- see LICENSE.md
 
 from pesummary.utils.utils import (
     logger, number_of_columns_for_legend, _check_latex_install, gelman_rubin,
 )
 from pesummary.core.plots.seaborn.kde import kdeplot
+from pesummary.core.plots.corner import corner
 from pesummary.core.plots.figure import figure, ExistingFigure
 from pesummary import conf
 
 import matplotlib.lines as mlines
-import corner
 import copy
 from itertools import cycle
 
 import numpy as np
 from scipy import signal
 
 __author__ = ["Charlie Hoy <charlie.hoy@ligo.org>"]
@@ -832,15 +832,15 @@
     xs = np.zeros([len(included_parameters), len(samples[parameters[0]])])
     for num, i in enumerate(included_parameters):
         xs[num] = samples[i]
     default_kwargs.update(kwargs)
     default_kwargs["range"] = [1.0] * len(included_parameters)
     default_kwargs["labels"] = [latex_labels[i] for i in included_parameters]
 
-    _figure = ExistingFigure(corner.corner(xs.T, **default_kwargs))
+    _figure = ExistingFigure(corner(xs.T, included_parameters, **default_kwargs))
     # grab the axes of the subplots
     axes = _figure.get_axes()
     axes_of_interest = axes[:2]
     location = []
     for i in axes_of_interest:
         extent = i.get_window_extent().transformed(_figure.dpi_scale_trans.inverted())
         location.append([extent.x0 * _figure.dpi, extent.y0 * _figure.dpi])
```

### Comparing `pesummary-1.2.0/pesummary/core/plots/population.py` & `pesummary-1.3.0/pesummary/core/plots/population.py`

 * *Files identical despite different names*

### Comparing `pesummary-1.2.0/pesummary/core/plots/publication.py` & `pesummary-1.3.0/pesummary/core/plots/publication.py`

 * *Files identical despite different names*

### Comparing `pesummary-1.2.0/pesummary/core/plots/seaborn/kde.py` & `pesummary-1.3.0/pesummary/core/plots/seaborn/kde.py`

 * *Files identical despite different names*

### Comparing `pesummary-1.2.0/pesummary/core/plots/seaborn/violin.py` & `pesummary-1.3.0/pesummary/core/plots/seaborn/violin.py`

 * *Files identical despite different names*

### Comparing `pesummary-1.2.0/pesummary/core/reweight.py` & `pesummary-1.3.0/pesummary/core/reweight.py`

 * *Files identical despite different names*

### Comparing `pesummary-1.2.0/pesummary/core/webpage/base.py` & `pesummary-1.3.0/pesummary/core/webpage/base.py`

 * *Files identical despite different names*

### Comparing `pesummary-1.2.0/pesummary/core/webpage/copyright.txt` & `pesummary-1.3.0/pesummary/core/webpage/copyright.txt`

 * *Files identical despite different names*

### Comparing `pesummary-1.2.0/pesummary/core/webpage/main.py` & `pesummary-1.3.0/pesummary/core/webpage/main.py`

 * *Files identical despite different names*

### Comparing `pesummary-1.2.0/pesummary/core/webpage/tables.py` & `pesummary-1.3.0/pesummary/core/webpage/tables.py`

 * *Files identical despite different names*

### Comparing `pesummary-1.2.0/pesummary/core/webpage/webpage.py` & `pesummary-1.3.0/pesummary/core/webpage/webpage.py`

 * *Files identical despite different names*

### Comparing `pesummary-1.2.0/pesummary/gw/classification.py` & `pesummary-1.3.0/pesummary/gw/classification.py`

 * *Files identical despite different names*

### Comparing `pesummary-1.2.0/pesummary/gw/cli/inputs.py` & `pesummary-1.3.0/pesummary/gw/cli/inputs.py`

 * *Files 4% similar despite different names*

```diff
@@ -81,26 +81,27 @@
             }
         )
         return data
 
     @property
     def grab_data_kwargs(self):
         kwargs = super(_GWInput, self).grab_data_kwargs
-        for _property in ["f_low", "f_ref", "f_final", "delta_f"]:
+        for _property in ["f_start", "f_low", "f_ref", "f_final", "delta_f"]:
             if getattr(self, _property) is None:
                 setattr(self, "_{}".format(_property), [None] * len(self.labels))
             elif len(getattr(self, _property)) == 1 and len(self.labels) != 1:
                 setattr(
                     self, "_{}".format(_property),
                     getattr(self, _property) * len(self.labels)
                 )
         if self.opts.approximant is None:
             approx = [None] * len(self.labels)
         else:
             approx = self.opts.approximant
+        self.approximant_flags = self.opts.approximant_flags
         resume_file = [
             os.path.join(
                 self.webdir, "checkpoint",
                 "{}_conversion_class.pickle".format(label)
             ) for label in self.labels
         ]
 
@@ -109,15 +110,16 @@
                 try:
                     psd = self.psd[label]
                 except KeyError:
                     psd = {}
                 kwargs[label].update(dict(
                     evolve_spins_forwards=self.evolve_spins_forwards,
                     evolve_spins_backwards=self.evolve_spins_backwards,
-                    f_low=self.f_low[num],
+                    f_start=self.f_start[num], f_low=self.f_low[num],
+                    approximant_flags=self.approximant_flags.get(label, {}),
                     approximant=approx[num], f_ref=self.f_ref[num],
                     NRSur_fits=self.NRSur_fits, return_kwargs=True,
                     multipole_snr=self.calculate_multipole_snr,
                     precessing_snr=self.calculate_precessing_snr,
                     psd=psd, f_final=self.f_final[num],
                     waveform_fits=self.waveform_fits,
                     multi_process=self.opts.multi_process,
@@ -141,15 +143,15 @@
                     self.f_ref[0], self.f_low[0], approx[0]
                 )
             )
             for num, label in enumerate(self.labels):
                 kwargs[label].update(dict(
                     evolve_spins_forwards=self.evolve_spins_forwards,
                     evolve_spins_backwards=self.evolve_spins_backwards,
-                    f_low=self.f_low[0],
+                    f_start=self.f_start[0], f_low=self.f_low[0],
                     approximant=approx[0], f_ref=self.f_ref[0],
                     NRSur_fits=self.NRSur_fits, return_kwargs=True,
                     multipole_snr=self.calculate_multipole_snr,
                     precessing_snr=self.calculate_precessing_snr,
                     psd=self.psd[self.labels[0]], f_final=self.f_final[0],
                     waveform_fits=self.waveform_fits,
                     multi_process=self.opts.multi_process,
@@ -188,14 +190,34 @@
             If None, the read function loops through all possible options
         """
         data = pesummary.core.cli.inputs._Input.grab_data_from_file(
             file, label, webdir, config=config, injection=injection,
             read_function=GWRead, file_format=file_format, nsamples=nsamples,
             disable_prior_sampling=disable_prior_sampling, **kwargs
         )
+        try:
+            for _kwgs in data["file_kwargs"][label]:
+                if "approximant_flags" in _kwgs["meta_data"]:
+                    for key, item in _kwargs["meta_data"]["approximant_flags"].items():
+                        warning_cond = (
+                            key in self.approximant_flags[label] and
+                            self.approximant_flags[label][key] != item
+                        )
+                        if warning_cond:
+                            logger.warning(
+                                "Approximant flag {}={} found in result file for {}. "
+                                "Ignoring and using the provided values {}={}".format(
+                                    key, self.approximant_flags[label][key], label,
+                                    key, item
+                                )
+                            )
+                        else:
+                            self.approximant_flags[label][key] = item
+        except Exception:
+            pass
         return data
 
     @property
     def reweight_samples(self):
         return self._reweight_samples
 
     @reweight_samples.setter
@@ -282,14 +304,36 @@
                             "No approximant passed. Waveform plots will not be "
                             "generated"
                         )
                     self._approximant[i] = None
                     break
 
     @property
+    def approximant_flags(self):
+        return self._approximant_flags
+
+    @approximant_flags.setter
+    def approximant_flags(self, approximant_flags):
+        if hasattr(self, "_approximant_flags"):
+            return
+        _approximant_flags = {key: {} for key in self.labels}
+        for key, item in approximant_flags.items():
+            _label, key = key.split(":")
+            if _label not in self.labels:
+                raise ValueError(
+                    "Unable to assign waveform flags for label:{} because "
+                    "it does not exist. Available labels are: {}. Approximant "
+                    "flags must be provided in the form LABEL:FLAG:VALUE".format(
+                        _label, ", ".join(self.labels)
+                    )
+                )
+            _approximant_flags[_label][key] = item
+        self._approximant_flags = _approximant_flags
+
+    @property
     def gracedb_server(self):
         return self._gracedb_server
 
     @gracedb_server.setter
     def gracedb_server(self, gracedb_server):
         if gracedb_server is None:
             self._gracedb_server = conf.gracedb_server
@@ -582,14 +626,24 @@
     @f_low.setter
     def f_low(self, f_low):
         self._f_low = f_low
         if f_low is not None:
             self._f_low = [float(i) for i in f_low]
 
     @property
+    def f_start(self):
+        return self._f_start
+
+    @f_start.setter
+    def f_start(self, f_start):
+        self._f_start = f_start
+        if f_start is not None:
+            self._f_start = [float(i) for i in f_start]
+
+    @property
     def f_ref(self):
         return self._f_ref
 
     @f_ref.setter
     def f_ref(self, f_ref):
         self._f_ref = f_ref
         if f_ref is not None:
@@ -951,14 +1005,15 @@
         super(SamplesInput, self).__init__(
             *args, gw=True, extra_options=[
                 "evolve_spins_forwards",
                 "evolve_spins_backwards",
                 "NRSur_fits",
                 "calculate_multipole_snr",
                 "calculate_precessing_snr",
+                "f_start",
                 "f_low",
                 "f_ref",
                 "f_final",
                 "psd",
                 "waveform_fits",
                 "redshift_method",
                 "cosmology",
@@ -983,14 +1038,15 @@
             self.existing_skymap = self.existing_data["skymap"]
         else:
             self.existing_approximant = None
             self.existing_psd = None
             self.existing_calibration = None
             self.existing_skymap = None
         self.approximant = self.opts.approximant
+        self.approximant_flags = self.opts.approximant_flags
         self.detectors = None
         self.skymap = None
         self.calibration = self.opts.calibration
         self.gwdata = self.opts.gwdata
         self.maxL_samples = []
 
     @property
@@ -1507,52 +1563,37 @@
                     raise ValueError(
                         "Please provide a 'cutoff_frequency' and 'approximant' "
                         "for each file"
                     )
                 else:
                     try:
                         if name == "cutoff_frequency":
-                            cond = (
-                                "inspiral" in self._cutoff_frequency_dict.keys()
-                                and "postinspiral" not in
-                                self._cutoff_frequency_dict.keys()
-                            )
-                            if cond:
+                            if "inspiral" in self._cutoff_frequency_dict.keys():
                                 _dict["inspiral"] = self._cutoff_frequency_dict[
                                     "inspiral"
                                 ]
-                            elif "postinspiral" in self._cutoff_frequency_dict.keys():
+                            if "postinspiral" in self._cutoff_frequency_dict.keys():
                                 _dict["postinspiral"] = self._cutoff_frequency_dict[
                                     "postinspiral"
                                 ]
                         elif name == "approximant":
-                            cond = (
-                                "inspiral" in self._approximant_dict.keys()
-                                and "postinspiral" not in
-                                self._approximant_dict.keys()
-                            )
-                            if cond:
+                            if "inspiral" in self._approximant_dict.keys():
                                 _dict["inspiral"] = self._approximant_dict[
                                     "inspiral"
                                 ]
-                            elif "postinspiral" in self._approximant_dict.keys():
+                            if "postinspiral" in self._approximant_dict.keys():
                                 _dict["postinspiral"] = self._approximant_dict[
                                     "postinspiral"
                                 ]
                         elif name == "remnant_fits":
-                            cond = (
-                                "inspiral" in self._remnant_fits_dict.keys()
-                                and "postinspiral" not in
-                                self._remnant_fits_dict.keys()
-                            )
-                            if cond:
+                            if "inspiral" in self._remnant_fits_dict.keys():
                                 _dict["inspiral"] = self._remnant_fits_dict[
                                     "inspiral"
                                 ]
-                            elif "postinspiral" in self._remnant_fits_dict.keys():
+                            if "postinspiral" in self._remnant_fits_dict.keys():
                                 _dict["postinspiral"] = self._remnant_fits_dict[
                                     "postinspiral"
                                 ]
                     except (AttributeError, KeyError, TypeError):
                         _dict["inspiral"] = None
                         _dict["postinspiral"] = None
```

### Comparing `pesummary-1.2.0/pesummary/gw/cli/parser.py` & `pesummary-1.3.0/pesummary/gw/cli/parser.py`

 * *Files 1% similar despite different names*

```diff
@@ -128,14 +128,26 @@
             "--approximant": {
                 "dest": "approximant",
                 "help": "waveform approximant used to generate samples",
                 "nargs": "+",
                 "short": "-a",
                 "key": "gw",
             },
+            "--approximant_flags": {
+                "dest": "approximant_flags",
+                "help": (
+                    "flags used to control variant of waveform approximant used. Must "
+                    "be in the form LABEL:FLAG:VALUE where LABEL is the analysis label "
+                    "that you wish to assign FLAG:VALUE to"
+                ),
+                "nargs": "+",
+                "action": DictionaryAction,
+                "default": {},
+                "key": "gw",
+            },
             "--sensitivity": {
                 "action": "store_true",
                 "default": False,
                 "help": "generate sky sensitivities for HL, HLV",
                 "key": "gw",
             },
             "--gracedb": {
@@ -249,32 +261,43 @@
                 "default": "aLIGOZeroDetHighPower",
                 "help": (
                     "The PSD to use for conversions when no psd file is "
                     "provided. Default aLIGOZeroDetHighPower"
                 ),
                 "key": "gw",
             },
+            "--f_start": {
+                "dest": "f_start",
+                "nargs": "+",
+                "help": "Starting frequency of the supplied waveform",
+                "key": "gw",
+            },
             "--f_low": {
                 "dest": "f_low",
                 "nargs": "+",
-                "help": "Low frequency cutoff used to generate the samples",
+                "help": (
+                    "Low frequency cutoff for likelihood integration used to generate "
+                    "the samples"
+                ),
                 "key": "gw",
             },
             "--f_ref": {
                 "dest": "f_ref",
-                "help": "Reference frequency used to generate the samples",
+                "help": (
+                    "Reference frequency of the waveform used to generate the samples"
+                ),
                 "nargs": "+",
                 "key": "gw",
             },
             "--f_final": {
                 "dest": "f_final",
                 "nargs": "+",
                 "type": float,
                 "help": (
-                    "Final frequency to use when calculating the precessing snr"
+                    "Final frequency of the waveform. Used when calculating the precessing snr"
                 ),
                 "key": "gw"
             },
             "--delta_f": {
                 "dest": "delta_f",
                 "help": (
                     "Difference in frequency samples when calculating the "
```

### Comparing `pesummary-1.2.0/pesummary/gw/conversions/__init__.py` & `pesummary-1.3.0/pesummary/gw/conversions/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -44,20 +44,24 @@
     data: dict, list
         either a dictionary or samples or a list of parameters and a list of
         samples. See the examples below for details
     extra_kwargs: dict, optional
         dictionary of kwargs associated with this set of posterior samples.
     f_low: float, optional
         the low frequency cut-off to use when evolving the spins
+    f_start: float, optional
+        the starting frequency of the waveform
     f_ref: float, optional
         the reference frequency when spins are defined
     f_final: float, optional
         the final frequency to use when integrating over frequencies
     approximant: str, optional
         the approximant to use when evolving the spins
+    approximant_flags: dict, optional
+        dictionary of flags to control the variant of waveform model used
     evolve_spins_forwards: float/str, optional
         the final velocity to evolve the spins up to.
     evolve_spins_backwards: str, optional
         method to use when evolving the spins backwards to an infinite separation
     return_kwargs: Bool, optional
         if True, return a modified dictionary of kwargs containing information
         about the conversion
@@ -223,14 +227,15 @@
                 parameters = Parameters(args[0])
             else:
                 parameters = args[0]
             samples = args[1]
             samples = np.atleast_2d(samples).tolist()
         extra_kwargs = kwargs.get("extra_kwargs", {"sampler": {}, "meta_data": {}})
         f_low = kwargs.get("f_low", None)
+        f_start = kwargs.get("f_start", None)
         f_ref = kwargs.get("f_ref", None)
         f_final = kwargs.get("f_final", None)
         delta_f = kwargs.get("delta_f", None)
 
         for param, value in {"f_final": f_final, "delta_f": delta_f}.items():
             if value is not None and param in extra_kwargs["meta_data"].keys():
                 logger.warning(
@@ -255,14 +260,15 @@
                     )
                 )
                 extra_kwargs["meta_data"][param] = getattr(
                     conf, "default_{}".format(param)
                 )
 
         approximant = kwargs.get("approximant", None)
+        approximant_flags = kwargs.get("approximant_flags", {})
         NRSurrogate = kwargs.get("NRSur_fits", False)
         redshift_method = kwargs.get("redshift_method", "approx")
         cosmology = kwargs.get("cosmology", "Planck15")
         force_non_evolved = kwargs.get("force_non_evolved", False)
         force_remnant = kwargs.get("force_BBH_remnant_computation", False)
         force_evolve = kwargs.get("force_BH_spin_evolution", False)
         disable_remnant = kwargs.get("disable_remnant", False)
@@ -344,36 +350,49 @@
                         approximant
                     )
                 )
             evolve_spins_forwards = False
 
         multipole_snr = kwargs.get("multipole_snr", False)
         precessing_snr = kwargs.get("precessing_snr", False)
-        if f_low is not None and "f_low" in extra_kwargs["meta_data"].keys():
-            logger.warning(
-                base_replace.format(
-                    "f_low", extra_kwargs["meta_data"]["f_low"], f_low
+
+        for freq, name in zip([f_start, f_low], ["f_start", "f_low"]):
+            if freq is not None and name in extra_kwargs["meta_data"].keys():
+                logger.warning(
+                    base_replace.format(
+                        name, extra_kwargs["meta_data"][name], freq
+                    )
                 )
-            )
-            extra_kwargs["meta_data"]["f_low"] = f_low
-        elif f_low is not None:
-            extra_kwargs["meta_data"]["f_low"] = f_low
-        elif f_low is None and "f_low" in extra_kwargs["meta_data"].keys():
-            logger.debug(
-                "Found f_low in input file. Using {}Hz".format(
-                    extra_kwargs["meta_data"][param]
+                extra_kwargs["meta_data"][name] = freq
+            elif freq is not None:
+                extra_kwargs["meta_data"][name] = freq
+            elif freq is None and name in extra_kwargs["meta_data"].keys():
+                logger.debug(
+                    "Found {} in input file. Using {}Hz".format(
+                        name, extra_kwargs["meta_data"][name]
+                    )
                 )
-            )
-        else:
+            else:
+                logger.warning(
+                    "Could not find {} in input file and one was not passed from "
+                    "the command line. Using {}Hz as default".format(
+                        name, conf.default_flow
+                    )
+                )
+                extra_kwargs["meta_data"][name] = conf.default_flow
+        if len(approximant_flags) and "approximant_flags" in extra_kwargs["meta_data"].keys():
             logger.warning(
-                "Could not find minimum frequency in input file and "
-                "one was not passed from the command line. Using {}Hz "
-                "as default".format(conf.default_flow)
+                base_replace.format(
+                    "approximant_flags", extra_kwargs["meta_data"]["approximant_flags"],
+                    approximant_flags
+                )
             )
-            extra_kwargs["meta_data"]["f_low"] = conf.default_flow
+            extra_kwargs["meta_data"]["approximant_flags"] = approximant_flags
+        elif len(approximant_flags):
+            extra_kwargs["meta_data"]["approximant_flags"] = approximant_flags
         if approximant is not None and "approximant" in extra_kwargs["meta_data"].keys():
             logger.warning(
                 base_replace.format(
                     "approximant", extra_kwargs["meta_data"]["approximant"],
                     approximant
                 )
             )
@@ -1003,29 +1022,44 @@
     def _psi_J(self):
         samples = self.specific_parameter_samples([
             "psi", "theta_jn", "phi_jl", "beta"
         ])
         psi = psi_J(samples[0], samples[1], samples[2], samples[3])
         self.append_data("psi_J", psi)
 
-    def _time_in_each_ifo(self):
+    def _retrieve_detectors(self):
         detectors = []
         if "IFOs" in list(self.extra_kwargs["meta_data"].keys()):
             detectors = self.extra_kwargs["meta_data"]["IFOs"].split(" ")
         else:
             for i in self.parameters:
                 if "optimal_snr" in i and i != "network_optimal_snr":
                     det = i.split("_optimal_snr")[0]
                     detectors.append(det)
+        return detectors
 
+    def _time_in_each_ifo(self):
+        detectors = self._retrieve_detectors()
         samples = self.specific_parameter_samples(["ra", "dec", "geocent_time"])
         for i in detectors:
             time = time_in_each_ifo(i, samples[0], samples[1], samples[2])
             self.append_data("%s_time" % (i), time)
 
+    def _time_delay_between_ifos(self):
+        from itertools import combinations
+        detectors = sorted(self._retrieve_detectors())
+        for ifos in combinations(detectors, 2):
+            samples = self.specific_parameter_samples(
+                ["{}_time".format(_ifo) for _ifo in ifos]
+            )
+            self.append_data(
+                "%s_%s_time_delay" % (ifos[0], ifos[1]),
+                samples[1] - samples[0]
+            )
+
     def _lambda1_from_lambda_tilde(self):
         samples = self.specific_parameter_samples([
             "lambda_tilde", "mass_1", "mass_2"])
         lambda_1 = lambda1_from_lambda_tilde(samples[0], samples[1], samples[2])
         self.append_data("lambda_1", lambda_1)
 
     def _lambda2_from_lambda1(self):
@@ -1161,15 +1195,15 @@
         import copy
         required = [
             "mass_1", "mass_2", "spin_1z", "spin_2z", "psi", "iota", "ra",
             "dec", "geocent_time", "luminosity_distance", "phase",
             "reference_frequency"
         ]
         samples = self.specific_parameter_samples(required)
-        _f_low = self._retrieve_f_low()
+        _f_low = self._retrieve_stored_frequency("f_low")
         if isinstance(_f_low, (np.ndarray)):
             f_low = _f_low() * len(samples[0])
         else:
             f_low = [_f_low] * len(samples[0])
         original_list = copy.deepcopy(multipoles)
         rho, data_used = multipole_snr(
             *samples[:-1], f_low=f_low, psd=self.psd, f_ref=samples[-1],
@@ -1189,15 +1223,15 @@
             "phi_jl", "reference_frequency", "luminosity_distance", "phase"
         ]
         samples = self.specific_parameter_samples(required)
         try:
             spins = self.specific_parameter_samples(["spin_1z", "spin_2z"])
         except ValueError:
             spins = [None, None]
-        _f_low = self._retrieve_f_low()
+        _f_low = self._retrieve_stored_frequency("f_low")
         if isinstance(_f_low, (np.ndarray)):
             f_low = _f_low() * len(samples[0])
         else:
             f_low = [_f_low] * len(samples[0])
         [rho_p, b_bar, overlap, snrs], data_used = precessing_snr(
             samples[0], samples[1], samples[2], samples[3], samples[4],
             samples[5], samples[6], samples[7], samples[8], samples[9], samples[10],
@@ -1231,24 +1265,24 @@
                     "This indicates that the provided PSD may be different "
                     "from the one used in the sampling."
                 )
         except Exception:
             pass
         self.extra_kwargs["meta_data"]["precessing_snr"] = data_used
 
-    def _retrieve_f_low(self):
+    def _retrieve_stored_frequency(self, name):
         extra_kwargs = self.extra_kwargs["meta_data"]
-        if extra_kwargs != {} and "f_low" in list(extra_kwargs.keys()):
-            f_low = extra_kwargs["f_low"]
+        if extra_kwargs != {} and name in list(extra_kwargs.keys()):
+            freq = extra_kwargs[name]
         else:
             raise ValueError(
                 "Could not find f_low in input file. Please either modify the "
                 "input file or pass it from the command line"
             )
-        return f_low
+        return freq
 
     def _retrieve_approximant(self):
         extra_kwargs = self.extra_kwargs["meta_data"]
         if extra_kwargs != {} and "approximant" in list(extra_kwargs.keys()):
             approximant = extra_kwargs["approximant"]
         else:
             raise ValueError(
@@ -1269,15 +1303,15 @@
         if not _check_approximant_from_string(approximant):
             _msg = (
                 'Not evolving spins: approximant {0} unknown to '
                 'lalsimulation and gwsignal'.format(approximant)
             )
             logger.warning(_msg)
             raise EvolveSpinError(_msg)
-        f_low = self._retrieve_f_low()
+        f_low = self._retrieve_stored_frequency("f_low")
         if not forward:
             [tilt_1_evolved, tilt_2_evolved, phi_12_evolved], fits_used = evolve_spins(
                 samples[0], samples[1], samples[2], samples[3], samples[4],
                 samples[5], samples[6], f_low, samples[7][0],
                 approximant, evolve_limit="infinite_separation",
                 multi_process=self.multi_process, return_fits_used=True,
                 method=self.evolve_spins_backwards
@@ -1392,15 +1426,15 @@
         self.append_data(param, peak_luminosity)
         self.extra_kwargs["meta_data"]["peak_luminosity_NR_fits"] = fits
 
     def _final_remnant_properties_from_NRSurrogate(
         self, non_precessing=False,
         parameters=["final_mass", "final_spin", "final_kick"]
     ):
-        f_low = self._retrieve_f_low()
+        f_low = self._retrieve_stored_frequency("f_start")
         approximant = self._retrieve_approximant()
         samples = self._precessing_vs_non_precessing_parameters(
             non_precessing=non_precessing, evolved=False
         )
         frequency_samples = self.specific_parameter_samples([
             "reference_frequency"
         ])
@@ -1472,15 +1506,15 @@
             self.append_data(
                 "tidal_disruption_frequency_ratio", ratio
             )
 
     def _final_remnant_properties_from_waveform(
         self, non_precessing=False, parameters=["final_mass", "final_spin"],
     ):
-        f_low = self._retrieve_f_low()
+        f_low = self._retrieve_stored_frequency("f_start")
         approximant = self._retrieve_approximant()
         if "delta_t" in self.extra_kwargs["meta_data"].keys():
             delta_t = self.extra_kwargs["meta_data"]["delta_t"]
         else:
             delta_t = 1. / 4096
             if "seob" in approximant.lower():
                 logger.warning(
@@ -1493,23 +1527,24 @@
                 "empty", "spin_2z", "iota", "luminosity_distance",
                 "phase"
             ]
         else:
             sample_params = [
                 "mass_1", "mass_2", "spin_1x", "spin_1y", "spin_1z",
                 "spin_2x", "spin_2y", "spin_2z", "iota", "luminosity_distance",
-                "phase"
+                "phase", "reference_frequency"
             ]
         samples = self.specific_parameter_samples(sample_params)
         ind = self.parameters.index("spin_1x")
         _data, fits = _final_from_initial_BBH(
             *samples[:8], iota=samples[8], luminosity_distance=samples[9],
-            f_ref=[f_low] * len(samples[0]), phi_ref=samples[10],
-            delta_t=1. / 4096, approximant=approximant, return_fits_used=True,
-            multi_process=self.multi_process
+            f_low=[f_low] * len(samples[0]), f_ref=samples[-1],
+            phi_ref=samples[10], delta_t=1. / 4096, approximant=approximant,
+            xphm_flags=self.extra_kwargs["meta_data"].get("approximant_flags", {}),
+            return_fits_used=True, multi_process=self.multi_process
         )
         data = {"final_mass": _data[0], "final_spin": _data[1]}
         for param in parameters:
             self.append_data(param, data[param])
             self.extra_kwargs["meta_data"]["{}_NR_fits".format(param)] = fits
 
     def _final_mass_of_merger(self, evolved=False):
@@ -1524,15 +1559,15 @@
             "spin_2z", evolved=evolved, core_param=True,
             non_precessing=self.non_precessing
         )
         samples = self.specific_parameter_samples([
             "mass_1", "mass_2", spin_1z_param, spin_2z_param
         ])
         final_mass, fits = final_mass_of_merger(
-            *samples, return_fits_used=True
+            *samples, return_fits_used=True,
         )
         self.append_data(param, final_mass)
         self.extra_kwargs["meta_data"]["final_mass_NR_fits"] = fits
 
     def _final_mass_source(self, evolved=False):
         param = self._evolved_vs_non_evolved_parameter(
             "final_mass", evolved=evolved, non_precessing=self.non_precessing
@@ -1547,15 +1582,15 @@
         param = self._evolved_vs_non_evolved_parameter(
             "final_spin", evolved=evolved, non_precessing=self.non_precessing
         )
         samples = self._precessing_vs_non_precessing_parameters(
             non_precessing=non_precessing, evolved=evolved
         )
         final_spin, fits = final_spin_of_merger(
-            *samples, return_fits_used=True
+            *samples, return_fits_used=True,
         )
         self.append_data(param, final_spin)
         self.extra_kwargs["meta_data"]["final_spin_NR_fits"] = fits
 
     def _radiated_energy(self, evolved=False):
         param = self._evolved_vs_non_evolved_parameter(
             "radiated_energy", evolved=evolved, non_precessing=self.non_precessing
@@ -1986,14 +2021,15 @@
                     self._final_remnant_properties_from_NSBH_waveform(
                         parameters=_NSBH_parameters, source=True
                     )
         location = ["geocent_time", "ra", "dec"]
         if all(i in self.parameters for i in location):
             try:
                 self._time_in_each_ifo()
+                self._time_delay_between_ifos()
             except Exception as e:
                 logger.warning(
                     "Failed to generate posterior samples for the time in each "
                     "detector because %s" % (e)
                 )
         if any("_matched_filter_snr_angle" in i for i in self.parameters):
             if any("_matched_filter_abs_snr" in i for i in self.parameters):
```

### Comparing `pesummary-1.2.0/pesummary/gw/conversions/angles.py` & `pesummary-1.3.0/pesummary/gw/conversions/angles.py`

 * *Files identical despite different names*

### Comparing `pesummary-1.2.0/pesummary/gw/conversions/cosmology.py` & `pesummary-1.3.0/pesummary/gw/conversions/cosmology.py`

 * *Files identical despite different names*

### Comparing `pesummary-1.2.0/pesummary/gw/conversions/evolve.py` & `pesummary-1.3.0/pesummary/gw/conversions/evolve.py`

 * *Files identical despite different names*

### Comparing `pesummary-1.2.0/pesummary/gw/conversions/mass.py` & `pesummary-1.3.0/pesummary/gw/conversions/mass.py`

 * *Files identical despite different names*

### Comparing `pesummary-1.2.0/pesummary/gw/conversions/nrutils.py` & `pesummary-1.3.0/pesummary/gw/conversions/nrutils.py`

 * *Files identical despite different names*

### Comparing `pesummary-1.2.0/pesummary/gw/conversions/remnant.py` & `pesummary-1.3.0/pesummary/gw/conversions/remnant.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 # Licensed under an MIT style license -- see LICENSE.md
 
 import numpy as np
 
 from pesummary.utils.utils import logger, iterator
 from pesummary.utils.decorators import array_input
 from .spins import chi_p
+from .mass import eta_from_m1_m2
 
 __author__ = ["Charlie Hoy <charlie.hoy@ligo.org>"]
 
 try:
     import lalsimulation
     from lalsimulation import (
         FLAG_SEOBNRv4P_HAMILTONIAN_DERIVATIVE_NUMERICAL,
@@ -85,15 +86,16 @@
 
 
 def _return_final_mass_and_final_spin_from_waveform(
     mass_function=None, spin_function=None, mass_function_args=[],
     spin_function_args=[], mass_function_return_function=None,
     mass_function_return_index=None, spin_function_return_function=None,
     spin_function_return_index=None, mass_1_index=0, mass_2_index=1,
-    nsamples=0, approximant=None, default_SEOBNRv4P_kwargs=False
+    nsamples=0, approximant=None, default_SEOBNRv4P_kwargs=False,
+    mass_1=None, mass_2=None
 ):
     """Return the final mass and final spin given functions to use
 
     Parameters
     ----------
     mass_function: func
         function you wish to use to calculate the final mass
@@ -127,14 +129,20 @@
         the index of mass_2 in mass_function_args. Default is 1
     nsamples: int, optional
         the total number of samples
     approximant: str, optional
         the approximant used
     default_SEOBNRv4P_kwargs: Bool, optional
         if True, use the default SEOBNRv4P flags
+    mass_1: str, optional
+        function used to give samples for the primary mass. If provided,
+        mass_1_index is ignored
+    mass_2: str, optional
+        function used to give samples for the secondary mass. If provided,
+        mass_2_index is ignored
     """
     if default_SEOBNRv4P_kwargs:
         mode_array, seob_flags = _setup_SEOBNRv4P_args()
         mass_function_args += [mode_array, seob_flags]
         spin_function_args += [mode_array, seob_flags]
     fm = mass_function(*mass_function_args)
     if mass_function_return_function is not None:
@@ -142,17 +150,23 @@
     elif mass_function_return_index is not None:
         fm = fm[mass_function_return_index]
     fs = spin_function(*spin_function_args)
     if spin_function_return_function is not None:
         fs = eval("fs{}".format(spin_function_return_function))
     elif spin_function_return_index is not None:
         fs = fs[spin_function_return_index]
-    final_mass = fm * (
-        mass_function_args[mass_1_index] + mass_function_args[mass_2_index]
-    ) / MSUN_SI
+    if mass_1 is None:
+        mass1 = mass_function_args[mass_1_index]
+    else:
+        mass1 = eval(mass_1)
+    if mass_2 is None:
+        mass_function_args[mass_2_index]
+    else:
+        mass2 = eval(mass_2)
+    final_mass = fm * (mass1 + mass2) / MSUN_SI
     final_spin = fs
     return final_mass, final_spin
 
 
 def _setup_SEOBNRv4P_args(mode=[2, 2], seob_flags=DEFAULT_SEOBFLAGS):
     """Setup the SEOBNRv4P[HM] kwargs
     """
@@ -165,20 +179,121 @@
     SimInspiralModeArrayActivateMode(mode_array, mode[0], mode[1])
     _seob_flags = CreateDict()
     for key, item in seob_flags.items():
         DictInsertINT4Value(_seob_flags, key, item)
     return mode_array, _seob_flags
 
 
+def _SimIMRPhenomXFinalMass2017Wrapper(eta, spin_1z, spin_2z, mass_1, mass2):
+    """Wrapper for SimIMRPhenomXFinalMass2017 which takes
+    2 additional arguments: mass_1 and mass_2. This is needed
+    for the downstream `_return_final_mass_and_final_spin_from_waveform`
+    function
+
+    Parameters
+    ----------
+    eta: np.ndarray
+        symmetric mass ratio of the binary
+    spin_1z: np.ndarray
+        component of the primary spin aligned with the orbital angular momentum
+    spin_1z: np.ndarray
+        component of the secondary spin aligned with the orbital angular momentum
+    mass_1: np.ndarray
+        primary mass of the binary
+    mass_2: np.ndarray
+        secondary mass of the binary
+    """
+    from lalsimulation import SimIMRPhenomXFinalMass2017
+    return SimIMRPhenomXFinalMass2017(eta, spin_1z, spin_2z)
+
+
+def _SimIMRPhenomXFinalSpinWrapper(
+    eta, spin_1z, spin_2z, flags={}, chi_perp_mag=None, chi_p=None, spin_1x=None
+):
+    """Wrapper for SimIMRPhenomXFinalSpin2017 and SimIMRPhenomXPrecessingFinalSpin2017
+    which accounts for the different variants of PhenomX.
+
+    Parameters
+    ----------
+    eta: np.ndarray
+        symmetric mass ratio of the binary
+    spin_1z: np.ndarray
+        component of the primary spin aligned with the orbital angular momentum
+    spin_2z: np.ndarray
+        component of the secondary spin aligned with the orbital angular momentum
+    flags: dict, optional
+        dictionary containing flags to specify the different variants of PhenomX
+    chi_perp_mag: np.ndarray, optional
+        perpendicular magnitude of the binaries spin angular momentum. Must be
+        provided for precessing systems
+    chi_p: np.ndarray, optional
+        precessing spin of the binary. Must be provided for precessing systems
+    spin_1x: np.ndarray, optional
+        component of the primary spin which is perpendicular to the orbital
+        angular momentum, in the x-plane. Must be provided for precessing
+        systems
+    """
+    from lalsimulation import (
+        SimIMRPhenomXPrecessingFinalSpin2017, SimIMRPhenomXFinalSpin2017
+    )
+
+    _spinflag = int(flags.get("PhenomXPFinalSpinMod", 4))
+    _precflag = int(flags.get("PhenomXPrecVersion", 300))
+    final_spin_parallel = SimIMRPhenomXFinalSpin2017(eta, spin_1z, spin_2z)
+    if chi_perp_mag is None:
+        return final_spin_parallel
+    if _spinflag == 0:
+        if chi_p is None:
+            raise ValueError("Please provide samples for chi_p")
+        final_spin_perp = SimIMRPhenomXPrecessingFinalSpin2017(
+            eta, spin_1z, spin_2z, chi_p
+        )
+    elif _spinflag == 1:
+        if spin_1x is None:
+            raise ValueError("Please provide samples for spin_1x")
+        final_spin_perp = SimIMRPhenomXPrecessingFinalSpin2017(
+            eta, spin_1z, spin_2z, spin_1x
+        )
+    elif _spinflag == 3:
+        if _precflag in [220, 221, 222, 223, 224]:
+            logger.warning(
+                "Computing the remnant properties for PhenomX with "
+                "precession version: {} requires variables that are "
+                "not accessible with pesummary. Defaulting to final "
+                "spin version 0 ".format(_precflag)
+            )
+        if chi_p is None:
+            raise ValueError("Please provide samples for chi_p")
+        final_spin_perp = SimIMRPhenomXPrecessingFinalSpin2017(
+            eta, spin_1z, spin_2z, chi_p
+        )
+    elif _spinflag == 4:
+        final_spin_perp = SimIMRPhenomXPrecessingFinalSpin2017(
+            eta, spin_1z, spin_2z, chi_perp_mag
+        )
+    else:
+        raise ValueError(
+            "Unable to calculate remnant properties for specified PhenomX "
+            "variant."
+        )
+    if isinstance(final_spin_perp, (list, np.ndarray)):
+        final_spin_perp[final_spin_perp > 1.] = 1.
+    else:
+        if final_spin_perp > 1.:
+            final_spin_perp = 1.
+    return final_spin_perp
+
+
 @array_input()
 def _final_from_initial_BBH(
     mass_1, mass_2, spin_1x, spin_1y, spin_1z, spin_2x, spin_2y, spin_2z,
-    approximant="SEOBNRv4", iota=None, luminosity_distance=None, f_ref=None,
-    phi_ref=None, mode=[2, 2], delta_t=1. / 4096, seob_flags=DEFAULT_SEOBFLAGS,
-    return_fits_used=False, multi_process=None
+    approximant="SEOBNRv4", iota=None, luminosity_distance=None, f_low=20.,
+    f_ref=None, phi_ref=None, mode=[2, 2], delta_t=1. / 4096,
+    seob_flags=DEFAULT_SEOBFLAGS, xphm_flags={}, return_fits_used=False,
+    multi_process=None
 ):
     """Calculate the final mass and final spin given the initial parameters
     of the binary using the approximant directly
 
     Parameters
     ----------
     mass_1: float/np.ndarray
@@ -204,37 +319,43 @@
         sight of the source. Used when calculating the remnant fits for
         SEOBNRv4PHM. Since we only need the EOB dynamics here it does not matter
         what we pass
     luminosity_distance: float/np.ndarray, optional
         the luminosity distance of the source. Used when calculating the
         remnant fits for SEOBNRv4PHM. Since we only need the EOB dynamics here
         it does not matter what we pass.
+    f_low: float/np.ndarray, optional
+        the low frequency to evaluate the waveform model. Only used if
+        approximant=SEOBNRv5PHM
     f_ref: float/np.ndarray, optional
         the reference frequency at which the spins are defined
     phi_ref: float/np.ndarray, optional
         the coalescence phase of the binary
     mode: list, optional
         specific mode to use when calculating the remnant fits for SEOBNRv4PHM.
         Since we only need the EOB dynamics here it does not matter what we
         pass.
     delta_t: float, optional
         the sampling rate used in the analysis, Used when calculating the
         remnant fits for SEOBNRv4PHM
     seob_flags: dict, optional
         dictionary containing the SEOB flags. Used when calculating the remnant
         fits for SEOBNRv4PHM
+    xphm_flags: dict, optional
+        dictionary containing the XPHM flags used during the sampling. Used when
+        calculating the remnant fits for IMRPhenomXPHM
     return_fits_used: Bool, optional
         if True, return the approximant that was used.
     multi_process: int, optional
         the number of cores to use when calculating the remnant fits
     """
     from lalsimulation import (
         SimIMREOBFinalMassSpin, SimInspiralGetSpinSupportFromApproximant,
         SimIMRSpinPrecEOBWaveformAll, SimPhenomUtilsIMRPhenomDFinalMass,
-        SimPhenomUtilsPhenomPv2FinalSpin
+        SimPhenomUtilsPhenomPv2FinalSpin,
     )
     import multiprocessing
 
     def convert_args_for_multi_processing(kwargs):
         args = []
         for n in range(kwargs["nsamples"]):
             _args = []
@@ -242,58 +363,86 @@
                 if key == "mass_function_args" or key == "spin_function_args":
                     _args.append([key, [arg[n] for arg in item]])
                 else:
                     _args.append([key, item])
             args.append(_args)
         return args
 
-    try:
-        approx = getattr(lalsimulation, approximant)
-    except AttributeError:
-        raise ValueError(
-            "The waveform '{}' is not supported by lalsimulation"
-        )
-
     m1 = mass_1 * MSUN_SI
     m2 = mass_2 * MSUN_SI
     kwargs = {"nsamples": len(mass_1), "approximant": approximant}
-    if approximant.lower() in ["seobnrv4p", "seobnrv4phm"]:
+    cond1 = approximant.lower() in ["seobnrv4p", "seobnrv4phm"]
+    cond2 = "seobnrv5" in approximant.lower()
+    if cond1 or cond2:
         if any(i is None for i in [iota, luminosity_distance, f_ref, phi_ref]):
             raise ValueError(
                 "The approximant '{}' requires samples for iota, f_ref, "
                 "phi_ref and luminosity_distance. Please pass these "
                 "samples.".format(approximant)
             )
         if len(delta_t) == 1:
             delta_t = [delta_t[0]] * len(mass_1)
         elif len(delta_t) != len(mass_1):
             raise ValueError(
                 "Please provide either a single 'delta_t' that is is used for "
                 "all samples, or a single 'delta_t' for each sample"
             )
-        mode_array, _seob_flags = _setup_SEOBNRv4P_args(
-            mode=mode, seob_flags=seob_flags
-        )
-        args = np.array([
-            phi_ref, delta_t, m1, m2, f_ref, luminosity_distance, iota,
-            spin_1x, spin_1y, spin_1z, spin_2x, spin_2y, spin_2z,
-            [mode_array] * len(mass_1), [_seob_flags] * len(mass_1)
-        ])
-        kwargs.update(
-            {
-                "mass_function": SimIMRSpinPrecEOBWaveformAll,
-                "spin_function": SimIMRSpinPrecEOBWaveformAll,
-                "mass_function_args": args,
-                "spin_function_args": args,
-                "mass_function_return_function": "[21].data[6]",
-                "spin_function_return_function": "[21].data[7]",
-                "mass_1_index": 2,
-                "mass_2_index": 3,
-            }
-        )
+        if approximant.lower() in ["seobnrv4p", "seobnrv4phm"]:
+            mode_array, _seob_flags = _setup_SEOBNRv4P_args(
+                mode=mode, seob_flags=seob_flags
+            )
+            args = np.array([
+                phi_ref, delta_t, m1, m2, f_ref, luminosity_distance, iota,
+                spin_1x, spin_1y, spin_1z, spin_2x, spin_2y, spin_2z,
+                [mode_array] * len(mass_1), [_seob_flags] * len(mass_1)
+            ])
+            kwargs.update(
+                {
+                    "mass_function": SimIMRSpinPrecEOBWaveformAll,
+                    "spin_function": SimIMRSpinPrecEOBWaveformAll,
+                    "mass_function_args": args,
+                    "spin_function_args": args,
+                    "mass_function_return_function": "[21].data[6]",
+                    "spin_function_return_function": "[21].data[7]",
+                    "mass_1_index": 2,
+                    "mass_2_index": 3,
+                }
+            )
+        else:
+            from pesummary.gw.waveform import td_waveform
+            _samples = [
+                {
+                    "mass_1": mass_1[ind], "mass_2": mass_2[ind],
+                    "spin_1x": spin_1x[ind], "spin_1y": spin_1y[ind],
+                    "spin_1z": spin_1z[ind], "spin_2x": spin_2x[ind],
+                    "spin_2y": spin_2y[ind], "spin_2z": spin_2z[ind],
+                    "iota": iota[ind],
+                    "luminosity_distance": luminosity_distance[ind],
+                    "phase": phi_ref[ind]
+                } for ind in np.arange(len(mass_1))
+            ]
+            args = np.array([
+                _samples, [approximant] * len(mass_1), delta_t, f_low,
+                f_ref, [None] * len(mass_1), [0] * len(mass_1), [0] * len(mass_1),
+                [0] * len(mass_1), [None] * len(mass_1), [None] * len(mass_1),
+                [False] * len(mass_1), [None] * len(mass_1), [1] * len(mass_1),
+                [{}] * len(mass_1), [True] * len(mass_1)
+            ], dtype=object)
+            kwargs.update(
+                {
+                    "mass_function": td_waveform,
+                    "spin_function": td_waveform,
+                    "mass_function_args": args,
+                    "spin_function_args": args,
+                    "mass_function_return_function": "[1].model.final_mass",
+                    "spin_function_return_function": "[1].model.final_spin",
+                    "mass_1": "mass_function_args[0]['mass_1'] * MSUN_SI",
+                    "mass_2": "mass_function_args[0]['mass_2'] * MSUN_SI",
+                }
+            )
     elif approximant.lower() in ["seobnrv4"]:
         spin1 = np.array([spin_1x, spin_1y, spin_1z]).T
         spin2 = np.array([spin_2x, spin_2y, spin_2z]).T
         app = np.array([approx] * len(mass_1))
         kwargs.update(
             {
                 "mass_function": SimIMREOBFinalMassSpin,
@@ -316,14 +465,45 @@
         if SimInspiralGetSpinSupportFromApproximant(approx) > 2:
             # matches the waveform's internal usage as corrected in
             # https://git.ligo.org/lscsoft/lalsuite/-/merge_requests/1270
             _chi_p = chi_p(mass_1, mass_2, spin_1x, spin_1y, spin_2x, spin_2y)
             kwargs["spin_function_args"].append(_chi_p)
         else:
             kwargs["spin_function_args"].append(np.zeros_like(mass_1))
+    elif "phenomx" in approximant.lower():
+        _eta = eta_from_m1_m2(m1, m2)
+        kwargs.update(
+            {
+                "mass_function": _SimIMRPhenomXFinalMass2017Wrapper,
+                "spin_function": _SimIMRPhenomXFinalSpinWrapper,
+                "mass_function_args": [_eta, spin_1z, spin_2z, m1, m2],
+                "mass_1_index": 3,
+                "mass_2_index": 4,
+            }
+        )
+        if SimInspiralGetSpinSupportFromApproximant(approx) > 2:
+            chi1_perp = np.array([spin_1x, spin_1y])
+            chi2_perp = np.array([spin_2x, spin_2y])
+            _chi_p = chi_p(mass_1, mass_1, spin_1x, spin_1y, spin_2x, spin_2y)
+            chi_perp = np.sum([chi1_perp, chi2_perp], axis=0)
+            chi_perp_mag = np.linalg.norm(chi_perp, axis=0)
+            kwargs.update(
+                {
+                    "spin_function_args": [
+                        _eta, spin_1z, spin_2z, [xphm_flags] * len(_eta), chi_perp_mag,
+                        _chi_p, spin_1x
+                    ]
+                }
+            )
+        else:
+            kwargs.update(
+                {
+                    "spin_function_args": [_eta, spin_1z, spin_2z]
+                }
+            )
     else:
         raise ValueError(
             "The waveform '{}' is not support by this function.".format(
                 approximant
             )
         )
 
@@ -546,15 +726,16 @@
     if return_fits_used:
         return data[0]["final_kick"], data[1]
     return data["final_kick"]
 
 
 def final_mass_of_merger(
     *args, method="NR", approximant="SEOBNRv4", NRfit="average",
-    final_spin=None, return_fits_used=False, model="NRSur7dq4Remnant"
+    final_spin=None, return_fits_used=False, model="NRSur7dq4Remnant",
+    xphm_flags={}
 ):
     """Return the final mass resulting from a BBH merger
 
     Parameters
     ----------
     mass_1: float/np.ndarray
         float/array of masses for the primary object
@@ -573,14 +754,17 @@
     NRFit: str
         Name of the NR fit you wish to use if chosen method is NR
     return_fits_used: Bool, optional
         if True, return the NR fits that were used. Only used when
         NRFit='average' or when method='NRSurrogate'
     model: str, optional
         The NRSurrogate model to use when evaluating the fits
+    xphm_flags: dict, optional
+        List of flags used to control the variant of PhenomX during the sampling.
+        Default {}
     """
     if method.lower() == "nr":
         mass_func = final_mass_of_merger_from_NR
         kwargs = {
             "NRfit": NRfit, "final_spin": final_spin,
             "return_fits_used": return_fits_used
         }
@@ -588,22 +772,23 @@
         mass_func = final_mass_of_merger_from_NRSurrogate
         kwargs = {
             "approximant": approximant, "return_fits_used": return_fits_used,
             "model": model
         }
     else:
         mass_func = final_mass_of_merger_from_waveform
-        kwargs = {"approximant": approximant}
+        kwargs = {"approximant": approximant, "xphm_flags": xphm_flags}
 
     return mass_func(*args, **kwargs)
 
 
 def final_spin_of_merger(
     *args, method="NR", approximant="SEOBNRv4", NRfit="average",
-    return_fits_used=False, model="NRSur7dq4Remnant"
+    return_fits_used=False, model="NRSur7dq4Remnant",
+    xphm_flags={}
 ):
     """Return the final mass resulting from a BBH merger
 
     Parameters
     ----------
     mass_1: float/np.ndarray
         float/array of masses for the primary object
@@ -630,27 +815,30 @@
     NRFit: str
         Name of the NR fit you wish to use if chosen method is NR
     return_fits_used: Bool, optional
         if True, return the NR fits that were used. Only used when
         NRFit='average' or when method='NRSurrogate'
     model: str, optional
         The NRSurrogate model to use when evaluating the fits
+    xphm_flags: dict, optional
+        List of flags used to control the variant of PhenomX during the sampling.
+        Default {}
     """
     if method.lower() == "nr":
         spin_func = final_spin_of_merger_from_NR
         kwargs = {"NRfit": NRfit, "return_fits_used": return_fits_used}
     elif "nrsur" in method.lower():
         spin_func = final_spin_of_merger_from_NRSurrogate
         kwargs = {
             "approximant": approximant, "return_fits_used": return_fits_used,
             "model": model
         }
     else:
         spin_func = final_spin_of_merger_from_waveform
-        kwargs = {"approximant": approximant}
+        kwargs = {"approximant": approximant, "xphm_flags": xphm_flags}
 
     return spin_func(*args, **kwargs)
 
 
 def final_kick_of_merger(
     *args, method="NR", approximant="SEOBNRv4", NRfit="average",
     return_fits_used: False, model="NRSur7dq4Remnant"
```

### Comparing `pesummary-1.2.0/pesummary/gw/conversions/snr.py` & `pesummary-1.3.0/pesummary/gw/conversions/snr.py`

 * *Files 0% similar despite different names*

```diff
@@ -163,22 +163,27 @@
             psd_default = conf.psd
         ANALYTIC = True
         psd_default_kwargs.update({"psd": psd_default})
         psd = pycbc_default_psd(**psd_default_kwargs)
 
     detectors = list(psd.keys())
     if df != psd[detectors[0]].delta_f:
-        from pycbc.psd import estimate
+        from pesummary.gw.file.psd import PSDDict
         logger.warning(
             "Provided PSD has df={} and {} has been specified. Interpolation "
             "will be used".format(psd[detectors[0]].delta_f, df)
         )
-        psd = {
-            ifo: estimate.interpolate(psd[ifo], df) for ifo in psd.keys()
-        }
+        if isinstance(psd, PSDDict):
+            psd = psd.interpolate(f_low, df)
+        else:
+            from pesummary.gw.pycbc import interpolate_psd
+            psd = {
+                ifo: interpolate_psd(psd[ifo], f_low, df) for ifo in
+                psd.keys()
+            }
     return psd, ANALYTIC
 
 
 def _make_waveform(
     approx, theta_jn, phi_jl, phase, psi_J, mass_1, mass_2, tilt_1, tilt_2,
     phi_12, a_1, a_2, beta, distance, apply_detector_response=True, **kwargs
 ):
```

### Comparing `pesummary-1.2.0/pesummary/gw/conversions/spins.py` & `pesummary-1.3.0/pesummary/gw/conversions/spins.py`

 * *Files identical despite different names*

### Comparing `pesummary-1.2.0/pesummary/gw/conversions/tgr.py` & `pesummary-1.3.0/pesummary/gw/conversions/tgr.py`

 * *Files identical despite different names*

### Comparing `pesummary-1.2.0/pesummary/gw/conversions/tidal.py` & `pesummary-1.3.0/pesummary/gw/conversions/tidal.py`

 * *Files identical despite different names*

### Comparing `pesummary-1.2.0/pesummary/gw/conversions/time.py` & `pesummary-1.3.0/pesummary/gw/conversions/time.py`

 * *Files identical despite different names*

### Comparing `pesummary-1.2.0/pesummary/gw/cosmology.py` & `pesummary-1.3.0/pesummary/gw/cosmology.py`

 * *Files identical despite different names*

### Comparing `pesummary-1.2.0/pesummary/gw/fetch.py` & `pesummary-1.3.0/pesummary/gw/fetch.py`

 * *Files identical despite different names*

### Comparing `pesummary-1.2.0/pesummary/gw/file/__init__.py` & `pesummary-1.3.0/pesummary/gw/file/__init__.py`

 * *Files identical despite different names*

### Comparing `pesummary-1.2.0/pesummary/gw/file/calibration.py` & `pesummary-1.3.0/pesummary/gw/file/calibration.py`

 * *Files identical despite different names*

### Comparing `pesummary-1.2.0/pesummary/gw/file/formats/GWTC1.py` & `pesummary-1.3.0/pesummary/gw/file/formats/GWTC1.py`

 * *Files identical despite different names*

### Comparing `pesummary-1.2.0/pesummary/gw/file/formats/base_read.py` & `pesummary-1.3.0/pesummary/gw/file/formats/base_read.py`

 * *Files identical despite different names*

### Comparing `pesummary-1.2.0/pesummary/gw/file/formats/bilby.py` & `pesummary-1.3.0/pesummary/gw/file/formats/bilby.py`

 * *Files 6% similar despite different names*

```diff
@@ -157,52 +157,66 @@
                     if isinstance(item, bool):
                         kwargs["meta_data"][key] = str(item)
                     else:
                         kwargs["meta_data"][key] = item
                 except Exception:
                     pass
         try:
+            kwargs["meta_data"]["approximant_flags"] = \
+                f.meta_data["likelihood"]["waveform_arguments"]
             kwargs["meta_data"]["approximant"] = \
-                f.meta_data["likelihood"]["waveform_arguments"]["waveform_approximant"]
+                kwargs["meta_data"]["approximant_flags"].pop("waveform_approximant")
         except Exception:
             pass
         try:
             kwargs["meta_data"]["IFOs"] = \
                 " ".join(f.meta_data["likelihood"]["interferometers"].keys())
         except Exception:
             pass
         _config = config_from_object(f)
         if len(_config):
             if "config" in _config.keys():
                 _config = _config["config"]
             options = [
                 "minimum_frequency", "reference_frequency",
-                "waveform_approximant", "maximum_frequency"
+                "waveform_approximant", "maximum_frequency",
+                "waveform_arguments_dict"
+            ]
+            pesummary_names = [
+                "f_low", "f_ref", "approximant", "f_final",
+                "approximant_flags"
             ]
-            pesummary_names = ["f_low", "f_ref", "approximant", "f_final"]
             for opt, name in zip(options, pesummary_names):
                 if opt in _config.keys():
                     try:
                         _option = ast.literal_eval(_config[opt])
                     except ValueError:
                         try:
                             import re
-                            _config[opt] = re.sub(
+                            _option = re.sub(
                                 r'([A-Za-z/\.0-9\-\+][^\[\],:"}]*)', r'"\g<1>"', _config[opt]
                             )
-                            _option = ast.literal_eval(_config[opt])
+                            _option = ast.literal_eval(_option)
                         except Exception:
                             _option = _config[opt]
-                    if isinstance(_option, dict):
+                    if isinstance(_option, dict) and name != "approximant_flags":
                         _value = np.min([
-                            ast.literal_eval(value) for key, value in _option.items() if
-                            key != "waveform"
+                            ast.literal_eval(value) if not isinstance(value, (float, int)) else value
+                            for key, value in _option.items() if key != "waveform"
                         ])
+                        _f_start = [
+                            ast.literal_eval(value) if not isinstance(value, (float, int)) else value
+                            for key, value in _option.items() if key == "waveform"
+                        ]
+                        if len(_f_start):
+                            kwargs["meta_data"]["f_start"] = _f_start[0]
                     else:
                         _value = _option
+                    if _value is None and name == "approximant_flags":
+                        _value = {}
                     kwargs["meta_data"][name] = _value
         return kwargs
 
     @property
     def calibration_spline_posterior(self):
         if not any("recalib_" in i for i in self.parameters):
             return super(Bilby, self).calibration_spline_posterior
```

### Comparing `pesummary-1.2.0/pesummary/gw/file/formats/default.py` & `pesummary-1.3.0/pesummary/gw/file/formats/default.py`

 * *Files identical despite different names*

### Comparing `pesummary-1.2.0/pesummary/gw/file/formats/lalinference.py` & `pesummary-1.3.0/pesummary/gw/file/formats/lalinference.py`

 * *Files identical despite different names*

### Comparing `pesummary-1.2.0/pesummary/gw/file/formats/pesummary.py` & `pesummary-1.3.0/pesummary/gw/file/formats/pesummary.py`

 * *Files identical despite different names*

### Comparing `pesummary-1.2.0/pesummary/gw/file/formats/princeton.py` & `pesummary-1.3.0/pesummary/gw/file/formats/princeton.py`

 * *Files identical despite different names*

### Comparing `pesummary-1.2.0/pesummary/gw/file/formats/xml.py` & `pesummary-1.3.0/pesummary/gw/file/formats/xml.py`

 * *Files identical despite different names*

### Comparing `pesummary-1.2.0/pesummary/gw/file/injection.py` & `pesummary-1.3.0/pesummary/gw/file/injection.py`

 * *Files identical despite different names*

### Comparing `pesummary-1.2.0/pesummary/gw/file/meta_file.py` & `pesummary-1.3.0/pesummary/gw/file/meta_file.py`

 * *Files identical despite different names*

### Comparing `pesummary-1.2.0/pesummary/gw/file/psd.py` & `pesummary-1.3.0/pesummary/gw/file/psd.py`

 * *Files 6% similar despite different names*

```diff
@@ -137,36 +137,60 @@
             all kwargs passed to PSD.to_pycbc()
         """
         psd = {}
         for key, item in self.items():
             psd[key] = item.to_pycbc(*args, **kwargs)
         return PSDDict(psd)
 
+    def interpolate(self, low_freq_cutoff, delta_f):
+        """Interpolate a dictionary of PSDs to a new delta_f
+
+        Parameters
+        ----------
+        low_freq_cutoff: float
+            Frequencies below this value are set to zero.
+        delta_f : float, optional
+            Frequency resolution of the frequency series in Hertz.
+        """
+        psd = {}
+        for key, item in self.items():
+            psd[key] = item.interpolate(low_freq_cutoff, delta_f)
+        return PSDDict(psd)
+
 
 class PSD(np.ndarray):
     """Class to handle PSD data
     """
     def __new__(cls, input_array):
         obj = np.asarray(input_array).view(cls)
         if obj.shape[1] != 2:
             raise ValueError(
                 "Invalid input data. See the docs for instructions"
             )
         obj.delta_f = cls.delta_f(obj)
         obj.f_high = cls.f_high(obj)
+        obj.frequencies = cls.frequencies(obj)
         return obj
 
+    @property
+    def low_frequency(self):
+        return self.frequencies[0]
+
     @staticmethod
     def delta_f(array):
         return array.T[0][1] - array.T[0][0]
 
     @staticmethod
     def f_high(array):
         return array.T[0][-1]
 
+    @staticmethod
+    def frequencies(array):
+        return array.T[0]
+
     @classmethod
     def read(cls, path_to_file, **kwargs):
         """Read in a file and initialize the PSD class
 
         Parameters
         ----------
         path_to_file: str
@@ -255,14 +279,15 @@
         )
 
     def __array_finalize__(self, obj):
         if obj is None:
             return
         self.delta_f = getattr(obj, "delta_f", None)
         self.f_high = getattr(obj, "f_high", None)
+        self.frequencies = getattr(obj, "frequencies", None)
 
     def to_pycbc(
         self, low_freq_cutoff, f_high=None, length=None, delta_f=None,
         f_high_override=False
     ):
         """Convert the PSD object to an interpolated pycbc.types.FrequencySeries
 
@@ -301,7 +326,23 @@
             logger.warning(msg)
         if length is None:
             length = int(f_high / delta_f) + 1
         pycbc_psd = from_numpy_arrays(
             self.T[0], self.T[1], length, delta_f, low_freq_cutoff
         )
         return pycbc_psd
+
+    def interpolate(self, low_freq_cutoff, delta_f):
+        """Interpolate PSD to a new delta_f
+
+        Parameters
+        ----------
+        low_freq_cutoff: float
+            Frequencies below this value are set to zero.
+        delta_f : float, optional
+            Frequency resolution of the frequency series in Hertz.
+        """
+        from pesummary.gw.pycbc import interpolate_psd
+        psd = interpolate_psd(self.copy(), low_freq_cutoff, delta_f)
+        frequencies, strains = psd.sample_frequencies, psd
+        inds = np.where(frequencies >= low_freq_cutoff)
+        return PSD(np.vstack([frequencies[inds], strains[inds]]).T)
```

### Comparing `pesummary-1.2.0/pesummary/gw/file/read.py` & `pesummary-1.3.0/pesummary/gw/file/read.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 
 from pesummary.gw.file.formats.lalinference import LALInference
 from pesummary.gw.file.formats.bilby import Bilby
 from pesummary.gw.file.formats.default import Default
 from pesummary.gw.file.formats.pesummary import (
     TGRPESummary, PESummary, PESummaryDeprecated
 )
+from pesummary.gw.file.formats.pycbc import PyCBC
 from pesummary.gw.file.formats.GWTC1 import GWTC1
 from pesummary.core.file.read import (
     is_bilby_hdf5_file, is_bilby_json_file, is_pesummary_hdf5_file,
     is_pesummary_json_file, is_pesummary_hdf5_file_deprecated,
     is_pesummary_json_file_deprecated, _is_pesummary_hdf5_file,
     _is_pesummary_json_file
 )
@@ -96,21 +97,37 @@
             return True
         else:
             return False
     except Exception:
         return False
 
 
+def is_pycbc_file(path):
+    """Determine if the results file is a pycbc hdf5 file
+
+    Parameters
+    ----------
+    path: str
+        path to results file
+    """
+    import h5py
+    f = h5py.File(path, 'r')
+    if all(_ in f.attrs for _ in ["sampling_params", "variable_params", "model"]):
+        return True
+    return False
+
+
 GW_HDF5_LOAD = {
     is_lalinference_file: LALInference.load_file,
     is_bilby_hdf5_file: Bilby.load_file,
     is_tgr_pesummary_hdf5_file: TGRPESummary.load_file,
     is_pesummary_hdf5_file: PESummary.load_file,
     is_pesummary_hdf5_file_deprecated: PESummaryDeprecated.load_file,
-    is_GWTC1_file: GWTC1.load_file
+    is_GWTC1_file: GWTC1.load_file,
+    is_pycbc_file: PyCBC.load_file,
 }
 
 GW_JSON_LOAD = {
     is_bilby_json_file: Bilby.load_file,
     is_tgr_pesummary_json_file: TGRPESummary.load_file,
     is_pesummary_json_file: PESummary.load_file,
     is_pesummary_json_file_deprecated: PESummaryDeprecated.load_file
```

### Comparing `pesummary-1.2.0/pesummary/gw/file/skymap.py` & `pesummary-1.3.0/pesummary/gw/file/skymap.py`

 * *Files identical despite different names*

### Comparing `pesummary-1.2.0/pesummary/gw/file/standard_names.py` & `pesummary-1.3.0/pesummary/gw/file/standard_names.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,14 @@
 # Licensed under an MIT style license -- see LICENSE.md
 
+from itertools import combinations
+
 __author__ = ["Charlie Hoy <charlie.hoy@ligo.org>"]
-_IFOS = ["H1", "L1", "V1", "K1", "E1"]
+_IFOS = sorted(["H1", "L1", "V1", "K1", "E1"])
+_IFO_combinations = list(combinations(_IFOS, 2))
 tidal_params = ["lambda_1", "lambda_2", "delta_lambda", "lambda_tilde"]
 
 
 lalinference_map = {
     "logl": "log_likelihood",
     "logprior": "log_prior",
     "matched_filter_snr": "network_matched_filter_snr",
@@ -22,14 +25,17 @@
     "m1": "mass_1",
     "m2": "mass_2",
     "eta": "symmetric_mass_ratio",
     "mtotal": "total_mass",
     "h1_end_time": "H1_time",
     "l1_end_time": "L1_time",
     "v1_end_time": "V1_time",
+    "h1l1_delay": "H1_L1_time_delay",
+    "l1v1_delay": "L1_V1_time_delay",
+    "h1v1_delay": "H1_V1_time_delay",
     "a1z": "spin_1z",
     "a2z": "spin_2z",
     "m1_source": "mass_1_source",
     "m2_source": "mass_2_source",
     "mtotal_source": "total_mass_source",
     "mc_source": "chirp_mass_source",
     "phi1": "phi_1",
@@ -733,7 +739,15 @@
     descriptive_names["{}_matched_filter_snr_angle".format(detector)] = (
         "the angle of the complex component of the matched filter signal to "
         "noise ratio in the %s gravitational wave detector" % (detector)
     )
     descriptive_names["{}_time".format(detector)] = (
         "the GPS merger time at the %s gravitational wave detector" % (detector)
     )
+
+for detector_combination in _IFO_combinations:
+    descriptive_names["{}_{}_time_delay".format(*detector_combination)] = (
+        "the difference in GPS merger time between the %s and %s "
+        "gravitational wave detectors" % (
+            detector_combination[0], detector_combination[1]
+        )
+    )
```

### Comparing `pesummary-1.2.0/pesummary/gw/file/strain.py` & `pesummary-1.3.0/pesummary/gw/file/strain.py`

 * *Files identical despite different names*

### Comparing `pesummary-1.2.0/pesummary/gw/finish.py` & `pesummary-1.3.0/pesummary/gw/finish.py`

 * *Files identical despite different names*

### Comparing `pesummary-1.2.0/pesummary/gw/gracedb.py` & `pesummary-1.3.0/pesummary/gw/gracedb.py`

 * *Files identical despite different names*

### Comparing `pesummary-1.2.0/pesummary/gw/notebook/notebook.py` & `pesummary-1.3.0/pesummary/gw/notebook/notebook.py`

 * *Files identical despite different names*

### Comparing `pesummary-1.2.0/pesummary/gw/notebook/public.py` & `pesummary-1.3.0/pesummary/gw/notebook/public.py`

 * *Files identical despite different names*

### Comparing `pesummary-1.2.0/pesummary/gw/plots/bounds.py` & `pesummary-1.3.0/pesummary/gw/plots/bounds.py`

 * *Files identical despite different names*

### Comparing `pesummary-1.2.0/pesummary/gw/plots/cmap.py` & `pesummary-1.3.0/pesummary/gw/plots/cmap.py`

 * *Files identical despite different names*

### Comparing `pesummary-1.2.0/pesummary/gw/plots/cylon.csv` & `pesummary-1.3.0/pesummary/gw/plots/cylon.csv`

 * *Files identical despite different names*

### Comparing `pesummary-1.2.0/pesummary/gw/plots/detchar.py` & `pesummary-1.3.0/pesummary/gw/plots/detchar.py`

 * *Files identical despite different names*

### Comparing `pesummary-1.2.0/pesummary/gw/plots/latex_labels.py` & `pesummary-1.3.0/pesummary/gw/plots/latex_labels.py`

 * *Files 3% similar despite different names*

```diff
@@ -51,14 +51,17 @@
     "network_precessing_snr": r"$\rho_{\mathrm{p}}$",
     "_b_bar": r"$\bar{b}$",
     "_precessing_harmonics_overlap": r"$|\mathrm{O}^{\mathrm{prec}}_{0,1}|$",
     "H1_time": r"$t_{H} [\mathrm{s}]$",
     "L1_time": r"$t_{L} [\mathrm{s}]$",
     "V1_time": r"$t_{V} [\mathrm{s}]$",
     "E1_time": r"$t_{E} [\mathrm{s}]$",
+    "H1_L1_time_delay": r"$\Delta t_{HL} [\mathrm{s}]$",
+    "H1_V1_time_delay": r"$\Delta t_{HV} [\mathrm{s}]$",
+    "L1_V1_time_delay": r"$\Delta t_{LV} [\mathrm{s}]$",
     "spin_1x": r"$S_{1x}$",
     "spin_1y": r"$S_{1y}$",
     "spin_1z": r"$S_{1z}$",
     "spin_1z_evolved": r"$S_{1z}^{\mathrm{evol}}$",
     "spin_1z_infinity": r"$S_{1z,\infty}$",
     "spin_1z_infinity_only_prec_avg": (
         r"$S_{1z,\infty}^{\mathrm{only\, prec\, avg}}$"
```

### Comparing `pesummary-1.2.0/pesummary/gw/plots/main.py` & `pesummary-1.3.0/pesummary/gw/plots/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -290,15 +290,15 @@
         if os.path.isfile(filename) and checkpoint:
             return
         fig, _, _, _ = triangle_plot(
             *samples, kde=False, parameters=params, xlabel=latex_labels[0],
             ylabel=latex_labels[1], plot_datapoints=True, plot_density=False,
             levels=[1e-8], fill=False, grid=True, linewidths=[1.75],
             percentiles=[5, 95], percentile_plot=[label], labels=[label],
-            truth=truth
+            truth=truth, data_kwargs={"alpha": 0.3}
         )
         _PlotGeneration.save(
             fig, filename, preliminary=preliminary
         )
         
 
     def skymap_plot(self, label):
@@ -511,17 +511,19 @@
             return
         if detectors is None:
             detectors = ["H1", "L1"]
         else:
             detectors = detectors.split("_")
 
         fig = gw._waveform_plot(
-            detectors, maxL_samples, f_min=kwargs.get("f_low", 20.0),
+            detectors, maxL_samples, f_start=kwargs.get("f_start", 20.),
+            f_low=kwargs.get("f_low", 20.0),
             f_max=kwargs.get("f_final", 1024.),
-            f_ref=kwargs.get("f_ref", 20.)
+            f_ref=kwargs.get("f_ref", 20.),
+            approximant_flags=kwargs.get("approximant_flags", {})
         )
         _PlotGeneration.save(
             fig, filename, preliminary=preliminary
         )
 
     def waveform_td_plot(self, label):
         """Generate a time domain waveform plot for a given result file
@@ -567,17 +569,19 @@
             return
         if detectors is None:
             detectors = ["H1", "L1"]
         else:
             detectors = detectors.split("_")
 
         fig = gw._time_domain_waveform(
-            detectors, maxL_samples, f_min=kwargs.get("f_low", 20.0),
+            detectors, maxL_samples, f_start=kwargs.get("f_start", 20.),
+            f_low=kwargs.get("f_low", 20.0),
             f_max=kwargs.get("f_final", 1024.),
-            f_ref=kwargs.get("f_ref", 20.)
+            f_ref=kwargs.get("f_ref", 20.),
+            approximant_flags=kwargs.get("approximant_flags", {})
         )
         _PlotGeneration.save(
             fig, filename, preliminary=preliminary
         )
 
     def gwdata_plots(self, label):
         """Generate all plots associated with the gwdata
@@ -785,25 +789,23 @@
         preliminary: Bool, optional
             if True, add a preliminary watermark to the plot
         """
         filename = os.path.join(savedir, "compare_waveforms.png")
         if os.path.isfile(filename) and checkpoint:
             return
         samples = [maxL_samples[i] for i in labels]
-        f_min = np.max(
-            [kwargs[label]["meta_data"].get("f_low", 20.) for label in labels]
-        )
-        f_max = np.min(
-            [kwargs[label]["meta_data"].get("f_final", 1024.) for label in labels]
-        )
-        f_ref = kwargs[labels[0]]["meta_data"].get("f_ref", 20.)
-        fig = gw._waveform_comparison_plot(
-            samples, colors, labels, f_min=f_min, f_max=f_max,
-            f_ref=f_ref
-        )
+        for num, i in enumerate(labels):
+            samples[num]["approximant_flags"] = kwargs[i]["meta_data"].get(
+                "approximant_flags", {}
+            )
+            _defaults = [20., 20., 1024., 20.]
+            for freq, default in zip(["f_start", "f_low", "f_final", "f_ref"], _defaults):
+                samples[num][freq] = kwargs[i]["meta_data"].get(freq, default)
+
+        fig = gw._waveform_comparison_plot(samples, colors, labels)
         _PlotGeneration.save(
             fig, filename, preliminary=preliminary
         )
 
     def waveform_comparison_td_plot(self, label):
         """Generate a plot to compare the time domain waveform
 
@@ -811,23 +813,24 @@
         ----------
         label: str
             the label for the results file that you wish to plot
         """
         if any(self.approximant[i] == {} for i in self.labels):
             return
 
-        self._waveform_comparison_fd_plot(
+        self._waveform_comparison_td_plot(
             self.savedir, self.maxL_samples, self.labels, self.colors,
-            self.preliminary_comparison_pages, self.checkpoint
+            self.preliminary_comparison_pages, self.checkpoint,
+            **self.file_kwargs
         )
 
     @staticmethod
     def _waveform_comparison_td_plot(
         savedir, maxL_samples, labels, colors, preliminary=False,
-        checkpoint=False
+        checkpoint=False, **kwargs
     ):
         """Generate a plot to compare the time domain waveforms
 
         Parameters
         ----------
         savedir: str
             the directory you wish to save the plot in
@@ -840,15 +843,23 @@
         preliminary: Bool, optional
             if True, add a preliminary watermark to the plot
         """
         filename = os.path.join(savedir, "compare_time_domain_waveforms.png")
         if os.path.isfile(filename) and checkpoint:
             return
         samples = [maxL_samples[i] for i in labels]
-        fig = gw._time_domainwaveform_comparison_plot(samples, colors, labels)
+        for num, i in enumerate(labels):
+            samples[num]["approximant_flags"] = kwargs[i]["meta_data"].get(
+                "approximant_flags", {}
+            )
+            _defaults = [20., 20., 20.]
+            for freq, default in zip(["f_start", "f_low", "f_ref"], _defaults):
+                samples[num][freq] = kwargs[i]["meta_data"].get(freq, default)
+
+        fig = gw._time_domain_waveform_comparison_plot(samples, colors, labels)
         _PlotGeneration.save(
             fig, filename, preliminary=preliminary
         )
 
     def twod_comparison_contour_plot(self, label):
         """Generate 2d comparison contour plots
```

### Comparing `pesummary-1.2.0/pesummary/gw/plots/plot.py` & `pesummary-1.3.0/pesummary/gw/plots/plot.py`

 * *Files 8% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 import numpy as np
 import math
 from scipy.ndimage import gaussian_filter
 from astropy.time import Time
 
 _check_latex_install()
 
-from lal import MSUN_SI, PC_SI
+from lal import MSUN_SI, PC_SI, CreateDict
 
 __author__ = ["Charlie Hoy <charlie.hoy@ligo.org>"]
 try:
     import lalsimulation as lalsim
     LALSIMULATION = True
 except ImportError:
     LALSIMULATION = None
@@ -366,74 +366,77 @@
         fplus = (x * dx - y * dy).sum()
         fcross = (x * dy + y * dx).sum()
 
     return fplus, fcross
 
 
 @no_latex_plot
-def _waveform_plot(detectors, maxL_params, **kwargs):
+def _waveform_plot(
+    detectors, maxL_params, color=None, label=None, fig=None, ax=None,
+    **kwargs
+):
     """Plot the maximum likelihood waveform for a given approximant.
 
     Parameters
     ----------
     detectors: list
         list of detectors that you want to generate waveforms for
     maxL_params: dict
         dictionary of maximum likelihood parameter values
     kwargs: dict
         dictionary of optional keyword arguments
     """
     from gwpy.plot.colors import GW_OBSERVATORY_COLORS
+    from pesummary.gw.waveform import fd_waveform
     if math.isnan(maxL_params["mass_1"]):
         return
     logger.debug("Generating the maximum likelihood waveform plot")
     if not LALSIMULATION:
         raise Exception("lalsimulation could not be imported. please install "
                         "lalsuite to be able to use all features")
-    delta_frequency = kwargs.get("delta_f", 1. / 256)
-    minimum_frequency = kwargs.get("f_min", 5.)
-    maximum_frequency = kwargs.get("f_max", 1000.)
-    frequency_array = np.arange(minimum_frequency, maximum_frequency,
-                                delta_frequency)
 
-    approx = lalsim.GetApproximantFromString(maxL_params["approximant"])
-    mass_1 = maxL_params["mass_1"] * MSUN_SI
-    mass_2 = maxL_params["mass_2"] * MSUN_SI
-    luminosity_distance = maxL_params["luminosity_distance"] * PC_SI * 10**6
-    if "phi_jl" in maxL_params.keys():
-        iota, S1x, S1y, S1z, S2x, S2y, S2z = \
-            lalsim.SimInspiralTransformPrecessingNewInitialConditions(
-                maxL_params["theta_jn"], maxL_params["phi_jl"], maxL_params["tilt_1"],
-                maxL_params["tilt_2"], maxL_params["phi_12"], maxL_params["a_1"],
-                maxL_params["a_2"], mass_1, mass_2, kwargs.get("f_ref", 10.),
-                maxL_params["phase"])
-    else:
-        iota, S1x, S1y, S1z, S2x, S2y, S2z = maxL_params["iota"], 0., 0., 0., \
-            0., 0., 0.
-    phase = maxL_params["phase"] if "phase" in maxL_params.keys() else 0.0
-    for func in [lalsim.SimInspiralChooseFDWaveform, lalsim.SimInspiralFD]:
-        try:
-            h_plus, h_cross = func(
-                mass_1, mass_2, S1x, S1y, S1z, S2x, S2y, S2z, luminosity_distance, iota,
-                phase, 0.0, 0.0, 0.0, delta_frequency, minimum_frequency,
-                maximum_frequency, kwargs.get("f_ref", 10.), None, approx)
-        except Exception:
-            continue
-        break
-    h_plus = h_plus.data.data
-    h_cross = h_cross.data.data
-    h_plus = h_plus[:len(frequency_array)]
-    h_cross = h_cross[:len(frequency_array)]
-    fig, ax = figure(gca=True)
-    colors = [GW_OBSERVATORY_COLORS[i] for i in detectors]
+    if (fig is None) and (ax is None):
+        fig, ax = figure(gca=True)
+    elif ax is None:
+        ax = fig.gca()
+    elif fig is None:
+        raise ValueError("Please provide a figure for plotting")
+    if color is None:
+        color = [GW_OBSERVATORY_COLORS[i] for i in detectors]
+    elif len(color) != len(detectors):
+        raise ValueError(
+            "Please provide a list of colors for each detector"
+        )
+    if label is None:
+        label = detectors
+    elif len(label) != len(detectors):
+        raise ValueError(
+            "Please provide a list of labels for each detector"
+        )
+    minimum_frequency = kwargs.get("f_low", 5.)
+    starting_frequency = kwargs.get("f_start", 5.)
+    maximum_frequency = kwargs.get("f_max", 1000.)
+    approximant_flags = kwargs.get("approximant_flags", {})
     for num, i in enumerate(detectors):
-        ar = __antenna_response(i, maxL_params["ra"], maxL_params["dec"],
-                                maxL_params["psi"], maxL_params["geocent_time"])
-        ax.plot(frequency_array, abs(h_plus * ar[0] + h_cross * ar[1]),
-                color=colors[num], linewidth=1.0, label=i)
+        ht = fd_waveform(
+            maxL_params, maxL_params["approximant"],
+            kwargs.get("delta_f", 1. / 256), starting_frequency,
+            maximum_frequency, f_ref=kwargs.get("f_ref", starting_frequency),
+            project=i, flags=approximant_flags
+        )
+        mask = (
+            (ht.frequencies.value > starting_frequency) *
+            (ht.frequencies.value < maximum_frequency)
+        )
+        ax.plot(
+            ht.frequencies.value[mask], np.abs(ht)[mask], color=color[num],
+            linewidth=1.0, label=label[num]
+        )
+    if starting_frequency < minimum_frequency:
+        ax.axvspan(starting_frequency, minimum_frequency, alpha=0.1, color='grey')
     ax.set_xscale("log")
     ax.set_yscale("log")
     ax.set_xlabel(r"Frequency $[Hz]$")
     ax.set_ylabel(r"Strain")
     ax.grid(visible=True)
     ax.legend(loc="best")
     fig.tight_layout()
@@ -459,56 +462,28 @@
         dictionary of optional keyword arguments
     """
     logger.debug("Generating the maximum likelihood waveform comparison plot "
                  "for H1")
     if not LALSIMULATION:
         raise Exception("LALSimulation could not be imported. Please install "
                         "LALSuite to be able to use all features")
-    delta_frequency = kwargs.get("delta_f", 1. / 256)
-    minimum_frequency = kwargs.get("f_min", 5.)
-    maximum_frequency = kwargs.get("f_max", 1000.)
-    frequency_array = np.arange(minimum_frequency, maximum_frequency,
-                                delta_frequency)
 
     fig, ax = figure(gca=True)
     for num, i in enumerate(maxL_params_list):
-        if math.isnan(i["mass_1"]):
-            continue
-        approx = lalsim.GetApproximantFromString(i["approximant"])
-        mass_1 = i["mass_1"] * MSUN_SI
-        mass_2 = i["mass_2"] * MSUN_SI
-        luminosity_distance = i["luminosity_distance"] * PC_SI * 10**6
-        if "phi_jl" in i.keys():
-            iota, S1x, S1y, S1z, S2x, S2y, S2z = \
-                lalsim.SimInspiralTransformPrecessingNewInitialConditions(
-                    i["theta_jn"], i["phi_jl"], i["tilt_1"],
-                    i["tilt_2"], i["phi_12"], i["a_1"],
-                    i["a_2"], mass_1, mass_2, kwargs.get("f_ref", 10.),
-                    i["phase"])
-        else:
-            iota, S1x, S1y, S1z, S2x, S2y, S2z = i["iota"], 0., 0., 0., \
-                0., 0., 0.
-        phase = i["phase"] if "phase" in i.keys() else 0.0
-        for func in [lalsim.SimInspiralChooseFDWaveform, lalsim.SimInspiralFD]:
-            try:
-                h_plus, h_cross = func(
-                    mass_1, mass_2, S1x, S1y, S1z, S2x, S2y, S2z, luminosity_distance,
-                    iota, phase, 0.0, 0.0, 0.0, delta_frequency, minimum_frequency,
-                    maximum_frequency, kwargs.get("f_ref", 10.), None, approx)
-            except Exception:
-                continue
-            break
-        h_plus = h_plus.data.data
-        h_cross = h_cross.data.data
-        h_plus = h_plus[:len(frequency_array)]
-        h_cross = h_cross[:len(frequency_array)]
-        ar = __antenna_response("H1", i["ra"], i["dec"], i["psi"],
-                                i["geocent_time"])
-        ax.plot(frequency_array, abs(h_plus * ar[0] + h_cross * ar[1]),
-                color=colors[num], label=labels[num], linewidth=2.0)
+        _kwargs = {
+            "f_start": i.get("f_start", 20.),
+            "f_low": i.get("f_low", 20.),
+            "f_max": i.get("f_final", 1024.),
+            "f_ref": i.get("f_ref", 20.),
+            "approximant_flags": i.get("approximant_flags", {})
+        }
+        _ = _waveform_plot(
+            ["H1"], i, fig=fig, ax=ax, color=[colors[num]],
+            label=[labels[num]], **_kwargs
+        )
     ax.set_xscale("log")
     ax.set_yscale("log")
     ax.grid(visible=True)
     ax.legend(loc="best")
     ax.set_xlabel(r"Frequency $[Hz]$")
     ax.set_ylabel(r"Strain")
     fig.tight_layout()
@@ -1024,15 +999,18 @@
         r"$22^{h}$", r"$20^{h}$", r"$18^{h}$", r"$16^{h}$", r"$14^{h}$",
         r"$12^{h}$", r"$10^{h}$", r"$8^{h}$", r"$6^{h}$", r"$4^{h}$",
         r"$2^{h}$"])
     return fig
 
 
 @no_latex_plot
-def _time_domain_waveform(detectors, maxL_params, **kwargs):
+def _time_domain_waveform(
+    detectors, maxL_params, color=None, label=None, fig=None, ax=None,
+    **kwargs
+):
     """
     Plot the maximum likelihood waveform for a given approximant
     in the time domain.
 
     Parameters
     ----------
     detectors: list
@@ -1040,61 +1018,75 @@
     maxL_params: dict
         dictionary of maximum likelihood parameter values
     kwargs: dict
         dictionary of optional keyword arguments
     """
     from gwpy.timeseries import TimeSeries
     from gwpy.plot.colors import GW_OBSERVATORY_COLORS
+    from pesummary.gw.waveform import td_waveform
+    from pesummary.utils.samples_dict import SamplesDict
     if math.isnan(maxL_params["mass_1"]):
         return
     logger.debug("Generating the maximum likelihood waveform time domain plot")
     if not LALSIMULATION:
         raise Exception("lalsimulation could not be imported. please install "
                         "lalsuite to be able to use all features")
-    delta_t = 1. / 4096.
-    minimum_frequency = kwargs.get("f_min", 5.)
-    t_start = maxL_params['geocent_time']
-    t_finish = maxL_params['geocent_time'] + 4.
-    time_array = np.arange(t_start, t_finish, delta_t)
 
-    approx = lalsim.GetApproximantFromString(maxL_params["approximant"])
-    mass_1 = maxL_params["mass_1"] * MSUN_SI
-    mass_2 = maxL_params["mass_2"] * MSUN_SI
-    luminosity_distance = maxL_params["luminosity_distance"] * PC_SI * 10**6
-    if "phi_jl" in maxL_params.keys():
-        iota, S1x, S1y, S1z, S2x, S2y, S2z = \
-            lalsim.SimInspiralTransformPrecessingNewInitialConditions(
-                maxL_params["theta_jn"], maxL_params["phi_jl"], maxL_params["tilt_1"],
-                maxL_params["tilt_2"], maxL_params["phi_12"], maxL_params["a_1"],
-                maxL_params["a_2"], mass_1, mass_2, kwargs.get("f_ref", 10.),
-                maxL_params["phase"])
-    else:
-        iota, S1x, S1y, S1z, S2x, S2y, S2z = maxL_params["iota"], 0., 0., 0., \
-            0., 0., 0.
-    phase = maxL_params["phase"] if "phase" in maxL_params.keys() else 0.0
+    approximant = maxL_params["approximant"]
+    minimum_frequency = kwargs.get("f_low", 5.)
+    starting_frequency = kwargs.get("f_start", 5.)
+    approximant_flags = kwargs.get("approximant_flags", {})
+    _samples = SamplesDict(
+        {
+            key: [item] for key, item in maxL_params.items() if
+            key != "approximant"
+        }
+    )
+    _samples.generate_all_posterior_samples(disable_remnant=True)
+    _samples = {key: item[0] for key, item in _samples.items()}
     chirptime = lalsim.SimIMRPhenomXASDuration(
-        mass_1, mass_2, S1z, S2z, minimum_frequency
+        _samples["mass_1"] * MSUN_SI, _samples["mass_2"] * MSUN_SI,
+        _samples.get("spin_1z", 0), _samples.get("spin_2z", 0),
+        minimum_frequency
     )
     duration = np.max([2**np.ceil(np.log2(chirptime)), 1.0])
-    h_plus, h_cross = lalsim.SimInspiralChooseTDWaveform(
-        mass_1, mass_2, S1x, S1y, S1z, S2x, S2y, S2z, luminosity_distance, iota,
-        phase, 0.0, 0.0, 0.0, delta_t, minimum_frequency,
-        kwargs.get("f_ref", 10.), None, approx)
-
-    fig, ax = figure(gca=True)
-    colors = [GW_OBSERVATORY_COLORS[i] for i in detectors]
+    if (fig is None) and (ax is None):
+        fig, ax = figure(gca=True)
+    elif ax is None:
+        ax = fig.gca()
+    elif fig is None:
+        raise ValueError("Please provide a figure for plotting")
+    if color is None:
+        color = [GW_OBSERVATORY_COLORS[i] for i in detectors]
+    elif len(color) != len(detectors):
+        raise ValueError(
+            "Please provide a list of colors for each detector"
+        )
+    if label is None:
+        label = detectors
+    elif len(label) != len(detectors):
+        raise ValueError(
+            "Please provide a list of labels for each detector"
+        )
     for num, i in enumerate(detectors):
-        ar = __antenna_response(i, maxL_params["ra"], maxL_params["dec"],
-                                maxL_params["psi"], maxL_params["geocent_time"])
-        h_t = h_plus.data.data * ar[0] + h_cross.data.data * ar[1]
-        h_t = TimeSeries(h_t[:], dt=h_plus.deltaT, t0=h_plus.epoch)
-        h_t.times = [float(np.array(i)) + t_start for i in h_t.times]
-        ax.plot(h_t.times, h_t,
-                color=colors[num], linewidth=1.0, label=i)
-        ax.set_xlim([t_start - 0.75 * duration, t_start + duration / 4])
+        ht = td_waveform(
+            maxL_params, approximant, kwargs.get("delta_t", 1. / 4096.),
+            starting_frequency, f_ref=kwargs.get("f_ref", 10.), project=i,
+            flags=approximant_flags
+        )
+        ax.plot(
+            ht.times.value, ht, color=color[num], linewidth=1.0,
+            label=label[num]
+        )
+        ax.set_xlim(
+            [
+                maxL_params["geocent_time"] - 0.75 * duration,
+                maxL_params["geocent_time"] + duration / 4
+            ]
+        )
     ax.set_xlabel(r"Time $[s]$")
     ax.set_ylabel(r"Strain")
     ax.grid(visible=True)
     ax.legend(loc="best")
     fig.tight_layout()
     return fig
 
@@ -1119,56 +1111,29 @@
     """
     from gwpy.timeseries import TimeSeries
     logger.debug("Generating the maximum likelihood time domain waveform "
                  "comparison plot for H1")
     if not LALSIMULATION:
         raise Exception("LALSimulation could not be imported. Please install "
                         "LALSuite to be able to use all features")
-    delta_t = 1. / 4096.
-    minimum_frequency = kwargs.get("f_min", 5.)
-
     fig, ax = figure(gca=True)
     for num, i in enumerate(maxL_params_list):
-        if math.isnan(i["mass_1"]):
-            continue
-        t_start = i['geocent_time']
-        t_finish = i['geocent_time'] + 4.
-        time_array = np.arange(t_start, t_finish, delta_t)
-
-        approx = lalsim.GetApproximantFromString(i["approximant"])
-        mass_1 = i["mass_1"] * MSUN_SI
-        mass_2 = i["mass_2"] * MSUN_SI
-        luminosity_distance = i["luminosity_distance"] * PC_SI * 10**6
-        if "phi_jl" in i.keys():
-            iota, S1x, S1y, S1z, S2x, S2y, S2z = \
-                lalsim.SimInspiralTransformPrecessingNewInitialConditions(
-                    i["theta_jn"], i["phi_jl"], i["tilt_1"],
-                    i["tilt_2"], i["phi_12"], i["a_1"],
-                    i["a_2"], mass_1, mass_2, kwargs.get("f_ref", 10.),
-                    i["phase"])
-        else:
-            iota, S1x, S1y, S1z, S2x, S2y, S2z = i["iota"], 0., 0., 0., \
-                0., 0., 0.
-        phase = i["phase"] if "phase" in i.keys() else 0.0
-        h_plus, h_cross = lalsim.SimInspiralChooseTDWaveform(
-            mass_1, mass_2, S1x, S1y, S1z, S2x, S2y, S2z, luminosity_distance,
-            iota, phase, 0.0, 0.0, 0.0, delta_t, minimum_frequency,
-            kwargs.get("f_ref", 10.), None, approx)
-
-        ar = __antenna_response("H1", i["ra"], i["dec"], i["psi"],
-                                i["geocent_time"])
-        h_t = h_plus.data.data * ar[0] + h_cross.data.data * ar[1]
-        h_t = TimeSeries(h_t[:], dt=h_plus.deltaT, t0=h_plus.epoch)
-        h_t.times = [float(np.array(i)) + t_start for i in h_t.times]
-
-        ax.plot(h_t.times, h_t,
-                color=colors[num], label=labels[num], linewidth=2.0)
+        _kwargs = {
+            "f_start": i.get("f_start", 20.),
+            "f_low": i.get("f_low", 20.),
+            "f_max": i.get("f_final", 1024.),
+            "f_ref": i.get("f_ref", 20.),
+            "approximant_flags": i.get("approximant_flags", {})
+        }
+        _ = _time_domain_waveform(
+            ["H1"], i, fig=fig, ax=ax, color=[colors[num]],
+            label=[labels[num]], **_kwargs
+        )
     ax.set_xlabel(r"Time $[s]$")
     ax.set_ylabel(r"Strain")
-    ax.set_xlim([t_start - 3, t_start + 0.5])
     ax.grid(visible=True)
     ax.legend(loc="best")
     fig.tight_layout()
     return fig
 
 
 def _psd_plot(frequencies, strains, colors=None, labels=None, fmin=None, fmax=None):
```

### Comparing `pesummary-1.2.0/pesummary/gw/plots/public.py` & `pesummary-1.3.0/pesummary/gw/plots/public.py`

 * *Files identical despite different names*

### Comparing `pesummary-1.2.0/pesummary/gw/plots/publication.py` & `pesummary-1.3.0/pesummary/gw/plots/publication.py`

 * *Files identical despite different names*

### Comparing `pesummary-1.2.0/pesummary/gw/plots/tgr.py` & `pesummary-1.3.0/pesummary/gw/plots/tgr.py`

 * *Files identical despite different names*

### Comparing `pesummary-1.2.0/pesummary/gw/pycbc.py` & `pesummary-1.3.0/pesummary/gw/pycbc.py`

 * *Files 6% similar despite different names*

```diff
@@ -126,7 +126,24 @@
         duration = np.max(duration)
         t_len = 2**np.ceil(np.log2(duration) + 1)
         df = 1. / t_len
     flen = int(f_final / df) + 1
     _psd = psd(flen, df, f_low)
     setattr(_psd, "__name__", psd.__name__)
     return {ifo: _psd for ifo in detectors}
+
+
+def interpolate_psd(psd, low_freq_cutoff, delta_f):
+    """Interpolate PSD to a new delta_f
+
+    Parameters
+    ----------
+    low_freq_cutoff: float
+        Frequencies below this value are set to zero.
+    delta_f : float, optional
+        Frequency resolution of the frequency series in Hertz.
+    """
+    from pesummary.gw.file.psd import PSD
+    from pycbc.psd import estimate
+    if isinstance(psd, PSD):
+        psd = psd.to_pycbc(low_freq_cutoff)
+    return estimate.interpolate(psd, delta_f)
```

### Comparing `pesummary-1.2.0/pesummary/gw/reweight.py` & `pesummary-1.3.0/pesummary/gw/reweight.py`

 * *Files identical despite different names*

### Comparing `pesummary-1.2.0/pesummary/gw/waveform.py` & `pesummary-1.3.0/pesummary/gw/waveform.py`

 * *Files 20% similar despite different names*

```diff
@@ -6,15 +6,17 @@
     SimInspiralGetSpinFreqFromApproximant, SIM_INSPIRAL_SPINS_CASEBYCASE,
     SIM_INSPIRAL_SPINS_FLOW
 )
 from pesummary.utils.utils import iterator, logger
 from pesummary.utils.exceptions import EvolveSpinError
 
 __author__ = ["Charlie Hoy <charlie.hoy@ligo.org>"]
-
+_python_module_from_approximant_name = {
+    "SEOBNRv5": "lalsimulation.gwsignal.models.pyseobnr_model"
+}
 
 def _get_spin_freq_from_approximant(approximant):
     """Determine whether the reference frequency is the starting frequency
     for a given approximant string.
 
     Parameters
     ----------
@@ -26,16 +28,15 @@
         approx = getattr(lalsim, approximant)
         return SimInspiralGetSpinFreqFromApproximant(approx)
     except AttributeError:
         from lalsimulation import (
             SIM_INSPIRAL_SPINS_NONPRECESSING, SIM_INSPIRAL_SPINS_F_REF
         )
         # check to see if approximant is in gwsignal
-        from lalsimulation.gwsignal.models import gwsignal_get_waveform_generator
-        approx = gwsignal_get_waveform_generator(approximant)
+        approx = _gwsignal_generator_from_string(approximant)
         meta = approx.metadata
         if meta["type"] == "aligned_spin":
             return SIM_INSPIRAL_SPINS_NONPRECESSING
         elif meta["type"] == "precessing_spin":
             if meta["f_ref_spin"]:
                 return SIM_INSPIRAL_SPINS_F_REF
             return SIM_INSPIRAL_SPINS_FLOW
@@ -85,17 +86,16 @@
     ----------
     approximant: str
         approximant you wish to check
     """
     if hasattr(lalsim, approximant):
         return True
     else:
-        from lalsimulation.gwsignal.models import gwsignal_get_waveform_generator
         try:
-            _ = gwsignal_get_waveform_generator(approximant)
+            _ = _gwsignal_generator_from_string(approximant)
         except (ValueError, NameError):
             return False
         return True
 
 
 def _lal_approximant_from_string(approximant):
     """Return the LAL approximant number given an approximant string
@@ -104,14 +104,85 @@
     ----------
     approximant: str
         approximant you wish to convert
     """
     return lalsim.GetApproximantFromString(approximant)
 
 
+def _gwsignal_generator_from_string(approximant, version="v1", **kwargs):
+    """Return the GW signal generator given an approximant string
+
+    Parameters
+    ----------
+    approximant: str
+        approximant you wish to convert
+    version: str, optional
+        version of gwsignal_get_waveform_generator to use. 'v1' ignores
+        all kwargs and simply passes the approximant name to
+        gwsignal_get_waveform_generator. 'v2' passes the approximant name
+        and python_module to gwsignal_get_waveform_generator. The python_module
+        can either be provided to _gwsignal_generator_from_string directly or if
+        not provided, PESummary will use the stored default values. Default 'v1'
+    kwargs: dict, optional
+        optional kwargs to pass to gwsignal_get_waveform_generator
+    """
+    from lalsimulation.gwsignal.models import gwsignal_get_waveform_generator
+    if version == "v1":
+        return gwsignal_get_waveform_generator(approximant)
+    elif version == "v2":
+        fallback = [
+            value for key, value in _python_module_from_approximant_name.items()
+            if key in approximant
+        ]
+        if len(fallback):
+            fallback = fallback[0]
+        else:
+            fallback = None
+        module = kwargs.get("python_module", fallback)
+        if module is None:
+            raise ValueError(
+                "Please provide a python_module defining the gwsignal "
+                "generator as pesummary does not have a default value"
+            )
+        return gwsignal_get_waveform_generator(
+            approximant, python_module=module
+        )
+    else:
+        raise ValueError(
+            "Unknown version {}. Please use either v1 or v2".format(version)
+        )
+
+
+def _insert_flags(flags, LAL_parameters=None):
+    """Insert waveform specific flags to a LAL dictionary
+
+    Parameters
+    ----------
+    flags: dict
+        dictionary of flags you wish to add to a LAL dictionary
+    LAL_parameters: LALDict, optional
+        An existing LAL dictionary to add mode array to. If not provided, a new
+        LAL dictionary is created. Default None.
+    """
+    if LAL_parameters is None:
+        import lal
+        LAL_parameters = lal.CreateDict()
+    for key, item in flags.items():
+        func = getattr(lalsim, "SimInspiralWaveformParamsInsert" + key, None)
+        if func is not None:
+            func(LAL_parameters, int(item))
+        else:
+            logger.warning(
+                "Unable to add flag {} to LAL dictionary as no function "
+                "SimInspiralWaveformParamsInsert{} found in "
+                "LALSimulation.".format(key, key)
+            )
+    return LAL_parameters
+
+
 def _insert_mode_array(modes, LAL_parameters=None):
     """Add a mode array to a LAL dictionary
 
     Parameters
     ----------
     modes: 2d list
         2d list of modes you wish to add to a LAL dictionary. Must be of the
@@ -248,15 +319,16 @@
     ht = hp * antenna[0] + hc * antenna[1]
     return ht
 
 
 def fd_waveform(
     samples, approximant, delta_f, f_low, f_high, f_ref=20., project=None,
     ind=0, longAscNodes=0., eccentricity=0., LAL_parameters=None,
-    mode_array=None, pycbc=False, flen=None
+    mode_array=None, pycbc=False, flen=None, flags={}, debug=False,
+    **kwargs
 ):
     """Generate a gravitational wave in the frequency domain
 
     Parameters
     ----------
     approximant: str
         name of the approximant to use when generating the waveform
@@ -285,60 +357,76 @@
         [[l1, m1], [l2, m2]]
     pycbc: Bool, optional
         return a the waveform as a pycbc.frequencyseries.FrequencySeries
         object
     flen: int
         Length of the frequency series in samples. Default is None. Only used
         when pycbc=True
+    debug: bool, optional
+        if True, return the model object used to generate the waveform. Only
+        used when the waveform approximant is not in LALSimulation
+    flags: dict, optional
+        waveform specific flags to add to LAL dictionary
+    **kwargs: dict, optional
+        all kwargs passed to _calculate_hp_hc_fd
     """
     from gwpy.frequencyseries import FrequencySeries
 
     waveform_args, _samples = _waveform_args(
         samples, f_ref=f_ref, ind=ind, longAscNodes=longAscNodes,
         eccentricity=eccentricity
     )
-    approx = _lal_approximant_from_string(approximant)
+    if len(flags):
+        LAL_parameters = _insert_flags(
+            flags, LAL_parameters=LAL_parameters
+        )
     if mode_array is not None:
         LAL_parameters = _insert_mode_array(
             mode_array, LAL_parameters=LAL_parameters
         )
-    hp, hc = lalsim.SimInspiralChooseFDWaveform(
-        *waveform_args, delta_f, f_low, f_high, f_ref, LAL_parameters, approx
+    (hp, hc), model = _calculate_hp_hc_fd(
+        waveform_args, delta_f, f_low, f_high, f_ref, LAL_parameters, approximant,
+        debug=True, **kwargs
     )
     hp = FrequencySeries(hp.data.data, df=hp.deltaF, f0=0.)
     hc = FrequencySeries(hc.data.data, df=hc.deltaF, f0=0.)
     if pycbc:
         hp, hc = hp.to_pycbc(), hc.to_pycbc()
         if flen is not None:
             hp.resize(flen)
             hc.resize(flen)
-    if project is None:
+    if project is None and debug:
+        return {"h_plus": hp, "h_cross": hc}, model
+    elif project is None:
         return {"h_plus": hp, "h_cross": hc}
     ht = _project_waveform(
         project, hp, hc, _samples["ra"], _samples["dec"], _samples["psi"],
         _samples["geocent_time"]
     )
+    if debug:
+        return ht, model
     return ht
 
 
 def _wrapper_for_td_waveform(args):
     """Wrapper function for td_waveform for a pool of workers
 
     Parameters
     ----------
     args: tuple
         All args passed to td_waveform
     """
-    return td_waveform(*args)
+    return td_waveform(*args[:-1], **args[-1])
 
 
 def td_waveform(
     samples, approximant, delta_t, f_low, f_ref=20., project=None, ind=0,
     longAscNodes=0., eccentricity=0., LAL_parameters=None, mode_array=None,
-    pycbc=False, level=None, multi_process=1
+    pycbc=False, level=None, multi_process=1, flags={}, debug=False,
+    **kwargs
 ):
     """Generate a gravitational wave in the time domain
 
     Parameters
     ----------
     approximant: str
         name of the approximant to use when generating the waveform
@@ -366,17 +454,24 @@
     pycbc: Bool, optional
         return a the waveform as a pycbc.timeseries.TimeSeries object
     level: list, optional
         the symmetric confidence interval of the time domain waveform. Level
         must be greater than 0 and less than 1
     multi_process: int, optional
         number of cores to run on when generating waveforms. Only used when
-        level is not None
-    """
-    approx = _lal_approximant_from_string(approximant)
+        level is not None,
+    flags: dict, optional
+        waveform specific flags to add to LAL dictionary. Default {}
+    kwargs: dict, optional
+        all kwargs passed to _td_waveform
+    """
+    if len(flags):
+        LAL_parameters = _insert_flags(
+            flags, LAL_parameters=LAL_parameters
+        )
     if mode_array is not None:
         LAL_parameters = _insert_mode_array(
             mode_array, LAL_parameters=LAL_parameters
         )
     if level is not None:
         import multiprocessing
         from pesummary.core.plots.interpolate import Bounded_interp1d
@@ -384,15 +479,15 @@
         _key = list(samples.keys())[0]
         N = len(samples[_key])
         with multiprocessing.Pool(multi_process) as pool:
             args = np.array([
                 [samples] * N, [approximant] * N, [delta_t] * N, [f_low] * N,
                 [f_ref] * N, [project] * N, np.arange(N), [longAscNodes] * N,
                 [eccentricity] * N, [LAL_parameters] * N, [mode_array] * N,
-                [pycbc] * N, [None] * N
+                [pycbc] * N, [None] * N, [kwargs] * N
             ], dtype="object").T
             td_waveform_list = list(
                 iterator(
                     pool.imap(_wrapper_for_td_waveform, args),
                     tqdm=True, logger=logger, total=N,
                     desc="Generating waveforms"
                 )
@@ -450,26 +545,30 @@
             upper = upper["h_t"]
             lower = lower["h_t"]
 
     waveform_args, _samples = _waveform_args(
         samples, ind=ind, longAscNodes=longAscNodes, eccentricity=eccentricity,
         f_ref=f_ref
     )
-    waveform = _td_waveform(
-        waveform_args, approx, delta_t, f_low, f_ref, LAL_parameters, _samples,
-        pycbc=pycbc, project=project
-    )
-    if level is not None:
+    waveform, model = _td_waveform(
+        waveform_args, approximant, delta_t, f_low, f_ref, LAL_parameters,
+        _samples, pycbc=pycbc, project=project, debug=True, **kwargs
+    )
+    if level is not None and debug:
+        return waveform, upper, lower, new_t, model
+    elif level is not None:
         return waveform, upper, lower, new_t
+    elif debug:
+        return waveform, model
     return waveform
 
 
 def _td_waveform(
     waveform_args, approximant, delta_t, f_low, f_ref, LAL_parameters, samples,
-    pycbc=False, project=None
+    pycbc=False, project=None, debug=False, **kwargs
 ):
     """Generate a gravitational wave in the time domain
 
     Parameters
     ----------
     waveform_args: tuple
         args to pass to lalsimulation.SimInspiralChooseTDWaveform
@@ -487,26 +586,34 @@
         dictionary of posterior samples to use when projecting the waveform
         onto a given detector
     pycbc: Bool, optional
         return a the waveform as a pycbc.timeseries.TimeSeries object
     project: str, optional
         name of the detector to project the waveform onto. If None,
         the plus and cross polarizations are returned. Default None
+    debug: bool, optional
+        if True, return the model object used to generate the waveform. Only
+        used when the waveform approximant is not in LALSimulation
+    kwargs: dict, optional
+        all kwargs passed to _calculate_hp_hc_td
     """
     from gwpy.timeseries import TimeSeries
     from astropy.units import Quantity
 
-    hp, hc = lalsim.SimInspiralChooseTDWaveform(
-        *waveform_args, delta_t, f_low, f_ref, LAL_parameters, approximant
+    (hp, hc), model = _calculate_hp_hc_td(
+        waveform_args, delta_t, f_low, f_ref, LAL_parameters, approximant,
+        debug=True, **kwargs
     )
     hp = TimeSeries(hp.data.data, dt=hp.deltaT, t0=hp.epoch)
     hc = TimeSeries(hc.data.data, dt=hc.deltaT, t0=hc.epoch)
     if pycbc:
         hp, hc = hp.to_pycbc(), hc.to_pycbc()
-    if project is None:
+    if project is None and debug:
+        return {"h_plus": hp, "h_cross": hc}, model
+    elif project is None:
         return {"h_plus": hp, "h_cross": hc}
     ht = _project_waveform(
         project, hp, hc, samples["ra"], samples["dec"], samples["psi"],
         samples["geocent_time"]
     )
     if "{}_time".format(project) not in samples.keys():
         from pesummary.gw.conversions import time_in_each_ifo
@@ -516,14 +623,172 @@
             )
         except Exception:
             logger.warning(
                 "Unable to calculate samples for '{}_time' using the provided "
                 "posterior samples. Unable to shift merger to merger time in "
                 "the detector".format(project)
             )
+            if debug:
+                return ht, model
             return ht
     else:
         _detector_time = samples["{}_time".format(project)]
     ht.times = (
         Quantity(ht.times, unit="s") + Quantity(_detector_time, unit="s")
     )
+    if debug:
+        return ht, model
     return ht
+
+
+def _calculate_hp_hc_td(
+    waveform_args, delta_t, f_low, f_ref, LAL_parameters, approximant,
+    debug=False, **kwargs
+):
+    """Calculate the plus and cross polarizations in the time domain.
+    If the approximant is in LALSimulation, the
+    SimInspiralChooseTDWaveform function is used. If the approximant is
+    not in LALSimulation, gwsignal is used
+
+    Parameters
+    ----------
+    waveform_args: tuple
+        args to pass to lalsimulation.SimInspiralChooseTDWaveform
+    delta_t: float
+        spacing between time samples
+    f_low: float
+        frequency to start evaluating the waveform
+    f_ref: float, optional
+        reference frequency
+    LAL_parameters: LALDict
+        LAL dictionary containing accessory parameters. Default None
+    approximant: str
+        lalsimulation approximant number to use when generating a waveform
+    debug: bool, optional
+        if True, return the model object used to generate the waveform. Only
+        used when the waveform approximant is not in LALSimulation
+    **kwargs: dict, optional
+        all kwargs passed to _setup_gwsignal
+    """
+    if hasattr(lalsim, approximant):
+        approx = _lal_approximant_from_string(approximant)
+        result = lalsim.SimInspiralChooseTDWaveform(
+            *waveform_args, delta_t, f_low, f_ref, LAL_parameters, approx
+        )
+        if debug:
+            return result, None
+        return result
+    wfm_gen = _setup_gwsignal(
+        waveform_args, f_low, f_ref, approximant, delta_t=delta_t, **kwargs
+    )
+    hpc = wfm_gen.generate_td_polarizations()
+    if debug:
+        return hpc, wfm_gen
+    return hpc
+
+
+def _calculate_hp_hc_fd(
+    waveform_args, delta_f, f_low, f_high, f_ref, LAL_parameters, approximant,
+    debug=False, **kwargs
+):
+    """Calculate the plus and cross polarizations in the frequency domain.
+    If the approximant is in LALSimulation, the
+    SimInspiralChooseFDWaveform function is used. If the approximant is
+    not in LALSimulation, gwsignal is used
+
+    Parameters
+    ----------
+    waveform_args: tuple
+        args to pass to lalsimulation.SimInspiralChooseFDWaveform
+    delta_f: float
+        spacing between frequency samples
+    f_low: float
+        frequency to start evaluating the waveform
+    f_high: float, optional
+        frequency to stop evaluating the waveform
+    f_ref: float, optional
+        reference frequency
+    LAL_parameters: LALDict
+        LAL dictionary containing accessory parameters. Default None
+    approximant: str
+        lalsimulation approximant number to use when generating a waveform
+    debug: bool, optional
+        if True, return the model object used to generate the waveform. Only
+        used when the waveform approximant is not in LALSimulation
+    """
+    if hasattr(lalsim, approximant):
+        approx = _lal_approximant_from_string(approximant)
+        for func in [lalsim.SimInspiralChooseFDWaveform, lalsim.SimInspiralFD]:
+            try:
+                result = func(
+                    *waveform_args, delta_f, f_low, f_high, f_ref,
+                    LAL_parameters, approx
+                )
+                if debug:
+                    return result, None
+                return result
+            except Exception:
+                continue
+            break
+    wfm_gen = _setup_gwsignal(
+        waveform_args, f_low, f_ref, approximant, delta_f=delta_f,
+        f_high=f_high, **kwargs
+    )
+    hpc = wfm_gen.generate_fd_polarizations()
+    if debug:
+        return hpc, wfm_gen
+    return hpc
+
+
+def _setup_gwsignal(
+    waveform_args, f_low, f_ref, approximant, delta_t=None, delta_f=None,
+    f_high=None, **kwargs
+):
+    """Setup a waveform generator with gwsignal
+
+    Parameters
+    ----------
+    waveform_args: tuple
+        args to pass to lalsimulation.SimInspiralChoose*DWaveform
+    f_low: float
+        frequency to start evaluating the waveform
+    f_ref: float, optional
+        reference frequency
+    approximant: str
+        lalsimulation approximant number to use when generating a waveform
+    delta_t: float, optional
+        spacing between frequency samples
+    delta_f: float, optional
+        spacing between frequency samples
+    f_high: float, optional
+        frequency to stop evaluating the waveform
+    kwargs: dict, optional
+        all kwargs passed to _gwsignal_generator_from_string
+    """
+    from lalsimulation.gwsignal.core.parameter_conventions import (
+        common_units_dictionary
+    )
+    from astropy import units
+    names = [
+        "mass1", "mass2", "spin1x", "spin1y", "spin1z", "spin2x", "spin2y",
+        "spin2z", "distance", "inclination", "phi_ref", "longAscNodes",
+        "eccentricity", "meanPerAno"
+    ]
+    params_dict = {name: waveform_args[ii] for ii, name in enumerate(names)}
+    if delta_t is not None:
+        params_dict["deltaT"] = delta_t
+    if delta_f is not None:
+        params_dict["deltaF"] = delta_f
+    params_dict["f22_start"] = f_low
+    params_dict["f22_ref"] = f_ref
+    if f_high is None:
+        params_dict["f_max"] = 0.5 / params_dict["deltaT"]
+    else:
+        params_dict["f_max"] = f_high
+    wf_gen = _gwsignal_generator_from_string(approximant, **kwargs)
+    for key, item in params_dict.items():
+        params_dict[key] = item * common_units_dictionary.get(key, 1)
+    params_dict["mass1"] *= units.kg
+    params_dict["mass2"] *= units.kg
+    params_dict["distance"] *= units.m
+    wfm_gen = wf_gen._generate_waveform_class(**params_dict)
+    return wfm_gen
```

### Comparing `pesummary-1.2.0/pesummary/gw/webpage/main.py` & `pesummary-1.3.0/pesummary/gw/webpage/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -196,14 +196,17 @@
             if not all(len(np.unique(samples[p])) > 1 for p in params):
                 continue
             headings = self.categorize_parameters(params)
             for hh in headings[::-1]:
                 if len(hh[1]) and hh[0] not in ["others"]:
                     heading = hh[0]
                     break
+                elif len(hh[1]) and "geocent_time" in params:
+                    heading = "timings"
+                    break
             if heading not in sort.keys():
                 sort[heading] = []
             sort[heading] += params
         return sort
 
     def _kde_from_same_samples(self, param, samples):
         """Generate KDEs for a set of samples
@@ -234,15 +237,16 @@
     def make_navbar_for_result_page(self):
         """Make a navbar for the result page homepage
         """
         links = super(_WebpageGeneration, self).make_navbar_for_result_page()
         for num, label in enumerate(self.labels):
             links[label].append(
                 ["2d Histograms", [
-                    {"masses": label}, {"spins": label}, {"location": label}
+                    {"masses": label}, {"spins": label},
+                    {"location": label}, {"timings": label}
                 ]]
             )
             if self.pepredicates_probs[label] is not None:
                 links[label].append({"Classification": label})
         return links
 
     def generate_webpages(self):
@@ -872,18 +876,18 @@
                 "reject": []
             },
             "location": {
                 "accept": [
                     "ra", "dec", "psi", "luminosity_distance", "redshift",
                     "comoving_distance"
                 ],
-                "reject": ["mass_ratio", "radiated", "ram", "ran", "rat"]
+                "reject": ["mass_ratio", "radiated", "ram", "ran", "rat", "time", "delay"]
             },
             "timings": {
-                "accept": ["time"], "reject": []
+                "accept": ["time", "delay"], "reject": []
             },
             "SNR": {
                 "accept": ["snr", "subdominant_multipoles"], "reject": []
             },
             "calibration": {
                 "accept": ["spcal", "recalib", "frequency"],
                 "reject": ["minimum", "tidal_disruption", "quasinormal"]
@@ -910,15 +914,19 @@
 
     def default_comparison_homepage_plots(self):
         """Return a list of default plots for the comparison homepage
         """
         path = self.image_path["other"]
         base = os.path.join(path, "{}.png")
         contents = [
-            [base.format("combined_skymap"), base.format("compare_waveforms")]
+            [
+                base.format("combined_skymap"),
+                base.format("compare_time_domain_waveforms"),
+                base.format("compare_waveforms")
+            ]
         ]
         return contents
 
     def default_corner_params(self):
         """Return a list of default corner parameters used by the corner
         plotting function
         """
```

### Comparing `pesummary-1.2.0/pesummary/gw/webpage/public.py` & `pesummary-1.3.0/pesummary/gw/webpage/public.py`

 * *Files identical despite different names*

### Comparing `pesummary-1.2.0/pesummary/gw/webpage/tgr.py` & `pesummary-1.3.0/pesummary/gw/webpage/tgr.py`

 * *Files identical despite different names*

### Comparing `pesummary-1.2.0/pesummary/io/__init__.py` & `pesummary-1.3.0/pesummary/io/__init__.py`

 * *Files identical despite different names*

### Comparing `pesummary-1.2.0/pesummary/io/read.py` & `pesummary-1.3.0/pesummary/io/read.py`

 * *Files identical despite different names*

### Comparing `pesummary-1.2.0/pesummary/io/write.py` & `pesummary-1.3.0/pesummary/io/write.py`

 * *Files identical despite different names*

### Comparing `pesummary-1.2.0/pesummary/tests/action_test.py` & `pesummary-1.3.0/pesummary/tests/action_test.py`

 * *Files identical despite different names*

### Comparing `pesummary-1.2.0/pesummary/tests/base.py` & `pesummary-1.3.0/pesummary/tests/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -90,27 +90,31 @@
         ))
         for section in sections:
             html.append("%s/html/%s%s_%s%s_%s_all.html" % (outdir, label, num, label, num, section))
         for j in parameters:
             html.append("%s/html/%s%s_%s%s_%s.html" % (outdir, label, num, label, num, j))
         if gw:
             # 2d histogram pages
-            for section in ["location", "masses", "spins"]:
+            for section in ["location", "masses", "spins", "timings"]:
                 if section == "location":
                     pairs = [p for p in gw_2d_plots if "luminosity_distance" in p]
                     if not any(all(p in parameters for p in _) for _ in pairs):
                         continue
                 elif section == "masses":
                     pairs = [p for p in gw_2d_plots if "mass_1" in p]
                     if not any(all(p in parameters for p in _) for _ in pairs):
                         continue
                 elif section == "spins":
                     pairs = [p for p in gw_2d_plots if "chi_p" in p]
                     if not any(all(p in parameters for p in _) for _ in pairs):
                         continue
+                elif section == "timings":
+                    pairs = [p for p in gw_2d_plots if "geocent_time" in p]
+                    if not any(all(p in parameters for p in _) for _ in pairs):
+                        continue
                 html.append("%s/html/%s%s_%s%s_%s.html" % (outdir, label, num, label, num, section))
         if existing_plot:
             html.append("%s/html/%s%s_%s%s_Additional.html" % (outdir, label, num, label, num))
 
     if number > 1:
         html.append("%s/html/Comparison.html" % (outdir))
         html.append("%s/html/Comparison_Custom.html" % (outdir))
@@ -123,15 +127,15 @@
             html.append("%s/html/Comparison_%s_all.html" % (outdir, section))
     return sorted(html)
 
 
 def get_list_of_plots(
     gw=False, number=1, mcmc=False, label=None, outdir=".outdir",
     comparison=True, psd=False, calibration=False, existing_plot=False,
-    expert=False, parameters=[], extra_gw_plots=True
+    expert=False, waveform=False, parameters=[], extra_gw_plots=True
 ):
     """Return a list of plots that should be generated from a typical workflow
     """
     from pesummary.conf import gw_2d_plots
     if not gw and not len(parameters):
         import string
 
@@ -158,14 +162,17 @@
                 plots.append("%s/plots/%s%s_2d_posterior_%s_%s.png" % (
                     outdir, label, num, pair[0], pair[1]
                 ))
         if psd:
             plots.append("%s/plots/%s%s_psd_plot.png" % (outdir, label, num))
         if calibration:
             plots.append("%s/plots/%s%s_calibration_plot.png" % (outdir, label, num))
+        if waveform:
+            plots.append("%s/plots/%s%s_waveform.png" % (outdir, label, num))
+            plots.append("%s/plots/%s%s_waveform_time_domain.png" % (outdir, label, num))
         if existing_plot:
             plots.append("%s/plots/test.png" % (outdir))
         if expert:
             for j in parameters:
                 plots.append("%s/plots/%s%s_2d_contour_%s_log_likelihood.png" % (outdir, label, num, j))
                 plots.append("%s/plots/%s%s_1d_posterior_%s_bootstrap.png" % (outdir, label, num, j))
                 plots.append("%s/plots/%s%s_sample_evolution_%s_log_likelihood_colored.png" % (outdir, label, num, j))
```

### Comparing `pesummary-1.2.0/pesummary/tests/bilby.sh` & `pesummary-1.3.0/pesummary/tests/bilby.sh`

 * *Files identical despite different names*

### Comparing `pesummary-1.2.0/pesummary/tests/bilby_mcmc.sh` & `pesummary-1.3.0/pesummary/tests/bilby_mcmc.sh`

 * *Files identical despite different names*

### Comparing `pesummary-1.2.0/pesummary/tests/bilby_pipe.sh` & `pesummary-1.3.0/pesummary/tests/bilby_pipe.sh`

 * *Files identical despite different names*

### Comparing `pesummary-1.2.0/pesummary/tests/bounded_kde_test.py` & `pesummary-1.3.0/pesummary/tests/bounded_kde_test.py`

 * *Files identical despite different names*

### Comparing `pesummary-1.2.0/pesummary/tests/calibration_test.py` & `pesummary-1.3.0/pesummary/tests/calibration_test.py`

 * *Files identical despite different names*

### Comparing `pesummary-1.2.0/pesummary/tests/classification_test.py` & `pesummary-1.3.0/pesummary/tests/classification_test.py`

 * *Files identical despite different names*

### Comparing `pesummary-1.2.0/pesummary/tests/conversion_test.py` & `pesummary-1.3.0/pesummary/tests/conversion_test.py`

 * *Files identical despite different names*

### Comparing `pesummary-1.2.0/pesummary/tests/cosmology_test.py` & `pesummary-1.3.0/pesummary/tests/cosmology_test.py`

 * *Files identical despite different names*

### Comparing `pesummary-1.2.0/pesummary/tests/executable_test.py` & `pesummary-1.3.0/pesummary/tests/executable_test.py`

 * *Files identical despite different names*

### Comparing `pesummary-1.2.0/pesummary/tests/executables.sh` & `pesummary-1.3.0/pesummary/tests/executables.sh`

 * *Files identical despite different names*

### Comparing `pesummary-1.2.0/pesummary/tests/existing_file.py` & `pesummary-1.3.0/pesummary/tests/existing_file.py`

 * *Files identical despite different names*

### Comparing `pesummary-1.2.0/pesummary/tests/fetch_test.py` & `pesummary-1.3.0/pesummary/tests/fetch_test.py`

 * *Files identical despite different names*

### Comparing `pesummary-1.2.0/pesummary/tests/files/calibration_envelope.txt` & `pesummary-1.3.0/pesummary/tests/files/calibration_envelope.txt`

 * *Files identical despite different names*

### Comparing `pesummary-1.2.0/pesummary/tests/files/config_bilby.ini` & `pesummary-1.3.0/pesummary/tests/files/config_bilby.ini`

 * *Files identical despite different names*

### Comparing `pesummary-1.2.0/pesummary/tests/files/config_lalinference.ini` & `pesummary-1.3.0/pesummary/tests/files/config_lalinference.ini`

 * *Files identical despite different names*

### Comparing `pesummary-1.2.0/pesummary/tests/files/lal_pdf_for_summarytgr.dat.gz` & `pesummary-1.3.0/pesummary/tests/files/lal_pdf_for_summarytgr.dat.gz`

 * *Files identical despite different names*

### Comparing `pesummary-1.2.0/pesummary/tests/files/psd_file.txt` & `pesummary-1.3.0/pesummary/tests/files/psd_file.txt`

 * *Files identical despite different names*

### Comparing `pesummary-1.2.0/pesummary/tests/finish_test.py` & `pesummary-1.3.0/pesummary/tests/finish_test.py`

 * *Files identical despite different names*

### Comparing `pesummary-1.2.0/pesummary/tests/imports.sh` & `pesummary-1.3.0/pesummary/tests/imports.sh`

 * *Files identical despite different names*

### Comparing `pesummary-1.2.0/pesummary/tests/injection_test.py` & `pesummary-1.3.0/pesummary/tests/injection_test.py`

 * *Files identical despite different names*

### Comparing `pesummary-1.2.0/pesummary/tests/input_test.py` & `pesummary-1.3.0/pesummary/tests/input_test.py`

 * *Files identical despite different names*

### Comparing `pesummary-1.2.0/pesummary/tests/lalinference.sh` & `pesummary-1.3.0/pesummary/tests/lalinference.sh`

 * *Files identical despite different names*

### Comparing `pesummary-1.2.0/pesummary/tests/ligo_skymap_test.py` & `pesummary-1.3.0/pesummary/tests/ligo_skymap_test.py`

 * *Files identical despite different names*

### Comparing `pesummary-1.2.0/pesummary/tests/main_injection.xml` & `pesummary-1.3.0/pesummary/tests/main_injection.xml`

 * *Files identical despite different names*

### Comparing `pesummary-1.2.0/pesummary/tests/meta_file_test.py` & `pesummary-1.3.0/pesummary/tests/meta_file_test.py`

 * *Files identical despite different names*

### Comparing `pesummary-1.2.0/pesummary/tests/notebook_test.py` & `pesummary-1.3.0/pesummary/tests/notebook_test.py`

 * *Files identical despite different names*

### Comparing `pesummary-1.2.0/pesummary/tests/plot_test.py` & `pesummary-1.3.0/pesummary/tests/plot_test.py`

 * *Files identical despite different names*

### Comparing `pesummary-1.2.0/pesummary/tests/psd_test.py` & `pesummary-1.3.0/pesummary/tests/psd_test.py`

 * *Files 11% similar despite different names*

```diff
@@ -83,40 +83,60 @@
         g = PSDDict.read(
             common_string="%s/{}_test.dat" % (tmpdir), detectors=["H1", "V1"]
         )
         for ifo, psd in g.items():
             np.testing.assert_almost_equal(psd.frequencies, f[ifo].frequencies)
             np.testing.assert_almost_equal(psd.strains, f[ifo].strains)
 
+    def test_interpolate(self):
+        """Test the interpolate method
+        """
+        f = PSDDict(self.psd_data)
+        g = f.interpolate(
+            f["H1"].low_frequency, f["H1"].delta_f / 2
+        )
+        for ifo, psd in f.items():
+            np.testing.assert_almost_equal(g[ifo].delta_f, psd.delta_f / 2)
+            np.testing.assert_almost_equal(g[ifo].low_frequency, psd.low_frequency)
 
 
 class TestPSD(object):
     """Test the PSD class
     """
     def setup_method(self):
         """Setup the testing class
         """
-        self.obj = PSD([[10, 20], [10, 20]])
+        self.obj = PSD([[10, 20], [10.25, 20], [10.5, 20]])
         if not os.path.isdir(tmpdir):
             os.mkdir(tmpdir)
 
     def teardown_method(self):
         """Remove all files and directories created from this class
         """
         if os.path.isdir(tmpdir):
             shutil.rmtree(tmpdir)
 
     def test_save_to_file(self):
         """Test the save to file method
         """
         self.obj.save_to_file("{}/test.dat".format(tmpdir))
         data = np.genfromtxt("{}/test.dat".format(tmpdir))
-        np.testing.assert_almost_equal(data.T[0], [10, 10])
-        np.testing.assert_almost_equal(data.T[1], [20, 20])
+        np.testing.assert_almost_equal(data.T[0], [10, 10.25, 10.5])
+        np.testing.assert_almost_equal(data.T[1], [20, 20, 20])
 
     def test_invalid_input(self):
         """Test that the appropiate error is raised if the input is wrong
         """
         import pytest
 
         with pytest.raises(IndexError):
             obj = PSD([10, 10])
+
+    def test_interpolate(self):
+        """Test the interpolate method
+        """
+        g = self.obj.interpolate(
+            self.obj.low_frequency,
+            self.obj.delta_f / 2
+        )
+        np.testing.assert_almost_equal(g.delta_f, self.obj.delta_f / 2)
+        np.testing.assert_almost_equal(g.low_frequency, self.obj.low_frequency)
```

### Comparing `pesummary-1.2.0/pesummary/tests/pycbc.sh` & `pesummary-1.3.0/pesummary/tests/pycbc.sh`

 * *Files 2% similar despite different names*

```diff
@@ -7,9 +7,9 @@
 done
 
 
 version=`python -c "import pycbc; print(pycbc.__version__)"`
 curl -O https://raw.githubusercontent.com/gwastro/pycbc/v${version}/examples/inference/single/single.ini
 sed -i '/no-save-data/d' ./single.ini
 sed -i 's/dlogz = 0.01/dlogz = 1000/' ./single.ini
-pycbc_inference --config-file single.ini --output-file ./pycbc.hdf5
-summarypages --webdir ./outdir/webpage --samples ./pycbc.hdf5 --gw --path_to_samples samples
+pycbc_inference --config-file single.ini --output-file ./pycbc.hdf
+summarypages --webdir ./outdir/webpage --samples ./pycbc.hdf --gw --path_to_samples samples
```

### Comparing `pesummary-1.2.0/pesummary/tests/pycbc_test.py` & `pesummary-1.3.0/pesummary/tests/pycbc_test.py`

 * *Files identical despite different names*

### Comparing `pesummary-1.2.0/pesummary/tests/read_test.py` & `pesummary-1.3.0/pesummary/tests/read_test.py`

 * *Files identical despite different names*

### Comparing `pesummary-1.2.0/pesummary/tests/reweight_test.py` & `pesummary-1.3.0/pesummary/tests/reweight_test.py`

 * *Files identical despite different names*

### Comparing `pesummary-1.2.0/pesummary/tests/strain_test.py` & `pesummary-1.3.0/pesummary/tests/strain_test.py`

 * *Files identical despite different names*

### Comparing `pesummary-1.2.0/pesummary/tests/summaryplots_test.py` & `pesummary-1.3.0/pesummary/tests/summaryplots_test.py`

 * *Files 2% similar despite different names*

```diff
@@ -58,15 +58,15 @@
         opts = parser.parse_args(default_arguments)
         inputs = PlottingInput(opts)
         webpage = GWPlotGeneration(inputs)
         webpage.generate_plots()
         plots = sorted(glob(f"{self.dir}/plots/*.png"))
         expected_plots = get_list_of_plots(
             gw=True, label="H1", outdir=self.dir, psd=True,
-            calibration=False
+            calibration=False, waveform=True
         )
         for i, j in zip(expected_plots, plots):
             print(i, j)
         assert all(i == j for i,j in zip(sorted(expected_plots), sorted(plots)))
 
     def test_plot_generation_for_lalinference_structure(self):
         parser = ArgumentParser()
@@ -86,15 +86,15 @@
             "--labels", "H10", "--no_ligo_skymap", "--disable_expert"]
         opts = parser.parse_args(default_arguments)
         inputs = PlottingInput(opts)
         webpage = GWPlotGeneration(inputs)
         webpage.generate_plots()
         plots = sorted(glob(f"{self.dir}/plots/*.png"))
         expected_plots = get_list_of_plots(
-            gw=True, label="H1", outdir=self.dir,
+            gw=True, label="H1", outdir=self.dir, waveform=True
         )
         assert all(i == j for i,j in zip(sorted(expected_plots), sorted(plots)))
 
     def test_plot_generation_for_comparison(self):
         parser = ArgumentParser()
         parser.add_all_known_options_to_parser()
         make_result_file(
@@ -108,26 +108,27 @@
             gw=True, extension="hdf5", bilby=True, outdir=self.dir,
             n_samples=10
         )
         os.rename(
             f"{self.dir}/test.h5", f"{self.dir}/bilby_example.h5"
         )
         default_arguments = [
-            "--approximant", "IMRPhenomPv2", "IMRPhenomP",
+            "--approximant", "IMRPhenomPv2", "IMRPhenomPv3",
             "--webdir", self.dir,
             "--samples", f"{self.dir}/bilby_example.h5",
             f"{self.dir}/lalinference_example.h5",
             "--labels", "H10", "H11", "--no_ligo_skymap", "--disable_expert"]
         opts = parser.parse_args(default_arguments)
         inputs = PlottingInput(opts)
         webpage = GWPlotGeneration(inputs)
         webpage.generate_plots()
         plots = sorted(glob(f"{self.dir}/plots/*.png"))
         expected_plots = get_list_of_plots(
-            gw=True, label="H1", number=2, outdir=self.dir
+            gw=True, label="H1", number=2, outdir=self.dir,
+            waveform=True
         )
         for i,j in zip(sorted(plots), sorted(expected_plots)):
             print(i, j)
         assert all(i == j for i,j in zip(sorted(plots), sorted(expected_plots)))
 
     def test_plot_generation_for_add_to_existing(self):
         parser = ArgumentParser()
@@ -157,25 +158,26 @@
         webpage.generate_plots()
         webpage = GWWebpageGeneration(inputs)
         webpage.generate_webpages()
         meta_file = GWMetaFile(inputs)
         parser = ArgumentParser()
         parser.add_all_known_options_to_parser()
         default_arguments = [
-            "--approximant", "IMRPhenomP",
+            "--approximant", "IMRPhenomPv3",
             "--existing_webdir", self.dir,
             "--samples", f"{self.dir}/lalinference_example.h5",
             "--labels", "H11", "--no_ligo_skymap", "--disable_expert"]
         opts = parser.parse_args(default_arguments)
         inputs = PlottingInput(opts)
         webpage = GWPlotGeneration(inputs) 
         webpage.generate_plots()
         plots = sorted(glob(f"{self.dir}/plots/*.png"))
         expected_plots = get_list_of_plots(
-            gw=True, label="H1", number=2, outdir=self.dir
+            gw=True, label="H1", number=2, outdir=self.dir,
+            waveform=True
         )
         assert all(i == j for i, j in zip(sorted(plots), sorted(expected_plots)))
 
     def test_plot_generation_for_multiple_without_comparison(self):
         parser = ArgumentParser()
         parser.add_all_known_options_to_parser()
         make_result_file(
@@ -189,32 +191,30 @@
             gw=True, extension="hdf5", bilby=True,
             outdir=self.dir, n_samples=10
         )
         os.rename(
             f"{self.dir}/test.h5", f"{self.dir}/bilby_example.h5"
         )
         default_arguments = [
-            "--approximant", "IMRPhenomPv2", "IMRPhenomP",
+            "--approximant", "IMRPhenomPv2", "IMRPhenomPv3",
             "--webdir", self.dir,
             "--samples", f"{self.dir}/bilby_example.h5",
             f"{self.dir}/lalinference_example.h5",
             "--labels", "H10", "H11", "--no_ligo_skymap",
             "--disable_comparison", "--disable_expert"
         ]
         opts = parser.parse_args(default_arguments)
         inputs = PlottingInput(opts)
         webpage = GWPlotGeneration(inputs)
         webpage.generate_plots()
         plots = sorted(glob(f"{self.dir}/plots/*.png"))
         expected_plots = get_list_of_plots(
             gw=True, label="H1", number=2, outdir=self.dir,
-            comparison=False
+            comparison=False, waveform=True
         )
-        for i,j in zip(sorted(plots), sorted(expected_plots)):
-            print(i, j)
         assert all(i == j for i,j in zip(sorted(plots), sorted(expected_plots)))
 
     def test_plot_generation_for_add_to_existing_without_comparison(self):
         parser = ArgumentParser()
         parser.add_all_known_options_to_parser()
         make_result_file(
             gw=True, extension="hdf5", lalinference=True,
@@ -241,23 +241,23 @@
         webpage.generate_plots()
         webpage = GWWebpageGeneration(inputs)
         webpage.generate_webpages()
         meta_file = GWMetaFile(inputs)
         parser = ArgumentParser()
         parser.add_all_known_options_to_parser()
         default_arguments = [
-            "--approximant", "IMRPhenomP",
+            "--approximant", "IMRPhenomPv3",
             "--existing_webdir", self.dir,
             "--samples", f"{self.dir}/lalinference_example.h5",
             "--labels", "H11", "--no_ligo_skymap",
             "--disable_comparison", "--disable_expert"
         ]
         opts = parser.parse_args(default_arguments)
         inputs = PlottingInput(opts)
         webpage = GWPlotGeneration(inputs)
         webpage.generate_plots()
         plots = sorted(glob(f"{self.dir}/plots/*.png"))
         expected_plots = get_list_of_plots(
             gw=True, label="H1", number=2, outdir=self.dir,
-            comparison=False
+            comparison=False, waveform=True
         )
         assert all(i == j for i, j in zip(sorted(plots), sorted(expected_plots)))
```

### Comparing `pesummary-1.2.0/pesummary/tests/utils_test.py` & `pesummary-1.3.0/pesummary/tests/utils_test.py`

 * *Files identical despite different names*

### Comparing `pesummary-1.2.0/pesummary/tests/waveform_test.py` & `pesummary-1.3.0/pesummary/tests/waveform_test.py`

 * *Files identical despite different names*

### Comparing `pesummary-1.2.0/pesummary/tests/webpage_test.py` & `pesummary-1.3.0/pesummary/tests/webpage_test.py`

 * *Files identical despite different names*

### Comparing `pesummary-1.2.0/pesummary/tests/workflow_test.py` & `pesummary-1.3.0/pesummary/tests/workflow_test.py`

 * *Files identical despite different names*

### Comparing `pesummary-1.2.0/pesummary/tests/write_test.py` & `pesummary-1.3.0/pesummary/tests/write_test.py`

 * *Files identical despite different names*

### Comparing `pesummary-1.2.0/pesummary/utils/array.py` & `pesummary-1.3.0/pesummary/utils/array.py`

 * *Files identical despite different names*

### Comparing `pesummary-1.2.0/pesummary/utils/bounded_1d_kde.py` & `pesummary-1.3.0/pesummary/utils/bounded_1d_kde.py`

 * *Files identical despite different names*

### Comparing `pesummary-1.2.0/pesummary/utils/bounded_2d_kde.py` & `pesummary-1.3.0/pesummary/utils/bounded_2d_kde.py`

 * *Files identical despite different names*

### Comparing `pesummary-1.2.0/pesummary/utils/credible_interval.py` & `pesummary-1.3.0/pesummary/utils/credible_interval.py`

 * *Files identical despite different names*

### Comparing `pesummary-1.2.0/pesummary/utils/decorators.py` & `pesummary-1.3.0/pesummary/utils/decorators.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 # Licensed under an MIT style license -- see LICENSE.md
 
 import functools
 import copy
 import numpy as np
+import os
 from pesummary.utils.utils import logger
 
 __author__ = ["Charlie Hoy <charlie.hoy@ligo.org>"]
 
 
 def open_config(index=0):
     """Open a configuration file. The function first looks for a config file
@@ -27,14 +28,22 @@
     @open_config(index=None)
     def open(parameters, samples, config=config):
         print(list(config['condor'].keys()))
     """
     import configparser
 
     def _safe_read(config, config_file):
+        setattr(config, "error", False)
+        if not os.path.isfile(config_file):
+            try:
+                return config.read_string(config_file)
+            except Exception as e:
+                setattr(config, "error", "No such file or directory")
+                return None
+
         setattr(config, "path_to_file", config_file)
         try:
             setattr(config, "error", False)
             return config.read(config_file)
         except configparser.MissingSectionHeaderError:
             with open(config_file, "r") as f:
                 _config = '[config]\n' + f.read()
```

### Comparing `pesummary-1.2.0/pesummary/utils/dict.py` & `pesummary-1.3.0/pesummary/utils/dict.py`

 * *Files identical despite different names*

### Comparing `pesummary-1.2.0/pesummary/utils/kde_list.py` & `pesummary-1.3.0/pesummary/utils/kde_list.py`

 * *Files identical despite different names*

### Comparing `pesummary-1.2.0/pesummary/utils/list.py` & `pesummary-1.3.0/pesummary/utils/list.py`

 * *Files identical despite different names*

### Comparing `pesummary-1.2.0/pesummary/utils/parameters.py` & `pesummary-1.3.0/pesummary/utils/parameters.py`

 * *Files identical despite different names*

### Comparing `pesummary-1.2.0/pesummary/utils/pdf.py` & `pesummary-1.3.0/pesummary/utils/pdf.py`

 * *Files identical despite different names*

### Comparing `pesummary-1.2.0/pesummary/utils/probability_dict.py` & `pesummary-1.3.0/pesummary/utils/probability_dict.py`

 * *Files identical despite different names*

### Comparing `pesummary-1.2.0/pesummary/utils/samples_dict.py` & `pesummary-1.3.0/pesummary/utils/samples_dict.py`

 * *Files identical despite different names*

### Comparing `pesummary-1.2.0/pesummary/utils/tqdm.py` & `pesummary-1.3.0/pesummary/utils/tqdm.py`

 * *Files identical despite different names*

### Comparing `pesummary-1.2.0/pesummary/utils/utils.py` & `pesummary-1.3.0/pesummary/utils/utils.py`

 * *Files identical despite different names*

### Comparing `pesummary-1.2.0/pesummary.egg-info/PKG-INFO` & `pesummary-1.3.0/pesummary.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pesummary
-Version: 1.2.0
+Version: 1.3.0
 Summary: Python package to produce summary pages for Parameter estimation codes
 Author-email: Charlie Hoy <charlie.hoy@ligo.org>
 License: MIT
 Project-URL: Homepage, https://lscsoft.docs.ligo.org/pesummary
 Project-URL: Documentation, https://lscsoft.docs.ligo.org/pesummary/
 Project-URL: Issue Tracker, https://git.ligo.org/lscsoft/pesummary/-/issues/
 Project-URL: Source Code, https://git.ligo.org/lscsoft/pesummary.git
@@ -35,28 +35,29 @@
 Requires-Dist: statsmodels
 Requires-Dist: scipy>=1.8.0
 Requires-Dist: tables
 Requires-Dist: tqdm>=4.44.0
 Provides-Extra: docs
 Requires-Dist: ipykernel; extra == "docs"
 Requires-Dist: nbsphinx; extra == "docs"
+Requires-Dist: pycbc; extra == "docs"
 Requires-Dist: requests; extra == "docs"
 Requires-Dist: Sphinx!=5.0.0,>=4.0.0; extra == "docs"
 Requires-Dist: sphinx-argparse; extra == "docs"
 Requires-Dist: sphinx_rtd_theme; extra == "docs"
 Requires-Dist: sphinx-panels; extra == "docs"
 Requires-Dist: sphinxcontrib-programoutput; extra == "docs"
 Provides-Extra: lint
 Requires-Dist: flake8>=3.7.0; extra == "lint"
 Requires-Dist: flake8-bandit; extra == "lint"
 Provides-Extra: test
 Requires-Dist: astropy!=4.3.0,>=4.0; extra == "test"
 Requires-Dist: beautifulsoup4; extra == "test"
 Requires-Dist: bilby_pipe; extra == "test"
-Requires-Dist: coverage; extra == "test"
+Requires-Dist: coverage<=7.4.4; extra == "test"
 Requires-Dist: coverage-badge; extra == "test"
 Requires-Dist: cython>=0.28.5; extra == "test"
 Requires-Dist: markupsafe==2.0.1; extra == "test"
 Requires-Dist: pycbc>=2.0.3; extra == "test"
 Requires-Dist: pytest>=3.0.0; extra == "test"
 Requires-Dist: pytest-xdist; extra == "test"
 Requires-Dist: pytest-rerunfailures; extra == "test"
```

### Comparing `pesummary-1.2.0/pesummary.egg-info/SOURCES.txt` & `pesummary-1.3.0/pesummary.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -16,15 +16,14 @@
 containers/write_dockerfile.py
 docs/.gitattributes
 docs/citing_pesummary.rst
 docs/conf.py
 docs/front.html.in
 docs/index.rst
 docs/installation.rst
-docs/rtd-environment.yml
 docs/virtual_environment.rst
 docs/what_is_pesummary.rst
 docs/conf/configuration.rst
 docs/core/Array.rst
 docs/core/MCMCSamplesDict.rst
 docs/core/MultiAnalysisSamplesDict.rst
 docs/core/ProbabilityDict.rst
@@ -59,14 +58,15 @@
 docs/core/tutorials/examples/MultiAnalysisReverseTriangle.png
 docs/core/tutorials/examples/MultiAnalysisTriangle.png
 docs/core/tutorials/examples/violin.png
 docs/gw/Conversion.rst
 docs/gw/SamplesDict.rst
 docs/gw/calibration.rst
 docs/gw/classification.rst
+docs/gw/corner.rst
 docs/gw/fetch.rst
 docs/gw/file_formats.rst
 docs/gw/index.rst
 docs/gw/parameters.rst
 docs/gw/pesummary_file.rst
 docs/gw/psd.rst
 docs/gw/read.rst
@@ -78,17 +78,19 @@
 docs/gw/cli/summaryclassification.rst
 docs/gw/cli/summarydetchar.rst
 docs/gw/cli/summarygracedb.rst
 docs/gw/cli/summarypipe.rst
 docs/gw/cli/summaryrecreate.rst
 docs/gw/cli/summaryreview.rst
 docs/gw/cli/summarytgr.rst
+docs/gw/examples/GW150914_corner.png
 docs/gw/examples/GW190412_violin.png
 docs/gw/examples/bounded_violin.png
 docs/gw/examples/gaussian_violin.png
+docs/gw/examples/kde_corner.png
 docs/gw/examples/split_violin.png
 docs/gw/summarypages/about.rst
 docs/gw/summarypages/downloads.rst
 docs/gw/summarypages/home.rst
 docs/gw/summarypages/logging.rst
 docs/gw/summarypages/publication.rst
 docs/gw/summarypages/version.rst
@@ -309,14 +311,15 @@
 pesummary/gw/file/formats/__init__.py
 pesummary/gw/file/formats/base_read.py
 pesummary/gw/file/formats/bilby.py
 pesummary/gw/file/formats/default.py
 pesummary/gw/file/formats/lalinference.py
 pesummary/gw/file/formats/pesummary.py
 pesummary/gw/file/formats/princeton.py
+pesummary/gw/file/formats/pycbc.py
 pesummary/gw/file/formats/xml.py
 pesummary/gw/notebook/__init__.py
 pesummary/gw/notebook/notebook.py
 pesummary/gw/notebook/public.py
 pesummary/gw/plots/__init__.py
 pesummary/gw/plots/bounds.py
 pesummary/gw/plots/cmap.py
```

### Comparing `pesummary-1.2.0/pesummary.egg-info/entry_points.txt` & `pesummary-1.3.0/pesummary.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `pesummary-1.2.0/pyproject.toml` & `pesummary-1.3.0/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -45,14 +45,15 @@
 ]
 dynamic = ['version']
 
 [project.optional-dependencies]
 docs = [
 	"ipykernel",
 	"nbsphinx",
+	"pycbc",
 	"requests",
 	"Sphinx >=4.0.0,!=5.0.0",
 	"sphinx-argparse",
 	"sphinx_rtd_theme",
 	"sphinx-panels",
 	"sphinxcontrib-programoutput",
 ]
@@ -60,15 +61,15 @@
 	"flake8 >=3.7.0",
 	"flake8-bandit",
 ]
 test = [
 	"astropy >=4.0,!=4.3.0",
 	"beautifulsoup4",
 	"bilby_pipe",
-	"coverage",
+	"coverage <=7.4.4", # v7.5.0 incompatible with coverage-badge <=1.1.0
 	"coverage-badge",
 	"cython >=0.28.5",
 	"markupsafe ==2.0.1",
 	"pycbc >=2.0.3",
 	"pytest >=3.0.0",
 	"pytest-xdist",
 	"pytest-rerunfailures",
```

### Comparing `pesummary-1.2.0/setup.py` & `pesummary-1.3.0/setup.py`

 * *Files identical despite different names*

