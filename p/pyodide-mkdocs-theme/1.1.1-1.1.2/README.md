# Comparing `tmp/pyodide_mkdocs_theme-1.1.1.tar.gz` & `tmp/pyodide_mkdocs_theme-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyodide_mkdocs_theme-1.1.1.tar", max compression
+gzip compressed data, was "pyodide_mkdocs_theme-1.1.2.tar", max compression
```

## Comparing `pyodide_mkdocs_theme-1.1.1.tar` & `pyodide_mkdocs_theme-1.1.2.tar`

### file list

```diff
@@ -1,78 +1,78 @@
--rw-r--r--   0        0        0    35118 2024-04-04 09:39:00.129784 pyodide_mkdocs_theme-1.1.1/LICENSE
--rwxr-xr-x   0        0        0     1337 2024-04-08 19:01:06.251164 pyodide_mkdocs_theme-1.1.1/README.md
--rw-r--r--   0        0        0     1347 2024-06-01 14:49:26.747869 pyodide_mkdocs_theme-1.1.1/pyodide_mkdocs_theme/__init__.py
--rw-r--r--   0        0        0     2932 2024-06-01 14:48:42.918567 pyodide_mkdocs_theme-1.1.1/pyodide_mkdocs_theme/__main__.py
--rw-r--r--   0        0        0       22 2024-06-01 14:49:26.791870 pyodide_mkdocs_theme-1.1.1/pyodide_mkdocs_theme/__version__.py
--rw-r--r--   0        0        0      807 2024-04-12 21:48:00.494695 pyodide_mkdocs_theme-1.1.1/pyodide_mkdocs_theme/pyodide_macros/__init__.py
--rw-r--r--   0        0        0     1322 2024-05-15 21:11:56.281098 pyodide_mkdocs_theme-1.1.1/pyodide_mkdocs_theme/pyodide_macros/deprecation.py
--rw-r--r--   0        0        0     1063 2024-05-15 21:11:56.293098 pyodide_mkdocs_theme-1.1.1/pyodide_mkdocs_theme/pyodide_macros/exceptions.py
--rw-r--r--   0        0        0     1190 2024-05-12 18:52:50.335028 pyodide_mkdocs_theme-1.1.1/pyodide_mkdocs_theme/pyodide_macros/html_builder/__init__.py
--rw-r--r--   0        0        0     5919 2024-05-15 21:11:56.321099 pyodide_mkdocs_theme-1.1.1/pyodide_mkdocs_theme/pyodide_macros/html_builder/_html_builder.py
--rw-r--r--   0        0        0     2996 2024-05-27 09:57:27.861116 pyodide_mkdocs_theme-1.1.1/pyodide_mkdocs_theme/pyodide_macros/macros/IDEs.py
--rw-r--r--   0        0        0        0 2024-05-15 21:11:56.329099 pyodide_mkdocs_theme-1.1.1/pyodide_mkdocs_theme/pyodide_macros/macros/__init__.py
--rw-r--r--   0        0        0     6043 2024-04-27 20:26:40.306387 pyodide_mkdocs_theme-1.1.1/pyodide_mkdocs_theme/pyodide_macros/macros/autres.py
--rw-r--r--   0        0        0    17204 2024-05-27 09:57:27.861116 pyodide_mkdocs_theme-1.1.1/pyodide_mkdocs_theme/pyodide_macros/macros/ide_files_data.py
--rw-r--r--   0        0        0    13843 2024-05-27 15:46:51.107092 pyodide_mkdocs_theme-1.1.1/pyodide_mkdocs_theme/pyodide_macros/macros/ide_ide.py
--rw-r--r--   0        0        0    19389 2024-05-27 15:43:10.834870 pyodide_mkdocs_theme-1.1.1/pyodide_mkdocs_theme/pyodide_macros/macros/ide_manager.py
--rw-r--r--   0        0        0     4972 2024-05-27 09:57:27.861116 pyodide_mkdocs_theme-1.1.1/pyodide_mkdocs_theme/pyodide_macros/macros/ide_pybtn.py
--rw-r--r--   0        0        0     3460 2024-05-27 09:57:27.861116 pyodide_mkdocs_theme-1.1.1/pyodide_mkdocs_theme/pyodide_macros/macros/ide_terminal.py
--rw-r--r--   0        0        0     2435 2024-05-15 21:11:56.389101 pyodide_mkdocs_theme-1.1.1/pyodide_mkdocs_theme/pyodide_macros/macros/isolated_components.py
--rw-r--r--   0        0        0    11591 2024-05-30 18:15:00.841773 pyodide_mkdocs_theme-1.1.1/pyodide_mkdocs_theme/pyodide_macros/macros/qcm.py
--rw-r--r--   0        0        0    14303 2024-06-01 14:48:42.918567 pyodide_mkdocs_theme-1.1.1/pyodide_mkdocs_theme/pyodide_macros/messages.py
--rw-r--r--   0        0        0     7422 2024-05-27 09:57:27.861116 pyodide_mkdocs_theme-1.1.1/pyodide_mkdocs_theme/pyodide_macros/pages_and_ides_configs.py
--rw-r--r--   0        0        0    16171 2024-05-27 09:57:27.861116 pyodide_mkdocs_theme-1.1.1/pyodide_mkdocs_theme/pyodide_macros/parsing.py
--rw-r--r--   0        0        0     4776 2024-05-15 21:11:56.421101 pyodide_mkdocs_theme-1.1.1/pyodide_mkdocs_theme/pyodide_macros/paths_utils.py
--rw-r--r--   0        0        0        0 2024-05-15 21:11:56.421101 pyodide_mkdocs_theme-1.1.1/pyodide_mkdocs_theme/pyodide_macros/plugin/__init__.py
--rw-r--r--   0        0        0    15211 2024-05-15 21:11:56.421101 pyodide_mkdocs_theme-1.1.1/pyodide_mkdocs_theme/pyodide_macros/plugin/config.py
--rw-r--r--   0        0        0    11391 2024-05-25 09:20:37.108858 pyodide_mkdocs_theme-1.1.1/pyodide_mkdocs_theme/pyodide_macros/plugin/maestro_IDE.py
--rw-r--r--   0        0        0     9693 2024-05-15 21:11:56.421101 pyodide_mkdocs_theme-1.1.1/pyodide_mkdocs_theme/pyodide_macros/plugin/maestro_base.py
--rw-r--r--   0        0        0     1603 2024-05-15 21:11:56.425101 pyodide_mkdocs_theme-1.1.1/pyodide_mkdocs_theme/pyodide_macros/plugin/maestro_extras.py
--rw-r--r--   0        0        0     6652 2024-05-15 21:11:56.425101 pyodide_mkdocs_theme-1.1.1/pyodide_mkdocs_theme/pyodide_macros/plugin/maestro_indent.py
--rw-r--r--   0        0        0     2877 2024-04-24 20:11:56.666105 pyodide_mkdocs_theme-1.1.1/pyodide_mkdocs_theme/pyodide_macros/plugin/maestro_tools.py
--rw-r--r--   0        0        0     9272 2024-06-01 14:48:42.926567 pyodide_mkdocs_theme-1.1.1/pyodide_mkdocs_theme/pyodide_macros/plugin/pyodide_macros_plugin.py
--rw-r--r--   0        0        0     2658 2024-04-11 09:41:00.023938 pyodide_mkdocs_theme-1.1.1/pyodide_mkdocs_theme/pyodide_macros/pyodide_logger.py
--rw-r--r--   0        0        0     1163 2024-05-15 21:11:56.425101 pyodide_mkdocs_theme-1.1.1/pyodide_mkdocs_theme/pyodide_macros/scripts_templates.py
--rw-r--r--   0        0        0     9846 2024-05-27 09:57:27.865116 pyodide_mkdocs_theme-1.1.1/pyodide_mkdocs_theme/pyodide_macros/tools_and_constants.py
--rw-r--r--   0        0        0     3739 2024-06-01 14:49:26.747869 pyodide_mkdocs_theme-1.1.1/pyodide_mkdocs_theme/scripts/custom_lang.py
--rw-r--r--   0        0        0     4776 2024-05-27 09:57:27.865116 pyodide_mkdocs_theme-1.1.1/pyodide_mkdocs_theme/scripts/mkdocs.yml
--rw-r--r--   0        0        0     2902 2024-05-27 09:57:27.865116 pyodide_mkdocs_theme-1.1.1/pyodide_mkdocs_theme/scripts/model.py
--rw-r--r--   0        0        0      823 2024-05-15 21:11:56.425101 pyodide_mkdocs_theme-1.1.1/pyodide_mkdocs_theme/templates/README.md
--rw-r--r--   0        0        0        0 2024-05-15 21:11:56.425101 pyodide_mkdocs_theme-1.1.1/pyodide_mkdocs_theme/templates/__init__.py
--rw-r--r--   0        0        0     2857 2024-05-15 21:11:56.425101 pyodide_mkdocs_theme-1.1.1/pyodide_mkdocs_theme/templates/assets/images/.qcm-circle.svg
--rw-r--r--   0        0        0     1645 2024-05-15 21:11:56.425101 pyodide_mkdocs_theme-1.1.1/pyodide_mkdocs_theme/templates/assets/images/icons8-check-64.png
--rw-r--r--   0        0        0     1328 2024-05-15 21:11:56.425101 pyodide_mkdocs_theme-1.1.1/pyodide_mkdocs_theme/templates/assets/images/icons8-download-64.png
--rw-r--r--   0        0        0     1761 2024-05-15 21:11:56.425101 pyodide_mkdocs_theme-1.1.1/pyodide_mkdocs_theme/templates/assets/images/icons8-play-64.png
--rw-r--r--   0        0        0     1283 2024-05-15 21:11:56.425101 pyodide_mkdocs_theme-1.1.1/pyodide_mkdocs_theme/templates/assets/images/icons8-restart-64.png
--rw-r--r--   0        0        0      952 2024-05-15 21:11:56.429102 pyodide_mkdocs_theme-1.1.1/pyodide_mkdocs_theme/templates/assets/images/icons8-save-64.png
--rw-r--r--   0        0        0     1296 2024-05-15 21:11:56.429102 pyodide_mkdocs_theme-1.1.1/pyodide_mkdocs_theme/templates/assets/images/icons8-upload-64.png
--rw-r--r--   0        0        0        0 2024-05-16 21:25:14.310769 pyodide_mkdocs_theme-1.1.1/pyodide_mkdocs_theme/templates/hooks/libsAfter.html
--rw-r--r--   0        0        0        0 2024-05-16 21:25:14.310769 pyodide_mkdocs_theme-1.1.1/pyodide_mkdocs_theme/templates/hooks/libsBefore.html
--rw-r--r--   0        0        0        0 2024-05-16 21:25:14.310769 pyodide_mkdocs_theme-1.1.1/pyodide_mkdocs_theme/templates/hooks/scriptsAfter.html
--rw-r--r--   0        0        0        0 2024-05-16 21:25:14.310769 pyodide_mkdocs_theme-1.1.1/pyodide_mkdocs_theme/templates/hooks/scriptsBefore.html
--rw-r--r--   0        0        0     6152 2024-06-01 14:48:42.930567 pyodide_mkdocs_theme-1.1.1/pyodide_mkdocs_theme/templates/js-libs/0_config-libs.js
--rw-r--r--   0        0        0    14903 2024-06-01 14:48:42.930567 pyodide_mkdocs_theme-1.1.1/pyodide_mkdocs_theme/templates/js-libs/functools-libs.js
--rw-r--r--   0        0        0     1770 2024-06-01 14:49:23.195763 pyodide_mkdocs_theme-1.1.1/pyodide_mkdocs_theme/templates/js-libs/jsLogger-libs.js
--rw-r--r--   0        0        0     1490 2024-04-09 19:35:36.230493 pyodide_mkdocs_theme-1.1.1/pyodide_mkdocs_theme/templates/js-libs/mathjax-libs.js
--rw-r--r--   0        0        0     4361 2024-04-29 14:09:33.373857 pyodide_mkdocs_theme-1.1.1/pyodide_mkdocs_theme/templates/js-libs/z_globalGuiButtons-libs.js
--rw-r--r--   0        0        0    13514 2024-06-01 14:48:42.930567 pyodide_mkdocs_theme-1.1.1/pyodide_mkdocs_theme/templates/js-per-pages/0_genericPythonSnippets-pyodide.js
--rw-r--r--   0        0        0    15301 2024-05-27 09:57:27.865116 pyodide_mkdocs_theme-1.1.1/pyodide_mkdocs_theme/templates/js-per-pages/1_pyodideSectionsRunner-pyodide.js
--rw-r--r--   0        0        0     1157 2024-05-27 09:57:27.865116 pyodide_mkdocs_theme-1.1.1/pyodide_mkdocs_theme/templates/js-per-pages/2_btnRunner-pyodide.js
--rw-r--r--   0        0        0     9294 2024-06-01 14:48:42.930567 pyodide_mkdocs_theme-1.1.1/pyodide_mkdocs_theme/templates/js-per-pages/2_terminalRunner-terms.js
--rw-r--r--   0        0        0    17299 2024-06-01 14:48:42.930567 pyodide_mkdocs_theme-1.1.1/pyodide_mkdocs_theme/templates/js-per-pages/3_ideRunner-ides.js
--rw-r--r--   0        0        0    12716 2024-05-15 21:11:56.437102 pyodide_mkdocs_theme-1.1.1/pyodide_mkdocs_theme/templates/js-per-pages/qcms-qcm.js
--rw-r--r--   0        0        0     7237 2024-05-27 09:57:27.869116 pyodide_mkdocs_theme-1.1.1/pyodide_mkdocs_theme/templates/js-per-pages/start-pyodide.js
--rw-r--r--   0        0        0    11534 2024-06-01 14:48:42.930567 pyodide_mkdocs_theme-1.1.1/pyodide_mkdocs_theme/templates/js-scripts/error-logs-generator-scripts.js
--rw-r--r--   0        0        0     4455 2024-05-15 21:11:56.489103 pyodide_mkdocs_theme-1.1.1/pyodide_mkdocs_theme/templates/js-scripts/z_doLast-subscriptions-scripts.js
--rw-r--r--   0        0        0     5341 2024-05-15 21:11:56.505103 pyodide_mkdocs_theme-1.1.1/pyodide_mkdocs_theme/templates/main.html
--rw-r--r--   0        0        0     2635 2024-05-15 21:11:56.505103 pyodide_mkdocs_theme-1.1.1/pyodide_mkdocs_theme/templates/mkdocs_theme.yml
--rw-r--r--   0        0        0      802 2024-04-03 22:13:32.135114 pyodide_mkdocs_theme-1.1.1/pyodide_mkdocs_theme/templates/partials/copyright.html
--rw-r--r--   0        0        0     2084 2024-04-03 21:47:24.620870 pyodide_mkdocs_theme-1.1.1/pyodide_mkdocs_theme/templates/partials/footer.html
--rw-r--r--   0        0        0      578 2024-04-03 22:14:08.956199 pyodide_mkdocs_theme-1.1.1/pyodide_mkdocs_theme/templates/partials/social.html
--rw-r--r--   0        0        0     3831 2024-05-15 21:11:56.517104 pyodide_mkdocs_theme-1.1.1/pyodide_mkdocs_theme/templates/pyodide-css/0_generic-tooltips-libs.css
--rw-r--r--   0        0        0     1078 2024-05-15 21:11:56.517104 pyodide_mkdocs_theme-1.1.1/pyodide_mkdocs_theme/templates/pyodide-css/header-btns-libs.css
--rw-r--r--   0        0        0     1947 2024-05-15 21:11:56.517104 pyodide_mkdocs_theme-1.1.1/pyodide_mkdocs_theme/templates/pyodide-css/hourglass-libs.css
--rw-r--r--   0        0        0     3764 2024-05-16 18:56:03.284304 pyodide_mkdocs_theme-1.1.1/pyodide_mkdocs_theme/templates/pyodide-css/ide-libs.css
--rw-r--r--   0        0        0     3904 2024-05-15 21:11:56.525104 pyodide_mkdocs_theme-1.1.1/pyodide_mkdocs_theme/templates/pyodide-css/qcm-libs.css
--rw-r--r--   0        0        0     1918 2024-05-15 21:11:56.525104 pyodide_mkdocs_theme-1.1.1/pyodide_mkdocs_theme/templates/pyodide-css/terminal-libs.css
--rw-r--r--   0        0        0     1766 2024-06-01 14:49:23.235765 pyodide_mkdocs_theme-1.1.1/pyproject.toml
--rw-r--r--   0        0        0     2864 1970-01-01 00:00:00.000000 pyodide_mkdocs_theme-1.1.1/PKG-INFO
+-rw-r--r--   0        0        0    35118 2024-04-04 09:39:00.129784 pyodide_mkdocs_theme-1.1.2/LICENSE
+-rwxr-xr-x   0        0        0     1337 2024-04-08 19:01:06.251164 pyodide_mkdocs_theme-1.1.2/README.md
+-rw-r--r--   0        0        0     1347 2024-06-03 15:14:11.561658 pyodide_mkdocs_theme-1.1.2/pyodide_mkdocs_theme/__init__.py
+-rw-r--r--   0        0        0     2938 2024-06-01 14:58:39.892295 pyodide_mkdocs_theme-1.1.2/pyodide_mkdocs_theme/__main__.py
+-rw-r--r--   0        0        0       22 2024-06-03 15:14:11.609660 pyodide_mkdocs_theme-1.1.2/pyodide_mkdocs_theme/__version__.py
+-rw-r--r--   0        0        0      807 2024-04-12 21:48:00.494695 pyodide_mkdocs_theme-1.1.2/pyodide_mkdocs_theme/pyodide_macros/__init__.py
+-rw-r--r--   0        0        0     1322 2024-05-15 21:11:56.281098 pyodide_mkdocs_theme-1.1.2/pyodide_mkdocs_theme/pyodide_macros/deprecation.py
+-rw-r--r--   0        0        0     1063 2024-05-15 21:11:56.293098 pyodide_mkdocs_theme-1.1.2/pyodide_mkdocs_theme/pyodide_macros/exceptions.py
+-rw-r--r--   0        0        0     1190 2024-05-12 18:52:50.335028 pyodide_mkdocs_theme-1.1.2/pyodide_mkdocs_theme/pyodide_macros/html_builder/__init__.py
+-rw-r--r--   0        0        0     5919 2024-05-15 21:11:56.321099 pyodide_mkdocs_theme-1.1.2/pyodide_mkdocs_theme/pyodide_macros/html_builder/_html_builder.py
+-rw-r--r--   0        0        0     2996 2024-05-27 09:57:27.861116 pyodide_mkdocs_theme-1.1.2/pyodide_mkdocs_theme/pyodide_macros/macros/IDEs.py
+-rw-r--r--   0        0        0        0 2024-05-15 21:11:56.329099 pyodide_mkdocs_theme-1.1.2/pyodide_mkdocs_theme/pyodide_macros/macros/__init__.py
+-rw-r--r--   0        0        0     6043 2024-04-27 20:26:40.306387 pyodide_mkdocs_theme-1.1.2/pyodide_mkdocs_theme/pyodide_macros/macros/autres.py
+-rw-r--r--   0        0        0    17204 2024-05-27 09:57:27.861116 pyodide_mkdocs_theme-1.1.2/pyodide_mkdocs_theme/pyodide_macros/macros/ide_files_data.py
+-rw-r--r--   0        0        0    13843 2024-06-01 14:49:35.212120 pyodide_mkdocs_theme-1.1.2/pyodide_mkdocs_theme/pyodide_macros/macros/ide_ide.py
+-rw-r--r--   0        0        0    19389 2024-06-01 14:49:35.220121 pyodide_mkdocs_theme-1.1.2/pyodide_mkdocs_theme/pyodide_macros/macros/ide_manager.py
+-rw-r--r--   0        0        0     4972 2024-05-27 09:57:27.861116 pyodide_mkdocs_theme-1.1.2/pyodide_mkdocs_theme/pyodide_macros/macros/ide_pybtn.py
+-rw-r--r--   0        0        0     3460 2024-05-27 09:57:27.861116 pyodide_mkdocs_theme-1.1.2/pyodide_mkdocs_theme/pyodide_macros/macros/ide_terminal.py
+-rw-r--r--   0        0        0     2435 2024-05-15 21:11:56.389101 pyodide_mkdocs_theme-1.1.2/pyodide_mkdocs_theme/pyodide_macros/macros/isolated_components.py
+-rw-r--r--   0        0        0    11591 2024-05-30 18:15:00.841773 pyodide_mkdocs_theme-1.1.2/pyodide_mkdocs_theme/pyodide_macros/macros/qcm.py
+-rw-r--r--   0        0        0    14303 2024-06-01 14:49:35.220121 pyodide_mkdocs_theme-1.1.2/pyodide_mkdocs_theme/pyodide_macros/messages.py
+-rw-r--r--   0        0        0     7422 2024-05-27 09:57:27.861116 pyodide_mkdocs_theme-1.1.2/pyodide_mkdocs_theme/pyodide_macros/pages_and_ides_configs.py
+-rw-r--r--   0        0        0    16144 2024-06-03 06:54:52.461032 pyodide_mkdocs_theme-1.1.2/pyodide_mkdocs_theme/pyodide_macros/parsing.py
+-rw-r--r--   0        0        0     4776 2024-05-15 21:11:56.421101 pyodide_mkdocs_theme-1.1.2/pyodide_mkdocs_theme/pyodide_macros/paths_utils.py
+-rw-r--r--   0        0        0        0 2024-05-15 21:11:56.421101 pyodide_mkdocs_theme-1.1.2/pyodide_mkdocs_theme/pyodide_macros/plugin/__init__.py
+-rw-r--r--   0        0        0    15211 2024-05-15 21:11:56.421101 pyodide_mkdocs_theme-1.1.2/pyodide_mkdocs_theme/pyodide_macros/plugin/config.py
+-rw-r--r--   0        0        0    11391 2024-05-25 09:20:37.108858 pyodide_mkdocs_theme-1.1.2/pyodide_mkdocs_theme/pyodide_macros/plugin/maestro_IDE.py
+-rw-r--r--   0        0        0     9979 2024-06-03 15:11:29.513885 pyodide_mkdocs_theme-1.1.2/pyodide_mkdocs_theme/pyodide_macros/plugin/maestro_base.py
+-rw-r--r--   0        0        0     1603 2024-05-15 21:11:56.425101 pyodide_mkdocs_theme-1.1.2/pyodide_mkdocs_theme/pyodide_macros/plugin/maestro_extras.py
+-rw-r--r--   0        0        0     6765 2024-06-03 15:11:29.521885 pyodide_mkdocs_theme-1.1.2/pyodide_mkdocs_theme/pyodide_macros/plugin/maestro_indent.py
+-rw-r--r--   0        0        0     2877 2024-04-24 20:11:56.666105 pyodide_mkdocs_theme-1.1.2/pyodide_mkdocs_theme/pyodide_macros/plugin/maestro_tools.py
+-rw-r--r--   0        0        0     9272 2024-06-01 14:49:35.220121 pyodide_mkdocs_theme-1.1.2/pyodide_mkdocs_theme/pyodide_macros/plugin/pyodide_macros_plugin.py
+-rw-r--r--   0        0        0     2658 2024-04-11 09:41:00.023938 pyodide_mkdocs_theme-1.1.2/pyodide_mkdocs_theme/pyodide_macros/pyodide_logger.py
+-rw-r--r--   0        0        0     1163 2024-05-15 21:11:56.425101 pyodide_mkdocs_theme-1.1.2/pyodide_mkdocs_theme/pyodide_macros/scripts_templates.py
+-rw-r--r--   0        0        0     9846 2024-05-27 09:57:27.865116 pyodide_mkdocs_theme-1.1.2/pyodide_mkdocs_theme/pyodide_macros/tools_and_constants.py
+-rw-r--r--   0        0        0     3739 2024-06-03 15:14:11.545658 pyodide_mkdocs_theme-1.1.2/pyodide_mkdocs_theme/scripts/custom_lang.py
+-rw-r--r--   0        0        0     4776 2024-05-27 09:57:27.865116 pyodide_mkdocs_theme-1.1.2/pyodide_mkdocs_theme/scripts/mkdocs.yml
+-rw-r--r--   0        0        0     2902 2024-05-27 09:57:27.865116 pyodide_mkdocs_theme-1.1.2/pyodide_mkdocs_theme/scripts/model.py
+-rw-r--r--   0        0        0      823 2024-05-15 21:11:56.425101 pyodide_mkdocs_theme-1.1.2/pyodide_mkdocs_theme/templates/README.md
+-rw-r--r--   0        0        0        0 2024-05-15 21:11:56.425101 pyodide_mkdocs_theme-1.1.2/pyodide_mkdocs_theme/templates/__init__.py
+-rw-r--r--   0        0        0     2857 2024-05-15 21:11:56.425101 pyodide_mkdocs_theme-1.1.2/pyodide_mkdocs_theme/templates/assets/images/.qcm-circle.svg
+-rw-r--r--   0        0        0     1645 2024-05-15 21:11:56.425101 pyodide_mkdocs_theme-1.1.2/pyodide_mkdocs_theme/templates/assets/images/icons8-check-64.png
+-rw-r--r--   0        0        0     1328 2024-05-15 21:11:56.425101 pyodide_mkdocs_theme-1.1.2/pyodide_mkdocs_theme/templates/assets/images/icons8-download-64.png
+-rw-r--r--   0        0        0     1761 2024-05-15 21:11:56.425101 pyodide_mkdocs_theme-1.1.2/pyodide_mkdocs_theme/templates/assets/images/icons8-play-64.png
+-rw-r--r--   0        0        0     1283 2024-05-15 21:11:56.425101 pyodide_mkdocs_theme-1.1.2/pyodide_mkdocs_theme/templates/assets/images/icons8-restart-64.png
+-rw-r--r--   0        0        0      952 2024-05-15 21:11:56.429102 pyodide_mkdocs_theme-1.1.2/pyodide_mkdocs_theme/templates/assets/images/icons8-save-64.png
+-rw-r--r--   0        0        0     1296 2024-05-15 21:11:56.429102 pyodide_mkdocs_theme-1.1.2/pyodide_mkdocs_theme/templates/assets/images/icons8-upload-64.png
+-rw-r--r--   0        0        0        0 2024-05-16 21:25:14.310769 pyodide_mkdocs_theme-1.1.2/pyodide_mkdocs_theme/templates/hooks/libsAfter.html
+-rw-r--r--   0        0        0        0 2024-05-16 21:25:14.310769 pyodide_mkdocs_theme-1.1.2/pyodide_mkdocs_theme/templates/hooks/libsBefore.html
+-rw-r--r--   0        0        0        0 2024-05-16 21:25:14.310769 pyodide_mkdocs_theme-1.1.2/pyodide_mkdocs_theme/templates/hooks/scriptsAfter.html
+-rw-r--r--   0        0        0        0 2024-05-16 21:25:14.310769 pyodide_mkdocs_theme-1.1.2/pyodide_mkdocs_theme/templates/hooks/scriptsBefore.html
+-rw-r--r--   0        0        0     6152 2024-06-01 14:49:35.220121 pyodide_mkdocs_theme-1.1.2/pyodide_mkdocs_theme/templates/js-libs/0_config-libs.js
+-rw-r--r--   0        0        0    14903 2024-06-01 14:49:35.220121 pyodide_mkdocs_theme-1.1.2/pyodide_mkdocs_theme/templates/js-libs/functools-libs.js
+-rw-r--r--   0        0        0     1770 2024-06-03 15:14:08.685592 pyodide_mkdocs_theme-1.1.2/pyodide_mkdocs_theme/templates/js-libs/jsLogger-libs.js
+-rw-r--r--   0        0        0     1490 2024-04-09 19:35:36.230493 pyodide_mkdocs_theme-1.1.2/pyodide_mkdocs_theme/templates/js-libs/mathjax-libs.js
+-rw-r--r--   0        0        0     4361 2024-04-29 14:09:33.373857 pyodide_mkdocs_theme-1.1.2/pyodide_mkdocs_theme/templates/js-libs/z_globalGuiButtons-libs.js
+-rw-r--r--   0        0        0    13514 2024-06-01 14:49:35.220121 pyodide_mkdocs_theme-1.1.2/pyodide_mkdocs_theme/templates/js-per-pages/0_genericPythonSnippets-pyodide.js
+-rw-r--r--   0        0        0    15301 2024-05-27 09:57:27.865116 pyodide_mkdocs_theme-1.1.2/pyodide_mkdocs_theme/templates/js-per-pages/1_pyodideSectionsRunner-pyodide.js
+-rw-r--r--   0        0        0     1157 2024-05-27 09:57:27.865116 pyodide_mkdocs_theme-1.1.2/pyodide_mkdocs_theme/templates/js-per-pages/2_btnRunner-pyodide.js
+-rw-r--r--   0        0        0     9294 2024-06-01 14:49:35.220121 pyodide_mkdocs_theme-1.1.2/pyodide_mkdocs_theme/templates/js-per-pages/2_terminalRunner-terms.js
+-rw-r--r--   0        0        0    17299 2024-06-01 14:49:35.220121 pyodide_mkdocs_theme-1.1.2/pyodide_mkdocs_theme/templates/js-per-pages/3_ideRunner-ides.js
+-rw-r--r--   0        0        0    12716 2024-05-15 21:11:56.437102 pyodide_mkdocs_theme-1.1.2/pyodide_mkdocs_theme/templates/js-per-pages/qcms-qcm.js
+-rw-r--r--   0        0        0     7237 2024-05-27 09:57:27.869116 pyodide_mkdocs_theme-1.1.2/pyodide_mkdocs_theme/templates/js-per-pages/start-pyodide.js
+-rw-r--r--   0        0        0    11534 2024-06-03 15:12:10.114833 pyodide_mkdocs_theme-1.1.2/pyodide_mkdocs_theme/templates/js-scripts/error-logs-generator-scripts.js
+-rw-r--r--   0        0        0     4455 2024-05-15 21:11:56.489103 pyodide_mkdocs_theme-1.1.2/pyodide_mkdocs_theme/templates/js-scripts/z_doLast-subscriptions-scripts.js
+-rw-r--r--   0        0        0     5341 2024-05-15 21:11:56.505103 pyodide_mkdocs_theme-1.1.2/pyodide_mkdocs_theme/templates/main.html
+-rw-r--r--   0        0        0     2635 2024-05-15 21:11:56.505103 pyodide_mkdocs_theme-1.1.2/pyodide_mkdocs_theme/templates/mkdocs_theme.yml
+-rw-r--r--   0        0        0      802 2024-04-03 22:13:32.135114 pyodide_mkdocs_theme-1.1.2/pyodide_mkdocs_theme/templates/partials/copyright.html
+-rw-r--r--   0        0        0     2084 2024-04-03 21:47:24.620870 pyodide_mkdocs_theme-1.1.2/pyodide_mkdocs_theme/templates/partials/footer.html
+-rw-r--r--   0        0        0      578 2024-04-03 22:14:08.956199 pyodide_mkdocs_theme-1.1.2/pyodide_mkdocs_theme/templates/partials/social.html
+-rw-r--r--   0        0        0     3831 2024-05-15 21:11:56.517104 pyodide_mkdocs_theme-1.1.2/pyodide_mkdocs_theme/templates/pyodide-css/0_generic-tooltips-libs.css
+-rw-r--r--   0        0        0     1078 2024-05-15 21:11:56.517104 pyodide_mkdocs_theme-1.1.2/pyodide_mkdocs_theme/templates/pyodide-css/header-btns-libs.css
+-rw-r--r--   0        0        0     1947 2024-05-15 21:11:56.517104 pyodide_mkdocs_theme-1.1.2/pyodide_mkdocs_theme/templates/pyodide-css/hourglass-libs.css
+-rw-r--r--   0        0        0     3764 2024-05-16 18:56:03.284304 pyodide_mkdocs_theme-1.1.2/pyodide_mkdocs_theme/templates/pyodide-css/ide-libs.css
+-rw-r--r--   0        0        0     3904 2024-05-15 21:11:56.525104 pyodide_mkdocs_theme-1.1.2/pyodide_mkdocs_theme/templates/pyodide-css/qcm-libs.css
+-rw-r--r--   0        0        0     1918 2024-05-15 21:11:56.525104 pyodide_mkdocs_theme-1.1.2/pyodide_mkdocs_theme/templates/pyodide-css/terminal-libs.css
+-rw-r--r--   0        0        0     1766 2024-06-03 15:14:08.737593 pyodide_mkdocs_theme-1.1.2/pyproject.toml
+-rw-r--r--   0        0        0     2864 1970-01-01 00:00:00.000000 pyodide_mkdocs_theme-1.1.2/PKG-INFO
```

### Comparing `pyodide_mkdocs_theme-1.1.1/LICENSE` & `pyodide_mkdocs_theme-1.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-1.1.1/README.md` & `pyodide_mkdocs_theme-1.1.2/README.md`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-1.1.1/pyodide_mkdocs_theme/__init__.py` & `pyodide_mkdocs_theme-1.1.2/pyodide_mkdocs_theme/__init__.py`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-1.1.1/pyodide_mkdocs_theme/__main__.py` & `pyodide_mkdocs_theme-1.1.2/pyodide_mkdocs_theme/__main__.py`

 * *Files 1% similar despite different names*

```diff
@@ -35,29 +35,29 @@
     epilog = "Copyleft GNU GPLv3 🄯 2024 Frédéric Zinelli. "
              "This program comes with ABSOLUTELY NO WARRANTY."
 )
 parser.add_argument(
     '-V', '--version', action='version', version=f'pyodide-mkdocs-theme {__version__}'
 )
 parser.add_argument(
-    '--lang', action='store_true', help='Print the base python code to customize some messages.'
+    '--lang', action='store_true', help='Print the base python code to customize some messages'
 )
 parser.add_argument(
-    '--mime', action='store_true', help='Open a page in the browser, to the MDN documentation about MIME types.'
+    '--mime', action='store_true', help='Open a page in the browser, to the MDN documentation about MIME types'
 )
 parser.add_argument(
-    '--py', action='store_true', help='Print an example of python file, for {{IDE(...)}} or {{terminal(...)}} macros.'
+    '--py', action='store_true', help='Print an example of python file, for {{IDE(...)}} or {{terminal(...)}} macros'
 )
 parser.add_argument(
-    '--yml', action='store_true', help='Print a base configuration for the mkdocs.yml file.'
+    '--yml', action='store_true', help='Print a base configuration for the mkdocs.yml file'
 )
 parser.add_argument(
     '-F', '--file', default="",
     help='Use this argument to write the information into a file instead of the stdout '
-         '(existing content will be overridden. Use an absolute path or relative to cwd).'
+         '(existing content will be overridden. Use an absolute path or a path relative to the cwd)'
 )
 
 
 
 def main():
     # pylint: disable=multiple-statements
