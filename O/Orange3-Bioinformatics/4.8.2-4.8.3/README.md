# Comparing `tmp/Orange3-Bioinformatics-4.8.2.tar.gz` & `tmp/orange3_bioinformatics-4.8.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Orange3-Bioinformatics-4.8.2.tar", last modified: Wed Mar 20 15:26:28 2024, max compression
+gzip compressed data, was "orange3_bioinformatics-4.8.3.tar", last modified: Mon Jun  3 10:07:16 2024, max compression
```

## Comparing `Orange3-Bioinformatics-4.8.2.tar` & `orange3_bioinformatics-4.8.3.tar`

### file list

```diff
@@ -1,306 +1,306 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 15:26:28.555232 Orange3-Bioinformatics-4.8.2/
--rw-r--r--   0 runner    (1001) docker     (127)      462 2024-03-20 15:26:21.000000 Orange3-Bioinformatics-4.8.2/.coveragerc
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 15:26:28.491232 Orange3-Bioinformatics-4.8.2/.github/
--rw-r--r--   0 runner    (1001) docker     (127)      646 2024-03-20 15:26:21.000000 Orange3-Bioinformatics-4.8.2/.github/FUNDING.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 15:26:28.495232 Orange3-Bioinformatics-4.8.2/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (127)      723 2024-03-20 15:26:21.000000 Orange3-Bioinformatics-4.8.2/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0 runner    (1001) docker     (127)      622 2024-03-20 15:26:21.000000 Orange3-Bioinformatics-4.8.2/.github/ISSUE_TEMPLATE/feature_request.md
--rwxr-xr-x   0 runner    (1001) docker     (127)      217 2024-03-20 15:26:21.000000 Orange3-Bioinformatics-4.8.2/.github/PULL_REQUEST_TEMPLATE.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 15:26:28.495232 Orange3-Bioinformatics-4.8.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      964 2024-03-20 15:26:21.000000 Orange3-Bioinformatics-4.8.2/.github/workflows/lint.yml
--rw-r--r--   0 runner    (1001) docker     (127)      175 2024-03-20 15:26:21.000000 Orange3-Bioinformatics-4.8.2/.github/workflows/rebase.yml
--rw-r--r--   0 runner    (1001) docker     (127)      213 2024-03-20 15:26:21.000000 Orange3-Bioinformatics-4.8.2/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (127)      184 2024-03-20 15:26:21.000000 Orange3-Bioinformatics-4.8.2/.github/workflows/test.yml
--rwxr-xr-x   0 runner    (1001) docker     (127)      755 2024-03-20 15:26:21.000000 Orange3-Bioinformatics-4.8.2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      471 2024-03-20 15:26:21.000000 Orange3-Bioinformatics-4.8.2/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     9025 2024-03-20 15:26:21.000000 Orange3-Bioinformatics-4.8.2/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (127)     3348 2024-03-20 15:26:21.000000 Orange3-Bioinformatics-4.8.2/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (127)    35147 2024-03-20 15:26:21.000000 Orange3-Bioinformatics-4.8.2/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 15:26:28.555232 Orange3-Bioinformatics-4.8.2/Orange3_Bioinformatics.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3012 2024-03-20 15:26:28.000000 Orange3-Bioinformatics-4.8.2/Orange3_Bioinformatics.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    11598 2024-03-20 15:26:28.000000 Orange3-Bioinformatics-4.8.2/Orange3_Bioinformatics.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-20 15:26:28.000000 Orange3-Bioinformatics-4.8.2/Orange3_Bioinformatics.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      223 2024-03-20 15:26:28.000000 Orange3-Bioinformatics-4.8.2/Orange3_Bioinformatics.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-03-20 15:26:28.000000 Orange3-Bioinformatics-4.8.2/Orange3_Bioinformatics.egg-info/namespace_packages.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-20 15:26:28.000000 Orange3-Bioinformatics-4.8.2/Orange3_Bioinformatics.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      351 2024-03-20 15:26:28.000000 Orange3-Bioinformatics-4.8.2/Orange3_Bioinformatics.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-03-20 15:26:28.000000 Orange3-Bioinformatics-4.8.2/Orange3_Bioinformatics.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     3012 2024-03-20 15:26:28.555232 Orange3-Bioinformatics-4.8.2/PKG-INFO
--rwxr-xr-x   0 runner    (1001) docker     (127)     2707 2024-03-20 15:26:21.000000 Orange3-Bioinformatics-4.8.2/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      728 2024-03-20 15:26:21.000000 Orange3-Bioinformatics-4.8.2/README.pypi
--rw-r--r--   0 runner    (1001) docker     (127)      206 2024-03-20 15:26:21.000000 Orange3-Bioinformatics-4.8.2/codecov.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 15:26:28.495232 Orange3-Bioinformatics-4.8.2/doc/
--rw-r--r--   0 runner    (1001) docker     (127)     7464 2024-03-20 15:26:21.000000 Orange3-Bioinformatics-4.8.2/doc/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 15:26:28.499232 Orange3-Bioinformatics-4.8.2/doc/_static/
--rw-r--r--   0 runner    (1001) docker     (127)     1302 2024-03-20 15:26:21.000000 Orange3-Bioinformatics-4.8.2/doc/_static/bioinformatics-sidebar-logo.svg
--rw-r--r--   0 runner    (1001) docker     (127)      537 2024-03-20 15:26:21.000000 Orange3-Bioinformatics-4.8.2/doc/_static/custom.css
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 15:26:28.499232 Orange3-Bioinformatics-4.8.2/doc/_templates/
--rw-r--r--   0 runner    (1001) docker     (127)      314 2024-03-20 15:26:21.000000 Orange3-Bioinformatics-4.8.2/doc/_templates/about.html
--rw-r--r--   0 runner    (1001) docker     (127)      333 2024-03-20 15:26:21.000000 Orange3-Bioinformatics-4.8.2/doc/_templates/globaltoc.html
--rw-r--r--   0 runner    (1001) docker     (127)      495 2024-03-20 15:26:21.000000 Orange3-Bioinformatics-4.8.2/doc/_templates/useful_links.html
--rw-r--r--   0 runner    (1001) docker     (127)    10192 2024-03-20 15:26:21.000000 Orange3-Bioinformatics-4.8.2/doc/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)      113 2024-03-20 15:26:21.000000 Orange3-Bioinformatics-4.8.2/doc/contents.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2319 2024-03-20 15:26:21.000000 Orange3-Bioinformatics-4.8.2/doc/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)     7009 2024-03-20 15:26:21.000000 Orange3-Bioinformatics-4.8.2/doc/make.bat
--rw-r--r--   0 runner    (1001) docker     (127)      439 2024-03-20 15:26:21.000000 Orange3-Bioinformatics-4.8.2/doc/scripting_reference.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 15:26:28.499232 Orange3-Bioinformatics-4.8.2/doc/scripting_references/
--rw-r--r--   0 runner    (1001) docker     (127)      309 2024-03-20 15:26:21.000000 Orange3-Bioinformatics-4.8.2/doc/scripting_references/annotation.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 15:26:28.483232 Orange3-Bioinformatics-4.8.2/doc/scripting_references/code/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 15:26:28.499232 Orange3-Bioinformatics-4.8.2/doc/scripting_references/code/geo/
--rw-r--r--   0 runner    (1001) docker     (127)      705 2024-03-20 15:26:21.000000 Orange3-Bioinformatics-4.8.2/doc/scripting_references/code/geo/dataset_info.py
--rw-r--r--   0 runner    (1001) docker     (127)     1352 2024-03-20 15:26:21.000000 Orange3-Bioinformatics-4.8.2/doc/scripting_references/code/geo/dataset_samples.py
--rw-r--r--   0 runner    (1001) docker     (127)      553 2024-03-20 15:26:21.000000 Orange3-Bioinformatics-4.8.2/doc/scripting_references/code/geo/predict_disease_state.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 15:26:28.499232 Orange3-Bioinformatics-4.8.2/doc/scripting_references/code/go/
--rw-r--r--   0 runner    (1001) docker     (127)      843 2024-03-20 15:26:21.000000 Orange3-Bioinformatics-4.8.2/doc/scripting_references/code/go/enrichment.py
--rw-r--r--   0 runner    (1001) docker     (127)      823 2024-03-20 15:26:21.000000 Orange3-Bioinformatics-4.8.2/doc/scripting_references/code/go/gene_annotations.py
--rw-r--r--   0 runner    (1001) docker     (127)     1113 2024-03-20 15:26:21.000000 Orange3-Bioinformatics-4.8.2/doc/scripting_references/dicty_phenotypes.rst
--rw-r--r--   0 runner    (1001) docker     (127)      965 2024-03-20 15:26:21.000000 Orange3-Bioinformatics-4.8.2/doc/scripting_references/geneset.rst
--rw-r--r--   0 runner    (1001) docker     (127)     4033 2024-03-20 15:26:21.000000 Orange3-Bioinformatics-4.8.2/doc/scripting_references/geo.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2086 2024-03-20 15:26:21.000000 Orange3-Bioinformatics-4.8.2/doc/scripting_references/go.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2816 2024-03-20 15:26:21.000000 Orange3-Bioinformatics-4.8.2/doc/scripting_references/kegg.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1179 2024-03-20 15:26:21.000000 Orange3-Bioinformatics-4.8.2/doc/scripting_references/marker_genes.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2660 2024-03-20 15:26:21.000000 Orange3-Bioinformatics-4.8.2/doc/scripting_references/ncbi_gene.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2180 2024-03-20 15:26:21.000000 Orange3-Bioinformatics-4.8.2/doc/scripting_references/ncbi_taxonomy.rst
--rw-r--r--   0 runner    (1001) docker     (127)      182 2024-03-20 15:26:21.000000 Orange3-Bioinformatics-4.8.2/doc/scripting_references/resolwe.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3949 2024-03-20 15:26:21.000000 Orange3-Bioinformatics-4.8.2/doc/scripting_references/serverfiles.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 15:26:28.503232 Orange3-Bioinformatics-4.8.2/doc/widgets/
--rw-r--r--   0 runner    (1001) docker     (127)     4895 2024-03-20 15:26:21.000000 Orange3-Bioinformatics-4.8.2/doc/widgets/annotate_projection.md
--rw-r--r--   0 runner    (1001) docker     (127)     2752 2024-03-20 15:26:21.000000 Orange3-Bioinformatics-4.8.2/doc/widgets/cluster_analysis.md
--rw-r--r--   0 runner    (1001) docker     (127)     1399 2024-03-20 15:26:21.000000 Orange3-Bioinformatics-4.8.2/doc/widgets/databases_update.md
--rw-r--r--   0 runner    (1001) docker     (127)     1398 2024-03-20 15:26:21.000000 Orange3-Bioinformatics-4.8.2/doc/widgets/dicty_express.md
--rw-r--r--   0 runner    (1001) docker     (127)     4105 2024-03-20 15:26:21.000000 Orange3-Bioinformatics-4.8.2/doc/widgets/differential_expression.md
--rw-r--r--   0 runner    (1001) docker     (127)     2238 2024-03-20 15:26:21.000000 Orange3-Bioinformatics-4.8.2/doc/widgets/gene_set_enrichment.md
--rw-r--r--   0 runner    (1001) docker     (127)     2957 2024-03-20 15:26:21.000000 Orange3-Bioinformatics-4.8.2/doc/widgets/gene_sets.md
--rw-r--r--   0 runner    (1001) docker     (127)     1716 2024-03-20 15:26:21.000000 Orange3-Bioinformatics-4.8.2/doc/widgets/genes.md
--rw-r--r--   0 runner    (1001) docker     (127)     2159 2024-03-20 15:26:21.000000 Orange3-Bioinformatics-4.8.2/doc/widgets/geo_data_sets.md
--rw-r--r--   0 runner    (1001) docker     (127)     5027 2024-03-20 15:26:21.000000 Orange3-Bioinformatics-4.8.2/doc/widgets/go_browser.md
--rw-r--r--   0 runner    (1001) docker     (127)     1866 2024-03-20 15:26:21.000000 Orange3-Bioinformatics-4.8.2/doc/widgets/homologs.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 15:26:28.503232 Orange3-Bioinformatics-4.8.2/doc/widgets/icons/
--rw-r--r--   0 runner    (1001) docker     (127)    35120 2024-03-20 15:26:21.000000 Orange3-Bioinformatics-4.8.2/doc/widgets/icons/annotator.png
--rw-r--r--   0 runner    (1001) docker     (127)     1638 2024-03-20 15:26:21.000000 Orange3-Bioinformatics-4.8.2/doc/widgets/icons/cluster-analysis.png
--rw-r--r--   0 runner    (1001) docker     (127)     1809 2024-03-20 15:26:21.000000 Orange3-Bioinformatics-4.8.2/doc/widgets/icons/databases-update.png
--rw-r--r--   0 runner    (1001) docker     (127)     1423 2024-03-20 15:26:21.000000 Orange3-Bioinformatics-4.8.2/doc/widgets/icons/dicty-express.png
--rw-r--r--   0 runner    (1001) docker     (127)     1639 2024-03-20 15:26:21.000000 Orange3-Bioinformatics-4.8.2/doc/widgets/icons/differential-expression.png
--rw-r--r--   0 runner    (1001) docker     (127)     1719 2024-03-20 15:26:21.000000 Orange3-Bioinformatics-4.8.2/doc/widgets/icons/gene-set-enrichment.png
--rw-r--r--   0 runner    (1001) docker     (127)     1640 2024-03-20 15:26:21.000000 Orange3-Bioinformatics-4.8.2/doc/widgets/icons/genes.png
--rw-r--r--   0 runner    (1001) docker     (127)     1728 2024-03-20 15:26:21.000000 Orange3-Bioinformatics-4.8.2/doc/widgets/icons/geo-data-sets.png
--rw-r--r--   0 runner    (1001) docker     (127)     1943 2024-03-20 15:26:21.000000 Orange3-Bioinformatics-4.8.2/doc/widgets/icons/go-browser.png
--rw-r--r--   0 runner    (1001) docker     (127)     1750 2024-03-20 15:26:21.000000 Orange3-Bioinformatics-4.8.2/doc/widgets/icons/kegg-pathways.png
--rw-r--r--   0 runner    (1001) docker     (127)    13657 2024-03-20 15:26:21.000000 Orange3-Bioinformatics-4.8.2/doc/widgets/icons/volcano-plot.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 15:26:28.487232 Orange3-Bioinformatics-4.8.2/doc/widgets/images/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 15:26:28.507232 Orange3-Bioinformatics-4.8.2/doc/widgets/images/annotate_projection/
--rw-r--r--   0 runner    (1001) docker     (127)   499949 2024-03-20 15:26:21.000000 Orange3-Bioinformatics-4.8.2/doc/widgets/images/annotate_projection/annotator-example.png
--rw-r--r--   0 runner    (1001) docker     (127)   220708 2024-03-20 15:26:21.000000 Orange3-Bioinformatics-4.8.2/doc/widgets/images/annotate_projection/annotator-example2.png
--rw-r--r--   0 runner    (1001) docker     (127)   291477 2024-03-20 15:26:21.000000 Orange3-Bioinformatics-4.8.2/doc/widgets/images/annotate_projection/annotator-stamped.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 15:26:28.507232 Orange3-Bioinformatics-4.8.2/doc/widgets/images/cluster_analysis/
--rw-r--r--   0 runner    (1001) docker     (127)    93180 2024-03-20 15:26:21.000000 Orange3-Bioinformatics-4.8.2/doc/widgets/images/cluster_analysis/Cluster-Analysis-example.png
--rw-r--r--   0 runner    (1001) docker     (127)    50174 2024-03-20 15:26:21.000000 Orange3-Bioinformatics-4.8.2/doc/widgets/images/cluster_analysis/Cluster-Analysis-stamped.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 15:26:28.507232 Orange3-Bioinformatics-4.8.2/doc/widgets/images/database_update/
--rw-r--r--   0 runner    (1001) docker     (127)     8208 2024-03-20 15:26:21.000000 Orange3-Bioinformatics-4.8.2/doc/widgets/images/database_update/Add-Dataset.png
--rw-r--r--   0 runner    (1001) docker     (127)    18674 2024-03-20 15:26:21.000000 Orange3-Bioinformatics-4.8.2/doc/widgets/images/database_update/Databases-Update-stamped.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 15:26:28.507232 Orange3-Bioinformatics-4.8.2/doc/widgets/images/dicty_express/
--rw-r--r--   0 runner    (1001) docker     (127)   168071 2024-03-20 15:26:21.000000 Orange3-Bioinformatics-4.8.2/doc/widgets/images/dicty_express/dictyExpress-Example.png
--rw-r--r--   0 runner    (1001) docker     (127)    36132 2024-03-20 15:26:21.000000 Orange3-Bioinformatics-4.8.2/doc/widgets/images/dicty_express/dictyExpress-stamped.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 15:26:28.511232 Orange3-Bioinformatics-4.8.2/doc/widgets/images/differential_expression/
--rw-r--r--   0 runner    (1001) docker     (127)   176490 2024-03-20 15:26:21.000000 Orange3-Bioinformatics-4.8.2/doc/widgets/images/differential_expression/Differential-Expression-Example.png
--rw-r--r--   0 runner    (1001) docker     (127)    30207 2024-03-20 15:26:21.000000 Orange3-Bioinformatics-4.8.2/doc/widgets/images/differential_expression/Differential-Expression-stamped.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 15:26:28.511232 Orange3-Bioinformatics-4.8.2/doc/widgets/images/gene-sets/
--rw-r--r--   0 runner    (1001) docker     (127)    84453 2024-03-20 15:26:21.000000 Orange3-Bioinformatics-4.8.2/doc/widgets/images/gene-sets/Gene-Sets-example.png
--rw-r--r--   0 runner    (1001) docker     (127)    92526 2024-03-20 15:26:21.000000 Orange3-Bioinformatics-4.8.2/doc/widgets/images/gene-sets/Gene-Sets-example2.png
--rw-r--r--   0 runner    (1001) docker     (127)    28864 2024-03-20 15:26:21.000000 Orange3-Bioinformatics-4.8.2/doc/widgets/images/gene-sets/Gene-Sets-stamped.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 15:26:28.511232 Orange3-Bioinformatics-4.8.2/doc/widgets/images/gene_set_enrichment/
--rw-r--r--   0 runner    (1001) docker     (127)    97576 2024-03-20 15:26:21.000000 Orange3-Bioinformatics-4.8.2/doc/widgets/images/gene_set_enrichment/Gene-Set-Enrichment-Example.png
--rw-r--r--   0 runner    (1001) docker     (127)    55357 2024-03-20 15:26:21.000000 Orange3-Bioinformatics-4.8.2/doc/widgets/images/gene_set_enrichment/Gene-Set-Enrichment-stamped.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 15:26:28.511232 Orange3-Bioinformatics-4.8.2/doc/widgets/images/genes/
--rw-r--r--   0 runner    (1001) docker     (127)   203400 2024-03-20 15:26:21.000000 Orange3-Bioinformatics-4.8.2/doc/widgets/images/genes/genes-Example.png
--rw-r--r--   0 runner    (1001) docker     (127)    57611 2024-03-20 15:26:21.000000 Orange3-Bioinformatics-4.8.2/doc/widgets/images/genes/genes-stamped.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 15:26:28.511232 Orange3-Bioinformatics-4.8.2/doc/widgets/images/geo_data_sets/
--rw-r--r--   0 runner    (1001) docker     (127)   195727 2024-03-20 15:26:21.000000 Orange3-Bioinformatics-4.8.2/doc/widgets/images/geo_data_sets/GEO-Data-Sets-Example.png
--rw-r--r--   0 runner    (1001) docker     (127)    23593 2024-03-20 15:26:21.000000 Orange3-Bioinformatics-4.8.2/doc/widgets/images/geo_data_sets/GEO-Data-Sets-stamped.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 15:26:28.511232 Orange3-Bioinformatics-4.8.2/doc/widgets/images/go_browser/
--rw-r--r--   0 runner    (1001) docker     (127)    24895 2024-03-20 15:26:21.000000 Orange3-Bioinformatics-4.8.2/doc/widgets/images/go_browser/Filter-Select.png
--rw-r--r--   0 runner    (1001) docker     (127)   270407 2024-03-20 15:26:21.000000 Orange3-Bioinformatics-4.8.2/doc/widgets/images/go_browser/GO-Browser-Example.png
--rw-r--r--   0 runner    (1001) docker     (127)    72500 2024-03-20 15:26:21.000000 Orange3-Bioinformatics-4.8.2/doc/widgets/images/go_browser/GO-Browser-stamped.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 15:26:28.515232 Orange3-Bioinformatics-4.8.2/doc/widgets/images/homologs/
--rw-r--r--   0 runner    (1001) docker     (127)    74532 2024-03-20 15:26:21.000000 Orange3-Bioinformatics-4.8.2/doc/widgets/images/homologs/Homologs-Example.png
--rw-r--r--   0 runner    (1001) docker     (127)     6463 2024-03-20 15:26:21.000000 Orange3-Bioinformatics-4.8.2/doc/widgets/images/homologs/Homologs-stamped.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 15:26:28.515232 Orange3-Bioinformatics-4.8.2/doc/widgets/images/kegg_pathways/
--rw-r--r--   0 runner    (1001) docker     (127)   175266 2024-03-20 15:26:21.000000 Orange3-Bioinformatics-4.8.2/doc/widgets/images/kegg_pathways/KEGG-Pathways-Example.png
--rw-r--r--   0 runner    (1001) docker     (127)    51393 2024-03-20 15:26:21.000000 Orange3-Bioinformatics-4.8.2/doc/widgets/images/kegg_pathways/KEGG-Pathways-stamped.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 15:26:28.515232 Orange3-Bioinformatics-4.8.2/doc/widgets/images/marker_genes/
--rw-r--r--   0 runner    (1001) docker     (127)   112894 2024-03-20 15:26:21.000000 Orange3-Bioinformatics-4.8.2/doc/widgets/images/marker_genes/Marker-Genes-example.png
--rw-r--r--   0 runner    (1001) docker     (127)    17416 2024-03-20 15:26:21.000000 Orange3-Bioinformatics-4.8.2/doc/widgets/images/marker_genes/Marker-Genes-stamped.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 15:26:28.515232 Orange3-Bioinformatics-4.8.2/doc/widgets/images/single_sample_scoring/
--rw-r--r--   0 runner    (1001) docker     (127)    81226 2024-03-20 15:26:21.000000 Orange3-Bioinformatics-4.8.2/doc/widgets/images/single_sample_scoring/Single-Sample-Scoring-Example.png
--rw-r--r--   0 runner    (1001) docker     (127)     4440 2024-03-20 15:26:21.000000 Orange3-Bioinformatics-4.8.2/doc/widgets/images/single_sample_scoring/Single-Sample-Scoring-stamped.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 15:26:28.515232 Orange3-Bioinformatics-4.8.2/doc/widgets/images/volcano_plot/
--rw-r--r--   0 runner    (1001) docker     (127)   106338 2024-03-20 15:26:21.000000 Orange3-Bioinformatics-4.8.2/doc/widgets/images/volcano_plot/Volcano-Plot-Example.png
--rw-r--r--   0 runner    (1001) docker     (127)    41623 2024-03-20 15:26:21.000000 Orange3-Bioinformatics-4.8.2/doc/widgets/images/volcano_plot/Volcano-Plot-stamped.png
--rw-r--r--   0 runner    (1001) docker     (127)     1911 2024-03-20 15:26:21.000000 Orange3-Bioinformatics-4.8.2/doc/widgets/kegg_pathways.md
--rw-r--r--   0 runner    (1001) docker     (127)     2401 2024-03-20 15:26:21.000000 Orange3-Bioinformatics-4.8.2/doc/widgets/marker_genes.md
--rw-r--r--   0 runner    (1001) docker     (127)     1608 2024-03-20 15:26:21.000000 Orange3-Bioinformatics-4.8.2/doc/widgets/single_sample_scoring.md
--rw-r--r--   0 runner    (1001) docker     (127)     2523 2024-03-20 15:26:21.000000 Orange3-Bioinformatics-4.8.2/doc/widgets/volcano_plot.md
--rw-r--r--   0 runner    (1001) docker     (127)     4011 2024-03-20 15:26:21.000000 Orange3-Bioinformatics-4.8.2/doc/widgets.json
--rw-r--r--   0 runner    (1001) docker     (127)      361 2024-03-20 15:26:21.000000 Orange3-Bioinformatics-4.8.2/doc/widgets.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 15:26:28.515232 Orange3-Bioinformatics-4.8.2/orangecontrib/
--rwxr-xr-x   0 runner    (1001) docker     (127)      164 2024-03-20 15:26:21.000000 Orange3-Bioinformatics-4.8.2/orangecontrib/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 15:26:28.515232 Orange3-Bioinformatics-4.8.2/orangecontrib/bioinformatics/
--rwxr-xr-x   0 runner    (1001) docker     (127)      252 2024-03-20 15:26:21.000000 Orange3-Bioinformatics-4.8.2/orangecontrib/bioinformatics/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 15:26:28.515232 Orange3-Bioinformatics-4.8.2/orangecontrib/bioinformatics/annotation/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-20 15:26:21.000000 Orange3-Bioinformatics-4.8.2/orangecontrib/bioinformatics/annotation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    23226 2024-03-20 15:26:21.000000 Orange3-Bioinformatics-4.8.2/orangecontrib/bioinformatics/annotation/annotate_projection.py
--rw-r--r--   0 runner    (1001) docker     (127)     9477 2024-03-20 15:26:21.000000 Orange3-Bioinformatics-4.8.2/orangecontrib/bioinformatics/annotation/annotate_samples.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 15:26:28.515232 Orange3-Bioinformatics-4.8.2/orangecontrib/bioinformatics/cluster_analysis/
--rw-r--r--   0 runner    (1001) docker     (127)    13553 2024-03-20 15:26:21.000000 Orange3-Bioinformatics-4.8.2/orangecontrib/bioinformatics/cluster_analysis/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 15:26:28.519232 Orange3-Bioinformatics-4.8.2/orangecontrib/bioinformatics/dicty/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-20 15:26:21.000000 Orange3-Bioinformatics-4.8.2/orangecontrib/bioinformatics/dicty/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4383 2024-03-20 15:26:21.000000 Orange3-Bioinformatics-4.8.2/orangecontrib/bioinformatics/dicty/phenotypes.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 15:26:28.519232 Orange3-Bioinformatics-4.8.2/orangecontrib/bioinformatics/geneset/
--rw-r--r--   0 runner    (1001) docker     (127)     1897 2024-03-20 15:26:21.000000 Orange3-Bioinformatics-4.8.2/orangecontrib/bioinformatics/geneset/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8982 2024-03-20 15:26:21.000000 Orange3-Bioinformatics-4.8.2/orangecontrib/bioinformatics/geneset/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 15:26:28.519232 Orange3-Bioinformatics-4.8.2/orangecontrib/bioinformatics/geo/
--rwxr-xr-x   0 runner    (1001) docker     (127)     5030 2024-03-20 15:26:21.000000 Orange3-Bioinformatics-4.8.2/orangecontrib/bioinformatics/geo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1664 2024-03-20 15:26:21.000000 Orange3-Bioinformatics-4.8.2/orangecontrib/bioinformatics/geo/dataset.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 15:26:28.519232 Orange3-Bioinformatics-4.8.2/orangecontrib/bioinformatics/go/
--rw-r--r--   0 runner    (1001) docker     (127)    27098 2024-03-20 15:26:21.000000 Orange3-Bioinformatics-4.8.2/orangecontrib/bioinformatics/go/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      360 2024-03-20 15:26:21.000000 Orange3-Bioinformatics-4.8.2/orangecontrib/bioinformatics/go/config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 15:26:28.519232 Orange3-Bioinformatics-4.8.2/orangecontrib/bioinformatics/kegg/
--rw-r--r--   0 runner    (1001) docker     (127)    12217 2024-03-20 15:26:21.000000 Orange3-Bioinformatics-4.8.2/orangecontrib/bioinformatics/kegg/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    21289 2024-03-20 15:26:21.000000 Orange3-Bioinformatics-4.8.2/orangecontrib/bioinformatics/kegg/api.py
--rw-r--r--   0 runner    (1001) docker     (127)     2452 2024-03-20 15:26:21.000000 Orange3-Bioinformatics-4.8.2/orangecontrib/bioinformatics/kegg/brite.py
--rw-r--r--   0 runner    (1001) docker     (127)     8347 2024-03-20 15:26:21.000000 Orange3-Bioinformatics-4.8.2/orangecontrib/bioinformatics/kegg/caching.py
--rw-r--r--   0 runner    (1001) docker     (127)      950 2024-03-20 15:26:21.000000 Orange3-Bioinformatics-4.8.2/orangecontrib/bioinformatics/kegg/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)    17989 2024-03-20 15:26:21.000000 Orange3-Bioinformatics-4.8.2/orangecontrib/bioinformatics/kegg/databases.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 15:26:28.519232 Orange3-Bioinformatics-4.8.2/orangecontrib/bioinformatics/kegg/entry/
--rw-r--r--   0 runner    (1001) docker     (127)     5021 2024-03-20 15:26:21.000000 Orange3-Bioinformatics-4.8.2/orangecontrib/bioinformatics/kegg/entry/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5564 2024-03-20 15:26:21.000000 Orange3-Bioinformatics-4.8.2/orangecontrib/bioinformatics/kegg/entry/fields.py
--rw-r--r--   0 runner    (1001) docker     (127)     4913 2024-03-20 15:26:21.000000 Orange3-Bioinformatics-4.8.2/orangecontrib/bioinformatics/kegg/entry/parser.py
--rw-r--r--   0 runner    (1001) docker     (127)     8795 2024-03-20 15:26:21.000000 Orange3-Bioinformatics-4.8.2/orangecontrib/bioinformatics/kegg/pathway.py
--rw-r--r--   0 runner    (1001) docker     (127)      792 2024-03-20 15:26:21.000000 Orange3-Bioinformatics-4.8.2/orangecontrib/bioinformatics/kegg/service.py
--rw-r--r--   0 runner    (1001) docker     (127)     2912 2024-03-20 15:26:21.000000 Orange3-Bioinformatics-4.8.2/orangecontrib/bioinformatics/kegg/types.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 15:26:28.519232 Orange3-Bioinformatics-4.8.2/orangecontrib/bioinformatics/ncbi/
--rwxr-xr-x   0 runner    (1001) docker     (127)       61 2024-03-20 15:26:21.000000 Orange3-Bioinformatics-4.8.2/orangecontrib/bioinformatics/ncbi/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 15:26:28.519232 Orange3-Bioinformatics-4.8.2/orangecontrib/bioinformatics/ncbi/gene/
--rwxr-xr-x   0 runner    (1001) docker     (127)    14166 2024-03-20 15:26:21.000000 Orange3-Bioinformatics-4.8.2/orangecontrib/bioinformatics/ncbi/gene/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1668 2024-03-20 15:26:21.000000 Orange3-Bioinformatics-4.8.2/orangecontrib/bioinformatics/ncbi/gene/config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 15:26:28.523232 Orange3-Bioinformatics-4.8.2/orangecontrib/bioinformatics/ncbi/homologene/
--rw-r--r--   0 runner    (1001) docker     (127)     2093 2024-03-20 15:26:21.000000 Orange3-Bioinformatics-4.8.2/orangecontrib/bioinformatics/ncbi/homologene/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 15:26:28.523232 Orange3-Bioinformatics-4.8.2/orangecontrib/bioinformatics/ncbi/taxonomy/
--rwxr-xr-x   0 runner    (1001) docker     (127)     4487 2024-03-20 15:26:21.000000 Orange3-Bioinformatics-4.8.2/orangecontrib/bioinformatics/ncbi/taxonomy/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    11321 2024-03-20 15:26:21.000000 Orange3-Bioinformatics-4.8.2/orangecontrib/bioinformatics/ncbi/taxonomy/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 15:26:28.523232 Orange3-Bioinformatics-4.8.2/orangecontrib/bioinformatics/preprocess/
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-03-20 15:26:21.000000 Orange3-Bioinformatics-4.8.2/orangecontrib/bioinformatics/preprocess/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2314 2024-03-20 15:26:21.000000 Orange3-Bioinformatics-4.8.2/orangecontrib/bioinformatics/preprocess/normalize.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 15:26:28.523232 Orange3-Bioinformatics-4.8.2/orangecontrib/bioinformatics/resolwe/
--rwxr-xr-x   0 runner    (1001) docker     (127)     1061 2024-03-20 15:26:21.000000 Orange3-Bioinformatics-4.8.2/orangecontrib/bioinformatics/resolwe/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     3335 2024-03-20 15:26:21.000000 Orange3-Bioinformatics-4.8.2/orangecontrib/bioinformatics/resolwe/genapi.py
--rw-r--r--   0 runner    (1001) docker     (127)     3051 2024-03-20 15:26:21.000000 Orange3-Bioinformatics-4.8.2/orangecontrib/bioinformatics/resolwe/resapi.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2560 2024-03-20 15:26:21.000000 Orange3-Bioinformatics-4.8.2/orangecontrib/bioinformatics/resolwe/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 15:26:28.523232 Orange3-Bioinformatics-4.8.2/orangecontrib/bioinformatics/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      467 2024-03-20 15:26:21.000000 Orange3-Bioinformatics-4.8.2/orangecontrib/bioinformatics/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 15:26:28.523232 Orange3-Bioinformatics-4.8.2/orangecontrib/bioinformatics/tests/annotation/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-20 15:26:21.000000 Orange3-Bioinformatics-4.8.2/orangecontrib/bioinformatics/tests/annotation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    15903 2024-03-20 15:26:21.000000 Orange3-Bioinformatics-4.8.2/orangecontrib/bioinformatics/tests/annotation/test_annotate_projection.py
--rw-r--r--   0 runner    (1001) docker     (127)    14374 2024-03-20 15:26:21.000000 Orange3-Bioinformatics-4.8.2/orangecontrib/bioinformatics/tests/annotation/test_annotate_samples.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 15:26:28.523232 Orange3-Bioinformatics-4.8.2/orangecontrib/bioinformatics/tests/kegg/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-20 15:26:21.000000 Orange3-Bioinformatics-4.8.2/orangecontrib/bioinformatics/tests/kegg/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3065 2024-03-20 15:26:21.000000 Orange3-Bioinformatics-4.8.2/orangecontrib/bioinformatics/tests/kegg/test_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     2849 2024-03-20 15:26:21.000000 Orange3-Bioinformatics-4.8.2/orangecontrib/bioinformatics/tests/kegg/test_databases.py
--rw-r--r--   0 runner    (1001) docker     (127)     1741 2024-03-20 15:26:21.000000 Orange3-Bioinformatics-4.8.2/orangecontrib/bioinformatics/tests/kegg/test_entry.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 15:26:28.523232 Orange3-Bioinformatics-4.8.2/orangecontrib/bioinformatics/tests/ncbi/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-20 15:26:21.000000 Orange3-Bioinformatics-4.8.2/orangecontrib/bioinformatics/tests/ncbi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3710 2024-03-20 15:26:21.000000 Orange3-Bioinformatics-4.8.2/orangecontrib/bioinformatics/tests/ncbi/test_gene.py
--rw-r--r--   0 runner    (1001) docker     (127)      585 2024-03-20 15:26:21.000000 Orange3-Bioinformatics-4.8.2/orangecontrib/bioinformatics/tests/ncbi/test_homologene.py
--rw-r--r--   0 runner    (1001) docker     (127)     3488 2024-03-20 15:26:21.000000 Orange3-Bioinformatics-4.8.2/orangecontrib/bioinformatics/tests/ncbi/test_taxonomy.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 15:26:28.527232 Orange3-Bioinformatics-4.8.2/orangecontrib/bioinformatics/tests/preprocess/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-20 15:26:21.000000 Orange3-Bioinformatics-4.8.2/orangecontrib/bioinformatics/tests/preprocess/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1626 2024-03-20 15:26:21.000000 Orange3-Bioinformatics-4.8.2/orangecontrib/bioinformatics/tests/preprocess/test_normalize.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 15:26:28.527232 Orange3-Bioinformatics-4.8.2/orangecontrib/bioinformatics/tests/resolwe/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-20 15:26:21.000000 Orange3-Bioinformatics-4.8.2/orangecontrib/bioinformatics/tests/resolwe/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1995 2024-03-20 15:26:21.000000 Orange3-Bioinformatics-4.8.2/orangecontrib/bioinformatics/tests/resolwe/test_genapi.py
--rw-r--r--   0 runner    (1001) docker     (127)     3195 2024-03-20 15:26:21.000000 Orange3-Bioinformatics-4.8.2/orangecontrib/bioinformatics/tests/test_geneset.py
--rw-r--r--   0 runner    (1001) docker     (127)     2549 2024-03-20 15:26:21.000000 Orange3-Bioinformatics-4.8.2/orangecontrib/bioinformatics/tests/test_geo.py
--rw-r--r--   0 runner    (1001) docker     (127)     4060 2024-03-20 15:26:21.000000 Orange3-Bioinformatics-4.8.2/orangecontrib/bioinformatics/tests/test_statistics.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 15:26:28.527232 Orange3-Bioinformatics-4.8.2/orangecontrib/bioinformatics/tests/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-20 15:26:21.000000 Orange3-Bioinformatics-4.8.2/orangecontrib/bioinformatics/tests/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1825 2024-03-20 15:26:21.000000 Orange3-Bioinformatics-4.8.2/orangecontrib/bioinformatics/tests/utils/test_gui.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 15:26:28.527232 Orange3-Bioinformatics-4.8.2/orangecontrib/bioinformatics/tests/widgets/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-20 15:26:21.000000 Orange3-Bioinformatics-4.8.2/orangecontrib/bioinformatics/tests/widgets/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 15:26:28.527232 Orange3-Bioinformatics-4.8.2/orangecontrib/bioinformatics/tests/widgets/components/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-20 15:26:21.000000 Orange3-Bioinformatics-4.8.2/orangecontrib/bioinformatics/tests/widgets/components/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6181 2024-03-20 15:26:21.000000 Orange3-Bioinformatics-4.8.2/orangecontrib/bioinformatics/tests/widgets/components/test_gene_set_selection.py
--rw-r--r--   0 runner    (1001) docker     (127)     8052 2024-03-20 15:26:21.000000 Orange3-Bioinformatics-4.8.2/orangecontrib/bioinformatics/tests/widgets/components/test_resolwe.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 15:26:28.527232 Orange3-Bioinformatics-4.8.2/orangecontrib/bioinformatics/tests/widgets/data/
--rw-r--r--   0 runner    (1001) docker     (127)     3828 2024-03-20 15:26:21.000000 Orange3-Bioinformatics-4.8.2/orangecontrib/bioinformatics/tests/widgets/data/genes.tab
--rw-r--r--   0 runner    (1001) docker     (127)    12006 2024-03-20 15:26:21.000000 Orange3-Bioinformatics-4.8.2/orangecontrib/bioinformatics/tests/widgets/data/markers-panglao.pkl
--rw-r--r--   0 runner    (1001) docker     (127)    16086 2024-03-20 15:26:21.000000 Orange3-Bioinformatics-4.8.2/orangecontrib/bioinformatics/tests/widgets/test_OWAnnotateProjection.py
--rw-r--r--   0 runner    (1001) docker     (127)     1351 2024-03-20 15:26:21.000000 Orange3-Bioinformatics-4.8.2/orangecontrib/bioinformatics/tests/widgets/test_OWDifferentialExpression.py
--rw-r--r--   0 runner    (1001) docker     (127)     2519 2024-03-20 15:26:21.000000 Orange3-Bioinformatics-4.8.2/orangecontrib/bioinformatics/tests/widgets/test_OWGEODatasets.py
--rw-r--r--   0 runner    (1001) docker     (127)     2986 2024-03-20 15:26:21.000000 Orange3-Bioinformatics-4.8.2/orangecontrib/bioinformatics/tests/widgets/test_OWGeneSets.py
--rw-r--r--   0 runner    (1001) docker     (127)     3894 2024-03-20 15:26:21.000000 Orange3-Bioinformatics-4.8.2/orangecontrib/bioinformatics/tests/widgets/test_OWGenes.py
--rw-r--r--   0 runner    (1001) docker     (127)     6113 2024-03-20 15:26:21.000000 Orange3-Bioinformatics-4.8.2/orangecontrib/bioinformatics/tests/widgets/test_OWGenialisExpressions.py
--rw-r--r--   0 runner    (1001) docker     (127)     3024 2024-03-20 15:26:21.000000 Orange3-Bioinformatics-4.8.2/orangecontrib/bioinformatics/tests/widgets/test_OWHomologs.py
--rw-r--r--   0 runner    (1001) docker     (127)    28933 2024-03-20 15:26:21.000000 Orange3-Bioinformatics-4.8.2/orangecontrib/bioinformatics/tests/widgets/test_OWMarkerGenes.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 15:26:28.527232 Orange3-Bioinformatics-4.8.2/orangecontrib/bioinformatics/utils/
--rwxr-xr-x   0 runner    (1001) docker     (127)      542 2024-03-20 15:26:21.000000 Orange3-Bioinformatics-4.8.2/orangecontrib/bioinformatics/utils/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1604 2024-03-20 15:26:21.000000 Orange3-Bioinformatics-4.8.2/orangecontrib/bioinformatics/utils/serverfiles.py
--rw-r--r--   0 runner    (1001) docker     (127)    11389 2024-03-20 15:26:21.000000 Orange3-Bioinformatics-4.8.2/orangecontrib/bioinformatics/utils/statistics.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 15:26:28.531232 Orange3-Bioinformatics-4.8.2/orangecontrib/bioinformatics/widgets/
--rw-r--r--   0 runner    (1001) docker     (127)    36783 2024-03-20 15:26:21.000000 Orange3-Bioinformatics-4.8.2/orangecontrib/bioinformatics/widgets/OWAnnotateProjection.py
--rw-r--r--   0 runner    (1001) docker     (127)    31640 2024-03-20 15:26:21.000000 Orange3-Bioinformatics-4.8.2/orangecontrib/bioinformatics/widgets/OWClusterAnalysis.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    32295 2024-03-20 15:26:21.000000 Orange3-Bioinformatics-4.8.2/orangecontrib/bioinformatics/widgets/OWDatabasesUpdate.py
--rw-r--r--   0 runner    (1001) docker     (127)    46600 2024-03-20 15:26:21.000000 Orange3-Bioinformatics-4.8.2/orangecontrib/bioinformatics/widgets/OWDifferentialExpression.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    20747 2024-03-20 15:26:21.000000 Orange3-Bioinformatics-4.8.2/orangecontrib/bioinformatics/widgets/OWGEODatasets.py
--rw-r--r--   0 runner    (1001) docker     (127)    41488 2024-03-20 15:26:21.000000 Orange3-Bioinformatics-4.8.2/orangecontrib/bioinformatics/widgets/OWGOBrowser.py
--rw-r--r--   0 runner    (1001) docker     (127)    20668 2024-03-20 15:26:21.000000 Orange3-Bioinformatics-4.8.2/orangecontrib/bioinformatics/widgets/OWGeneSetEnrichment.py
--rw-r--r--   0 runner    (1001) docker     (127)    13325 2024-03-20 15:26:21.000000 Orange3-Bioinformatics-4.8.2/orangecontrib/bioinformatics/widgets/OWGeneSets.py
--rw-r--r--   0 runner    (1001) docker     (127)    24379 2024-03-20 15:26:21.000000 Orange3-Bioinformatics-4.8.2/orangecontrib/bioinformatics/widgets/OWGenes.py
--rw-r--r--   0 runner    (1001) docker     (127)    25847 2024-03-20 15:26:21.000000 Orange3-Bioinformatics-4.8.2/orangecontrib/bioinformatics/widgets/OWGenialisExpressions.py
--rw-r--r--   0 runner    (1001) docker     (127)     9305 2024-03-20 15:26:21.000000 Orange3-Bioinformatics-4.8.2/orangecontrib/bioinformatics/widgets/OWHomologs.py
--rw-r--r--   0 runner    (1001) docker     (127)    31662 2024-03-20 15:26:21.000000 Orange3-Bioinformatics-4.8.2/orangecontrib/bioinformatics/widgets/OWKEGGPathwayBrowser.py
--rw-r--r--   0 runner    (1001) docker     (127)    43015 2024-03-20 15:26:21.000000 Orange3-Bioinformatics-4.8.2/orangecontrib/bioinformatics/widgets/OWMarkerGenes.py
--rw-r--r--   0 runner    (1001) docker     (127)     4900 2024-03-20 15:26:21.000000 Orange3-Bioinformatics-4.8.2/orangecontrib/bioinformatics/widgets/OWSingleSampleScoring.py
--rw-r--r--   0 runner    (1001) docker     (127)     5822 2024-03-20 15:26:21.000000 Orange3-Bioinformatics-4.8.2/orangecontrib/bioinformatics/widgets/OWVolcanoPlot.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    11169 2024-03-20 15:26:21.000000 Orange3-Bioinformatics-4.8.2/orangecontrib/bioinformatics/widgets/OWdictyExpress.py
--rw-r--r--   0 runner    (1001) docker     (127)      698 2024-03-20 15:26:21.000000 Orange3-Bioinformatics-4.8.2/orangecontrib/bioinformatics/widgets/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 15:26:28.531232 Orange3-Bioinformatics-4.8.2/orangecontrib/bioinformatics/widgets/components/
--rw-r--r--   0 runner    (1001) docker     (127)       82 2024-03-20 15:26:21.000000 Orange3-Bioinformatics-4.8.2/orangecontrib/bioinformatics/widgets/components/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10742 2024-03-20 15:26:21.000000 Orange3-Bioinformatics-4.8.2/orangecontrib/bioinformatics/widgets/components/gene_set_selection.py
--rw-r--r--   0 runner    (1001) docker     (127)    17254 2024-03-20 15:26:21.000000 Orange3-Bioinformatics-4.8.2/orangecontrib/bioinformatics/widgets/components/resolwe.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 15:26:28.551232 Orange3-Bioinformatics-4.8.2/orangecontrib/bioinformatics/widgets/icons/
--rwxr-xr-x   0 runner    (1001) docker     (127)     1302 2024-03-20 15:26:21.000000 Orange3-Bioinformatics-4.8.2/orangecontrib/bioinformatics/widgets/icons/Category-Bioinformatics.svg
--rw-r--r--   0 runner    (1001) docker     (127)     4230 2024-03-20 15:26:21.000000 Orange3-Bioinformatics-4.8.2/orangecontrib/bioinformatics/widgets/icons/OWAnnotateProjection.svg
--rw-r--r--   0 runner    (1001) docker     (127)     1396 2024-03-20 15:26:21.000000 Orange3-Bioinformatics-4.8.2/orangecontrib/bioinformatics/widgets/icons/OWClusterAnalysis.svg
--rwxr-xr-x   0 runner    (1001) docker     (127)     2519 2024-03-20 15:26:21.000000 Orange3-Bioinformatics-4.8.2/orangecontrib/bioinformatics/widgets/icons/OWDatabasesUpdate.svg
--rw-r--r--   0 runner    (1001) docker     (127)      954 2024-03-20 15:26:21.000000 Orange3-Bioinformatics-4.8.2/orangecontrib/bioinformatics/widgets/icons/OWDifferentialExpression.svg
--rwxr-xr-x   0 runner    (1001) docker     (127)     1960 2024-03-20 15:26:21.000000 Orange3-Bioinformatics-4.8.2/orangecontrib/bioinformatics/widgets/icons/OWGEODatasets.svg
--rw-r--r--   0 runner    (1001) docker     (127)     1659 2024-03-20 15:26:21.000000 Orange3-Bioinformatics-4.8.2/orangecontrib/bioinformatics/widgets/icons/OWGOBrowser.svg
--rw-r--r--   0 runner    (1001) docker     (127)     1147 2024-03-20 15:26:21.000000 Orange3-Bioinformatics-4.8.2/orangecontrib/bioinformatics/widgets/icons/OWGeneInfo.svg
--rw-r--r--   0 runner    (1001) docker     (127)     1971 2024-03-20 15:26:21.000000 Orange3-Bioinformatics-4.8.2/orangecontrib/bioinformatics/widgets/icons/OWGeneSetEnrichment.svg
--rw-r--r--   0 runner    (1001) docker     (127)     1189 2024-03-20 15:26:21.000000 Orange3-Bioinformatics-4.8.2/orangecontrib/bioinformatics/widgets/icons/OWGeneSets.svg
--rw-r--r--   0 runner    (1001) docker     (127)     2486 2024-03-20 15:26:21.000000 Orange3-Bioinformatics-4.8.2/orangecontrib/bioinformatics/widgets/icons/OWGenialisExpressions.svg
--rw-r--r--   0 runner    (1001) docker     (127)      829 2024-03-20 15:26:21.000000 Orange3-Bioinformatics-4.8.2/orangecontrib/bioinformatics/widgets/icons/OWHomologs.svg
--rw-r--r--   0 runner    (1001) docker     (127)     1980 2024-03-20 15:26:21.000000 Orange3-Bioinformatics-4.8.2/orangecontrib/bioinformatics/widgets/icons/OWKEGGPathwayBrowser.svg
--rw-r--r--   0 runner    (1001) docker     (127)     1256 2024-03-20 15:26:21.000000 Orange3-Bioinformatics-4.8.2/orangecontrib/bioinformatics/widgets/icons/OWMarkerGenes.svg
--rw-r--r--   0 runner    (1001) docker     (127)     1023 2024-03-20 15:26:21.000000 Orange3-Bioinformatics-4.8.2/orangecontrib/bioinformatics/widgets/icons/OWSingleSampleScoring.svg
--rw-r--r--   0 runner    (1001) docker     (127)     2154 2024-03-20 15:26:21.000000 Orange3-Bioinformatics-4.8.2/orangecontrib/bioinformatics/widgets/icons/OWVolcanoPlot.svg
--rwxr-xr-x   0 runner    (1001) docker     (127) 12157657 2024-03-20 15:26:21.000000 Orange3-Bioinformatics-4.8.2/orangecontrib/bioinformatics/widgets/icons/OWdictyExpress.png
--rw-r--r--   0 runner    (1001) docker     (127)     2864 2024-03-20 15:26:21.000000 Orange3-Bioinformatics-4.8.2/orangecontrib/bioinformatics/widgets/icons/OWdictyExpress.svg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 15:26:28.555232 Orange3-Bioinformatics-4.8.2/orangecontrib/bioinformatics/widgets/utils/
--rw-r--r--   0 runner    (1001) docker     (127)      575 2024-03-20 15:26:21.000000 Orange3-Bioinformatics-4.8.2/orangecontrib/bioinformatics/widgets/utils/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1217 2024-03-20 15:26:21.000000 Orange3-Bioinformatics-4.8.2/orangecontrib/bioinformatics/widgets/utils/concurrent.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     4121 2024-03-20 15:26:21.000000 Orange3-Bioinformatics-4.8.2/orangecontrib/bioinformatics/widgets/utils/data.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 15:26:28.555232 Orange3-Bioinformatics-4.8.2/orangecontrib/bioinformatics/widgets/utils/gui/
--rw-r--r--   0 runner    (1001) docker     (127)     4943 2024-03-20 15:26:21.000000 Orange3-Bioinformatics-4.8.2/orangecontrib/bioinformatics/widgets/utils/gui/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3474 2024-03-20 15:26:21.000000 Orange3-Bioinformatics-4.8.2/orangecontrib/bioinformatics/widgets/utils/gui/gene_scoring.py
--rw-r--r--   0 runner    (1001) docker     (127)     7267 2024-03-20 15:26:21.000000 Orange3-Bioinformatics-4.8.2/orangecontrib/bioinformatics/widgets/utils/gui/gene_sets.py
--rw-r--r--   0 runner    (1001) docker     (127)    13615 2024-03-20 15:26:21.000000 Orange3-Bioinformatics-4.8.2/orangecontrib/bioinformatics/widgets/utils/gui/label_selection.py
--rw-r--r--   0 runner    (1001) docker     (127)     5722 2024-03-20 15:26:21.000000 Orange3-Bioinformatics-4.8.2/orangecontrib/bioinformatics/widgets/utils/gui/list_completer.py
--rw-r--r--   0 runner    (1001) docker     (127)      567 2024-03-20 15:26:21.000000 Orange3-Bioinformatics-4.8.2/orangecontrib/bioinformatics/widgets/utils/itemdelegates.py
--rw-r--r--   0 runner    (1001) docker     (127)     2862 2024-03-20 15:26:21.000000 Orange3-Bioinformatics-4.8.2/orangecontrib/bioinformatics/widgets/utils/itemmodels.py
--rw-r--r--   0 runner    (1001) docker     (127)     2764 2024-03-20 15:26:21.000000 Orange3-Bioinformatics-4.8.2/orangecontrib/bioinformatics/widgets/utils/settings.py
--rw-r--r--   0 runner    (1001) docker     (127)      710 2024-03-20 15:26:21.000000 Orange3-Bioinformatics-4.8.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      235 2024-03-20 15:26:21.000000 Orange3-Bioinformatics-4.8.2/readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2253 2024-03-20 15:26:28.555232 Orange3-Bioinformatics-4.8.2/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (127)     1229 2024-03-20 15:26:21.000000 Orange3-Bioinformatics-4.8.2/setup.py
--rw-r--r--   0 runner    (1001) docker     (127)     1718 2024-03-20 15:26:21.000000 Orange3-Bioinformatics-4.8.2/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 10:07:16.539341 orange3_bioinformatics-4.8.3/
+-rw-r--r--   0 runner    (1001) docker     (127)      462 2024-06-03 10:07:11.000000 orange3_bioinformatics-4.8.3/.coveragerc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 10:07:16.479340 orange3_bioinformatics-4.8.3/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)      646 2024-06-03 10:07:11.000000 orange3_bioinformatics-4.8.3/.github/FUNDING.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 10:07:16.479340 orange3_bioinformatics-4.8.3/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (127)      723 2024-06-03 10:07:11.000000 orange3_bioinformatics-4.8.3/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0 runner    (1001) docker     (127)      622 2024-06-03 10:07:11.000000 orange3_bioinformatics-4.8.3/.github/ISSUE_TEMPLATE/feature_request.md
+-rwxr-xr-x   0 runner    (1001) docker     (127)      217 2024-06-03 10:07:11.000000 orange3_bioinformatics-4.8.3/.github/PULL_REQUEST_TEMPLATE.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 10:07:16.479340 orange3_bioinformatics-4.8.3/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      964 2024-06-03 10:07:11.000000 orange3_bioinformatics-4.8.3/.github/workflows/lint.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      175 2024-06-03 10:07:11.000000 orange3_bioinformatics-4.8.3/.github/workflows/rebase.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      213 2024-06-03 10:07:11.000000 orange3_bioinformatics-4.8.3/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      184 2024-06-03 10:07:11.000000 orange3_bioinformatics-4.8.3/.github/workflows/test.yml
+-rwxr-xr-x   0 runner    (1001) docker     (127)      755 2024-06-03 10:07:11.000000 orange3_bioinformatics-4.8.3/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      471 2024-06-03 10:07:11.000000 orange3_bioinformatics-4.8.3/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     9025 2024-06-03 10:07:11.000000 orange3_bioinformatics-4.8.3/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3348 2024-06-03 10:07:11.000000 orange3_bioinformatics-4.8.3/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (127)    35147 2024-06-03 10:07:11.000000 orange3_bioinformatics-4.8.3/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 10:07:16.539341 orange3_bioinformatics-4.8.3/Orange3_Bioinformatics.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3012 2024-06-03 10:07:16.000000 orange3_bioinformatics-4.8.3/Orange3_Bioinformatics.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    11598 2024-06-03 10:07:16.000000 orange3_bioinformatics-4.8.3/Orange3_Bioinformatics.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-03 10:07:16.000000 orange3_bioinformatics-4.8.3/Orange3_Bioinformatics.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      223 2024-06-03 10:07:16.000000 orange3_bioinformatics-4.8.3/Orange3_Bioinformatics.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-06-03 10:07:16.000000 orange3_bioinformatics-4.8.3/Orange3_Bioinformatics.egg-info/namespace_packages.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-03 10:07:16.000000 orange3_bioinformatics-4.8.3/Orange3_Bioinformatics.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      351 2024-06-03 10:07:16.000000 orange3_bioinformatics-4.8.3/Orange3_Bioinformatics.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-06-03 10:07:16.000000 orange3_bioinformatics-4.8.3/Orange3_Bioinformatics.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     3012 2024-06-03 10:07:16.539341 orange3_bioinformatics-4.8.3/PKG-INFO
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2707 2024-06-03 10:07:11.000000 orange3_bioinformatics-4.8.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      728 2024-06-03 10:07:11.000000 orange3_bioinformatics-4.8.3/README.pypi
+-rw-r--r--   0 runner    (1001) docker     (127)      206 2024-06-03 10:07:11.000000 orange3_bioinformatics-4.8.3/codecov.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 10:07:16.483340 orange3_bioinformatics-4.8.3/doc/
+-rw-r--r--   0 runner    (1001) docker     (127)     7464 2024-06-03 10:07:11.000000 orange3_bioinformatics-4.8.3/doc/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 10:07:16.483340 orange3_bioinformatics-4.8.3/doc/_static/
+-rw-r--r--   0 runner    (1001) docker     (127)     1302 2024-06-03 10:07:11.000000 orange3_bioinformatics-4.8.3/doc/_static/bioinformatics-sidebar-logo.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      537 2024-06-03 10:07:11.000000 orange3_bioinformatics-4.8.3/doc/_static/custom.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 10:07:16.483340 orange3_bioinformatics-4.8.3/doc/_templates/
+-rw-r--r--   0 runner    (1001) docker     (127)      314 2024-06-03 10:07:11.000000 orange3_bioinformatics-4.8.3/doc/_templates/about.html
+-rw-r--r--   0 runner    (1001) docker     (127)      333 2024-06-03 10:07:11.000000 orange3_bioinformatics-4.8.3/doc/_templates/globaltoc.html
+-rw-r--r--   0 runner    (1001) docker     (127)      495 2024-06-03 10:07:11.000000 orange3_bioinformatics-4.8.3/doc/_templates/useful_links.html
+-rw-r--r--   0 runner    (1001) docker     (127)    10192 2024-06-03 10:07:11.000000 orange3_bioinformatics-4.8.3/doc/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)      113 2024-06-03 10:07:11.000000 orange3_bioinformatics-4.8.3/doc/contents.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2319 2024-06-03 10:07:11.000000 orange3_bioinformatics-4.8.3/doc/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     7009 2024-06-03 10:07:11.000000 orange3_bioinformatics-4.8.3/doc/make.bat
+-rw-r--r--   0 runner    (1001) docker     (127)      439 2024-06-03 10:07:11.000000 orange3_bioinformatics-4.8.3/doc/scripting_reference.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 10:07:16.483340 orange3_bioinformatics-4.8.3/doc/scripting_references/
+-rw-r--r--   0 runner    (1001) docker     (127)      309 2024-06-03 10:07:11.000000 orange3_bioinformatics-4.8.3/doc/scripting_references/annotation.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 10:07:16.471340 orange3_bioinformatics-4.8.3/doc/scripting_references/code/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 10:07:16.487340 orange3_bioinformatics-4.8.3/doc/scripting_references/code/geo/
+-rw-r--r--   0 runner    (1001) docker     (127)      705 2024-06-03 10:07:11.000000 orange3_bioinformatics-4.8.3/doc/scripting_references/code/geo/dataset_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1352 2024-06-03 10:07:11.000000 orange3_bioinformatics-4.8.3/doc/scripting_references/code/geo/dataset_samples.py
+-rw-r--r--   0 runner    (1001) docker     (127)      553 2024-06-03 10:07:11.000000 orange3_bioinformatics-4.8.3/doc/scripting_references/code/geo/predict_disease_state.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 10:07:16.487340 orange3_bioinformatics-4.8.3/doc/scripting_references/code/go/
+-rw-r--r--   0 runner    (1001) docker     (127)      843 2024-06-03 10:07:11.000000 orange3_bioinformatics-4.8.3/doc/scripting_references/code/go/enrichment.py
+-rw-r--r--   0 runner    (1001) docker     (127)      823 2024-06-03 10:07:11.000000 orange3_bioinformatics-4.8.3/doc/scripting_references/code/go/gene_annotations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1113 2024-06-03 10:07:11.000000 orange3_bioinformatics-4.8.3/doc/scripting_references/dicty_phenotypes.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      965 2024-06-03 10:07:11.000000 orange3_bioinformatics-4.8.3/doc/scripting_references/geneset.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     4033 2024-06-03 10:07:11.000000 orange3_bioinformatics-4.8.3/doc/scripting_references/geo.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2086 2024-06-03 10:07:11.000000 orange3_bioinformatics-4.8.3/doc/scripting_references/go.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2816 2024-06-03 10:07:11.000000 orange3_bioinformatics-4.8.3/doc/scripting_references/kegg.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1179 2024-06-03 10:07:11.000000 orange3_bioinformatics-4.8.3/doc/scripting_references/marker_genes.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2660 2024-06-03 10:07:11.000000 orange3_bioinformatics-4.8.3/doc/scripting_references/ncbi_gene.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2180 2024-06-03 10:07:11.000000 orange3_bioinformatics-4.8.3/doc/scripting_references/ncbi_taxonomy.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      182 2024-06-03 10:07:11.000000 orange3_bioinformatics-4.8.3/doc/scripting_references/resolwe.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3949 2024-06-03 10:07:11.000000 orange3_bioinformatics-4.8.3/doc/scripting_references/serverfiles.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 10:07:16.487340 orange3_bioinformatics-4.8.3/doc/widgets/
+-rw-r--r--   0 runner    (1001) docker     (127)     4895 2024-06-03 10:07:11.000000 orange3_bioinformatics-4.8.3/doc/widgets/annotate_projection.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2752 2024-06-03 10:07:11.000000 orange3_bioinformatics-4.8.3/doc/widgets/cluster_analysis.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1399 2024-06-03 10:07:11.000000 orange3_bioinformatics-4.8.3/doc/widgets/databases_update.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1398 2024-06-03 10:07:11.000000 orange3_bioinformatics-4.8.3/doc/widgets/dicty_express.md
+-rw-r--r--   0 runner    (1001) docker     (127)     4105 2024-06-03 10:07:11.000000 orange3_bioinformatics-4.8.3/doc/widgets/differential_expression.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2238 2024-06-03 10:07:11.000000 orange3_bioinformatics-4.8.3/doc/widgets/gene_set_enrichment.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2957 2024-06-03 10:07:11.000000 orange3_bioinformatics-4.8.3/doc/widgets/gene_sets.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1716 2024-06-03 10:07:11.000000 orange3_bioinformatics-4.8.3/doc/widgets/genes.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2159 2024-06-03 10:07:11.000000 orange3_bioinformatics-4.8.3/doc/widgets/geo_data_sets.md
+-rw-r--r--   0 runner    (1001) docker     (127)     5027 2024-06-03 10:07:11.000000 orange3_bioinformatics-4.8.3/doc/widgets/go_browser.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1866 2024-06-03 10:07:11.000000 orange3_bioinformatics-4.8.3/doc/widgets/homologs.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 10:07:16.491340 orange3_bioinformatics-4.8.3/doc/widgets/icons/
+-rw-r--r--   0 runner    (1001) docker     (127)    35120 2024-06-03 10:07:11.000000 orange3_bioinformatics-4.8.3/doc/widgets/icons/annotator.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1638 2024-06-03 10:07:11.000000 orange3_bioinformatics-4.8.3/doc/widgets/icons/cluster-analysis.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1809 2024-06-03 10:07:11.000000 orange3_bioinformatics-4.8.3/doc/widgets/icons/databases-update.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1423 2024-06-03 10:07:11.000000 orange3_bioinformatics-4.8.3/doc/widgets/icons/dicty-express.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1639 2024-06-03 10:07:11.000000 orange3_bioinformatics-4.8.3/doc/widgets/icons/differential-expression.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1719 2024-06-03 10:07:11.000000 orange3_bioinformatics-4.8.3/doc/widgets/icons/gene-set-enrichment.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1640 2024-06-03 10:07:11.000000 orange3_bioinformatics-4.8.3/doc/widgets/icons/genes.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1728 2024-06-03 10:07:11.000000 orange3_bioinformatics-4.8.3/doc/widgets/icons/geo-data-sets.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1943 2024-06-03 10:07:11.000000 orange3_bioinformatics-4.8.3/doc/widgets/icons/go-browser.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1750 2024-06-03 10:07:11.000000 orange3_bioinformatics-4.8.3/doc/widgets/icons/kegg-pathways.png
+-rw-r--r--   0 runner    (1001) docker     (127)    13657 2024-06-03 10:07:11.000000 orange3_bioinformatics-4.8.3/doc/widgets/icons/volcano-plot.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 10:07:16.475340 orange3_bioinformatics-4.8.3/doc/widgets/images/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 10:07:16.491340 orange3_bioinformatics-4.8.3/doc/widgets/images/annotate_projection/
+-rw-r--r--   0 runner    (1001) docker     (127)   499949 2024-06-03 10:07:11.000000 orange3_bioinformatics-4.8.3/doc/widgets/images/annotate_projection/annotator-example.png
+-rw-r--r--   0 runner    (1001) docker     (127)   220708 2024-06-03 10:07:11.000000 orange3_bioinformatics-4.8.3/doc/widgets/images/annotate_projection/annotator-example2.png
+-rw-r--r--   0 runner    (1001) docker     (127)   291477 2024-06-03 10:07:11.000000 orange3_bioinformatics-4.8.3/doc/widgets/images/annotate_projection/annotator-stamped.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 10:07:16.491340 orange3_bioinformatics-4.8.3/doc/widgets/images/cluster_analysis/
+-rw-r--r--   0 runner    (1001) docker     (127)    93180 2024-06-03 10:07:11.000000 orange3_bioinformatics-4.8.3/doc/widgets/images/cluster_analysis/Cluster-Analysis-example.png
+-rw-r--r--   0 runner    (1001) docker     (127)    50174 2024-06-03 10:07:11.000000 orange3_bioinformatics-4.8.3/doc/widgets/images/cluster_analysis/Cluster-Analysis-stamped.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 10:07:16.491340 orange3_bioinformatics-4.8.3/doc/widgets/images/database_update/
+-rw-r--r--   0 runner    (1001) docker     (127)     8208 2024-06-03 10:07:11.000000 orange3_bioinformatics-4.8.3/doc/widgets/images/database_update/Add-Dataset.png
+-rw-r--r--   0 runner    (1001) docker     (127)    18674 2024-06-03 10:07:11.000000 orange3_bioinformatics-4.8.3/doc/widgets/images/database_update/Databases-Update-stamped.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 10:07:16.491340 orange3_bioinformatics-4.8.3/doc/widgets/images/dicty_express/
+-rw-r--r--   0 runner    (1001) docker     (127)   168071 2024-06-03 10:07:11.000000 orange3_bioinformatics-4.8.3/doc/widgets/images/dicty_express/dictyExpress-Example.png
+-rw-r--r--   0 runner    (1001) docker     (127)    36132 2024-06-03 10:07:11.000000 orange3_bioinformatics-4.8.3/doc/widgets/images/dicty_express/dictyExpress-stamped.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 10:07:16.491340 orange3_bioinformatics-4.8.3/doc/widgets/images/differential_expression/
+-rw-r--r--   0 runner    (1001) docker     (127)   176490 2024-06-03 10:07:11.000000 orange3_bioinformatics-4.8.3/doc/widgets/images/differential_expression/Differential-Expression-Example.png
+-rw-r--r--   0 runner    (1001) docker     (127)    30207 2024-06-03 10:07:11.000000 orange3_bioinformatics-4.8.3/doc/widgets/images/differential_expression/Differential-Expression-stamped.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 10:07:16.495340 orange3_bioinformatics-4.8.3/doc/widgets/images/gene-sets/
+-rw-r--r--   0 runner    (1001) docker     (127)    84453 2024-06-03 10:07:11.000000 orange3_bioinformatics-4.8.3/doc/widgets/images/gene-sets/Gene-Sets-example.png
+-rw-r--r--   0 runner    (1001) docker     (127)    92526 2024-06-03 10:07:11.000000 orange3_bioinformatics-4.8.3/doc/widgets/images/gene-sets/Gene-Sets-example2.png
+-rw-r--r--   0 runner    (1001) docker     (127)    28864 2024-06-03 10:07:11.000000 orange3_bioinformatics-4.8.3/doc/widgets/images/gene-sets/Gene-Sets-stamped.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 10:07:16.495340 orange3_bioinformatics-4.8.3/doc/widgets/images/gene_set_enrichment/
+-rw-r--r--   0 runner    (1001) docker     (127)    97576 2024-06-03 10:07:11.000000 orange3_bioinformatics-4.8.3/doc/widgets/images/gene_set_enrichment/Gene-Set-Enrichment-Example.png
+-rw-r--r--   0 runner    (1001) docker     (127)    55357 2024-06-03 10:07:11.000000 orange3_bioinformatics-4.8.3/doc/widgets/images/gene_set_enrichment/Gene-Set-Enrichment-stamped.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 10:07:16.495340 orange3_bioinformatics-4.8.3/doc/widgets/images/genes/
+-rw-r--r--   0 runner    (1001) docker     (127)   203400 2024-06-03 10:07:11.000000 orange3_bioinformatics-4.8.3/doc/widgets/images/genes/genes-Example.png
+-rw-r--r--   0 runner    (1001) docker     (127)    57611 2024-06-03 10:07:11.000000 orange3_bioinformatics-4.8.3/doc/widgets/images/genes/genes-stamped.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 10:07:16.495340 orange3_bioinformatics-4.8.3/doc/widgets/images/geo_data_sets/
+-rw-r--r--   0 runner    (1001) docker     (127)   195727 2024-06-03 10:07:11.000000 orange3_bioinformatics-4.8.3/doc/widgets/images/geo_data_sets/GEO-Data-Sets-Example.png
+-rw-r--r--   0 runner    (1001) docker     (127)    23593 2024-06-03 10:07:11.000000 orange3_bioinformatics-4.8.3/doc/widgets/images/geo_data_sets/GEO-Data-Sets-stamped.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 10:07:16.495340 orange3_bioinformatics-4.8.3/doc/widgets/images/go_browser/
+-rw-r--r--   0 runner    (1001) docker     (127)    24895 2024-06-03 10:07:11.000000 orange3_bioinformatics-4.8.3/doc/widgets/images/go_browser/Filter-Select.png
+-rw-r--r--   0 runner    (1001) docker     (127)   270407 2024-06-03 10:07:11.000000 orange3_bioinformatics-4.8.3/doc/widgets/images/go_browser/GO-Browser-Example.png
+-rw-r--r--   0 runner    (1001) docker     (127)    72500 2024-06-03 10:07:11.000000 orange3_bioinformatics-4.8.3/doc/widgets/images/go_browser/GO-Browser-stamped.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 10:07:16.495340 orange3_bioinformatics-4.8.3/doc/widgets/images/homologs/
+-rw-r--r--   0 runner    (1001) docker     (127)    74532 2024-06-03 10:07:11.000000 orange3_bioinformatics-4.8.3/doc/widgets/images/homologs/Homologs-Example.png
+-rw-r--r--   0 runner    (1001) docker     (127)     6463 2024-06-03 10:07:11.000000 orange3_bioinformatics-4.8.3/doc/widgets/images/homologs/Homologs-stamped.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 10:07:16.499340 orange3_bioinformatics-4.8.3/doc/widgets/images/kegg_pathways/
+-rw-r--r--   0 runner    (1001) docker     (127)   175266 2024-06-03 10:07:11.000000 orange3_bioinformatics-4.8.3/doc/widgets/images/kegg_pathways/KEGG-Pathways-Example.png
+-rw-r--r--   0 runner    (1001) docker     (127)    51393 2024-06-03 10:07:11.000000 orange3_bioinformatics-4.8.3/doc/widgets/images/kegg_pathways/KEGG-Pathways-stamped.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 10:07:16.499340 orange3_bioinformatics-4.8.3/doc/widgets/images/marker_genes/
+-rw-r--r--   0 runner    (1001) docker     (127)   112894 2024-06-03 10:07:11.000000 orange3_bioinformatics-4.8.3/doc/widgets/images/marker_genes/Marker-Genes-example.png
+-rw-r--r--   0 runner    (1001) docker     (127)    17416 2024-06-03 10:07:11.000000 orange3_bioinformatics-4.8.3/doc/widgets/images/marker_genes/Marker-Genes-stamped.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 10:07:16.499340 orange3_bioinformatics-4.8.3/doc/widgets/images/single_sample_scoring/
+-rw-r--r--   0 runner    (1001) docker     (127)    81226 2024-06-03 10:07:11.000000 orange3_bioinformatics-4.8.3/doc/widgets/images/single_sample_scoring/Single-Sample-Scoring-Example.png
+-rw-r--r--   0 runner    (1001) docker     (127)     4440 2024-06-03 10:07:11.000000 orange3_bioinformatics-4.8.3/doc/widgets/images/single_sample_scoring/Single-Sample-Scoring-stamped.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 10:07:16.499340 orange3_bioinformatics-4.8.3/doc/widgets/images/volcano_plot/
+-rw-r--r--   0 runner    (1001) docker     (127)   106338 2024-06-03 10:07:11.000000 orange3_bioinformatics-4.8.3/doc/widgets/images/volcano_plot/Volcano-Plot-Example.png
+-rw-r--r--   0 runner    (1001) docker     (127)    41623 2024-06-03 10:07:11.000000 orange3_bioinformatics-4.8.3/doc/widgets/images/volcano_plot/Volcano-Plot-stamped.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1911 2024-06-03 10:07:11.000000 orange3_bioinformatics-4.8.3/doc/widgets/kegg_pathways.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2683 2024-06-03 10:07:11.000000 orange3_bioinformatics-4.8.3/doc/widgets/marker_genes.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1608 2024-06-03 10:07:11.000000 orange3_bioinformatics-4.8.3/doc/widgets/single_sample_scoring.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2523 2024-06-03 10:07:11.000000 orange3_bioinformatics-4.8.3/doc/widgets/volcano_plot.md
+-rw-r--r--   0 runner    (1001) docker     (127)     4011 2024-06-03 10:07:11.000000 orange3_bioinformatics-4.8.3/doc/widgets.json
+-rw-r--r--   0 runner    (1001) docker     (127)      361 2024-06-03 10:07:11.000000 orange3_bioinformatics-4.8.3/doc/widgets.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 10:07:16.499340 orange3_bioinformatics-4.8.3/orangecontrib/
+-rwxr-xr-x   0 runner    (1001) docker     (127)      164 2024-06-03 10:07:11.000000 orange3_bioinformatics-4.8.3/orangecontrib/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 10:07:16.499340 orange3_bioinformatics-4.8.3/orangecontrib/bioinformatics/
+-rwxr-xr-x   0 runner    (1001) docker     (127)      252 2024-06-03 10:07:11.000000 orange3_bioinformatics-4.8.3/orangecontrib/bioinformatics/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 10:07:16.499340 orange3_bioinformatics-4.8.3/orangecontrib/bioinformatics/annotation/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 10:07:11.000000 orange3_bioinformatics-4.8.3/orangecontrib/bioinformatics/annotation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23226 2024-06-03 10:07:11.000000 orange3_bioinformatics-4.8.3/orangecontrib/bioinformatics/annotation/annotate_projection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9477 2024-06-03 10:07:11.000000 orange3_bioinformatics-4.8.3/orangecontrib/bioinformatics/annotation/annotate_samples.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 10:07:16.499340 orange3_bioinformatics-4.8.3/orangecontrib/bioinformatics/cluster_analysis/
+-rw-r--r--   0 runner    (1001) docker     (127)    13553 2024-06-03 10:07:11.000000 orange3_bioinformatics-4.8.3/orangecontrib/bioinformatics/cluster_analysis/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 10:07:16.499340 orange3_bioinformatics-4.8.3/orangecontrib/bioinformatics/dicty/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 10:07:11.000000 orange3_bioinformatics-4.8.3/orangecontrib/bioinformatics/dicty/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4383 2024-06-03 10:07:11.000000 orange3_bioinformatics-4.8.3/orangecontrib/bioinformatics/dicty/phenotypes.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 10:07:16.499340 orange3_bioinformatics-4.8.3/orangecontrib/bioinformatics/geneset/
+-rw-r--r--   0 runner    (1001) docker     (127)     1897 2024-06-03 10:07:11.000000 orange3_bioinformatics-4.8.3/orangecontrib/bioinformatics/geneset/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8982 2024-06-03 10:07:11.000000 orange3_bioinformatics-4.8.3/orangecontrib/bioinformatics/geneset/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 10:07:16.499340 orange3_bioinformatics-4.8.3/orangecontrib/bioinformatics/geo/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     5030 2024-06-03 10:07:11.000000 orange3_bioinformatics-4.8.3/orangecontrib/bioinformatics/geo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1664 2024-06-03 10:07:11.000000 orange3_bioinformatics-4.8.3/orangecontrib/bioinformatics/geo/dataset.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 10:07:16.503340 orange3_bioinformatics-4.8.3/orangecontrib/bioinformatics/go/
+-rw-r--r--   0 runner    (1001) docker     (127)    27098 2024-06-03 10:07:11.000000 orange3_bioinformatics-4.8.3/orangecontrib/bioinformatics/go/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      360 2024-06-03 10:07:11.000000 orange3_bioinformatics-4.8.3/orangecontrib/bioinformatics/go/config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 10:07:16.503340 orange3_bioinformatics-4.8.3/orangecontrib/bioinformatics/kegg/
+-rw-r--r--   0 runner    (1001) docker     (127)    12217 2024-06-03 10:07:11.000000 orange3_bioinformatics-4.8.3/orangecontrib/bioinformatics/kegg/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21289 2024-06-03 10:07:11.000000 orange3_bioinformatics-4.8.3/orangecontrib/bioinformatics/kegg/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2452 2024-06-03 10:07:11.000000 orange3_bioinformatics-4.8.3/orangecontrib/bioinformatics/kegg/brite.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8347 2024-06-03 10:07:11.000000 orange3_bioinformatics-4.8.3/orangecontrib/bioinformatics/kegg/caching.py
+-rw-r--r--   0 runner    (1001) docker     (127)      950 2024-06-03 10:07:11.000000 orange3_bioinformatics-4.8.3/orangecontrib/bioinformatics/kegg/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17989 2024-06-03 10:07:11.000000 orange3_bioinformatics-4.8.3/orangecontrib/bioinformatics/kegg/databases.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 10:07:16.503340 orange3_bioinformatics-4.8.3/orangecontrib/bioinformatics/kegg/entry/
+-rw-r--r--   0 runner    (1001) docker     (127)     5021 2024-06-03 10:07:11.000000 orange3_bioinformatics-4.8.3/orangecontrib/bioinformatics/kegg/entry/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5564 2024-06-03 10:07:11.000000 orange3_bioinformatics-4.8.3/orangecontrib/bioinformatics/kegg/entry/fields.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4913 2024-06-03 10:07:11.000000 orange3_bioinformatics-4.8.3/orangecontrib/bioinformatics/kegg/entry/parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8795 2024-06-03 10:07:11.000000 orange3_bioinformatics-4.8.3/orangecontrib/bioinformatics/kegg/pathway.py
+-rw-r--r--   0 runner    (1001) docker     (127)      792 2024-06-03 10:07:11.000000 orange3_bioinformatics-4.8.3/orangecontrib/bioinformatics/kegg/service.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2912 2024-06-03 10:07:11.000000 orange3_bioinformatics-4.8.3/orangecontrib/bioinformatics/kegg/types.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 10:07:16.503340 orange3_bioinformatics-4.8.3/orangecontrib/bioinformatics/ncbi/
+-rwxr-xr-x   0 runner    (1001) docker     (127)       61 2024-06-03 10:07:11.000000 orange3_bioinformatics-4.8.3/orangecontrib/bioinformatics/ncbi/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 10:07:16.503340 orange3_bioinformatics-4.8.3/orangecontrib/bioinformatics/ncbi/gene/
+-rwxr-xr-x   0 runner    (1001) docker     (127)    14166 2024-06-03 10:07:11.000000 orange3_bioinformatics-4.8.3/orangecontrib/bioinformatics/ncbi/gene/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1668 2024-06-03 10:07:11.000000 orange3_bioinformatics-4.8.3/orangecontrib/bioinformatics/ncbi/gene/config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 10:07:16.503340 orange3_bioinformatics-4.8.3/orangecontrib/bioinformatics/ncbi/homologene/
+-rw-r--r--   0 runner    (1001) docker     (127)     2093 2024-06-03 10:07:11.000000 orange3_bioinformatics-4.8.3/orangecontrib/bioinformatics/ncbi/homologene/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 10:07:16.503340 orange3_bioinformatics-4.8.3/orangecontrib/bioinformatics/ncbi/taxonomy/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4487 2024-06-03 10:07:11.000000 orange3_bioinformatics-4.8.3/orangecontrib/bioinformatics/ncbi/taxonomy/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    11321 2024-06-03 10:07:11.000000 orange3_bioinformatics-4.8.3/orangecontrib/bioinformatics/ncbi/taxonomy/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 10:07:16.503340 orange3_bioinformatics-4.8.3/orangecontrib/bioinformatics/preprocess/
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-06-03 10:07:11.000000 orange3_bioinformatics-4.8.3/orangecontrib/bioinformatics/preprocess/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2314 2024-06-03 10:07:11.000000 orange3_bioinformatics-4.8.3/orangecontrib/bioinformatics/preprocess/normalize.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 10:07:16.507340 orange3_bioinformatics-4.8.3/orangecontrib/bioinformatics/resolwe/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1061 2024-06-03 10:07:11.000000 orange3_bioinformatics-4.8.3/orangecontrib/bioinformatics/resolwe/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3335 2024-06-03 10:07:11.000000 orange3_bioinformatics-4.8.3/orangecontrib/bioinformatics/resolwe/genapi.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3051 2024-06-03 10:07:11.000000 orange3_bioinformatics-4.8.3/orangecontrib/bioinformatics/resolwe/resapi.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2560 2024-06-03 10:07:11.000000 orange3_bioinformatics-4.8.3/orangecontrib/bioinformatics/resolwe/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 10:07:16.507340 orange3_bioinformatics-4.8.3/orangecontrib/bioinformatics/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      467 2024-06-03 10:07:11.000000 orange3_bioinformatics-4.8.3/orangecontrib/bioinformatics/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 10:07:16.507340 orange3_bioinformatics-4.8.3/orangecontrib/bioinformatics/tests/annotation/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 10:07:11.000000 orange3_bioinformatics-4.8.3/orangecontrib/bioinformatics/tests/annotation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15903 2024-06-03 10:07:11.000000 orange3_bioinformatics-4.8.3/orangecontrib/bioinformatics/tests/annotation/test_annotate_projection.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14374 2024-06-03 10:07:11.000000 orange3_bioinformatics-4.8.3/orangecontrib/bioinformatics/tests/annotation/test_annotate_samples.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 10:07:16.507340 orange3_bioinformatics-4.8.3/orangecontrib/bioinformatics/tests/kegg/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 10:07:11.000000 orange3_bioinformatics-4.8.3/orangecontrib/bioinformatics/tests/kegg/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3065 2024-06-03 10:07:11.000000 orange3_bioinformatics-4.8.3/orangecontrib/bioinformatics/tests/kegg/test_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2849 2024-06-03 10:07:11.000000 orange3_bioinformatics-4.8.3/orangecontrib/bioinformatics/tests/kegg/test_databases.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1741 2024-06-03 10:07:11.000000 orange3_bioinformatics-4.8.3/orangecontrib/bioinformatics/tests/kegg/test_entry.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 10:07:16.507340 orange3_bioinformatics-4.8.3/orangecontrib/bioinformatics/tests/ncbi/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 10:07:11.000000 orange3_bioinformatics-4.8.3/orangecontrib/bioinformatics/tests/ncbi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3710 2024-06-03 10:07:11.000000 orange3_bioinformatics-4.8.3/orangecontrib/bioinformatics/tests/ncbi/test_gene.py
+-rw-r--r--   0 runner    (1001) docker     (127)      585 2024-06-03 10:07:11.000000 orange3_bioinformatics-4.8.3/orangecontrib/bioinformatics/tests/ncbi/test_homologene.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3488 2024-06-03 10:07:11.000000 orange3_bioinformatics-4.8.3/orangecontrib/bioinformatics/tests/ncbi/test_taxonomy.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 10:07:16.507340 orange3_bioinformatics-4.8.3/orangecontrib/bioinformatics/tests/preprocess/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 10:07:11.000000 orange3_bioinformatics-4.8.3/orangecontrib/bioinformatics/tests/preprocess/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1626 2024-06-03 10:07:11.000000 orange3_bioinformatics-4.8.3/orangecontrib/bioinformatics/tests/preprocess/test_normalize.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 10:07:16.507340 orange3_bioinformatics-4.8.3/orangecontrib/bioinformatics/tests/resolwe/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 10:07:11.000000 orange3_bioinformatics-4.8.3/orangecontrib/bioinformatics/tests/resolwe/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1995 2024-06-03 10:07:11.000000 orange3_bioinformatics-4.8.3/orangecontrib/bioinformatics/tests/resolwe/test_genapi.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3195 2024-06-03 10:07:11.000000 orange3_bioinformatics-4.8.3/orangecontrib/bioinformatics/tests/test_geneset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2549 2024-06-03 10:07:11.000000 orange3_bioinformatics-4.8.3/orangecontrib/bioinformatics/tests/test_geo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4060 2024-06-03 10:07:11.000000 orange3_bioinformatics-4.8.3/orangecontrib/bioinformatics/tests/test_statistics.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 10:07:16.511340 orange3_bioinformatics-4.8.3/orangecontrib/bioinformatics/tests/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 10:07:11.000000 orange3_bioinformatics-4.8.3/orangecontrib/bioinformatics/tests/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1825 2024-06-03 10:07:11.000000 orange3_bioinformatics-4.8.3/orangecontrib/bioinformatics/tests/utils/test_gui.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 10:07:16.511340 orange3_bioinformatics-4.8.3/orangecontrib/bioinformatics/tests/widgets/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 10:07:11.000000 orange3_bioinformatics-4.8.3/orangecontrib/bioinformatics/tests/widgets/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 10:07:16.511340 orange3_bioinformatics-4.8.3/orangecontrib/bioinformatics/tests/widgets/components/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 10:07:11.000000 orange3_bioinformatics-4.8.3/orangecontrib/bioinformatics/tests/widgets/components/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6181 2024-06-03 10:07:11.000000 orange3_bioinformatics-4.8.3/orangecontrib/bioinformatics/tests/widgets/components/test_gene_set_selection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8052 2024-06-03 10:07:11.000000 orange3_bioinformatics-4.8.3/orangecontrib/bioinformatics/tests/widgets/components/test_resolwe.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 10:07:16.511340 orange3_bioinformatics-4.8.3/orangecontrib/bioinformatics/tests/widgets/data/
+-rw-r--r--   0 runner    (1001) docker     (127)     3828 2024-06-03 10:07:11.000000 orange3_bioinformatics-4.8.3/orangecontrib/bioinformatics/tests/widgets/data/genes.tab
+-rw-r--r--   0 runner    (1001) docker     (127)    12006 2024-06-03 10:07:11.000000 orange3_bioinformatics-4.8.3/orangecontrib/bioinformatics/tests/widgets/data/markers-panglao.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)    16086 2024-06-03 10:07:11.000000 orange3_bioinformatics-4.8.3/orangecontrib/bioinformatics/tests/widgets/test_OWAnnotateProjection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1351 2024-06-03 10:07:11.000000 orange3_bioinformatics-4.8.3/orangecontrib/bioinformatics/tests/widgets/test_OWDifferentialExpression.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2519 2024-06-03 10:07:11.000000 orange3_bioinformatics-4.8.3/orangecontrib/bioinformatics/tests/widgets/test_OWGEODatasets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2986 2024-06-03 10:07:11.000000 orange3_bioinformatics-4.8.3/orangecontrib/bioinformatics/tests/widgets/test_OWGeneSets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3894 2024-06-03 10:07:11.000000 orange3_bioinformatics-4.8.3/orangecontrib/bioinformatics/tests/widgets/test_OWGenes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6113 2024-06-03 10:07:11.000000 orange3_bioinformatics-4.8.3/orangecontrib/bioinformatics/tests/widgets/test_OWGenialisExpressions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3024 2024-06-03 10:07:11.000000 orange3_bioinformatics-4.8.3/orangecontrib/bioinformatics/tests/widgets/test_OWHomologs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28959 2024-06-03 10:07:11.000000 orange3_bioinformatics-4.8.3/orangecontrib/bioinformatics/tests/widgets/test_OWMarkerGenes.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 10:07:16.511340 orange3_bioinformatics-4.8.3/orangecontrib/bioinformatics/utils/
+-rwxr-xr-x   0 runner    (1001) docker     (127)      542 2024-06-03 10:07:11.000000 orange3_bioinformatics-4.8.3/orangecontrib/bioinformatics/utils/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1604 2024-06-03 10:07:11.000000 orange3_bioinformatics-4.8.3/orangecontrib/bioinformatics/utils/serverfiles.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11389 2024-06-03 10:07:11.000000 orange3_bioinformatics-4.8.3/orangecontrib/bioinformatics/utils/statistics.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 10:07:16.515340 orange3_bioinformatics-4.8.3/orangecontrib/bioinformatics/widgets/
+-rw-r--r--   0 runner    (1001) docker     (127)    36783 2024-06-03 10:07:11.000000 orange3_bioinformatics-4.8.3/orangecontrib/bioinformatics/widgets/OWAnnotateProjection.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31640 2024-06-03 10:07:11.000000 orange3_bioinformatics-4.8.3/orangecontrib/bioinformatics/widgets/OWClusterAnalysis.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    32295 2024-06-03 10:07:11.000000 orange3_bioinformatics-4.8.3/orangecontrib/bioinformatics/widgets/OWDatabasesUpdate.py
+-rw-r--r--   0 runner    (1001) docker     (127)    46600 2024-06-03 10:07:11.000000 orange3_bioinformatics-4.8.3/orangecontrib/bioinformatics/widgets/OWDifferentialExpression.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    20747 2024-06-03 10:07:11.000000 orange3_bioinformatics-4.8.3/orangecontrib/bioinformatics/widgets/OWGEODatasets.py
+-rw-r--r--   0 runner    (1001) docker     (127)    41488 2024-06-03 10:07:11.000000 orange3_bioinformatics-4.8.3/orangecontrib/bioinformatics/widgets/OWGOBrowser.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20668 2024-06-03 10:07:11.000000 orange3_bioinformatics-4.8.3/orangecontrib/bioinformatics/widgets/OWGeneSetEnrichment.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13325 2024-06-03 10:07:11.000000 orange3_bioinformatics-4.8.3/orangecontrib/bioinformatics/widgets/OWGeneSets.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24379 2024-06-03 10:07:11.000000 orange3_bioinformatics-4.8.3/orangecontrib/bioinformatics/widgets/OWGenes.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25847 2024-06-03 10:07:11.000000 orange3_bioinformatics-4.8.3/orangecontrib/bioinformatics/widgets/OWGenialisExpressions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9305 2024-06-03 10:07:11.000000 orange3_bioinformatics-4.8.3/orangecontrib/bioinformatics/widgets/OWHomologs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31662 2024-06-03 10:07:11.000000 orange3_bioinformatics-4.8.3/orangecontrib/bioinformatics/widgets/OWKEGGPathwayBrowser.py
+-rw-r--r--   0 runner    (1001) docker     (127)    43956 2024-06-03 10:07:11.000000 orange3_bioinformatics-4.8.3/orangecontrib/bioinformatics/widgets/OWMarkerGenes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4900 2024-06-03 10:07:11.000000 orange3_bioinformatics-4.8.3/orangecontrib/bioinformatics/widgets/OWSingleSampleScoring.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5822 2024-06-03 10:07:11.000000 orange3_bioinformatics-4.8.3/orangecontrib/bioinformatics/widgets/OWVolcanoPlot.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    11169 2024-06-03 10:07:11.000000 orange3_bioinformatics-4.8.3/orangecontrib/bioinformatics/widgets/OWdictyExpress.py
+-rw-r--r--   0 runner    (1001) docker     (127)      698 2024-06-03 10:07:11.000000 orange3_bioinformatics-4.8.3/orangecontrib/bioinformatics/widgets/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 10:07:16.515340 orange3_bioinformatics-4.8.3/orangecontrib/bioinformatics/widgets/components/
+-rw-r--r--   0 runner    (1001) docker     (127)       82 2024-06-03 10:07:11.000000 orange3_bioinformatics-4.8.3/orangecontrib/bioinformatics/widgets/components/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10742 2024-06-03 10:07:11.000000 orange3_bioinformatics-4.8.3/orangecontrib/bioinformatics/widgets/components/gene_set_selection.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17254 2024-06-03 10:07:11.000000 orange3_bioinformatics-4.8.3/orangecontrib/bioinformatics/widgets/components/resolwe.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 10:07:16.535340 orange3_bioinformatics-4.8.3/orangecontrib/bioinformatics/widgets/icons/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1302 2024-06-03 10:07:11.000000 orange3_bioinformatics-4.8.3/orangecontrib/bioinformatics/widgets/icons/Category-Bioinformatics.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     4230 2024-06-03 10:07:11.000000 orange3_bioinformatics-4.8.3/orangecontrib/bioinformatics/widgets/icons/OWAnnotateProjection.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     1396 2024-06-03 10:07:11.000000 orange3_bioinformatics-4.8.3/orangecontrib/bioinformatics/widgets/icons/OWClusterAnalysis.svg
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2519 2024-06-03 10:07:11.000000 orange3_bioinformatics-4.8.3/orangecontrib/bioinformatics/widgets/icons/OWDatabasesUpdate.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      954 2024-06-03 10:07:11.000000 orange3_bioinformatics-4.8.3/orangecontrib/bioinformatics/widgets/icons/OWDifferentialExpression.svg
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1960 2024-06-03 10:07:11.000000 orange3_bioinformatics-4.8.3/orangecontrib/bioinformatics/widgets/icons/OWGEODatasets.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     1659 2024-06-03 10:07:11.000000 orange3_bioinformatics-4.8.3/orangecontrib/bioinformatics/widgets/icons/OWGOBrowser.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     1147 2024-06-03 10:07:11.000000 orange3_bioinformatics-4.8.3/orangecontrib/bioinformatics/widgets/icons/OWGeneInfo.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     1971 2024-06-03 10:07:11.000000 orange3_bioinformatics-4.8.3/orangecontrib/bioinformatics/widgets/icons/OWGeneSetEnrichment.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     1189 2024-06-03 10:07:11.000000 orange3_bioinformatics-4.8.3/orangecontrib/bioinformatics/widgets/icons/OWGeneSets.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     2486 2024-06-03 10:07:11.000000 orange3_bioinformatics-4.8.3/orangecontrib/bioinformatics/widgets/icons/OWGenialisExpressions.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      829 2024-06-03 10:07:11.000000 orange3_bioinformatics-4.8.3/orangecontrib/bioinformatics/widgets/icons/OWHomologs.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     1980 2024-06-03 10:07:11.000000 orange3_bioinformatics-4.8.3/orangecontrib/bioinformatics/widgets/icons/OWKEGGPathwayBrowser.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     1256 2024-06-03 10:07:11.000000 orange3_bioinformatics-4.8.3/orangecontrib/bioinformatics/widgets/icons/OWMarkerGenes.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     1023 2024-06-03 10:07:11.000000 orange3_bioinformatics-4.8.3/orangecontrib/bioinformatics/widgets/icons/OWSingleSampleScoring.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     2154 2024-06-03 10:07:11.000000 orange3_bioinformatics-4.8.3/orangecontrib/bioinformatics/widgets/icons/OWVolcanoPlot.svg
+-rwxr-xr-x   0 runner    (1001) docker     (127) 12157657 2024-06-03 10:07:11.000000 orange3_bioinformatics-4.8.3/orangecontrib/bioinformatics/widgets/icons/OWdictyExpress.png
+-rw-r--r--   0 runner    (1001) docker     (127)     2864 2024-06-03 10:07:11.000000 orange3_bioinformatics-4.8.3/orangecontrib/bioinformatics/widgets/icons/OWdictyExpress.svg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 10:07:16.535340 orange3_bioinformatics-4.8.3/orangecontrib/bioinformatics/widgets/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      575 2024-06-03 10:07:11.000000 orange3_bioinformatics-4.8.3/orangecontrib/bioinformatics/widgets/utils/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1217 2024-06-03 10:07:11.000000 orange3_bioinformatics-4.8.3/orangecontrib/bioinformatics/widgets/utils/concurrent.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4121 2024-06-03 10:07:11.000000 orange3_bioinformatics-4.8.3/orangecontrib/bioinformatics/widgets/utils/data.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 10:07:16.535340 orange3_bioinformatics-4.8.3/orangecontrib/bioinformatics/widgets/utils/gui/
+-rw-r--r--   0 runner    (1001) docker     (127)     4943 2024-06-03 10:07:11.000000 orange3_bioinformatics-4.8.3/orangecontrib/bioinformatics/widgets/utils/gui/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3474 2024-06-03 10:07:11.000000 orange3_bioinformatics-4.8.3/orangecontrib/bioinformatics/widgets/utils/gui/gene_scoring.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7267 2024-06-03 10:07:11.000000 orange3_bioinformatics-4.8.3/orangecontrib/bioinformatics/widgets/utils/gui/gene_sets.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13615 2024-06-03 10:07:11.000000 orange3_bioinformatics-4.8.3/orangecontrib/bioinformatics/widgets/utils/gui/label_selection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5722 2024-06-03 10:07:11.000000 orange3_bioinformatics-4.8.3/orangecontrib/bioinformatics/widgets/utils/gui/list_completer.py
+-rw-r--r--   0 runner    (1001) docker     (127)      567 2024-06-03 10:07:11.000000 orange3_bioinformatics-4.8.3/orangecontrib/bioinformatics/widgets/utils/itemdelegates.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2862 2024-06-03 10:07:11.000000 orange3_bioinformatics-4.8.3/orangecontrib/bioinformatics/widgets/utils/itemmodels.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2764 2024-06-03 10:07:11.000000 orange3_bioinformatics-4.8.3/orangecontrib/bioinformatics/widgets/utils/settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)      710 2024-06-03 10:07:11.000000 orange3_bioinformatics-4.8.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      235 2024-06-03 10:07:11.000000 orange3_bioinformatics-4.8.3/readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2253 2024-06-03 10:07:16.539341 orange3_bioinformatics-4.8.3/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1229 2024-06-03 10:07:11.000000 orange3_bioinformatics-4.8.3/setup.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1718 2024-06-03 10:07:11.000000 orange3_bioinformatics-4.8.3/tox.ini
```

### Comparing `Orange3-Bioinformatics-4.8.2/.github/FUNDING.yml` & `orange3_bioinformatics-4.8.3/.github/FUNDING.yml`

 * *Files identical despite different names*

### Comparing `Orange3-Bioinformatics-4.8.2/.github/ISSUE_TEMPLATE/bug_report.md` & `orange3_bioinformatics-4.8.3/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `Orange3-Bioinformatics-4.8.2/.github/ISSUE_TEMPLATE/feature_request.md` & `orange3_bioinformatics-4.8.3/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `Orange3-Bioinformatics-4.8.2/.github/workflows/lint.yml` & `orange3_bioinformatics-4.8.3/.github/workflows/lint.yml`

 * *Files identical despite different names*

### Comparing `Orange3-Bioinformatics-4.8.2/.gitignore` & `orange3_bioinformatics-4.8.3/.gitignore`

 * *Files identical despite different names*

### Comparing `Orange3-Bioinformatics-4.8.2/CHANGELOG.md` & `orange3_bioinformatics-4.8.3/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `Orange3-Bioinformatics-4.8.2/CODE_OF_CONDUCT.md` & `orange3_bioinformatics-4.8.3/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `Orange3-Bioinformatics-4.8.2/LICENSE` & `orange3_bioinformatics-4.8.3/LICENSE`

 * *Files identical despite different names*

### Comparing `Orange3-Bioinformatics-4.8.2/Orange3_Bioinformatics.egg-info/PKG-INFO` & `orange3_bioinformatics-4.8.3/Orange3_Bioinformatics.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Orange3-Bioinformatics
-Version: 4.8.2
+Version: 4.8.3
 Summary: Orange Bioinformatics add-on for Orange data mining software package.
 Home-page: https://github.com/biolab/orange3-bioinformatics
 Author: Bioinformatics Laboratory, FRI UL
 Author-email: info@biolab.si
 Maintainer: Jaka Kokosar
 License: GPL3+
 Project-URL: Bug Tracker, https://github.com/biolab/orange3-bioinformatics/issues
