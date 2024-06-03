# Comparing `tmp/docs2kg-0.0.7.tar.gz` & `tmp/docs2kg-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "docs2kg-0.0.7.tar", last modified: Mon Jun  3 10:27:29 2024, max compression
+gzip compressed data, was "docs2kg-0.1.1.tar", last modified: Mon Jun  3 10:03:23 2024, max compression
```

## Comparing `docs2kg-0.0.7.tar` & `docs2kg-0.1.1.tar`

### file list

```diff
@@ -1,122 +1,122 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 10:27:29.151563 docs2kg-0.0.7/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 10:27:29.139563 docs2kg-0.0.7/Docs2KG/
--rw-r--r--   0 runner    (1001) docker     (127)       61 2024-06-03 10:27:21.000000 docs2kg-0.0.7/Docs2KG/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 10:27:29.139563 docs2kg-0.0.7/Docs2KG/kg/
--rw-r--r--   0 runner    (1001) docker     (127)      873 2024-06-03 10:27:21.000000 docs2kg-0.0.7/Docs2KG/kg/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5447 2024-06-03 10:27:21.000000 docs2kg-0.0.7/Docs2KG/kg/docs_linkage.py
--rw-r--r--   0 runner    (1001) docker     (127)     6269 2024-06-03 10:27:21.000000 docs2kg-0.0.7/Docs2KG/kg/email_layout_kg.py
--rw-r--r--   0 runner    (1001) docker     (127)     5538 2024-06-03 10:27:21.000000 docs2kg-0.0.7/Docs2KG/kg/excel_layout_kg.py
--rw-r--r--   0 runner    (1001) docker     (127)    22047 2024-06-03 10:27:21.000000 docs2kg-0.0.7/Docs2KG/kg/pdf_layout_kg.py
--rw-r--r--   0 runner    (1001) docker     (127)    20174 2024-06-03 10:27:21.000000 docs2kg-0.0.7/Docs2KG/kg/semantic_kg.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 10:27:29.139563 docs2kg-0.0.7/Docs2KG/kg/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 10:27:21.000000 docs2kg-0.0.7/Docs2KG/kg/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    15156 2024-06-03 10:27:21.000000 docs2kg-0.0.7/Docs2KG/kg/utils/json2triplets.py
--rw-r--r--   0 runner    (1001) docker     (127)     5398 2024-06-03 10:27:21.000000 docs2kg-0.0.7/Docs2KG/kg/utils/neo4j_connector.py
--rw-r--r--   0 runner    (1001) docker     (127)     6275 2024-06-03 10:27:21.000000 docs2kg-0.0.7/Docs2KG/kg/web_layout_kg.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 10:27:29.139563 docs2kg-0.0.7/Docs2KG/modules/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 10:27:21.000000 docs2kg-0.0.7/Docs2KG/modules/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 10:27:29.143563 docs2kg-0.0.7/Docs2KG/modules/llm/
--rw-r--r--   0 runner    (1001) docker     (127)      398 2024-06-03 10:27:21.000000 docs2kg-0.0.7/Docs2KG/modules/llm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      399 2024-06-03 10:27:21.000000 docs2kg-0.0.7/Docs2KG/modules/llm/image2description.py
--rw-r--r--   0 runner    (1001) docker     (127)    13124 2024-06-03 10:27:21.000000 docs2kg-0.0.7/Docs2KG/modules/llm/markdown2json.py
--rw-r--r--   0 runner    (1001) docker     (127)     1664 2024-06-03 10:27:21.000000 docs2kg-0.0.7/Docs2KG/modules/llm/openai_call.py
--rw-r--r--   0 runner    (1001) docker     (127)     4444 2024-06-03 10:27:21.000000 docs2kg-0.0.7/Docs2KG/modules/llm/sheet2metadata.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 10:27:29.143563 docs2kg-0.0.7/Docs2KG/modules/native/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 10:27:21.000000 docs2kg-0.0.7/Docs2KG/modules/native/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2896 2024-06-03 10:27:21.000000 docs2kg-0.0.7/Docs2KG/modules/native/markdown2json.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 10:27:29.143563 docs2kg-0.0.7/Docs2KG/parser/
--rw-r--r--   0 runner    (1001) docker     (127)      522 2024-06-03 10:27:21.000000 docs2kg-0.0.7/Docs2KG/parser/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 10:27:29.143563 docs2kg-0.0.7/Docs2KG/parser/email/
--rw-r--r--   0 runner    (1001) docker     (127)      228 2024-06-03 10:27:21.000000 docs2kg-0.0.7/Docs2KG/parser/email/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      797 2024-06-03 10:27:21.000000 docs2kg-0.0.7/Docs2KG/parser/email/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     4765 2024-06-03 10:27:21.000000 docs2kg-0.0.7/Docs2KG/parser/email/email_compose.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 10:27:29.143563 docs2kg-0.0.7/Docs2KG/parser/email/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 10:27:21.000000 docs2kg-0.0.7/Docs2KG/parser/email/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4850 2024-06-03 10:27:21.000000 docs2kg-0.0.7/Docs2KG/parser/email/utils/email_connector.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 10:27:29.143563 docs2kg-0.0.7/Docs2KG/parser/excel/
--rw-r--r--   0 runner    (1001) docker     (127)      170 2024-06-03 10:27:21.000000 docs2kg-0.0.7/Docs2KG/parser/excel/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2136 2024-06-03 10:27:21.000000 docs2kg-0.0.7/Docs2KG/parser/excel/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     2072 2024-06-03 10:27:21.000000 docs2kg-0.0.7/Docs2KG/parser/excel/excel2image.py
--rw-r--r--   0 runner    (1001) docker     (127)     1095 2024-06-03 10:27:21.000000 docs2kg-0.0.7/Docs2KG/parser/excel/excel2markdown.py
--rw-r--r--   0 runner    (1001) docker     (127)     2405 2024-06-03 10:27:21.000000 docs2kg-0.0.7/Docs2KG/parser/excel/excel2table.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 10:27:29.147563 docs2kg-0.0.7/Docs2KG/parser/pdf/
--rw-r--r--   0 runner    (1001) docker     (127)      477 2024-06-03 10:27:21.000000 docs2kg-0.0.7/Docs2KG/parser/pdf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1541 2024-06-03 10:27:21.000000 docs2kg-0.0.7/Docs2KG/parser/pdf/base.py
--rw-r--r--   0 runner    (1001) docker     (127)      430 2024-06-03 10:27:21.000000 docs2kg-0.0.7/Docs2KG/parser/pdf/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     3145 2024-06-03 10:27:21.000000 docs2kg-0.0.7/Docs2KG/parser/pdf/pdf2blocks.py
--rw-r--r--   0 runner    (1001) docker     (127)     1649 2024-06-03 10:27:21.000000 docs2kg-0.0.7/Docs2KG/parser/pdf/pdf2image.py
--rw-r--r--   0 runner    (1001) docker     (127)     5264 2024-06-03 10:27:21.000000 docs2kg-0.0.7/Docs2KG/parser/pdf/pdf2metadata.py
--rw-r--r--   0 runner    (1001) docker     (127)     2133 2024-06-03 10:27:21.000000 docs2kg-0.0.7/Docs2KG/parser/pdf/pdf2tables.py
--rw-r--r--   0 runner    (1001) docker     (127)     2765 2024-06-03 10:27:21.000000 docs2kg-0.0.7/Docs2KG/parser/pdf/pdf2text.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 10:27:29.147563 docs2kg-0.0.7/Docs2KG/parser/web/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 10:27:21.000000 docs2kg-0.0.7/Docs2KG/parser/web/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1507 2024-06-03 10:27:21.000000 docs2kg-0.0.7/Docs2KG/parser/web/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     1250 2024-06-03 10:27:21.000000 docs2kg-0.0.7/Docs2KG/parser/web/web2images.py
--rw-r--r--   0 runner    (1001) docker     (127)      811 2024-06-03 10:27:21.000000 docs2kg-0.0.7/Docs2KG/parser/web/web2markdown.py
--rw-r--r--   0 runner    (1001) docker     (127)     1281 2024-06-03 10:27:21.000000 docs2kg-0.0.7/Docs2KG/parser/web/web2tables.py
--rw-r--r--   0 runner    (1001) docker     (127)     1006 2024-06-03 10:27:21.000000 docs2kg-0.0.7/Docs2KG/parser/web/web2urls.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 10:27:29.147563 docs2kg-0.0.7/Docs2KG/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 10:27:21.000000 docs2kg-0.0.7/Docs2KG/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      484 2024-06-03 10:27:21.000000 docs2kg-0.0.7/Docs2KG/utils/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)      155 2024-06-03 10:27:21.000000 docs2kg-0.0.7/Docs2KG/utils/empty_check.py
--rw-r--r--   0 runner    (1001) docker     (127)      917 2024-06-03 10:27:21.000000 docs2kg-0.0.7/Docs2KG/utils/get_logger.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 10:27:29.147563 docs2kg-0.0.7/Docs2KG/utils/llm/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 10:27:21.000000 docs2kg-0.0.7/Docs2KG/utils/llm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1167 2024-06-03 10:27:21.000000 docs2kg-0.0.7/Docs2KG/utils/llm/count_tokens.py
--rw-r--r--   0 runner    (1001) docker     (127)     1021 2024-06-03 10:27:21.000000 docs2kg-0.0.7/Docs2KG/utils/llm/estimate_price.py
--rw-r--r--   0 runner    (1001) docker     (127)     1728 2024-06-03 10:27:21.000000 docs2kg-0.0.7/Docs2KG/utils/llm/track_usage.py
--rw-r--r--   0 runner    (1001) docker     (127)     7360 2024-06-03 10:27:21.000000 docs2kg-0.0.7/Docs2KG/utils/rect.py
--rw-r--r--   0 runner    (1001) docker     (127)      946 2024-06-03 10:27:21.000000 docs2kg-0.0.7/Docs2KG/utils/timer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 10:27:29.151563 docs2kg-0.0.7/Docs2KG.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3536 2024-06-03 10:27:29.000000 docs2kg-0.0.7/Docs2KG.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2849 2024-06-03 10:27:29.000000 docs2kg-0.0.7/Docs2KG.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-03 10:27:29.000000 docs2kg-0.0.7/Docs2KG.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      179 2024-06-03 10:27:29.000000 docs2kg-0.0.7/Docs2KG.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-06-03 10:27:29.000000 docs2kg-0.0.7/Docs2KG.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)    26526 2024-06-03 10:27:21.000000 docs2kg-0.0.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3536 2024-06-03 10:27:29.151563 docs2kg-0.0.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2120 2024-06-03 10:27:21.000000 docs2kg-0.0.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 10:27:29.147563 docs2kg-0.0.7/examples/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 10:27:21.000000 docs2kg-0.0.7/examples/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 10:27:29.147563 docs2kg-0.0.7/examples/demo/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 10:27:21.000000 docs2kg-0.0.7/examples/demo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1232 2024-06-03 10:27:21.000000 docs2kg-0.0.7/examples/demo/emails.py
--rw-r--r--   0 runner    (1001) docker     (127)     2067 2024-06-03 10:27:21.000000 docs2kg-0.0.7/examples/demo/excel.py
--rw-r--r--   0 runner    (1001) docker     (127)     5367 2024-06-03 10:27:21.000000 docs2kg-0.0.7/examples/demo/pdf_exported.py
--rw-r--r--   0 runner    (1001) docker     (127)     5709 2024-06-03 10:27:21.000000 docs2kg-0.0.7/examples/demo/pdf_scanned.py
--rw-r--r--   0 runner    (1001) docker     (127)     1194 2024-06-03 10:27:21.000000 docs2kg-0.0.7/examples/demo/web.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 10:27:29.151563 docs2kg-0.0.7/examples/kg/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 10:27:21.000000 docs2kg-0.0.7/examples/kg/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      942 2024-06-03 10:27:21.000000 docs2kg-0.0.7/examples/kg/docs_linkage.py
--rw-r--r--   0 runner    (1001) docker     (127)      243 2024-06-03 10:27:21.000000 docs2kg-0.0.7/examples/kg/layout_kg.py
--rw-r--r--   0 runner    (1001) docker     (127)      267 2024-06-03 10:27:21.000000 docs2kg-0.0.7/examples/kg/semantic_kg.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 10:27:29.151563 docs2kg-0.0.7/examples/kg/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 10:27:21.000000 docs2kg-0.0.7/examples/kg/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      253 2024-06-03 10:27:21.000000 docs2kg-0.0.7/examples/kg/utils/json2triplets.py
--rw-r--r--   0 runner    (1001) docker     (127)      978 2024-06-03 10:27:21.000000 docs2kg-0.0.7/examples/kg/utils/neo4j_connector.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 10:27:29.151563 docs2kg-0.0.7/examples/modules/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 10:27:21.000000 docs2kg-0.0.7/examples/modules/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      353 2024-06-03 10:27:21.000000 docs2kg-0.0.7/examples/modules/markdown_clean_md.py
--rw-r--r--   0 runner    (1001) docker     (127)      351 2024-06-03 10:27:21.000000 docs2kg-0.0.7/examples/modules/markdown_json.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 10:27:29.151563 docs2kg-0.0.7/examples/parser/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 10:27:21.000000 docs2kg-0.0.7/examples/parser/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 10:27:29.151563 docs2kg-0.0.7/examples/parser/email/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 10:27:21.000000 docs2kg-0.0.7/examples/parser/email/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      279 2024-06-03 10:27:21.000000 docs2kg-0.0.7/examples/parser/email/email_process.py
--rw-r--r--   0 runner    (1001) docker     (127)      481 2024-06-03 10:27:21.000000 docs2kg-0.0.7/examples/parser/email/email_pull.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 10:27:29.151563 docs2kg-0.0.7/examples/parser/excel/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 10:27:21.000000 docs2kg-0.0.7/examples/parser/excel/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      602 2024-06-03 10:27:21.000000 docs2kg-0.0.7/examples/parser/excel/excel_process.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 10:27:29.151563 docs2kg-0.0.7/examples/parser/pdf/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 10:27:21.000000 docs2kg-0.0.7/examples/parser/pdf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1265 2024-06-03 10:27:21.000000 docs2kg-0.0.7/examples/parser/pdf/pdf_metadata_summary.py
--rw-r--r--   0 runner    (1001) docker     (127)     1315 2024-06-03 10:27:21.000000 docs2kg-0.0.7/examples/parser/pdf/pdf_process.py
--rw-r--r--   0 runner    (1001) docker     (127)     1283 2024-06-03 10:27:21.000000 docs2kg-0.0.7/examples/parser/pdf/pdf_scanned_process.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 10:27:29.151563 docs2kg-0.0.7/examples/parser/web/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 10:27:21.000000 docs2kg-0.0.7/examples/parser/web/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      603 2024-06-03 10:27:21.000000 docs2kg-0.0.7/examples/parser/web/web_process.py
--rw-r--r--   0 runner    (1001) docker     (127)      201 2024-06-03 10:27:21.000000 docs2kg-0.0.7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      215 2024-06-03 10:27:29.151563 docs2kg-0.0.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2019 2024-06-03 10:27:21.000000 docs2kg-0.0.7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 10:27:29.151563 docs2kg-0.0.7/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 10:27:21.000000 docs2kg-0.0.7/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 10:03:23.070428 docs2kg-0.1.1/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 10:03:23.058428 docs2kg-0.1.1/Docs2KG/
+-rw-r--r--   0 runner    (1001) docker     (127)       61 2024-06-03 10:03:15.000000 docs2kg-0.1.1/Docs2KG/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 10:03:23.058428 docs2kg-0.1.1/Docs2KG/kg/
+-rw-r--r--   0 runner    (1001) docker     (127)      873 2024-06-03 10:03:15.000000 docs2kg-0.1.1/Docs2KG/kg/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5447 2024-06-03 10:03:15.000000 docs2kg-0.1.1/Docs2KG/kg/docs_linkage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6269 2024-06-03 10:03:15.000000 docs2kg-0.1.1/Docs2KG/kg/email_layout_kg.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5538 2024-06-03 10:03:15.000000 docs2kg-0.1.1/Docs2KG/kg/excel_layout_kg.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22047 2024-06-03 10:03:15.000000 docs2kg-0.1.1/Docs2KG/kg/pdf_layout_kg.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20174 2024-06-03 10:03:15.000000 docs2kg-0.1.1/Docs2KG/kg/semantic_kg.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 10:03:23.058428 docs2kg-0.1.1/Docs2KG/kg/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 10:03:15.000000 docs2kg-0.1.1/Docs2KG/kg/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15156 2024-06-03 10:03:15.000000 docs2kg-0.1.1/Docs2KG/kg/utils/json2triplets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5398 2024-06-03 10:03:15.000000 docs2kg-0.1.1/Docs2KG/kg/utils/neo4j_connector.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6275 2024-06-03 10:03:15.000000 docs2kg-0.1.1/Docs2KG/kg/web_layout_kg.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 10:03:23.058428 docs2kg-0.1.1/Docs2KG/modules/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 10:03:15.000000 docs2kg-0.1.1/Docs2KG/modules/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 10:03:23.062428 docs2kg-0.1.1/Docs2KG/modules/llm/
+-rw-r--r--   0 runner    (1001) docker     (127)      398 2024-06-03 10:03:15.000000 docs2kg-0.1.1/Docs2KG/modules/llm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      399 2024-06-03 10:03:15.000000 docs2kg-0.1.1/Docs2KG/modules/llm/image2description.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13124 2024-06-03 10:03:15.000000 docs2kg-0.1.1/Docs2KG/modules/llm/markdown2json.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1664 2024-06-03 10:03:15.000000 docs2kg-0.1.1/Docs2KG/modules/llm/openai_call.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4444 2024-06-03 10:03:15.000000 docs2kg-0.1.1/Docs2KG/modules/llm/sheet2metadata.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 10:03:23.062428 docs2kg-0.1.1/Docs2KG/modules/native/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 10:03:15.000000 docs2kg-0.1.1/Docs2KG/modules/native/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2896 2024-06-03 10:03:15.000000 docs2kg-0.1.1/Docs2KG/modules/native/markdown2json.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 10:03:23.062428 docs2kg-0.1.1/Docs2KG/parser/
+-rw-r--r--   0 runner    (1001) docker     (127)      522 2024-06-03 10:03:15.000000 docs2kg-0.1.1/Docs2KG/parser/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 10:03:23.062428 docs2kg-0.1.1/Docs2KG/parser/email/
+-rw-r--r--   0 runner    (1001) docker     (127)      228 2024-06-03 10:03:15.000000 docs2kg-0.1.1/Docs2KG/parser/email/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      797 2024-06-03 10:03:15.000000 docs2kg-0.1.1/Docs2KG/parser/email/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4765 2024-06-03 10:03:15.000000 docs2kg-0.1.1/Docs2KG/parser/email/email_compose.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 10:03:23.062428 docs2kg-0.1.1/Docs2KG/parser/email/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 10:03:15.000000 docs2kg-0.1.1/Docs2KG/parser/email/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4850 2024-06-03 10:03:15.000000 docs2kg-0.1.1/Docs2KG/parser/email/utils/email_connector.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 10:03:23.062428 docs2kg-0.1.1/Docs2KG/parser/excel/
+-rw-r--r--   0 runner    (1001) docker     (127)      170 2024-06-03 10:03:15.000000 docs2kg-0.1.1/Docs2KG/parser/excel/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2136 2024-06-03 10:03:15.000000 docs2kg-0.1.1/Docs2KG/parser/excel/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2072 2024-06-03 10:03:15.000000 docs2kg-0.1.1/Docs2KG/parser/excel/excel2image.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1095 2024-06-03 10:03:15.000000 docs2kg-0.1.1/Docs2KG/parser/excel/excel2markdown.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2405 2024-06-03 10:03:15.000000 docs2kg-0.1.1/Docs2KG/parser/excel/excel2table.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 10:03:23.066428 docs2kg-0.1.1/Docs2KG/parser/pdf/
+-rw-r--r--   0 runner    (1001) docker     (127)      477 2024-06-03 10:03:15.000000 docs2kg-0.1.1/Docs2KG/parser/pdf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1541 2024-06-03 10:03:15.000000 docs2kg-0.1.1/Docs2KG/parser/pdf/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)      430 2024-06-03 10:03:15.000000 docs2kg-0.1.1/Docs2KG/parser/pdf/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3145 2024-06-03 10:03:15.000000 docs2kg-0.1.1/Docs2KG/parser/pdf/pdf2blocks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1649 2024-06-03 10:03:15.000000 docs2kg-0.1.1/Docs2KG/parser/pdf/pdf2image.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5264 2024-06-03 10:03:15.000000 docs2kg-0.1.1/Docs2KG/parser/pdf/pdf2metadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2133 2024-06-03 10:03:15.000000 docs2kg-0.1.1/Docs2KG/parser/pdf/pdf2tables.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2765 2024-06-03 10:03:15.000000 docs2kg-0.1.1/Docs2KG/parser/pdf/pdf2text.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 10:03:23.066428 docs2kg-0.1.1/Docs2KG/parser/web/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 10:03:15.000000 docs2kg-0.1.1/Docs2KG/parser/web/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1507 2024-06-03 10:03:15.000000 docs2kg-0.1.1/Docs2KG/parser/web/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1250 2024-06-03 10:03:15.000000 docs2kg-0.1.1/Docs2KG/parser/web/web2images.py
+-rw-r--r--   0 runner    (1001) docker     (127)      811 2024-06-03 10:03:15.000000 docs2kg-0.1.1/Docs2KG/parser/web/web2markdown.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1281 2024-06-03 10:03:15.000000 docs2kg-0.1.1/Docs2KG/parser/web/web2tables.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1006 2024-06-03 10:03:15.000000 docs2kg-0.1.1/Docs2KG/parser/web/web2urls.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 10:03:23.066428 docs2kg-0.1.1/Docs2KG/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 10:03:15.000000 docs2kg-0.1.1/Docs2KG/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      484 2024-06-03 10:03:15.000000 docs2kg-0.1.1/Docs2KG/utils/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)      155 2024-06-03 10:03:15.000000 docs2kg-0.1.1/Docs2KG/utils/empty_check.py
+-rw-r--r--   0 runner    (1001) docker     (127)      917 2024-06-03 10:03:15.000000 docs2kg-0.1.1/Docs2KG/utils/get_logger.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 10:03:23.066428 docs2kg-0.1.1/Docs2KG/utils/llm/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 10:03:15.000000 docs2kg-0.1.1/Docs2KG/utils/llm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1167 2024-06-03 10:03:15.000000 docs2kg-0.1.1/Docs2KG/utils/llm/count_tokens.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1021 2024-06-03 10:03:15.000000 docs2kg-0.1.1/Docs2KG/utils/llm/estimate_price.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1728 2024-06-03 10:03:15.000000 docs2kg-0.1.1/Docs2KG/utils/llm/track_usage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7360 2024-06-03 10:03:15.000000 docs2kg-0.1.1/Docs2KG/utils/rect.py
+-rw-r--r--   0 runner    (1001) docker     (127)      946 2024-06-03 10:03:15.000000 docs2kg-0.1.1/Docs2KG/utils/timer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 10:03:23.070428 docs2kg-0.1.1/Docs2KG.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3235 2024-06-03 10:03:23.000000 docs2kg-0.1.1/Docs2KG.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2849 2024-06-03 10:03:23.000000 docs2kg-0.1.1/Docs2KG.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-03 10:03:23.000000 docs2kg-0.1.1/Docs2KG.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      179 2024-06-03 10:03:23.000000 docs2kg-0.1.1/Docs2KG.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-06-03 10:03:23.000000 docs2kg-0.1.1/Docs2KG.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    26526 2024-06-03 10:03:15.000000 docs2kg-0.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3235 2024-06-03 10:03:23.070428 docs2kg-0.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2120 2024-06-03 10:03:15.000000 docs2kg-0.1.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 10:03:23.066428 docs2kg-0.1.1/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 10:03:15.000000 docs2kg-0.1.1/examples/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 10:03:23.066428 docs2kg-0.1.1/examples/demo/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 10:03:15.000000 docs2kg-0.1.1/examples/demo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1232 2024-06-03 10:03:15.000000 docs2kg-0.1.1/examples/demo/emails.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2067 2024-06-03 10:03:15.000000 docs2kg-0.1.1/examples/demo/excel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5367 2024-06-03 10:03:15.000000 docs2kg-0.1.1/examples/demo/pdf_exported.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5709 2024-06-03 10:03:15.000000 docs2kg-0.1.1/examples/demo/pdf_scanned.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1194 2024-06-03 10:03:15.000000 docs2kg-0.1.1/examples/demo/web.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 10:03:23.070428 docs2kg-0.1.1/examples/kg/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 10:03:15.000000 docs2kg-0.1.1/examples/kg/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      942 2024-06-03 10:03:15.000000 docs2kg-0.1.1/examples/kg/docs_linkage.py
+-rw-r--r--   0 runner    (1001) docker     (127)      243 2024-06-03 10:03:15.000000 docs2kg-0.1.1/examples/kg/layout_kg.py
+-rw-r--r--   0 runner    (1001) docker     (127)      267 2024-06-03 10:03:15.000000 docs2kg-0.1.1/examples/kg/semantic_kg.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 10:03:23.070428 docs2kg-0.1.1/examples/kg/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 10:03:15.000000 docs2kg-0.1.1/examples/kg/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      253 2024-06-03 10:03:15.000000 docs2kg-0.1.1/examples/kg/utils/json2triplets.py
+-rw-r--r--   0 runner    (1001) docker     (127)      978 2024-06-03 10:03:15.000000 docs2kg-0.1.1/examples/kg/utils/neo4j_connector.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 10:03:23.070428 docs2kg-0.1.1/examples/modules/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 10:03:15.000000 docs2kg-0.1.1/examples/modules/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      353 2024-06-03 10:03:15.000000 docs2kg-0.1.1/examples/modules/markdown_clean_md.py
+-rw-r--r--   0 runner    (1001) docker     (127)      351 2024-06-03 10:03:15.000000 docs2kg-0.1.1/examples/modules/markdown_json.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 10:03:23.070428 docs2kg-0.1.1/examples/parser/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 10:03:15.000000 docs2kg-0.1.1/examples/parser/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 10:03:23.070428 docs2kg-0.1.1/examples/parser/email/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 10:03:15.000000 docs2kg-0.1.1/examples/parser/email/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      279 2024-06-03 10:03:15.000000 docs2kg-0.1.1/examples/parser/email/email_process.py
+-rw-r--r--   0 runner    (1001) docker     (127)      481 2024-06-03 10:03:15.000000 docs2kg-0.1.1/examples/parser/email/email_pull.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 10:03:23.070428 docs2kg-0.1.1/examples/parser/excel/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 10:03:15.000000 docs2kg-0.1.1/examples/parser/excel/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      602 2024-06-03 10:03:15.000000 docs2kg-0.1.1/examples/parser/excel/excel_process.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 10:03:23.070428 docs2kg-0.1.1/examples/parser/pdf/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 10:03:15.000000 docs2kg-0.1.1/examples/parser/pdf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1265 2024-06-03 10:03:15.000000 docs2kg-0.1.1/examples/parser/pdf/pdf_metadata_summary.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1315 2024-06-03 10:03:15.000000 docs2kg-0.1.1/examples/parser/pdf/pdf_process.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1283 2024-06-03 10:03:15.000000 docs2kg-0.1.1/examples/parser/pdf/pdf_scanned_process.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 10:03:23.070428 docs2kg-0.1.1/examples/parser/web/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 10:03:15.000000 docs2kg-0.1.1/examples/parser/web/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      603 2024-06-03 10:03:15.000000 docs2kg-0.1.1/examples/parser/web/web_process.py
+-rw-r--r--   0 runner    (1001) docker     (127)      201 2024-06-03 10:03:15.000000 docs2kg-0.1.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      215 2024-06-03 10:03:23.070428 docs2kg-0.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1443 2024-06-03 10:03:15.000000 docs2kg-0.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 10:03:23.070428 docs2kg-0.1.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 10:03:15.000000 docs2kg-0.1.1/tests/__init__.py
```

### Comparing `docs2kg-0.0.7/Docs2KG/kg/__init__.py` & `docs2kg-0.1.1/Docs2KG/kg/__init__.py`

 * *Files identical despite different names*

### Comparing `docs2kg-0.0.7/Docs2KG/kg/docs_linkage.py` & `docs2kg-0.1.1/Docs2KG/kg/docs_linkage.py`

 * *Files identical despite different names*

### Comparing `docs2kg-0.0.7/Docs2KG/kg/email_layout_kg.py` & `docs2kg-0.1.1/Docs2KG/kg/email_layout_kg.py`

 * *Files identical despite different names*

### Comparing `docs2kg-0.0.7/Docs2KG/kg/excel_layout_kg.py` & `docs2kg-0.1.1/Docs2KG/kg/excel_layout_kg.py`

 * *Files identical despite different names*

### Comparing `docs2kg-0.0.7/Docs2KG/kg/pdf_layout_kg.py` & `docs2kg-0.1.1/Docs2KG/kg/pdf_layout_kg.py`

 * *Files identical despite different names*

### Comparing `docs2kg-0.0.7/Docs2KG/kg/semantic_kg.py` & `docs2kg-0.1.1/Docs2KG/kg/semantic_kg.py`

 * *Files identical despite different names*

### Comparing `docs2kg-0.0.7/Docs2KG/kg/utils/json2triplets.py` & `docs2kg-0.1.1/Docs2KG/kg/utils/json2triplets.py`

 * *Files identical despite different names*

### Comparing `docs2kg-0.0.7/Docs2KG/kg/utils/neo4j_connector.py` & `docs2kg-0.1.1/Docs2KG/kg/utils/neo4j_connector.py`

 * *Files identical despite different names*

### Comparing `docs2kg-0.0.7/Docs2KG/kg/web_layout_kg.py` & `docs2kg-0.1.1/Docs2KG/kg/web_layout_kg.py`

 * *Files identical despite different names*

### Comparing `docs2kg-0.0.7/Docs2KG/modules/llm/markdown2json.py` & `docs2kg-0.1.1/Docs2KG/modules/llm/markdown2json.py`

 * *Files identical despite different names*

### Comparing `docs2kg-0.0.7/Docs2KG/modules/llm/openai_call.py` & `docs2kg-0.1.1/Docs2KG/modules/llm/openai_call.py`

 * *Files identical despite different names*

### Comparing `docs2kg-0.0.7/Docs2KG/modules/llm/sheet2metadata.py` & `docs2kg-0.1.1/Docs2KG/modules/llm/sheet2metadata.py`

 * *Files identical despite different names*

### Comparing `docs2kg-0.0.7/Docs2KG/modules/native/markdown2json.py` & `docs2kg-0.1.1/Docs2KG/modules/native/markdown2json.py`

 * *Files identical despite different names*

### Comparing `docs2kg-0.0.7/Docs2KG/parser/__init__.py` & `docs2kg-0.1.1/Docs2KG/parser/__init__.py`

 * *Files identical despite different names*

### Comparing `docs2kg-0.0.7/Docs2KG/parser/email/base.py` & `docs2kg-0.1.1/Docs2KG/parser/email/base.py`

 * *Files identical despite different names*

### Comparing `docs2kg-0.0.7/Docs2KG/parser/email/email_compose.py` & `docs2kg-0.1.1/Docs2KG/parser/email/email_compose.py`

 * *Files identical despite different names*

### Comparing `docs2kg-0.0.7/Docs2KG/parser/email/utils/email_connector.py` & `docs2kg-0.1.1/Docs2KG/parser/email/utils/email_connector.py`

 * *Files identical despite different names*

### Comparing `docs2kg-0.0.7/Docs2KG/parser/excel/base.py` & `docs2kg-0.1.1/Docs2KG/parser/excel/base.py`

 * *Files identical despite different names*

### Comparing `docs2kg-0.0.7/Docs2KG/parser/excel/excel2image.py` & `docs2kg-0.1.1/Docs2KG/parser/excel/excel2image.py`

 * *Files identical despite different names*

### Comparing `docs2kg-0.0.7/Docs2KG/parser/excel/excel2markdown.py` & `docs2kg-0.1.1/Docs2KG/parser/excel/excel2markdown.py`

 * *Files identical despite different names*

### Comparing `docs2kg-0.0.7/Docs2KG/parser/excel/excel2table.py` & `docs2kg-0.1.1/Docs2KG/parser/excel/excel2table.py`

 * *Files identical despite different names*

### Comparing `docs2kg-0.0.7/Docs2KG/parser/pdf/base.py` & `docs2kg-0.1.1/Docs2KG/parser/pdf/base.py`

 * *Files identical despite different names*

### Comparing `docs2kg-0.0.7/Docs2KG/parser/pdf/pdf2blocks.py` & `docs2kg-0.1.1/Docs2KG/parser/pdf/pdf2blocks.py`

 * *Files identical despite different names*

### Comparing `docs2kg-0.0.7/Docs2KG/parser/pdf/pdf2image.py` & `docs2kg-0.1.1/Docs2KG/parser/pdf/pdf2image.py`

 * *Files identical despite different names*

### Comparing `docs2kg-0.0.7/Docs2KG/parser/pdf/pdf2metadata.py` & `docs2kg-0.1.1/Docs2KG/parser/pdf/pdf2metadata.py`

 * *Files identical despite different names*

### Comparing `docs2kg-0.0.7/Docs2KG/parser/pdf/pdf2tables.py` & `docs2kg-0.1.1/Docs2KG/parser/pdf/pdf2tables.py`

 * *Files identical despite different names*

### Comparing `docs2kg-0.0.7/Docs2KG/parser/pdf/pdf2text.py` & `docs2kg-0.1.1/Docs2KG/parser/pdf/pdf2text.py`

 * *Files identical despite different names*

### Comparing `docs2kg-0.0.7/Docs2KG/parser/web/base.py` & `docs2kg-0.1.1/Docs2KG/parser/web/base.py`

 * *Files identical despite different names*

### Comparing `docs2kg-0.0.7/Docs2KG/parser/web/web2images.py` & `docs2kg-0.1.1/Docs2KG/parser/web/web2images.py`

 * *Files identical despite different names*

### Comparing `docs2kg-0.0.7/Docs2KG/parser/web/web2markdown.py` & `docs2kg-0.1.1/Docs2KG/parser/web/web2markdown.py`

 * *Files identical despite different names*

### Comparing `docs2kg-0.0.7/Docs2KG/parser/web/web2tables.py` & `docs2kg-0.1.1/Docs2KG/parser/web/web2tables.py`

 * *Files identical despite different names*

### Comparing `docs2kg-0.0.7/Docs2KG/parser/web/web2urls.py` & `docs2kg-0.1.1/Docs2KG/parser/web/web2urls.py`

 * *Files identical despite different names*

### Comparing `docs2kg-0.0.7/Docs2KG/utils/get_logger.py` & `docs2kg-0.1.1/Docs2KG/utils/get_logger.py`

 * *Files identical despite different names*

### Comparing `docs2kg-0.0.7/Docs2KG/utils/llm/count_tokens.py` & `docs2kg-0.1.1/Docs2KG/utils/llm/count_tokens.py`

 * *Files identical despite different names*

### Comparing `docs2kg-0.0.7/Docs2KG/utils/llm/estimate_price.py` & `docs2kg-0.1.1/Docs2KG/utils/llm/estimate_price.py`

 * *Files identical despite different names*

### Comparing `docs2kg-0.0.7/Docs2KG/utils/llm/track_usage.py` & `docs2kg-0.1.1/Docs2KG/utils/llm/track_usage.py`

 * *Files identical despite different names*

### Comparing `docs2kg-0.0.7/Docs2KG/utils/rect.py` & `docs2kg-0.1.1/Docs2KG/utils/rect.py`

 * *Files identical despite different names*

### Comparing `docs2kg-0.0.7/Docs2KG/utils/timer.py` & `docs2kg-0.1.1/Docs2KG/utils/timer.py`

 * *Files identical despite different names*

### Comparing `docs2kg-0.0.7/Docs2KG.egg-info/PKG-INFO` & `docs2kg-0.1.1/Docs2KG.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Docs2KG
-Version: 0.0.7
+Version: 0.1.1
 Summary: Unified Knowledge Graph Construction from Heterogeneous Documents Assisted by Large Language Models
 Home-page: https://docs2kg.ai4wa.com
 Author: AI4WA
 Author-email: admin@ai4wa.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
