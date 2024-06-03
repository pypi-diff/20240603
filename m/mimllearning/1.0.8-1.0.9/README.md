# Comparing `tmp/mimllearning-1.0.8.tar.gz` & `tmp/mimllearning-1.0.9.tar.gz`

## Comparing `mimllearning-1.0.8.tar` & `mimllearning-1.0.9.tar`

### file list

```diff
@@ -1,322 +1,322 @@
--rw-r--r--   0        0        0     1839 2020-02-02 00:00:00.000000 mimllearning-1.0.8/readme.md
--rw-r--r--   0        0        0     1307 2020-02-02 00:00:00.000000 mimllearning-1.0.8/.github/workflows/static.yml
--rw-r--r--   0        0        0      625 2020-02-02 00:00:00.000000 mimllearning-1.0.8/docs/Makefile
--rwxr-xr-x   0        0        0      800 2020-02-02 00:00:00.000000 mimllearning-1.0.8/docs/make.bat
--rw-r--r--   0        0        0   543085 2020-02-02 00:00:00.000000 mimllearning-1.0.8/docs/build/doctrees/environment.pickle
--rw-r--r--   0        0        0     2817 2020-02-02 00:00:00.000000 mimllearning-1.0.8/docs/build/doctrees/miml.doctree
--rw-r--r--   0        0        0     2856 2020-02-02 00:00:00.000000 mimllearning-1.0.8/docs/build/doctrees/classifier/index.doctree
--rw-r--r--   0        0        0     6082 2020-02-02 00:00:00.000000 mimllearning-1.0.8/docs/build/doctrees/classifier/mi.doctree
--rw-r--r--   0        0        0     7561 2020-02-02 00:00:00.000000 mimllearning-1.0.8/docs/build/doctrees/classifier/mimlTOmi.doctree
--rw-r--r--   0        0        0     4479 2020-02-02 00:00:00.000000 mimllearning-1.0.8/docs/build/doctrees/classifier/mimlTOml.doctree
--rw-r--r--   0        0        0     4564 2020-02-02 00:00:00.000000 mimllearning-1.0.8/docs/build/doctrees/classifier/miml_classifier.doctree
--rw-r--r--   0        0        0    14723 2020-02-02 00:00:00.000000 mimllearning-1.0.8/docs/build/doctrees/classifier/_autosummary/miml.classifier.mi.apr_classifier.APRClassifier.doctree
--rw-r--r--   0        0        0    15004 2020-02-02 00:00:00.000000 mimllearning-1.0.8/docs/build/doctrees/classifier/_autosummary/miml.classifier.mi.mi_wrapper_classifier.MIWrapperClassifier.doctree
--rw-r--r--   0        0        0    18929 2020-02-02 00:00:00.000000 mimllearning-1.0.8/docs/build/doctrees/classifier/_autosummary/miml.classifier.mimlTOmi.miml_to_mi_br_classifier.MIMLtoMIBRClassifier.doctree
--rw-r--r--   0        0        0    18554 2020-02-02 00:00:00.000000 mimllearning-1.0.8/docs/build/doctrees/classifier/_autosummary/miml.classifier.mimlTOmi.miml_to_mi_classifier.MIMLtoMIClassifier.doctree
--rw-r--r--   0        0        0    18925 2020-02-02 00:00:00.000000 mimllearning-1.0.8/docs/build/doctrees/classifier/_autosummary/miml.classifier.mimlTOmi.miml_to_mi_lp_classifier.MIMLtoMILPClassifier.doctree
--rw-r--r--   0        0        0    21010 2020-02-02 00:00:00.000000 mimllearning-1.0.8/docs/build/doctrees/classifier/_autosummary/miml.classifier.mimlTOml.miml_to_ml_classifier.MIMLtoMLClassifier.doctree
--rw-r--r--   0        0        0    15952 2020-02-02 00:00:00.000000 mimllearning-1.0.8/docs/build/doctrees/classifier/_autosummary/miml.classifier.miml_classifier.MIMLClassifier.doctree
--rw-r--r--   0        0        0     4387 2020-02-02 00:00:00.000000 mimllearning-1.0.8/docs/build/doctrees/data/bag.doctree
--rw-r--r--   0        0        0     4014 2020-02-02 00:00:00.000000 mimllearning-1.0.8/docs/build/doctrees/data/dataset_utils.doctree
--rw-r--r--   0        0        0     2799 2020-02-02 00:00:00.000000 mimllearning-1.0.8/docs/build/doctrees/data/index.doctree
--rw-r--r--   0        0        0     4557 2020-02-02 00:00:00.000000 mimllearning-1.0.8/docs/build/doctrees/data/instance.doctree
--rw-r--r--   0        0        0     4600 2020-02-02 00:00:00.000000 mimllearning-1.0.8/docs/build/doctrees/data/miml_dataset.doctree
--rw-r--r--   0        0        0    31754 2020-02-02 00:00:00.000000 mimllearning-1.0.8/docs/build/doctrees/data/_autosummary/miml.data.bag.Bag.doctree
--rw-r--r--   0        0        0    52596 2020-02-02 00:00:00.000000 mimllearning-1.0.8/docs/build/doctrees/data/_autosummary/miml.data.instance.Instance.doctree
--rw-r--r--   0        0        0    53297 2020-02-02 00:00:00.000000 mimllearning-1.0.8/docs/build/doctrees/data/_autosummary/miml.data.miml_dataset.MIMLDataset.doctree
--rw-r--r--   0        0        0     2742 2020-02-02 00:00:00.000000 mimllearning-1.0.8/docs/build/doctrees/report/index.doctree
--rw-r--r--   0        0        0     4345 2020-02-02 00:00:00.000000 mimllearning-1.0.8/docs/build/doctrees/report/report.doctree
--rw-r--r--   0        0        0    20548 2020-02-02 00:00:00.000000 mimllearning-1.0.8/docs/build/doctrees/report/_autosummary/miml.report.report.Report.doctree
--rw-r--r--   0        0        0     2833 2020-02-02 00:00:00.000000 mimllearning-1.0.8/docs/build/doctrees/transformation/index.doctree
--rw-r--r--   0        0        0     6481 2020-02-02 00:00:00.000000 mimllearning-1.0.8/docs/build/doctrees/transformation/mimlTOmi.doctree
--rw-r--r--   0        0        0     9116 2020-02-02 00:00:00.000000 mimllearning-1.0.8/docs/build/doctrees/transformation/mimlTOml.doctree
--rw-r--r--   0        0        0    12013 2020-02-02 00:00:00.000000 mimllearning-1.0.8/docs/build/doctrees/transformation/_autosummary/miml.transformation.mimlTOmi.binary_relevance_transformation.BinaryRelevanceTransformation.doctree
--rw-r--r--   0        0        0    14709 2020-02-02 00:00:00.000000 mimllearning-1.0.8/docs/build/doctrees/transformation/_autosummary/miml.transformation.mimlTOmi.label_powerset_transformation.LabelPowersetTransformation.doctree
--rw-r--r--   0        0        0    11160 2020-02-02 00:00:00.000000 mimllearning-1.0.8/docs/build/doctrees/transformation/_autosummary/miml.transformation.mimlTOml.arithmetic.ArithmeticTransformation.doctree
--rw-r--r--   0        0        0    11106 2020-02-02 00:00:00.000000 mimllearning-1.0.8/docs/build/doctrees/transformation/_autosummary/miml.transformation.mimlTOml.geometric.GeometricTransformation.doctree
--rw-r--r--   0        0        0    10938 2020-02-02 00:00:00.000000 mimllearning-1.0.8/docs/build/doctrees/transformation/_autosummary/miml.transformation.mimlTOml.miml_to_ml_transformation.MIMLtoMLTransformation.doctree
--rw-r--r--   0        0        0    10848 2020-02-02 00:00:00.000000 mimllearning-1.0.8/docs/build/doctrees/transformation/_autosummary/miml.transformation.mimlTOml.minmax.MinMaxTransformation.doctree
--rw-r--r--   0        0        0      230 2020-02-02 00:00:00.000000 mimllearning-1.0.8/docs/build/html/.buildinfo
--rw-r--r--   0        0        0    31431 2020-02-02 00:00:00.000000 mimllearning-1.0.8/docs/build/html/genindex.html
--rw-r--r--   0        0        0    20453 2020-02-02 00:00:00.000000 mimllearning-1.0.8/docs/build/html/index.html
--rw-r--r--   0        0        0     1149 2020-02-02 00:00:00.000000 mimllearning-1.0.8/docs/build/html/objects.inv
--rw-r--r--   0        0        0    18108 2020-02-02 00:00:00.000000 mimllearning-1.0.8/docs/build/html/search.html
--rw-r--r--   0        0        0    23504 2020-02-02 00:00:00.000000 mimllearning-1.0.8/docs/build/html/searchindex.js
--rw-r--r--   0        0        0      164 2020-02-02 00:00:00.000000 mimllearning-1.0.8/docs/build/html/_sources/miml.rst
--rw-r--r--   0        0        0      112 2020-02-02 00:00:00.000000 mimllearning-1.0.8/docs/build/html/_sources/classifier/index.rst
--rw-r--r--   0        0        0      170 2020-02-02 00:00:00.000000 mimllearning-1.0.8/docs/build/html/_sources/classifier/mi.rst
--rw-r--r--   0        0        0      301 2020-02-02 00:00:00.000000 mimllearning-1.0.8/docs/build/html/_sources/classifier/mimlTOmi.rst
--rw-r--r--   0        0        0      156 2020-02-02 00:00:00.000000 mimllearning-1.0.8/docs/build/html/_sources/classifier/mimlTOml.rst
--rw-r--r--   0        0        0      151 2020-02-02 00:00:00.000000 mimllearning-1.0.8/docs/build/html/_sources/classifier/miml_classifier.rst
--rw-r--r--   0        0        0      410 2020-02-02 00:00:00.000000 mimllearning-1.0.8/docs/build/html/_sources/classifier/_autosummary/miml.classifier.mi.apr_classifier.APRClassifier.rst
--rw-r--r--   0        0        0      475 2020-02-02 00:00:00.000000 mimllearning-1.0.8/docs/build/html/_sources/classifier/_autosummary/miml.classifier.mi.mi_wrapper_classifier.MIWrapperClassifier.rst
--rw-r--r--   0        0        0      631 2020-02-02 00:00:00.000000 mimllearning-1.0.8/docs/build/html/_sources/classifier/_autosummary/miml.classifier.mimlTOmi.miml_to_mi_br_classifier.MIMLtoMIBRClassifier.rst
--rw-r--r--   0        0        0      600 2020-02-02 00:00:00.000000 mimllearning-1.0.8/docs/build/html/_sources/classifier/_autosummary/miml.classifier.mimlTOmi.miml_to_mi_classifier.MIMLtoMIClassifier.rst
--rw-r--r--   0        0        0      631 2020-02-02 00:00:00.000000 mimllearning-1.0.8/docs/build/html/_sources/classifier/_autosummary/miml.classifier.mimlTOmi.miml_to_mi_lp_classifier.MIMLtoMILPClassifier.rst
--rw-r--r--   0        0        0      600 2020-02-02 00:00:00.000000 mimllearning-1.0.8/docs/build/html/_sources/classifier/_autosummary/miml.classifier.mimlTOml.miml_to_ml_classifier.MIMLtoMLClassifier.rst
--rw-r--r--   0        0        0      511 2020-02-02 00:00:00.000000 mimllearning-1.0.8/docs/build/html/_sources/classifier/_autosummary/miml.classifier.miml_classifier.MIMLClassifier.rst
--rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 mimllearning-1.0.8/docs/build/html/_sources/data/bag.rst
--rw-r--r--   0        0        0      149 2020-02-02 00:00:00.000000 mimllearning-1.0.8/docs/build/html/_sources/data/dataset_utils.rst
--rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 mimllearning-1.0.8/docs/build/html/_sources/data/index.rst
--rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 mimllearning-1.0.8/docs/build/html/_sources/data/instance.rst
--rw-r--r--   0        0        0      154 2020-02-02 00:00:00.000000 mimllearning-1.0.8/docs/build/html/_sources/data/miml_dataset.rst
--rw-r--r--   0        0        0      724 2020-02-02 00:00:00.000000 mimllearning-1.0.8/docs/build/html/_sources/data/_autosummary/miml.data.bag.Bag.rst
--rw-r--r--   0        0        0      199 2020-02-02 00:00:00.000000 mimllearning-1.0.8/docs/build/html/_sources/data/_autosummary/miml.data.instance.Instance.rst
--rw-r--r--   0        0        0     1507 2020-02-02 00:00:00.000000 mimllearning-1.0.8/docs/build/html/_sources/data/_autosummary/miml.data.miml_dataset.MIMLDataset.rst
--rw-r--r--   0        0        0       62 2020-02-02 00:00:00.000000 mimllearning-1.0.8/docs/build/html/_sources/report/index.rst
--rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 mimllearning-1.0.8/docs/build/html/_sources/report/report.rst
--rw-r--r--   0        0        0      392 2020-02-02 00:00:00.000000 mimllearning-1.0.8/docs/build/html/_sources/report/_autosummary/miml.report.report.Report.rst
--rw-r--r--   0        0        0       88 2020-02-02 00:00:00.000000 mimllearning-1.0.8/docs/build/html/_sources/transformation/index.rst
--rw-r--r--   0        0        0      280 2020-02-02 00:00:00.000000 mimllearning-1.0.8/docs/build/html/_sources/transformation/mimlTOmi.rst
--rw-r--r--   0        0        0      373 2020-02-02 00:00:00.000000 mimllearning-1.0.8/docs/build/html/_sources/transformation/mimlTOml.rst
--rw-r--r--   0        0        0      574 2020-02-02 00:00:00.000000 mimllearning-1.0.8/docs/build/html/_sources/transformation/_autosummary/miml.transformation.mimlTOmi.binary_relevance_transformation.BinaryRelevanceTransformation.rst
--rw-r--r--   0        0        0      656 2020-02-02 00:00:00.000000 mimllearning-1.0.8/docs/build/html/_sources/transformation/_autosummary/miml.transformation.mimlTOmi.label_powerset_transformation.LabelPowersetTransformation.rst
--rw-r--r--   0        0        0      477 2020-02-02 00:00:00.000000 mimllearning-1.0.8/docs/build/html/_sources/transformation/_autosummary/miml.transformation.mimlTOml.arithmetic.ArithmeticTransformation.rst
--rw-r--r--   0        0        0      468 2020-02-02 00:00:00.000000 mimllearning-1.0.8/docs/build/html/_sources/transformation/_autosummary/miml.transformation.mimlTOml.geometric.GeometricTransformation.rst
--rw-r--r--   0        0        0      516 2020-02-02 00:00:00.000000 mimllearning-1.0.8/docs/build/html/_sources/transformation/_autosummary/miml.transformation.mimlTOml.miml_to_ml_transformation.MIMLtoMLTransformation.rst
--rw-r--r--   0        0        0      441 2020-02-02 00:00:00.000000 mimllearning-1.0.8/docs/build/html/_sources/transformation/_autosummary/miml.transformation.mimlTOml.minmax.MinMaxTransformation.rst
--rw-r--r--   0        0        0    15094 2020-02-02 00:00:00.000000 mimllearning-1.0.8/docs/build/html/_static/basic.css
--rw-r--r--   0        0        0     4472 2020-02-02 00:00:00.000000 mimllearning-1.0.8/docs/build/html/_static/doctools.js
--rw-r--r--   0        0        0      319 2020-02-02 00:00:00.000000 mimllearning-1.0.8/docs/build/html/_static/documentation_options.js
--rw-r--r--   0        0        0      286 2020-02-02 00:00:00.000000 mimllearning-1.0.8/docs/build/html/_static/file.png
--rw-r--r--   0        0        0     4758 2020-02-02 00:00:00.000000 mimllearning-1.0.8/docs/build/html/_static/language_data.js
--rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 mimllearning-1.0.8/docs/build/html/_static/minus.png
--rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 mimllearning-1.0.8/docs/build/html/_static/plus.png
--rw-r--r--   0        0        0    12755 2020-02-02 00:00:00.000000 mimllearning-1.0.8/docs/build/html/_static/pygments.css
--rw-r--r--   0        0        0      419 2020-02-02 00:00:00.000000 mimllearning-1.0.8/docs/build/html/_static/sbt-webpack-macros.html
--rw-r--r--   0        0        0    20731 2020-02-02 00:00:00.000000 mimllearning-1.0.8/docs/build/html/_static/searchtools.js
--rw-r--r--   0        0        0     5123 2020-02-02 00:00:00.000000 mimllearning-1.0.8/docs/build/html/_static/sphinx_highlight.js
--rw-r--r--   0        0        0     1983 2020-02-02 00:00:00.000000 mimllearning-1.0.8/docs/build/html/_static/webpack-macros.html
--rw-r--r--   0        0        0     1186 2020-02-02 00:00:00.000000 mimllearning-1.0.8/docs/build/html/_static/images/logo_binder.svg
--rw-r--r--   0        0        0     7601 2020-02-02 00:00:00.000000 mimllearning-1.0.8/docs/build/html/_static/images/logo_colab.png
--rw-r--r--   0        0        0      681 2020-02-02 00:00:00.000000 mimllearning-1.0.8/docs/build/html/_static/images/logo_deepnote.svg
--rw-r--r--   0        0        0     1758 2020-02-02 00:00:00.000000 mimllearning-1.0.8/docs/build/html/_static/images/logo_jupyterhub.svg
--rw-r--r--   0        0        0     1541 2020-02-02 00:00:00.000000 mimllearning-1.0.8/docs/build/html/_static/locales/ar/LC_MESSAGES/booktheme.mo
--rw-r--r--   0        0        0     1459 2020-02-02 00:00:00.000000 mimllearning-1.0.8/docs/build/html/_static/locales/ar/LC_MESSAGES/booktheme.po
--rw-r--r--   0        0        0     1708 2020-02-02 00:00:00.000000 mimllearning-1.0.8/docs/build/html/_static/locales/bg/LC_MESSAGES/booktheme.mo
--rw-r--r--   0        0        0     1626 2020-02-02 00:00:00.000000 mimllearning-1.0.8/docs/build/html/_static/locales/bg/LC_MESSAGES/booktheme.po
--rw-r--r--   0        0        0     1646 2020-02-02 00:00:00.000000 mimllearning-1.0.8/docs/build/html/_static/locales/bn/LC_MESSAGES/booktheme.mo
--rw-r--r--   0        0        0     1564 2020-02-02 00:00:00.000000 mimllearning-1.0.8/docs/build/html/_static/locales/bn/LC_MESSAGES/booktheme.po
--rw-r--r--   0        0        0     1246 2020-02-02 00:00:00.000000 mimllearning-1.0.8/docs/build/html/_static/locales/ca/LC_MESSAGES/booktheme.mo
--rw-r--r--   0        0        0     1166 2020-02-02 00:00:00.000000 mimllearning-1.0.8/docs/build/html/_static/locales/ca/LC_MESSAGES/booktheme.po
--rw-r--r--   0        0        0     1405 2020-02-02 00:00:00.000000 mimllearning-1.0.8/docs/build/html/_static/locales/cs/LC_MESSAGES/booktheme.mo
--rw-r--r--   0        0        0     1323 2020-02-02 00:00:00.000000 mimllearning-1.0.8/docs/build/html/_static/locales/cs/LC_MESSAGES/booktheme.po
--rw-r--r--   0        0        0     1304 2020-02-02 00:00:00.000000 mimllearning-1.0.8/docs/build/html/_static/locales/da/LC_MESSAGES/booktheme.mo
--rw-r--r--   0        0        0     1222 2020-02-02 00:00:00.000000 mimllearning-1.0.8/docs/build/html/_static/locales/da/LC_MESSAGES/booktheme.po
--rw-r--r--   0        0        0     1388 2020-02-02 00:00:00.000000 mimllearning-1.0.8/docs/build/html/_static/locales/de/LC_MESSAGES/booktheme.mo
--rw-r--r--   0        0        0     1306 2020-02-02 00:00:00.000000 mimllearning-1.0.8/docs/build/html/_static/locales/de/LC_MESSAGES/booktheme.po
--rw-r--r--   0        0        0     1722 2020-02-02 00:00:00.000000 mimllearning-1.0.8/docs/build/html/_static/locales/el/LC_MESSAGES/booktheme.mo
--rw-r--r--   0        0        0     1640 2020-02-02 00:00:00.000000 mimllearning-1.0.8/docs/build/html/_static/locales/el/LC_MESSAGES/booktheme.po
--rw-r--r--   0        0        0     1337 2020-02-02 00:00:00.000000 mimllearning-1.0.8/docs/build/html/_static/locales/eo/LC_MESSAGES/booktheme.mo
--rw-r--r--   0        0        0     1255 2020-02-02 00:00:00.000000 mimllearning-1.0.8/docs/build/html/_static/locales/eo/LC_MESSAGES/booktheme.po
--rw-r--r--   0        0        0     1396 2020-02-02 00:00:00.000000 mimllearning-1.0.8/docs/build/html/_static/locales/es/LC_MESSAGES/booktheme.mo
--rw-r--r--   0        0        0     1314 2020-02-02 00:00:00.000000 mimllearning-1.0.8/docs/build/html/_static/locales/es/LC_MESSAGES/booktheme.po
--rw-r--r--   0        0        0     1341 2020-02-02 00:00:00.000000 mimllearning-1.0.8/docs/build/html/_static/locales/et/LC_MESSAGES/booktheme.mo
--rw-r--r--   0        0        0     1259 2020-02-02 00:00:00.000000 mimllearning-1.0.8/docs/build/html/_static/locales/et/LC_MESSAGES/booktheme.po
--rw-r--r--   0        0        0     1368 2020-02-02 00:00:00.000000 mimllearning-1.0.8/docs/build/html/_static/locales/fi/LC_MESSAGES/booktheme.mo
--rw-r--r--   0        0        0     1286 2020-02-02 00:00:00.000000 mimllearning-1.0.8/docs/build/html/_static/locales/fi/LC_MESSAGES/booktheme.po
--rw-r--r--   0        0        0     1412 2020-02-02 00:00:00.000000 mimllearning-1.0.8/docs/build/html/_static/locales/fr/LC_MESSAGES/booktheme.mo
--rw-r--r--   0        0        0     1330 2020-02-02 00:00:00.000000 mimllearning-1.0.8/docs/build/html/_static/locales/fr/LC_MESSAGES/booktheme.po
--rw-r--r--   0        0        0     1402 2020-02-02 00:00:00.000000 mimllearning-1.0.8/docs/build/html/_static/locales/hr/LC_MESSAGES/booktheme.mo
--rw-r--r--   0        0        0     1320 2020-02-02 00:00:00.000000 mimllearning-1.0.8/docs/build/html/_static/locales/hr/LC_MESSAGES/booktheme.po
--rw-r--r--   0        0        0     1323 2020-02-02 00:00:00.000000 mimllearning-1.0.8/docs/build/html/_static/locales/id/LC_MESSAGES/booktheme.mo
--rw-r--r--   0        0        0     1241 2020-02-02 00:00:00.000000 mimllearning-1.0.8/docs/build/html/_static/locales/id/LC_MESSAGES/booktheme.po
--rw-r--r--   0        0        0     1403 2020-02-02 00:00:00.000000 mimllearning-1.0.8/docs/build/html/_static/locales/it/LC_MESSAGES/booktheme.mo
--rw-r--r--   0        0        0     1321 2020-02-02 00:00:00.000000 mimllearning-1.0.8/docs/build/html/_static/locales/it/LC_MESSAGES/booktheme.po
--rw-r--r--   0        0        0     1445 2020-02-02 00:00:00.000000 mimllearning-1.0.8/docs/build/html/_static/locales/iw/LC_MESSAGES/booktheme.mo
--rw-r--r--   0        0        0     1363 2020-02-02 00:00:00.000000 mimllearning-1.0.8/docs/build/html/_static/locales/iw/LC_MESSAGES/booktheme.po
--rw-r--r--   0        0        0     1471 2020-02-02 00:00:00.000000 mimllearning-1.0.8/docs/build/html/_static/locales/ja/LC_MESSAGES/booktheme.mo
--rw-r--r--   0        0        0     1389 2020-02-02 00:00:00.000000 mimllearning-1.0.8/docs/build/html/_static/locales/ja/LC_MESSAGES/booktheme.po
--rw-r--r--   0        0        0     1375 2020-02-02 00:00:00.000000 mimllearning-1.0.8/docs/build/html/_static/locales/ko/LC_MESSAGES/booktheme.mo
--rw-r--r--   0        0        0     1293 2020-02-02 00:00:00.000000 mimllearning-1.0.8/docs/build/html/_static/locales/ko/LC_MESSAGES/booktheme.po
--rw-r--r--   0        0        0     1413 2020-02-02 00:00:00.000000 mimllearning-1.0.8/docs/build/html/_static/locales/lt/LC_MESSAGES/booktheme.mo
--rw-r--r--   0        0        0     1331 2020-02-02 00:00:00.000000 mimllearning-1.0.8/docs/build/html/_static/locales/lt/LC_MESSAGES/booktheme.po
--rw-r--r--   0        0        0     1404 2020-02-02 00:00:00.000000 mimllearning-1.0.8/docs/build/html/_static/locales/lv/LC_MESSAGES/booktheme.mo
--rw-r--r--   0        0        0     1322 2020-02-02 00:00:00.000000 mimllearning-1.0.8/docs/build/html/_static/locales/lv/LC_MESSAGES/booktheme.po
--rw-r--r--   0        0        0     1883 2020-02-02 00:00:00.000000 mimllearning-1.0.8/docs/build/html/_static/locales/ml/LC_MESSAGES/booktheme.mo
--rw-r--r--   0        0        0     1803 2020-02-02 00:00:00.000000 mimllearning-1.0.8/docs/build/html/_static/locales/ml/LC_MESSAGES/booktheme.po
--rw-r--r--   0        0        0     1674 2020-02-02 00:00:00.000000 mimllearning-1.0.8/docs/build/html/_static/locales/mr/LC_MESSAGES/booktheme.mo
--rw-r--r--   0        0        0     1594 2020-02-02 00:00:00.000000 mimllearning-1.0.8/docs/build/html/_static/locales/mr/LC_MESSAGES/booktheme.po
--rw-r--r--   0        0        0     1213 2020-02-02 00:00:00.000000 mimllearning-1.0.8/docs/build/html/_static/locales/ms/LC_MESSAGES/booktheme.mo
--rw-r--r--   0        0        0     1133 2020-02-02 00:00:00.000000 mimllearning-1.0.8/docs/build/html/_static/locales/ms/LC_MESSAGES/booktheme.po
--rw-r--r--   0        0        0     1356 2020-02-02 00:00:00.000000 mimllearning-1.0.8/docs/build/html/_static/locales/nl/LC_MESSAGES/booktheme.mo
--rw-r--r--   0        0        0     1274 2020-02-02 00:00:00.000000 mimllearning-1.0.8/docs/build/html/_static/locales/nl/LC_MESSAGES/booktheme.po
--rw-r--r--   0        0        0     1317 2020-02-02 00:00:00.000000 mimllearning-1.0.8/docs/build/html/_static/locales/no/LC_MESSAGES/booktheme.mo
--rw-r--r--   0        0        0     1235 2020-02-02 00:00:00.000000 mimllearning-1.0.8/docs/build/html/_static/locales/no/LC_MESSAGES/booktheme.po
--rw-r--r--   0        0        0     1371 2020-02-02 00:00:00.000000 mimllearning-1.0.8/docs/build/html/_static/locales/pl/LC_MESSAGES/booktheme.mo
--rw-r--r--   0        0        0     1289 2020-02-02 00:00:00.000000 mimllearning-1.0.8/docs/build/html/_static/locales/pl/LC_MESSAGES/booktheme.po
--rw-r--r--   0        0        0     1364 2020-02-02 00:00:00.000000 mimllearning-1.0.8/docs/build/html/_static/locales/pt/LC_MESSAGES/booktheme.mo
--rw-r--r--   0        0        0     1282 2020-02-02 00:00:00.000000 mimllearning-1.0.8/docs/build/html/_static/locales/pt/LC_MESSAGES/booktheme.po
--rw-r--r--   0        0        0     1390 2020-02-02 00:00:00.000000 mimllearning-1.0.8/docs/build/html/_static/locales/ro/LC_MESSAGES/booktheme.mo
--rw-r--r--   0        0        0     1308 2020-02-02 00:00:00.000000 mimllearning-1.0.8/docs/build/html/_static/locales/ro/LC_MESSAGES/booktheme.po
--rw-r--r--   0        0        0     1722 2020-02-02 00:00:00.000000 mimllearning-1.0.8/docs/build/html/_static/locales/ru/LC_MESSAGES/booktheme.mo
--rw-r--r--   0        0        0     1640 2020-02-02 00:00:00.000000 mimllearning-1.0.8/docs/build/html/_static/locales/ru/LC_MESSAGES/booktheme.po
--rw-r--r--   0        0        0     1393 2020-02-02 00:00:00.000000 mimllearning-1.0.8/docs/build/html/_static/locales/sk/LC_MESSAGES/booktheme.mo
--rw-r--r--   0        0        0     1311 2020-02-02 00:00:00.000000 mimllearning-1.0.8/docs/build/html/_static/locales/sk/LC_MESSAGES/booktheme.po
--rw-r--r--   0        0        0     1374 2020-02-02 00:00:00.000000 mimllearning-1.0.8/docs/build/html/_static/locales/sl/LC_MESSAGES/booktheme.mo
--rw-r--r--   0        0        0     1292 2020-02-02 00:00:00.000000 mimllearning-1.0.8/docs/build/html/_static/locales/sl/LC_MESSAGES/booktheme.po
--rw-r--r--   0        0        0     1679 2020-02-02 00:00:00.000000 mimllearning-1.0.8/docs/build/html/_static/locales/sr/LC_MESSAGES/booktheme.mo
--rw-r--r--   0        0        0     1597 2020-02-02 00:00:00.000000 mimllearning-1.0.8/docs/build/html/_static/locales/sr/LC_MESSAGES/booktheme.po
--rw-r--r--   0        0        0     1365 2020-02-02 00:00:00.000000 mimllearning-1.0.8/docs/build/html/_static/locales/sv/LC_MESSAGES/booktheme.mo
--rw-r--r--   0        0        0     1283 2020-02-02 00:00:00.000000 mimllearning-1.0.8/docs/build/html/_static/locales/sv/LC_MESSAGES/booktheme.po
--rw-r--r--   0        0        0     1928 2020-02-02 00:00:00.000000 mimllearning-1.0.8/docs/build/html/_static/locales/ta/LC_MESSAGES/booktheme.mo
--rw-r--r--   0        0        0     1848 2020-02-02 00:00:00.000000 mimllearning-1.0.8/docs/build/html/_static/locales/ta/LC_MESSAGES/booktheme.po
--rw-r--r--   0        0        0     1806 2020-02-02 00:00:00.000000 mimllearning-1.0.8/docs/build/html/_static/locales/te/LC_MESSAGES/booktheme.mo
--rw-r--r--   0        0        0     1726 2020-02-02 00:00:00.000000 mimllearning-1.0.8/docs/build/html/_static/locales/te/LC_MESSAGES/booktheme.po
--rw-r--r--   0        0        0     1628 2020-02-02 00:00:00.000000 mimllearning-1.0.8/docs/build/html/_static/locales/tg/LC_MESSAGES/booktheme.mo
--rw-r--r--   0        0        0     1546 2020-02-02 00:00:00.000000 mimllearning-1.0.8/docs/build/html/_static/locales/tg/LC_MESSAGES/booktheme.po
--rw-r--r--   0        0        0     1766 2020-02-02 00:00:00.000000 mimllearning-1.0.8/docs/build/html/_static/locales/th/LC_MESSAGES/booktheme.mo
--rw-r--r--   0        0        0     1684 2020-02-02 00:00:00.000000 mimllearning-1.0.8/docs/build/html/_static/locales/th/LC_MESSAGES/booktheme.po
--rw-r--r--   0        0        0     1273 2020-02-02 00:00:00.000000 mimllearning-1.0.8/docs/build/html/_static/locales/tl/LC_MESSAGES/booktheme.mo
--rw-r--r--   0        0        0     1193 2020-02-02 00:00:00.000000 mimllearning-1.0.8/docs/build/html/_static/locales/tl/LC_MESSAGES/booktheme.po
--rw-r--r--   0        0        0     1373 2020-02-02 00:00:00.000000 mimllearning-1.0.8/docs/build/html/_static/locales/tr/LC_MESSAGES/booktheme.mo
--rw-r--r--   0        0        0     1291 2020-02-02 00:00:00.000000 mimllearning-1.0.8/docs/build/html/_static/locales/tr/LC_MESSAGES/booktheme.po
--rw-r--r--   0        0        0     1681 2020-02-02 00:00:00.000000 mimllearning-1.0.8/docs/build/html/_static/locales/uk/LC_MESSAGES/booktheme.mo
--rw-r--r--   0        0        0     1601 2020-02-02 00:00:00.000000 mimllearning-1.0.8/docs/build/html/_static/locales/uk/LC_MESSAGES/booktheme.po
--rw-r--r--   0        0        0     1462 2020-02-02 00:00:00.000000 mimllearning-1.0.8/docs/build/html/_static/locales/ur/LC_MESSAGES/booktheme.mo
--rw-r--r--   0        0        0     1382 2020-02-02 00:00:00.000000 mimllearning-1.0.8/docs/build/html/_static/locales/ur/LC_MESSAGES/booktheme.po
--rw-r--r--   0        0        0     1431 2020-02-02 00:00:00.000000 mimllearning-1.0.8/docs/build/html/_static/locales/vi/LC_MESSAGES/booktheme.mo
--rw-r--r--   0        0        0     1349 2020-02-02 00:00:00.000000 mimllearning-1.0.8/docs/build/html/_static/locales/vi/LC_MESSAGES/booktheme.po
--rw-r--r--   0        0        0     1310 2020-02-02 00:00:00.000000 mimllearning-1.0.8/docs/build/html/_static/locales/zh_CN/LC_MESSAGES/booktheme.mo
--rw-r--r--   0        0        0     1228 2020-02-02 00:00:00.000000 mimllearning-1.0.8/docs/build/html/_static/locales/zh_CN/LC_MESSAGES/booktheme.po
--rw-r--r--   0        0        0     1341 2020-02-02 00:00:00.000000 mimllearning-1.0.8/docs/build/html/_static/locales/zh_TW/LC_MESSAGES/booktheme.mo
--rw-r--r--   0        0        0     1259 2020-02-02 00:00:00.000000 mimllearning-1.0.8/docs/build/html/_static/locales/zh_TW/LC_MESSAGES/booktheme.po
--rw-r--r--   0        0        0    81602 2020-02-02 00:00:00.000000 mimllearning-1.0.8/docs/build/html/_static/scripts/bootstrap.js
--rw-r--r--   0        0        0      237 2020-02-02 00:00:00.000000 mimllearning-1.0.8/docs/build/html/_static/scripts/bootstrap.js.LICENSE.txt
--rw-r--r--   0        0        0   332914 2020-02-02 00:00:00.000000 mimllearning-1.0.8/docs/build/html/_static/scripts/bootstrap.js.map
--rw-r--r--   0        0        0     9399 2020-02-02 00:00:00.000000 mimllearning-1.0.8/docs/build/html/_static/scripts/pydata-sphinx-theme.js
--rw-r--r--   0        0        0    44317 2020-02-02 00:00:00.000000 mimllearning-1.0.8/docs/build/html/_static/scripts/pydata-sphinx-theme.js.map
--rw-r--r--   0        0        0     3075 2020-02-02 00:00:00.000000 mimllearning-1.0.8/docs/build/html/_static/scripts/sphinx-book-theme.js
--rw-r--r--   0        0        0    13066 2020-02-02 00:00:00.000000 mimllearning-1.0.8/docs/build/html/_static/scripts/sphinx-book-theme.js.map
--rw-r--r--   0        0        0   208854 2020-02-02 00:00:00.000000 mimllearning-1.0.8/docs/build/html/_static/styles/bootstrap.css
--rw-r--r--   0        0        0   555088 2020-02-02 00:00:00.000000 mimllearning-1.0.8/docs/build/html/_static/styles/bootstrap.css.map
--rw-r--r--   0        0        0    72327 2020-02-02 00:00:00.000000 mimllearning-1.0.8/docs/build/html/_static/styles/pydata-sphinx-theme.css
--rw-r--r--   0        0        0   294060 2020-02-02 00:00:00.000000 mimllearning-1.0.8/docs/build/html/_static/styles/pydata-sphinx-theme.css.map
--rw-r--r--   0        0        0    14558 2020-02-02 00:00:00.000000 mimllearning-1.0.8/docs/build/html/_static/styles/sphinx-book-theme.css
--rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 mimllearning-1.0.8/docs/build/html/_static/styles/theme.css
--rw-r--r--   0        0        0     7427 2020-02-02 00:00:00.000000 mimllearning-1.0.8/docs/build/html/_static/vendor/fontawesome/6.5.1/LICENSE.txt
--rw-r--r--   0        0        0   102621 2020-02-02 00:00:00.000000 mimllearning-1.0.8/docs/build/html/_static/vendor/fontawesome/6.5.1/css/all.min.css
--rw-r--r--   0        0        0  1485766 2020-02-02 00:00:00.000000 mimllearning-1.0.8/docs/build/html/_static/vendor/fontawesome/6.5.1/js/all.min.js
--rw-r--r--   0        0        0      219 2020-02-02 00:00:00.000000 mimllearning-1.0.8/docs/build/html/_static/vendor/fontawesome/6.5.1/js/all.min.js.LICENSE.txt
--rw-r--r--   0        0        0   207972 2020-02-02 00:00:00.000000 mimllearning-1.0.8/docs/build/html/_static/vendor/fontawesome/6.5.1/webfonts/fa-brands-400.ttf
--rw-r--r--   0        0        0   117372 2020-02-02 00:00:00.000000 mimllearning-1.0.8/docs/build/html/_static/vendor/fontawesome/6.5.1/webfonts/fa-brands-400.woff2
--rw-r--r--   0        0        0    68004 2020-02-02 00:00:00.000000 mimllearning-1.0.8/docs/build/html/_static/vendor/fontawesome/6.5.1/webfonts/fa-regular-400.ttf
--rw-r--r--   0        0        0    25452 2020-02-02 00:00:00.000000 mimllearning-1.0.8/docs/build/html/_static/vendor/fontawesome/6.5.1/webfonts/fa-regular-400.woff2
--rw-r--r--   0        0        0   419720 2020-02-02 00:00:00.000000 mimllearning-1.0.8/docs/build/html/_static/vendor/fontawesome/6.5.1/webfonts/fa-solid-900.ttf
--rw-r--r--   0        0        0   156496 2020-02-02 00:00:00.000000 mimllearning-1.0.8/docs/build/html/_static/vendor/fontawesome/6.5.1/webfonts/fa-solid-900.woff2
--rw-r--r--   0        0        0    10832 2020-02-02 00:00:00.000000 mimllearning-1.0.8/docs/build/html/_static/vendor/fontawesome/6.5.1/webfonts/fa-v4compatibility.ttf
--rw-r--r--   0        0        0     4792 2020-02-02 00:00:00.000000 mimllearning-1.0.8/docs/build/html/_static/vendor/fontawesome/6.5.1/webfonts/fa-v4compatibility.woff2
--rw-r--r--   0        0        0    19595 2020-02-02 00:00:00.000000 mimllearning-1.0.8/docs/build/html/classifier/index.html
--rw-r--r--   0        0        0    20416 2020-02-02 00:00:00.000000 mimllearning-1.0.8/docs/build/html/classifier/mi.html
--rw-r--r--   0        0        0    21510 2020-02-02 00:00:00.000000 mimllearning-1.0.8/docs/build/html/classifier/mimlTOmi.html
--rw-r--r--   0        0        0    20217 2020-02-02 00:00:00.000000 mimllearning-1.0.8/docs/build/html/classifier/mimlTOml.html
--rw-r--r--   0        0        0    20198 2020-02-02 00:00:00.000000 mimllearning-1.0.8/docs/build/html/classifier/miml_classifier.html
--rw-r--r--   0        0        0    24737 2020-02-02 00:00:00.000000 mimllearning-1.0.8/docs/build/html/classifier/_autosummary/miml.classifier.mi.apr_classifier.APRClassifier.html
--rw-r--r--   0        0        0    24964 2020-02-02 00:00:00.000000 mimllearning-1.0.8/docs/build/html/classifier/_autosummary/miml.classifier.mi.mi_wrapper_classifier.MIWrapperClassifier.html
--rw-r--r--   0        0        0    25646 2020-02-02 00:00:00.000000 mimllearning-1.0.8/docs/build/html/classifier/_autosummary/miml.classifier.mimlTOmi.miml_to_mi_br_classifier.MIMLtoMIBRClassifier.html
--rw-r--r--   0        0        0    25287 2020-02-02 00:00:00.000000 mimllearning-1.0.8/docs/build/html/classifier/_autosummary/miml.classifier.mimlTOmi.miml_to_mi_classifier.MIMLtoMIClassifier.html
--rw-r--r--   0        0        0    25424 2020-02-02 00:00:00.000000 mimllearning-1.0.8/docs/build/html/classifier/_autosummary/miml.classifier.mimlTOmi.miml_to_mi_lp_classifier.MIMLtoMILPClassifier.html
--rw-r--r--   0        0        0    26240 2020-02-02 00:00:00.000000 mimllearning-1.0.8/docs/build/html/classifier/_autosummary/miml.classifier.mimlTOml.miml_to_ml_classifier.MIMLtoMLClassifier.html
--rw-r--r--   0        0        0    24250 2020-02-02 00:00:00.000000 mimllearning-1.0.8/docs/build/html/classifier/_autosummary/miml.classifier.miml_classifier.MIMLClassifier.html
--rw-r--r--   0        0        0    19868 2020-02-02 00:00:00.000000 mimllearning-1.0.8/docs/build/html/data/bag.html
--rw-r--r--   0        0        0    19704 2020-02-02 00:00:00.000000 mimllearning-1.0.8/docs/build/html/data/dataset_utils.html
--rw-r--r--   0        0        0    19980 2020-02-02 00:00:00.000000 mimllearning-1.0.8/docs/build/html/data/index.html
--rw-r--r--   0        0        0    19878 2020-02-02 00:00:00.000000 mimllearning-1.0.8/docs/build/html/data/instance.html
--rw-r--r--   0        0        0    20019 2020-02-02 00:00:00.000000 mimllearning-1.0.8/docs/build/html/data/miml_dataset.html
--rw-r--r--   0        0        0    27162 2020-02-02 00:00:00.000000 mimllearning-1.0.8/docs/build/html/data/_autosummary/miml.data.bag.Bag.html
--rw-r--r--   0        0        0    43163 2020-02-02 00:00:00.000000 mimllearning-1.0.8/docs/build/html/data/_autosummary/miml.data.instance.Instance.html
--rw-r--r--   0        0        0    30686 2020-02-02 00:00:00.000000 mimllearning-1.0.8/docs/build/html/data/_autosummary/miml.data.miml_dataset.MIMLDataset.html
--rw-r--r--   0        0        0    19479 2020-02-02 00:00:00.000000 mimllearning-1.0.8/docs/build/html/report/index.html
--rw-r--r--   0        0        0    19845 2020-02-02 00:00:00.000000 mimllearning-1.0.8/docs/build/html/report/report.html
--rw-r--r--   0        0        0    27555 2020-02-02 00:00:00.000000 mimllearning-1.0.8/docs/build/html/report/_autosummary/miml.report.report.Report.html
--rw-r--r--   0        0        0    19571 2020-02-02 00:00:00.000000 mimllearning-1.0.8/docs/build/html/transformation/index.html
--rw-r--r--   0        0        0    21018 2020-02-02 00:00:00.000000 mimllearning-1.0.8/docs/build/html/transformation/mimlTOmi.html
--rw-r--r--   0        0        0    22202 2020-02-02 00:00:00.000000 mimllearning-1.0.8/docs/build/html/transformation/mimlTOml.html
--rw-r--r--   0        0        0    24505 2020-02-02 00:00:00.000000 mimllearning-1.0.8/docs/build/html/transformation/_autosummary/miml.transformation.mimlTOmi.binary_relevance_transformation.BinaryRelevanceTransformation.html
--rw-r--r--   0        0        0    24774 2020-02-02 00:00:00.000000 mimllearning-1.0.8/docs/build/html/transformation/_autosummary/miml.transformation.mimlTOmi.label_powerset_transformation.LabelPowersetTransformation.html
--rw-r--r--   0        0        0    23957 2020-02-02 00:00:00.000000 mimllearning-1.0.8/docs/build/html/transformation/_autosummary/miml.transformation.mimlTOml.arithmetic.ArithmeticTransformation.html
--rw-r--r--   0        0        0    24101 2020-02-02 00:00:00.000000 mimllearning-1.0.8/docs/build/html/transformation/_autosummary/miml.transformation.mimlTOml.geometric.GeometricTransformation.html
--rw-r--r--   0        0        0    23685 2020-02-02 00:00:00.000000 mimllearning-1.0.8/docs/build/html/transformation/_autosummary/miml.transformation.mimlTOml.miml_to_ml_transformation.MIMLtoMLTransformation.html
--rw-r--r--   0        0        0    24044 2020-02-02 00:00:00.000000 mimllearning-1.0.8/docs/build/html/transformation/_autosummary/miml.transformation.mimlTOml.minmax.MinMaxTransformation.html
--rw-r--r--   0        0        0     1617 2020-02-02 00:00:00.000000 mimllearning-1.0.8/docs/source/conf.py
--rw-r--r--   0        0        0      165 2020-02-02 00:00:00.000000 mimllearning-1.0.8/docs/source/index.rst
--rw-r--r--   0        0        0      748 2020-02-02 00:00:00.000000 mimllearning-1.0.8/docs/source/_templates/base.rst
--rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 mimllearning-1.0.8/docs/source/_templates/base.rstZone.Identifier
--rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 mimllearning-1.0.8/docs/source/_templates/class.rst
--rw-r--r--   0        0        0      112 2020-02-02 00:00:00.000000 mimllearning-1.0.8/docs/source/classifier/index.rst
--rw-r--r--   0        0        0      170 2020-02-02 00:00:00.000000 mimllearning-1.0.8/docs/source/classifier/mi.rst
--rw-r--r--   0        0        0      301 2020-02-02 00:00:00.000000 mimllearning-1.0.8/docs/source/classifier/mimlTOmi.rst
--rw-r--r--   0        0        0      156 2020-02-02 00:00:00.000000 mimllearning-1.0.8/docs/source/classifier/mimlTOml.rst
--rw-r--r--   0        0        0      151 2020-02-02 00:00:00.000000 mimllearning-1.0.8/docs/source/classifier/miml_classifier.rst
--rw-r--r--   0        0        0      410 2020-02-02 00:00:00.000000 mimllearning-1.0.8/docs/source/classifier/_autosummary/miml.classifier.mi.apr_classifier.APRClassifier.rst
--rw-r--r--   0        0        0      475 2020-02-02 00:00:00.000000 mimllearning-1.0.8/docs/source/classifier/_autosummary/miml.classifier.mi.mi_wrapper_classifier.MIWrapperClassifier.rst
--rw-r--r--   0        0        0      631 2020-02-02 00:00:00.000000 mimllearning-1.0.8/docs/source/classifier/_autosummary/miml.classifier.mimlTOmi.miml_to_mi_br_classifier.MIMLtoMIBRClassifier.rst
--rw-r--r--   0        0        0      600 2020-02-02 00:00:00.000000 mimllearning-1.0.8/docs/source/classifier/_autosummary/miml.classifier.mimlTOmi.miml_to_mi_classifier.MIMLtoMIClassifier.rst
--rw-r--r--   0        0        0      631 2020-02-02 00:00:00.000000 mimllearning-1.0.8/docs/source/classifier/_autosummary/miml.classifier.mimlTOmi.miml_to_mi_lp_classifier.MIMLtoMILPClassifier.rst
--rw-r--r--   0        0        0      600 2020-02-02 00:00:00.000000 mimllearning-1.0.8/docs/source/classifier/_autosummary/miml.classifier.mimlTOml.miml_to_ml_classifier.MIMLtoMLClassifier.rst
--rw-r--r--   0        0        0      511 2020-02-02 00:00:00.000000 mimllearning-1.0.8/docs/source/classifier/_autosummary/miml.classifier.miml_classifier.MIMLClassifier.rst
--rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 mimllearning-1.0.8/docs/source/data/bag.rst
--rw-r--r--   0        0        0      149 2020-02-02 00:00:00.000000 mimllearning-1.0.8/docs/source/data/dataset_utils.rst
--rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 mimllearning-1.0.8/docs/source/data/index.rst
--rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 mimllearning-1.0.8/docs/source/data/instance.rst
--rw-r--r--   0        0        0      154 2020-02-02 00:00:00.000000 mimllearning-1.0.8/docs/source/data/miml_dataset.rst
--rw-r--r--   0        0        0      724 2020-02-02 00:00:00.000000 mimllearning-1.0.8/docs/source/data/_autosummary/miml.data.bag.Bag.rst
--rw-r--r--   0        0        0      199 2020-02-02 00:00:00.000000 mimllearning-1.0.8/docs/source/data/_autosummary/miml.data.instance.Instance.rst
--rw-r--r--   0        0        0     1507 2020-02-02 00:00:00.000000 mimllearning-1.0.8/docs/source/data/_autosummary/miml.data.miml_dataset.MIMLDataset.rst
--rw-r--r--   0        0        0       62 2020-02-02 00:00:00.000000 mimllearning-1.0.8/docs/source/report/index.rst
--rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 mimllearning-1.0.8/docs/source/report/report.rst
--rw-r--r--   0        0        0      392 2020-02-02 00:00:00.000000 mimllearning-1.0.8/docs/source/report/_autosummary/miml.report.report.Report.rst
--rw-r--r--   0        0        0       88 2020-02-02 00:00:00.000000 mimllearning-1.0.8/docs/source/transformation/index.rst
--rw-r--r--   0        0        0      280 2020-02-02 00:00:00.000000 mimllearning-1.0.8/docs/source/transformation/mimlTOmi.rst
--rw-r--r--   0        0        0      373 2020-02-02 00:00:00.000000 mimllearning-1.0.8/docs/source/transformation/mimlTOml.rst
--rw-r--r--   0        0        0      574 2020-02-02 00:00:00.000000 mimllearning-1.0.8/docs/source/transformation/_autosummary/miml.transformation.mimlTOmi.binary_relevance_transformation.BinaryRelevanceTransformation.rst
--rw-r--r--   0        0        0      656 2020-02-02 00:00:00.000000 mimllearning-1.0.8/docs/source/transformation/_autosummary/miml.transformation.mimlTOmi.label_powerset_transformation.LabelPowersetTransformation.rst
--rw-r--r--   0        0        0      477 2020-02-02 00:00:00.000000 mimllearning-1.0.8/docs/source/transformation/_autosummary/miml.transformation.mimlTOml.arithmetic.ArithmeticTransformation.rst
--rw-r--r--   0        0        0      468 2020-02-02 00:00:00.000000 mimllearning-1.0.8/docs/source/transformation/_autosummary/miml.transformation.mimlTOml.geometric.GeometricTransformation.rst
--rw-r--r--   0        0        0      516 2020-02-02 00:00:00.000000 mimllearning-1.0.8/docs/source/transformation/_autosummary/miml.transformation.mimlTOml.miml_to_ml_transformation.MIMLtoMLTransformation.rst
--rw-r--r--   0        0        0      441 2020-02-02 00:00:00.000000 mimllearning-1.0.8/docs/source/transformation/_autosummary/miml.transformation.mimlTOml.minmax.MinMaxTransformation.rst
--rw-r--r--   0        0        0   258069 2020-02-02 00:00:00.000000 mimllearning-1.0.8/documentation/AnteproyectoDamianTFG.pdf
--rw-r--r--   0        0        0      137 2020-02-02 00:00:00.000000 mimllearning-1.0.8/src/miml/__init__.py
--rw-r--r--   0        0        0      145 2020-02-02 00:00:00.000000 mimllearning-1.0.8/src/miml/classifier/__init__.py
--rw-r--r--   0        0        0     3230 2020-02-02 00:00:00.000000 mimllearning-1.0.8/src/miml/classifier/miml_classifier.py
--rw-r--r--   0        0        0       99 2020-02-02 00:00:00.000000 mimllearning-1.0.8/src/miml/classifier/mi/__init__.py
--rw-r--r--   0        0        0     3233 2020-02-02 00:00:00.000000 mimllearning-1.0.8/src/miml/classifier/mi/apr_classifier.py
--rw-r--r--   0        0        0     3677 2020-02-02 00:00:00.000000 mimllearning-1.0.8/src/miml/classifier/mi/mi_wrapper_classifier.py
--rw-r--r--   0        0        0      175 2020-02-02 00:00:00.000000 mimllearning-1.0.8/src/miml/classifier/mimlTOmi/__init__.py
--rw-r--r--   0        0        0     3083 2020-02-02 00:00:00.000000 mimllearning-1.0.8/src/miml/classifier/mimlTOmi/miml_to_mi_br_classifier.py
--rw-r--r--   0        0        0     3139 2020-02-02 00:00:00.000000 mimllearning-1.0.8/src/miml/classifier/mimlTOmi/miml_to_mi_classifier.py
--rw-r--r--   0        0        0     2980 2020-02-02 00:00:00.000000 mimllearning-1.0.8/src/miml/classifier/mimlTOmi/miml_to_mi_lp_classifier.py
--rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 mimllearning-1.0.8/src/miml/classifier/mimlTOml/__init__.py
--rw-r--r--   0        0        0     4211 2020-02-02 00:00:00.000000 mimllearning-1.0.8/src/miml/classifier/mimlTOml/miml_to_ml_classifier.py
--rw-r--r--   0        0        0      134 2020-02-02 00:00:00.000000 mimllearning-1.0.8/src/miml/data/__init__.py
--rw-r--r--   0        0        0    10742 2020-02-02 00:00:00.000000 mimllearning-1.0.8/src/miml/data/bag.py
--rw-r--r--   0        0        0     6624 2020-02-02 00:00:00.000000 mimllearning-1.0.8/src/miml/data/dataset_utils.py
--rw-r--r--   0        0        0     6845 2020-02-02 00:00:00.000000 mimllearning-1.0.8/src/miml/data/instance.py
--rw-r--r--   0        0        0    27336 2020-02-02 00:00:00.000000 mimllearning-1.0.8/src/miml/data/miml_dataset.py
--rw-r--r--   0        0        0   735908 2020-02-02 00:00:00.000000 mimllearning-1.0.8/src/miml/datasets/miml_birds.arff
--rw-r--r--   0        0        0   842801 2020-02-02 00:00:00.000000 mimllearning-1.0.8/src/miml/datasets/miml_birds.csv
--rw-r--r--   0        0        0   134841 2020-02-02 00:00:00.000000 mimllearning-1.0.8/src/miml/datasets/miml_birds_random_20test.arff
--rw-r--r--   0        0        0   498562 2020-02-02 00:00:00.000000 mimllearning-1.0.8/src/miml/datasets/miml_birds_random_80train.arff
--rw-r--r--   0        0        0      377 2020-02-02 00:00:00.000000 mimllearning-1.0.8/src/miml/datasets/toy.arff
--rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 mimllearning-1.0.8/src/miml/report/__init__.py
--rw-r--r--   0        0        0     9612 2020-02-02 00:00:00.000000 mimllearning-1.0.8/src/miml/report/report.py
--rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 mimllearning-1.0.8/src/miml/transformation/__init__.py
--rw-r--r--   0        0        0      148 2020-02-02 00:00:00.000000 mimllearning-1.0.8/src/miml/transformation/mimlTOmi/__init__.py
--rw-r--r--   0        0        0     2414 2020-02-02 00:00:00.000000 mimllearning-1.0.8/src/miml/transformation/mimlTOmi/binary_relevance_transformation.py
--rw-r--r--   0        0        0     3470 2020-02-02 00:00:00.000000 mimllearning-1.0.8/src/miml/transformation/mimlTOmi/label_powerset_transformation.py
--rw-r--r--   0        0        0      203 2020-02-02 00:00:00.000000 mimllearning-1.0.8/src/miml/transformation/mimlTOml/__init__.py
--rw-r--r--   0        0        0     2652 2020-02-02 00:00:00.000000 mimllearning-1.0.8/src/miml/transformation/mimlTOml/arithmetic.py
--rw-r--r--   0        0        0     2757 2020-02-02 00:00:00.000000 mimllearning-1.0.8/src/miml/transformation/mimlTOml/geometric.py
--rw-r--r--   0        0        0      472 2020-02-02 00:00:00.000000 mimllearning-1.0.8/src/miml/transformation/mimlTOml/miml_to_ml_transformation.py
--rw-r--r--   0        0        0     3041 2020-02-02 00:00:00.000000 mimllearning-1.0.8/src/miml/transformation/mimlTOml/minmax.py
--rw-r--r--   0        0        0   140069 2020-02-02 00:00:00.000000 mimllearning-1.0.8/src/miml/tutorial/classifiers_comparison_experiment_miml.ipynb
--rw-r--r--   0        0        0     6180 2020-02-02 00:00:00.000000 mimllearning-1.0.8/src/miml/tutorial/classifiers_mimltomi.ipynb
--rw-r--r--   0        0        0    16103 2020-02-02 00:00:00.000000 mimllearning-1.0.8/src/miml/tutorial/classifiers_mimltoml.ipynb
--rw-r--r--   0        0        0   172650 2020-02-02 00:00:00.000000 mimllearning-1.0.8/src/miml/tutorial/data_miml.ipynb
--rw-r--r--   0        0        0     6592 2020-02-02 00:00:00.000000 mimllearning-1.0.8/src/miml/tutorial/train_test_experiment_miml.ipynb
--rw-r--r--   0        0        0    14927 2020-02-02 00:00:00.000000 mimllearning-1.0.8/src/miml/tutorial/transformations_miml.ipynb
--rw-r--r--   0        0        0      328 2020-02-02 00:00:00.000000 mimllearning-1.0.8/.gitignore
--rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 mimllearning-1.0.8/LICENSE.txt
--rw-r--r--   0        0        0     1839 2020-02-02 00:00:00.000000 mimllearning-1.0.8/README.md
--rw-r--r--   0        0        0      831 2020-02-02 00:00:00.000000 mimllearning-1.0.8/pyproject.toml
--rw-r--r--   0        0        0     2356 2020-02-02 00:00:00.000000 mimllearning-1.0.8/PKG-INFO
+-rw-r--r--   0        0        0     1839 2020-02-02 00:00:00.000000 mimllearning-1.0.9/readme.md
+-rw-r--r--   0        0        0     1307 2020-02-02 00:00:00.000000 mimllearning-1.0.9/.github/workflows/static.yml
+-rw-r--r--   0        0        0      625 2020-02-02 00:00:00.000000 mimllearning-1.0.9/docs/Makefile
+-rwxr-xr-x   0        0        0      800 2020-02-02 00:00:00.000000 mimllearning-1.0.9/docs/make.bat
+-rw-r--r--   0        0        0   543085 2020-02-02 00:00:00.000000 mimllearning-1.0.9/docs/build/doctrees/environment.pickle
+-rw-r--r--   0        0        0     2817 2020-02-02 00:00:00.000000 mimllearning-1.0.9/docs/build/doctrees/miml.doctree
+-rw-r--r--   0        0        0     2856 2020-02-02 00:00:00.000000 mimllearning-1.0.9/docs/build/doctrees/classifier/index.doctree
+-rw-r--r--   0        0        0     6082 2020-02-02 00:00:00.000000 mimllearning-1.0.9/docs/build/doctrees/classifier/mi.doctree
+-rw-r--r--   0        0        0     7561 2020-02-02 00:00:00.000000 mimllearning-1.0.9/docs/build/doctrees/classifier/mimlTOmi.doctree
+-rw-r--r--   0        0        0     4479 2020-02-02 00:00:00.000000 mimllearning-1.0.9/docs/build/doctrees/classifier/mimlTOml.doctree
+-rw-r--r--   0        0        0     4564 2020-02-02 00:00:00.000000 mimllearning-1.0.9/docs/build/doctrees/classifier/miml_classifier.doctree
+-rw-r--r--   0        0        0    14723 2020-02-02 00:00:00.000000 mimllearning-1.0.9/docs/build/doctrees/classifier/_autosummary/miml.classifier.mi.apr_classifier.APRClassifier.doctree
+-rw-r--r--   0        0        0    15004 2020-02-02 00:00:00.000000 mimllearning-1.0.9/docs/build/doctrees/classifier/_autosummary/miml.classifier.mi.mi_wrapper_classifier.MIWrapperClassifier.doctree
+-rw-r--r--   0        0        0    18929 2020-02-02 00:00:00.000000 mimllearning-1.0.9/docs/build/doctrees/classifier/_autosummary/miml.classifier.mimlTOmi.miml_to_mi_br_classifier.MIMLtoMIBRClassifier.doctree
+-rw-r--r--   0        0        0    18554 2020-02-02 00:00:00.000000 mimllearning-1.0.9/docs/build/doctrees/classifier/_autosummary/miml.classifier.mimlTOmi.miml_to_mi_classifier.MIMLtoMIClassifier.doctree
+-rw-r--r--   0        0        0    18925 2020-02-02 00:00:00.000000 mimllearning-1.0.9/docs/build/doctrees/classifier/_autosummary/miml.classifier.mimlTOmi.miml_to_mi_lp_classifier.MIMLtoMILPClassifier.doctree
+-rw-r--r--   0        0        0    21010 2020-02-02 00:00:00.000000 mimllearning-1.0.9/docs/build/doctrees/classifier/_autosummary/miml.classifier.mimlTOml.miml_to_ml_classifier.MIMLtoMLClassifier.doctree
+-rw-r--r--   0        0        0    15952 2020-02-02 00:00:00.000000 mimllearning-1.0.9/docs/build/doctrees/classifier/_autosummary/miml.classifier.miml_classifier.MIMLClassifier.doctree
+-rw-r--r--   0        0        0     4387 2020-02-02 00:00:00.000000 mimllearning-1.0.9/docs/build/doctrees/data/bag.doctree
+-rw-r--r--   0        0        0     4014 2020-02-02 00:00:00.000000 mimllearning-1.0.9/docs/build/doctrees/data/dataset_utils.doctree
+-rw-r--r--   0        0        0     2799 2020-02-02 00:00:00.000000 mimllearning-1.0.9/docs/build/doctrees/data/index.doctree
+-rw-r--r--   0        0        0     4557 2020-02-02 00:00:00.000000 mimllearning-1.0.9/docs/build/doctrees/data/instance.doctree
+-rw-r--r--   0        0        0     4600 2020-02-02 00:00:00.000000 mimllearning-1.0.9/docs/build/doctrees/data/miml_dataset.doctree
+-rw-r--r--   0        0        0    31754 2020-02-02 00:00:00.000000 mimllearning-1.0.9/docs/build/doctrees/data/_autosummary/miml.data.bag.Bag.doctree
+-rw-r--r--   0        0        0    52596 2020-02-02 00:00:00.000000 mimllearning-1.0.9/docs/build/doctrees/data/_autosummary/miml.data.instance.Instance.doctree
+-rw-r--r--   0        0        0    53297 2020-02-02 00:00:00.000000 mimllearning-1.0.9/docs/build/doctrees/data/_autosummary/miml.data.miml_dataset.MIMLDataset.doctree
+-rw-r--r--   0        0        0     2742 2020-02-02 00:00:00.000000 mimllearning-1.0.9/docs/build/doctrees/report/index.doctree
+-rw-r--r--   0        0        0     4345 2020-02-02 00:00:00.000000 mimllearning-1.0.9/docs/build/doctrees/report/report.doctree
+-rw-r--r--   0        0        0    20548 2020-02-02 00:00:00.000000 mimllearning-1.0.9/docs/build/doctrees/report/_autosummary/miml.report.report.Report.doctree
+-rw-r--r--   0        0        0     2833 2020-02-02 00:00:00.000000 mimllearning-1.0.9/docs/build/doctrees/transformation/index.doctree
+-rw-r--r--   0        0        0     6481 2020-02-02 00:00:00.000000 mimllearning-1.0.9/docs/build/doctrees/transformation/mimlTOmi.doctree
+-rw-r--r--   0        0        0     9116 2020-02-02 00:00:00.000000 mimllearning-1.0.9/docs/build/doctrees/transformation/mimlTOml.doctree
+-rw-r--r--   0        0        0    12013 2020-02-02 00:00:00.000000 mimllearning-1.0.9/docs/build/doctrees/transformation/_autosummary/miml.transformation.mimlTOmi.binary_relevance_transformation.BinaryRelevanceTransformation.doctree
+-rw-r--r--   0        0        0    14709 2020-02-02 00:00:00.000000 mimllearning-1.0.9/docs/build/doctrees/transformation/_autosummary/miml.transformation.mimlTOmi.label_powerset_transformation.LabelPowersetTransformation.doctree
+-rw-r--r--   0        0        0    11160 2020-02-02 00:00:00.000000 mimllearning-1.0.9/docs/build/doctrees/transformation/_autosummary/miml.transformation.mimlTOml.arithmetic.ArithmeticTransformation.doctree
+-rw-r--r--   0        0        0    11106 2020-02-02 00:00:00.000000 mimllearning-1.0.9/docs/build/doctrees/transformation/_autosummary/miml.transformation.mimlTOml.geometric.GeometricTransformation.doctree
+-rw-r--r--   0        0        0    10938 2020-02-02 00:00:00.000000 mimllearning-1.0.9/docs/build/doctrees/transformation/_autosummary/miml.transformation.mimlTOml.miml_to_ml_transformation.MIMLtoMLTransformation.doctree
+-rw-r--r--   0        0        0    10848 2020-02-02 00:00:00.000000 mimllearning-1.0.9/docs/build/doctrees/transformation/_autosummary/miml.transformation.mimlTOml.minmax.MinMaxTransformation.doctree
+-rw-r--r--   0        0        0      230 2020-02-02 00:00:00.000000 mimllearning-1.0.9/docs/build/html/.buildinfo
+-rw-r--r--   0        0        0    31431 2020-02-02 00:00:00.000000 mimllearning-1.0.9/docs/build/html/genindex.html
+-rw-r--r--   0        0        0    20453 2020-02-02 00:00:00.000000 mimllearning-1.0.9/docs/build/html/index.html
+-rw-r--r--   0        0        0     1149 2020-02-02 00:00:00.000000 mimllearning-1.0.9/docs/build/html/objects.inv
+-rw-r--r--   0        0        0    18108 2020-02-02 00:00:00.000000 mimllearning-1.0.9/docs/build/html/search.html
+-rw-r--r--   0        0        0    23504 2020-02-02 00:00:00.000000 mimllearning-1.0.9/docs/build/html/searchindex.js
+-rw-r--r--   0        0        0      164 2020-02-02 00:00:00.000000 mimllearning-1.0.9/docs/build/html/_sources/miml.rst
+-rw-r--r--   0        0        0      112 2020-02-02 00:00:00.000000 mimllearning-1.0.9/docs/build/html/_sources/classifier/index.rst
+-rw-r--r--   0        0        0      170 2020-02-02 00:00:00.000000 mimllearning-1.0.9/docs/build/html/_sources/classifier/mi.rst
+-rw-r--r--   0        0        0      301 2020-02-02 00:00:00.000000 mimllearning-1.0.9/docs/build/html/_sources/classifier/mimlTOmi.rst
+-rw-r--r--   0        0        0      156 2020-02-02 00:00:00.000000 mimllearning-1.0.9/docs/build/html/_sources/classifier/mimlTOml.rst
+-rw-r--r--   0        0        0      151 2020-02-02 00:00:00.000000 mimllearning-1.0.9/docs/build/html/_sources/classifier/miml_classifier.rst
+-rw-r--r--   0        0        0      410 2020-02-02 00:00:00.000000 mimllearning-1.0.9/docs/build/html/_sources/classifier/_autosummary/miml.classifier.mi.apr_classifier.APRClassifier.rst
+-rw-r--r--   0        0        0      475 2020-02-02 00:00:00.000000 mimllearning-1.0.9/docs/build/html/_sources/classifier/_autosummary/miml.classifier.mi.mi_wrapper_classifier.MIWrapperClassifier.rst
+-rw-r--r--   0        0        0      631 2020-02-02 00:00:00.000000 mimllearning-1.0.9/docs/build/html/_sources/classifier/_autosummary/miml.classifier.mimlTOmi.miml_to_mi_br_classifier.MIMLtoMIBRClassifier.rst
+-rw-r--r--   0        0        0      600 2020-02-02 00:00:00.000000 mimllearning-1.0.9/docs/build/html/_sources/classifier/_autosummary/miml.classifier.mimlTOmi.miml_to_mi_classifier.MIMLtoMIClassifier.rst
+-rw-r--r--   0        0        0      631 2020-02-02 00:00:00.000000 mimllearning-1.0.9/docs/build/html/_sources/classifier/_autosummary/miml.classifier.mimlTOmi.miml_to_mi_lp_classifier.MIMLtoMILPClassifier.rst
+-rw-r--r--   0        0        0      600 2020-02-02 00:00:00.000000 mimllearning-1.0.9/docs/build/html/_sources/classifier/_autosummary/miml.classifier.mimlTOml.miml_to_ml_classifier.MIMLtoMLClassifier.rst
+-rw-r--r--   0        0        0      511 2020-02-02 00:00:00.000000 mimllearning-1.0.9/docs/build/html/_sources/classifier/_autosummary/miml.classifier.miml_classifier.MIMLClassifier.rst
+-rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 mimllearning-1.0.9/docs/build/html/_sources/data/bag.rst
+-rw-r--r--   0        0        0      149 2020-02-02 00:00:00.000000 mimllearning-1.0.9/docs/build/html/_sources/data/dataset_utils.rst
+-rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 mimllearning-1.0.9/docs/build/html/_sources/data/index.rst
+-rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 mimllearning-1.0.9/docs/build/html/_sources/data/instance.rst
+-rw-r--r--   0        0        0      154 2020-02-02 00:00:00.000000 mimllearning-1.0.9/docs/build/html/_sources/data/miml_dataset.rst
+-rw-r--r--   0        0        0      724 2020-02-02 00:00:00.000000 mimllearning-1.0.9/docs/build/html/_sources/data/_autosummary/miml.data.bag.Bag.rst
+-rw-r--r--   0        0        0      199 2020-02-02 00:00:00.000000 mimllearning-1.0.9/docs/build/html/_sources/data/_autosummary/miml.data.instance.Instance.rst
+-rw-r--r--   0        0        0     1507 2020-02-02 00:00:00.000000 mimllearning-1.0.9/docs/build/html/_sources/data/_autosummary/miml.data.miml_dataset.MIMLDataset.rst
+-rw-r--r--   0        0        0       62 2020-02-02 00:00:00.000000 mimllearning-1.0.9/docs/build/html/_sources/report/index.rst
+-rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 mimllearning-1.0.9/docs/build/html/_sources/report/report.rst
+-rw-r--r--   0        0        0      392 2020-02-02 00:00:00.000000 mimllearning-1.0.9/docs/build/html/_sources/report/_autosummary/miml.report.report.Report.rst
+-rw-r--r--   0        0        0       88 2020-02-02 00:00:00.000000 mimllearning-1.0.9/docs/build/html/_sources/transformation/index.rst
+-rw-r--r--   0        0        0      280 2020-02-02 00:00:00.000000 mimllearning-1.0.9/docs/build/html/_sources/transformation/mimlTOmi.rst
+-rw-r--r--   0        0        0      373 2020-02-02 00:00:00.000000 mimllearning-1.0.9/docs/build/html/_sources/transformation/mimlTOml.rst
+-rw-r--r--   0        0        0      574 2020-02-02 00:00:00.000000 mimllearning-1.0.9/docs/build/html/_sources/transformation/_autosummary/miml.transformation.mimlTOmi.binary_relevance_transformation.BinaryRelevanceTransformation.rst
+-rw-r--r--   0        0        0      656 2020-02-02 00:00:00.000000 mimllearning-1.0.9/docs/build/html/_sources/transformation/_autosummary/miml.transformation.mimlTOmi.label_powerset_transformation.LabelPowersetTransformation.rst
+-rw-r--r--   0        0        0      477 2020-02-02 00:00:00.000000 mimllearning-1.0.9/docs/build/html/_sources/transformation/_autosummary/miml.transformation.mimlTOml.arithmetic.ArithmeticTransformation.rst
+-rw-r--r--   0        0        0      468 2020-02-02 00:00:00.000000 mimllearning-1.0.9/docs/build/html/_sources/transformation/_autosummary/miml.transformation.mimlTOml.geometric.GeometricTransformation.rst
+-rw-r--r--   0        0        0      516 2020-02-02 00:00:00.000000 mimllearning-1.0.9/docs/build/html/_sources/transformation/_autosummary/miml.transformation.mimlTOml.miml_to_ml_transformation.MIMLtoMLTransformation.rst
+-rw-r--r--   0        0        0      441 2020-02-02 00:00:00.000000 mimllearning-1.0.9/docs/build/html/_sources/transformation/_autosummary/miml.transformation.mimlTOml.minmax.MinMaxTransformation.rst
+-rw-r--r--   0        0        0    15094 2020-02-02 00:00:00.000000 mimllearning-1.0.9/docs/build/html/_static/basic.css
+-rw-r--r--   0        0        0     4472 2020-02-02 00:00:00.000000 mimllearning-1.0.9/docs/build/html/_static/doctools.js
+-rw-r--r--   0        0        0      319 2020-02-02 00:00:00.000000 mimllearning-1.0.9/docs/build/html/_static/documentation_options.js
+-rw-r--r--   0        0        0      286 2020-02-02 00:00:00.000000 mimllearning-1.0.9/docs/build/html/_static/file.png
+-rw-r--r--   0        0        0     4758 2020-02-02 00:00:00.000000 mimllearning-1.0.9/docs/build/html/_static/language_data.js
+-rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 mimllearning-1.0.9/docs/build/html/_static/minus.png
+-rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 mimllearning-1.0.9/docs/build/html/_static/plus.png
+-rw-r--r--   0        0        0    12755 2020-02-02 00:00:00.000000 mimllearning-1.0.9/docs/build/html/_static/pygments.css
+-rw-r--r--   0        0        0      419 2020-02-02 00:00:00.000000 mimllearning-1.0.9/docs/build/html/_static/sbt-webpack-macros.html
+-rw-r--r--   0        0        0    20731 2020-02-02 00:00:00.000000 mimllearning-1.0.9/docs/build/html/_static/searchtools.js
+-rw-r--r--   0        0        0     5123 2020-02-02 00:00:00.000000 mimllearning-1.0.9/docs/build/html/_static/sphinx_highlight.js
+-rw-r--r--   0        0        0     1983 2020-02-02 00:00:00.000000 mimllearning-1.0.9/docs/build/html/_static/webpack-macros.html
+-rw-r--r--   0        0        0     1186 2020-02-02 00:00:00.000000 mimllearning-1.0.9/docs/build/html/_static/images/logo_binder.svg
+-rw-r--r--   0        0        0     7601 2020-02-02 00:00:00.000000 mimllearning-1.0.9/docs/build/html/_static/images/logo_colab.png
+-rw-r--r--   0        0        0      681 2020-02-02 00:00:00.000000 mimllearning-1.0.9/docs/build/html/_static/images/logo_deepnote.svg
+-rw-r--r--   0        0        0     1758 2020-02-02 00:00:00.000000 mimllearning-1.0.9/docs/build/html/_static/images/logo_jupyterhub.svg
+-rw-r--r--   0        0        0     1541 2020-02-02 00:00:00.000000 mimllearning-1.0.9/docs/build/html/_static/locales/ar/LC_MESSAGES/booktheme.mo
+-rw-r--r--   0        0        0     1459 2020-02-02 00:00:00.000000 mimllearning-1.0.9/docs/build/html/_static/locales/ar/LC_MESSAGES/booktheme.po
+-rw-r--r--   0        0        0     1708 2020-02-02 00:00:00.000000 mimllearning-1.0.9/docs/build/html/_static/locales/bg/LC_MESSAGES/booktheme.mo
+-rw-r--r--   0        0        0     1626 2020-02-02 00:00:00.000000 mimllearning-1.0.9/docs/build/html/_static/locales/bg/LC_MESSAGES/booktheme.po
+-rw-r--r--   0        0        0     1646 2020-02-02 00:00:00.000000 mimllearning-1.0.9/docs/build/html/_static/locales/bn/LC_MESSAGES/booktheme.mo
+-rw-r--r--   0        0        0     1564 2020-02-02 00:00:00.000000 mimllearning-1.0.9/docs/build/html/_static/locales/bn/LC_MESSAGES/booktheme.po
+-rw-r--r--   0        0        0     1246 2020-02-02 00:00:00.000000 mimllearning-1.0.9/docs/build/html/_static/locales/ca/LC_MESSAGES/booktheme.mo
+-rw-r--r--   0        0        0     1166 2020-02-02 00:00:00.000000 mimllearning-1.0.9/docs/build/html/_static/locales/ca/LC_MESSAGES/booktheme.po
+-rw-r--r--   0        0        0     1405 2020-02-02 00:00:00.000000 mimllearning-1.0.9/docs/build/html/_static/locales/cs/LC_MESSAGES/booktheme.mo
+-rw-r--r--   0        0        0     1323 2020-02-02 00:00:00.000000 mimllearning-1.0.9/docs/build/html/_static/locales/cs/LC_MESSAGES/booktheme.po
+-rw-r--r--   0        0        0     1304 2020-02-02 00:00:00.000000 mimllearning-1.0.9/docs/build/html/_static/locales/da/LC_MESSAGES/booktheme.mo
+-rw-r--r--   0        0        0     1222 2020-02-02 00:00:00.000000 mimllearning-1.0.9/docs/build/html/_static/locales/da/LC_MESSAGES/booktheme.po
+-rw-r--r--   0        0        0     1388 2020-02-02 00:00:00.000000 mimllearning-1.0.9/docs/build/html/_static/locales/de/LC_MESSAGES/booktheme.mo
+-rw-r--r--   0        0        0     1306 2020-02-02 00:00:00.000000 mimllearning-1.0.9/docs/build/html/_static/locales/de/LC_MESSAGES/booktheme.po
+-rw-r--r--   0        0        0     1722 2020-02-02 00:00:00.000000 mimllearning-1.0.9/docs/build/html/_static/locales/el/LC_MESSAGES/booktheme.mo
+-rw-r--r--   0        0        0     1640 2020-02-02 00:00:00.000000 mimllearning-1.0.9/docs/build/html/_static/locales/el/LC_MESSAGES/booktheme.po
+-rw-r--r--   0        0        0     1337 2020-02-02 00:00:00.000000 mimllearning-1.0.9/docs/build/html/_static/locales/eo/LC_MESSAGES/booktheme.mo
+-rw-r--r--   0        0        0     1255 2020-02-02 00:00:00.000000 mimllearning-1.0.9/docs/build/html/_static/locales/eo/LC_MESSAGES/booktheme.po
+-rw-r--r--   0        0        0     1396 2020-02-02 00:00:00.000000 mimllearning-1.0.9/docs/build/html/_static/locales/es/LC_MESSAGES/booktheme.mo
+-rw-r--r--   0        0        0     1314 2020-02-02 00:00:00.000000 mimllearning-1.0.9/docs/build/html/_static/locales/es/LC_MESSAGES/booktheme.po
+-rw-r--r--   0        0        0     1341 2020-02-02 00:00:00.000000 mimllearning-1.0.9/docs/build/html/_static/locales/et/LC_MESSAGES/booktheme.mo
+-rw-r--r--   0        0        0     1259 2020-02-02 00:00:00.000000 mimllearning-1.0.9/docs/build/html/_static/locales/et/LC_MESSAGES/booktheme.po
+-rw-r--r--   0        0        0     1368 2020-02-02 00:00:00.000000 mimllearning-1.0.9/docs/build/html/_static/locales/fi/LC_MESSAGES/booktheme.mo
+-rw-r--r--   0        0        0     1286 2020-02-02 00:00:00.000000 mimllearning-1.0.9/docs/build/html/_static/locales/fi/LC_MESSAGES/booktheme.po
+-rw-r--r--   0        0        0     1412 2020-02-02 00:00:00.000000 mimllearning-1.0.9/docs/build/html/_static/locales/fr/LC_MESSAGES/booktheme.mo
+-rw-r--r--   0        0        0     1330 2020-02-02 00:00:00.000000 mimllearning-1.0.9/docs/build/html/_static/locales/fr/LC_MESSAGES/booktheme.po
+-rw-r--r--   0        0        0     1402 2020-02-02 00:00:00.000000 mimllearning-1.0.9/docs/build/html/_static/locales/hr/LC_MESSAGES/booktheme.mo
+-rw-r--r--   0        0        0     1320 2020-02-02 00:00:00.000000 mimllearning-1.0.9/docs/build/html/_static/locales/hr/LC_MESSAGES/booktheme.po
+-rw-r--r--   0        0        0     1323 2020-02-02 00:00:00.000000 mimllearning-1.0.9/docs/build/html/_static/locales/id/LC_MESSAGES/booktheme.mo
+-rw-r--r--   0        0        0     1241 2020-02-02 00:00:00.000000 mimllearning-1.0.9/docs/build/html/_static/locales/id/LC_MESSAGES/booktheme.po
+-rw-r--r--   0        0        0     1403 2020-02-02 00:00:00.000000 mimllearning-1.0.9/docs/build/html/_static/locales/it/LC_MESSAGES/booktheme.mo
+-rw-r--r--   0        0        0     1321 2020-02-02 00:00:00.000000 mimllearning-1.0.9/docs/build/html/_static/locales/it/LC_MESSAGES/booktheme.po
+-rw-r--r--   0        0        0     1445 2020-02-02 00:00:00.000000 mimllearning-1.0.9/docs/build/html/_static/locales/iw/LC_MESSAGES/booktheme.mo
+-rw-r--r--   0        0        0     1363 2020-02-02 00:00:00.000000 mimllearning-1.0.9/docs/build/html/_static/locales/iw/LC_MESSAGES/booktheme.po
+-rw-r--r--   0        0        0     1471 2020-02-02 00:00:00.000000 mimllearning-1.0.9/docs/build/html/_static/locales/ja/LC_MESSAGES/booktheme.mo
+-rw-r--r--   0        0        0     1389 2020-02-02 00:00:00.000000 mimllearning-1.0.9/docs/build/html/_static/locales/ja/LC_MESSAGES/booktheme.po
+-rw-r--r--   0        0        0     1375 2020-02-02 00:00:00.000000 mimllearning-1.0.9/docs/build/html/_static/locales/ko/LC_MESSAGES/booktheme.mo
+-rw-r--r--   0        0        0     1293 2020-02-02 00:00:00.000000 mimllearning-1.0.9/docs/build/html/_static/locales/ko/LC_MESSAGES/booktheme.po
+-rw-r--r--   0        0        0     1413 2020-02-02 00:00:00.000000 mimllearning-1.0.9/docs/build/html/_static/locales/lt/LC_MESSAGES/booktheme.mo
+-rw-r--r--   0        0        0     1331 2020-02-02 00:00:00.000000 mimllearning-1.0.9/docs/build/html/_static/locales/lt/LC_MESSAGES/booktheme.po
+-rw-r--r--   0        0        0     1404 2020-02-02 00:00:00.000000 mimllearning-1.0.9/docs/build/html/_static/locales/lv/LC_MESSAGES/booktheme.mo
+-rw-r--r--   0        0        0     1322 2020-02-02 00:00:00.000000 mimllearning-1.0.9/docs/build/html/_static/locales/lv/LC_MESSAGES/booktheme.po
+-rw-r--r--   0        0        0     1883 2020-02-02 00:00:00.000000 mimllearning-1.0.9/docs/build/html/_static/locales/ml/LC_MESSAGES/booktheme.mo
+-rw-r--r--   0        0        0     1803 2020-02-02 00:00:00.000000 mimllearning-1.0.9/docs/build/html/_static/locales/ml/LC_MESSAGES/booktheme.po
+-rw-r--r--   0        0        0     1674 2020-02-02 00:00:00.000000 mimllearning-1.0.9/docs/build/html/_static/locales/mr/LC_MESSAGES/booktheme.mo
+-rw-r--r--   0        0        0     1594 2020-02-02 00:00:00.000000 mimllearning-1.0.9/docs/build/html/_static/locales/mr/LC_MESSAGES/booktheme.po
+-rw-r--r--   0        0        0     1213 2020-02-02 00:00:00.000000 mimllearning-1.0.9/docs/build/html/_static/locales/ms/LC_MESSAGES/booktheme.mo
+-rw-r--r--   0        0        0     1133 2020-02-02 00:00:00.000000 mimllearning-1.0.9/docs/build/html/_static/locales/ms/LC_MESSAGES/booktheme.po
+-rw-r--r--   0        0        0     1356 2020-02-02 00:00:00.000000 mimllearning-1.0.9/docs/build/html/_static/locales/nl/LC_MESSAGES/booktheme.mo
+-rw-r--r--   0        0        0     1274 2020-02-02 00:00:00.000000 mimllearning-1.0.9/docs/build/html/_static/locales/nl/LC_MESSAGES/booktheme.po
+-rw-r--r--   0        0        0     1317 2020-02-02 00:00:00.000000 mimllearning-1.0.9/docs/build/html/_static/locales/no/LC_MESSAGES/booktheme.mo
+-rw-r--r--   0        0        0     1235 2020-02-02 00:00:00.000000 mimllearning-1.0.9/docs/build/html/_static/locales/no/LC_MESSAGES/booktheme.po
+-rw-r--r--   0        0        0     1371 2020-02-02 00:00:00.000000 mimllearning-1.0.9/docs/build/html/_static/locales/pl/LC_MESSAGES/booktheme.mo
+-rw-r--r--   0        0        0     1289 2020-02-02 00:00:00.000000 mimllearning-1.0.9/docs/build/html/_static/locales/pl/LC_MESSAGES/booktheme.po
+-rw-r--r--   0        0        0     1364 2020-02-02 00:00:00.000000 mimllearning-1.0.9/docs/build/html/_static/locales/pt/LC_MESSAGES/booktheme.mo
+-rw-r--r--   0        0        0     1282 2020-02-02 00:00:00.000000 mimllearning-1.0.9/docs/build/html/_static/locales/pt/LC_MESSAGES/booktheme.po
+-rw-r--r--   0        0        0     1390 2020-02-02 00:00:00.000000 mimllearning-1.0.9/docs/build/html/_static/locales/ro/LC_MESSAGES/booktheme.mo
+-rw-r--r--   0        0        0     1308 2020-02-02 00:00:00.000000 mimllearning-1.0.9/docs/build/html/_static/locales/ro/LC_MESSAGES/booktheme.po
+-rw-r--r--   0        0        0     1722 2020-02-02 00:00:00.000000 mimllearning-1.0.9/docs/build/html/_static/locales/ru/LC_MESSAGES/booktheme.mo
+-rw-r--r--   0        0        0     1640 2020-02-02 00:00:00.000000 mimllearning-1.0.9/docs/build/html/_static/locales/ru/LC_MESSAGES/booktheme.po
+-rw-r--r--   0        0        0     1393 2020-02-02 00:00:00.000000 mimllearning-1.0.9/docs/build/html/_static/locales/sk/LC_MESSAGES/booktheme.mo
+-rw-r--r--   0        0        0     1311 2020-02-02 00:00:00.000000 mimllearning-1.0.9/docs/build/html/_static/locales/sk/LC_MESSAGES/booktheme.po
+-rw-r--r--   0        0        0     1374 2020-02-02 00:00:00.000000 mimllearning-1.0.9/docs/build/html/_static/locales/sl/LC_MESSAGES/booktheme.mo
+-rw-r--r--   0        0        0     1292 2020-02-02 00:00:00.000000 mimllearning-1.0.9/docs/build/html/_static/locales/sl/LC_MESSAGES/booktheme.po
+-rw-r--r--   0        0        0     1679 2020-02-02 00:00:00.000000 mimllearning-1.0.9/docs/build/html/_static/locales/sr/LC_MESSAGES/booktheme.mo
+-rw-r--r--   0        0        0     1597 2020-02-02 00:00:00.000000 mimllearning-1.0.9/docs/build/html/_static/locales/sr/LC_MESSAGES/booktheme.po
+-rw-r--r--   0        0        0     1365 2020-02-02 00:00:00.000000 mimllearning-1.0.9/docs/build/html/_static/locales/sv/LC_MESSAGES/booktheme.mo
+-rw-r--r--   0        0        0     1283 2020-02-02 00:00:00.000000 mimllearning-1.0.9/docs/build/html/_static/locales/sv/LC_MESSAGES/booktheme.po
+-rw-r--r--   0        0        0     1928 2020-02-02 00:00:00.000000 mimllearning-1.0.9/docs/build/html/_static/locales/ta/LC_MESSAGES/booktheme.mo
+-rw-r--r--   0        0        0     1848 2020-02-02 00:00:00.000000 mimllearning-1.0.9/docs/build/html/_static/locales/ta/LC_MESSAGES/booktheme.po
+-rw-r--r--   0        0        0     1806 2020-02-02 00:00:00.000000 mimllearning-1.0.9/docs/build/html/_static/locales/te/LC_MESSAGES/booktheme.mo
+-rw-r--r--   0        0        0     1726 2020-02-02 00:00:00.000000 mimllearning-1.0.9/docs/build/html/_static/locales/te/LC_MESSAGES/booktheme.po
+-rw-r--r--   0        0        0     1628 2020-02-02 00:00:00.000000 mimllearning-1.0.9/docs/build/html/_static/locales/tg/LC_MESSAGES/booktheme.mo
+-rw-r--r--   0        0        0     1546 2020-02-02 00:00:00.000000 mimllearning-1.0.9/docs/build/html/_static/locales/tg/LC_MESSAGES/booktheme.po
+-rw-r--r--   0        0        0     1766 2020-02-02 00:00:00.000000 mimllearning-1.0.9/docs/build/html/_static/locales/th/LC_MESSAGES/booktheme.mo
+-rw-r--r--   0        0        0     1684 2020-02-02 00:00:00.000000 mimllearning-1.0.9/docs/build/html/_static/locales/th/LC_MESSAGES/booktheme.po
+-rw-r--r--   0        0        0     1273 2020-02-02 00:00:00.000000 mimllearning-1.0.9/docs/build/html/_static/locales/tl/LC_MESSAGES/booktheme.mo
+-rw-r--r--   0        0        0     1193 2020-02-02 00:00:00.000000 mimllearning-1.0.9/docs/build/html/_static/locales/tl/LC_MESSAGES/booktheme.po
+-rw-r--r--   0        0        0     1373 2020-02-02 00:00:00.000000 mimllearning-1.0.9/docs/build/html/_static/locales/tr/LC_MESSAGES/booktheme.mo
+-rw-r--r--   0        0        0     1291 2020-02-02 00:00:00.000000 mimllearning-1.0.9/docs/build/html/_static/locales/tr/LC_MESSAGES/booktheme.po
+-rw-r--r--   0        0        0     1681 2020-02-02 00:00:00.000000 mimllearning-1.0.9/docs/build/html/_static/locales/uk/LC_MESSAGES/booktheme.mo
+-rw-r--r--   0        0        0     1601 2020-02-02 00:00:00.000000 mimllearning-1.0.9/docs/build/html/_static/locales/uk/LC_MESSAGES/booktheme.po
+-rw-r--r--   0        0        0     1462 2020-02-02 00:00:00.000000 mimllearning-1.0.9/docs/build/html/_static/locales/ur/LC_MESSAGES/booktheme.mo
+-rw-r--r--   0        0        0     1382 2020-02-02 00:00:00.000000 mimllearning-1.0.9/docs/build/html/_static/locales/ur/LC_MESSAGES/booktheme.po
+-rw-r--r--   0        0        0     1431 2020-02-02 00:00:00.000000 mimllearning-1.0.9/docs/build/html/_static/locales/vi/LC_MESSAGES/booktheme.mo
+-rw-r--r--   0        0        0     1349 2020-02-02 00:00:00.000000 mimllearning-1.0.9/docs/build/html/_static/locales/vi/LC_MESSAGES/booktheme.po
+-rw-r--r--   0        0        0     1310 2020-02-02 00:00:00.000000 mimllearning-1.0.9/docs/build/html/_static/locales/zh_CN/LC_MESSAGES/booktheme.mo
+-rw-r--r--   0        0        0     1228 2020-02-02 00:00:00.000000 mimllearning-1.0.9/docs/build/html/_static/locales/zh_CN/LC_MESSAGES/booktheme.po
+-rw-r--r--   0        0        0     1341 2020-02-02 00:00:00.000000 mimllearning-1.0.9/docs/build/html/_static/locales/zh_TW/LC_MESSAGES/booktheme.mo
+-rw-r--r--   0        0        0     1259 2020-02-02 00:00:00.000000 mimllearning-1.0.9/docs/build/html/_static/locales/zh_TW/LC_MESSAGES/booktheme.po
+-rw-r--r--   0        0        0    81602 2020-02-02 00:00:00.000000 mimllearning-1.0.9/docs/build/html/_static/scripts/bootstrap.js
+-rw-r--r--   0        0        0      237 2020-02-02 00:00:00.000000 mimllearning-1.0.9/docs/build/html/_static/scripts/bootstrap.js.LICENSE.txt
+-rw-r--r--   0        0        0   332914 2020-02-02 00:00:00.000000 mimllearning-1.0.9/docs/build/html/_static/scripts/bootstrap.js.map
+-rw-r--r--   0        0        0     9399 2020-02-02 00:00:00.000000 mimllearning-1.0.9/docs/build/html/_static/scripts/pydata-sphinx-theme.js
+-rw-r--r--   0        0        0    44317 2020-02-02 00:00:00.000000 mimllearning-1.0.9/docs/build/html/_static/scripts/pydata-sphinx-theme.js.map
+-rw-r--r--   0        0        0     3075 2020-02-02 00:00:00.000000 mimllearning-1.0.9/docs/build/html/_static/scripts/sphinx-book-theme.js
+-rw-r--r--   0        0        0    13066 2020-02-02 00:00:00.000000 mimllearning-1.0.9/docs/build/html/_static/scripts/sphinx-book-theme.js.map
+-rw-r--r--   0        0        0   208854 2020-02-02 00:00:00.000000 mimllearning-1.0.9/docs/build/html/_static/styles/bootstrap.css
+-rw-r--r--   0        0        0   555088 2020-02-02 00:00:00.000000 mimllearning-1.0.9/docs/build/html/_static/styles/bootstrap.css.map
+-rw-r--r--   0        0        0    72327 2020-02-02 00:00:00.000000 mimllearning-1.0.9/docs/build/html/_static/styles/pydata-sphinx-theme.css
+-rw-r--r--   0        0        0   294060 2020-02-02 00:00:00.000000 mimllearning-1.0.9/docs/build/html/_static/styles/pydata-sphinx-theme.css.map
+-rw-r--r--   0        0        0    14558 2020-02-02 00:00:00.000000 mimllearning-1.0.9/docs/build/html/_static/styles/sphinx-book-theme.css
+-rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 mimllearning-1.0.9/docs/build/html/_static/styles/theme.css
+-rw-r--r--   0        0        0     7427 2020-02-02 00:00:00.000000 mimllearning-1.0.9/docs/build/html/_static/vendor/fontawesome/6.5.1/LICENSE.txt
+-rw-r--r--   0        0        0   102621 2020-02-02 00:00:00.000000 mimllearning-1.0.9/docs/build/html/_static/vendor/fontawesome/6.5.1/css/all.min.css
+-rw-r--r--   0        0        0  1485766 2020-02-02 00:00:00.000000 mimllearning-1.0.9/docs/build/html/_static/vendor/fontawesome/6.5.1/js/all.min.js
+-rw-r--r--   0        0        0      219 2020-02-02 00:00:00.000000 mimllearning-1.0.9/docs/build/html/_static/vendor/fontawesome/6.5.1/js/all.min.js.LICENSE.txt
+-rw-r--r--   0        0        0   207972 2020-02-02 00:00:00.000000 mimllearning-1.0.9/docs/build/html/_static/vendor/fontawesome/6.5.1/webfonts/fa-brands-400.ttf
+-rw-r--r--   0        0        0   117372 2020-02-02 00:00:00.000000 mimllearning-1.0.9/docs/build/html/_static/vendor/fontawesome/6.5.1/webfonts/fa-brands-400.woff2
+-rw-r--r--   0        0        0    68004 2020-02-02 00:00:00.000000 mimllearning-1.0.9/docs/build/html/_static/vendor/fontawesome/6.5.1/webfonts/fa-regular-400.ttf
+-rw-r--r--   0        0        0    25452 2020-02-02 00:00:00.000000 mimllearning-1.0.9/docs/build/html/_static/vendor/fontawesome/6.5.1/webfonts/fa-regular-400.woff2
+-rw-r--r--   0        0        0   419720 2020-02-02 00:00:00.000000 mimllearning-1.0.9/docs/build/html/_static/vendor/fontawesome/6.5.1/webfonts/fa-solid-900.ttf
+-rw-r--r--   0        0        0   156496 2020-02-02 00:00:00.000000 mimllearning-1.0.9/docs/build/html/_static/vendor/fontawesome/6.5.1/webfonts/fa-solid-900.woff2
+-rw-r--r--   0        0        0    10832 2020-02-02 00:00:00.000000 mimllearning-1.0.9/docs/build/html/_static/vendor/fontawesome/6.5.1/webfonts/fa-v4compatibility.ttf
+-rw-r--r--   0        0        0     4792 2020-02-02 00:00:00.000000 mimllearning-1.0.9/docs/build/html/_static/vendor/fontawesome/6.5.1/webfonts/fa-v4compatibility.woff2
+-rw-r--r--   0        0        0    19595 2020-02-02 00:00:00.000000 mimllearning-1.0.9/docs/build/html/classifier/index.html
+-rw-r--r--   0        0        0    20416 2020-02-02 00:00:00.000000 mimllearning-1.0.9/docs/build/html/classifier/mi.html
+-rw-r--r--   0        0        0    21510 2020-02-02 00:00:00.000000 mimllearning-1.0.9/docs/build/html/classifier/mimlTOmi.html
+-rw-r--r--   0        0        0    20217 2020-02-02 00:00:00.000000 mimllearning-1.0.9/docs/build/html/classifier/mimlTOml.html
+-rw-r--r--   0        0        0    20198 2020-02-02 00:00:00.000000 mimllearning-1.0.9/docs/build/html/classifier/miml_classifier.html
+-rw-r--r--   0        0        0    24737 2020-02-02 00:00:00.000000 mimllearning-1.0.9/docs/build/html/classifier/_autosummary/miml.classifier.mi.apr_classifier.APRClassifier.html
+-rw-r--r--   0        0        0    24964 2020-02-02 00:00:00.000000 mimllearning-1.0.9/docs/build/html/classifier/_autosummary/miml.classifier.mi.mi_wrapper_classifier.MIWrapperClassifier.html
+-rw-r--r--   0        0        0    25646 2020-02-02 00:00:00.000000 mimllearning-1.0.9/docs/build/html/classifier/_autosummary/miml.classifier.mimlTOmi.miml_to_mi_br_classifier.MIMLtoMIBRClassifier.html
+-rw-r--r--   0        0        0    25287 2020-02-02 00:00:00.000000 mimllearning-1.0.9/docs/build/html/classifier/_autosummary/miml.classifier.mimlTOmi.miml_to_mi_classifier.MIMLtoMIClassifier.html
+-rw-r--r--   0        0        0    25424 2020-02-02 00:00:00.000000 mimllearning-1.0.9/docs/build/html/classifier/_autosummary/miml.classifier.mimlTOmi.miml_to_mi_lp_classifier.MIMLtoMILPClassifier.html
+-rw-r--r--   0        0        0    26240 2020-02-02 00:00:00.000000 mimllearning-1.0.9/docs/build/html/classifier/_autosummary/miml.classifier.mimlTOml.miml_to_ml_classifier.MIMLtoMLClassifier.html
+-rw-r--r--   0        0        0    24250 2020-02-02 00:00:00.000000 mimllearning-1.0.9/docs/build/html/classifier/_autosummary/miml.classifier.miml_classifier.MIMLClassifier.html
+-rw-r--r--   0        0        0    19868 2020-02-02 00:00:00.000000 mimllearning-1.0.9/docs/build/html/data/bag.html
+-rw-r--r--   0        0        0    19704 2020-02-02 00:00:00.000000 mimllearning-1.0.9/docs/build/html/data/dataset_utils.html
+-rw-r--r--   0        0        0    19980 2020-02-02 00:00:00.000000 mimllearning-1.0.9/docs/build/html/data/index.html
+-rw-r--r--   0        0        0    19878 2020-02-02 00:00:00.000000 mimllearning-1.0.9/docs/build/html/data/instance.html
+-rw-r--r--   0        0        0    20019 2020-02-02 00:00:00.000000 mimllearning-1.0.9/docs/build/html/data/miml_dataset.html
+-rw-r--r--   0        0        0    27162 2020-02-02 00:00:00.000000 mimllearning-1.0.9/docs/build/html/data/_autosummary/miml.data.bag.Bag.html
+-rw-r--r--   0        0        0    43163 2020-02-02 00:00:00.000000 mimllearning-1.0.9/docs/build/html/data/_autosummary/miml.data.instance.Instance.html
+-rw-r--r--   0        0        0    30686 2020-02-02 00:00:00.000000 mimllearning-1.0.9/docs/build/html/data/_autosummary/miml.data.miml_dataset.MIMLDataset.html
+-rw-r--r--   0        0        0    19479 2020-02-02 00:00:00.000000 mimllearning-1.0.9/docs/build/html/report/index.html
+-rw-r--r--   0        0        0    19845 2020-02-02 00:00:00.000000 mimllearning-1.0.9/docs/build/html/report/report.html
+-rw-r--r--   0        0        0    27555 2020-02-02 00:00:00.000000 mimllearning-1.0.9/docs/build/html/report/_autosummary/miml.report.report.Report.html
+-rw-r--r--   0        0        0    19571 2020-02-02 00:00:00.000000 mimllearning-1.0.9/docs/build/html/transformation/index.html
+-rw-r--r--   0        0        0    21018 2020-02-02 00:00:00.000000 mimllearning-1.0.9/docs/build/html/transformation/mimlTOmi.html
+-rw-r--r--   0        0        0    22202 2020-02-02 00:00:00.000000 mimllearning-1.0.9/docs/build/html/transformation/mimlTOml.html
+-rw-r--r--   0        0        0    24505 2020-02-02 00:00:00.000000 mimllearning-1.0.9/docs/build/html/transformation/_autosummary/miml.transformation.mimlTOmi.binary_relevance_transformation.BinaryRelevanceTransformation.html
+-rw-r--r--   0        0        0    24774 2020-02-02 00:00:00.000000 mimllearning-1.0.9/docs/build/html/transformation/_autosummary/miml.transformation.mimlTOmi.label_powerset_transformation.LabelPowersetTransformation.html
+-rw-r--r--   0        0        0    23957 2020-02-02 00:00:00.000000 mimllearning-1.0.9/docs/build/html/transformation/_autosummary/miml.transformation.mimlTOml.arithmetic.ArithmeticTransformation.html
+-rw-r--r--   0        0        0    24101 2020-02-02 00:00:00.000000 mimllearning-1.0.9/docs/build/html/transformation/_autosummary/miml.transformation.mimlTOml.geometric.GeometricTransformation.html
+-rw-r--r--   0        0        0    23685 2020-02-02 00:00:00.000000 mimllearning-1.0.9/docs/build/html/transformation/_autosummary/miml.transformation.mimlTOml.miml_to_ml_transformation.MIMLtoMLTransformation.html
+-rw-r--r--   0        0        0    24044 2020-02-02 00:00:00.000000 mimllearning-1.0.9/docs/build/html/transformation/_autosummary/miml.transformation.mimlTOml.minmax.MinMaxTransformation.html
+-rw-r--r--   0        0        0     1617 2020-02-02 00:00:00.000000 mimllearning-1.0.9/docs/source/conf.py
+-rw-r--r--   0        0        0      165 2020-02-02 00:00:00.000000 mimllearning-1.0.9/docs/source/index.rst
+-rw-r--r--   0        0        0      748 2020-02-02 00:00:00.000000 mimllearning-1.0.9/docs/source/_templates/base.rst
+-rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 mimllearning-1.0.9/docs/source/_templates/base.rstZone.Identifier
+-rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 mimllearning-1.0.9/docs/source/_templates/class.rst
+-rw-r--r--   0        0        0      112 2020-02-02 00:00:00.000000 mimllearning-1.0.9/docs/source/classifier/index.rst
+-rw-r--r--   0        0        0      170 2020-02-02 00:00:00.000000 mimllearning-1.0.9/docs/source/classifier/mi.rst
+-rw-r--r--   0        0        0      301 2020-02-02 00:00:00.000000 mimllearning-1.0.9/docs/source/classifier/mimlTOmi.rst
+-rw-r--r--   0        0        0      156 2020-02-02 00:00:00.000000 mimllearning-1.0.9/docs/source/classifier/mimlTOml.rst
+-rw-r--r--   0        0        0      151 2020-02-02 00:00:00.000000 mimllearning-1.0.9/docs/source/classifier/miml_classifier.rst
+-rw-r--r--   0        0        0      410 2020-02-02 00:00:00.000000 mimllearning-1.0.9/docs/source/classifier/_autosummary/miml.classifier.mi.apr_classifier.APRClassifier.rst
+-rw-r--r--   0        0        0      475 2020-02-02 00:00:00.000000 mimllearning-1.0.9/docs/source/classifier/_autosummary/miml.classifier.mi.mi_wrapper_classifier.MIWrapperClassifier.rst
+-rw-r--r--   0        0        0      631 2020-02-02 00:00:00.000000 mimllearning-1.0.9/docs/source/classifier/_autosummary/miml.classifier.mimlTOmi.miml_to_mi_br_classifier.MIMLtoMIBRClassifier.rst
+-rw-r--r--   0        0        0      600 2020-02-02 00:00:00.000000 mimllearning-1.0.9/docs/source/classifier/_autosummary/miml.classifier.mimlTOmi.miml_to_mi_classifier.MIMLtoMIClassifier.rst
+-rw-r--r--   0        0        0      631 2020-02-02 00:00:00.000000 mimllearning-1.0.9/docs/source/classifier/_autosummary/miml.classifier.mimlTOmi.miml_to_mi_lp_classifier.MIMLtoMILPClassifier.rst
+-rw-r--r--   0        0        0      600 2020-02-02 00:00:00.000000 mimllearning-1.0.9/docs/source/classifier/_autosummary/miml.classifier.mimlTOml.miml_to_ml_classifier.MIMLtoMLClassifier.rst
+-rw-r--r--   0        0        0      511 2020-02-02 00:00:00.000000 mimllearning-1.0.9/docs/source/classifier/_autosummary/miml.classifier.miml_classifier.MIMLClassifier.rst
+-rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 mimllearning-1.0.9/docs/source/data/bag.rst
+-rw-r--r--   0        0        0      149 2020-02-02 00:00:00.000000 mimllearning-1.0.9/docs/source/data/dataset_utils.rst
+-rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 mimllearning-1.0.9/docs/source/data/index.rst
+-rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 mimllearning-1.0.9/docs/source/data/instance.rst
+-rw-r--r--   0        0        0      154 2020-02-02 00:00:00.000000 mimllearning-1.0.9/docs/source/data/miml_dataset.rst
+-rw-r--r--   0        0        0      724 2020-02-02 00:00:00.000000 mimllearning-1.0.9/docs/source/data/_autosummary/miml.data.bag.Bag.rst
+-rw-r--r--   0        0        0      199 2020-02-02 00:00:00.000000 mimllearning-1.0.9/docs/source/data/_autosummary/miml.data.instance.Instance.rst
+-rw-r--r--   0        0        0     1507 2020-02-02 00:00:00.000000 mimllearning-1.0.9/docs/source/data/_autosummary/miml.data.miml_dataset.MIMLDataset.rst
+-rw-r--r--   0        0        0       62 2020-02-02 00:00:00.000000 mimllearning-1.0.9/docs/source/report/index.rst
+-rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 mimllearning-1.0.9/docs/source/report/report.rst
+-rw-r--r--   0        0        0      392 2020-02-02 00:00:00.000000 mimllearning-1.0.9/docs/source/report/_autosummary/miml.report.report.Report.rst
+-rw-r--r--   0        0        0       88 2020-02-02 00:00:00.000000 mimllearning-1.0.9/docs/source/transformation/index.rst
+-rw-r--r--   0        0        0      280 2020-02-02 00:00:00.000000 mimllearning-1.0.9/docs/source/transformation/mimlTOmi.rst
+-rw-r--r--   0        0        0      373 2020-02-02 00:00:00.000000 mimllearning-1.0.9/docs/source/transformation/mimlTOml.rst
+-rw-r--r--   0        0        0      574 2020-02-02 00:00:00.000000 mimllearning-1.0.9/docs/source/transformation/_autosummary/miml.transformation.mimlTOmi.binary_relevance_transformation.BinaryRelevanceTransformation.rst
+-rw-r--r--   0        0        0      656 2020-02-02 00:00:00.000000 mimllearning-1.0.9/docs/source/transformation/_autosummary/miml.transformation.mimlTOmi.label_powerset_transformation.LabelPowersetTransformation.rst
+-rw-r--r--   0        0        0      477 2020-02-02 00:00:00.000000 mimllearning-1.0.9/docs/source/transformation/_autosummary/miml.transformation.mimlTOml.arithmetic.ArithmeticTransformation.rst
+-rw-r--r--   0        0        0      468 2020-02-02 00:00:00.000000 mimllearning-1.0.9/docs/source/transformation/_autosummary/miml.transformation.mimlTOml.geometric.GeometricTransformation.rst
+-rw-r--r--   0        0        0      516 2020-02-02 00:00:00.000000 mimllearning-1.0.9/docs/source/transformation/_autosummary/miml.transformation.mimlTOml.miml_to_ml_transformation.MIMLtoMLTransformation.rst
+-rw-r--r--   0        0        0      441 2020-02-02 00:00:00.000000 mimllearning-1.0.9/docs/source/transformation/_autosummary/miml.transformation.mimlTOml.minmax.MinMaxTransformation.rst
+-rw-r--r--   0        0        0   258069 2020-02-02 00:00:00.000000 mimllearning-1.0.9/documentation/AnteproyectoDamianTFG.pdf
+-rw-r--r--   0        0        0      137 2020-02-02 00:00:00.000000 mimllearning-1.0.9/src/miml/__init__.py
+-rw-r--r--   0        0        0      145 2020-02-02 00:00:00.000000 mimllearning-1.0.9/src/miml/classifier/__init__.py
+-rw-r--r--   0        0        0     3230 2020-02-02 00:00:00.000000 mimllearning-1.0.9/src/miml/classifier/miml_classifier.py
+-rw-r--r--   0        0        0       99 2020-02-02 00:00:00.000000 mimllearning-1.0.9/src/miml/classifier/mi/__init__.py
+-rw-r--r--   0        0        0     3233 2020-02-02 00:00:00.000000 mimllearning-1.0.9/src/miml/classifier/mi/apr_classifier.py
+-rw-r--r--   0        0        0     3847 2020-02-02 00:00:00.000000 mimllearning-1.0.9/src/miml/classifier/mi/mi_wrapper_classifier.py
+-rw-r--r--   0        0        0      175 2020-02-02 00:00:00.000000 mimllearning-1.0.9/src/miml/classifier/mimlTOmi/__init__.py
+-rw-r--r--   0        0        0     3083 2020-02-02 00:00:00.000000 mimllearning-1.0.9/src/miml/classifier/mimlTOmi/miml_to_mi_br_classifier.py
+-rw-r--r--   0        0        0     3139 2020-02-02 00:00:00.000000 mimllearning-1.0.9/src/miml/classifier/mimlTOmi/miml_to_mi_classifier.py
+-rw-r--r--   0        0        0     2980 2020-02-02 00:00:00.000000 mimllearning-1.0.9/src/miml/classifier/mimlTOmi/miml_to_mi_lp_classifier.py
+-rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 mimllearning-1.0.9/src/miml/classifier/mimlTOml/__init__.py
+-rw-r--r--   0        0        0     4211 2020-02-02 00:00:00.000000 mimllearning-1.0.9/src/miml/classifier/mimlTOml/miml_to_ml_classifier.py
+-rw-r--r--   0        0        0      134 2020-02-02 00:00:00.000000 mimllearning-1.0.9/src/miml/data/__init__.py
+-rw-r--r--   0        0        0    10742 2020-02-02 00:00:00.000000 mimllearning-1.0.9/src/miml/data/bag.py
+-rw-r--r--   0        0        0     6624 2020-02-02 00:00:00.000000 mimllearning-1.0.9/src/miml/data/dataset_utils.py
+-rw-r--r--   0        0        0     6845 2020-02-02 00:00:00.000000 mimllearning-1.0.9/src/miml/data/instance.py
+-rw-r--r--   0        0        0    27336 2020-02-02 00:00:00.000000 mimllearning-1.0.9/src/miml/data/miml_dataset.py
+-rw-r--r--   0        0        0   735908 2020-02-02 00:00:00.000000 mimllearning-1.0.9/src/miml/datasets/miml_birds.arff
+-rw-r--r--   0        0        0   842801 2020-02-02 00:00:00.000000 mimllearning-1.0.9/src/miml/datasets/miml_birds.csv
+-rw-r--r--   0        0        0   134841 2020-02-02 00:00:00.000000 mimllearning-1.0.9/src/miml/datasets/miml_birds_random_20test.arff
+-rw-r--r--   0        0        0   498562 2020-02-02 00:00:00.000000 mimllearning-1.0.9/src/miml/datasets/miml_birds_random_80train.arff
+-rw-r--r--   0        0        0      377 2020-02-02 00:00:00.000000 mimllearning-1.0.9/src/miml/datasets/toy.arff
+-rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 mimllearning-1.0.9/src/miml/report/__init__.py
+-rw-r--r--   0        0        0     9612 2020-02-02 00:00:00.000000 mimllearning-1.0.9/src/miml/report/report.py
+-rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 mimllearning-1.0.9/src/miml/transformation/__init__.py
+-rw-r--r--   0        0        0      148 2020-02-02 00:00:00.000000 mimllearning-1.0.9/src/miml/transformation/mimlTOmi/__init__.py
+-rw-r--r--   0        0        0     2414 2020-02-02 00:00:00.000000 mimllearning-1.0.9/src/miml/transformation/mimlTOmi/binary_relevance_transformation.py
+-rw-r--r--   0        0        0     3470 2020-02-02 00:00:00.000000 mimllearning-1.0.9/src/miml/transformation/mimlTOmi/label_powerset_transformation.py
+-rw-r--r--   0        0        0      203 2020-02-02 00:00:00.000000 mimllearning-1.0.9/src/miml/transformation/mimlTOml/__init__.py
+-rw-r--r--   0        0        0     2652 2020-02-02 00:00:00.000000 mimllearning-1.0.9/src/miml/transformation/mimlTOml/arithmetic.py
+-rw-r--r--   0        0        0     2757 2020-02-02 00:00:00.000000 mimllearning-1.0.9/src/miml/transformation/mimlTOml/geometric.py
+-rw-r--r--   0        0        0      472 2020-02-02 00:00:00.000000 mimllearning-1.0.9/src/miml/transformation/mimlTOml/miml_to_ml_transformation.py
+-rw-r--r--   0        0        0     3041 2020-02-02 00:00:00.000000 mimllearning-1.0.9/src/miml/transformation/mimlTOml/minmax.py
+-rw-r--r--   0        0        0   140069 2020-02-02 00:00:00.000000 mimllearning-1.0.9/src/miml/tutorial/classifiers_comparison_experiment_miml.ipynb
+-rw-r--r--   0        0        0     6180 2020-02-02 00:00:00.000000 mimllearning-1.0.9/src/miml/tutorial/classifiers_mimltomi.ipynb
+-rw-r--r--   0        0        0    16103 2020-02-02 00:00:00.000000 mimllearning-1.0.9/src/miml/tutorial/classifiers_mimltoml.ipynb
+-rw-r--r--   0        0        0   172650 2020-02-02 00:00:00.000000 mimllearning-1.0.9/src/miml/tutorial/data_miml.ipynb
+-rw-r--r--   0        0        0     6592 2020-02-02 00:00:00.000000 mimllearning-1.0.9/src/miml/tutorial/train_test_experiment_miml.ipynb
+-rw-r--r--   0        0        0    14927 2020-02-02 00:00:00.000000 mimllearning-1.0.9/src/miml/tutorial/transformations_miml.ipynb
+-rw-r--r--   0        0        0      328 2020-02-02 00:00:00.000000 mimllearning-1.0.9/.gitignore
+-rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 mimllearning-1.0.9/LICENSE.txt
+-rw-r--r--   0        0        0     1839 2020-02-02 00:00:00.000000 mimllearning-1.0.9/README.md
+-rw-r--r--   0        0        0      831 2020-02-02 00:00:00.000000 mimllearning-1.0.9/pyproject.toml
+-rw-r--r--   0        0        0     2356 2020-02-02 00:00:00.000000 mimllearning-1.0.9/PKG-INFO
```