```

### Comparing `Orange3-Bioinformatics-4.8.2/Orange3_Bioinformatics.egg-info/SOURCES.txt` & `orange3_bioinformatics-4.8.3/Orange3_Bioinformatics.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `Orange3-Bioinformatics-4.8.2/PKG-INFO` & `orange3_bioinformatics-4.8.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Orange3-Bioinformatics
-Version: 4.8.2
+Version: 4.8.3
 Summary: Orange Bioinformatics add-on for Orange data mining software package.
 Home-page: https://github.com/biolab/orange3-bioinformatics
 Author: Bioinformatics Laboratory, FRI UL
 Author-email: info@biolab.si
 Maintainer: Jaka Kokosar
 License: GPL3+
 Project-URL: Bug Tracker, https://github.com/biolab/orange3-bioinformatics/issues
```

### Comparing `Orange3-Bioinformatics-4.8.2/README.md` & `orange3_bioinformatics-4.8.3/README.md`

 * *Files identical despite different names*

### Comparing `Orange3-Bioinformatics-4.8.2/README.pypi` & `orange3_bioinformatics-4.8.3/README.pypi`

 * *Files identical despite different names*

### Comparing `Orange3-Bioinformatics-4.8.2/doc/Makefile` & `orange3_bioinformatics-4.8.3/doc/Makefile`

 * *Files identical despite different names*