```

### Comparing `pyodide_mkdocs_theme-1.1.1/pyodide_mkdocs_theme/pyodide_macros/__init__.py` & `pyodide_mkdocs_theme-1.1.2/pyodide_mkdocs_theme/pyodide_macros/__init__.py`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-1.1.1/pyodide_mkdocs_theme/pyodide_macros/deprecation.py` & `pyodide_mkdocs_theme-1.1.2/pyodide_mkdocs_theme/pyodide_macros/deprecation.py`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-1.1.1/pyodide_mkdocs_theme/pyodide_macros/exceptions.py` & `pyodide_mkdocs_theme-1.1.2/pyodide_mkdocs_theme/pyodide_macros/exceptions.py`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-1.1.1/pyodide_mkdocs_theme/pyodide_macros/html_builder/__init__.py` & `pyodide_mkdocs_theme-1.1.2/pyodide_mkdocs_theme/pyodide_macros/html_builder/__init__.py`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-1.1.1/pyodide_mkdocs_theme/pyodide_macros/html_builder/_html_builder.py` & `pyodide_mkdocs_theme-1.1.2/pyodide_mkdocs_theme/pyodide_macros/html_builder/_html_builder.py`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-1.1.1/pyodide_mkdocs_theme/pyodide_macros/macros/IDEs.py` & `pyodide_mkdocs_theme-1.1.2/pyodide_mkdocs_theme/pyodide_macros/macros/IDEs.py`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-1.1.1/pyodide_mkdocs_theme/pyodide_macros/macros/autres.py` & `pyodide_mkdocs_theme-1.1.2/pyodide_mkdocs_theme/pyodide_macros/macros/autres.py`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-1.1.1/pyodide_mkdocs_theme/pyodide_macros/macros/ide_files_data.py` & `pyodide_mkdocs_theme-1.1.2/pyodide_mkdocs_theme/pyodide_macros/macros/ide_files_data.py`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-1.1.1/pyodide_mkdocs_theme/pyodide_macros/macros/ide_ide.py` & `pyodide_mkdocs_theme-1.1.2/pyodide_mkdocs_theme/pyodide_macros/macros/ide_ide.py`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-1.1.1/pyodide_mkdocs_theme/pyodide_macros/macros/ide_manager.py` & `pyodide_mkdocs_theme-1.1.2/pyodide_mkdocs_theme/pyodide_macros/macros/ide_manager.py`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-1.1.1/pyodide_mkdocs_theme/pyodide_macros/macros/ide_pybtn.py` & `pyodide_mkdocs_theme-1.1.2/pyodide_mkdocs_theme/pyodide_macros/macros/ide_pybtn.py`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-1.1.1/pyodide_mkdocs_theme/pyodide_macros/macros/ide_terminal.py` & `pyodide_mkdocs_theme-1.1.2/pyodide_mkdocs_theme/pyodide_macros/macros/ide_terminal.py`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-1.1.1/pyodide_mkdocs_theme/pyodide_macros/macros/isolated_components.py` & `pyodide_mkdocs_theme-1.1.2/pyodide_mkdocs_theme/pyodide_macros/macros/isolated_components.py`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-1.1.1/pyodide_mkdocs_theme/pyodide_macros/macros/qcm.py` & `pyodide_mkdocs_theme-1.1.2/pyodide_mkdocs_theme/pyodide_macros/macros/qcm.py`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-1.1.1/pyodide_mkdocs_theme/pyodide_macros/messages.py` & `pyodide_mkdocs_theme-1.1.2/pyodide_mkdocs_theme/pyodide_macros/messages.py`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-1.1.1/pyodide_mkdocs_theme/pyodide_macros/pages_and_ides_configs.py` & `pyodide_mkdocs_theme-1.1.2/pyodide_mkdocs_theme/pyodide_macros/pages_and_ides_configs.py`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-1.1.1/pyodide_mkdocs_theme/pyodide_macros/parsing.py` & `pyodide_mkdocs_theme-1.1.2/pyodide_mkdocs_theme/pyodide_macros/parsing.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,17 +15,16 @@
 You should have received a copy of the GNU General Public License
 along with this program.
 If not, see <https://www.gnu.org/licenses/>.
 """
 
 
 import re
-from pathlib import Path
+# from pathlib import Path
 from typing import Callable, List, Optional
-from string import printable
 from random import shuffle
 from functools import lru_cache
 
 from mkdocs.exceptions import BuildError
 
 from .exceptions import PyodideMacrosParsingError
 from .tools_and_constants import LZW_DELIMITER, DebugConfig
```

### Comparing `pyodide_mkdocs_theme-1.1.1/pyodide_mkdocs_theme/pyodide_macros/paths_utils.py` & `pyodide_mkdocs_theme-1.1.2/pyodide_mkdocs_theme/pyodide_macros/paths_utils.py`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-1.1.1/pyodide_mkdocs_theme/pyodide_macros/plugin/config.py` & `pyodide_mkdocs_theme-1.1.2/pyodide_mkdocs_theme/pyodide_macros/plugin/config.py`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-1.1.1/pyodide_mkdocs_theme/pyodide_macros/plugin/maestro_IDE.py` & `pyodide_mkdocs_theme-1.1.2/pyodide_mkdocs_theme/pyodide_macros/plugin/maestro_IDE.py`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-1.1.1/pyodide_mkdocs_theme/pyodide_macros/plugin/maestro_base.py` & `pyodide_mkdocs_theme-1.1.2/pyodide_mkdocs_theme/pyodide_macros/plugin/maestro_base.py`

 * *Files 9% similar despite different names*

```diff
@@ -61,42 +61,49 @@
     It is also used as "sink" for the super calls of other classes that are not implemented
     on the MacrosPlugin class.
 
     Note that, for the ConfigExtractor for to properly work, the class hierarchy has to
     extend MacrosPlugin at some point.
     """
 