### Comparing `mimllearning-1.0.8/readme.md` & `mimllearning-1.0.9/readme.md`

 * *Files identical despite different names*

### Comparing `mimllearning-1.0.8/.github/workflows/static.yml` & `mimllearning-1.0.9/.github/workflows/static.yml`

 * *Files identical despite different names*

### Comparing `mimllearning-1.0.8/docs/Makefile` & `mimllearning-1.0.9/docs/Makefile`

 * *Files identical despite different names*

### Comparing `mimllearning-1.0.8/docs/make.bat` & `mimllearning-1.0.9/docs/make.bat`

 * *Files identical despite different names*

### Comparing `mimllearning-1.0.8/docs/build/doctrees/environment.pickle` & `mimllearning-1.0.9/docs/build/doctrees/environment.pickle`

 * *Files identical despite different names*

### Comparing `mimllearning-1.0.8/docs/build/doctrees/miml.doctree` & `mimllearning-1.0.9/docs/build/doctrees/miml.doctree`

 * *Files identical despite different names*

### Comparing `mimllearning-1.0.8/docs/build/doctrees/classifier/index.doctree` & `mimllearning-1.0.9/docs/build/doctrees/classifier/index.doctree`

 * *Files identical despite different names*

### Comparing `mimllearning-1.0.8/docs/build/doctrees/classifier/mi.doctree` & `mimllearning-1.0.9/docs/build/doctrees/classifier/mi.doctree`

 * *Files identical despite different names*