### Comparing `Orange3-Bioinformatics-4.8.2/doc/_static/bioinformatics-sidebar-logo.svg` & `orange3_bioinformatics-4.8.3/doc/_static/bioinformatics-sidebar-logo.svg`

 * *Files identical despite different names*

### Comparing `Orange3-Bioinformatics-4.8.2/doc/_static/custom.css` & `orange3_bioinformatics-4.8.3/doc/_static/custom.css`

 * *Files identical despite different names*

### Comparing `Orange3-Bioinformatics-4.8.2/doc/conf.py` & `orange3_bioinformatics-4.8.3/doc/conf.py`

 * *Files identical despite different names*

### Comparing `Orange3-Bioinformatics-4.8.2/doc/index.rst` & `orange3_bioinformatics-4.8.3/doc/index.rst`

 * *Files identical despite different names*

### Comparing `Orange3-Bioinformatics-4.8.2/doc/make.bat` & `orange3_bioinformatics-4.8.3/doc/make.bat`

 * *Files identical despite different names*

### Comparing `Orange3-Bioinformatics-4.8.2/doc/scripting_references/code/geo/dataset_info.py` & `orange3_bioinformatics-4.8.3/doc/scripting_references/code/geo/dataset_info.py`

 * *Files identical despite different names*

### Comparing `Orange3-Bioinformatics-4.8.2/doc/scripting_references/code/geo/dataset_samples.py` & `orange3_bioinformatics-4.8.3/doc/scripting_references/code/geo/dataset_samples.py`

 * *Files identical despite different names*

