# Comparing `tmp/docs2kg-0.1.3.tar.gz` & `tmp/docs2kg-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "docs2kg-0.1.3.tar", last modified: Mon Jun  3 11:05:23 2024, max compression
+gzip compressed data, was "docs2kg-0.1.6.tar", last modified: Mon Jun  3 11:17:49 2024, max compression
```

## Comparing `docs2kg-0.1.3.tar` & `docs2kg-0.1.6.tar`

### file list

```diff
@@ -1,122 +1,122 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 11:05:23.322534 docs2kg-0.1.3/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 11:05:23.306534 docs2kg-0.1.3/Docs2KG/
--rw-r--r--   0 runner    (1001) docker     (127)       61 2024-06-03 11:05:15.000000 docs2kg-0.1.3/Docs2KG/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 11:05:23.310534 docs2kg-0.1.3/Docs2KG/kg/
--rw-r--r--   0 runner    (1001) docker     (127)      873 2024-06-03 11:05:15.000000 docs2kg-0.1.3/Docs2KG/kg/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5447 2024-06-03 11:05:15.000000 docs2kg-0.1.3/Docs2KG/kg/docs_linkage.py
--rw-r--r--   0 runner    (1001) docker     (127)     6269 2024-06-03 11:05:15.000000 docs2kg-0.1.3/Docs2KG/kg/email_layout_kg.py
--rw-r--r--   0 runner    (1001) docker     (127)     5538 2024-06-03 11:05:15.000000 docs2kg-0.1.3/Docs2KG/kg/excel_layout_kg.py
--rw-r--r--   0 runner    (1001) docker     (127)    22047 2024-06-03 11:05:15.000000 docs2kg-0.1.3/Docs2KG/kg/pdf_layout_kg.py
--rw-r--r--   0 runner    (1001) docker     (127)    20174 2024-06-03 11:05:15.000000 docs2kg-0.1.3/Docs2KG/kg/semantic_kg.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 11:05:23.310534 docs2kg-0.1.3/Docs2KG/kg/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 11:05:15.000000 docs2kg-0.1.3/Docs2KG/kg/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    15156 2024-06-03 11:05:15.000000 docs2kg-0.1.3/Docs2KG/kg/utils/json2triplets.py
--rw-r--r--   0 runner    (1001) docker     (127)     5398 2024-06-03 11:05:15.000000 docs2kg-0.1.3/Docs2KG/kg/utils/neo4j_connector.py
--rw-r--r--   0 runner    (1001) docker     (127)     6275 2024-06-03 11:05:15.000000 docs2kg-0.1.3/Docs2KG/kg/web_layout_kg.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 11:05:23.310534 docs2kg-0.1.3/Docs2KG/modules/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 11:05:15.000000 docs2kg-0.1.3/Docs2KG/modules/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 11:05:23.310534 docs2kg-0.1.3/Docs2KG/modules/llm/
--rw-r--r--   0 runner    (1001) docker     (127)      398 2024-06-03 11:05:15.000000 docs2kg-0.1.3/Docs2KG/modules/llm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      399 2024-06-03 11:05:15.000000 docs2kg-0.1.3/Docs2KG/modules/llm/image2description.py
--rw-r--r--   0 runner    (1001) docker     (127)    13124 2024-06-03 11:05:15.000000 docs2kg-0.1.3/Docs2KG/modules/llm/markdown2json.py
--rw-r--r--   0 runner    (1001) docker     (127)     1664 2024-06-03 11:05:15.000000 docs2kg-0.1.3/Docs2KG/modules/llm/openai_call.py
--rw-r--r--   0 runner    (1001) docker     (127)     4444 2024-06-03 11:05:15.000000 docs2kg-0.1.3/Docs2KG/modules/llm/sheet2metadata.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 11:05:23.310534 docs2kg-0.1.3/Docs2KG/modules/native/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 11:05:15.000000 docs2kg-0.1.3/Docs2KG/modules/native/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2896 2024-06-03 11:05:15.000000 docs2kg-0.1.3/Docs2KG/modules/native/markdown2json.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 11:05:23.310534 docs2kg-0.1.3/Docs2KG/parser/
--rw-r--r--   0 runner    (1001) docker     (127)      522 2024-06-03 11:05:15.000000 docs2kg-0.1.3/Docs2KG/parser/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 11:05:23.310534 docs2kg-0.1.3/Docs2KG/parser/email/
--rw-r--r--   0 runner    (1001) docker     (127)      228 2024-06-03 11:05:15.000000 docs2kg-0.1.3/Docs2KG/parser/email/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      797 2024-06-03 11:05:15.000000 docs2kg-0.1.3/Docs2KG/parser/email/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     4765 2024-06-03 11:05:15.000000 docs2kg-0.1.3/Docs2KG/parser/email/email_compose.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 11:05:23.310534 docs2kg-0.1.3/Docs2KG/parser/email/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 11:05:15.000000 docs2kg-0.1.3/Docs2KG/parser/email/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4850 2024-06-03 11:05:15.000000 docs2kg-0.1.3/Docs2KG/parser/email/utils/email_connector.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 11:05:23.310534 docs2kg-0.1.3/Docs2KG/parser/excel/
--rw-r--r--   0 runner    (1001) docker     (127)      170 2024-06-03 11:05:15.000000 docs2kg-0.1.3/Docs2KG/parser/excel/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2136 2024-06-03 11:05:15.000000 docs2kg-0.1.3/Docs2KG/parser/excel/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     2072 2024-06-03 11:05:15.000000 docs2kg-0.1.3/Docs2KG/parser/excel/excel2image.py
--rw-r--r--   0 runner    (1001) docker     (127)     1095 2024-06-03 11:05:15.000000 docs2kg-0.1.3/Docs2KG/parser/excel/excel2markdown.py
--rw-r--r--   0 runner    (1001) docker     (127)     2405 2024-06-03 11:05:15.000000 docs2kg-0.1.3/Docs2KG/parser/excel/excel2table.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 11:05:23.314534 docs2kg-0.1.3/Docs2KG/parser/pdf/
--rw-r--r--   0 runner    (1001) docker     (127)      477 2024-06-03 11:05:15.000000 docs2kg-0.1.3/Docs2KG/parser/pdf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1541 2024-06-03 11:05:15.000000 docs2kg-0.1.3/Docs2KG/parser/pdf/base.py
--rw-r--r--   0 runner    (1001) docker     (127)      430 2024-06-03 11:05:15.000000 docs2kg-0.1.3/Docs2KG/parser/pdf/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     3145 2024-06-03 11:05:15.000000 docs2kg-0.1.3/Docs2KG/parser/pdf/pdf2blocks.py
--rw-r--r--   0 runner    (1001) docker     (127)     1649 2024-06-03 11:05:15.000000 docs2kg-0.1.3/Docs2KG/parser/pdf/pdf2image.py
--rw-r--r--   0 runner    (1001) docker     (127)     5264 2024-06-03 11:05:15.000000 docs2kg-0.1.3/Docs2KG/parser/pdf/pdf2metadata.py
--rw-r--r--   0 runner    (1001) docker     (127)     2133 2024-06-03 11:05:15.000000 docs2kg-0.1.3/Docs2KG/parser/pdf/pdf2tables.py
--rw-r--r--   0 runner    (1001) docker     (127)     2765 2024-06-03 11:05:15.000000 docs2kg-0.1.3/Docs2KG/parser/pdf/pdf2text.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 11:05:23.314534 docs2kg-0.1.3/Docs2KG/parser/web/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 11:05:15.000000 docs2kg-0.1.3/Docs2KG/parser/web/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1507 2024-06-03 11:05:15.000000 docs2kg-0.1.3/Docs2KG/parser/web/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     1250 2024-06-03 11:05:15.000000 docs2kg-0.1.3/Docs2KG/parser/web/web2images.py
--rw-r--r--   0 runner    (1001) docker     (127)      811 2024-06-03 11:05:15.000000 docs2kg-0.1.3/Docs2KG/parser/web/web2markdown.py
--rw-r--r--   0 runner    (1001) docker     (127)     1281 2024-06-03 11:05:15.000000 docs2kg-0.1.3/Docs2KG/parser/web/web2tables.py
--rw-r--r--   0 runner    (1001) docker     (127)     1006 2024-06-03 11:05:15.000000 docs2kg-0.1.3/Docs2KG/parser/web/web2urls.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 11:05:23.314534 docs2kg-0.1.3/Docs2KG/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 11:05:15.000000 docs2kg-0.1.3/Docs2KG/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      484 2024-06-03 11:05:15.000000 docs2kg-0.1.3/Docs2KG/utils/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)      155 2024-06-03 11:05:15.000000 docs2kg-0.1.3/Docs2KG/utils/empty_check.py
--rw-r--r--   0 runner    (1001) docker     (127)      917 2024-06-03 11:05:15.000000 docs2kg-0.1.3/Docs2KG/utils/get_logger.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 11:05:23.314534 docs2kg-0.1.3/Docs2KG/utils/llm/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 11:05:15.000000 docs2kg-0.1.3/Docs2KG/utils/llm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1167 2024-06-03 11:05:15.000000 docs2kg-0.1.3/Docs2KG/utils/llm/count_tokens.py
--rw-r--r--   0 runner    (1001) docker     (127)     1021 2024-06-03 11:05:15.000000 docs2kg-0.1.3/Docs2KG/utils/llm/estimate_price.py
--rw-r--r--   0 runner    (1001) docker     (127)     1728 2024-06-03 11:05:15.000000 docs2kg-0.1.3/Docs2KG/utils/llm/track_usage.py
--rw-r--r--   0 runner    (1001) docker     (127)     7360 2024-06-03 11:05:15.000000 docs2kg-0.1.3/Docs2KG/utils/rect.py
--rw-r--r--   0 runner    (1001) docker     (127)      946 2024-06-03 11:05:15.000000 docs2kg-0.1.3/Docs2KG/utils/timer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 11:05:23.322534 docs2kg-0.1.3/Docs2KG.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3394 2024-06-03 11:05:23.000000 docs2kg-0.1.3/Docs2KG.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2849 2024-06-03 11:05:23.000000 docs2kg-0.1.3/Docs2KG.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-03 11:05:23.000000 docs2kg-0.1.3/Docs2KG.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      179 2024-06-03 11:05:23.000000 docs2kg-0.1.3/Docs2KG.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-06-03 11:05:23.000000 docs2kg-0.1.3/Docs2KG.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)    26526 2024-06-03 11:05:15.000000 docs2kg-0.1.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3394 2024-06-03 11:05:23.322534 docs2kg-0.1.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2120 2024-06-03 11:05:15.000000 docs2kg-0.1.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 11:05:23.318534 docs2kg-0.1.3/examples/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 11:05:15.000000 docs2kg-0.1.3/examples/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 11:05:23.318534 docs2kg-0.1.3/examples/demo/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 11:05:15.000000 docs2kg-0.1.3/examples/demo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1232 2024-06-03 11:05:15.000000 docs2kg-0.1.3/examples/demo/emails.py
--rw-r--r--   0 runner    (1001) docker     (127)     2067 2024-06-03 11:05:15.000000 docs2kg-0.1.3/examples/demo/excel.py
--rw-r--r--   0 runner    (1001) docker     (127)     5367 2024-06-03 11:05:15.000000 docs2kg-0.1.3/examples/demo/pdf_exported.py
--rw-r--r--   0 runner    (1001) docker     (127)     5709 2024-06-03 11:05:15.000000 docs2kg-0.1.3/examples/demo/pdf_scanned.py
--rw-r--r--   0 runner    (1001) docker     (127)     1194 2024-06-03 11:05:15.000000 docs2kg-0.1.3/examples/demo/web.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 11:05:23.318534 docs2kg-0.1.3/examples/kg/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 11:05:15.000000 docs2kg-0.1.3/examples/kg/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      942 2024-06-03 11:05:15.000000 docs2kg-0.1.3/examples/kg/docs_linkage.py
--rw-r--r--   0 runner    (1001) docker     (127)      243 2024-06-03 11:05:15.000000 docs2kg-0.1.3/examples/kg/layout_kg.py
--rw-r--r--   0 runner    (1001) docker     (127)      267 2024-06-03 11:05:15.000000 docs2kg-0.1.3/examples/kg/semantic_kg.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 11:05:23.318534 docs2kg-0.1.3/examples/kg/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 11:05:15.000000 docs2kg-0.1.3/examples/kg/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      253 2024-06-03 11:05:15.000000 docs2kg-0.1.3/examples/kg/utils/json2triplets.py
--rw-r--r--   0 runner    (1001) docker     (127)      978 2024-06-03 11:05:15.000000 docs2kg-0.1.3/examples/kg/utils/neo4j_connector.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 11:05:23.318534 docs2kg-0.1.3/examples/modules/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 11:05:15.000000 docs2kg-0.1.3/examples/modules/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      353 2024-06-03 11:05:15.000000 docs2kg-0.1.3/examples/modules/markdown_clean_md.py
--rw-r--r--   0 runner    (1001) docker     (127)      351 2024-06-03 11:05:15.000000 docs2kg-0.1.3/examples/modules/markdown_json.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 11:05:23.318534 docs2kg-0.1.3/examples/parser/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 11:05:15.000000 docs2kg-0.1.3/examples/parser/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 11:05:23.318534 docs2kg-0.1.3/examples/parser/email/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 11:05:15.000000 docs2kg-0.1.3/examples/parser/email/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      279 2024-06-03 11:05:15.000000 docs2kg-0.1.3/examples/parser/email/email_process.py
--rw-r--r--   0 runner    (1001) docker     (127)      481 2024-06-03 11:05:15.000000 docs2kg-0.1.3/examples/parser/email/email_pull.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 11:05:23.318534 docs2kg-0.1.3/examples/parser/excel/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 11:05:15.000000 docs2kg-0.1.3/examples/parser/excel/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      602 2024-06-03 11:05:15.000000 docs2kg-0.1.3/examples/parser/excel/excel_process.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 11:05:23.322534 docs2kg-0.1.3/examples/parser/pdf/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 11:05:15.000000 docs2kg-0.1.3/examples/parser/pdf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1265 2024-06-03 11:05:15.000000 docs2kg-0.1.3/examples/parser/pdf/pdf_metadata_summary.py
--rw-r--r--   0 runner    (1001) docker     (127)     1315 2024-06-03 11:05:15.000000 docs2kg-0.1.3/examples/parser/pdf/pdf_process.py
--rw-r--r--   0 runner    (1001) docker     (127)     1283 2024-06-03 11:05:15.000000 docs2kg-0.1.3/examples/parser/pdf/pdf_scanned_process.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 11:05:23.322534 docs2kg-0.1.3/examples/parser/web/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 11:05:15.000000 docs2kg-0.1.3/examples/parser/web/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      603 2024-06-03 11:05:15.000000 docs2kg-0.1.3/examples/parser/web/web_process.py
--rw-r--r--   0 runner    (1001) docker     (127)      201 2024-06-03 11:05:15.000000 docs2kg-0.1.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      215 2024-06-03 11:05:23.322534 docs2kg-0.1.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2287 2024-06-03 11:05:15.000000 docs2kg-0.1.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 11:05:23.322534 docs2kg-0.1.3/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 11:05:15.000000 docs2kg-0.1.3/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 11:17:49.568599 docs2kg-0.1.6/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 11:17:49.552599 docs2kg-0.1.6/Docs2KG/
+-rw-r--r--   0 runner    (1001) docker     (127)       61 2024-06-03 11:17:41.000000 docs2kg-0.1.6/Docs2KG/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 11:17:49.556599 docs2kg-0.1.6/Docs2KG/kg/
+-rw-r--r--   0 runner    (1001) docker     (127)      873 2024-06-03 11:17:41.000000 docs2kg-0.1.6/Docs2KG/kg/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5447 2024-06-03 11:17:41.000000 docs2kg-0.1.6/Docs2KG/kg/docs_linkage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6269 2024-06-03 11:17:41.000000 docs2kg-0.1.6/Docs2KG/kg/email_layout_kg.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5538 2024-06-03 11:17:41.000000 docs2kg-0.1.6/Docs2KG/kg/excel_layout_kg.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22047 2024-06-03 11:17:41.000000 docs2kg-0.1.6/Docs2KG/kg/pdf_layout_kg.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20174 2024-06-03 11:17:41.000000 docs2kg-0.1.6/Docs2KG/kg/semantic_kg.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 11:17:49.556599 docs2kg-0.1.6/Docs2KG/kg/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 11:17:41.000000 docs2kg-0.1.6/Docs2KG/kg/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15156 2024-06-03 11:17:41.000000 docs2kg-0.1.6/Docs2KG/kg/utils/json2triplets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5398 2024-06-03 11:17:41.000000 docs2kg-0.1.6/Docs2KG/kg/utils/neo4j_connector.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6275 2024-06-03 11:17:41.000000 docs2kg-0.1.6/Docs2KG/kg/web_layout_kg.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 11:17:49.556599 docs2kg-0.1.6/Docs2KG/modules/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 11:17:41.000000 docs2kg-0.1.6/Docs2KG/modules/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 11:17:49.556599 docs2kg-0.1.6/Docs2KG/modules/llm/
+-rw-r--r--   0 runner    (1001) docker     (127)      398 2024-06-03 11:17:41.000000 docs2kg-0.1.6/Docs2KG/modules/llm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      399 2024-06-03 11:17:41.000000 docs2kg-0.1.6/Docs2KG/modules/llm/image2description.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13124 2024-06-03 11:17:41.000000 docs2kg-0.1.6/Docs2KG/modules/llm/markdown2json.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1664 2024-06-03 11:17:41.000000 docs2kg-0.1.6/Docs2KG/modules/llm/openai_call.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4444 2024-06-03 11:17:41.000000 docs2kg-0.1.6/Docs2KG/modules/llm/sheet2metadata.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 11:17:49.556599 docs2kg-0.1.6/Docs2KG/modules/native/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 11:17:41.000000 docs2kg-0.1.6/Docs2KG/modules/native/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2896 2024-06-03 11:17:41.000000 docs2kg-0.1.6/Docs2KG/modules/native/markdown2json.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 11:17:49.556599 docs2kg-0.1.6/Docs2KG/parser/
+-rw-r--r--   0 runner    (1001) docker     (127)      522 2024-06-03 11:17:41.000000 docs2kg-0.1.6/Docs2KG/parser/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 11:17:49.556599 docs2kg-0.1.6/Docs2KG/parser/email/
+-rw-r--r--   0 runner    (1001) docker     (127)      228 2024-06-03 11:17:41.000000 docs2kg-0.1.6/Docs2KG/parser/email/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      797 2024-06-03 11:17:41.000000 docs2kg-0.1.6/Docs2KG/parser/email/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4765 2024-06-03 11:17:41.000000 docs2kg-0.1.6/Docs2KG/parser/email/email_compose.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 11:17:49.556599 docs2kg-0.1.6/Docs2KG/parser/email/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 11:17:41.000000 docs2kg-0.1.6/Docs2KG/parser/email/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4850 2024-06-03 11:17:41.000000 docs2kg-0.1.6/Docs2KG/parser/email/utils/email_connector.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 11:17:49.560599 docs2kg-0.1.6/Docs2KG/parser/excel/
+-rw-r--r--   0 runner    (1001) docker     (127)      170 2024-06-03 11:17:41.000000 docs2kg-0.1.6/Docs2KG/parser/excel/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2136 2024-06-03 11:17:41.000000 docs2kg-0.1.6/Docs2KG/parser/excel/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2072 2024-06-03 11:17:41.000000 docs2kg-0.1.6/Docs2KG/parser/excel/excel2image.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1095 2024-06-03 11:17:41.000000 docs2kg-0.1.6/Docs2KG/parser/excel/excel2markdown.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2405 2024-06-03 11:17:41.000000 docs2kg-0.1.6/Docs2KG/parser/excel/excel2table.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 11:17:49.560599 docs2kg-0.1.6/Docs2KG/parser/pdf/
+-rw-r--r--   0 runner    (1001) docker     (127)      477 2024-06-03 11:17:41.000000 docs2kg-0.1.6/Docs2KG/parser/pdf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1541 2024-06-03 11:17:41.000000 docs2kg-0.1.6/Docs2KG/parser/pdf/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)      430 2024-06-03 11:17:41.000000 docs2kg-0.1.6/Docs2KG/parser/pdf/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3145 2024-06-03 11:17:41.000000 docs2kg-0.1.6/Docs2KG/parser/pdf/pdf2blocks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1649 2024-06-03 11:17:41.000000 docs2kg-0.1.6/Docs2KG/parser/pdf/pdf2image.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5264 2024-06-03 11:17:41.000000 docs2kg-0.1.6/Docs2KG/parser/pdf/pdf2metadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2133 2024-06-03 11:17:41.000000 docs2kg-0.1.6/Docs2KG/parser/pdf/pdf2tables.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2765 2024-06-03 11:17:41.000000 docs2kg-0.1.6/Docs2KG/parser/pdf/pdf2text.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 11:17:49.560599 docs2kg-0.1.6/Docs2KG/parser/web/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 11:17:41.000000 docs2kg-0.1.6/Docs2KG/parser/web/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1507 2024-06-03 11:17:41.000000 docs2kg-0.1.6/Docs2KG/parser/web/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1250 2024-06-03 11:17:41.000000 docs2kg-0.1.6/Docs2KG/parser/web/web2images.py
+-rw-r--r--   0 runner    (1001) docker     (127)      811 2024-06-03 11:17:41.000000 docs2kg-0.1.6/Docs2KG/parser/web/web2markdown.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1281 2024-06-03 11:17:41.000000 docs2kg-0.1.6/Docs2KG/parser/web/web2tables.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1006 2024-06-03 11:17:41.000000 docs2kg-0.1.6/Docs2KG/parser/web/web2urls.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 11:17:49.560599 docs2kg-0.1.6/Docs2KG/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 11:17:41.000000 docs2kg-0.1.6/Docs2KG/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      484 2024-06-03 11:17:41.000000 docs2kg-0.1.6/Docs2KG/utils/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)      155 2024-06-03 11:17:41.000000 docs2kg-0.1.6/Docs2KG/utils/empty_check.py
+-rw-r--r--   0 runner    (1001) docker     (127)      917 2024-06-03 11:17:41.000000 docs2kg-0.1.6/Docs2KG/utils/get_logger.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 11:17:49.560599 docs2kg-0.1.6/Docs2KG/utils/llm/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 11:17:41.000000 docs2kg-0.1.6/Docs2KG/utils/llm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1167 2024-06-03 11:17:41.000000 docs2kg-0.1.6/Docs2KG/utils/llm/count_tokens.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1021 2024-06-03 11:17:41.000000 docs2kg-0.1.6/Docs2KG/utils/llm/estimate_price.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1728 2024-06-03 11:17:41.000000 docs2kg-0.1.6/Docs2KG/utils/llm/track_usage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7360 2024-06-03 11:17:41.000000 docs2kg-0.1.6/Docs2KG/utils/rect.py
+-rw-r--r--   0 runner    (1001) docker     (127)      946 2024-06-03 11:17:41.000000 docs2kg-0.1.6/Docs2KG/utils/timer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 11:17:49.568599 docs2kg-0.1.6/Docs2KG.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3515 2024-06-03 11:17:49.000000 docs2kg-0.1.6/Docs2KG.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2849 2024-06-03 11:17:49.000000 docs2kg-0.1.6/Docs2KG.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-03 11:17:49.000000 docs2kg-0.1.6/Docs2KG.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      179 2024-06-03 11:17:49.000000 docs2kg-0.1.6/Docs2KG.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-06-03 11:17:49.000000 docs2kg-0.1.6/Docs2KG.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    26526 2024-06-03 11:17:41.000000 docs2kg-0.1.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3515 2024-06-03 11:17:49.568599 docs2kg-0.1.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2120 2024-06-03 11:17:41.000000 docs2kg-0.1.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 11:17:49.564599 docs2kg-0.1.6/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 11:17:41.000000 docs2kg-0.1.6/examples/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 11:17:49.564599 docs2kg-0.1.6/examples/demo/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 11:17:41.000000 docs2kg-0.1.6/examples/demo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1232 2024-06-03 11:17:41.000000 docs2kg-0.1.6/examples/demo/emails.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2067 2024-06-03 11:17:41.000000 docs2kg-0.1.6/examples/demo/excel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5367 2024-06-03 11:17:41.000000 docs2kg-0.1.6/examples/demo/pdf_exported.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5709 2024-06-03 11:17:41.000000 docs2kg-0.1.6/examples/demo/pdf_scanned.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1194 2024-06-03 11:17:41.000000 docs2kg-0.1.6/examples/demo/web.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 11:17:49.564599 docs2kg-0.1.6/examples/kg/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 11:17:41.000000 docs2kg-0.1.6/examples/kg/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      942 2024-06-03 11:17:41.000000 docs2kg-0.1.6/examples/kg/docs_linkage.py
+-rw-r--r--   0 runner    (1001) docker     (127)      243 2024-06-03 11:17:41.000000 docs2kg-0.1.6/examples/kg/layout_kg.py
+-rw-r--r--   0 runner    (1001) docker     (127)      267 2024-06-03 11:17:41.000000 docs2kg-0.1.6/examples/kg/semantic_kg.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 11:17:49.564599 docs2kg-0.1.6/examples/kg/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 11:17:41.000000 docs2kg-0.1.6/examples/kg/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      253 2024-06-03 11:17:41.000000 docs2kg-0.1.6/examples/kg/utils/json2triplets.py
+-rw-r--r--   0 runner    (1001) docker     (127)      978 2024-06-03 11:17:41.000000 docs2kg-0.1.6/examples/kg/utils/neo4j_connector.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 11:17:49.564599 docs2kg-0.1.6/examples/modules/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 11:17:41.000000 docs2kg-0.1.6/examples/modules/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      353 2024-06-03 11:17:41.000000 docs2kg-0.1.6/examples/modules/markdown_clean_md.py
+-rw-r--r--   0 runner    (1001) docker     (127)      351 2024-06-03 11:17:41.000000 docs2kg-0.1.6/examples/modules/markdown_json.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 11:17:49.564599 docs2kg-0.1.6/examples/parser/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 11:17:41.000000 docs2kg-0.1.6/examples/parser/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 11:17:49.564599 docs2kg-0.1.6/examples/parser/email/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 11:17:41.000000 docs2kg-0.1.6/examples/parser/email/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      279 2024-06-03 11:17:41.000000 docs2kg-0.1.6/examples/parser/email/email_process.py
+-rw-r--r--   0 runner    (1001) docker     (127)      481 2024-06-03 11:17:41.000000 docs2kg-0.1.6/examples/parser/email/email_pull.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 11:17:49.564599 docs2kg-0.1.6/examples/parser/excel/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 11:17:41.000000 docs2kg-0.1.6/examples/parser/excel/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      602 2024-06-03 11:17:41.000000 docs2kg-0.1.6/examples/parser/excel/excel_process.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 11:17:49.564599 docs2kg-0.1.6/examples/parser/pdf/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 11:17:41.000000 docs2kg-0.1.6/examples/parser/pdf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1265 2024-06-03 11:17:41.000000 docs2kg-0.1.6/examples/parser/pdf/pdf_metadata_summary.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1315 2024-06-03 11:17:41.000000 docs2kg-0.1.6/examples/parser/pdf/pdf_process.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1283 2024-06-03 11:17:41.000000 docs2kg-0.1.6/examples/parser/pdf/pdf_scanned_process.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 11:17:49.568599 docs2kg-0.1.6/examples/parser/web/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 11:17:41.000000 docs2kg-0.1.6/examples/parser/web/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      603 2024-06-03 11:17:41.000000 docs2kg-0.1.6/examples/parser/web/web_process.py
+-rw-r--r--   0 runner    (1001) docker     (127)      201 2024-06-03 11:17:41.000000 docs2kg-0.1.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      215 2024-06-03 11:17:49.568599 docs2kg-0.1.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2168 2024-06-03 11:17:41.000000 docs2kg-0.1.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 11:17:49.568599 docs2kg-0.1.6/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 11:17:41.000000 docs2kg-0.1.6/tests/__init__.py
```

### Comparing `docs2kg-0.1.3/Docs2KG/kg/__init__.py` & `docs2kg-0.1.6/Docs2KG/kg/__init__.py`

 * *Files identical despite different names*

### Comparing `docs2kg-0.1.3/Docs2KG/kg/docs_linkage.py` & `docs2kg-0.1.6/Docs2KG/kg/docs_linkage.py`

 * *Files identical despite different names*

### Comparing `docs2kg-0.1.3/Docs2KG/kg/email_layout_kg.py` & `docs2kg-0.1.6/Docs2KG/kg/email_layout_kg.py`

 * *Files identical despite different names*

### Comparing `docs2kg-0.1.3/Docs2KG/kg/excel_layout_kg.py` & `docs2kg-0.1.6/Docs2KG/kg/excel_layout_kg.py`

 * *Files identical despite different names*

### Comparing `docs2kg-0.1.3/Docs2KG/kg/pdf_layout_kg.py` & `docs2kg-0.1.6/Docs2KG/kg/pdf_layout_kg.py`

 * *Files identical despite different names*

### Comparing `docs2kg-0.1.3/Docs2KG/kg/semantic_kg.py` & `docs2kg-0.1.6/Docs2KG/kg/semantic_kg.py`

 * *Files identical despite different names*

### Comparing `docs2kg-0.1.3/Docs2KG/kg/utils/json2triplets.py` & `docs2kg-0.1.6/Docs2KG/kg/utils/json2triplets.py`

 * *Files identical despite different names*

### Comparing `docs2kg-0.1.3/Docs2KG/kg/utils/neo4j_connector.py` & `docs2kg-0.1.6/Docs2KG/kg/utils/neo4j_connector.py`

 * *Files identical despite different names*

### Comparing `docs2kg-0.1.3/Docs2KG/kg/web_layout_kg.py` & `docs2kg-0.1.6/Docs2KG/kg/web_layout_kg.py`

 * *Files identical despite different names*

### Comparing `docs2kg-0.1.3/Docs2KG/modules/llm/markdown2json.py` & `docs2kg-0.1.6/Docs2KG/modules/llm/markdown2json.py`

 * *Files identical despite different names*

### Comparing `docs2kg-0.1.3/Docs2KG/modules/llm/openai_call.py` & `docs2kg-0.1.6/Docs2KG/modules/llm/openai_call.py`

 * *Files identical despite different names*

### Comparing `docs2kg-0.1.3/Docs2KG/modules/llm/sheet2metadata.py` & `docs2kg-0.1.6/Docs2KG/modules/llm/sheet2metadata.py`

 * *Files identical despite different names*

### Comparing `docs2kg-0.1.3/Docs2KG/modules/native/markdown2json.py` & `docs2kg-0.1.6/Docs2KG/modules/native/markdown2json.py`

 * *Files identical despite different names*

### Comparing `docs2kg-0.1.3/Docs2KG/parser/__init__.py` & `docs2kg-0.1.6/Docs2KG/parser/__init__.py`

 * *Files identical despite different names*

### Comparing `docs2kg-0.1.3/Docs2KG/parser/email/base.py` & `docs2kg-0.1.6/Docs2KG/parser/email/base.py`

 * *Files identical despite different names*

### Comparing `docs2kg-0.1.3/Docs2KG/parser/email/email_compose.py` & `docs2kg-0.1.6/Docs2KG/parser/email/email_compose.py`

 * *Files identical despite different names*

### Comparing `docs2kg-0.1.3/Docs2KG/parser/email/utils/email_connector.py` & `docs2kg-0.1.6/Docs2KG/parser/email/utils/email_connector.py`

 * *Files identical despite different names*

### Comparing `docs2kg-0.1.3/Docs2KG/parser/excel/base.py` & `docs2kg-0.1.6/Docs2KG/parser/excel/base.py`

 * *Files identical despite different names*

### Comparing `docs2kg-0.1.3/Docs2KG/parser/excel/excel2image.py` & `docs2kg-0.1.6/Docs2KG/parser/excel/excel2image.py`

 * *Files identical despite different names*

### Comparing `docs2kg-0.1.3/Docs2KG/parser/excel/excel2markdown.py` & `docs2kg-0.1.6/Docs2KG/parser/excel/excel2markdown.py`

 * *Files identical despite different names*

### Comparing `docs2kg-0.1.3/Docs2KG/parser/excel/excel2table.py` & `docs2kg-0.1.6/Docs2KG/parser/excel/excel2table.py`

 * *Files identical despite different names*

### Comparing `docs2kg-0.1.3/Docs2KG/parser/pdf/base.py` & `docs2kg-0.1.6/Docs2KG/parser/pdf/base.py`

 * *Files identical despite different names*

### Comparing `docs2kg-0.1.3/Docs2KG/parser/pdf/pdf2blocks.py` & `docs2kg-0.1.6/Docs2KG/parser/pdf/pdf2blocks.py`

 * *Files identical despite different names*

### Comparing `docs2kg-0.1.3/Docs2KG/parser/pdf/pdf2image.py` & `docs2kg-0.1.6/Docs2KG/parser/pdf/pdf2image.py`

 * *Files identical despite different names*

### Comparing `docs2kg-0.1.3/Docs2KG/parser/pdf/pdf2metadata.py` & `docs2kg-0.1.6/Docs2KG/parser/pdf/pdf2metadata.py`

 * *Files identical despite different names*

### Comparing `docs2kg-0.1.3/Docs2KG/parser/pdf/pdf2tables.py` & `docs2kg-0.1.6/Docs2KG/parser/pdf/pdf2tables.py`

 * *Files identical despite different names*

### Comparing `docs2kg-0.1.3/Docs2KG/parser/pdf/pdf2text.py` & `docs2kg-0.1.6/Docs2KG/parser/pdf/pdf2text.py`

 * *Files identical despite different names*

### Comparing `docs2kg-0.1.3/Docs2KG/parser/web/base.py` & `docs2kg-0.1.6/Docs2KG/parser/web/base.py`

 * *Files identical despite different names*

### Comparing `docs2kg-0.1.3/Docs2KG/parser/web/web2images.py` & `docs2kg-0.1.6/Docs2KG/parser/web/web2images.py`

 * *Files identical despite different names*

### Comparing `docs2kg-0.1.3/Docs2KG/parser/web/web2markdown.py` & `docs2kg-0.1.6/Docs2KG/parser/web/web2markdown.py`

 * *Files identical despite different names*

### Comparing `docs2kg-0.1.3/Docs2KG/parser/web/web2tables.py` & `docs2kg-0.1.6/Docs2KG/parser/web/web2tables.py`

 * *Files identical despite different names*

### Comparing `docs2kg-0.1.3/Docs2KG/parser/web/web2urls.py` & `docs2kg-0.1.6/Docs2KG/parser/web/web2urls.py`

 * *Files identical despite different names*

### Comparing `docs2kg-0.1.3/Docs2KG/utils/get_logger.py` & `docs2kg-0.1.6/Docs2KG/utils/get_logger.py`

 * *Files identical despite different names*

### Comparing `docs2kg-0.1.3/Docs2KG/utils/llm/count_tokens.py` & `docs2kg-0.1.6/Docs2KG/utils/llm/count_tokens.py`

 * *Files identical despite different names*

### Comparing `docs2kg-0.1.3/Docs2KG/utils/llm/estimate_price.py` & `docs2kg-0.1.6/Docs2KG/utils/llm/estimate_price.py`

 * *Files identical despite different names*

### Comparing `docs2kg-0.1.3/Docs2KG/utils/llm/track_usage.py` & `docs2kg-0.1.6/Docs2KG/utils/llm/track_usage.py`

 * *Files identical despite different names*

### Comparing `docs2kg-0.1.3/Docs2KG/utils/rect.py` & `docs2kg-0.1.6/Docs2KG/utils/rect.py`

 * *Files identical despite different names*

### Comparing `docs2kg-0.1.3/Docs2KG/utils/timer.py` & `docs2kg-0.1.6/Docs2KG/utils/timer.py`

 * *Files identical despite different names*

### Comparing `docs2kg-0.1.3/Docs2KG.egg-info/PKG-INFO` & `docs2kg-0.1.6/Docs2KG.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 Metadata-Version: 2.1
 Name: Docs2KG