### Comparing `mimllearning-1.0.8/docs/build/doctrees/classifier/mimlTOmi.doctree` & `mimllearning-1.0.9/docs/build/doctrees/classifier/mimlTOmi.doctree`

 * *Files identical despite different names*

### Comparing `mimllearning-1.0.8/docs/build/doctrees/classifier/mimlTOml.doctree` & `mimllearning-1.0.9/docs/build/doctrees/classifier/mimlTOml.doctree`

 * *Files identical despite different names*

### Comparing `mimllearning-1.0.8/docs/build/doctrees/classifier/miml_classifier.doctree` & `mimllearning-1.0.9/docs/build/doctrees/classifier/miml_classifier.doctree`

 * *Files identical despite different names*

### Comparing `mimllearning-1.0.8/docs/build/doctrees/classifier/_autosummary/miml.classifier.mi.apr_classifier.APRClassifier.doctree` & `mimllearning-1.0.9/docs/build/doctrees/classifier/_autosummary/miml.classifier.mi.apr_classifier.APRClassifier.doctree`

 * *Files identical despite different names*

### Comparing `mimllearning-1.0.8/docs/build/doctrees/classifier/_autosummary/miml.classifier.mi.mi_wrapper_classifier.MIWrapperClassifier.doctree` & `mimllearning-1.0.9/docs/build/doctrees/classifier/_autosummary/miml.classifier.mi.mi_wrapper_classifier.MIWrapperClassifier.doctree`

 * *Files identical despite different names*