### Comparing `Orange3-Bioinformatics-4.8.2/doc/scripting_references/code/geo/predict_disease_state.py` & `orange3_bioinformatics-4.8.3/doc/scripting_references/code/geo/predict_disease_state.py`

 * *Files identical despite different names*

### Comparing `Orange3-Bioinformatics-4.8.2/doc/scripting_references/code/go/enrichment.py` & `orange3_bioinformatics-4.8.3/doc/scripting_references/code/go/enrichment.py`

 * *Files identical despite different names*

### Comparing `Orange3-Bioinformatics-4.8.2/doc/scripting_references/code/go/gene_annotations.py` & `orange3_bioinformatics-4.8.3/doc/scripting_references/code/go/gene_annotations.py`

 * *Files identical despite different names*

### Comparing `Orange3-Bioinformatics-4.8.2/doc/scripting_references/dicty_phenotypes.rst` & `orange3_bioinformatics-4.8.3/doc/scripting_references/dicty_phenotypes.rst`

 * *Files identical despite different names*

### Comparing `Orange3-Bioinformatics-4.8.2/doc/scripting_references/geneset.rst` & `orange3_bioinformatics-4.8.3/doc/scripting_references/geneset.rst`

 * *Files identical despite different names*

### Comparing `Orange3-Bioinformatics-4.8.2/doc/scripting_references/geo.rst` & `orange3_bioinformatics-4.8.3/doc/scripting_references/geo.rst`

 * *Files identical despite different names*