+    # bypass_indent_errors:                  bool = ConfigExtractor('build')
+    # check_python_files:                    bool = ConfigExtractor('build')
+    # soft_check:                            bool = ConfigExtractor('build')
+
     ignore_macros_plugin_diffs:              bool = ConfigExtractor('build')
     skip_py_md_paths_names_validation:       bool = ConfigExtractor('build')
     load_yaml_encoding:                      str  = ConfigExtractor('build')
     macros_with_indents:                List[str] = ConfigExtractor('build')
-    encrypt_corrections_and_rems:            bool = ConfigExtractor('build')
-    forbid_secrets_without_corr_or_REMs:     bool = ConfigExtractor('build')
-    forbid_hidden_corr_and_REMs_without_secrets: bool = ConfigExtractor('build')
-    forbid_corr_and_REMs_with_infinite_attempts: bool = ConfigExtractor('build')
     python_libs:                        List[str] = ConfigExtractor('build')
-    # bypass_indent_errors:                  bool = ConfigExtractor('build')
-    # check_python_files:                    bool = ConfigExtractor('build')
-    # soft_check:                            bool = ConfigExtractor('build')
 
-    show_assertion_code_on_failed_test:      bool = ConfigExtractor("ides")
-    max_attempts_before_corr_available:      bool = ConfigExtractor("ides")
-    decrease_attempts_on_user_code_failure:  bool = ConfigExtractor("ides")
-    default_ide_height_lines:                 int = ConfigExtractor("ides")
-    deactivate_stdout_for_secrets: Optional[bool] = ConfigExtractor("ides")
-    show_only_assertion_errors_for_secrets: Optional[bool] = ConfigExtractor("ides")
-
-    default_height_ide_term:              int = ConfigExtractor("terms")
-    default_height_isolated_term:             int = ConfigExtractor("terms")
-    stdout_cut_off:                           int = ConfigExtractor("terms")
+    encrypt_corrections_and_rems:            bool = ConfigExtractor('build')        # meta
+    forbid_secrets_without_corr_or_REMs:     bool = ConfigExtractor('build')        # meta
+    forbid_hidden_corr_and_REMs_without_secrets: bool = ConfigExtractor('build')    # meta
+    forbid_corr_and_REMs_with_infinite_attempts: bool = ConfigExtractor('build')    # meta
+
+
+    show_assertion_code_on_failed_test:      bool = ConfigExtractor("ides")         # meta
+    decrease_attempts_on_user_code_failure:  bool = ConfigExtractor("ides")         # meta
+    deactivate_stdout_for_secrets: Optional[bool] = ConfigExtractor("ides")         # meta
+    show_only_assertion_errors_for_secrets: Optional[bool] = ConfigExtractor("ides")# meta
+
+    max_attempts_before_corr_available:      bool = ConfigExtractor("ides")         # arg
+    default_ide_height_lines:                 int = ConfigExtractor("ides")         # arg
+
+
+    stdout_cut_off:                           int = ConfigExtractor("terms")        # meta
+
+    default_height_ide_term:                  int = ConfigExtractor("terms")        # arg
+    default_height_isolated_term:             int = ConfigExtractor("terms")        # arg
+
 