### Comparing `mimllearning-1.0.8/docs/build/doctrees/classifier/_autosummary/miml.classifier.mimlTOmi.miml_to_mi_br_classifier.MIMLtoMIBRClassifier.doctree` & `mimllearning-1.0.9/docs/build/doctrees/classifier/_autosummary/miml.classifier.mimlTOmi.miml_to_mi_br_classifier.MIMLtoMIBRClassifier.doctree`

 * *Files identical despite different names*

### Comparing `mimllearning-1.0.8/docs/build/doctrees/classifier/_autosummary/miml.classifier.mimlTOmi.miml_to_mi_classifier.MIMLtoMIClassifier.doctree` & `mimllearning-1.0.9/docs/build/doctrees/classifier/_autosummary/miml.classifier.mimlTOmi.miml_to_mi_classifier.MIMLtoMIClassifier.doctree`

 * *Files identical despite different names*

### Comparing `mimllearning-1.0.8/docs/build/doctrees/classifier/_autosummary/miml.classifier.mimlTOmi.miml_to_mi_lp_classifier.MIMLtoMILPClassifier.doctree` & `mimllearning-1.0.9/docs/build/doctrees/classifier/_autosummary/miml.classifier.mimlTOmi.miml_to_mi_lp_classifier.MIMLtoMILPClassifier.doctree`

 * *Files identical despite different names*