### Comparing `Orange3-Bioinformatics-4.8.2/doc/scripting_references/go.rst` & `orange3_bioinformatics-4.8.3/doc/scripting_references/go.rst`

 * *Files identical despite different names*

### Comparing `Orange3-Bioinformatics-4.8.2/doc/scripting_references/kegg.rst` & `orange3_bioinformatics-4.8.3/doc/scripting_references/kegg.rst`

 * *Files identical despite different names*

### Comparing `Orange3-Bioinformatics-4.8.2/doc/scripting_references/marker_genes.rst` & `orange3_bioinformatics-4.8.3/doc/scripting_references/marker_genes.rst`

 * *Files identical despite different names*

### Comparing `Orange3-Bioinformatics-4.8.2/doc/scripting_references/ncbi_gene.rst` & `orange3_bioinformatics-4.8.3/doc/scripting_references/ncbi_gene.rst`

 * *Files identical despite different names*

### Comparing `Orange3-Bioinformatics-4.8.2/doc/scripting_references/ncbi_taxonomy.rst` & `orange3_bioinformatics-4.8.3/doc/scripting_references/ncbi_taxonomy.rst`

 * *Files identical despite different names*

### Comparing `Orange3-Bioinformatics-4.8.2/doc/scripting_references/serverfiles.rst` & `orange3_bioinformatics-4.8.3/doc/scripting_references/serverfiles.rst`

 * *Files identical despite different names*