+    hide:    Optional[bool] = ConfigExtractor("qcms")                               # arg
+    multi:   Optional[bool] = ConfigExtractor("qcms")                               # arg
+    shuffle: Optional[bool] = ConfigExtractor("qcms")                               # arg
 
-    hide:    Optional[bool] = ConfigExtractor("qcms")
-    multi:   Optional[bool] = ConfigExtractor("qcms")
-    shuffle: Optional[bool] = ConfigExtractor("qcms")
 
     _dev_mode:               bool = ConfigExtractor()
     j2_block_start_string:    str = ConfigExtractor()
     j2_block_end_string:      str = ConfigExtractor()
     j2_variable_start_string: str = ConfigExtractor()
     j2_variable_end_string:   str = ConfigExtractor()
```

### Comparing `pyodide_mkdocs_theme-1.1.1/pyodide_mkdocs_theme/pyodide_macros/plugin/maestro_extras.py` & `pyodide_mkdocs_theme-1.1.2/pyodide_mkdocs_theme/pyodide_macros/plugin/maestro_extras.py`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-1.1.1/pyodide_mkdocs_theme/pyodide_macros/plugin/maestro_indent.py` & `pyodide_mkdocs_theme-1.1.2/pyodide_mkdocs_theme/pyodide_macros/plugin/maestro_indent.py`

 * *Files 12% similar despite different names*