### Comparing `mimllearning-1.0.8/docs/build/doctrees/classifier/_autosummary/miml.classifier.mimlTOml.miml_to_ml_classifier.MIMLtoMLClassifier.doctree` & `mimllearning-1.0.9/docs/build/doctrees/classifier/_autosummary/miml.classifier.mimlTOml.miml_to_ml_classifier.MIMLtoMLClassifier.doctree`

 * *Files identical despite different names*

### Comparing `mimllearning-1.0.8/docs/build/doctrees/classifier/_autosummary/miml.classifier.miml_classifier.MIMLClassifier.doctree` & `mimllearning-1.0.9/docs/build/doctrees/classifier/_autosummary/miml.classifier.miml_classifier.MIMLClassifier.doctree`

 * *Files identical despite different names*

### Comparing `mimllearning-1.0.8/docs/build/doctrees/data/bag.doctree` & `mimllearning-1.0.9/docs/build/doctrees/data/bag.doctree`

 * *Files identical despite different names*

### Comparing `mimllearning-1.0.8/docs/build/doctrees/data/dataset_utils.doctree` & `mimllearning-1.0.9/docs/build/doctrees/data/dataset_utils.doctree`

 * *Files identical despite different names*

### Comparing `mimllearning-1.0.8/docs/build/doctrees/data/index.doctree` & `mimllearning-1.0.9/docs/build/doctrees/data/index.doctree`

 * *Files identical despite different names*