### Comparing `Orange3-Bioinformatics-4.8.2/doc/widgets/annotate_projection.md` & `orange3_bioinformatics-4.8.3/doc/widgets/annotate_projection.md`

 * *Files identical despite different names*

### Comparing `Orange3-Bioinformatics-4.8.2/doc/widgets/cluster_analysis.md` & `orange3_bioinformatics-4.8.3/doc/widgets/cluster_analysis.md`

 * *Files identical despite different names*

### Comparing `Orange3-Bioinformatics-4.8.2/doc/widgets/databases_update.md` & `orange3_bioinformatics-4.8.3/doc/widgets/databases_update.md`

 * *Files identical despite different names*

### Comparing `Orange3-Bioinformatics-4.8.2/doc/widgets/dicty_express.md` & `orange3_bioinformatics-4.8.3/doc/widgets/dicty_express.md`

 * *Files identical despite different names*

### Comparing `Orange3-Bioinformatics-4.8.2/doc/widgets/differential_expression.md` & `orange3_bioinformatics-4.8.3/doc/widgets/differential_expression.md`

 * *Files identical despite different names*

### Comparing `Orange3-Bioinformatics-4.8.2/doc/widgets/gene_set_enrichment.md` & `orange3_bioinformatics-4.8.3/doc/widgets/gene_set_enrichment.md`

 * *Files identical despite different names*

### Comparing `Orange3-Bioinformatics-4.8.2/doc/widgets/gene_sets.md` & `orange3_bioinformatics-4.8.3/doc/widgets/gene_sets.md`

 * *Files identical despite different names*

### Comparing `Orange3-Bioinformatics-4.8.2/doc/widgets/genes.md` & `orange3_bioinformatics-4.8.3/doc/widgets/genes.md`

 * *Files identical despite different names*

### Comparing `Orange3-Bioinformatics-4.8.2/doc/widgets/geo_data_sets.md` & `orange3_bioinformatics-4.8.3/doc/widgets/geo_data_sets.md`

 * *Files identical despite different names*

### Comparing `Orange3-Bioinformatics-4.8.2/doc/widgets/go_browser.md` & `orange3_bioinformatics-4.8.3/doc/widgets/go_browser.md`

 * *Files identical despite different names*

### Comparing `Orange3-Bioinformatics-4.8.2/doc/widgets/homologs.md` & `orange3_bioinformatics-4.8.3/doc/widgets/homologs.md`

 * *Files identical despite different names*

### Comparing `Orange3-Bioinformatics-4.8.2/doc/widgets/icons/annotator.png` & `orange3_bioinformatics-4.8.3/doc/widgets/icons/annotator.png`

 * *Files identical despite different names*

### Comparing `Orange3-Bioinformatics-4.8.2/doc/widgets/icons/cluster-analysis.png` & `orange3_bioinformatics-4.8.3/doc/widgets/icons/cluster-analysis.png`

 * *Files identical despite different names*

### Comparing `Orange3-Bioinformatics-4.8.2/doc/widgets/icons/databases-update.png` & `orange3_bioinformatics-4.8.3/doc/widgets/icons/databases-update.png`

 * *Files identical despite different names*

### Comparing `Orange3-Bioinformatics-4.8.2/doc/widgets/icons/dicty-express.png` & `orange3_bioinformatics-4.8.3/doc/widgets/icons/dicty-express.png`

 * *Files identical despite different names*

### Comparing `Orange3-Bioinformatics-4.8.2/doc/widgets/icons/differential-expression.png` & `orange3_bioinformatics-4.8.3/doc/widgets/icons/differential-expression.png`

 * *Files identical despite different names*

### Comparing `Orange3-Bioinformatics-4.8.2/doc/widgets/icons/gene-set-enrichment.png` & `orange3_bioinformatics-4.8.3/doc/widgets/icons/gene-set-enrichment.png`

 * *Files identical despite different names*

### Comparing `Orange3-Bioinformatics-4.8.2/doc/widgets/icons/genes.png` & `orange3_bioinformatics-4.8.3/doc/widgets/icons/genes.png`

 * *Files identical despite different names*

### Comparing `Orange3-Bioinformatics-4.8.2/doc/widgets/icons/geo-data-sets.png` & `orange3_bioinformatics-4.8.3/doc/widgets/icons/geo-data-sets.png`

 * *Files identical despite different names*

### Comparing `Orange3-Bioinformatics-4.8.2/doc/widgets/icons/go-browser.png` & `orange3_bioinformatics-4.8.3/doc/widgets/icons/go-browser.png`

 * *Files identical despite different names*

### Comparing `Orange3-Bioinformatics-4.8.2/doc/widgets/icons/kegg-pathways.png` & `orange3_bioinformatics-4.8.3/doc/widgets/icons/kegg-pathways.png`

 * *Files identical despite different names*

### Comparing `Orange3-Bioinformatics-4.8.2/doc/widgets/icons/volcano-plot.png` & `orange3_bioinformatics-4.8.3/doc/widgets/icons/volcano-plot.png`

 * *Files identical despite different names*

### Comparing `Orange3-Bioinformatics-4.8.2/doc/widgets/images/annotate_projection/annotator-example.png` & `orange3_bioinformatics-4.8.3/doc/widgets/images/annotate_projection/annotator-example.png`

 * *Files identical despite different names*

### Comparing `Orange3-Bioinformatics-4.8.2/doc/widgets/images/annotate_projection/annotator-example2.png` & `orange3_bioinformatics-4.8.3/doc/widgets/images/annotate_projection/annotator-example2.png`

 * *Files identical despite different names*

### Comparing `Orange3-Bioinformatics-4.8.2/doc/widgets/images/annotate_projection/annotator-stamped.png` & `orange3_bioinformatics-4.8.3/doc/widgets/images/annotate_projection/annotator-stamped.png`

 * *Files identical despite different names*

### Comparing `Orange3-Bioinformatics-4.8.2/doc/widgets/images/cluster_analysis/Cluster-Analysis-example.png` & `orange3_bioinformatics-4.8.3/doc/widgets/images/cluster_analysis/Cluster-Analysis-example.png`

 * *Files identical despite different names*

### Comparing `Orange3-Bioinformatics-4.8.2/doc/widgets/images/cluster_analysis/Cluster-Analysis-stamped.png` & `orange3_bioinformatics-4.8.3/doc/widgets/images/cluster_analysis/Cluster-Analysis-stamped.png`

 * *Files identical despite different names*

### Comparing `Orange3-Bioinformatics-4.8.2/doc/widgets/images/database_update/Add-Dataset.png` & `orange3_bioinformatics-4.8.3/doc/widgets/images/database_update/Add-Dataset.png`

 * *Files identical despite different names*

### Comparing `Orange3-Bioinformatics-4.8.2/doc/widgets/images/database_update/Databases-Update-stamped.png` & `orange3_bioinformatics-4.8.3/doc/widgets/images/database_update/Databases-Update-stamped.png`

 * *Files identical despite different names*

### Comparing `Orange3-Bioinformatics-4.8.2/doc/widgets/images/dicty_express/dictyExpress-Example.png` & `orange3_bioinformatics-4.8.3/doc/widgets/images/dicty_express/dictyExpress-Example.png`

 * *Files identical despite different names*

### Comparing `Orange3-Bioinformatics-4.8.2/doc/widgets/images/dicty_express/dictyExpress-stamped.png` & `orange3_bioinformatics-4.8.3/doc/widgets/images/dicty_express/dictyExpress-stamped.png`

 * *Files identical despite different names*

### Comparing `Orange3-Bioinformatics-4.8.2/doc/widgets/images/differential_expression/Differential-Expression-Example.png` & `orange3_bioinformatics-4.8.3/doc/widgets/images/differential_expression/Differential-Expression-Example.png`

 * *Files identical despite different names*

### Comparing `Orange3-Bioinformatics-4.8.2/doc/widgets/images/differential_expression/Differential-Expression-stamped.png` & `orange3_bioinformatics-4.8.3/doc/widgets/images/differential_expression/Differential-Expression-stamped.png`

 * *Files identical despite different names*

### Comparing `Orange3-Bioinformatics-4.8.2/doc/widgets/images/gene-sets/Gene-Sets-example.png` & `orange3_bioinformatics-4.8.3/doc/widgets/images/gene-sets/Gene-Sets-example.png`

 * *Files identical despite different names*

### Comparing `Orange3-Bioinformatics-4.8.2/doc/widgets/images/gene-sets/Gene-Sets-example2.png` & `orange3_bioinformatics-4.8.3/doc/widgets/images/gene-sets/Gene-Sets-example2.png`

 * *Files identical despite different names*

### Comparing `Orange3-Bioinformatics-4.8.2/doc/widgets/images/gene-sets/Gene-Sets-stamped.png` & `orange3_bioinformatics-4.8.3/doc/widgets/images/gene-sets/Gene-Sets-stamped.png`

 * *Files identical despite different names*

### Comparing `Orange3-Bioinformatics-4.8.2/doc/widgets/images/gene_set_enrichment/Gene-Set-Enrichment-Example.png` & `orange3_bioinformatics-4.8.3/doc/widgets/images/gene_set_enrichment/Gene-Set-Enrichment-Example.png`

 * *Files identical despite different names*

### Comparing `Orange3-Bioinformatics-4.8.2/doc/widgets/images/gene_set_enrichment/Gene-Set-Enrichment-stamped.png` & `orange3_bioinformatics-4.8.3/doc/widgets/images/gene_set_enrichment/Gene-Set-Enrichment-stamped.png`

 * *Files identical despite different names*

### Comparing `Orange3-Bioinformatics-4.8.2/doc/widgets/images/genes/genes-Example.png` & `orange3_bioinformatics-4.8.3/doc/widgets/images/genes/genes-Example.png`

 * *Files identical despite different names*

### Comparing `Orange3-Bioinformatics-4.8.2/doc/widgets/images/genes/genes-stamped.png` & `orange3_bioinformatics-4.8.3/doc/widgets/images/genes/genes-stamped.png`

 * *Files identical despite different names*

### Comparing `Orange3-Bioinformatics-4.8.2/doc/widgets/images/geo_data_sets/GEO-Data-Sets-Example.png` & `orange3_bioinformatics-4.8.3/doc/widgets/images/geo_data_sets/GEO-Data-Sets-Example.png`

 * *Files identical despite different names*

### Comparing `Orange3-Bioinformatics-4.8.2/doc/widgets/images/geo_data_sets/GEO-Data-Sets-stamped.png` & `orange3_bioinformatics-4.8.3/doc/widgets/images/geo_data_sets/GEO-Data-Sets-stamped.png`

 * *Files identical despite different names*

### Comparing `Orange3-Bioinformatics-4.8.2/doc/widgets/images/go_browser/Filter-Select.png` & `orange3_bioinformatics-4.8.3/doc/widgets/images/go_browser/Filter-Select.png`

 * *Files identical despite different names*

### Comparing `Orange3-Bioinformatics-4.8.2/doc/widgets/images/go_browser/GO-Browser-Example.png` & `orange3_bioinformatics-4.8.3/doc/widgets/images/go_browser/GO-Browser-Example.png`

 * *Files identical despite different names*

### Comparing `Orange3-Bioinformatics-4.8.2/doc/widgets/images/go_browser/GO-Browser-stamped.png` & `orange3_bioinformatics-4.8.3/doc/widgets/images/go_browser/GO-Browser-stamped.png`

 * *Files identical despite different names*

### Comparing `Orange3-Bioinformatics-4.8.2/doc/widgets/images/homologs/Homologs-Example.png` & `orange3_bioinformatics-4.8.3/doc/widgets/images/homologs/Homologs-Example.png`

 * *Files identical despite different names*

### Comparing `Orange3-Bioinformatics-4.8.2/doc/widgets/images/homologs/Homologs-stamped.png` & `orange3_bioinformatics-4.8.3/doc/widgets/images/homologs/Homologs-stamped.png`

 * *Files identical despite different names*

### Comparing `Orange3-Bioinformatics-4.8.2/doc/widgets/images/kegg_pathways/KEGG-Pathways-Example.png` & `orange3_bioinformatics-4.8.3/doc/widgets/images/kegg_pathways/KEGG-Pathways-Example.png`

 * *Files identical despite different names*

### Comparing `Orange3-Bioinformatics-4.8.2/doc/widgets/images/kegg_pathways/KEGG-Pathways-stamped.png` & `orange3_bioinformatics-4.8.3/doc/widgets/images/kegg_pathways/KEGG-Pathways-stamped.png`

 * *Files identical despite different names*

### Comparing `Orange3-Bioinformatics-4.8.2/doc/widgets/images/marker_genes/Marker-Genes-example.png` & `orange3_bioinformatics-4.8.3/doc/widgets/images/marker_genes/Marker-Genes-example.png`

 * *Files identical despite different names*

### Comparing `Orange3-Bioinformatics-4.8.2/doc/widgets/images/marker_genes/Marker-Genes-stamped.png` & `orange3_bioinformatics-4.8.3/doc/widgets/images/marker_genes/Marker-Genes-stamped.png`

 * *Files identical despite different names*

### Comparing `Orange3-Bioinformatics-4.8.2/doc/widgets/images/single_sample_scoring/Single-Sample-Scoring-Example.png` & `orange3_bioinformatics-4.8.3/doc/widgets/images/single_sample_scoring/Single-Sample-Scoring-Example.png`

 * *Files identical despite different names*

### Comparing `Orange3-Bioinformatics-4.8.2/doc/widgets/images/single_sample_scoring/Single-Sample-Scoring-stamped.png` & `orange3_bioinformatics-4.8.3/doc/widgets/images/single_sample_scoring/Single-Sample-Scoring-stamped.png`

 * *Files identical despite different names*

### Comparing `Orange3-Bioinformatics-4.8.2/doc/widgets/images/volcano_plot/Volcano-Plot-Example.png` & `orange3_bioinformatics-4.8.3/doc/widgets/images/volcano_plot/Volcano-Plot-Example.png`

 * *Files identical despite different names*

### Comparing `Orange3-Bioinformatics-4.8.2/doc/widgets/images/volcano_plot/Volcano-Plot-stamped.png` & `orange3_bioinformatics-4.8.3/doc/widgets/images/volcano_plot/Volcano-Plot-stamped.png`

 * *Files identical despite different names*

### Comparing `Orange3-Bioinformatics-4.8.2/doc/widgets/kegg_pathways.md` & `orange3_bioinformatics-4.8.3/doc/widgets/kegg_pathways.md`

 * *Files identical despite different names*

### Comparing `Orange3-Bioinformatics-4.8.2/doc/widgets/marker_genes.md` & `orange3_bioinformatics-4.8.3/doc/widgets/marker_genes.md`

 * *Files 12% similar despite different names*

```diff
@@ -15,14 +15,20 @@
  	<cite>Oscar Franzén, Li-Ming Gan, Johan L M Björkegren, PanglaoDB: a web server for exploration of mouse and human single-cell RNA sequencing data, Database, Volume 2019, 2019, baz046, https://doi.org/10.1093/database/baz046</cite>
  
  </br>
  
  - CellMarker
   
   	<cite>[CellMarker: a manually curated resource of cell markers in human and mouse.][1] Nucleic Acids Research. 2018.</cite>
+
+</br>
+
+ - DictyBase
+
+ 	<cite>Fey, P., Dodson, R., Basu, S., Chisholm, R. L., One Stop Shop for Everything Dictyostelium: dictyBase and the Dicty Stock Center. Dictyostelium discoideum Protocols. Methods Mol. Biol. 983:59-92, edited by Ludwig Eichinger and Francisco Rivero.</cite>
  
 
 Data is preprocessed in Orange readable format and it is hosted [here.][2] One can use [Databases update](databases_update.md)
 widget to download (or update) files locally.
 
 ![](images/marker_genes/Marker-Genes-stamped.png)
```