```diff
@@ -15,40 +15,39 @@
 You should have received a copy of the GNU General Public License
 along with this program.
 If not, see <https://www.gnu.org/licenses/>.
 """
 
 
 import re
-from typing import Dict, List, Optional, Tuple
+from typing import List, Optional, Tuple
 from functools import wraps
 
 
 from mkdocs.config.defaults import MkDocsConfig
 from mkdocs.structure.pages import Page
 from mkdocs.exceptions import BuildError
 
 
 from ..exceptions import PyodideConfigurationError
 from ..tools_and_constants import MACROS_WITH_INDENT
-from ..pyodide_logger import logger
 from ..deprecation import deprecation_warning
 from ..parsing import IndentParser
 from .maestro_base import BaseMaestro
 
 
 
 # pylint: disable-next=pointless-string-statement, line-too-long
 '''
 - Macros are run in "reading order" of the original document, included content also being use this way => fully predictable
 - WARNING with md_include, which interleave other calls in the "current context"... => need an external md page parser
 - Process:
     1. remove raw markers. NOTE: nested raw markups aren't allowed => easy
     2. tokenize (longest tokens first)
-    3. _carefully parse the thing... _ keeping in mind that the input is md text, not actual python...
+    3. _carefully parse the thing, _keeping in mind that the input is md text, not actual python_...
        and store the indents of the calls to multiline macros in a reversed stack (store a pari indent/macro name,
        to enforce validity of executions on usage)
     4. each time a macro starts running (spotted through the custom macro decorator), pop the current indent to use,
        AND STACK IT , because of potential nested macro calls: A(BCD) => when going back to A, there is no way
        to know if the macro will reach for the indentation value of A, for example.
        Each time the macro returns, pop the current indent from the second stack
     5. for nested macro, add the included indentation data on top of the current reversed stack
@@ -60,31 +59,31 @@
 
 
 
 class MaestroIndent(BaseMaestro):
     """ Manage Indentation logistic """
 
 
-    # _pages_indents: 'PageIndents'
-    # """
-    # Cache storing the indentations for each jinja/macro template in a Page.
-    # A page is entirely studied the first time it's seen and the result of the indentation levels
-    # are stored.
-    # The data stays correct throughout the md->html conversion because the indentation levels
-    # "horizontal") are not affected by the content growing ("vertical").
-    # """
-
     _running_macro: Optional[str] = None
     """
     Name of the macro currently running (or the last one called. None if no macro called yet).
     """
 
     _parser: IndentParser
+
     _indents_store: List[Tuple[str,int]]
+    """ List of all indentations for the "macro with indents" calls throughout the page, in
+        reading order (=dfs).
+        Data are stored in reversed fashion, because consumed using `list.pop()`.
+    """
     _indents_stack: List[str]
+    """ Stack the current indentation level to use, the last element being the current one.
+        This allows the use of macros through multi layered inclusions (see `md_include`),
+        getting back the correct indentations when "stepping out" of the included content.
+    """
 
 
     def on_config(self, config:MkDocsConfig):
 
         nope = [ w for w in self.macros_with_indents if not w.isidentifier() ]
         if nope:
             raise PyodideConfigurationError(
@@ -115,27 +114,30 @@
         site_navigation=None,
         **kwargs
     ):
         indentations = self._parser.parse(markdown, self.location(page))
         self._indents_store = [*reversed(indentations)]
         self._indents_stack = []
 
-        return super().on_page_markdown( markdown, page, config, site_navigation=site_navigation, **kwargs)
+        return super().on_page_markdown(
+            markdown, page, config, site_navigation=site_navigation, **kwargs
+        )
 
 
 
     #----------------------------------------------------------------------------
 
 
 
     # Override MacroPlugin
     def macro(self, func, name=""):     # pylint: disable=arguments-renamed
         """
         Add an extra wrapper around the macro, so that it gathers automatically the name of
         the macro currently running (for better error messages).
+        Also validate the call config for macros with indents
         """
         name = name or func.__name__
 
         @wraps(func)
         def wrapper(*a,**kw):
             self._running_macro = name
             need_indent = self.is_macro_with_indent(name)
```