-Version: 0.1.3
+Version: 0.1.6
 Summary: Unified Knowledge Graph Construction from Heterogeneous Documents Assisted by Large Language Models
 Home-page: https://docs2kg.ai4wa.com
 Author: AI4WA
 Author-email: admin@ai4wa.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
+Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
+Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: pymupdf
```

### Comparing `docs2kg-0.1.3/Docs2KG.egg-info/SOURCES.txt` & `docs2kg-0.1.6/Docs2KG.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `docs2kg-0.1.3/LICENSE` & `docs2kg-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `docs2kg-0.1.3/PKG-INFO` & `docs2kg-0.1.6/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 Metadata-Version: 2.1
 Name: Docs2KG
-Version: 0.1.3
+Version: 0.1.6
 Summary: Unified Knowledge Graph Construction from Heterogeneous Documents Assisted by Large Language Models
 Home-page: https://docs2kg.ai4wa.com
 Author: AI4WA
 Author-email: admin@ai4wa.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
+Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
+Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: pymupdf
```

### Comparing `docs2kg-0.1.3/README.md` & `docs2kg-0.1.6/README.md`

 * *Files identical despite different names*

### Comparing `docs2kg-0.1.3/examples/demo/emails.py` & `docs2kg-0.1.6/examples/demo/emails.py`

 * *Files identical despite different names*

### Comparing `docs2kg-0.1.3/examples/demo/excel.py` & `docs2kg-0.1.6/examples/demo/excel.py`

 * *Files identical despite different names*

### Comparing `docs2kg-0.1.3/examples/demo/pdf_exported.py` & `docs2kg-0.1.6/examples/demo/pdf_exported.py`

 * *Files identical despite different names*

### Comparing `docs2kg-0.1.3/examples/demo/pdf_scanned.py` & `docs2kg-0.1.6/examples/demo/pdf_scanned.py`

 * *Files identical despite different names*

### Comparing `docs2kg-0.1.3/examples/demo/web.py` & `docs2kg-0.1.6/examples/demo/web.py`

 * *Files identical despite different names*

### Comparing `docs2kg-0.1.3/examples/kg/docs_linkage.py` & `docs2kg-0.1.6/examples/kg/docs_linkage.py`

 * *Files identical despite different names*

### Comparing `docs2kg-0.1.3/examples/kg/utils/neo4j_connector.py` & `docs2kg-0.1.6/examples/kg/utils/neo4j_connector.py`

 * *Files identical despite different names*

### Comparing `docs2kg-0.1.3/examples/parser/excel/excel_process.py` & `docs2kg-0.1.6/examples/parser/excel/excel_process.py`

 * *Files identical despite different names*

### Comparing `docs2kg-0.1.3/examples/parser/pdf/pdf_metadata_summary.py` & `docs2kg-0.1.6/examples/parser/pdf/pdf_metadata_summary.py`

 * *Files identical despite different names*

### Comparing `docs2kg-0.1.3/examples/parser/pdf/pdf_process.py` & `docs2kg-0.1.6/examples/parser/pdf/pdf_process.py`

 * *Files identical despite different names*

### Comparing `docs2kg-0.1.3/examples/parser/pdf/pdf_scanned_process.py` & `docs2kg-0.1.6/examples/parser/pdf/pdf_scanned_process.py`

 * *Files identical despite different names*

### Comparing `docs2kg-0.1.3/examples/parser/web/web_process.py` & `docs2kg-0.1.6/examples/parser/web/web_process.py`

 * *Files identical despite different names*

### Comparing `docs2kg-0.1.3/setup.py` & `docs2kg-0.1.6/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -40,19 +40,18 @@
     include_package_data=True,  # To include other types of files specified in MANIFEST.in or found in your packages
     install_requires=read_requirements(),
     python_requires=">=3.8",  # Specify your Python version compatibility
     classifiers=[
         # Classifiers help users find your project by categorizing it
         "Development Status :: 3 - Alpha",
         "Intended Audience :: Developers",
+        "Intended Audience :: Science/Research",
         # license: GNU LESSER GENERAL PUBLIC LICENSE
         "License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)",
+        # topic
+        "Topic :: Scientific/Engineering :: Artificial Intelligence",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
     ],
     url="https://docs2kg.ai4wa.com",
-    # add intended audience
-    intented_audience="Developers, Researchers, Data Scientists, Data Engineers",
-    topic="Knowledge Graph Construction, Large Language Model, "
-    "Machine Learning, Data Engineering, LLM, Retrieval Augmented Generation",
 )
```