### Comparing `Orange3-Bioinformatics-4.8.2/doc/widgets/single_sample_scoring.md` & `orange3_bioinformatics-4.8.3/doc/widgets/single_sample_scoring.md`

 * *Files identical despite different names*

### Comparing `Orange3-Bioinformatics-4.8.2/doc/widgets/volcano_plot.md` & `orange3_bioinformatics-4.8.3/doc/widgets/volcano_plot.md`

 * *Files identical despite different names*

### Comparing `Orange3-Bioinformatics-4.8.2/doc/widgets.json` & `orange3_bioinformatics-4.8.3/doc/widgets.json`

 * *Files identical despite different names*

### Comparing `Orange3-Bioinformatics-4.8.2/orangecontrib/bioinformatics/annotation/annotate_projection.py` & `orange3_bioinformatics-4.8.3/orangecontrib/bioinformatics/annotation/annotate_projection.py`

 * *Files identical despite different names*

### Comparing `Orange3-Bioinformatics-4.8.2/orangecontrib/bioinformatics/annotation/annotate_samples.py` & `orange3_bioinformatics-4.8.3/orangecontrib/bioinformatics/annotation/annotate_samples.py`

 * *Files identical despite different names*

### Comparing `Orange3-Bioinformatics-4.8.2/orangecontrib/bioinformatics/cluster_analysis/__init__.py` & `orange3_bioinformatics-4.8.3/orangecontrib/bioinformatics/cluster_analysis/__init__.py`

 * *Files identical despite different names*

### Comparing `Orange3-Bioinformatics-4.8.2/orangecontrib/bioinformatics/dicty/phenotypes.py` & `orange3_bioinformatics-4.8.3/orangecontrib/bioinformatics/dicty/phenotypes.py`

 * *Files identical despite different names*

### Comparing `Orange3-Bioinformatics-4.8.2/orangecontrib/bioinformatics/geneset/__init__.py` & `orange3_bioinformatics-4.8.3/orangecontrib/bioinformatics/geneset/__init__.py`

 * *Files identical despite different names*

### Comparing `Orange3-Bioinformatics-4.8.2/orangecontrib/bioinformatics/geneset/utils.py` & `orange3_bioinformatics-4.8.3/orangecontrib/bioinformatics/geneset/utils.py`

 * *Files identical despite different names*

### Comparing `Orange3-Bioinformatics-4.8.2/orangecontrib/bioinformatics/geo/__init__.py` & `orange3_bioinformatics-4.8.3/orangecontrib/bioinformatics/geo/__init__.py`

 * *Files identical despite different names*

### Comparing `Orange3-Bioinformatics-4.8.2/orangecontrib/bioinformatics/geo/dataset.py` & `orange3_bioinformatics-4.8.3/orangecontrib/bioinformatics/geo/dataset.py`

 * *Files identical despite different names*

### Comparing `Orange3-Bioinformatics-4.8.2/orangecontrib/bioinformatics/go/__init__.py` & `orange3_bioinformatics-4.8.3/orangecontrib/bioinformatics/go/__init__.py`

 * *Files identical despite different names*

### Comparing `Orange3-Bioinformatics-4.8.2/orangecontrib/bioinformatics/kegg/__init__.py` & `orange3_bioinformatics-4.8.3/orangecontrib/bioinformatics/kegg/__init__.py`

 * *Files identical despite different names*

### Comparing `Orange3-Bioinformatics-4.8.2/orangecontrib/bioinformatics/kegg/api.py` & `orange3_bioinformatics-4.8.3/orangecontrib/bioinformatics/kegg/api.py`

 * *Files identical despite different names*

### Comparing `Orange3-Bioinformatics-4.8.2/orangecontrib/bioinformatics/kegg/brite.py` & `orange3_bioinformatics-4.8.3/orangecontrib/bioinformatics/kegg/brite.py`

 * *Files identical despite different names*

### Comparing `Orange3-Bioinformatics-4.8.2/orangecontrib/bioinformatics/kegg/caching.py` & `orange3_bioinformatics-4.8.3/orangecontrib/bioinformatics/kegg/caching.py`

 * *Files identical despite different names*

### Comparing `Orange3-Bioinformatics-4.8.2/orangecontrib/bioinformatics/kegg/conf.py` & `orange3_bioinformatics-4.8.3/orangecontrib/bioinformatics/kegg/conf.py`

 * *Files identical despite different names*

### Comparing `Orange3-Bioinformatics-4.8.2/orangecontrib/bioinformatics/kegg/databases.py` & `orange3_bioinformatics-4.8.3/orangecontrib/bioinformatics/kegg/databases.py`

 * *Files identical despite different names*

### Comparing `Orange3-Bioinformatics-4.8.2/orangecontrib/bioinformatics/kegg/entry/__init__.py` & `orange3_bioinformatics-4.8.3/orangecontrib/bioinformatics/kegg/entry/__init__.py`

 * *Files identical despite different names*

### Comparing `Orange3-Bioinformatics-4.8.2/orangecontrib/bioinformatics/kegg/entry/fields.py` & `orange3_bioinformatics-4.8.3/orangecontrib/bioinformatics/kegg/entry/fields.py`

 * *Files identical despite different names*

### Comparing `Orange3-Bioinformatics-4.8.2/orangecontrib/bioinformatics/kegg/entry/parser.py` & `orange3_bioinformatics-4.8.3/orangecontrib/bioinformatics/kegg/entry/parser.py`

 * *Files identical despite different names*

### Comparing `Orange3-Bioinformatics-4.8.2/orangecontrib/bioinformatics/kegg/pathway.py` & `orange3_bioinformatics-4.8.3/orangecontrib/bioinformatics/kegg/pathway.py`

 * *Files identical despite different names*

### Comparing `Orange3-Bioinformatics-4.8.2/orangecontrib/bioinformatics/kegg/service.py` & `orange3_bioinformatics-4.8.3/orangecontrib/bioinformatics/kegg/service.py`

 * *Files identical despite different names*

### Comparing `Orange3-Bioinformatics-4.8.2/orangecontrib/bioinformatics/kegg/types.py` & `orange3_bioinformatics-4.8.3/orangecontrib/bioinformatics/kegg/types.py`

 * *Files identical despite different names*

### Comparing `Orange3-Bioinformatics-4.8.2/orangecontrib/bioinformatics/ncbi/gene/__init__.py` & `orange3_bioinformatics-4.8.3/orangecontrib/bioinformatics/ncbi/gene/__init__.py`

 * *Files identical despite different names*

### Comparing `Orange3-Bioinformatics-4.8.2/orangecontrib/bioinformatics/ncbi/gene/config.py` & `orange3_bioinformatics-4.8.3/orangecontrib/bioinformatics/ncbi/gene/config.py`

 * *Files identical despite different names*

### Comparing `Orange3-Bioinformatics-4.8.2/orangecontrib/bioinformatics/ncbi/homologene/__init__.py` & `orange3_bioinformatics-4.8.3/orangecontrib/bioinformatics/ncbi/homologene/__init__.py`

 * *Files identical despite different names*

### Comparing `Orange3-Bioinformatics-4.8.2/orangecontrib/bioinformatics/ncbi/taxonomy/__init__.py` & `orange3_bioinformatics-4.8.3/orangecontrib/bioinformatics/ncbi/taxonomy/__init__.py`

 * *Files identical despite different names*

### Comparing `Orange3-Bioinformatics-4.8.2/orangecontrib/bioinformatics/ncbi/taxonomy/utils.py` & `orange3_bioinformatics-4.8.3/orangecontrib/bioinformatics/ncbi/taxonomy/utils.py`

 * *Files identical despite different names*

### Comparing `Orange3-Bioinformatics-4.8.2/orangecontrib/bioinformatics/preprocess/normalize.py` & `orange3_bioinformatics-4.8.3/orangecontrib/bioinformatics/preprocess/normalize.py`

 * *Files identical despite different names*

### Comparing `Orange3-Bioinformatics-4.8.2/orangecontrib/bioinformatics/resolwe/__init__.py` & `orange3_bioinformatics-4.8.3/orangecontrib/bioinformatics/resolwe/__init__.py`

 * *Files identical despite different names*

### Comparing `Orange3-Bioinformatics-4.8.2/orangecontrib/bioinformatics/resolwe/genapi.py` & `orange3_bioinformatics-4.8.3/orangecontrib/bioinformatics/resolwe/genapi.py`

 * *Files identical despite different names*

### Comparing `Orange3-Bioinformatics-4.8.2/orangecontrib/bioinformatics/resolwe/resapi.py` & `orange3_bioinformatics-4.8.3/orangecontrib/bioinformatics/resolwe/resapi.py`

 * *Files identical despite different names*

### Comparing `Orange3-Bioinformatics-4.8.2/orangecontrib/bioinformatics/resolwe/utils.py` & `orange3_bioinformatics-4.8.3/orangecontrib/bioinformatics/resolwe/utils.py`

 * *Files identical despite different names*

### Comparing `Orange3-Bioinformatics-4.8.2/orangecontrib/bioinformatics/tests/annotation/test_annotate_projection.py` & `orange3_bioinformatics-4.8.3/orangecontrib/bioinformatics/tests/annotation/test_annotate_projection.py`

 * *Files identical despite different names*

### Comparing `Orange3-Bioinformatics-4.8.2/orangecontrib/bioinformatics/tests/annotation/test_annotate_samples.py` & `orange3_bioinformatics-4.8.3/orangecontrib/bioinformatics/tests/annotation/test_annotate_samples.py`

 * *Files identical despite different names*

### Comparing `Orange3-Bioinformatics-4.8.2/orangecontrib/bioinformatics/tests/kegg/test_api.py` & `orange3_bioinformatics-4.8.3/orangecontrib/bioinformatics/tests/kegg/test_api.py`

 * *Files identical despite different names*

### Comparing `Orange3-Bioinformatics-4.8.2/orangecontrib/bioinformatics/tests/kegg/test_databases.py` & `orange3_bioinformatics-4.8.3/orangecontrib/bioinformatics/tests/kegg/test_databases.py`

 * *Files identical despite different names*

### Comparing `Orange3-Bioinformatics-4.8.2/orangecontrib/bioinformatics/tests/kegg/test_entry.py` & `orange3_bioinformatics-4.8.3/orangecontrib/bioinformatics/tests/kegg/test_entry.py`

 * *Files identical despite different names*

### Comparing `Orange3-Bioinformatics-4.8.2/orangecontrib/bioinformatics/tests/ncbi/test_gene.py` & `orange3_bioinformatics-4.8.3/orangecontrib/bioinformatics/tests/ncbi/test_gene.py`

 * *Files identical despite different names*

### Comparing `Orange3-Bioinformatics-4.8.2/orangecontrib/bioinformatics/tests/ncbi/test_homologene.py` & `orange3_bioinformatics-4.8.3/orangecontrib/bioinformatics/tests/ncbi/test_homologene.py`

 * *Files identical despite different names*

### Comparing `Orange3-Bioinformatics-4.8.2/orangecontrib/bioinformatics/tests/ncbi/test_taxonomy.py` & `orange3_bioinformatics-4.8.3/orangecontrib/bioinformatics/tests/ncbi/test_taxonomy.py`

 * *Files identical despite different names*

### Comparing `Orange3-Bioinformatics-4.8.2/orangecontrib/bioinformatics/tests/preprocess/test_normalize.py` & `orange3_bioinformatics-4.8.3/orangecontrib/bioinformatics/tests/preprocess/test_normalize.py`

 * *Files identical despite different names*

### Comparing `Orange3-Bioinformatics-4.8.2/orangecontrib/bioinformatics/tests/resolwe/test_genapi.py` & `orange3_bioinformatics-4.8.3/orangecontrib/bioinformatics/tests/resolwe/test_genapi.py`

 * *Files identical despite different names*

### Comparing `Orange3-Bioinformatics-4.8.2/orangecontrib/bioinformatics/tests/test_geneset.py` & `orange3_bioinformatics-4.8.3/orangecontrib/bioinformatics/tests/test_geneset.py`

 * *Files identical despite different names*

### Comparing `Orange3-Bioinformatics-4.8.2/orangecontrib/bioinformatics/tests/test_geo.py` & `orange3_bioinformatics-4.8.3/orangecontrib/bioinformatics/tests/test_geo.py`

 * *Files identical despite different names*

### Comparing `Orange3-Bioinformatics-4.8.2/orangecontrib/bioinformatics/tests/test_statistics.py` & `orange3_bioinformatics-4.8.3/orangecontrib/bioinformatics/tests/test_statistics.py`

 * *Files identical despite different names*

### Comparing `Orange3-Bioinformatics-4.8.2/orangecontrib/bioinformatics/tests/utils/test_gui.py` & `orange3_bioinformatics-4.8.3/orangecontrib/bioinformatics/tests/utils/test_gui.py`

 * *Files identical despite different names*

### Comparing `Orange3-Bioinformatics-4.8.2/orangecontrib/bioinformatics/tests/widgets/components/test_gene_set_selection.py` & `orange3_bioinformatics-4.8.3/orangecontrib/bioinformatics/tests/widgets/components/test_gene_set_selection.py`

 * *Files identical despite different names*

### Comparing `Orange3-Bioinformatics-4.8.2/orangecontrib/bioinformatics/tests/widgets/components/test_resolwe.py` & `orange3_bioinformatics-4.8.3/orangecontrib/bioinformatics/tests/widgets/components/test_resolwe.py`

 * *Files identical despite different names*

### Comparing `Orange3-Bioinformatics-4.8.2/orangecontrib/bioinformatics/tests/widgets/data/genes.tab` & `orange3_bioinformatics-4.8.3/orangecontrib/bioinformatics/tests/widgets/data/genes.tab`

 * *Files identical despite different names*

### Comparing `Orange3-Bioinformatics-4.8.2/orangecontrib/bioinformatics/tests/widgets/data/markers-panglao.pkl` & `orange3_bioinformatics-4.8.3/orangecontrib/bioinformatics/tests/widgets/data/markers-panglao.pkl`

 * *Files identical despite different names*

### Comparing `Orange3-Bioinformatics-4.8.2/orangecontrib/bioinformatics/tests/widgets/test_OWAnnotateProjection.py` & `orange3_bioinformatics-4.8.3/orangecontrib/bioinformatics/tests/widgets/test_OWAnnotateProjection.py`

 * *Files identical despite different names*

### Comparing `Orange3-Bioinformatics-4.8.2/orangecontrib/bioinformatics/tests/widgets/test_OWDifferentialExpression.py` & `orange3_bioinformatics-4.8.3/orangecontrib/bioinformatics/tests/widgets/test_OWDifferentialExpression.py`

 * *Files identical despite different names*

### Comparing `Orange3-Bioinformatics-4.8.2/orangecontrib/bioinformatics/tests/widgets/test_OWGEODatasets.py` & `orange3_bioinformatics-4.8.3/orangecontrib/bioinformatics/tests/widgets/test_OWGEODatasets.py`

 * *Files identical despite different names*

### Comparing `Orange3-Bioinformatics-4.8.2/orangecontrib/bioinformatics/tests/widgets/test_OWGeneSets.py` & `orange3_bioinformatics-4.8.3/orangecontrib/bioinformatics/tests/widgets/test_OWGeneSets.py`

 * *Files identical despite different names*

### Comparing `Orange3-Bioinformatics-4.8.2/orangecontrib/bioinformatics/tests/widgets/test_OWGenes.py` & `orange3_bioinformatics-4.8.3/orangecontrib/bioinformatics/tests/widgets/test_OWGenes.py`

 * *Files identical despite different names*

### Comparing `Orange3-Bioinformatics-4.8.2/orangecontrib/bioinformatics/tests/widgets/test_OWGenialisExpressions.py` & `orange3_bioinformatics-4.8.3/orangecontrib/bioinformatics/tests/widgets/test_OWGenialisExpressions.py`

 * *Files identical despite different names*

### Comparing `Orange3-Bioinformatics-4.8.2/orangecontrib/bioinformatics/tests/widgets/test_OWHomologs.py` & `orange3_bioinformatics-4.8.3/orangecontrib/bioinformatics/tests/widgets/test_OWHomologs.py`

 * *Files identical despite different names*

### Comparing `Orange3-Bioinformatics-4.8.2/orangecontrib/bioinformatics/tests/widgets/test_OWMarkerGenes.py` & `orange3_bioinformatics-4.8.3/orangecontrib/bioinformatics/tests/widgets/test_OWMarkerGenes.py`

 * *Files 1% similar despite different names*

```diff
@@ -302,28 +302,29 @@
 
     def test_available_sources(self):
         """
         Test if all sources retrieved. Currently there are two sources available.
         When more available unittest will be changed.
         """
         self.assertListEqual(
-            ["CellMarker", "Panglao"], list(self.widget.available_sources.keys())
+            ["CellMarker", "DictyBase", "Panglao"],
+            list(self.widget.available_sources.keys()),
         )
 
     def test_source_changed(self):
         """
         Test changing the source of the data.
         """
         # cell marker data
         self.assertEqual("Panglao", self.widget.db_source_cb.currentText())
         self.assertTrue(isinstance(self.widget.data, Table))
         self.assertEqual(len(self.panglao), len(self.widget.data))
 
         # Panglao data
-        simulate.combobox_activate_index(self.widget.controls.source_index, 1)
+        simulate.combobox_activate_index(self.widget.controls.source_index, 2)
         self.assertEqual("CellMarker", self.widget.db_source_cb.currentText())
         self.assertTrue(isinstance(self.widget.data, Table))
         self.assertEqual(len(self.cell_markers), len(self.widget.data))
 
         # cell marker data
         simulate.combobox_activate_index(self.widget.controls.source_index, 0)
         self.assertEqual("Panglao", self.widget.db_source_cb.currentText())
@@ -359,15 +360,15 @@
         self.assertEqual(
             sum(self.panglao.get_column("Organism") == "Mouse"), len(model)
         )
         self.assertEqual(
             len(np.unique(cell_types[~human_rows])), len(model.rootItem.childItems)
         )
 
-        simulate.combobox_activate_index(self.widget.controls.source_index, 1)
+        simulate.combobox_activate_index(self.widget.controls.source_index, 2)
         simulate.combobox_activate_index(self.widget.controls.organism_index, 0)
         self.assertEqual("CellMarker", self.widget.db_source_cb.currentText())
         self.assertEqual("Human", self.widget.group_cb.currentText())
 
         human_rows = self.widget.data.get_column("Organism") == "Human"
         cell_types = self.widget.data.get_column("Cell Type")
 
@@ -375,15 +376,15 @@
         self.assertEqual(
             sum(self.cell_markers.get_column("Organism") == "Human"), len(model)
         )
         self.assertEqual(
             len(np.unique(cell_types[human_rows])), len(model.rootItem.childItems)
         )
 
-        simulate.combobox_activate_index(self.widget.controls.source_index, 1)
+        simulate.combobox_activate_index(self.widget.controls.source_index, 2)
         simulate.combobox_activate_index(self.widget.controls.organism_index, 1)
         self.assertEqual("CellMarker", self.widget.db_source_cb.currentText())
         self.assertEqual("Mouse", self.widget.group_cb.currentText())
 
         model = self.widget.available_markers_view.model().sourceModel()
         self.assertEqual(
             sum(self.cell_markers.get_column("Organism") == "Mouse"), len(model)
```

### Comparing `Orange3-Bioinformatics-4.8.2/orangecontrib/bioinformatics/utils/__init__.py` & `orange3_bioinformatics-4.8.3/orangecontrib/bioinformatics/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `Orange3-Bioinformatics-4.8.2/orangecontrib/bioinformatics/utils/serverfiles.py` & `orange3_bioinformatics-4.8.3/orangecontrib/bioinformatics/utils/serverfiles.py`

 * *Files identical despite different names*

### Comparing `Orange3-Bioinformatics-4.8.2/orangecontrib/bioinformatics/utils/statistics.py` & `orange3_bioinformatics-4.8.3/orangecontrib/bioinformatics/utils/statistics.py`

 * *Files identical despite different names*

### Comparing `Orange3-Bioinformatics-4.8.2/orangecontrib/bioinformatics/widgets/OWAnnotateProjection.py` & `orange3_bioinformatics-4.8.3/orangecontrib/bioinformatics/widgets/OWAnnotateProjection.py`

 * *Files identical despite different names*

### Comparing `Orange3-Bioinformatics-4.8.2/orangecontrib/bioinformatics/widgets/OWClusterAnalysis.py` & `orange3_bioinformatics-4.8.3/orangecontrib/bioinformatics/widgets/OWClusterAnalysis.py`

 * *Files identical despite different names*