### Comparing `pyodide_mkdocs_theme-1.1.1/pyodide_mkdocs_theme/pyodide_macros/plugin/maestro_tools.py` & `pyodide_mkdocs_theme-1.1.2/pyodide_mkdocs_theme/pyodide_macros/plugin/maestro_tools.py`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-1.1.1/pyodide_mkdocs_theme/pyodide_macros/plugin/pyodide_macros_plugin.py` & `pyodide_mkdocs_theme-1.1.2/pyodide_mkdocs_theme/pyodide_macros/plugin/pyodide_macros_plugin.py`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-1.1.1/pyodide_mkdocs_theme/pyodide_macros/pyodide_logger.py` & `pyodide_mkdocs_theme-1.1.2/pyodide_mkdocs_theme/pyodide_macros/pyodide_logger.py`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-1.1.1/pyodide_mkdocs_theme/pyodide_macros/scripts_templates.py` & `pyodide_mkdocs_theme-1.1.2/pyodide_mkdocs_theme/pyodide_macros/scripts_templates.py`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-1.1.1/pyodide_mkdocs_theme/pyodide_macros/tools_and_constants.py` & `pyodide_mkdocs_theme-1.1.2/pyodide_mkdocs_theme/pyodide_macros/tools_and_constants.py`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-1.1.1/pyodide_mkdocs_theme/scripts/custom_lang.py` & `pyodide_mkdocs_theme-1.1.2/pyodide_mkdocs_theme/scripts/custom_lang.py`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-1.1.1/pyodide_mkdocs_theme/scripts/mkdocs.yml` & `pyodide_mkdocs_theme-1.1.2/pyodide_mkdocs_theme/scripts/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-1.1.1/pyodide_mkdocs_theme/scripts/model.py` & `pyodide_mkdocs_theme-1.1.2/pyodide_mkdocs_theme/scripts/model.py`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-1.1.1/pyodide_mkdocs_theme/templates/README.md` & `pyodide_mkdocs_theme-1.1.2/pyodide_mkdocs_theme/templates/README.md`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-1.1.1/pyodide_mkdocs_theme/templates/assets/images/.qcm-circle.svg` & `pyodide_mkdocs_theme-1.1.2/pyodide_mkdocs_theme/templates/assets/images/.qcm-circle.svg`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-1.1.1/pyodide_mkdocs_theme/templates/assets/images/icons8-check-64.png` & `pyodide_mkdocs_theme-1.1.2/pyodide_mkdocs_theme/templates/assets/images/icons8-check-64.png`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-1.1.1/pyodide_mkdocs_theme/templates/assets/images/icons8-download-64.png` & `pyodide_mkdocs_theme-1.1.2/pyodide_mkdocs_theme/templates/assets/images/icons8-download-64.png`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-1.1.1/pyodide_mkdocs_theme/templates/assets/images/icons8-play-64.png` & `pyodide_mkdocs_theme-1.1.2/pyodide_mkdocs_theme/templates/assets/images/icons8-play-64.png`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-1.1.1/pyodide_mkdocs_theme/templates/assets/images/icons8-restart-64.png` & `pyodide_mkdocs_theme-1.1.2/pyodide_mkdocs_theme/templates/assets/images/icons8-restart-64.png`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-1.1.1/pyodide_mkdocs_theme/templates/assets/images/icons8-save-64.png` & `pyodide_mkdocs_theme-1.1.2/pyodide_mkdocs_theme/templates/assets/images/icons8-save-64.png`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-1.1.1/pyodide_mkdocs_theme/templates/assets/images/icons8-upload-64.png` & `pyodide_mkdocs_theme-1.1.2/pyodide_mkdocs_theme/templates/assets/images/icons8-upload-64.png`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-1.1.1/pyodide_mkdocs_theme/templates/js-libs/0_config-libs.js` & `pyodide_mkdocs_theme-1.1.2/pyodide_mkdocs_theme/templates/js-libs/0_config-libs.js`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-1.1.1/pyodide_mkdocs_theme/templates/js-libs/functools-libs.js` & `pyodide_mkdocs_theme-1.1.2/pyodide_mkdocs_theme/templates/js-libs/functools-libs.js`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-1.1.1/pyodide_mkdocs_theme/templates/js-libs/jsLogger-libs.js` & `pyodide_mkdocs_theme-1.1.2/pyodide_mkdocs_theme/templates/js-libs/jsLogger-libs.js`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-1.1.1/pyodide_mkdocs_theme/templates/js-libs/mathjax-libs.js` & `pyodide_mkdocs_theme-1.1.2/pyodide_mkdocs_theme/templates/js-libs/mathjax-libs.js`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-1.1.1/pyodide_mkdocs_theme/templates/js-libs/z_globalGuiButtons-libs.js` & `pyodide_mkdocs_theme-1.1.2/pyodide_mkdocs_theme/templates/js-libs/z_globalGuiButtons-libs.js`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-1.1.1/pyodide_mkdocs_theme/templates/js-per-pages/0_genericPythonSnippets-pyodide.js` & `pyodide_mkdocs_theme-1.1.2/pyodide_mkdocs_theme/templates/js-per-pages/0_genericPythonSnippets-pyodide.js`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-1.1.1/pyodide_mkdocs_theme/templates/js-per-pages/1_pyodideSectionsRunner-pyodide.js` & `pyodide_mkdocs_theme-1.1.2/pyodide_mkdocs_theme/templates/js-per-pages/1_pyodideSectionsRunner-pyodide.js`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-1.1.1/pyodide_mkdocs_theme/templates/js-per-pages/2_btnRunner-pyodide.js` & `pyodide_mkdocs_theme-1.1.2/pyodide_mkdocs_theme/templates/js-per-pages/2_btnRunner-pyodide.js`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-1.1.1/pyodide_mkdocs_theme/templates/js-per-pages/2_terminalRunner-terms.js` & `pyodide_mkdocs_theme-1.1.2/pyodide_mkdocs_theme/templates/js-per-pages/2_terminalRunner-terms.js`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-1.1.1/pyodide_mkdocs_theme/templates/js-per-pages/3_ideRunner-ides.js` & `pyodide_mkdocs_theme-1.1.2/pyodide_mkdocs_theme/templates/js-per-pages/3_ideRunner-ides.js`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-1.1.1/pyodide_mkdocs_theme/templates/js-per-pages/qcms-qcm.js` & `pyodide_mkdocs_theme-1.1.2/pyodide_mkdocs_theme/templates/js-per-pages/qcms-qcm.js`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-1.1.1/pyodide_mkdocs_theme/templates/js-per-pages/start-pyodide.js` & `pyodide_mkdocs_theme-1.1.2/pyodide_mkdocs_theme/templates/js-per-pages/start-pyodide.js`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-1.1.1/pyodide_mkdocs_theme/templates/js-scripts/error-logs-generator-scripts.js` & `pyodide_mkdocs_theme-1.1.2/pyodide_mkdocs_theme/templates/js-scripts/error-logs-generator-scripts.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -268,15 +268,15 @@
 Couldn't determine the line number of the assertion in:
       ${ callLine }
     Error message:\n${ errLines.join('\n') }`)
     }
 
     // The double quotes are all escaped to make sure no multiline string in the code
     // can cause troubles.
-    const escapedCode = code.replace(/"/g, '\\"').replace(/\\/g, '\\\\')
+    const escapedCode = code.replace(/\\/g, '\\\\').replace(/"/g, '\\"')
     const lineNo = +numMatch[1]
     const astExplorer = `
 
 def _hack_1():
     import ast
     code = """${ escapedCode }"""
     tree = ast.parse(code)