@@ -35,18 +35,18 @@
 Requires-Dist: neo4j
 
 # Open Source Framework: Docs2KG
 
 **Unified Knowledge Graph Construction from Heterogeneous Documents Assisted by Large
 Language Models**
 
-![Lint](https://github.com/AI4WA/Docs2KG/blob/main/https://github.com/AI4WA/Docs2KG/actions/workflows/lint.yml/badge.svg)
-![Documentation](https://github.com/AI4WA/Docs2KG/blob/main/https://github.com/AI4WA/Docs2KG/actions/workflows/docs.yml/badge.svg)
-[![Demo](https://img.shields.io/badge/Demo-Available-blue)](https://github.com/AI4WA/Docs2KG/blob/main/https://docs2kg.ai4wa.com/Video/)
-![Status](https://github.com/AI4WA/Docs2KG/blob/main/https://img.shields.io/badge/Status-Work%20in%20Progress-yellow)
+![Lint](https://github.com/AI4WA/Docs2KG/actions/workflows/lint.yml/badge.svg)
+![Documentation](https://github.com/AI4WA/Docs2KG/actions/workflows/docs.yml/badge.svg)
+[![Demo](https://img.shields.io/badge/Demo-Available-blue)](https://docs2kg.ai4wa.com/Video/)
+![Status](https://img.shields.io/badge/Status-Work%20in%20Progress-yellow)
 
 Three pillars of the LLM applications in our opinion:
 
 - Data
 - RAG
 - LLM
 
@@ -72,29 +72,29 @@
 - We proposed a way to organize the data within the centralized place, via a Unified Knowledge Graph altogether with
   semi-structured data.
 
 ### Overall Architecture
 
 The overall workflow will be:
 
-![img.png](https://github.com/AI4WA/Docs2KG/blob/main/docs/images/Docs2KG.jpg)
+![img.png](docs/images/Docs2KG.jpg)
 
 ## System Architecture
 
-![img.png](https://github.com/AI4WA/Docs2KG/blob/main/docs/images/Modules.jpg)
+![img.png](docs/images/Modules.jpg)
 
 ### PDF
 
 The Main data under this category is PDF.
 
 So we need to be able to extract the text and images from the PDF.
 
 ## Unified Knowledge Graph
 
-![img.png](https://github.com/AI4WA/Docs2KG/blob/main/docs/images/KGConstruction.jpg)
+![img.png](docs/images/KGConstruction.jpg)
 
 ## Setup
 
 ```bash
 python3 -m venv venv
 source venv/bin/activate
 pip install -r requirements.txt
```

### Comparing `docs2kg-0.0.7/Docs2KG.egg-info/SOURCES.txt` & `docs2kg-0.1.1/Docs2KG.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `docs2kg-0.0.7/LICENSE` & `docs2kg-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `docs2kg-0.0.7/PKG-INFO` & `docs2kg-0.1.1/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Docs2KG
-Version: 0.0.7
+Version: 0.1.1
 Summary: Unified Knowledge Graph Construction from Heterogeneous Documents Assisted by Large Language Models
 Home-page: https://docs2kg.ai4wa.com
 Author: AI4WA
 Author-email: admin@ai4wa.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
@@ -35,18 +35,18 @@
 Requires-Dist: neo4j
 
 # Open Source Framework: Docs2KG
 
 **Unified Knowledge Graph Construction from Heterogeneous Documents Assisted by Large
 Language Models**
 
-![Lint](https://github.com/AI4WA/Docs2KG/blob/main/https://github.com/AI4WA/Docs2KG/actions/workflows/lint.yml/badge.svg)
-![Documentation](https://github.com/AI4WA/Docs2KG/blob/main/https://github.com/AI4WA/Docs2KG/actions/workflows/docs.yml/badge.svg)
-[![Demo](https://img.shields.io/badge/Demo-Available-blue)](https://github.com/AI4WA/Docs2KG/blob/main/https://docs2kg.ai4wa.com/Video/)
-![Status](https://github.com/AI4WA/Docs2KG/blob/main/https://img.shields.io/badge/Status-Work%20in%20Progress-yellow)
+![Lint](https://github.com/AI4WA/Docs2KG/actions/workflows/lint.yml/badge.svg)
+![Documentation](https://github.com/AI4WA/Docs2KG/actions/workflows/docs.yml/badge.svg)
+[![Demo](https://img.shields.io/badge/Demo-Available-blue)](https://docs2kg.ai4wa.com/Video/)
+![Status](https://img.shields.io/badge/Status-Work%20in%20Progress-yellow)
 
 Three pillars of the LLM applications in our opinion:
 
 - Data
 - RAG
 - LLM
 
@@ -72,29 +72,29 @@
 - We proposed a way to organize the data within the centralized place, via a Unified Knowledge Graph altogether with
   semi-structured data.
 
 ### Overall Architecture
 
 The overall workflow will be:
 
-![img.png](https://github.com/AI4WA/Docs2KG/blob/main/docs/images/Docs2KG.jpg)
+![img.png](docs/images/Docs2KG.jpg)
 
 ## System Architecture
 
-![img.png](https://github.com/AI4WA/Docs2KG/blob/main/docs/images/Modules.jpg)
+![img.png](docs/images/Modules.jpg)
 
 ### PDF
 
 The Main data under this category is PDF.
 
 So we need to be able to extract the text and images from the PDF.
 
 ## Unified Knowledge Graph
 
-![img.png](https://github.com/AI4WA/Docs2KG/blob/main/docs/images/KGConstruction.jpg)
+![img.png](docs/images/KGConstruction.jpg)
 
 ## Setup
 
 ```bash
 python3 -m venv venv
 source venv/bin/activate
 pip install -r requirements.txt
```

### Comparing `docs2kg-0.0.7/README.md` & `docs2kg-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `docs2kg-0.0.7/examples/demo/emails.py` & `docs2kg-0.1.1/examples/demo/emails.py`

 * *Files identical despite different names*

### Comparing `docs2kg-0.0.7/examples/demo/excel.py` & `docs2kg-0.1.1/examples/demo/excel.py`

 * *Files identical despite different names*

### Comparing `docs2kg-0.0.7/examples/demo/pdf_exported.py` & `docs2kg-0.1.1/examples/demo/pdf_exported.py`

 * *Files identical despite different names*

### Comparing `docs2kg-0.0.7/examples/demo/pdf_scanned.py` & `docs2kg-0.1.1/examples/demo/pdf_scanned.py`

 * *Files identical despite different names*

### Comparing `docs2kg-0.0.7/examples/demo/web.py` & `docs2kg-0.1.1/examples/demo/web.py`

 * *Files identical despite different names*

### Comparing `docs2kg-0.0.7/examples/kg/docs_linkage.py` & `docs2kg-0.1.1/examples/kg/docs_linkage.py`

 * *Files identical despite different names*

### Comparing `docs2kg-0.0.7/examples/kg/utils/neo4j_connector.py` & `docs2kg-0.1.1/examples/kg/utils/neo4j_connector.py`

 * *Files identical despite different names*

### Comparing `docs2kg-0.0.7/examples/parser/excel/excel_process.py` & `docs2kg-0.1.1/examples/parser/excel/excel_process.py`

 * *Files identical despite different names*

### Comparing `docs2kg-0.0.7/examples/parser/pdf/pdf_metadata_summary.py` & `docs2kg-0.1.1/examples/parser/pdf/pdf_metadata_summary.py`

 * *Files identical despite different names*

### Comparing `docs2kg-0.0.7/examples/parser/pdf/pdf_process.py` & `docs2kg-0.1.1/examples/parser/pdf/pdf_process.py`

 * *Files identical despite different names*

### Comparing `docs2kg-0.0.7/examples/parser/pdf/pdf_scanned_process.py` & `docs2kg-0.1.1/examples/parser/pdf/pdf_scanned_process.py`

 * *Files identical despite different names*

### Comparing `docs2kg-0.0.7/examples/parser/web/web_process.py` & `docs2kg-0.1.1/examples/parser/web/web_process.py`

 * *Files identical despite different names*