### Comparing `Orange3-Bioinformatics-4.8.2/orangecontrib/bioinformatics/widgets/OWDatabasesUpdate.py` & `orange3_bioinformatics-4.8.3/orangecontrib/bioinformatics/widgets/OWDatabasesUpdate.py`

 * *Files identical despite different names*

### Comparing `Orange3-Bioinformatics-4.8.2/orangecontrib/bioinformatics/widgets/OWDifferentialExpression.py` & `orange3_bioinformatics-4.8.3/orangecontrib/bioinformatics/widgets/OWDifferentialExpression.py`

 * *Files identical despite different names*

### Comparing `Orange3-Bioinformatics-4.8.2/orangecontrib/bioinformatics/widgets/OWGEODatasets.py` & `orange3_bioinformatics-4.8.3/orangecontrib/bioinformatics/widgets/OWGEODatasets.py`

 * *Files identical despite different names*

### Comparing `Orange3-Bioinformatics-4.8.2/orangecontrib/bioinformatics/widgets/OWGOBrowser.py` & `orange3_bioinformatics-4.8.3/orangecontrib/bioinformatics/widgets/OWGOBrowser.py`

 * *Files identical despite different names*

### Comparing `Orange3-Bioinformatics-4.8.2/orangecontrib/bioinformatics/widgets/OWGeneSetEnrichment.py` & `orange3_bioinformatics-4.8.3/orangecontrib/bioinformatics/widgets/OWGeneSetEnrichment.py`

 * *Files identical despite different names*

### Comparing `Orange3-Bioinformatics-4.8.2/orangecontrib/bioinformatics/widgets/OWGeneSets.py` & `orange3_bioinformatics-4.8.3/orangecontrib/bioinformatics/widgets/OWGeneSets.py`

 * *Files identical despite different names*

### Comparing `Orange3-Bioinformatics-4.8.2/orangecontrib/bioinformatics/widgets/OWGenes.py` & `orange3_bioinformatics-4.8.3/orangecontrib/bioinformatics/widgets/OWGenes.py`

 * *Files identical despite different names*

### Comparing `Orange3-Bioinformatics-4.8.2/orangecontrib/bioinformatics/widgets/OWGenialisExpressions.py` & `orange3_bioinformatics-4.8.3/orangecontrib/bioinformatics/widgets/OWGenialisExpressions.py`

 * *Files identical despite different names*

### Comparing `Orange3-Bioinformatics-4.8.2/orangecontrib/bioinformatics/widgets/OWHomologs.py` & `orange3_bioinformatics-4.8.3/orangecontrib/bioinformatics/widgets/OWHomologs.py`

 * *Files identical despite different names*

### Comparing `Orange3-Bioinformatics-4.8.2/orangecontrib/bioinformatics/widgets/OWKEGGPathwayBrowser.py` & `orange3_bioinformatics-4.8.3/orangecontrib/bioinformatics/widgets/OWKEGGPathwayBrowser.py`

 * *Files identical despite different names*

### Comparing `Orange3-Bioinformatics-4.8.2/orangecontrib/bioinformatics/widgets/OWMarkerGenes.py` & `orange3_bioinformatics-4.8.3/orangecontrib/bioinformatics/widgets/OWMarkerGenes.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """ OWMarkerGenes """
+
 from typing import List, Tuple, Iterable, Optional
 from functools import partial
 
 import numpy as np
 import requests
 
 from AnyQt import QtGui, QtCore
@@ -37,18 +38,22 @@
     GENE_AS_ATTRIBUTE_NAME,
 )
 from orangecontrib.bioinformatics.widgets.utils.settings import (
     MarkerGroupContextHandler,
 )
 
 SERVER_FILES_DOMAIN = 'marker_genes'
-GROUP_BY_ITEMS = ["Cell Type", "Function"]
+GROUP_BY_ITEMS = ["Cell Type", "Function", "Milestones", "Regulon cluster"]
 FILTER_COLUMNS_DEFAULT = ["Name", "Entrez ID"]
 NUM_LINES_TEXT = 5
-MAP_GROUP_TO_TAX_ID = {'Human': '9606', 'Mouse': '10090'}
+MAP_GROUP_TO_TAX_ID = {
+    'Human': '9606',
+    'Mouse': '10090',
+    "Dictyostelium discoideum": '44689',
+}
 
 
 class TreeItem(object):
     def __init__(
         self,
         name: str,
         is_type_item: bool,
@@ -651,18 +656,19 @@
         parent_column
             Column which is the group for items in the tree.
         """
         parents_dict = {}
         names = data_table.get_column("Name")
         types = data_table.get_column(parent_column)
         for n, pt, row in zip(names, types, data_table):
-            if pt not in parents_dict:
-                parents_dict[pt] = TreeItem(pt, True, None, parent)
+            if pt != "?":
+                if pt not in parents_dict:
+                    parents_dict[pt] = TreeItem(pt, True, None, parent)
 
-            TreeItem(n, False, row, parents_dict[pt])
+                TreeItem(n, False, row, parents_dict[pt])
 
     def set_expanded(self, index: QModelIndex, expanded: bool) -> None:
         """
         Sets the expanded flag of the item. This flag tell whether the item in the view
         is expanded.
 
         Parameters
@@ -850,16 +856,20 @@
     selected_root_attribute = Setting(0)
 
     settingsHandler = MarkerGroupContextHandler()  # noqa: N815
     selected_genes = settings.ContextSetting([])
 
     settings_version = 2
 
+    available_groups = GROUP_BY_ITEMS
+    _available_groups = None
+
     _data = None
     _available_sources = None
+    _selected_root_attribute = None
 
     def __init__(self) -> None:
         super().__init__()
 
         # define the layout
         main_area = QWidget(self.mainArea)
         self.mainArea.layout().addWidget(main_area)
@@ -933,15 +943,14 @@
         self.group_cb.activated[int].connect(self._set_group_index)
 
         box = gui.widgetBox(self.controlArea, 'Group by', margin=0)
         self.group_by_cb = gui.comboBox(
             box,
             self,
             'selected_root_attribute',
-            items=GROUP_BY_ITEMS,
             callback=self._setup,
         )
 
         gui.rubber(self.controlArea)
         gui.auto_commit(self.controlArea, self, "auto_commit", "Commit")
 
     def sizeHint(self):
@@ -1014,14 +1023,24 @@
                 self.organism_index = idx
                 self.selected_organism = group_values[idx]
             elif group_values:
                 self.organism_index = min(
                     max(self.organism_index, 0), len(group_values) - 1
                 )
 
+            self.available_groups = [
+                item
+                for item in GROUP_BY_ITEMS
+                if any(meta.name == item for meta in domain.metas)
+            ]
+
+            self.group_by_cb.clear()
+            self.group_by_cb.addItems(self.available_groups)
+            self.group_by_cb.setCurrentIndex(self.selected_root_attribute)
+
             self._set_group_index(self.organism_index)
 
     def _load_data(self) -> None:
         """
         Collect available data sources (marker genes data sets).
         """
         self.Warning.using_local_files.clear()
@@ -1064,16 +1083,23 @@
         Setup the views with data.
         """
         self.closeContext()
         self.selected_genes = []
         self.openContext((self.selected_organism, self.selected_source))
         data_not_selected, data_selected = self._filter_data_group(self.data)
 
+        if self._available_groups:
+            if (
+                self._available_groups[self._selected_root_attribute]
+                not in self.available_groups
+            ):
+                self.selected_root_attribute = 0
+
         # add model to available markers view
-        group_by = GROUP_BY_ITEMS[self.selected_root_attribute]
+        group_by = self.available_groups[self.selected_root_attribute]
         tree_model = TreeModel(data_not_selected, group_by)
         proxy_model = FilterProxyModel(self.filter_line_edit)
         proxy_model.setSourceModel(tree_model)
 
         self.available_markers_view.setModel(proxy_model)
         self.available_markers_view.selectionModel().selectionChanged.connect(
             partial(self._on_selection_changed, self.available_markers_view)
@@ -1092,14 +1118,16 @@
         )
         self.selected_markers_view.model().sourceModel().data_removed.connect(
             self._selected_markers_changed
         )
 
         # update output and messages
         self._selected_markers_changed()
+        self._selected_root_attribute = self.selected_root_attribute
+        self._available_groups = self.available_groups
 
     def _filter_data_group(self, data: Table) -> Tuple[Table, Tuple]:
         """
         Function filter the table based on the selected group (Mouse, Human) and divide
         them in two groups based on selected_data variable.
 
         Parameters
@@ -1122,15 +1150,15 @@
         else:
             mask = gvec == self.organism_index
         data = data[mask]
 
         # divide data based on selected_genes variable (context)
         unique_gene_names = np.core.defchararray.add(
             data.get_column("Entrez ID").astype(str),
-            data.get_column("Cell Type").astype(str),
+            data.get_column(self.available_groups[0]).astype(str),
         )
         mask = np.isin(unique_gene_names, self.selected_genes)
         data_not_selected = data[~mask]
         data_selected = data[mask]
         return data_not_selected, data_selected
 
     def commit(self) -> None:
@@ -1180,15 +1208,15 @@
 
     def _selected_markers_changed(self) -> None:
         """
         This function is called when markers in the selected view are added or removed.
         """
         rows = self.selected_markers_view.model().sourceModel().rootItem.get_data_rows()
         self.selected_genes = [
-            row["Entrez ID"].value + row["Cell Type"].value for row in rows
+            row["Entrez ID"].value + row[self.available_groups[0]].value for row in rows
         ]
         self.commit()
 
     def _on_selection_changed(self, view: TreeView) -> None:
         """
         When selection in one of the view changes in a view button should change a sign
         in the correct direction and other view should reset the selection.
```

### Comparing `Orange3-Bioinformatics-4.8.2/orangecontrib/bioinformatics/widgets/OWSingleSampleScoring.py` & `orange3_bioinformatics-4.8.3/orangecontrib/bioinformatics/widgets/OWSingleSampleScoring.py`

 * *Files identical despite different names*

### Comparing `Orange3-Bioinformatics-4.8.2/orangecontrib/bioinformatics/widgets/OWVolcanoPlot.py` & `orange3_bioinformatics-4.8.3/orangecontrib/bioinformatics/widgets/OWVolcanoPlot.py`

 * *Files identical despite different names*

### Comparing `Orange3-Bioinformatics-4.8.2/orangecontrib/bioinformatics/widgets/OWdictyExpress.py` & `orange3_bioinformatics-4.8.3/orangecontrib/bioinformatics/widgets/OWdictyExpress.py`

 * *Files identical despite different names*

### Comparing `Orange3-Bioinformatics-4.8.2/orangecontrib/bioinformatics/widgets/__init__.py` & `orange3_bioinformatics-4.8.3/orangecontrib/bioinformatics/widgets/__init__.py`

 * *Files identical despite different names*

### Comparing `Orange3-Bioinformatics-4.8.2/orangecontrib/bioinformatics/widgets/components/gene_set_selection.py` & `orange3_bioinformatics-4.8.3/orangecontrib/bioinformatics/widgets/components/gene_set_selection.py`

 * *Files identical despite different names*

### Comparing `Orange3-Bioinformatics-4.8.2/orangecontrib/bioinformatics/widgets/components/resolwe.py` & `orange3_bioinformatics-4.8.3/orangecontrib/bioinformatics/widgets/components/resolwe.py`

 * *Files identical despite different names*

### Comparing `Orange3-Bioinformatics-4.8.2/orangecontrib/bioinformatics/widgets/icons/Category-Bioinformatics.svg` & `orange3_bioinformatics-4.8.3/orangecontrib/bioinformatics/widgets/icons/Category-Bioinformatics.svg`

 * *Files identical despite different names*

### Comparing `Orange3-Bioinformatics-4.8.2/orangecontrib/bioinformatics/widgets/icons/OWAnnotateProjection.svg` & `orange3_bioinformatics-4.8.3/orangecontrib/bioinformatics/widgets/icons/OWAnnotateProjection.svg`

 * *Files identical despite different names*

### Comparing `Orange3-Bioinformatics-4.8.2/orangecontrib/bioinformatics/widgets/icons/OWClusterAnalysis.svg` & `orange3_bioinformatics-4.8.3/orangecontrib/bioinformatics/widgets/icons/OWClusterAnalysis.svg`

 * *Files identical despite different names*

### Comparing `Orange3-Bioinformatics-4.8.2/orangecontrib/bioinformatics/widgets/icons/OWDatabasesUpdate.svg` & `orange3_bioinformatics-4.8.3/orangecontrib/bioinformatics/widgets/icons/OWDatabasesUpdate.svg`

 * *Files identical despite different names*

### Comparing `Orange3-Bioinformatics-4.8.2/orangecontrib/bioinformatics/widgets/icons/OWDifferentialExpression.svg` & `orange3_bioinformatics-4.8.3/orangecontrib/bioinformatics/widgets/icons/OWDifferentialExpression.svg`

 * *Files identical despite different names*

### Comparing `Orange3-Bioinformatics-4.8.2/orangecontrib/bioinformatics/widgets/icons/OWGEODatasets.svg` & `orange3_bioinformatics-4.8.3/orangecontrib/bioinformatics/widgets/icons/OWGEODatasets.svg`

 * *Files identical despite different names*

### Comparing `Orange3-Bioinformatics-4.8.2/orangecontrib/bioinformatics/widgets/icons/OWGOBrowser.svg` & `orange3_bioinformatics-4.8.3/orangecontrib/bioinformatics/widgets/icons/OWGOBrowser.svg`

 * *Files identical despite different names*

### Comparing `Orange3-Bioinformatics-4.8.2/orangecontrib/bioinformatics/widgets/icons/OWGeneInfo.svg` & `orange3_bioinformatics-4.8.3/orangecontrib/bioinformatics/widgets/icons/OWGeneInfo.svg`

 * *Files identical despite different names*

### Comparing `Orange3-Bioinformatics-4.8.2/orangecontrib/bioinformatics/widgets/icons/OWGeneSetEnrichment.svg` & `orange3_bioinformatics-4.8.3/orangecontrib/bioinformatics/widgets/icons/OWGeneSetEnrichment.svg`

 * *Files identical despite different names*

### Comparing `Orange3-Bioinformatics-4.8.2/orangecontrib/bioinformatics/widgets/icons/OWGeneSets.svg` & `orange3_bioinformatics-4.8.3/orangecontrib/bioinformatics/widgets/icons/OWGeneSets.svg`

 * *Files identical despite different names*

### Comparing `Orange3-Bioinformatics-4.8.2/orangecontrib/bioinformatics/widgets/icons/OWGenialisExpressions.svg` & `orange3_bioinformatics-4.8.3/orangecontrib/bioinformatics/widgets/icons/OWGenialisExpressions.svg`

 * *Files identical despite different names*

### Comparing `Orange3-Bioinformatics-4.8.2/orangecontrib/bioinformatics/widgets/icons/OWHomologs.svg` & `orange3_bioinformatics-4.8.3/orangecontrib/bioinformatics/widgets/icons/OWHomologs.svg`

 * *Files identical despite different names*

### Comparing `Orange3-Bioinformatics-4.8.2/orangecontrib/bioinformatics/widgets/icons/OWKEGGPathwayBrowser.svg` & `orange3_bioinformatics-4.8.3/orangecontrib/bioinformatics/widgets/icons/OWKEGGPathwayBrowser.svg`

 * *Files identical despite different names*

### Comparing `Orange3-Bioinformatics-4.8.2/orangecontrib/bioinformatics/widgets/icons/OWMarkerGenes.svg` & `orange3_bioinformatics-4.8.3/orangecontrib/bioinformatics/widgets/icons/OWMarkerGenes.svg`

 * *Files identical despite different names*

### Comparing `Orange3-Bioinformatics-4.8.2/orangecontrib/bioinformatics/widgets/icons/OWSingleSampleScoring.svg` & `orange3_bioinformatics-4.8.3/orangecontrib/bioinformatics/widgets/icons/OWSingleSampleScoring.svg`

 * *Files identical despite different names*

### Comparing `Orange3-Bioinformatics-4.8.2/orangecontrib/bioinformatics/widgets/icons/OWVolcanoPlot.svg` & `orange3_bioinformatics-4.8.3/orangecontrib/bioinformatics/widgets/icons/OWVolcanoPlot.svg`

 * *Files identical despite different names*

### Comparing `Orange3-Bioinformatics-4.8.2/orangecontrib/bioinformatics/widgets/icons/OWdictyExpress.png` & `orange3_bioinformatics-4.8.3/orangecontrib/bioinformatics/widgets/icons/OWdictyExpress.png`

 * *Files identical despite different names*

### Comparing `Orange3-Bioinformatics-4.8.2/orangecontrib/bioinformatics/widgets/icons/OWdictyExpress.svg` & `orange3_bioinformatics-4.8.3/orangecontrib/bioinformatics/widgets/icons/OWdictyExpress.svg`

 * *Files identical despite different names*

### Comparing `Orange3-Bioinformatics-4.8.2/orangecontrib/bioinformatics/widgets/utils/__init__.py` & `orange3_bioinformatics-4.8.3/orangecontrib/bioinformatics/widgets/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `Orange3-Bioinformatics-4.8.2/orangecontrib/bioinformatics/widgets/utils/concurrent.py` & `orange3_bioinformatics-4.8.3/orangecontrib/bioinformatics/widgets/utils/concurrent.py`

 * *Files identical despite different names*

### Comparing `Orange3-Bioinformatics-4.8.2/orangecontrib/bioinformatics/widgets/utils/data.py` & `orange3_bioinformatics-4.8.3/orangecontrib/bioinformatics/widgets/utils/data.py`

 * *Files identical despite different names*

### Comparing `Orange3-Bioinformatics-4.8.2/orangecontrib/bioinformatics/widgets/utils/gui/__init__.py` & `orange3_bioinformatics-4.8.3/orangecontrib/bioinformatics/widgets/utils/gui/__init__.py`

 * *Files identical despite different names*

### Comparing `Orange3-Bioinformatics-4.8.2/orangecontrib/bioinformatics/widgets/utils/gui/gene_scoring.py` & `orange3_bioinformatics-4.8.3/orangecontrib/bioinformatics/widgets/utils/gui/gene_scoring.py`

 * *Files identical despite different names*

### Comparing `Orange3-Bioinformatics-4.8.2/orangecontrib/bioinformatics/widgets/utils/gui/gene_sets.py` & `orange3_bioinformatics-4.8.3/orangecontrib/bioinformatics/widgets/utils/gui/gene_sets.py`

 * *Files identical despite different names*

### Comparing `Orange3-Bioinformatics-4.8.2/orangecontrib/bioinformatics/widgets/utils/gui/label_selection.py` & `orange3_bioinformatics-4.8.3/orangecontrib/bioinformatics/widgets/utils/gui/label_selection.py`

 * *Files identical despite different names*

### Comparing `Orange3-Bioinformatics-4.8.2/orangecontrib/bioinformatics/widgets/utils/gui/list_completer.py` & `orange3_bioinformatics-4.8.3/orangecontrib/bioinformatics/widgets/utils/gui/list_completer.py`

 * *Files identical despite different names*

### Comparing `Orange3-Bioinformatics-4.8.2/orangecontrib/bioinformatics/widgets/utils/itemdelegates.py` & `orange3_bioinformatics-4.8.3/orangecontrib/bioinformatics/widgets/utils/itemdelegates.py`

 * *Files identical despite different names*

### Comparing `Orange3-Bioinformatics-4.8.2/orangecontrib/bioinformatics/widgets/utils/itemmodels.py` & `orange3_bioinformatics-4.8.3/orangecontrib/bioinformatics/widgets/utils/itemmodels.py`

 * *Files identical despite different names*

### Comparing `Orange3-Bioinformatics-4.8.2/orangecontrib/bioinformatics/widgets/utils/settings.py` & `orange3_bioinformatics-4.8.3/orangecontrib/bioinformatics/widgets/utils/settings.py`

 * *Files identical despite different names*

### Comparing `Orange3-Bioinformatics-4.8.2/pyproject.toml` & `orange3_bioinformatics-4.8.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `Orange3-Bioinformatics-4.8.2/setup.cfg` & `orange3_bioinformatics-4.8.3/setup.cfg`

 * *Files identical despite different names*

### Comparing `Orange3-Bioinformatics-4.8.2/setup.py` & `orange3_bioinformatics-4.8.3/setup.py`

 * *Files identical despite different names*

### Comparing `Orange3-Bioinformatics-4.8.2/tox.ini` & `orange3_bioinformatics-4.8.3/tox.ini`

 * *Files identical despite different names*