### Comparing `mimllearning-1.0.8/docs/build/doctrees/data/instance.doctree` & `mimllearning-1.0.9/docs/build/doctrees/data/instance.doctree`

 * *Files identical despite different names*

### Comparing `mimllearning-1.0.8/docs/build/doctrees/data/miml_dataset.doctree` & `mimllearning-1.0.9/docs/build/doctrees/data/miml_dataset.doctree`

 * *Files identical despite different names*

### Comparing `mimllearning-1.0.8/docs/build/doctrees/data/_autosummary/miml.data.bag.Bag.doctree` & `mimllearning-1.0.9/docs/build/doctrees/data/_autosummary/miml.data.bag.Bag.doctree`

 * *Files identical despite different names*

### Comparing `mimllearning-1.0.8/docs/build/doctrees/data/_autosummary/miml.data.instance.Instance.doctree` & `mimllearning-1.0.9/docs/build/doctrees/data/_autosummary/miml.data.instance.Instance.doctree`

 * *Files identical despite different names*

### Comparing `mimllearning-1.0.8/docs/build/doctrees/data/_autosummary/miml.data.miml_dataset.MIMLDataset.doctree` & `mimllearning-1.0.9/docs/build/doctrees/data/_autosummary/miml.data.miml_dataset.MIMLDataset.doctree`

 * *Files identical despite different names*

### Comparing `mimllearning-1.0.8/docs/build/doctrees/report/index.doctree` & `mimllearning-1.0.9/docs/build/doctrees/report/index.doctree`

 * *Files identical despite different names*

### Comparing `mimllearning-1.0.8/docs/build/doctrees/report/report.doctree` & `mimllearning-1.0.9/docs/build/doctrees/report/report.doctree`

 * *Files identical despite different names*

### Comparing `mimllearning-1.0.8/docs/build/doctrees/report/_autosummary/miml.report.report.Report.doctree` & `mimllearning-1.0.9/docs/build/doctrees/report/_autosummary/miml.report.report.Report.doctree`

 * *Files identical despite different names*

### Comparing `mimllearning-1.0.8/docs/build/doctrees/transformation/index.doctree` & `mimllearning-1.0.9/docs/build/doctrees/transformation/index.doctree`

 * *Files identical despite different names*

### Comparing `mimllearning-1.0.8/docs/build/doctrees/transformation/mimlTOmi.doctree` & `mimllearning-1.0.9/docs/build/doctrees/transformation/mimlTOmi.doctree`

 * *Files identical despite different names*

### Comparing `mimllearning-1.0.8/docs/build/doctrees/transformation/mimlTOml.doctree` & `mimllearning-1.0.9/docs/build/doctrees/transformation/mimlTOml.doctree`

 * *Files identical despite different names*

### Comparing `mimllearning-1.0.8/docs/build/doctrees/transformation/_autosummary/miml.transformation.mimlTOmi.binary_relevance_transformation.BinaryRelevanceTransformation.doctree` & `mimllearning-1.0.9/docs/build/doctrees/transformation/_autosummary/miml.transformation.mimlTOmi.binary_relevance_transformation.BinaryRelevanceTransformation.doctree`

 * *Files identical despite different names*

### Comparing `mimllearning-1.0.8/docs/build/doctrees/transformation/_autosummary/miml.transformation.mimlTOmi.label_powerset_transformation.LabelPowersetTransformation.doctree` & `mimllearning-1.0.9/docs/build/doctrees/transformation/_autosummary/miml.transformation.mimlTOmi.label_powerset_transformation.LabelPowersetTransformation.doctree`

 * *Files identical despite different names*

### Comparing `mimllearning-1.0.8/docs/build/doctrees/transformation/_autosummary/miml.transformation.mimlTOml.arithmetic.ArithmeticTransformation.doctree` & `mimllearning-1.0.9/docs/build/doctrees/transformation/_autosummary/miml.transformation.mimlTOml.arithmetic.ArithmeticTransformation.doctree`

 * *Files identical despite different names*

### Comparing `mimllearning-1.0.8/docs/build/doctrees/transformation/_autosummary/miml.transformation.mimlTOml.geometric.GeometricTransformation.doctree` & `mimllearning-1.0.9/docs/build/doctrees/transformation/_autosummary/miml.transformation.mimlTOml.geometric.GeometricTransformation.doctree`

 * *Files identical despite different names*

### Comparing `mimllearning-1.0.8/docs/build/doctrees/transformation/_autosummary/miml.transformation.mimlTOml.miml_to_ml_transformation.MIMLtoMLTransformation.doctree` & `mimllearning-1.0.9/docs/build/doctrees/transformation/_autosummary/miml.transformation.mimlTOml.miml_to_ml_transformation.MIMLtoMLTransformation.doctree`

 * *Files identical despite different names*

### Comparing `mimllearning-1.0.8/docs/build/doctrees/transformation/_autosummary/miml.transformation.mimlTOml.minmax.MinMaxTransformation.doctree` & `mimllearning-1.0.9/docs/build/doctrees/transformation/_autosummary/miml.transformation.mimlTOml.minmax.MinMaxTransformation.doctree`

 * *Files identical despite different names*

### Comparing `mimllearning-1.0.8/docs/build/html/genindex.html` & `mimllearning-1.0.9/docs/build/html/genindex.html`

 * *Files identical despite different names*

### Comparing `mimllearning-1.0.8/docs/build/html/index.html` & `mimllearning-1.0.9/docs/build/html/index.html`

 * *Files identical despite different names*

### Comparing `mimllearning-1.0.8/docs/build/html/objects.inv` & `mimllearning-1.0.9/docs/build/html/objects.inv`

 * *Files identical despite different names*

### Comparing `mimllearning-1.0.8/docs/build/html/search.html` & `mimllearning-1.0.9/docs/build/html/search.html`

 * *Files identical despite different names*

### Comparing `mimllearning-1.0.8/docs/build/html/searchindex.js` & `mimllearning-1.0.9/docs/build/html/searchindex.js`

 * *Files identical despite different names*

### Comparing `mimllearning-1.0.8/docs/build/html/_sources/classifier/_autosummary/miml.classifier.mimlTOmi.miml_to_mi_br_classifier.MIMLtoMIBRClassifier.rst` & `mimllearning-1.0.9/docs/build/html/_sources/classifier/_autosummary/miml.classifier.mimlTOmi.miml_to_mi_br_classifier.MIMLtoMIBRClassifier.rst`

 * *Files identical despite different names*

### Comparing `mimllearning-1.0.8/docs/build/html/_sources/classifier/_autosummary/miml.classifier.mimlTOmi.miml_to_mi_classifier.MIMLtoMIClassifier.rst` & `mimllearning-1.0.9/docs/build/html/_sources/classifier/_autosummary/miml.classifier.mimlTOmi.miml_to_mi_classifier.MIMLtoMIClassifier.rst`

 * *Files identical despite different names*

### Comparing `mimllearning-1.0.8/docs/build/html/_sources/classifier/_autosummary/miml.classifier.mimlTOmi.miml_to_mi_lp_classifier.MIMLtoMILPClassifier.rst` & `mimllearning-1.0.9/docs/build/html/_sources/classifier/_autosummary/miml.classifier.mimlTOmi.miml_to_mi_lp_classifier.MIMLtoMILPClassifier.rst`

 * *Files identical despite different names*

### Comparing `mimllearning-1.0.8/docs/build/html/_sources/classifier/_autosummary/miml.classifier.mimlTOml.miml_to_ml_classifier.MIMLtoMLClassifier.rst` & `mimllearning-1.0.9/docs/build/html/_sources/classifier/_autosummary/miml.classifier.mimlTOml.miml_to_ml_classifier.MIMLtoMLClassifier.rst`

 * *Files identical despite different names*

### Comparing `mimllearning-1.0.8/docs/build/html/_sources/data/_autosummary/miml.data.bag.Bag.rst` & `mimllearning-1.0.9/docs/build/html/_sources/data/_autosummary/miml.data.bag.Bag.rst`

 * *Files identical despite different names*

### Comparing `mimllearning-1.0.8/docs/build/html/_sources/data/_autosummary/miml.data.miml_dataset.MIMLDataset.rst` & `mimllearning-1.0.9/docs/build/html/_sources/data/_autosummary/miml.data.miml_dataset.MIMLDataset.rst`

 * *Files identical despite different names*

### Comparing `mimllearning-1.0.8/docs/build/html/_sources/transformation/_autosummary/miml.transformation.mimlTOmi.binary_relevance_transformation.BinaryRelevanceTransformation.rst` & `mimllearning-1.0.9/docs/build/html/_sources/transformation/_autosummary/miml.transformation.mimlTOmi.binary_relevance_transformation.BinaryRelevanceTransformation.rst`

 * *Files identical despite different names*

### Comparing `mimllearning-1.0.8/docs/build/html/_sources/transformation/_autosummary/miml.transformation.mimlTOmi.label_powerset_transformation.LabelPowersetTransformation.rst` & `mimllearning-1.0.9/docs/build/html/_sources/transformation/_autosummary/miml.transformation.mimlTOmi.label_powerset_transformation.LabelPowersetTransformation.rst`

 * *Files identical despite different names*

### Comparing `mimllearning-1.0.8/docs/build/html/_sources/transformation/_autosummary/miml.transformation.mimlTOml.miml_to_ml_transformation.MIMLtoMLTransformation.rst` & `mimllearning-1.0.9/docs/build/html/_sources/transformation/_autosummary/miml.transformation.mimlTOml.miml_to_ml_transformation.MIMLtoMLTransformation.rst`

 * *Files identical despite different names*

### Comparing `mimllearning-1.0.8/docs/build/html/_static/basic.css` & `mimllearning-1.0.9/docs/build/html/_static/basic.css`

 * *Files identical despite different names*

### Comparing `mimllearning-1.0.8/docs/build/html/_static/doctools.js` & `mimllearning-1.0.9/docs/build/html/_static/doctools.js`

 * *Files identical despite different names*

### Comparing `mimllearning-1.0.8/docs/build/html/_static/language_data.js` & `mimllearning-1.0.9/docs/build/html/_static/language_data.js`

 * *Files identical despite different names*

### Comparing `mimllearning-1.0.8/docs/build/html/_static/pygments.css` & `mimllearning-1.0.9/docs/build/html/_static/pygments.css`

 * *Files identical despite different names*

### Comparing `mimllearning-1.0.8/docs/build/html/_static/searchtools.js` & `mimllearning-1.0.9/docs/build/html/_static/searchtools.js`

 * *Files identical despite different names*

### Comparing `mimllearning-1.0.8/docs/build/html/_static/sphinx_highlight.js` & `mimllearning-1.0.9/docs/build/html/_static/sphinx_highlight.js`

 * *Files identical despite different names*

### Comparing `mimllearning-1.0.8/docs/build/html/_static/webpack-macros.html` & `mimllearning-1.0.9/docs/build/html/_static/webpack-macros.html`

 * *Files identical despite different names*

### Comparing `mimllearning-1.0.8/docs/build/html/_static/images/logo_binder.svg` & `mimllearning-1.0.9/docs/build/html/_static/images/logo_binder.svg`

 * *Files identical despite different names*

### Comparing `mimllearning-1.0.8/docs/build/html/_static/images/logo_colab.png` & `mimllearning-1.0.9/docs/build/html/_static/images/logo_colab.png`

 * *Files identical despite different names*

### Comparing `mimllearning-1.0.8/docs/build/html/_static/images/logo_deepnote.svg` & `mimllearning-1.0.9/docs/build/html/_static/images/logo_deepnote.svg`

 * *Files identical despite different names*

### Comparing `mimllearning-1.0.8/docs/build/html/_static/images/logo_jupyterhub.svg` & `mimllearning-1.0.9/docs/build/html/_static/images/logo_jupyterhub.svg`

 * *Files identical despite different names*

### Comparing `mimllearning-1.0.8/docs/build/html/_static/locales/ar/LC_MESSAGES/booktheme.mo` & `mimllearning-1.0.9/docs/build/html/_static/locales/ar/LC_MESSAGES/booktheme.mo`

 * *Files identical despite different names*

### Comparing `mimllearning-1.0.8/docs/build/html/_static/locales/ar/LC_MESSAGES/booktheme.po` & `mimllearning-1.0.9/docs/build/html/_static/locales/ar/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `mimllearning-1.0.8/docs/build/html/_static/locales/bg/LC_MESSAGES/booktheme.mo` & `mimllearning-1.0.9/docs/build/html/_static/locales/bg/LC_MESSAGES/booktheme.mo`

 * *Files identical despite different names*

### Comparing `mimllearning-1.0.8/docs/build/html/_static/locales/bg/LC_MESSAGES/booktheme.po` & `mimllearning-1.0.9/docs/build/html/_static/locales/bg/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `mimllearning-1.0.8/docs/build/html/_static/locales/bn/LC_MESSAGES/booktheme.mo` & `mimllearning-1.0.9/docs/build/html/_static/locales/bn/LC_MESSAGES/booktheme.mo`

 * *Files identical despite different names*

### Comparing `mimllearning-1.0.8/docs/build/html/_static/locales/bn/LC_MESSAGES/booktheme.po` & `mimllearning-1.0.9/docs/build/html/_static/locales/bn/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `mimllearning-1.0.8/docs/build/html/_static/locales/ca/LC_MESSAGES/booktheme.mo` & `mimllearning-1.0.9/docs/build/html/_static/locales/ca/LC_MESSAGES/booktheme.mo`

 * *Files identical despite different names*