```

### Comparing `pyodide_mkdocs_theme-1.1.1/pyodide_mkdocs_theme/templates/js-scripts/z_doLast-subscriptions-scripts.js` & `pyodide_mkdocs_theme-1.1.2/pyodide_mkdocs_theme/templates/js-scripts/z_doLast-subscriptions-scripts.js`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-1.1.1/pyodide_mkdocs_theme/templates/main.html` & `pyodide_mkdocs_theme-1.1.2/pyodide_mkdocs_theme/templates/main.html`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-1.1.1/pyodide_mkdocs_theme/templates/mkdocs_theme.yml` & `pyodide_mkdocs_theme-1.1.2/pyodide_mkdocs_theme/templates/mkdocs_theme.yml`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-1.1.1/pyodide_mkdocs_theme/templates/partials/copyright.html` & `pyodide_mkdocs_theme-1.1.2/pyodide_mkdocs_theme/templates/partials/copyright.html`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-1.1.1/pyodide_mkdocs_theme/templates/partials/footer.html` & `pyodide_mkdocs_theme-1.1.2/pyodide_mkdocs_theme/templates/partials/footer.html`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-1.1.1/pyodide_mkdocs_theme/templates/partials/social.html` & `pyodide_mkdocs_theme-1.1.2/pyodide_mkdocs_theme/templates/partials/social.html`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-1.1.1/pyodide_mkdocs_theme/templates/pyodide-css/0_generic-tooltips-libs.css` & `pyodide_mkdocs_theme-1.1.2/pyodide_mkdocs_theme/templates/pyodide-css/0_generic-tooltips-libs.css`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-1.1.1/pyodide_mkdocs_theme/templates/pyodide-css/header-btns-libs.css` & `pyodide_mkdocs_theme-1.1.2/pyodide_mkdocs_theme/templates/pyodide-css/header-btns-libs.css`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-1.1.1/pyodide_mkdocs_theme/templates/pyodide-css/hourglass-libs.css` & `pyodide_mkdocs_theme-1.1.2/pyodide_mkdocs_theme/templates/pyodide-css/hourglass-libs.css`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-1.1.1/pyodide_mkdocs_theme/templates/pyodide-css/ide-libs.css` & `pyodide_mkdocs_theme-1.1.2/pyodide_mkdocs_theme/templates/pyodide-css/ide-libs.css`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-1.1.1/pyodide_mkdocs_theme/templates/pyodide-css/qcm-libs.css` & `pyodide_mkdocs_theme-1.1.2/pyodide_mkdocs_theme/templates/pyodide-css/qcm-libs.css`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-1.1.1/pyodide_mkdocs_theme/templates/pyodide-css/terminal-libs.css` & `pyodide_mkdocs_theme-1.1.2/pyodide_mkdocs_theme/templates/pyodide-css/terminal-libs.css`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-1.1.1/pyproject.toml` & `pyodide_mkdocs_theme-1.1.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pyodide-mkdocs-theme"
-version = "1.1.1"
+version = "1.1.2"
 description = "Package embedding the necessary tools to host pyodide, ACE editors, jQuery terminals in mkdocs documentations"
 authors = ["Frédéric Zinelli <frederic.zinelli@gmail.com>"]
 readme = "README.md"
 keywords = [
     "mkdocs", "mkdocs-plugin", "pyodide", "IDE", "terminal"
 ]
 classifiers = [
```

### Comparing `pyodide_mkdocs_theme-1.1.1/PKG-INFO` & `pyodide_mkdocs_theme-1.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyodide-mkdocs-theme
-Version: 1.1.1
+Version: 1.1.2
 Summary: Package embedding the necessary tools to host pyodide, ACE editors, jQuery terminals in mkdocs documentations
 Keywords: mkdocs,mkdocs-plugin,pyodide,IDE,terminal
 Author: Frédéric Zinelli
 Author-email: frederic.zinelli@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Plugins
```