### Comparing `mimllearning-1.0.8/docs/build/html/_static/locales/ca/LC_MESSAGES/booktheme.po` & `mimllearning-1.0.9/docs/build/html/_static/locales/ca/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `mimllearning-1.0.8/docs/build/html/_static/locales/cs/LC_MESSAGES/booktheme.mo` & `mimllearning-1.0.9/docs/build/html/_static/locales/cs/LC_MESSAGES/booktheme.mo`

 * *Files identical despite different names*

### Comparing `mimllearning-1.0.8/docs/build/html/_static/locales/cs/LC_MESSAGES/booktheme.po` & `mimllearning-1.0.9/docs/build/html/_static/locales/cs/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `mimllearning-1.0.8/docs/build/html/_static/locales/da/LC_MESSAGES/booktheme.mo` & `mimllearning-1.0.9/docs/build/html/_static/locales/da/LC_MESSAGES/booktheme.mo`

 * *Files identical despite different names*

### Comparing `mimllearning-1.0.8/docs/build/html/_static/locales/da/LC_MESSAGES/booktheme.po` & `mimllearning-1.0.9/docs/build/html/_static/locales/da/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `mimllearning-1.0.8/docs/build/html/_static/locales/de/LC_MESSAGES/booktheme.mo` & `mimllearning-1.0.9/docs/build/html/_static/locales/de/LC_MESSAGES/booktheme.mo`

 * *Files identical despite different names*

### Comparing `mimllearning-1.0.8/docs/build/html/_static/locales/de/LC_MESSAGES/booktheme.po` & `mimllearning-1.0.9/docs/build/html/_static/locales/de/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `mimllearning-1.0.8/docs/build/html/_static/locales/el/LC_MESSAGES/booktheme.mo` & `mimllearning-1.0.9/docs/build/html/_static/locales/el/LC_MESSAGES/booktheme.mo`

 * *Files identical despite different names*

### Comparing `mimllearning-1.0.8/docs/build/html/_static/locales/el/LC_MESSAGES/booktheme.po` & `mimllearning-1.0.9/docs/build/html/_static/locales/el/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `mimllearning-1.0.8/docs/build/html/_static/locales/eo/LC_MESSAGES/booktheme.mo` & `mimllearning-1.0.9/docs/build/html/_static/locales/eo/LC_MESSAGES/booktheme.mo`

 * *Files identical despite different names*

### Comparing `mimllearning-1.0.8/docs/build/html/_static/locales/eo/LC_MESSAGES/booktheme.po` & `mimllearning-1.0.9/docs/build/html/_static/locales/eo/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `mimllearning-1.0.8/docs/build/html/_static/locales/es/LC_MESSAGES/booktheme.mo` & `mimllearning-1.0.9/docs/build/html/_static/locales/es/LC_MESSAGES/booktheme.mo`

 * *Files identical despite different names*

### Comparing `mimllearning-1.0.8/docs/build/html/_static/locales/es/LC_MESSAGES/booktheme.po` & `mimllearning-1.0.9/docs/build/html/_static/locales/es/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `mimllearning-1.0.8/docs/build/html/_static/locales/et/LC_MESSAGES/booktheme.mo` & `mimllearning-1.0.9/docs/build/html/_static/locales/et/LC_MESSAGES/booktheme.mo`

 * *Files identical despite different names*

### Comparing `mimllearning-1.0.8/docs/build/html/_static/locales/et/LC_MESSAGES/booktheme.po` & `mimllearning-1.0.9/docs/build/html/_static/locales/et/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `mimllearning-1.0.8/docs/build/html/_static/locales/fi/LC_MESSAGES/booktheme.mo` & `mimllearning-1.0.9/docs/build/html/_static/locales/fi/LC_MESSAGES/booktheme.mo`

 * *Files identical despite different names*

### Comparing `mimllearning-1.0.8/docs/build/html/_static/locales/fi/LC_MESSAGES/booktheme.po` & `mimllearning-1.0.9/docs/build/html/_static/locales/fi/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `mimllearning-1.0.8/docs/build/html/_static/locales/fr/LC_MESSAGES/booktheme.mo` & `mimllearning-1.0.9/docs/build/html/_static/locales/fr/LC_MESSAGES/booktheme.mo`

 * *Files identical despite different names*

### Comparing `mimllearning-1.0.8/docs/build/html/_static/locales/fr/LC_MESSAGES/booktheme.po` & `mimllearning-1.0.9/docs/build/html/_static/locales/fr/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `mimllearning-1.0.8/docs/build/html/_static/locales/hr/LC_MESSAGES/booktheme.mo` & `mimllearning-1.0.9/docs/build/html/_static/locales/hr/LC_MESSAGES/booktheme.mo`

 * *Files identical despite different names*

### Comparing `mimllearning-1.0.8/docs/build/html/_static/locales/hr/LC_MESSAGES/booktheme.po` & `mimllearning-1.0.9/docs/build/html/_static/locales/hr/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `mimllearning-1.0.8/docs/build/html/_static/locales/id/LC_MESSAGES/booktheme.mo` & `mimllearning-1.0.9/docs/build/html/_static/locales/id/LC_MESSAGES/booktheme.mo`

 * *Files identical despite different names*

### Comparing `mimllearning-1.0.8/docs/build/html/_static/locales/id/LC_MESSAGES/booktheme.po` & `mimllearning-1.0.9/docs/build/html/_static/locales/id/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `mimllearning-1.0.8/docs/build/html/_static/locales/it/LC_MESSAGES/booktheme.mo` & `mimllearning-1.0.9/docs/build/html/_static/locales/it/LC_MESSAGES/booktheme.mo`

 * *Files identical despite different names*

### Comparing `mimllearning-1.0.8/docs/build/html/_static/locales/it/LC_MESSAGES/booktheme.po` & `mimllearning-1.0.9/docs/build/html/_static/locales/it/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `mimllearning-1.0.8/docs/build/html/_static/locales/iw/LC_MESSAGES/booktheme.mo` & `mimllearning-1.0.9/docs/build/html/_static/locales/iw/LC_MESSAGES/booktheme.mo`

 * *Files identical despite different names*

### Comparing `mimllearning-1.0.8/docs/build/html/_static/locales/iw/LC_MESSAGES/booktheme.po` & `mimllearning-1.0.9/docs/build/html/_static/locales/iw/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `mimllearning-1.0.8/docs/build/html/_static/locales/ja/LC_MESSAGES/booktheme.mo` & `mimllearning-1.0.9/docs/build/html/_static/locales/ja/LC_MESSAGES/booktheme.mo`

 * *Files identical despite different names*

### Comparing `mimllearning-1.0.8/docs/build/html/_static/locales/ja/LC_MESSAGES/booktheme.po` & `mimllearning-1.0.9/docs/build/html/_static/locales/ja/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `mimllearning-1.0.8/docs/build/html/_static/locales/ko/LC_MESSAGES/booktheme.mo` & `mimllearning-1.0.9/docs/build/html/_static/locales/ko/LC_MESSAGES/booktheme.mo`

 * *Files identical despite different names*

### Comparing `mimllearning-1.0.8/docs/build/html/_static/locales/ko/LC_MESSAGES/booktheme.po` & `mimllearning-1.0.9/docs/build/html/_static/locales/ko/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `mimllearning-1.0.8/docs/build/html/_static/locales/lt/LC_MESSAGES/booktheme.mo` & `mimllearning-1.0.9/docs/build/html/_static/locales/lt/LC_MESSAGES/booktheme.mo`

 * *Files identical despite different names*

### Comparing `mimllearning-1.0.8/docs/build/html/_static/locales/lt/LC_MESSAGES/booktheme.po` & `mimllearning-1.0.9/docs/build/html/_static/locales/lt/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `mimllearning-1.0.8/docs/build/html/_static/locales/lv/LC_MESSAGES/booktheme.mo` & `mimllearning-1.0.9/docs/build/html/_static/locales/lv/LC_MESSAGES/booktheme.mo`

 * *Files identical despite different names*

### Comparing `mimllearning-1.0.8/docs/build/html/_static/locales/lv/LC_MESSAGES/booktheme.po` & `mimllearning-1.0.9/docs/build/html/_static/locales/lv/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `mimllearning-1.0.8/docs/build/html/_static/locales/ml/LC_MESSAGES/booktheme.mo` & `mimllearning-1.0.9/docs/build/html/_static/locales/ml/LC_MESSAGES/booktheme.mo`

 * *Files identical despite different names*

### Comparing `mimllearning-1.0.8/docs/build/html/_static/locales/ml/LC_MESSAGES/booktheme.po` & `mimllearning-1.0.9/docs/build/html/_static/locales/ml/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `mimllearning-1.0.8/docs/build/html/_static/locales/mr/LC_MESSAGES/booktheme.mo` & `mimllearning-1.0.9/docs/build/html/_static/locales/mr/LC_MESSAGES/booktheme.mo`

 * *Files identical despite different names*

### Comparing `mimllearning-1.0.8/docs/build/html/_static/locales/mr/LC_MESSAGES/booktheme.po` & `mimllearning-1.0.9/docs/build/html/_static/locales/mr/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `mimllearning-1.0.8/docs/build/html/_static/locales/ms/LC_MESSAGES/booktheme.mo` & `mimllearning-1.0.9/docs/build/html/_static/locales/ms/LC_MESSAGES/booktheme.mo`

 * *Files identical despite different names*

### Comparing `mimllearning-1.0.8/docs/build/html/_static/locales/ms/LC_MESSAGES/booktheme.po` & `mimllearning-1.0.9/docs/build/html/_static/locales/ms/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `mimllearning-1.0.8/docs/build/html/_static/locales/nl/LC_MESSAGES/booktheme.mo` & `mimllearning-1.0.9/docs/build/html/_static/locales/nl/LC_MESSAGES/booktheme.mo`

 * *Files identical despite different names*

### Comparing `mimllearning-1.0.8/docs/build/html/_static/locales/nl/LC_MESSAGES/booktheme.po` & `mimllearning-1.0.9/docs/build/html/_static/locales/nl/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `mimllearning-1.0.8/docs/build/html/_static/locales/no/LC_MESSAGES/booktheme.mo` & `mimllearning-1.0.9/docs/build/html/_static/locales/no/LC_MESSAGES/booktheme.mo`

 * *Files identical despite different names*

### Comparing `mimllearning-1.0.8/docs/build/html/_static/locales/no/LC_MESSAGES/booktheme.po` & `mimllearning-1.0.9/docs/build/html/_static/locales/no/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `mimllearning-1.0.8/docs/build/html/_static/locales/pl/LC_MESSAGES/booktheme.mo` & `mimllearning-1.0.9/docs/build/html/_static/locales/pl/LC_MESSAGES/booktheme.mo`

 * *Files identical despite different names*

### Comparing `mimllearning-1.0.8/docs/build/html/_static/locales/pl/LC_MESSAGES/booktheme.po` & `mimllearning-1.0.9/docs/build/html/_static/locales/pl/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `mimllearning-1.0.8/docs/build/html/_static/locales/pt/LC_MESSAGES/booktheme.mo` & `mimllearning-1.0.9/docs/build/html/_static/locales/pt/LC_MESSAGES/booktheme.mo`

 * *Files identical despite different names*

### Comparing `mimllearning-1.0.8/docs/build/html/_static/locales/pt/LC_MESSAGES/booktheme.po` & `mimllearning-1.0.9/docs/build/html/_static/locales/pt/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `mimllearning-1.0.8/docs/build/html/_static/locales/ro/LC_MESSAGES/booktheme.mo` & `mimllearning-1.0.9/docs/build/html/_static/locales/ro/LC_MESSAGES/booktheme.mo`

 * *Files identical despite different names*

### Comparing `mimllearning-1.0.8/docs/build/html/_static/locales/ro/LC_MESSAGES/booktheme.po` & `mimllearning-1.0.9/docs/build/html/_static/locales/ro/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `mimllearning-1.0.8/docs/build/html/_static/locales/ru/LC_MESSAGES/booktheme.mo` & `mimllearning-1.0.9/docs/build/html/_static/locales/ru/LC_MESSAGES/booktheme.mo`

 * *Files identical despite different names*

### Comparing `mimllearning-1.0.8/docs/build/html/_static/locales/ru/LC_MESSAGES/booktheme.po` & `mimllearning-1.0.9/docs/build/html/_static/locales/ru/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `mimllearning-1.0.8/docs/build/html/_static/locales/sk/LC_MESSAGES/booktheme.mo` & `mimllearning-1.0.9/docs/build/html/_static/locales/sk/LC_MESSAGES/booktheme.mo`

 * *Files identical despite different names*

### Comparing `mimllearning-1.0.8/docs/build/html/_static/locales/sk/LC_MESSAGES/booktheme.po` & `mimllearning-1.0.9/docs/build/html/_static/locales/sk/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `mimllearning-1.0.8/docs/build/html/_static/locales/sl/LC_MESSAGES/booktheme.mo` & `mimllearning-1.0.9/docs/build/html/_static/locales/sl/LC_MESSAGES/booktheme.mo`

 * *Files identical despite different names*

### Comparing `mimllearning-1.0.8/docs/build/html/_static/locales/sl/LC_MESSAGES/booktheme.po` & `mimllearning-1.0.9/docs/build/html/_static/locales/sl/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `mimllearning-1.0.8/docs/build/html/_static/locales/sr/LC_MESSAGES/booktheme.mo` & `mimllearning-1.0.9/docs/build/html/_static/locales/sr/LC_MESSAGES/booktheme.mo`

 * *Files identical despite different names*

### Comparing `mimllearning-1.0.8/docs/build/html/_static/locales/sr/LC_MESSAGES/booktheme.po` & `mimllearning-1.0.9/docs/build/html/_static/locales/sr/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `mimllearning-1.0.8/docs/build/html/_static/locales/sv/LC_MESSAGES/booktheme.mo` & `mimllearning-1.0.9/docs/build/html/_static/locales/sv/LC_MESSAGES/booktheme.mo`

 * *Files identical despite different names*

### Comparing `mimllearning-1.0.8/docs/build/html/_static/locales/sv/LC_MESSAGES/booktheme.po` & `mimllearning-1.0.9/docs/build/html/_static/locales/sv/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `mimllearning-1.0.8/docs/build/html/_static/locales/ta/LC_MESSAGES/booktheme.mo` & `mimllearning-1.0.9/docs/build/html/_static/locales/ta/LC_MESSAGES/booktheme.mo`

 * *Files identical despite different names*

### Comparing `mimllearning-1.0.8/docs/build/html/_static/locales/ta/LC_MESSAGES/booktheme.po` & `mimllearning-1.0.9/docs/build/html/_static/locales/ta/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `mimllearning-1.0.8/docs/build/html/_static/locales/te/LC_MESSAGES/booktheme.mo` & `mimllearning-1.0.9/docs/build/html/_static/locales/te/LC_MESSAGES/booktheme.mo`

 * *Files identical despite different names*

### Comparing `mimllearning-1.0.8/docs/build/html/_static/locales/te/LC_MESSAGES/booktheme.po` & `mimllearning-1.0.9/docs/build/html/_static/locales/te/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `mimllearning-1.0.8/docs/build/html/_static/locales/tg/LC_MESSAGES/booktheme.mo` & `mimllearning-1.0.9/docs/build/html/_static/locales/tg/LC_MESSAGES/booktheme.mo`

 * *Files identical despite different names*

### Comparing `mimllearning-1.0.8/docs/build/html/_static/locales/tg/LC_MESSAGES/booktheme.po` & `mimllearning-1.0.9/docs/build/html/_static/locales/tg/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `mimllearning-1.0.8/docs/build/html/_static/locales/th/LC_MESSAGES/booktheme.mo` & `mimllearning-1.0.9/docs/build/html/_static/locales/th/LC_MESSAGES/booktheme.mo`

 * *Files identical despite different names*

### Comparing `mimllearning-1.0.8/docs/build/html/_static/locales/th/LC_MESSAGES/booktheme.po` & `mimllearning-1.0.9/docs/build/html/_static/locales/th/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `mimllearning-1.0.8/docs/build/html/_static/locales/tl/LC_MESSAGES/booktheme.mo` & `mimllearning-1.0.9/docs/build/html/_static/locales/tl/LC_MESSAGES/booktheme.mo`

 * *Files identical despite different names*

### Comparing `mimllearning-1.0.8/docs/build/html/_static/locales/tl/LC_MESSAGES/booktheme.po` & `mimllearning-1.0.9/docs/build/html/_static/locales/tl/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `mimllearning-1.0.8/docs/build/html/_static/locales/tr/LC_MESSAGES/booktheme.mo` & `mimllearning-1.0.9/docs/build/html/_static/locales/tr/LC_MESSAGES/booktheme.mo`

 * *Files identical despite different names*

### Comparing `mimllearning-1.0.8/docs/build/html/_static/locales/tr/LC_MESSAGES/booktheme.po` & `mimllearning-1.0.9/docs/build/html/_static/locales/tr/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `mimllearning-1.0.8/docs/build/html/_static/locales/uk/LC_MESSAGES/booktheme.mo` & `mimllearning-1.0.9/docs/build/html/_static/locales/uk/LC_MESSAGES/booktheme.mo`

 * *Files identical despite different names*

### Comparing `mimllearning-1.0.8/docs/build/html/_static/locales/uk/LC_MESSAGES/booktheme.po` & `mimllearning-1.0.9/docs/build/html/_static/locales/uk/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `mimllearning-1.0.8/docs/build/html/_static/locales/ur/LC_MESSAGES/booktheme.mo` & `mimllearning-1.0.9/docs/build/html/_static/locales/ur/LC_MESSAGES/booktheme.mo`

 * *Files identical despite different names*

### Comparing `mimllearning-1.0.8/docs/build/html/_static/locales/ur/LC_MESSAGES/booktheme.po` & `mimllearning-1.0.9/docs/build/html/_static/locales/ur/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `mimllearning-1.0.8/docs/build/html/_static/locales/vi/LC_MESSAGES/booktheme.mo` & `mimllearning-1.0.9/docs/build/html/_static/locales/vi/LC_MESSAGES/booktheme.mo`

 * *Files identical despite different names*

### Comparing `mimllearning-1.0.8/docs/build/html/_static/locales/vi/LC_MESSAGES/booktheme.po` & `mimllearning-1.0.9/docs/build/html/_static/locales/vi/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `mimllearning-1.0.8/docs/build/html/_static/locales/zh_CN/LC_MESSAGES/booktheme.mo` & `mimllearning-1.0.9/docs/build/html/_static/locales/zh_CN/LC_MESSAGES/booktheme.mo`

 * *Files identical despite different names*

### Comparing `mimllearning-1.0.8/docs/build/html/_static/locales/zh_CN/LC_MESSAGES/booktheme.po` & `mimllearning-1.0.9/docs/build/html/_static/locales/zh_CN/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `mimllearning-1.0.8/docs/build/html/_static/locales/zh_TW/LC_MESSAGES/booktheme.mo` & `mimllearning-1.0.9/docs/build/html/_static/locales/zh_TW/LC_MESSAGES/booktheme.mo`

 * *Files identical despite different names*

### Comparing `mimllearning-1.0.8/docs/build/html/_static/locales/zh_TW/LC_MESSAGES/booktheme.po` & `mimllearning-1.0.9/docs/build/html/_static/locales/zh_TW/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `mimllearning-1.0.8/docs/build/html/_static/scripts/bootstrap.js` & `mimllearning-1.0.9/docs/build/html/_static/scripts/bootstrap.js`

 * *Files identical despite different names*

### Comparing `mimllearning-1.0.8/docs/build/html/_static/scripts/bootstrap.js.map` & `mimllearning-1.0.9/docs/build/html/_static/scripts/bootstrap.js.map`

 * *Files identical despite different names*

### Comparing `mimllearning-1.0.8/docs/build/html/_static/scripts/pydata-sphinx-theme.js` & `mimllearning-1.0.9/docs/build/html/_static/scripts/pydata-sphinx-theme.js`

 * *Files identical despite different names*

### Comparing `mimllearning-1.0.8/docs/build/html/_static/scripts/pydata-sphinx-theme.js.map` & `mimllearning-1.0.9/docs/build/html/_static/scripts/pydata-sphinx-theme.js.map`

 * *Files identical despite different names*

### Comparing `mimllearning-1.0.8/docs/build/html/_static/scripts/sphinx-book-theme.js` & `mimllearning-1.0.9/docs/build/html/_static/scripts/sphinx-book-theme.js`

 * *Files identical despite different names*

### Comparing `mimllearning-1.0.8/docs/build/html/_static/scripts/sphinx-book-theme.js.map` & `mimllearning-1.0.9/docs/build/html/_static/scripts/sphinx-book-theme.js.map`

 * *Files identical despite different names*

### Comparing `mimllearning-1.0.8/docs/build/html/_static/styles/bootstrap.css` & `mimllearning-1.0.9/docs/build/html/_static/styles/bootstrap.css`

 * *Files identical despite different names*

### Comparing `mimllearning-1.0.8/docs/build/html/_static/styles/bootstrap.css.map` & `mimllearning-1.0.9/docs/build/html/_static/styles/bootstrap.css.map`

 * *Files identical despite different names*

### Comparing `mimllearning-1.0.8/docs/build/html/_static/styles/pydata-sphinx-theme.css` & `mimllearning-1.0.9/docs/build/html/_static/styles/pydata-sphinx-theme.css`

 * *Files identical despite different names*

### Comparing `mimllearning-1.0.8/docs/build/html/_static/styles/pydata-sphinx-theme.css.map` & `mimllearning-1.0.9/docs/build/html/_static/styles/pydata-sphinx-theme.css.map`

 * *Files identical despite different names*

### Comparing `mimllearning-1.0.8/docs/build/html/_static/styles/sphinx-book-theme.css` & `mimllearning-1.0.9/docs/build/html/_static/styles/sphinx-book-theme.css`

 * *Files identical despite different names*

### Comparing `mimllearning-1.0.8/docs/build/html/_static/vendor/fontawesome/6.5.1/LICENSE.txt` & `mimllearning-1.0.9/docs/build/html/_static/vendor/fontawesome/6.5.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `mimllearning-1.0.8/docs/build/html/_static/vendor/fontawesome/6.5.1/css/all.min.css` & `mimllearning-1.0.9/docs/build/html/_static/vendor/fontawesome/6.5.1/css/all.min.css`

 * *Files identical despite different names*

### Comparing `mimllearning-1.0.8/docs/build/html/_static/vendor/fontawesome/6.5.1/js/all.min.js` & `mimllearning-1.0.9/docs/build/html/_static/vendor/fontawesome/6.5.1/js/all.min.js`

 * *Files identical despite different names*

### Comparing `mimllearning-1.0.8/docs/build/html/_static/vendor/fontawesome/6.5.1/webfonts/fa-brands-400.ttf` & `mimllearning-1.0.9/docs/build/html/_static/vendor/fontawesome/6.5.1/webfonts/fa-brands-400.ttf`

 * *Files identical despite different names*

### Comparing `mimllearning-1.0.8/docs/build/html/_static/vendor/fontawesome/6.5.1/webfonts/fa-brands-400.woff2` & `mimllearning-1.0.9/docs/build/html/_static/vendor/fontawesome/6.5.1/webfonts/fa-brands-400.woff2`

 * *Files identical despite different names*

### Comparing `mimllearning-1.0.8/docs/build/html/_static/vendor/fontawesome/6.5.1/webfonts/fa-regular-400.ttf` & `mimllearning-1.0.9/docs/build/html/_static/vendor/fontawesome/6.5.1/webfonts/fa-regular-400.ttf`

 * *Files identical despite different names*

### Comparing `mimllearning-1.0.8/docs/build/html/_static/vendor/fontawesome/6.5.1/webfonts/fa-regular-400.woff2` & `mimllearning-1.0.9/docs/build/html/_static/vendor/fontawesome/6.5.1/webfonts/fa-regular-400.woff2`

 * *Files identical despite different names*

### Comparing `mimllearning-1.0.8/docs/build/html/_static/vendor/fontawesome/6.5.1/webfonts/fa-solid-900.ttf` & `mimllearning-1.0.9/docs/build/html/_static/vendor/fontawesome/6.5.1/webfonts/fa-solid-900.ttf`

 * *Files identical despite different names*

### Comparing `mimllearning-1.0.8/docs/build/html/_static/vendor/fontawesome/6.5.1/webfonts/fa-solid-900.woff2` & `mimllearning-1.0.9/docs/build/html/_static/vendor/fontawesome/6.5.1/webfonts/fa-solid-900.woff2`

 * *Files identical despite different names*

### Comparing `mimllearning-1.0.8/docs/build/html/_static/vendor/fontawesome/6.5.1/webfonts/fa-v4compatibility.ttf` & `mimllearning-1.0.9/docs/build/html/_static/vendor/fontawesome/6.5.1/webfonts/fa-v4compatibility.ttf`

 * *Files identical despite different names*

### Comparing `mimllearning-1.0.8/docs/build/html/_static/vendor/fontawesome/6.5.1/webfonts/fa-v4compatibility.woff2` & `mimllearning-1.0.9/docs/build/html/_static/vendor/fontawesome/6.5.1/webfonts/fa-v4compatibility.woff2`

 * *Files identical despite different names*

### Comparing `mimllearning-1.0.8/docs/build/html/classifier/index.html` & `mimllearning-1.0.9/docs/build/html/classifier/index.html`

 * *Files identical despite different names*

### Comparing `mimllearning-1.0.8/docs/build/html/classifier/mi.html` & `mimllearning-1.0.9/docs/build/html/classifier/mi.html`

 * *Files identical despite different names*

### Comparing `mimllearning-1.0.8/docs/build/html/classifier/mimlTOmi.html` & `mimllearning-1.0.9/docs/build/html/classifier/mimlTOmi.html`

 * *Files identical despite different names*

### Comparing `mimllearning-1.0.8/docs/build/html/classifier/mimlTOml.html` & `mimllearning-1.0.9/docs/build/html/classifier/mimlTOml.html`

 * *Files identical despite different names*

### Comparing `mimllearning-1.0.8/docs/build/html/classifier/miml_classifier.html` & `mimllearning-1.0.9/docs/build/html/classifier/miml_classifier.html`

 * *Files identical despite different names*

### Comparing `mimllearning-1.0.8/docs/build/html/classifier/_autosummary/miml.classifier.mi.apr_classifier.APRClassifier.html` & `mimllearning-1.0.9/docs/build/html/classifier/_autosummary/miml.classifier.mi.apr_classifier.APRClassifier.html`

 * *Files identical despite different names*

### Comparing `mimllearning-1.0.8/docs/build/html/classifier/_autosummary/miml.classifier.mi.mi_wrapper_classifier.MIWrapperClassifier.html` & `mimllearning-1.0.9/docs/build/html/classifier/_autosummary/miml.classifier.mi.mi_wrapper_classifier.MIWrapperClassifier.html`

 * *Files identical despite different names*

### Comparing `mimllearning-1.0.8/docs/build/html/classifier/_autosummary/miml.classifier.mimlTOmi.miml_to_mi_br_classifier.MIMLtoMIBRClassifier.html` & `mimllearning-1.0.9/docs/build/html/classifier/_autosummary/miml.classifier.mimlTOmi.miml_to_mi_br_classifier.MIMLtoMIBRClassifier.html`

 * *Files identical despite different names*

### Comparing `mimllearning-1.0.8/docs/build/html/classifier/_autosummary/miml.classifier.mimlTOmi.miml_to_mi_classifier.MIMLtoMIClassifier.html` & `mimllearning-1.0.9/docs/build/html/classifier/_autosummary/miml.classifier.mimlTOmi.miml_to_mi_classifier.MIMLtoMIClassifier.html`

 * *Files identical despite different names*

### Comparing `mimllearning-1.0.8/docs/build/html/classifier/_autosummary/miml.classifier.mimlTOmi.miml_to_mi_lp_classifier.MIMLtoMILPClassifier.html` & `mimllearning-1.0.9/docs/build/html/classifier/_autosummary/miml.classifier.mimlTOmi.miml_to_mi_lp_classifier.MIMLtoMILPClassifier.html`

 * *Files identical despite different names*

### Comparing `mimllearning-1.0.8/docs/build/html/classifier/_autosummary/miml.classifier.mimlTOml.miml_to_ml_classifier.MIMLtoMLClassifier.html` & `mimllearning-1.0.9/docs/build/html/classifier/_autosummary/miml.classifier.mimlTOml.miml_to_ml_classifier.MIMLtoMLClassifier.html`

 * *Files identical despite different names*

### Comparing `mimllearning-1.0.8/docs/build/html/classifier/_autosummary/miml.classifier.miml_classifier.MIMLClassifier.html` & `mimllearning-1.0.9/docs/build/html/classifier/_autosummary/miml.classifier.miml_classifier.MIMLClassifier.html`

 * *Files identical despite different names*

### Comparing `mimllearning-1.0.8/docs/build/html/data/bag.html` & `mimllearning-1.0.9/docs/build/html/data/bag.html`

 * *Files identical despite different names*

### Comparing `mimllearning-1.0.8/docs/build/html/data/dataset_utils.html` & `mimllearning-1.0.9/docs/build/html/data/dataset_utils.html`

 * *Files identical despite different names*

### Comparing `mimllearning-1.0.8/docs/build/html/data/index.html` & `mimllearning-1.0.9/docs/build/html/data/index.html`

 * *Files identical despite different names*

### Comparing `mimllearning-1.0.8/docs/build/html/data/instance.html` & `mimllearning-1.0.9/docs/build/html/data/instance.html`

 * *Files identical despite different names*

### Comparing `mimllearning-1.0.8/docs/build/html/data/miml_dataset.html` & `mimllearning-1.0.9/docs/build/html/data/miml_dataset.html`

 * *Files identical despite different names*

### Comparing `mimllearning-1.0.8/docs/build/html/data/_autosummary/miml.data.bag.Bag.html` & `mimllearning-1.0.9/docs/build/html/data/_autosummary/miml.data.bag.Bag.html`

 * *Files identical despite different names*

### Comparing `mimllearning-1.0.8/docs/build/html/data/_autosummary/miml.data.instance.Instance.html` & `mimllearning-1.0.9/docs/build/html/data/_autosummary/miml.data.instance.Instance.html`

 * *Files identical despite different names*

### Comparing `mimllearning-1.0.8/docs/build/html/data/_autosummary/miml.data.miml_dataset.MIMLDataset.html` & `mimllearning-1.0.9/docs/build/html/data/_autosummary/miml.data.miml_dataset.MIMLDataset.html`

 * *Files identical despite different names*

### Comparing `mimllearning-1.0.8/docs/build/html/report/index.html` & `mimllearning-1.0.9/docs/build/html/report/index.html`

 * *Files identical despite different names*

### Comparing `mimllearning-1.0.8/docs/build/html/report/report.html` & `mimllearning-1.0.9/docs/build/html/report/report.html`

 * *Files identical despite different names*

### Comparing `mimllearning-1.0.8/docs/build/html/report/_autosummary/miml.report.report.Report.html` & `mimllearning-1.0.9/docs/build/html/report/_autosummary/miml.report.report.Report.html`

 * *Files identical despite different names*

### Comparing `mimllearning-1.0.8/docs/build/html/transformation/index.html` & `mimllearning-1.0.9/docs/build/html/transformation/index.html`

 * *Files identical despite different names*

### Comparing `mimllearning-1.0.8/docs/build/html/transformation/mimlTOmi.html` & `mimllearning-1.0.9/docs/build/html/transformation/mimlTOmi.html`

 * *Files identical despite different names*

### Comparing `mimllearning-1.0.8/docs/build/html/transformation/mimlTOml.html` & `mimllearning-1.0.9/docs/build/html/transformation/mimlTOml.html`

 * *Files identical despite different names*

### Comparing `mimllearning-1.0.8/docs/build/html/transformation/_autosummary/miml.transformation.mimlTOmi.binary_relevance_transformation.BinaryRelevanceTransformation.html` & `mimllearning-1.0.9/docs/build/html/transformation/_autosummary/miml.transformation.mimlTOmi.binary_relevance_transformation.BinaryRelevanceTransformation.html`

 * *Files identical despite different names*

### Comparing `mimllearning-1.0.8/docs/build/html/transformation/_autosummary/miml.transformation.mimlTOmi.label_powerset_transformation.LabelPowersetTransformation.html` & `mimllearning-1.0.9/docs/build/html/transformation/_autosummary/miml.transformation.mimlTOmi.label_powerset_transformation.LabelPowersetTransformation.html`

 * *Files identical despite different names*

### Comparing `mimllearning-1.0.8/docs/build/html/transformation/_autosummary/miml.transformation.mimlTOml.arithmetic.ArithmeticTransformation.html` & `mimllearning-1.0.9/docs/build/html/transformation/_autosummary/miml.transformation.mimlTOml.arithmetic.ArithmeticTransformation.html`

 * *Files identical despite different names*

### Comparing `mimllearning-1.0.8/docs/build/html/transformation/_autosummary/miml.transformation.mimlTOml.geometric.GeometricTransformation.html` & `mimllearning-1.0.9/docs/build/html/transformation/_autosummary/miml.transformation.mimlTOml.geometric.GeometricTransformation.html`

 * *Files identical despite different names*

### Comparing `mimllearning-1.0.8/docs/build/html/transformation/_autosummary/miml.transformation.mimlTOml.miml_to_ml_transformation.MIMLtoMLTransformation.html` & `mimllearning-1.0.9/docs/build/html/transformation/_autosummary/miml.transformation.mimlTOml.miml_to_ml_transformation.MIMLtoMLTransformation.html`

 * *Files identical despite different names*

### Comparing `mimllearning-1.0.8/docs/build/html/transformation/_autosummary/miml.transformation.mimlTOml.minmax.MinMaxTransformation.html` & `mimllearning-1.0.9/docs/build/html/transformation/_autosummary/miml.transformation.mimlTOml.minmax.MinMaxTransformation.html`

 * *Files identical despite different names*

### Comparing `mimllearning-1.0.8/docs/source/conf.py` & `mimllearning-1.0.9/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `mimllearning-1.0.8/docs/source/_templates/base.rst` & `mimllearning-1.0.9/docs/source/_templates/base.rst`

 * *Files identical despite different names*

### Comparing `mimllearning-1.0.8/docs/source/classifier/_autosummary/miml.classifier.mimlTOmi.miml_to_mi_br_classifier.MIMLtoMIBRClassifier.rst` & `mimllearning-1.0.9/docs/source/classifier/_autosummary/miml.classifier.mimlTOmi.miml_to_mi_br_classifier.MIMLtoMIBRClassifier.rst`

 * *Files identical despite different names*

### Comparing `mimllearning-1.0.8/docs/source/classifier/_autosummary/miml.classifier.mimlTOmi.miml_to_mi_classifier.MIMLtoMIClassifier.rst` & `mimllearning-1.0.9/docs/source/classifier/_autosummary/miml.classifier.mimlTOmi.miml_to_mi_classifier.MIMLtoMIClassifier.rst`

 * *Files identical despite different names*

### Comparing `mimllearning-1.0.8/docs/source/classifier/_autosummary/miml.classifier.mimlTOmi.miml_to_mi_lp_classifier.MIMLtoMILPClassifier.rst` & `mimllearning-1.0.9/docs/source/classifier/_autosummary/miml.classifier.mimlTOmi.miml_to_mi_lp_classifier.MIMLtoMILPClassifier.rst`

 * *Files identical despite different names*

### Comparing `mimllearning-1.0.8/docs/source/classifier/_autosummary/miml.classifier.mimlTOml.miml_to_ml_classifier.MIMLtoMLClassifier.rst` & `mimllearning-1.0.9/docs/source/classifier/_autosummary/miml.classifier.mimlTOml.miml_to_ml_classifier.MIMLtoMLClassifier.rst`

 * *Files identical despite different names*

### Comparing `mimllearning-1.0.8/docs/source/data/_autosummary/miml.data.bag.Bag.rst` & `mimllearning-1.0.9/docs/source/data/_autosummary/miml.data.bag.Bag.rst`

 * *Files identical despite different names*

### Comparing `mimllearning-1.0.8/docs/source/data/_autosummary/miml.data.miml_dataset.MIMLDataset.rst` & `mimllearning-1.0.9/docs/source/data/_autosummary/miml.data.miml_dataset.MIMLDataset.rst`

 * *Files identical despite different names*

### Comparing `mimllearning-1.0.8/docs/source/transformation/_autosummary/miml.transformation.mimlTOmi.binary_relevance_transformation.BinaryRelevanceTransformation.rst` & `mimllearning-1.0.9/docs/source/transformation/_autosummary/miml.transformation.mimlTOmi.binary_relevance_transformation.BinaryRelevanceTransformation.rst`

 * *Files identical despite different names*

### Comparing `mimllearning-1.0.8/docs/source/transformation/_autosummary/miml.transformation.mimlTOmi.label_powerset_transformation.LabelPowersetTransformation.rst` & `mimllearning-1.0.9/docs/source/transformation/_autosummary/miml.transformation.mimlTOmi.label_powerset_transformation.LabelPowersetTransformation.rst`

 * *Files identical despite different names*

### Comparing `mimllearning-1.0.8/docs/source/transformation/_autosummary/miml.transformation.mimlTOml.miml_to_ml_transformation.MIMLtoMLTransformation.rst` & `mimllearning-1.0.9/docs/source/transformation/_autosummary/miml.transformation.mimlTOml.miml_to_ml_transformation.MIMLtoMLTransformation.rst`

 * *Files identical despite different names*

### Comparing `mimllearning-1.0.8/documentation/AnteproyectoDamianTFG.pdf` & `mimllearning-1.0.9/documentation/AnteproyectoDamianTFG.pdf`

 * *Files identical despite different names*

### Comparing `mimllearning-1.0.8/src/miml/classifier/miml_classifier.py` & `mimllearning-1.0.9/src/miml/classifier/miml_classifier.py`

 * *Files identical despite different names*

### Comparing `mimllearning-1.0.8/src/miml/classifier/mi/apr_classifier.py` & `mimllearning-1.0.9/src/miml/classifier/mi/apr_classifier.py`

 * *Files identical despite different names*

### Comparing `mimllearning-1.0.8/src/miml/classifier/mi/mi_wrapper_classifier.py` & `mimllearning-1.0.9/src/miml/classifier/mi/mi_wrapper_classifier.py`

 * *Files 2% similar despite different names*

```diff
@@ -93,9 +93,12 @@
         results: np.ndarray of shape (n_instances, n_labels, 1)
             Predicted probabilities for given data
         """
         bag_probs = []
         for bag in x_test:
             instance_probs = self.base_classifier.predict_proba(bag)
             avg_probs = np.mean(instance_probs, axis=0)
+            # sklearn.predict_proba change output if not multilabel. Adjusting output
+            if len(self.classes_) == 2:
+                avg_probs = avg_probs[1]
             bag_probs.append(avg_probs)
         return np.array(bag_probs)
```

### Comparing `mimllearning-1.0.8/src/miml/classifier/mimlTOmi/miml_to_mi_br_classifier.py` & `mimllearning-1.0.9/src/miml/classifier/mimlTOmi/miml_to_mi_br_classifier.py`

 * *Files identical despite different names*

### Comparing `mimllearning-1.0.8/src/miml/classifier/mimlTOmi/miml_to_mi_classifier.py` & `mimllearning-1.0.9/src/miml/classifier/mimlTOmi/miml_to_mi_classifier.py`

 * *Files identical despite different names*

### Comparing `mimllearning-1.0.8/src/miml/classifier/mimlTOmi/miml_to_mi_lp_classifier.py` & `mimllearning-1.0.9/src/miml/classifier/mimlTOmi/miml_to_mi_lp_classifier.py`

 * *Files identical despite different names*

### Comparing `mimllearning-1.0.8/src/miml/classifier/mimlTOml/miml_to_ml_classifier.py` & `mimllearning-1.0.9/src/miml/classifier/mimlTOml/miml_to_ml_classifier.py`

 * *Files identical despite different names*

### Comparing `mimllearning-1.0.8/src/miml/data/bag.py` & `mimllearning-1.0.9/src/miml/data/bag.py`

 * *Files identical despite different names*

### Comparing `mimllearning-1.0.8/src/miml/data/dataset_utils.py` & `mimllearning-1.0.9/src/miml/data/dataset_utils.py`

 * *Files identical despite different names*

### Comparing `mimllearning-1.0.8/src/miml/data/instance.py` & `mimllearning-1.0.9/src/miml/data/instance.py`

 * *Files identical despite different names*

### Comparing `mimllearning-1.0.8/src/miml/data/miml_dataset.py` & `mimllearning-1.0.9/src/miml/data/miml_dataset.py`

 * *Files identical despite different names*

### Comparing `mimllearning-1.0.8/src/miml/datasets/miml_birds.arff` & `mimllearning-1.0.9/src/miml/datasets/miml_birds.arff`

 * *Files identical despite different names*

### Comparing `mimllearning-1.0.8/src/miml/datasets/miml_birds.csv` & `mimllearning-1.0.9/src/miml/datasets/miml_birds.csv`

 * *Files identical despite different names*

### Comparing `mimllearning-1.0.8/src/miml/datasets/miml_birds_random_20test.arff` & `mimllearning-1.0.9/src/miml/datasets/miml_birds_random_20test.arff`

 * *Files identical despite different names*

### Comparing `mimllearning-1.0.8/src/miml/datasets/miml_birds_random_80train.arff` & `mimllearning-1.0.9/src/miml/datasets/miml_birds_random_80train.arff`

 * *Files identical despite different names*

### Comparing `mimllearning-1.0.8/src/miml/report/report.py` & `mimllearning-1.0.9/src/miml/report/report.py`

 * *Files identical despite different names*

### Comparing `mimllearning-1.0.8/src/miml/transformation/mimlTOmi/binary_relevance_transformation.py` & `mimllearning-1.0.9/src/miml/transformation/mimlTOmi/binary_relevance_transformation.py`

 * *Files identical despite different names*

### Comparing `mimllearning-1.0.8/src/miml/transformation/mimlTOmi/label_powerset_transformation.py` & `mimllearning-1.0.9/src/miml/transformation/mimlTOmi/label_powerset_transformation.py`

 * *Files identical despite different names*

### Comparing `mimllearning-1.0.8/src/miml/transformation/mimlTOml/arithmetic.py` & `mimllearning-1.0.9/src/miml/transformation/mimlTOml/arithmetic.py`

 * *Files identical despite different names*

### Comparing `mimllearning-1.0.8/src/miml/transformation/mimlTOml/geometric.py` & `mimllearning-1.0.9/src/miml/transformation/mimlTOml/geometric.py`

 * *Files identical despite different names*

### Comparing `mimllearning-1.0.8/src/miml/transformation/mimlTOml/minmax.py` & `mimllearning-1.0.9/src/miml/transformation/mimlTOml/minmax.py`

 * *Files identical despite different names*

### Comparing `mimllearning-1.0.8/src/miml/tutorial/classifiers_comparison_experiment_miml.ipynb` & `mimllearning-1.0.9/src/miml/tutorial/classifiers_comparison_experiment_miml.ipynb`

 * *Files identical despite different names*

### Comparing `mimllearning-1.0.8/src/miml/tutorial/classifiers_mimltomi.ipynb` & `mimllearning-1.0.9/src/miml/tutorial/classifiers_mimltomi.ipynb`

 * *Files identical despite different names*

### Comparing `mimllearning-1.0.8/src/miml/tutorial/classifiers_mimltoml.ipynb` & `mimllearning-1.0.9/src/miml/tutorial/classifiers_mimltoml.ipynb`

 * *Files identical despite different names*

### Comparing `mimllearning-1.0.8/src/miml/tutorial/data_miml.ipynb` & `mimllearning-1.0.9/src/miml/tutorial/data_miml.ipynb`

 * *Files identical despite different names*

### Comparing `mimllearning-1.0.8/src/miml/tutorial/train_test_experiment_miml.ipynb` & `mimllearning-1.0.9/src/miml/tutorial/train_test_experiment_miml.ipynb`

 * *Files identical despite different names*

### Comparing `mimllearning-1.0.8/src/miml/tutorial/transformations_miml.ipynb` & `mimllearning-1.0.9/src/miml/tutorial/transformations_miml.ipynb`

 * *Files identical despite different names*

### Comparing `mimllearning-1.0.8/LICENSE.txt` & `mimllearning-1.0.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `mimllearning-1.0.8/README.md` & `mimllearning-1.0.9/README.md`

 * *Files identical despite different names*

### Comparing `mimllearning-1.0.8/pyproject.toml` & `mimllearning-1.0.9/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -2,20 +2,20 @@
 requires = ["hatchling", "pkginfo >= 1.10"]
 build-backend = "hatchling.build"
 
 [tool.hatch.build.targets.wheel]
 packages = ["src/miml", "src/miml/*"]
 
 [metadata]
-version = "1.0.8"
+version = "1.0.9"
 name = "mimllearning"
 
 [project]
 name = "mimllearning"
-version = "1.0.8"
+version = "1.0.9"
 authors = [
   { name="Damian Martinez", email="damianmartinezavila@gmail.com" },
 ]
 description = "MIML Learning Library"
 license = "GPL-3.0"
 keywords = ["machine-learning", "python", "data-science", "miml", "multilabel", "multi-instance"]
 readme = "README.md"
```

### Comparing `mimllearning-1.0.8/PKG-INFO` & `mimllearning-1.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: mimllearning
-Version: 1.0.8
+Version: 1.0.9
 Summary: MIML Learning Library
 Project-URL: Homepage, https://github.com/p82maavd/miml
 Author-email: Damian Martinez <damianmartinezavila@gmail.com>
 License-Expression: GPL-3.0
 License-File: LICENSE.txt
 Keywords: data-science,machine-learning,miml,multi-instance,multilabel,python
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
```

