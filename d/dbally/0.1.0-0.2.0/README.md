# Comparing `tmp/dbally-0.1.0.tar.gz` & `tmp/dbally-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dbally-0.1.0.tar", last modified: Thu Apr 25 10:31:00 2024, max compression
+gzip compressed data, was "dbally-0.2.0.tar", last modified: Mon Jun  3 13:41:13 2024, max compression
```

## Comparing `dbally-0.1.0.tar` & `dbally-0.2.0.tar`

### file list

```diff
@@ -1,113 +1,118 @@
-drwxrwxr-x   0 mateusz   (1001) mateusz   (1001)        0 2024-04-25 10:31:00.917163 dbally-0.1.0/
--rw-rw-r--   0 mateusz   (1001) mateusz   (1001)     1089 2024-04-19 10:03:11.000000 dbally-0.1.0/LICENSE
--rw-rw-r--   0 mateusz   (1001) mateusz   (1001)       97 2024-04-03 11:01:33.000000 dbally-0.1.0/MANIFEST.in
--rw-r--r--   0 mateusz   (1001) mateusz   (1001)     8363 2024-04-25 10:31:00.913163 dbally-0.1.0/PKG-INFO
--rw-rw-r--   0 mateusz   (1001) mateusz   (1001)     6104 2024-04-19 10:03:11.000000 dbally-0.1.0/README.md
--rw-rw-r--   0 mateusz   (1001) mateusz   (1001)     4477 2024-04-19 10:03:11.000000 dbally-0.1.0/pyproject.toml
--rw-rw-r--   0 mateusz   (1001) mateusz   (1001)     1747 2024-04-25 10:31:00.917163 dbally-0.1.0/setup.cfg
--rwxrwxr-x   0 mateusz   (1001) mateusz   (1001)      150 2024-04-03 11:01:33.000000 dbally-0.1.0/setup.py
-drwxrwxr-x   0 mateusz   (1001) mateusz   (1001)        0 2024-04-25 10:31:00.801161 dbally-0.1.0/src/
-drwxrwxr-x   0 mateusz   (1001) mateusz   (1001)        0 2024-04-25 10:31:00.809161 dbally-0.1.0/src/dbally/
--rw-rw-r--   0 mateusz   (1001) mateusz   (1001)      668 2024-04-19 10:03:11.000000 dbally-0.1.0/src/dbally/__init__.py
--rw-rw-r--   0 mateusz   (1001) mateusz   (1001)       49 2024-04-25 10:22:49.000000 dbally-0.1.0/src/dbally/__version__.py
--rw-rw-r--   0 mateusz   (1001) mateusz   (1001)     2685 2024-04-19 10:03:11.000000 dbally-0.1.0/src/dbally/_main.py
-drwxrwxr-x   0 mateusz   (1001) mateusz   (1001)        0 2024-04-25 10:31:00.821161 dbally-0.1.0/src/dbally/assistants/
--rw-rw-r--   0 mateusz   (1001) mateusz   (1001)        0 2024-04-03 11:01:33.000000 dbally-0.1.0/src/dbally/assistants/__init__.py
--rw-rw-r--   0 mateusz   (1001) mateusz   (1001)     4192 2024-04-03 11:01:33.000000 dbally-0.1.0/src/dbally/assistants/base.py
--rw-rw-r--   0 mateusz   (1001) mateusz   (1001)     6238 2024-04-19 10:03:11.000000 dbally-0.1.0/src/dbally/assistants/openai.py
-drwxrwxr-x   0 mateusz   (1001) mateusz   (1001)        0 2024-04-25 10:31:00.825161 dbally-0.1.0/src/dbally/audit/
--rw-rw-r--   0 mateusz   (1001) mateusz   (1001)      347 2024-04-10 06:42:50.000000 dbally-0.1.0/src/dbally/audit/__init__.py
-drwxrwxr-x   0 mateusz   (1001) mateusz   (1001)        0 2024-04-25 10:31:00.829161 dbally-0.1.0/src/dbally/audit/event_handlers/
--rw-rw-r--   0 mateusz   (1001) mateusz   (1001)       59 2024-04-03 11:01:33.000000 dbally-0.1.0/src/dbally/audit/event_handlers/__init__.py
--rw-rw-r--   0 mateusz   (1001) mateusz   (1001)     2060 2024-04-19 10:03:11.000000 dbally-0.1.0/src/dbally/audit/event_handlers/base.py
--rw-rw-r--   0 mateusz   (1001) mateusz   (1001)     3988 2024-04-19 10:03:11.000000 dbally-0.1.0/src/dbally/audit/event_handlers/cli_event_handler.py
--rw-rw-r--   0 mateusz   (1001) mateusz   (1001)     2938 2024-04-19 10:03:11.000000 dbally-0.1.0/src/dbally/audit/event_handlers/langsmith_event_handler.py
--rw-rw-r--   0 mateusz   (1001) mateusz   (1001)      409 2024-04-03 11:01:33.000000 dbally-0.1.0/src/dbally/audit/event_span.py
--rw-rw-r--   0 mateusz   (1001) mateusz   (1001)     2670 2024-04-03 11:01:33.000000 dbally-0.1.0/src/dbally/audit/event_tracker.py
--rw-rw-r--   0 mateusz   (1001) mateusz   (1001)    11270 2024-04-25 10:22:49.000000 dbally-0.1.0/src/dbally/collection.py
-drwxrwxr-x   0 mateusz   (1001) mateusz   (1001)        0 2024-04-25 10:31:00.833161 dbally-0.1.0/src/dbally/data_models/
--rw-rw-r--   0 mateusz   (1001) mateusz   (1001)        0 2024-04-03 11:01:33.000000 dbally-0.1.0/src/dbally/data_models/__init__.py
--rw-rw-r--   0 mateusz   (1001) mateusz   (1001)      838 2024-04-10 07:45:19.000000 dbally-0.1.0/src/dbally/data_models/audit.py
--rw-rw-r--   0 mateusz   (1001) mateusz   (1001)     1729 2024-04-19 10:03:11.000000 dbally-0.1.0/src/dbally/data_models/execution_result.py
--rw-rw-r--   0 mateusz   (1001) mateusz   (1001)      610 2024-04-19 10:03:11.000000 dbally-0.1.0/src/dbally/data_models/llm_options.py
-drwxrwxr-x   0 mateusz   (1001) mateusz   (1001)        0 2024-04-25 10:31:00.841162 dbally-0.1.0/src/dbally/data_models/prompts/
--rw-rw-r--   0 mateusz   (1001) mateusz   (1001)      522 2024-04-03 11:01:33.000000 dbally-0.1.0/src/dbally/data_models/prompts/__init__.py
--rw-rw-r--   0 mateusz   (1001) mateusz   (1001)     1379 2024-04-03 11:01:33.000000 dbally-0.1.0/src/dbally/data_models/prompts/common_validation_utils.py
--rw-rw-r--   0 mateusz   (1001) mateusz   (1001)     2192 2024-04-03 11:01:33.000000 dbally-0.1.0/src/dbally/data_models/prompts/iql_prompt_template.py
--rw-rw-r--   0 mateusz   (1001) mateusz   (1001)     1686 2024-04-03 11:01:33.000000 dbally-0.1.0/src/dbally/data_models/prompts/nl_responder_prompt_template.py
--rw-rw-r--   0 mateusz   (1001) mateusz   (1001)     2638 2024-04-03 11:01:33.000000 dbally-0.1.0/src/dbally/data_models/prompts/prompt_template.py
--rw-rw-r--   0 mateusz   (1001) mateusz   (1001)     2028 2024-04-19 10:03:11.000000 dbally-0.1.0/src/dbally/data_models/prompts/query_explainer_prompt_template.py
--rw-rw-r--   0 mateusz   (1001) mateusz   (1001)     1777 2024-04-03 11:01:33.000000 dbally-0.1.0/src/dbally/data_models/prompts/view_selector_prompt_template.py
-drwxrwxr-x   0 mateusz   (1001) mateusz   (1001)        0 2024-04-25 10:31:00.845162 dbally-0.1.0/src/dbally/embedding_client/
--rw-rw-r--   0 mateusz   (1001) mateusz   (1001)      132 2024-04-10 06:42:50.000000 dbally-0.1.0/src/dbally/embedding_client/__init__.py
--rw-rw-r--   0 mateusz   (1001) mateusz   (1001)      545 2024-04-03 11:01:33.000000 dbally-0.1.0/src/dbally/embedding_client/base.py
--rw-rw-r--   0 mateusz   (1001) mateusz   (1001)     1661 2024-04-03 11:01:33.000000 dbally-0.1.0/src/dbally/embedding_client/openai.py
-drwxrwxr-x   0 mateusz   (1001) mateusz   (1001)        0 2024-04-25 10:31:00.853162 dbally-0.1.0/src/dbally/iql/
--rw-rw-r--   0 mateusz   (1001) mateusz   (1001)      238 2024-04-03 11:01:33.000000 dbally-0.1.0/src/dbally/iql/__init__.py
--rw-rw-r--   0 mateusz   (1001) mateusz   (1001)     1510 2024-04-03 11:01:33.000000 dbally-0.1.0/src/dbally/iql/_exceptions.py
--rw-rw-r--   0 mateusz   (1001) mateusz   (1001)     4845 2024-04-19 10:03:11.000000 dbally-0.1.0/src/dbally/iql/_processor.py
--rw-rw-r--   0 mateusz   (1001) mateusz   (1001)      840 2024-04-19 10:03:11.000000 dbally-0.1.0/src/dbally/iql/_query.py
--rw-rw-r--   0 mateusz   (1001) mateusz   (1001)     2573 2024-04-03 11:01:33.000000 dbally-0.1.0/src/dbally/iql/_type_validators.py
--rw-rw-r--   0 mateusz   (1001) mateusz   (1001)     2440 2024-04-19 10:03:11.000000 dbally-0.1.0/src/dbally/iql/syntax.py
-drwxrwxr-x   0 mateusz   (1001) mateusz   (1001)        0 2024-04-25 10:31:00.857162 dbally-0.1.0/src/dbally/iql_generator/
--rw-rw-r--   0 mateusz   (1001) mateusz   (1001)        0 2024-04-03 11:01:33.000000 dbally-0.1.0/src/dbally/iql_generator/__init__.py
--rw-rw-r--   0 mateusz   (1001) mateusz   (1001)     4256 2024-04-19 10:03:11.000000 dbally-0.1.0/src/dbally/iql_generator/iql_generator.py
-drwxrwxr-x   0 mateusz   (1001) mateusz   (1001)        0 2024-04-25 10:31:00.857162 dbally-0.1.0/src/dbally/llm_client/
--rw-rw-r--   0 mateusz   (1001) mateusz   (1001)        0 2024-04-03 11:01:33.000000 dbally-0.1.0/src/dbally/llm_client/__init__.py
--rw-rw-r--   0 mateusz   (1001) mateusz   (1001)     3093 2024-04-25 10:22:46.000000 dbally-0.1.0/src/dbally/llm_client/base.py
--rw-rw-r--   0 mateusz   (1001) mateusz   (1001)     2393 2024-04-19 10:03:11.000000 dbally-0.1.0/src/dbally/llm_client/openai_client.py
-drwxrwxr-x   0 mateusz   (1001) mateusz   (1001)        0 2024-04-25 10:31:00.861162 dbally-0.1.0/src/dbally/nl_responder/
--rw-rw-r--   0 mateusz   (1001) mateusz   (1001)        0 2024-04-03 11:01:33.000000 dbally-0.1.0/src/dbally/nl_responder/__init__.py
--rw-rw-r--   0 mateusz   (1001) mateusz   (1001)     4267 2024-04-22 11:03:10.000000 dbally-0.1.0/src/dbally/nl_responder/nl_responder.py
--rw-rw-r--   0 mateusz   (1001) mateusz   (1001)     2060 2024-04-03 11:01:33.000000 dbally-0.1.0/src/dbally/nl_responder/token_counters.py
-drwxrwxr-x   0 mateusz   (1001) mateusz   (1001)        0 2024-04-25 10:31:00.865162 dbally-0.1.0/src/dbally/prompts/
--rw-rw-r--   0 mateusz   (1001) mateusz   (1001)       71 2024-04-03 11:01:33.000000 dbally-0.1.0/src/dbally/prompts/__init__.py
--rw-rw-r--   0 mateusz   (1001) mateusz   (1001)     2361 2024-04-19 10:03:11.000000 dbally-0.1.0/src/dbally/prompts/prompt_builder.py
--rw-rw-r--   0 mateusz   (1001) mateusz   (1001)        0 2024-04-03 11:01:33.000000 dbally-0.1.0/src/dbally/py.typed
-drwxrwxr-x   0 mateusz   (1001) mateusz   (1001)        0 2024-04-25 10:31:00.877162 dbally-0.1.0/src/dbally/similarity/
--rw-rw-r--   0 mateusz   (1001) mateusz   (1001)      603 2024-04-25 10:22:46.000000 dbally-0.1.0/src/dbally/similarity/__init__.py
--rw-rw-r--   0 mateusz   (1001) mateusz   (1001)     3477 2024-04-25 10:22:46.000000 dbally-0.1.0/src/dbally/similarity/chroma_store.py
--rw-rw-r--   0 mateusz   (1001) mateusz   (1001)     7666 2024-04-19 10:03:11.000000 dbally-0.1.0/src/dbally/similarity/detector.py
--rw-rw-r--   0 mateusz   (1001) mateusz   (1001)     3388 2024-04-19 10:03:11.000000 dbally-0.1.0/src/dbally/similarity/faiss_store.py
--rw-rw-r--   0 mateusz   (1001) mateusz   (1001)      432 2024-04-19 10:03:11.000000 dbally-0.1.0/src/dbally/similarity/fetcher.py
--rw-rw-r--   0 mateusz   (1001) mateusz   (1001)     2146 2024-04-19 10:03:11.000000 dbally-0.1.0/src/dbally/similarity/index.py
--rw-rw-r--   0 mateusz   (1001) mateusz   (1001)     3560 2024-04-19 10:03:11.000000 dbally-0.1.0/src/dbally/similarity/sqlalchemy_base.py
--rw-rw-r--   0 mateusz   (1001) mateusz   (1001)     1000 2024-04-19 10:03:11.000000 dbally-0.1.0/src/dbally/similarity/store.py
-drwxrwxr-x   0 mateusz   (1001) mateusz   (1001)        0 2024-04-25 10:31:00.877162 dbally-0.1.0/src/dbally/utils/
--rw-rw-r--   0 mateusz   (1001) mateusz   (1001)        0 2024-04-03 11:01:33.000000 dbally-0.1.0/src/dbally/utils/__init__.py
--rw-rw-r--   0 mateusz   (1001) mateusz   (1001)      249 2024-04-03 11:01:33.000000 dbally-0.1.0/src/dbally/utils/errors.py
-drwxrwxr-x   0 mateusz   (1001) mateusz   (1001)        0 2024-04-25 10:31:00.881162 dbally-0.1.0/src/dbally/view_selection/
--rw-rw-r--   0 mateusz   (1001) mateusz   (1001)       99 2024-04-19 10:03:11.000000 dbally-0.1.0/src/dbally/view_selection/__init__.py
--rw-rw-r--   0 mateusz   (1001) mateusz   (1001)      748 2024-04-19 10:03:11.000000 dbally-0.1.0/src/dbally/view_selection/base.py
--rw-rw-r--   0 mateusz   (1001) mateusz   (1001)     3012 2024-04-19 10:03:11.000000 dbally-0.1.0/src/dbally/view_selection/llm_view_selector.py
--rw-rw-r--   0 mateusz   (1001) mateusz   (1001)      865 2024-04-03 11:01:33.000000 dbally-0.1.0/src/dbally/view_selection/random_view_selector.py
-drwxrwxr-x   0 mateusz   (1001) mateusz   (1001)        0 2024-04-25 10:31:00.893162 dbally-0.1.0/src/dbally/views/
--rw-rw-r--   0 mateusz   (1001) mateusz   (1001)        0 2024-04-03 11:01:33.000000 dbally-0.1.0/src/dbally/views/__init__.py
--rw-rw-r--   0 mateusz   (1001) mateusz   (1001)     1161 2024-04-19 10:03:11.000000 dbally-0.1.0/src/dbally/views/base.py
--rw-rw-r--   0 mateusz   (1001) mateusz   (1001)      414 2024-04-19 10:03:11.000000 dbally-0.1.0/src/dbally/views/decorators.py
--rw-rw-r--   0 mateusz   (1001) mateusz   (1001)     1822 2024-04-19 10:03:11.000000 dbally-0.1.0/src/dbally/views/exposed_functions.py
-drwxrwxr-x   0 mateusz   (1001) mateusz   (1001)        0 2024-04-25 10:31:00.897163 dbally-0.1.0/src/dbally/views/freeform/
--rw-rw-r--   0 mateusz   (1001) mateusz   (1001)        0 2024-04-25 10:22:46.000000 dbally-0.1.0/src/dbally/views/freeform/__init__.py
-drwxrwxr-x   0 mateusz   (1001) mateusz   (1001)        0 2024-04-25 10:31:00.901162 dbally-0.1.0/src/dbally/views/freeform/text2sql/
--rw-rw-r--   0 mateusz   (1001) mateusz   (1001)      358 2024-04-25 10:22:46.000000 dbally-0.1.0/src/dbally/views/freeform/text2sql/__init__.py
--rw-rw-r--   0 mateusz   (1001) mateusz   (1001)    12232 2024-04-25 10:22:46.000000 dbally-0.1.0/src/dbally/views/freeform/text2sql/_autodiscovery.py
--rw-rw-r--   0 mateusz   (1001) mateusz   (1001)     1358 2024-04-25 10:22:46.000000 dbally-0.1.0/src/dbally/views/freeform/text2sql/_config.py
--rw-rw-r--   0 mateusz   (1001) mateusz   (1001)      316 2024-04-25 10:22:46.000000 dbally-0.1.0/src/dbally/views/freeform/text2sql/_errors.py
--rw-rw-r--   0 mateusz   (1001) mateusz   (1001)     4275 2024-04-25 10:22:46.000000 dbally-0.1.0/src/dbally/views/freeform/text2sql/_view.py
--rw-rw-r--   0 mateusz   (1001) mateusz   (1001)     3474 2024-04-19 10:03:11.000000 dbally-0.1.0/src/dbally/views/methods_base.py
--rw-rw-r--   0 mateusz   (1001) mateusz   (1001)     3296 2024-04-19 10:03:11.000000 dbally-0.1.0/src/dbally/views/pandas_base.py
--rw-rw-r--   0 mateusz   (1001) mateusz   (1001)     3484 2024-04-19 10:03:11.000000 dbally-0.1.0/src/dbally/views/sqlalchemy_base.py
--rw-rw-r--   0 mateusz   (1001) mateusz   (1001)     3521 2024-04-19 10:03:11.000000 dbally-0.1.0/src/dbally/views/structured.py
-drwxrwxr-x   0 mateusz   (1001) mateusz   (1001)        0 2024-04-25 10:31:00.905163 dbally-0.1.0/src/dbally.egg-info/
--rw-r--r--   0 mateusz   (1001) mateusz   (1001)     8363 2024-04-25 10:31:00.000000 dbally-0.1.0/src/dbally.egg-info/PKG-INFO
--rw-rw-r--   0 mateusz   (1001) mateusz   (1001)     3126 2024-04-25 10:31:00.000000 dbally-0.1.0/src/dbally.egg-info/SOURCES.txt
--rw-rw-r--   0 mateusz   (1001) mateusz   (1001)        1 2024-04-25 10:31:00.000000 dbally-0.1.0/src/dbally.egg-info/dependency_links.txt
--rw-rw-r--   0 mateusz   (1001) mateusz   (1001)       47 2024-04-25 10:31:00.000000 dbally-0.1.0/src/dbally.egg-info/entry_points.txt
--rw-rw-r--   0 mateusz   (1001) mateusz   (1001)        1 2024-01-26 12:33:13.000000 dbally-0.1.0/src/dbally.egg-info/not-zip-safe
--rw-rw-r--   0 mateusz   (1001) mateusz   (1001)      525 2024-04-25 10:31:00.000000 dbally-0.1.0/src/dbally.egg-info/requires.txt
--rw-rw-r--   0 mateusz   (1001) mateusz   (1001)       18 2024-04-25 10:31:00.000000 dbally-0.1.0/src/dbally.egg-info/top_level.txt
-drwxrwxr-x   0 mateusz   (1001) mateusz   (1001)        0 2024-04-25 10:31:00.905163 dbally-0.1.0/src/dbally_cli/
--rw-rw-r--   0 mateusz   (1001) mateusz   (1001)        0 2024-04-03 11:01:33.000000 dbally-0.1.0/src/dbally_cli/__init__.py
--rw-rw-r--   0 mateusz   (1001) mateusz   (1001)      178 2024-04-19 10:03:11.000000 dbally-0.1.0/src/dbally_cli/main.py
--rw-rw-r--   0 mateusz   (1001) mateusz   (1001)     1842 2024-04-19 10:03:11.000000 dbally-0.1.0/src/dbally_cli/similarity.py
--rw-rw-r--   0 mateusz   (1001) mateusz   (1001)        0 2024-04-03 11:01:33.000000 dbally-0.1.0/src/py.typed
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-06-03 13:41:13.427283 dbally-0.2.0/
+-rw-r--r--   0 root         (0) root         (0)     1089 2024-06-03 13:41:08.000000 dbally-0.2.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       97 2024-06-03 13:41:08.000000 dbally-0.2.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     8292 2024-06-03 13:41:13.427283 dbally-0.2.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     6077 2024-06-03 13:41:08.000000 dbally-0.2.0/README.md
+-rw-r--r--   0 root         (0) root         (0)     4486 2024-06-03 13:41:08.000000 dbally-0.2.0/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)     1765 2024-06-03 13:41:13.427283 dbally-0.2.0/setup.cfg
+-rwxr-xr-x   0 root         (0) root         (0)      150 2024-06-03 13:41:08.000000 dbally-0.2.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-06-03 13:41:13.407283 dbally-0.2.0/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-06-03 13:41:13.407283 dbally-0.2.0/src/dbally/
+-rw-r--r--   0 root         (0) root         (0)     1747 2024-06-03 13:41:08.000000 dbally-0.2.0/src/dbally/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       50 2024-06-03 13:41:10.000000 dbally-0.2.0/src/dbally/__version__.py
+-rw-r--r--   0 root         (0) root         (0)       99 2024-06-03 13:41:08.000000 dbally-0.2.0/src/dbally/_exceptions.py
+-rw-r--r--   0 root         (0) root         (0)     2554 2024-06-03 13:41:08.000000 dbally-0.2.0/src/dbally/_main.py
+-rw-r--r--   0 root         (0) root         (0)      746 2024-06-03 13:41:08.000000 dbally-0.2.0/src/dbally/_types.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-06-03 13:41:13.407283 dbally-0.2.0/src/dbally/assistants/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-06-03 13:41:08.000000 dbally-0.2.0/src/dbally/assistants/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4192 2024-06-03 13:41:08.000000 dbally-0.2.0/src/dbally/assistants/base.py
+-rw-r--r--   0 root         (0) root         (0)     6238 2024-06-03 13:41:08.000000 dbally-0.2.0/src/dbally/assistants/openai.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-06-03 13:41:13.411283 dbally-0.2.0/src/dbally/audit/
+-rw-r--r--   0 root         (0) root         (0)      347 2024-06-03 13:41:08.000000 dbally-0.2.0/src/dbally/audit/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-06-03 13:41:13.411283 dbally-0.2.0/src/dbally/audit/event_handlers/
+-rw-r--r--   0 root         (0) root         (0)       59 2024-06-03 13:41:08.000000 dbally-0.2.0/src/dbally/audit/event_handlers/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2121 2024-06-03 13:41:08.000000 dbally-0.2.0/src/dbally/audit/event_handlers/base.py
+-rw-r--r--   0 root         (0) root         (0)     4655 2024-06-03 13:41:08.000000 dbally-0.2.0/src/dbally/audit/event_handlers/cli_event_handler.py
+-rw-r--r--   0 root         (0) root         (0)     3648 2024-06-03 13:41:08.000000 dbally-0.2.0/src/dbally/audit/event_handlers/langsmith_event_handler.py
+-rw-r--r--   0 root         (0) root         (0)      457 2024-06-03 13:41:08.000000 dbally-0.2.0/src/dbally/audit/event_span.py
+-rw-r--r--   0 root         (0) root         (0)     2718 2024-06-03 13:41:08.000000 dbally-0.2.0/src/dbally/audit/event_tracker.py
+-rw-r--r--   0 root         (0) root         (0)    11593 2024-06-03 13:41:08.000000 dbally-0.2.0/src/dbally/collection.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-06-03 13:41:13.411283 dbally-0.2.0/src/dbally/data_models/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-06-03 13:41:08.000000 dbally-0.2.0/src/dbally/data_models/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1029 2024-06-03 13:41:08.000000 dbally-0.2.0/src/dbally/data_models/audit.py
+-rw-r--r--   0 root         (0) root         (0)     1729 2024-06-03 13:41:08.000000 dbally-0.2.0/src/dbally/data_models/execution_result.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-06-03 13:41:13.411283 dbally-0.2.0/src/dbally/embeddings/
+-rw-r--r--   0 root         (0) root         (0)      135 2024-06-03 13:41:08.000000 dbally-0.2.0/src/dbally/embeddings/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1023 2024-06-03 13:41:08.000000 dbally-0.2.0/src/dbally/embeddings/_exceptions.py
+-rw-r--r--   0 root         (0) root         (0)      469 2024-06-03 13:41:08.000000 dbally-0.2.0/src/dbally/embeddings/base.py
+-rw-r--r--   0 root         (0) root         (0)     3131 2024-06-03 13:41:08.000000 dbally-0.2.0/src/dbally/embeddings/litellm.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-06-03 13:41:13.415283 dbally-0.2.0/src/dbally/iql/
+-rw-r--r--   0 root         (0) root         (0)      238 2024-06-03 13:41:08.000000 dbally-0.2.0/src/dbally/iql/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1510 2024-06-03 13:41:08.000000 dbally-0.2.0/src/dbally/iql/_exceptions.py
+-rw-r--r--   0 root         (0) root         (0)     5072 2024-06-03 13:41:08.000000 dbally-0.2.0/src/dbally/iql/_processor.py
+-rw-r--r--   0 root         (0) root         (0)     1048 2024-06-03 13:41:08.000000 dbally-0.2.0/src/dbally/iql/_query.py
+-rw-r--r--   0 root         (0) root         (0)     2573 2024-06-03 13:41:08.000000 dbally-0.2.0/src/dbally/iql/_type_validators.py
+-rw-r--r--   0 root         (0) root         (0)     2440 2024-06-03 13:41:08.000000 dbally-0.2.0/src/dbally/iql/syntax.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-06-03 13:41:13.415283 dbally-0.2.0/src/dbally/iql_generator/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-06-03 13:41:08.000000 dbally-0.2.0/src/dbally/iql_generator/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4090 2024-06-03 13:41:08.000000 dbally-0.2.0/src/dbally/iql_generator/iql_generator.py
+-rw-r--r--   0 root         (0) root         (0)     2100 2024-06-03 13:41:08.000000 dbally-0.2.0/src/dbally/iql_generator/iql_prompt_template.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-06-03 13:41:13.415283 dbally-0.2.0/src/dbally/llms/
+-rw-r--r--   0 root         (0) root         (0)       81 2024-06-03 13:41:08.000000 dbally-0.2.0/src/dbally/llms/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3514 2024-06-03 13:41:08.000000 dbally-0.2.0/src/dbally/llms/base.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-06-03 13:41:13.415283 dbally-0.2.0/src/dbally/llms/clients/
+-rw-r--r--   0 root         (0) root         (0)      184 2024-06-03 13:41:08.000000 dbally-0.2.0/src/dbally/llms/clients/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      970 2024-06-03 13:41:08.000000 dbally-0.2.0/src/dbally/llms/clients/_exceptions.py
+-rw-r--r--   0 root         (0) root         (0)     2562 2024-06-03 13:41:08.000000 dbally-0.2.0/src/dbally/llms/clients/base.py
+-rw-r--r--   0 root         (0) root         (0)     4102 2024-06-03 13:41:08.000000 dbally-0.2.0/src/dbally/llms/clients/litellm.py
+-rw-r--r--   0 root         (0) root         (0)     2648 2024-06-03 13:41:08.000000 dbally-0.2.0/src/dbally/llms/litellm.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-06-03 13:41:13.415283 dbally-0.2.0/src/dbally/nl_responder/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-06-03 13:41:08.000000 dbally-0.2.0/src/dbally/nl_responder/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3961 2024-06-03 13:41:08.000000 dbally-0.2.0/src/dbally/nl_responder/nl_responder.py
+-rw-r--r--   0 root         (0) root         (0)     1594 2024-06-03 13:41:08.000000 dbally-0.2.0/src/dbally/nl_responder/nl_responder_prompt_template.py
+-rw-r--r--   0 root         (0) root         (0)     1936 2024-06-03 13:41:08.000000 dbally-0.2.0/src/dbally/nl_responder/query_explainer_prompt_template.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-06-03 13:41:13.415283 dbally-0.2.0/src/dbally/prompts/
+-rw-r--r--   0 root         (0) root         (0)      230 2024-06-03 13:41:08.000000 dbally-0.2.0/src/dbally/prompts/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1365 2024-06-03 13:41:08.000000 dbally-0.2.0/src/dbally/prompts/common_validation_utils.py
+-rw-r--r--   0 root         (0) root         (0)     2620 2024-06-03 13:41:08.000000 dbally-0.2.0/src/dbally/prompts/prompt_template.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-06-03 13:41:08.000000 dbally-0.2.0/src/dbally/py.typed
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-06-03 13:41:13.419283 dbally-0.2.0/src/dbally/similarity/
+-rw-r--r--   0 root         (0) root         (0)      840 2024-06-03 13:41:08.000000 dbally-0.2.0/src/dbally/similarity/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3737 2024-06-03 13:41:08.000000 dbally-0.2.0/src/dbally/similarity/chroma_store.py
+-rw-r--r--   0 root         (0) root         (0)     3217 2024-06-03 13:41:08.000000 dbally-0.2.0/src/dbally/similarity/elastic_vector_search.py
+-rw-r--r--   0 root         (0) root         (0)     3478 2024-06-03 13:41:08.000000 dbally-0.2.0/src/dbally/similarity/elasticsearch_store.py
+-rw-r--r--   0 root         (0) root         (0)     3681 2024-06-03 13:41:08.000000 dbally-0.2.0/src/dbally/similarity/faiss_store.py
+-rw-r--r--   0 root         (0) root         (0)      432 2024-06-03 13:41:08.000000 dbally-0.2.0/src/dbally/similarity/fetcher.py
+-rw-r--r--   0 root         (0) root         (0)     2836 2024-06-03 13:41:08.000000 dbally-0.2.0/src/dbally/similarity/index.py
+-rw-r--r--   0 root         (0) root         (0)     4080 2024-06-03 13:41:08.000000 dbally-0.2.0/src/dbally/similarity/sqlalchemy_base.py
+-rw-r--r--   0 root         (0) root         (0)     1000 2024-06-03 13:41:08.000000 dbally-0.2.0/src/dbally/similarity/store.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-06-03 13:41:13.419283 dbally-0.2.0/src/dbally/utils/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-06-03 13:41:08.000000 dbally-0.2.0/src/dbally/utils/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      249 2024-06-03 13:41:08.000000 dbally-0.2.0/src/dbally/utils/errors.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-06-03 13:41:13.419283 dbally-0.2.0/src/dbally/view_selection/
+-rw-r--r--   0 root         (0) root         (0)       99 2024-06-03 13:41:08.000000 dbally-0.2.0/src/dbally/view_selection/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      955 2024-06-03 13:41:08.000000 dbally-0.2.0/src/dbally/view_selection/base.py
+-rw-r--r--   0 root         (0) root         (0)     3102 2024-06-03 13:41:08.000000 dbally-0.2.0/src/dbally/view_selection/llm_view_selector.py
+-rw-r--r--   0 root         (0) root         (0)     1072 2024-06-03 13:41:08.000000 dbally-0.2.0/src/dbally/view_selection/random_view_selector.py
+-rw-r--r--   0 root         (0) root         (0)     1685 2024-06-03 13:41:08.000000 dbally-0.2.0/src/dbally/view_selection/view_selector_prompt_template.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-06-03 13:41:13.423283 dbally-0.2.0/src/dbally/views/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-06-03 13:41:08.000000 dbally-0.2.0/src/dbally/views/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1728 2024-06-03 13:41:08.000000 dbally-0.2.0/src/dbally/views/base.py
+-rw-r--r--   0 root         (0) root         (0)      414 2024-06-03 13:41:08.000000 dbally-0.2.0/src/dbally/views/decorators.py
+-rw-r--r--   0 root         (0) root         (0)     1822 2024-06-03 13:41:08.000000 dbally-0.2.0/src/dbally/views/exposed_functions.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-06-03 13:41:13.423283 dbally-0.2.0/src/dbally/views/freeform/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-06-03 13:41:08.000000 dbally-0.2.0/src/dbally/views/freeform/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-06-03 13:41:13.423283 dbally-0.2.0/src/dbally/views/freeform/text2sql/
+-rw-r--r--   0 root         (0) root         (0)      214 2024-06-03 13:41:08.000000 dbally-0.2.0/src/dbally/views/freeform/text2sql/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1127 2024-06-03 13:41:08.000000 dbally-0.2.0/src/dbally/views/freeform/text2sql/config.py
+-rw-r--r--   0 root         (0) root         (0)      316 2024-06-03 13:41:08.000000 dbally-0.2.0/src/dbally/views/freeform/text2sql/errors.py
+-rw-r--r--   0 root         (0) root         (0)     9461 2024-06-03 13:41:08.000000 dbally-0.2.0/src/dbally/views/freeform/text2sql/view.py
+-rw-r--r--   0 root         (0) root         (0)     3474 2024-06-03 13:41:08.000000 dbally-0.2.0/src/dbally/views/methods_base.py
+-rw-r--r--   0 root         (0) root         (0)     3296 2024-06-03 13:41:08.000000 dbally-0.2.0/src/dbally/views/pandas_base.py
+-rw-r--r--   0 root         (0) root         (0)     3484 2024-06-03 13:41:08.000000 dbally-0.2.0/src/dbally/views/sqlalchemy_base.py
+-rw-r--r--   0 root         (0) root         (0)     4518 2024-06-03 13:41:08.000000 dbally-0.2.0/src/dbally/views/structured.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-06-03 13:41:13.423283 dbally-0.2.0/src/dbally.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     8292 2024-06-03 13:41:13.000000 dbally-0.2.0/src/dbally.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     3142 2024-06-03 13:41:13.000000 dbally-0.2.0/src/dbally.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-06-03 13:41:13.000000 dbally-0.2.0/src/dbally.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       47 2024-06-03 13:41:13.000000 dbally-0.2.0/src/dbally.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-06-03 13:41:13.000000 dbally-0.2.0/src/dbally.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)      513 2024-06-03 13:41:13.000000 dbally-0.2.0/src/dbally.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       33 2024-06-03 13:41:13.000000 dbally-0.2.0/src/dbally.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-06-03 13:41:13.423283 dbally-0.2.0/src/dbally_cli/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-06-03 13:41:08.000000 dbally-0.2.0/src/dbally_cli/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      116 2024-06-03 13:41:08.000000 dbally-0.2.0/src/dbally_cli/main.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-06-03 13:41:13.423283 dbally-0.2.0/src/dbally_codegen/
+-rw-r--r--   0 root         (0) root         (0)      262 2024-06-03 13:41:08.000000 dbally-0.2.0/src/dbally_codegen/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    14824 2024-06-03 13:41:08.000000 dbally-0.2.0/src/dbally_codegen/autodiscovery.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-06-03 13:41:08.000000 dbally-0.2.0/src/py.typed
```

### Comparing `dbally-0.1.0/LICENSE` & `dbally-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `dbally-0.1.0/PKG-INFO` & `dbally-0.2.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbally
-Version: 0.1.0
+Version: 0.2.0
 Summary: "Efficient, consistent and secure library for querying structured data with natural language"
 Author: deepsense.ai
 Author-email: contact@deepsense.ai
 License: MIT
 Project-URL: Documentation, https://db-ally.deepsense.ai/
 Project-URL: Source, https://github.com/deepsense-ai/db-ally
 Classifier: Development Status :: 2 - Pre-Alpha
@@ -22,39 +22,38 @@
 License-File: LICENSE
 Requires-Dist: pandas~=2.0.3
 Requires-Dist: python-dotenv>=0.5.1
 Requires-Dist: SQLAlchemy==2.0.25
 Requires-Dist: tabulate>=0.9.0
 Requires-Dist: click~=8.1.7
 Requires-Dist: numpy>=1.24.0
-Provides-Extra: openai
-Requires-Dist: openai>=1.10.0; extra == "openai"
-Requires-Dist: tiktoken>=0.6.0; extra == "openai"
+Provides-Extra: litellm
+Requires-Dist: litellm>=1.37.9; extra == "litellm"
 Provides-Extra: faiss
 Requires-Dist: faiss-cpu>=1.8.0; extra == "faiss"
+Provides-Extra: chromadb
+Requires-Dist: chromadb>=0.4.24; extra == "chromadb"
+Provides-Extra: langsmith
+Requires-Dist: langsmith~=0.1.57; extra == "langsmith"
 Provides-Extra: examples
 Requires-Dist: pydantic~=2.6.0; extra == "examples"
 Requires-Dist: pydantic_settings~=2.1.0; extra == "examples"
 Requires-Dist: psycopg2-binary~=2.9.9; extra == "examples"
-Provides-Extra: langsmith
-Requires-Dist: langsmith>=0.0.87; extra == "langsmith"
-Provides-Extra: transformers
-Requires-Dist: transformers>=4.37.1; extra == "transformers"
 Provides-Extra: benchmark
 Requires-Dist: asyncpg~=0.28.0; extra == "benchmark"
 Requires-Dist: eval-type-backport~=0.1.3; extra == "benchmark"
 Requires-Dist: hydra-core~=1.3.2; extra == "benchmark"
 Requires-Dist: loguru~=0.7.0; extra == "benchmark"
 Requires-Dist: neptune~=1.6.3; extra == "benchmark"
 Requires-Dist: pydantic~=2.6.1; extra == "benchmark"
 Requires-Dist: pydantic-core~=2.16.2; extra == "benchmark"
 Requires-Dist: pydantic-settings~=2.0.3; extra == "benchmark"
 Requires-Dist: psycopg2-binary~=2.9.9; extra == "benchmark"
-Provides-Extra: chromadb
-Requires-Dist: chromadb>=0.4.24; extra == "chromadb"
+Provides-Extra: elasticsearch
+Requires-Dist: elasticsearch==8.13.1; extra == "elasticsearch"
 
 # <h1 align="center">db-ally</h1>
 
 <p align="center">
     <em>Efficient, consistent and secure library for querying structured data with natural language</em>
 </p>
 
@@ -81,15 +80,15 @@
 
 In db-ally, developers define their use cases by implementing [**views**](https://db-ally.deepsense.ai/concepts/views) and **filters**. A list of possible filters is presented to the LLM in terms of [**IQL**](https://db-ally.deepsense.ai/concepts/iql) (Intermediate Query Language). Views are grouped and registered within a [**collection**](https://db-ally.deepsense.ai/concepts/views), which then serves as an entry point for asking questions in natural language.
 
 This is a basic implementation of a db-ally view for an example HR application, which retrieves candidates from an SQL database:
 
 ```python
 from dbally import decorators, SqlAlchemyBaseView, create_collection
-from dbally.llm_client.openai_client import OpenAIClient
+from dbally.llms.litellm import LiteLLM
 from sqlalchemy import create_engine
 
 class CandidateView(SqlAlchemyBaseView):
     """
     A view for retrieving candidates from the database.
     """
 
@@ -103,15 +102,15 @@
     def from_country(self, country: str):
         """
         Filter candidates from a specific country.
         """
         return Candidate.country == country
 
 engine = create_engine('sqlite:///candidates.db')
-llm = OpenAIClient(model_name="gpt-3.5-turbo")
+llm = LiteLLM(model_name="gpt-3.5-turbo")
 my_collection = create_collection("collection_name", llm)
 my_collection.add(CandidateView, lambda: CandidateView(engine))
 
 my_collection.ask("Find candidates from United States")
 ```
 
 For a concrete step-by-step example on how to use db-ally, go to [Quickstart](https://db-ally.deepsense.ai/quickstart/) guide. For a more learning-oriented experience, check our db-ally [Tutorial](https://db-ally.deepsense.ai/tutorials/tutorial_1).
@@ -132,20 +131,20 @@
 
 ```bash
 pip install dbally
 ```
 
 Additionally, you can install one of our extensions to use specific features.
 
-* `dbally[openai]`: Use [OpenAI's models](https://platform.openai.com/docs/models)
+* `dbally[litellm]`: Use [100+ LLMs](https://docs.litellm.ai/docs/providers)
 * `dbally[faiss]`: Use [Faiss](https://github.com/facebookresearch/faiss) indexes for similarity search
 * `dbally[langsmith]`: Use [LangSmith](https://www.langchain.com/langsmith) for query tracking
 
 ```bash
-pip install dbally[openai,faiss,langsmith]
+pip install dbally[litellm,faiss,langsmith]
 ```
 
 ## License
 
 db-ally is released under MIT license.
 
 ## How db-ally documentation is organized
```

### Comparing `dbally-0.1.0/README.md` & `dbally-0.2.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -27,15 +27,15 @@
 
 In db-ally, developers define their use cases by implementing [**views**](https://db-ally.deepsense.ai/concepts/views) and **filters**. A list of possible filters is presented to the LLM in terms of [**IQL**](https://db-ally.deepsense.ai/concepts/iql) (Intermediate Query Language). Views are grouped and registered within a [**collection**](https://db-ally.deepsense.ai/concepts/views), which then serves as an entry point for asking questions in natural language.
 
 This is a basic implementation of a db-ally view for an example HR application, which retrieves candidates from an SQL database:
 
 ```python
 from dbally import decorators, SqlAlchemyBaseView, create_collection
-from dbally.llm_client.openai_client import OpenAIClient
+from dbally.llms.litellm import LiteLLM
 from sqlalchemy import create_engine
 
 class CandidateView(SqlAlchemyBaseView):
     """
     A view for retrieving candidates from the database.
     """
 
@@ -49,15 +49,15 @@
     def from_country(self, country: str):
         """
         Filter candidates from a specific country.
         """
         return Candidate.country == country
 
 engine = create_engine('sqlite:///candidates.db')
-llm = OpenAIClient(model_name="gpt-3.5-turbo")
+llm = LiteLLM(model_name="gpt-3.5-turbo")
 my_collection = create_collection("collection_name", llm)
 my_collection.add(CandidateView, lambda: CandidateView(engine))
 
 my_collection.ask("Find candidates from United States")
 ```
 
 For a concrete step-by-step example on how to use db-ally, go to [Quickstart](https://db-ally.deepsense.ai/quickstart/) guide. For a more learning-oriented experience, check our db-ally [Tutorial](https://db-ally.deepsense.ai/tutorials/tutorial_1).
@@ -78,20 +78,20 @@
 
 ```bash
 pip install dbally
 ```
 
 Additionally, you can install one of our extensions to use specific features.
 
-* `dbally[openai]`: Use [OpenAI's models](https://platform.openai.com/docs/models)
+* `dbally[litellm]`: Use [100+ LLMs](https://docs.litellm.ai/docs/providers)
 * `dbally[faiss]`: Use [Faiss](https://github.com/facebookresearch/faiss) indexes for similarity search
 * `dbally[langsmith]`: Use [LangSmith](https://www.langchain.com/langsmith) for query tracking
 
 ```bash
-pip install dbally[openai,faiss,langsmith]
+pip install dbally[litellm,faiss,langsmith]
 ```
 
 ## License
 
 db-ally is released under MIT license.
 
 ## How db-ally documentation is organized
```

### Comparing `dbally-0.1.0/pyproject.toml` & `dbally-0.2.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -78,14 +78,16 @@
     '--doctest-glob=\*.rst',
     '--tb=short',
 ]
 testpaths = ['tests']
 
 [tool.pytest.ini_options]
 asyncio_mode = "auto"
+testpaths = ["tests"]
+pythonpath = ["."]
 
 [tool.mypy]
 warn_unused_configs = true
 ignore_missing_imports = true
 warn_unused_ignores = false
 show_error_codes = true
 check_untyped_defs = true
@@ -152,18 +154,15 @@
 assets = []
 commit_message = "{version}\n\nAutomatically generated by python-semantic-release"
 commit_parser = "angular"
 logging_use_named_masks = false
 major_on_zero = false
 allow_zero_version = true
 tag_format = "v{version}"
-version_variables = [
-    "setup.cfg:version",
-    "src/dbally/__version__.py:__version__",
-]
+version_variables = ["src/dbally/__version__.py:__version__"]
 build_command = "pip install build && python -m build"
 
 [tool.semantic_release.branches.main]
 match = "(main|master)"
 prerelease_token = "rc"
 prerelease = false
```

### Comparing `dbally-0.1.0/setup.cfg` & `dbally-0.2.0/setup.cfg`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = dbally
-version = 0.1.0
+version = attr: dbally.__version__.__version__
 description = "Efficient, consistent and secure library for querying structured data with natural language"
 long_description = file: README.md
 long_description_content_type = text/markdown
 author = deepsense.ai
 author_email = contact@deepsense.ai
 license = MIT
 license_files = LICENSE
@@ -36,39 +36,38 @@
 	python-dotenv>=0.5.1
 	SQLAlchemy==2.0.25
 	tabulate>=0.9.0
 	click~=8.1.7
 	numpy>=1.24.0
 
 [options.extras_require]
-openai = 
-	openai>=1.10.0
-	tiktoken>=0.6.0
+litellm = 
+	litellm>=1.37.9
 faiss = 
 	faiss-cpu>=1.8.0
+chromadb = 
+	chromadb>=0.4.24
+langsmith = 
+	langsmith~=0.1.57
 examples = 
 	pydantic~=2.6.0
 	pydantic_settings~=2.1.0
 	psycopg2-binary~=2.9.9
-langsmith = 
-	langsmith>=0.0.87
-transformers = 
-	transformers>=4.37.1
 benchmark = 
 	asyncpg~=0.28.0
 	eval-type-backport~=0.1.3
 	hydra-core~=1.3.2
 	loguru~=0.7.0
 	neptune~=1.6.3
 	pydantic~=2.6.1
 	pydantic-core~=2.16.2
 	pydantic-settings~=2.0.3
 	psycopg2-binary~=2.9.9
-chromadb = 
-	chromadb>=0.4.24
+elasticsearch = 
+	elasticsearch==8.13.1
 
 [options.packages.find]
 where = src
 
 [bdist_wheel]
 universal = 1
```

### Comparing `dbally-0.1.0/src/dbally/_main.py` & `dbally-0.2.0/src/dbally/_main.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 from typing import List, Optional
 
 from .audit.event_handlers.base import EventHandler
 from .collection import Collection
-from .llm_client.base import LLMClient
+from .llms import LLM
 from .nl_responder.nl_responder import NLResponder
 from .view_selection.base import ViewSelector
 from .view_selection.llm_view_selector import LLMViewSelector
 
 
 def create_collection(
     name: str,
-    llm_client: LLMClient,
+    llm: LLM,
     event_handlers: Optional[List[EventHandler]] = None,
     view_selector: Optional[ViewSelector] = None,
     nl_responder: Optional[NLResponder] = None,
 ) -> Collection:
     """
     Create a new [Collection](collection.md) that is a container for registering views and the\
     main entrypoint to db-ally features.
@@ -23,24 +23,23 @@
     provides a set of default values for various dependencies like LLM client, view selector,\
     IQL generator, and NL responder.
 
     ##Example
 
     ```python
         from dbally import create_collection
-        from dbally.llm_client.openai_client import OpenAIClient
+        from dbally.llms.litellm import LiteLLM
 
-        collection = create_collection("my_collection", llm_client=OpenAIClient())
+        collection = create_collection("my_collection", llm=LiteLLM())
     ```
 
     Args:
         name: Name of the collection is available for [Event handlers](event_handlers/index.md) and is\
         used to distinguish different db-ally runs.
-        llm_client: LLM client used by the collection to generate views and respond to natural language\
-        queries.
+        llm: LLM used by the collection to generate responses for natural language queries.
         event_handlers: Event handlers used by the collection during query executions. Can be used to\
         log events as [CLIEventHandler](event_handlers/cli_handler.md) or to validate system performance as\
         [LangSmithEventHandler](event_handlers/langsmith_handler.md).
         view_selector: View selector used by the collection to select the best view for the given query.\
         If None, a new instance of [LLMViewSelector][dbally.view_selection.llm_view_selector.LLMViewSelector]\
         will be used.
         nl_responder: NL responder used by the collection to respond to natural language queries. If None,\
@@ -48,18 +47,18 @@
 
     Returns:
         a new instance of db-ally Collection
 
     Raises:
         ValueError: if default LLM client is not configured
     """
-    view_selector = view_selector or LLMViewSelector(llm_client=llm_client)
-    nl_responder = nl_responder or NLResponder(llm_client=llm_client)
+    view_selector = view_selector or LLMViewSelector(llm=llm)
+    nl_responder = nl_responder or NLResponder(llm=llm)
     event_handlers = event_handlers or []
 
     return Collection(
         name,
         nl_responder=nl_responder,
         view_selector=view_selector,
-        llm_client=llm_client,
+        llm=llm,
         event_handlers=event_handlers,
     )
```

### Comparing `dbally-0.1.0/src/dbally/assistants/base.py` & `dbally-0.2.0/src/dbally/assistants/base.py`

 * *Files identical despite different names*

### Comparing `dbally-0.1.0/src/dbally/assistants/openai.py` & `dbally-0.2.0/src/dbally/assistants/openai.py`

 * *Files identical despite different names*

### Comparing `dbally-0.1.0/src/dbally/audit/event_handlers/base.py` & `dbally-0.2.0/src/dbally/audit/event_handlers/base.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import abc
 from abc import ABC
 from typing import Generic, TypeVar, Union
 
-from dbally.data_models.audit import LLMEvent, RequestEnd, RequestStart
+from dbally.data_models.audit import LLMEvent, RequestEnd, RequestStart, SimilarityEvent
 
 RequestCtx = TypeVar("RequestCtx")
 EventCtx = TypeVar("EventCtx")
 
 
 class EventHandler(Generic[RequestCtx, EventCtx], ABC):
     """
@@ -22,36 +22,36 @@
             user_request: Object containing name of collection and asked query
 
         Returns:
             Implementation-specific request context object, which is passed to the future callbacks
         """
 
     @abc.abstractmethod
-    async def event_start(self, event: Union[LLMEvent], request_context: RequestCtx) -> EventCtx:
+    async def event_start(self, event: Union[LLMEvent, SimilarityEvent], request_context: RequestCtx) -> EventCtx:
         """
         Function that is called during every event execution.
 
 
         Args:
-            event: LLMEvent to be logged with all the details.
+            event: db-ally event to be logged with all the details.
             request_context: Optional context passed from request_start method
 
         Returns:
             Implementation-specific request context object, which is passed to the `event_end` callback
         """
 
     @abc.abstractmethod
     async def event_end(
-        self, event: Union[None, LLMEvent], request_context: RequestCtx, event_context: EventCtx
+        self, event: Union[None, LLMEvent, SimilarityEvent], request_context: RequestCtx, event_context: EventCtx
     ) -> None:
         """
         Function that is called during every event execution.
 
         Args:
-            event: LLMEvent to be logged with all the details.
+            event: db-ally event to be logged with all the details.
             request_context: Optional context passed from request_start method
             event_context: Optional context passed from event_start method
         """
 
     @abc.abstractmethod
     async def request_end(self, output: RequestEnd, request_context: RequestCtx) -> None:
         """
```

### Comparing `dbally-0.1.0/src/dbally/audit/event_handlers/cli_event_handler.py` & `dbally-0.2.0/src/dbally/audit/event_handlers/cli_event_handler.py`

 * *Files 20% similar despite different names*

```diff
@@ -8,20 +8,20 @@
     RICH_OUTPUT = True
 except ImportError:
     RICH_OUTPUT = False
     # TODO: remove color tags from bare print
     pprint = print  # type: ignore
 
 from dbally.audit.event_handlers.base import EventHandler
-from dbally.data_models.audit import LLMEvent, RequestEnd, RequestStart
+from dbally.data_models.audit import LLMEvent, RequestEnd, RequestStart, SimilarityEvent
 
 
 class CLIEventHandler(EventHandler):
     """
-    This handler displays all interactions between LLM and user happending during `Collection.ask`\
+    This handler displays all interactions between LLM and user happening during `Collection.ask`\
     execution inside the terminal.
 
     ### Usage
 
     ```python
         import dbally
         from dbally.audit.event_handlers.cli_event_handler import CLIEventHandler
@@ -53,48 +53,61 @@
             user_request: Object containing name of collection and asked query
         """
 
         pprint(f"[orange3 bold]Request starts... \n[orange3 bold]MESSAGE: [grey53]{user_request.question}")
         pprint("[grey53]\n=======================================")
         pprint("[grey53]=======================================\n")
 
-    async def event_start(self, event: Union[LLMEvent], request_context: None) -> None:
+    async def event_start(self, event: Union[LLMEvent, SimilarityEvent], request_context: None) -> None:
         """
         Displays information that event has started, then all messages inside the prompt
 
 
         Args:
-            event: LLMEvent to be logged with all the details.
+            event: db-ally event to be logged with all the details.
             request_context: Optional context passed from request_start method
         """
 
         if isinstance(event, LLMEvent):
             pprint(f"[cyan bold]LLM event starts... \n[cyan bold]LLM EVENT PROMPT TYPE: [grey53]{event.type}")
 
             if isinstance(event.prompt, tuple):
                 for msg in event.prompt:
                     pprint(f"\n[orange3]{msg['role']}")
                     self._print_syntax(msg["content"], "text")
             else:
                 self._print_syntax(f"{event.prompt}", "text")
-
-    async def event_end(self, event: Union[None, LLMEvent], request_context: None, event_context: None) -> None:
+        elif isinstance(event, SimilarityEvent):
+            pprint(
+                f"[cyan bold]Similarity event starts... \n"
+                f"[cyan bold]INPUT: [grey53]{event.input_value}\n"
+                f"[cyan bold]STORE: [grey53]{event.store}\n"
+                f"[cyan bold]FETCHER: [grey53]{event.fetcher}\n"
+            )
+
+    async def event_end(
+        self, event: Union[None, LLMEvent, SimilarityEvent], request_context: None, event_context: None
+    ) -> None:
         """
         Displays the response from the LLM.
 
         Args:
-            event: LLMEvent to be logged with all the details.
+            event: db-ally event to be logged with all the details.
             request_context: Optional context passed from request_start method
             event_context: Optional context passed from event_start method
         """
 
         if isinstance(event, LLMEvent):
             pprint(f"\n[green bold]RESPONSE: {event.response}")
             pprint("[grey53]\n=======================================")
             pprint("[grey53]=======================================\n")
+        elif isinstance(event, SimilarityEvent):
+            pprint(f"[green bold]OUTPUT: {event.output_value}")
+            pprint("[grey53]\n=======================================")
+            pprint("[grey53]=======================================\n")
 
     async def request_end(self, output: RequestEnd, request_context: Optional[dict] = None) -> None:
         """
         Displays the output of the request, namely the `results` and the `context`
 
         Args:
             output: The output of the request.
```

### Comparing `dbally-0.1.0/src/dbally/audit/event_handlers/langsmith_event_handler.py` & `dbally-0.2.0/src/dbally/audit/event_handlers/langsmith_event_handler.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,29 +1,34 @@
 import socket
 from getpass import getuser
-from typing import Union
+from typing import Optional, Union
 
 from langsmith.client import Client
 from langsmith.run_trees import RunTree
 
 from dbally.audit.event_handlers.base import EventHandler
-from dbally.data_models.audit import LLMEvent, RequestEnd, RequestStart
+from dbally.data_models.audit import LLMEvent, RequestEnd, RequestStart, SimilarityEvent
 
 
 class LangSmithEventHandler(EventHandler[RunTree, RunTree]):
     """
     This handler Logs events to a LangSmith instance.
 
-
     !!! tip
         To learn how to use `LangSmithEventHandler` visit
         [How-To: Log db-ally runs to LangSmith](../../how-to/log_runs_to_langsmith.md)
     """
 
-    def __init__(self, api_key: str):
+    def __init__(self, api_key: Optional[str] = None):
+        """
+        Constructs a new langsmith event handler instance.
+
+        Args:
+            api_key: The api key for LangSmith. If None LANGCHAIN_API_KEY environment variable will be used.
+        """
         self._client = Client(api_key=api_key)
 
     async def request_start(self, user_request: RequestStart) -> RunTree:
         """
         Initializes the `RunTree` object with all required attributes.
 
         Args:
@@ -38,15 +43,15 @@
             inputs={"text": user_request.question},
             serialized={},
             client=self._client,
         )
 
         return run_tree
 
-    async def event_start(self, event: Union[None, LLMEvent], request_context: RunTree) -> RunTree:
+    async def event_start(self, event: Union[None, LLMEvent, SimilarityEvent], request_context: RunTree) -> RunTree:
         """
         Log the start of the event.
 
         Args:
             event: Event to be logged.
             request_context: Optional context passed from request_start method
 
@@ -58,35 +63,45 @@
         """
         if isinstance(event, LLMEvent):
             child_run = request_context.create_child(
                 name=event.type,
                 run_type="llm",
                 inputs={"prompts": [event.prompt]},
             )
+            return child_run
 
+        if isinstance(event, SimilarityEvent):
+            child_run = request_context.create_child(
+                name="Similarity Lookup",
+                run_type="tool",
+                inputs={"input": event.input_value, "store": event.store, "fetcher": event.fetcher},
+            )
             return child_run
 
         raise ValueError("Unsupported event")
 
-    async def event_end(self, event: Union[None, LLMEvent], request_context: RunTree, event_context: RunTree) -> None:
+    async def event_end(
+        self, event: Union[None, LLMEvent, SimilarityEvent], request_context: RunTree, event_context: RunTree
+    ) -> None:
         """
         Log the end of the event.
 
         Args:
             event: Event to be logged.
             request_context: Optional context passed from request_start method
             event_context: Optional context passed from event_start method
         """
         if isinstance(event, LLMEvent):
             event_context.end(outputs={"output": event.response})
+        elif isinstance(event, SimilarityEvent):
+            event_context.end(outputs={"output": event.output_value})
 
     async def request_end(self, output: RequestEnd, request_context: RunTree) -> None:
         """
         Log the end of the request.
 
         Args:
             output: The output of the request. In this case - PSQL query.
             request_context: Optional context passed from request_start method
         """
         request_context.end(outputs={"sql": output.result.context["sql"]})
-        res = request_context.post(exclude_child_runs=False)
-        res.result()
+        request_context.post(exclude_child_runs=False)
```

### Comparing `dbally-0.1.0/src/dbally/audit/event_tracker.py` & `dbally-0.2.0/src/dbally/audit/event_tracker.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from contextlib import asynccontextmanager
-from typing import AsyncIterator, Dict, List, Optional
+from typing import AsyncIterator, Dict, List, Optional, Union
 
 from dbally.audit.event_handlers.base import EventHandler
 from dbally.audit.event_span import EventSpan
-from dbally.data_models.audit import LLMEvent, RequestEnd, RequestStart
+from dbally.data_models.audit import LLMEvent, RequestEnd, RequestStart, SimilarityEvent
 
 
 class EventTracker:
     """
     Container for event handlers and is responsible for processing events."""
 
     _handlers: List[EventHandler]
@@ -65,15 +65,15 @@
         Args:
             event_handler: Event handler to be added.
         """
 
         self._handlers.append(event_handler)
 
     @asynccontextmanager
-    async def track_event(self, event: LLMEvent) -> AsyncIterator[EventSpan]:
+    async def track_event(self, event: Union[LLMEvent, SimilarityEvent]) -> AsyncIterator[EventSpan]:
         """
         Context manager for processing an event.
 
         Args:
             event: The event to be processed.
 
         Yields:
```

### Comparing `dbally-0.1.0/src/dbally/collection.py` & `dbally-0.2.0/src/dbally/collection.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 import asyncio
 import inspect
 import textwrap
 import time
-from typing import Callable, Dict, List, Optional, Tuple, Type, TypeVar
+from collections import defaultdict
+from typing import Callable, Dict, List, Optional, Type, TypeVar
 
 from dbally.audit.event_handlers.base import EventHandler
 from dbally.audit.event_tracker import EventTracker
 from dbally.data_models.audit import RequestEnd, RequestStart
 from dbally.data_models.execution_result import ExecutionResult
-from dbally.llm_client.base import LLMClient
+from dbally.llms.base import LLM
+from dbally.llms.clients.base import LLMOptions
 from dbally.nl_responder.nl_responder import NLResponder
 from dbally.similarity.index import AbstractSimilarityIndex
 from dbally.utils.errors import NoViewFoundError
 from dbally.view_selection.base import ViewSelector
-from dbally.views.base import BaseView
-from dbally.views.structured import BaseStructuredView
+from dbally.views.base import BaseView, IndexLocation
 
 
 class IndexUpdateError(Exception):
     """
     Exception for when updating any of the Collection's similarity indexes fails.
 
     Provides a dictionary mapping failed indexes to their
@@ -43,27 +44,27 @@
         function instead of instantiating this class directly.
     """
 
     def __init__(
         self,
         name: str,
         view_selector: ViewSelector,
-        llm_client: LLMClient,
+        llm: LLM,
         event_handlers: List[EventHandler],
         nl_responder: NLResponder,
         n_retries: int = 3,
     ) -> None:
         """
         Args:
             name: Name of the collection is available for [Event handlers](event_handlers/index.md) and is\
             used to distinguish different db-ally runs.
             view_selector: As you register more then one [View](views/index.md) within single collection,\
             before generating the IQL query, a View that fits query the most is selected by the\
             [ViewSelector](view_selection/index.md).
-            llm_client: LLM client used by the collection to generate views and respond to natural language queries.
+            llm: LLM used by the collection to generate views and respond to natural language queries.
             event_handlers: Event handlers used by the collection during query executions. Can be used\
             to log events as [CLIEventHandler](event_handlers/cli_handler.md) or to validate system performance\
             as [LangSmithEventHandler](event_handlers/langsmith_handler.md).
             nl_responder: Object that translates RAW response from db-ally into natural language.
             n_retries: IQL generator may produce invalid IQL. If this is the case this argument specifies\
             how many times db-ally will try to regenerate it. Previous try with the error message is\
             appended to the chat history to guide next generations.
@@ -71,15 +72,15 @@
         self.name = name
         self.n_retries = n_retries
         self._views: Dict[str, Callable[[], BaseView]] = {}
         self._builders: Dict[str, Callable[[], BaseView]] = {}
         self._view_selector = view_selector
         self._nl_responder = nl_responder
         self._event_handlers = event_handlers
-        self._llm_client = llm_client
+        self._llm = llm
 
     T = TypeVar("T", bound=BaseView)
 
     def add(self, view: Type[T], builder: Optional[Callable[[], T]] = None, name: Optional[str] = None) -> None:
         """
         Register new [View](views/index.md) that will be available to query via the collection.
 
@@ -153,15 +154,21 @@
         Returns:
             Dictionary of view names and descriptions
         """
         return {
             name: (textwrap.dedent(view.__doc__).strip() if view.__doc__ else "") for name, view in self._views.items()
         }
 
-    async def ask(self, question: str, dry_run: bool = False, return_natural_response: bool = False) -> ExecutionResult:
+    async def ask(
+        self,
+        question: str,
+        dry_run: bool = False,
+        return_natural_response: bool = False,
+        llm_options: Optional[LLMOptions] = None,
+    ) -> ExecutionResult:
         """
         Ask question in a text form and retrieve the answer based on the available views.
 
         Question answering is composed of following steps:
             1. View Selection
             2. IQL Generation
             3. IQL Parsing
@@ -169,105 +176,112 @@
             5. Query Execution
 
         Args:
             question: question posed using natural language representation e.g\
             "What job offers for Data Scientists do we have?"
             dry_run: if True, only generate the query without executing it
             return_natural_response: if True (and dry_run is False as natural response requires query results),
-                                     the natural response will be included in the answer
+                the natural response will be included in the answer
+            llm_options: options to use for the LLM client. If provided, these options will be merged with the default
+                options provided to the LLM client, prioritizing option values other than NOT_GIVEN
 
         Returns:
             ExecutionResult object representing the result of the query execution.
 
         Raises:
             ValueError: if collection is empty
             IQLError: if incorrect IQL was generated `n_retries` amount of times.
             ValueError: if incorrect IQL was generated `n_retries` amount of times.
         """
-        start_time = time.time()
+        start_time = time.monotonic()
 
         event_tracker = EventTracker.initialize_with_handlers(self._event_handlers)
 
         await event_tracker.request_start(RequestStart(question=question, collection_name=self.name))
 
         # select view
         views = self.list()
 
         if len(views) == 0:
             raise ValueError("Empty collection")
         if len(views) == 1:
             selected_view = next(iter(views))
         else:
-            selected_view = await self._view_selector.select_view(question, views, event_tracker)
+            selected_view = await self._view_selector.select_view(
+                question=question,
+                views=views,
+                event_tracker=event_tracker,
+                llm_options=llm_options,
+            )
 
         view = self.get(selected_view)
 
-        start_time_view = time.time()
+        start_time_view = time.monotonic()
         view_result = await view.ask(
             query=question,
-            llm_client=self._llm_client,
+            llm=self._llm,
             event_tracker=event_tracker,
             n_retries=self.n_retries,
             dry_run=dry_run,
+            llm_options=llm_options,
         )
-        end_time_view = time.time()
+        end_time_view = time.monotonic()
 
         textual_response = None
         if not dry_run and return_natural_response:
-            textual_response = await self._nl_responder.generate_response(view_result, question, event_tracker)
+            textual_response = await self._nl_responder.generate_response(
+                result=view_result,
+                question=question,
+                event_tracker=event_tracker,
+                llm_options=llm_options,
+            )
 
         result = ExecutionResult(
             results=view_result.results,
             context=view_result.context,
-            execution_time=time.time() - start_time,
+            execution_time=time.monotonic() - start_time,
             execution_time_view=end_time_view - start_time_view,
             view_name=selected_view,
             textual_response=textual_response,
         )
 
         await event_tracker.request_end(RequestEnd(result=result))
 
         return result
 
-    def get_similarity_indexes(self) -> Dict[AbstractSimilarityIndex, List[Tuple[str, str, str]]]:
+    def get_similarity_indexes(self) -> Dict[AbstractSimilarityIndex, List[IndexLocation]]:
         """
-        List all similarity indexes from all structured views in the collection.
+        List all similarity indexes from all views in the collection.
 
         Returns:
-            Dictionary with similarity indexes as keys and values containing lists of places where they are used
-            (represented by a tupple containing view name, method name and argument name)
+            Mapping of similarity indexes to their locations, following view format.
+            For:
+                - freeform views, the format is (view_name, table_name, column_name)
+                - structured views, the format is (view_name, filter_name, argument_name)
         """
-        indexes: Dict[AbstractSimilarityIndex, List[Tuple[str, str, str]]] = {}
+        indexes = defaultdict(list)
         for view_name in self._views:
             view = self.get(view_name)
-
-            if not isinstance(view, BaseStructuredView):
-                continue
-
-            filters = view.list_filters()
-            for filter_ in filters:
-                for param in filter_.parameters:
-                    if param.similarity_index:
-                        indexes.setdefault(param.similarity_index, []).append((view_name, filter_.name, param.name))
+            view_indexes = view.list_similarity_indexes()
+            for index, location in view_indexes.items():
+                indexes[index].extend(location)
         return indexes
 
     async def update_similarity_indexes(self) -> None:
         """
         Update all similarity indexes from all structured views in the collection.
 
         Raises:
             IndexUpdateError: if updating any of the indexes fails. The exception provides `failed_indexes` attribute,
                 a dictionary mapping failed indexes to their respective exceptions. Indexes not present in
                 the dictionary were updated successfully.
         """
         indexes = self.get_similarity_indexes()
-        update_corutines = [index.update() for index in indexes]
-        results = await asyncio.gather(*update_corutines, return_exceptions=True)
+        update_coroutines = [index.update() for index in indexes]
+        results = await asyncio.gather(*update_coroutines, return_exceptions=True)
         failed_indexes = {
             index: exception for index, exception in zip(indexes, results) if isinstance(exception, Exception)
         }
         if failed_indexes:
             failed_locations = [loc for index in failed_indexes for loc in indexes[index]]
-            description = ", ".join(
-                f"{view_name}.{method_name}.{param_name}" for view_name, method_name, param_name in failed_locations
-            )
-            raise IndexUpdateError(f"Failed to update similarity indexes for {description}", failed_indexes)
+            descriptions = ", ".join(".".join(name for name in location) for location in failed_locations)
+            raise IndexUpdateError(f"Failed to update similarity indexes for {descriptions}", failed_indexes)
```

### Comparing `dbally-0.1.0/src/dbally/data_models/audit.py` & `dbally-0.2.0/src/dbally/data_models/audit.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from dataclasses import dataclass
 from enum import Enum
 from typing import Optional, Union
 
 from dbally.data_models.execution_result import ExecutionResult
-from dbally.data_models.prompts.prompt_template import ChatFormat
+from dbally.prompts import ChatFormat
 
 
 class EventType(Enum):
     """
     Enum for event types.
     """
 
@@ -26,14 +26,27 @@
 
     completion_tokens: Optional[int] = None
     prompt_tokens: Optional[int] = None
     total_tokens: Optional[int] = None
 
 
 @dataclass
+class SimilarityEvent:
+    """
+    SimilarityEvent is fired when a SimilarityIndex lookup is performed.
+    """
+
+    store: str
+    fetcher: str
+
+    input_value: str
+    output_value: Optional[str] = None
+
+
+@dataclass
 class RequestStart:
     """
     Class representing request start data.
     """
 
     collection_name: str
     question: str
```

### Comparing `dbally-0.1.0/src/dbally/data_models/execution_result.py` & `dbally-0.2.0/src/dbally/data_models/execution_result.py`

 * *Files identical despite different names*

### Comparing `dbally-0.1.0/src/dbally/data_models/prompts/common_validation_utils.py` & `dbally-0.2.0/src/dbally/prompts/common_validation_utils.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import re
-from typing import Dict, List, Set, Tuple
+from typing import Dict, List, Set
 
-ChatFormat = Tuple[Dict[str, str], ...]
+ChatFormat = List[Dict[str, str]]
 
 
 class PromptTemplateError(Exception):
     """Error raised on incorrect PromptTemplate construction"""
 
 
 def _extract_variables(text: str) -> List[str]:
@@ -18,15 +18,15 @@
     Returns:
         list of variables extracted from text
     """
     pattern = r"\{([^}]+)\}"
     return re.findall(pattern, text)
 
 
-def _check_prompt_variables(chat: ChatFormat, variables_to_check: Set[str]) -> ChatFormat:
+def check_prompt_variables(chat: ChatFormat, variables_to_check: Set[str]) -> ChatFormat:
     """
     Function validates a given chat to make sure it contains variables required.
 
     Args:
         chat: chat to validate
         variables_to_check: set of variables to assert
```

### Comparing `dbally-0.1.0/src/dbally/data_models/prompts/iql_prompt_template.py` & `dbally-0.2.0/src/dbally/iql_generator/iql_prompt_template.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 from typing import Callable, Dict, Optional
 
-from dbally.data_models.prompts.common_validation_utils import _check_prompt_variables
-from dbally.data_models.prompts.prompt_template import ChatFormat, PromptTemplate
+from dbally.prompts import ChatFormat, PromptTemplate, check_prompt_variables
 from dbally.utils.errors import UnsupportedQueryError
 
 
 class IQLPromptTemplate(PromptTemplate):
     """
     Class for prompt templates meant for the IQL
     """
@@ -13,15 +12,15 @@
     def __init__(
         self,
         chat: ChatFormat,
         response_format: Optional[Dict[str, str]] = None,
         llm_response_parser: Callable = lambda x: x,
     ):
         super().__init__(chat, response_format, llm_response_parser)
-        self.chat = _check_prompt_variables(chat, {"filters", "question"})
+        self.chat = check_prompt_variables(chat, {"filters", "question"})
 
 
 def _validate_iql_response(llm_response: str) -> str:
     """
     Validates LLM response to IQL
 
     Args:
```

### Comparing `dbally-0.1.0/src/dbally/data_models/prompts/nl_responder_prompt_template.py` & `dbally-0.2.0/src/dbally/nl_responder/nl_responder_prompt_template.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 from typing import Callable, Dict, Optional
 
-from dbally.data_models.prompts.common_validation_utils import _check_prompt_variables
-from dbally.data_models.prompts.prompt_template import ChatFormat, PromptTemplate
+from dbally.prompts import ChatFormat, PromptTemplate, check_prompt_variables
 
 
 class NLResponderPromptTemplate(PromptTemplate):
     """
     Class for prompt templates meant for the natural response.
     """
 
@@ -21,15 +20,15 @@
         Args:
             chat: chat format
             response_format: response format
             llm_response_parser: function to parse llm response
         """
 
         super().__init__(chat, response_format, llm_response_parser)
-        self.chat = _check_prompt_variables(chat, {"rows", "question"})
+        self.chat = check_prompt_variables(chat, {"rows", "question"})
 
 
 default_nl_responder_template = NLResponderPromptTemplate(
     chat=(
         {
             "role": "system",
             "content": "You are a helpful assistant that helps answer the user's questions "
```

### Comparing `dbally-0.1.0/src/dbally/data_models/prompts/prompt_template.py` & `dbally-0.2.0/src/dbally/prompts/prompt_template.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from typing import Callable, Dict, Optional
 
 from typing_extensions import Self
 
-from dbally.data_models.prompts.common_validation_utils import ChatFormat, PromptTemplateError
+from .common_validation_utils import ChatFormat, PromptTemplateError
 
 
 def _check_chat_order(chat: ChatFormat) -> ChatFormat:
     """
     Pydantic validator. Checks if the chat template is constructed correctly (system, user, assistant alternating).
 
     Args:
@@ -37,15 +37,15 @@
 
 
 class PromptTemplate:
     """
     Class for prompt templates
 
     Attributes:
-        response_format: Optional argument used in the OpenAI API - used to force json output
+        response_format: Optional argument for OpenAI Turbo models - may be used to force json output
         llm_response_parser: Function parsing the LLM response into IQL
     """
 
     def __init__(
         self,
         chat: ChatFormat,
         response_format: Optional[Dict[str, str]] = None,
```

### Comparing `dbally-0.1.0/src/dbally/data_models/prompts/query_explainer_prompt_template.py` & `dbally-0.2.0/src/dbally/nl_responder/query_explainer_prompt_template.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 from typing import Callable, Dict, Optional
 
-from dbally.data_models.prompts.common_validation_utils import _check_prompt_variables
-from dbally.data_models.prompts.prompt_template import ChatFormat, PromptTemplate
+from dbally.prompts import ChatFormat, PromptTemplate, check_prompt_variables
 
 
 class QueryExplainerPromptTemplate(PromptTemplate):
     """
     Class for prompt templates meant to generate explanations for queries
     (when the data cannot be shown due to token limit).
 
@@ -18,15 +17,15 @@
     def __init__(
         self,
         chat: ChatFormat,
         response_format: Optional[Dict[str, str]] = None,
         llm_response_parser: Callable = lambda x: x,
     ) -> None:
         super().__init__(chat, response_format, llm_response_parser)
-        self.chat = _check_prompt_variables(chat, {"question", "query", "number_of_results"})
+        self.chat = check_prompt_variables(chat, {"question", "query", "number_of_results"})
 
 
 default_query_explainer_template = QueryExplainerPromptTemplate(
     chat=(
         {
             "role": "system",
             "content": "You are a helpful assistant that helps describe a table generated by a query "
```

### Comparing `dbally-0.1.0/src/dbally/data_models/prompts/view_selector_prompt_template.py` & `dbally-0.2.0/src/dbally/view_selection/view_selector_prompt_template.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,27 +1,26 @@
 import json
 from typing import Callable, Dict, Optional
 
-from dbally.data_models.prompts.common_validation_utils import _check_prompt_variables
-from dbally.data_models.prompts.prompt_template import ChatFormat, PromptTemplate
+from dbally.prompts import ChatFormat, PromptTemplate, check_prompt_variables
 
 
 class ViewSelectorPromptTemplate(PromptTemplate):
     """
     Class for prompt templates meant for the ViewSelector
     """
 
     def __init__(
         self,
         chat: ChatFormat,
         response_format: Optional[Dict[str, str]] = None,
         llm_response_parser: Callable = lambda x: x,
     ):
         super().__init__(chat, response_format, llm_response_parser)
-        self.chat = _check_prompt_variables(chat, {"views"})
+        self.chat = check_prompt_variables(chat, {"views"})
 
 
 def _convert_llm_json_response_to_selected_view(llm_response_json: str) -> str:
     """
     Converts LLM json response to IQL
 
     Args:
```

### Comparing `dbally-0.1.0/src/dbally/iql/_exceptions.py` & `dbally-0.2.0/src/dbally/iql/_exceptions.py`

 * *Files identical despite different names*

### Comparing `dbally-0.1.0/src/dbally/iql/_processor.py` & `dbally-0.2.0/src/dbally/iql/_processor.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import ast
-from typing import TYPE_CHECKING, Any, List, Union
+from typing import TYPE_CHECKING, Any, List, Optional, Union
 
+from dbally.audit.event_tracker import EventTracker
 from dbally.iql import syntax
 from dbally.iql._exceptions import (
     IQLArgumentParsingError,
     IQLArgumentValidationError,
     IQLError,
     IQLFunctionNotExists,
     IQLUnsupportedSyntaxError,
@@ -16,17 +17,20 @@
 
 
 class IQLProcessor:
     """
     Parses IQL string to tree structure.
     """
 
-    def __init__(self, source: str, allowed_functions: List["ExposedFunction"]):
+    def __init__(
+        self, source: str, allowed_functions: List["ExposedFunction"], event_tracker: Optional[EventTracker] = None
+    ) -> None:
         self.source = source
         self.allowed_functions = {func.name: func for func in allowed_functions}
+        self._event_tracker = event_tracker or EventTracker()
 
     async def process(self) -> syntax.Node:
         """
         Process IQL string to root IQL.Node.
 
         Returns:
             IQL.Node which is root of the tree representing IQL query.
@@ -80,15 +84,15 @@
         if len(func_def.parameters) != len(node.args):
             raise ValueError(f"The method {func.id} has incorrect number of arguments")
 
         for arg, arg_def in zip(node.args, func_def.parameters):
             arg_value = self._parse_arg(arg)
 
             if arg_def.similarity_index:
-                arg_value = await arg_def.similarity_index.similar(arg_value)
+                arg_value = await arg_def.similarity_index.similar(arg_value, event_tracker=self._event_tracker)
 
             check_result = validate_arg_type(arg_def.type, arg_value)
 
             if not check_result.valid:
                 raise IQLArgumentValidationError(message=check_result.reason or "", node=arg, source=self.source)
 
             args.append(check_result.casted_value if check_result.casted_value is not ... else arg_value)
```

### Comparing `dbally-0.1.0/src/dbally/iql/_type_validators.py` & `dbally-0.2.0/src/dbally/iql/_type_validators.py`

 * *Files identical despite different names*

### Comparing `dbally-0.1.0/src/dbally/iql/syntax.py` & `dbally-0.2.0/src/dbally/iql/syntax.py`

 * *Files identical despite different names*

### Comparing `dbally-0.1.0/src/dbally/iql_generator/iql_generator.py` & `dbally-0.2.0/src/dbally/iql_generator/iql_generator.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import copy
 from typing import Callable, List, Optional, Tuple, TypeVar
 
 from dbally.audit.event_tracker import EventTracker
-from dbally.data_models.prompts.iql_prompt_template import IQLPromptTemplate, default_iql_template
-from dbally.llm_client.base import LLMClient
-from dbally.prompts.prompt_builder import PromptBuilder
+from dbally.iql_generator.iql_prompt_template import IQLPromptTemplate, default_iql_template
+from dbally.llms.base import LLM
+from dbally.llms.clients.base import LLMOptions
 from dbally.views.exposed_functions import ExposedFunction
 
 
 class IQLGenerator:
     """
     Class used to generate IQL from natural language question.
 
@@ -22,58 +22,58 @@
     _ERROR_MSG_PREFIX = "Unfortunately, generated IQL is not valid. Please try again, \
                         generation of correct IQL is very important. Below you have errors generated by the system: \n"
 
     TException = TypeVar("TException", bound=Exception)
 
     def __init__(
         self,
-        llm_client: LLMClient,
+        llm: LLM,
         prompt_template: Optional[IQLPromptTemplate] = None,
-        prompt_builder: Optional[PromptBuilder] = None,
         promptify_view: Optional[Callable] = None,
     ) -> None:
         """
         Args:
-            llm_client: LLM client used to generate IQL
+            llm: LLM used to generate IQL
             prompt_template: If not provided by the users is set to `default_iql_template`
-            prompt_builder: PromptBuilder used to insert arguments into the prompt and adjust style per model.
             promptify_view: Function formatting filters for prompt
         """
-        self._llm_client = llm_client
+        self._llm = llm
         self._prompt_template = prompt_template or copy.deepcopy(default_iql_template)
-        self._prompt_builder = prompt_builder or PromptBuilder()
         self._promptify_view = promptify_view or _promptify_filters
 
     async def generate_iql(
         self,
         filters: List[ExposedFunction],
         question: str,
         event_tracker: EventTracker,
         conversation: Optional[IQLPromptTemplate] = None,
+        llm_options: Optional[LLMOptions] = None,
     ) -> Tuple[str, IQLPromptTemplate]:
         """
         Uses LLM to generate IQL in text form
 
         Args:
             question: user question
             filters: list of filters exposed by the view
             event_tracker: event store used to audit the generation process
             conversation: conversation to be continued
+            llm_options: options to use for the LLM client
 
         Returns:
             IQL - iql generated based on the user question
         """
         filters_for_prompt = self._promptify_view(filters)
 
         template = conversation or self._prompt_template
 
-        llm_response = await self._llm_client.text_generation(
+        llm_response = await self._llm.generate_text(
             template=template,
             fmt={"filters": filters_for_prompt, "question": question},
             event_tracker=event_tracker,
+            options=llm_options,
         )
 
         iql_filters = self._prompt_template.llm_response_parser(llm_response)
 
         if conversation is None:
             conversation = self._prompt_template
```

### Comparing `dbally-0.1.0/src/dbally/llm_client/base.py` & `dbally-0.2.0/src/dbally/view_selection/llm_view_selector.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,91 +1,83 @@
-# disable args docstring check as args are documented in OpenAI API docs
-# pylint: disable=W9015,R0914
-
-import abc
-from typing import Dict, List, Optional, Union
+import copy
+from typing import Callable, Dict, Optional
 
 from dbally.audit.event_tracker import EventTracker
-from dbally.data_models.audit import LLMEvent
-from dbally.data_models.llm_options import LLMOptions
-from dbally.prompts.prompt_builder import ChatFormat, PromptBuilder, PromptTemplate
+from dbally.iql_generator.iql_prompt_template import IQLPromptTemplate
+from dbally.llms.base import LLM
+from dbally.llms.clients.base import LLMOptions
+from dbally.view_selection.base import ViewSelector
+from dbally.view_selection.view_selector_prompt_template import default_view_selector_template
 
 
-class LLMClient(abc.ABC):
+class LLMViewSelector(ViewSelector):
     """
-    Abstract client for interaction with LLM.
+    The `LLMViewSelector` utilises LLMs to select the most suitable view to answer the user question.
+
+    Its primary function is to determine the optimal view that can effectively be used to answer a user's question.
 
-    It accepts parameters including the template, format, event tracker,
-    and optional generation parameters like frequency_penalty, max_tokens, and temperature
-    (the full list of options is provided by the [`LLMOptions` class][dbally.data_models.llm_options.LLMOptions]).
-    It constructs a prompt using the `PromptBuilder` instance and generates text using the `self.call` method.
+    The method used to select the most relevant view is `self.select_view`.
+    It formats views using view.name: view.description format and then calls LLM Client,
+    ultimately returning the name of the most suitable view.
     """
 
-    def __init__(self, model_name: str):
-        self.model_name = model_name
-        self._prompt_builder = PromptBuilder(self.model_name)
+    def __init__(
+        self,
+        llm: LLM,
+        prompt_template: Optional[IQLPromptTemplate] = None,
+        promptify_views: Optional[Callable[[Dict[str, str]], str]] = None,
+    ) -> None:
+        """
+        Args:
+            llm: LLM used to generate IQL
+            prompt_template: template for the prompt used for the view selection
+            promptify_views: Function formatting filters for prompt. By default names and descriptions of\
+            all views are concatenated
+        """
+        self._llm = llm
+        self._prompt_template = prompt_template or copy.deepcopy(default_view_selector_template)
+        self._promptify_views = promptify_views or _promptify_views
 
-    async def text_generation(  # pylint: disable=R0913
+    async def select_view(
         self,
-        template: PromptTemplate,
-        fmt: dict,
-        *,
-        event_tracker: Optional[EventTracker] = None,
-        frequency_penalty: Optional[float] = 0.0,
-        max_tokens: Optional[int] = 128,
-        n: Optional[int] = 1,
-        presence_penalty: Optional[float] = 0.0,
-        seed: Optional[int] = None,
-        stop: Optional[Union[str, List[str]]] = None,
-        temperature: Optional[float] = 1.0,
-        top_p: Optional[float] = 1.0,
+        question: str,
+        views: Dict[str, str],
+        event_tracker: EventTracker,
+        llm_options: Optional[LLMOptions] = None,
     ) -> str:
         """
-        For a given a PromptType and format dict creates a prompt and
-        returns the response from LLM.
+        Based on user question and list of available views select the most relevant one by prompting LLM.
+
+        Args:
+            question: user question asked in the natural language e.g "Do we have any data scientists?"
+            views: dictionary of available view names with corresponding descriptions.
+            event_tracker: event tracker used to audit the selection process.
+            llm_options: options to use for the LLM client.
 
         Returns:
-            Text response from LLM.
+            The most relevant view name.
         """
 
-        options = LLMOptions(
-            frequency_penalty=frequency_penalty,
-            max_tokens=max_tokens,
-            n=n,
-            presence_penalty=presence_penalty,
-            seed=seed,
-            stop=stop,
-            temperature=temperature,
-            top_p=top_p,
-        )
-
-        prompt = self._prompt_builder.build(template, fmt)
+        views_for_prompt = self._promptify_views(views)
 
-        event = LLMEvent(prompt=prompt, type=type(template).__name__)
+        llm_response = await self._llm.generate_text(
+            template=self._prompt_template,
+            fmt={"views": views_for_prompt, "question": question},
+            event_tracker=event_tracker,
+            options=llm_options,
+        )
+        selected_view = self._prompt_template.llm_response_parser(llm_response)
+        return selected_view
 
-        event_tracker = event_tracker or EventTracker()
-        async with event_tracker.track_event(event) as span:
-            event.response = await self.call(prompt, template.response_format, options, event)
-            span(event)
 
-        return event.response
+def _promptify_views(views: Dict[str, str]) -> str:
+    """
+    Formats views for prompt
 
-    @abc.abstractmethod
-    async def call(
-        self,
-        prompt: Union[str, ChatFormat],
-        response_format: Optional[Dict[str, str]],
-        options: LLMOptions,
-        event: LLMEvent,
-    ) -> str:
-        """
-        Calls LLM API endpoint.
+    Args:
+        views: dictionary of available view names with corresponding descriptions.
 
-        Args:
-            prompt: prompt passed to the LLM.
-            response_format: Optional argument used in the OpenAI API - used to force a json output
-            options: Additional settings used by LLM.
-            event: an LLMEvent instance which fields should be filled during the method execution.
+    Returns:
+        views_for_prompt: views formatted for prompt
+    """
 
-        Returns:
-            Response string from LLM.
-        """
+    return "\n".join([f"{name}: {description}" for name, description in views.items()])
```

### Comparing `dbally-0.1.0/src/dbally/nl_responder/nl_responder.py` & `dbally-0.2.0/src/dbally/nl_responder/nl_responder.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,102 +1,97 @@
 import copy
 from typing import Dict, List, Optional
 
 import pandas as pd
 
 from dbally.audit.event_tracker import EventTracker
 from dbally.data_models.execution_result import ViewExecutionResult
-from dbally.data_models.prompts.nl_responder_prompt_template import (
-    NLResponderPromptTemplate,
-    default_nl_responder_template,
-)
-from dbally.data_models.prompts.query_explainer_prompt_template import (
+from dbally.llms.base import LLM
+from dbally.llms.clients.base import LLMOptions
+from dbally.nl_responder.nl_responder_prompt_template import NLResponderPromptTemplate, default_nl_responder_template
+from dbally.nl_responder.query_explainer_prompt_template import (
     QueryExplainerPromptTemplate,
     default_query_explainer_template,
 )
-from dbally.llm_client.base import LLMClient
-from dbally.nl_responder.token_counters import count_tokens_for_huggingface, count_tokens_for_openai
 
 
 class NLResponder:
     """Class used to generate natural language response from the database output."""
 
     # Keys used to extract the query from the context (ordered by priority)
     QUERY_KEYS = ["iql", "sql", "query"]
 
     def __init__(
         self,
-        llm_client: LLMClient,
+        llm: LLM,
         query_explainer_prompt_template: Optional[QueryExplainerPromptTemplate] = None,
         nl_responder_prompt_template: Optional[NLResponderPromptTemplate] = None,
         max_tokens_count: int = 4096,
     ) -> None:
         """
         Args:
-            llm_client: LLM client used to generate natural language response
-            query_explainer_prompt_template: template for the prompt used to generate the iql explanation\
-            if not set defaults to `default_query_explainer_template`
-            nl_responder_prompt_template: template for the prompt used to generate the NL response\
-            if not set defaults to `nl_responder_prompt_template`
+            llm: LLM used to generate natural language response
+            query_explainer_prompt_template: template for the prompt used to generate the iql explanation
+                if not set defaults to `default_query_explainer_template`
+            nl_responder_prompt_template: template for the prompt used to generate the NL response
+                if not set defaults to `nl_responder_prompt_template`
             max_tokens_count: maximum number of tokens that can be used in the prompt
         """
-
-        self._llm_client = llm_client
+        self._llm = llm
         self._nl_responder_prompt_template = nl_responder_prompt_template or copy.deepcopy(
             default_nl_responder_template
         )
         self._query_explainer_prompt_template = query_explainer_prompt_template or copy.deepcopy(
             default_query_explainer_template
         )
         self._max_tokens_count = max_tokens_count
 
-    async def generate_response(self, result: ViewExecutionResult, question: str, event_tracker: EventTracker) -> str:
+    async def generate_response(
+        self,
+        result: ViewExecutionResult,
+        question: str,
+        event_tracker: EventTracker,
+        llm_options: Optional[LLMOptions] = None,
+    ) -> str:
         """
         Uses LLM to generate a response in natural language form.
 
         Args:
             result: object representing the result of the query execution
             question: user question
             event_tracker: event store used to audit the generation process
+            llm_options: options to use for the LLM client.
 
         Returns:
             Natural language response to the user question.
         """
-
         rows = _promptify_rows(result.results)
 
-        if "gpt" in self._llm_client.model_name:
-            tokens_count = count_tokens_for_openai(
-                messages=self._nl_responder_prompt_template.chat,
-                fmt={"rows": rows, "question": question},
-                model=self._llm_client.model_name,
-            )
-
-        else:
-            tokens_count = count_tokens_for_huggingface(
-                messages=self._nl_responder_prompt_template.chat,
-                fmt={"rows": rows, "question": question},
-                model=self._llm_client.model_name,
-            )
+        tokens_count = self._llm.count_tokens(
+            messages=self._nl_responder_prompt_template.chat,
+            fmt={"rows": rows, "question": question},
+        )
 
         if tokens_count > self._max_tokens_count:
             context = result.context
             query = next((context.get(key) for key in self.QUERY_KEYS if context.get(key)), question)
-            llm_response = await self._llm_client.text_generation(
+            llm_response = await self._llm.generate_text(
                 template=self._query_explainer_prompt_template,
                 fmt={"question": question, "query": query, "number_of_results": len(result.results)},
                 event_tracker=event_tracker,
+                options=llm_options,
             )
 
             return llm_response
 
-        llm_response = await self._llm_client.text_generation(
+        llm_response = await self._llm.generate_text(
             template=self._nl_responder_prompt_template,
             fmt={"rows": _promptify_rows(result.results), "question": question},
             event_tracker=event_tracker,
+            options=llm_options,
         )
         return llm_response
 
 
 def _promptify_rows(rows: List[Dict]) -> str:
     """
     Formats rows into a markdown table.
```

### Comparing `dbally-0.1.0/src/dbally/similarity/__init__.py` & `dbally-0.2.0/src/dbally/similarity/__init__.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,26 +1,39 @@
 from .fetcher import SimilarityFetcher
 from .index import AbstractSimilarityIndex, SimilarityIndex
 from .sqlalchemy_base import SimpleSqlAlchemyFetcher, SqlAlchemyFetcher
 from .store import SimilarityStore
 
 # depends on the faiss package
+
 try:
     from .faiss_store import FaissStore
 except ImportError:
     pass
 
 try:
     from .chroma_store import ChromadbStore
 except ImportError:
     pass
 
+try:
+    from .elasticsearch_store import ElasticsearchStore
+except ImportError:
+    pass
+
+try:
+    from .elastic_vector_search import ElasticVectorStore
+except ImportError:
+    pass
+
 __all__ = [
     "AbstractSimilarityIndex",
     "SimilarityIndex",
     "SqlAlchemyFetcher",
     "SimpleSqlAlchemyFetcher",
     "SimilarityStore",
     "SimilarityFetcher",
     "FaissStore",
+    "ElasticsearchStore",
+    "ElasticVectorStore",
     "ChromadbStore",
 ]
```

### Comparing `dbally-0.1.0/src/dbally/similarity/chroma_store.py` & `dbally-0.2.0/src/dbally/similarity/chroma_store.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 from hashlib import sha256
 from typing import List, Literal, Optional, Union
 
 import chromadb
 
-from dbally.embedding_client.base import EmbeddingClient
+from dbally.embeddings.base import EmbeddingClient
 from dbally.similarity.store import SimilarityStore
 
 
 class ChromadbStore(SimilarityStore):
     """Class that stores text embeddings using [Chroma](https://docs.trychroma.com/)"""
 
     def __init__(
         self,
         index_name: str,
-        chroma_client: chromadb.Client,
+        chroma_client: chromadb.ClientAPI,
         embedding_function: Union[EmbeddingClient, chromadb.EmbeddingFunction],
         max_distance: Optional[float] = None,
         distance_method: Literal["l2", "ip", "cosine"] = "l2",
     ):
         super().__init__()
         self.index_name = index_name
         self.chroma_client = chroma_client
@@ -90,7 +90,16 @@
         if isinstance(self.embedding_function, EmbeddingClient):
             embedding = await self.embedding_function.get_embeddings([text])
             retrieved = collection.query(query_embeddings=embedding, n_results=1)
         else:
             retrieved = collection.query(query_texts=[text], n_results=1)
 
         return self._return_best_match(retrieved)
+
+    def __repr__(self) -> str:
+        """
+        Returns the string representation of the object.
+
+        Returns:
+            str: The string representation of the object.
+        """
+        return f"{self.__class__.__name__}(index_name={self.index_name})"
```

### Comparing `dbally-0.1.0/src/dbally/similarity/faiss_store.py` & `dbally-0.2.0/src/dbally/similarity/faiss_store.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from pathlib import Path
 from typing import List, Optional
 
 import faiss
 import numpy as np
 
-from dbally.embedding_client.base import EmbeddingClient
+from dbally.embeddings.base import EmbeddingClient
 from dbally.similarity.store import SimilarityStore
 
 
 class FaissStore(SimilarityStore):
     """
     The FaissStore class stores text embeddings using Meta Faiss.
     """
@@ -88,7 +88,16 @@
         best_distance, best_idx = scores[0][0], similar[0][0]
 
         if best_idx != -1 and (self.max_distance is None or best_distance <= self.max_distance):
             with open(self.get_index_path().with_suffix(".npy"), "rb") as file:
                 data = np.load(file)
                 return data[best_idx]
         return None
+
+    def __repr__(self) -> str:
+        """
+        Returns the string representation of the FaissStore.
+
+        Returns:
+            str: The string representation of the FaissStore.
+        """
+        return f"{self.__class__.__name__}(index_dir={self.index_dir}, index_name={self.index_name})"
```

### Comparing `dbally-0.1.0/src/dbally/similarity/sqlalchemy_base.py` & `dbally-0.2.0/src/dbally/similarity/sqlalchemy_base.py`

 * *Files 5% similar despite different names*

```diff
@@ -32,14 +32,23 @@
         Returns:
             The fetched data.
         """
         with self.sqlalchemy_engine.connect() as conn:
             result = conn.execute(self.get_query())
             return [row[0] for row in result]
 
+    def __repr__(self) -> str:
+        """
+        Returns a string representation of the fetcher.
+
+        Returns:
+            str: The string representation of the fetcher.
+        """
+        return f"{self.__class__.__name__}()"
+
 
 class SimpleSqlAlchemyFetcher(SqlAlchemyFetcher):
     """
     Fetches the data from a single column in the database.
     """
 
     def __init__(
@@ -54,14 +63,23 @@
         Returns query that will be used to fetch the data from the database.
 
         Returns:
             The query to fetch the data.
         """
         return sqlalchemy.select(self.column).select_from(self.table).distinct()
 
+    def __repr__(self) -> str:
+        """
+        Returns a string representation of the fetcher.
+
+        Returns:
+            str: The string representation of the fetcher.
+        """
+        return f"{self.__class__.__name__}(table={self.table.name}, column={self.column.name})"
+
 
 class AbstractSqlAlchemyStore(SimilarityStore, metaclass=abc.ABCMeta):
     """
     Stores the data in the database using SQLAlchemy.
     """
 
     def __init__(self, sqlalchemy_engine: sqlalchemy.engine.Engine, table_name: str, threshold: float = 0.8) -> None:
```

### Comparing `dbally-0.1.0/src/dbally/similarity/store.py` & `dbally-0.2.0/src/dbally/similarity/store.py`

 * *Files identical despite different names*

### Comparing `dbally-0.1.0/src/dbally/view_selection/llm_view_selector.py` & `dbally-0.2.0/src/dbally/llms/base.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,74 +1,104 @@
-import copy
-from typing import Callable, Dict, Optional
+from abc import ABC, abstractmethod
+from functools import cached_property
+from typing import Dict, Generic, Optional, Type
 
 from dbally.audit.event_tracker import EventTracker
-from dbally.data_models.prompts import IQLPromptTemplate, default_view_selector_template
-from dbally.llm_client.base import LLMClient
-from dbally.prompts import PromptBuilder
-from dbally.view_selection.base import ViewSelector
+from dbally.data_models.audit import LLMEvent
+from dbally.llms.clients.base import LLMClient, LLMClientOptions, LLMOptions
+from dbally.prompts.common_validation_utils import ChatFormat
+from dbally.prompts.prompt_template import PromptTemplate
 
 
-class LLMViewSelector(ViewSelector):
+class LLM(Generic[LLMClientOptions], ABC):
     """
-    The `LLMViewSelector` utilises LLMs to select the most suitable view to answer the user question.
-
-    Its primary function is to determine the optimal view that can effectively be used to answer a user's question.
-
-    The method used to select the most relevant view is `self.select_view`.
-    It formats views using view.name: view.description format and then calls LLM Client,
-    ultimately returning the name of the most suitable view.
+    Abstract class for interaction with Large Language Model.
     """
 
-    def __init__(
-        self,
-        llm_client: LLMClient,
-        prompt_template: Optional[IQLPromptTemplate] = None,
-        prompt_builder: Optional[PromptBuilder] = None,
-        promptify_views: Optional[Callable[[Dict[str, str]], str]] = None,
-    ) -> None:
+    _options_cls: Type[LLMClientOptions]
+
+    def __init__(self, model_name: str, default_options: Optional[LLMOptions] = None) -> None:
         """
+        Constructs a new LLM instance.
+
         Args:
-            llm_client: LLM client used to generate IQL
-            prompt_template: template for the prompt used for the view selection
-            prompt_builder: PromptBuilder used to insert arguments into the prompt and adjust style per model
-            promptify_views: Function formatting filters for prompt. By default names and descriptions of\
-            all views are concatenated
-        """
-        self._llm_client = llm_client
-        self._prompt_template = prompt_template or copy.deepcopy(default_view_selector_template)
-        self._prompt_builder = prompt_builder or PromptBuilder()
-        self._promptify_views = promptify_views or _promptify_views
+            model_name: Name of the model to be used.
+            default_options: Default options to be used.
 
-    async def select_view(self, question: str, views: Dict[str, str], event_tracker: EventTracker) -> str:
+        Raises:
+            TypeError: If the subclass is missing the '_options_cls' attribute.
         """
-        Based on user question and list of available views select the most relevant one by prompting LLM.
+        self.model_name = model_name
+        self.default_options = default_options or self._options_cls()
+
+    def __init_subclass__(cls) -> None:
+        if not hasattr(cls, "_options_cls"):
+            raise TypeError(f"Class {cls.__name__} is missing the '_options_cls' attribute")
+
+    @cached_property
+    @abstractmethod
+    def client(self) -> LLMClient:
+        """
+        Client for the LLM.
+        """
+
+    def format_prompt(self, template: PromptTemplate, fmt: Dict[str, str]) -> ChatFormat:
+        """
+        Applies formatting to the prompt template.
 
         Args:
-            question: user question asked in the natural language e.g "Do we have any data scientists?"
-            views: dictionary of available view names with corresponding descriptions.
-            event_tracker: event tracker used to audit the selection process.
+            template: Prompt template in system/user/assistant openAI format.
+            fmt: Dictionary with formatting.
 
         Returns:
-            The most relevant view name.
+            Prompt in the format of the client.
         """
+        return [{**message, "content": message["content"].format(**fmt)} for message in template.chat]
 
-        views_for_prompt = self._promptify_views(views)
+    def count_tokens(self, messages: ChatFormat, fmt: Dict[str, str]) -> int:
+        """
+        Counts tokens in the messages.
 
-        llm_response = await self._llm_client.text_generation(
-            self._prompt_template, fmt={"views": views_for_prompt, "question": question}, event_tracker=event_tracker
-        )
-        selected_view = self._prompt_template.llm_response_parser(llm_response)
-        return selected_view
+        Args:
+            messages: Messages to count tokens for.
+            fmt: Arguments to be used with prompt.
 
+        Returns:
+            Number of tokens in the messages.
+        """
+        return sum(len(message["content"].format(**fmt)) for message in messages)
 
-def _promptify_views(views: Dict[str, str]) -> str:
-    """
-    Formats views for prompt
+    async def generate_text(
+        self,
+        template: PromptTemplate,
+        fmt: Dict[str, str],
+        *,
+        event_tracker: Optional[EventTracker] = None,
+        options: Optional[LLMOptions] = None,
+    ) -> str:
+        """
+        Prepares and sends a prompt to the LLM and returns the response.
 
-    Args:
+        Args:
+            template: Prompt template in system/user/assistant openAI format.
+            fmt: Dictionary with formatting.
+            event_tracker: Event store used to audit the generation process.
+            options: Options to use for the LLM client.
 
-    Returns:
-        views_for_prompt: views formatted for prompt
-    """
+        Returns:
+            Text response from LLM.
+        """
+        options = (self.default_options | options) if options else self.default_options
+        prompt = self.format_prompt(template, fmt)
+        event = LLMEvent(prompt=prompt, type=type(template).__name__)
+        event_tracker = event_tracker or EventTracker()
+
+        async with event_tracker.track_event(event) as span:
+            event.response = await self.client.call(
+                prompt=prompt,
+                response_format=template.response_format,
+                options=options,
+                event=event,
+            )
+            span(event)
 
-    return "\n".join([f"{name}: {description}" for name, description in views.items()])
+        return event.response
```

### Comparing `dbally-0.1.0/src/dbally/views/base.py` & `dbally-0.2.0/src/dbally/views/base.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,30 +1,51 @@
 import abc
+from typing import Dict, List, Optional, Tuple
 
 from dbally.audit.event_tracker import EventTracker
 from dbally.data_models.execution_result import ViewExecutionResult
-from dbally.llm_client.base import LLMClient
+from dbally.llms.base import LLM
+from dbally.llms.clients.base import LLMOptions
+from dbally.similarity import AbstractSimilarityIndex
+
+IndexLocation = Tuple[str, str, str]
 
 
 class BaseView(metaclass=abc.ABCMeta):
     """
     Base class for all [Views](../../concepts/views.md), which are the main building blocks of db-ally. All classes\
     implementing this interface have to be able to execute queries and return the result.
     """
 
     @abc.abstractmethod
     async def ask(
-        self, query: str, llm_client: LLMClient, event_tracker: EventTracker, n_retries: int = 3, dry_run: bool = False
+        self,
+        query: str,
+        llm: LLM,
+        event_tracker: EventTracker,
+        n_retries: int = 3,
+        dry_run: bool = False,
+        llm_options: Optional[LLMOptions] = None,
     ) -> ViewExecutionResult:
         """
         Executes the query and returns the result.
 
         Args:
             query: The natural language query to execute.
-            llm_client: The LLM client used to execute the query.
+            llm: The LLM used to execute the query.
             event_tracker: The event tracker used to audit the query execution.
             n_retries: The number of retries to execute the query in case of errors.
             dry_run: If True, the query will not be used to fetch data from the datasource.
+            llm_options: Options to use for the LLM.
 
         Returns:
             The result of the query.
         """
+
+    def list_similarity_indexes(self) -> Dict[AbstractSimilarityIndex, List[IndexLocation]]:
+        """
+        Lists all the similarity indexes used by the view.
+
+        Returns:
+            Mapping of similarity indexes to their locations.
+        """
+        return {}
```

### Comparing `dbally-0.1.0/src/dbally/views/exposed_functions.py` & `dbally-0.2.0/src/dbally/views/exposed_functions.py`

 * *Files identical despite different names*

### Comparing `dbally-0.1.0/src/dbally/views/freeform/text2sql/_view.py` & `dbally-0.2.0/src/dbally/views/structured.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,116 +1,129 @@
-from typing import Iterable, Tuple
-
-import sqlalchemy
-from sqlalchemy import text
+import abc
+from collections import defaultdict
+from typing import Dict, List, Optional
 
 from dbally.audit.event_tracker import EventTracker
 from dbally.data_models.execution_result import ViewExecutionResult
-from dbally.data_models.prompts import PromptTemplate
-from dbally.llm_client.base import LLMClient
-from dbally.views.base import BaseView
-
-from ._config import Text2SQLConfig
-from ._errors import Text2SQLError
-
-text2sql_prompt = PromptTemplate(
-    chat=(
-        {
-            "role": "system",
-            "content": "You are a very smart database programmer. "
-            "You have access to the following {dialect} tables:\n"
-            "{tables}\n"
-            "Create SQL query to answer user question. Return only SQL surrounded in ```sql <QUERY> ``` block.\n",
-        },
-        {"role": "user", "content": "{question}"},
-    ),
-)
+from dbally.iql import IQLError, IQLQuery
+from dbally.iql_generator.iql_generator import IQLGenerator
+from dbally.llms.base import LLM
+from dbally.llms.clients.base import LLMOptions
+from dbally.views.exposed_functions import ExposedFunction
+
+from ..similarity import AbstractSimilarityIndex
+from .base import BaseView, IndexLocation
 
 
-class Text2SQLFreeformView(BaseView):
+class BaseStructuredView(BaseView):
     """
-    Text2SQLFreeformView is a class designed to interact with the database using text2sql queries.
+    Base class for all structured [Views](../../concepts/views.md). All classes implementing this interface has\
+    to be able to list all available filters, apply them and execute queries.
     """
 
-    def __init__(self, engine: sqlalchemy.engine.Engine, config: Text2SQLConfig) -> None:
-        super().__init__()
-        self._engine = engine
-        self._config = config
+    def get_iql_generator(self, llm: LLM) -> IQLGenerator:
+        """
+        Returns the IQL generator for the view.
+
+        Args:
+            llm: LLM used to generate the IQL queries
+
+        Returns:
+            IQLGenerator: IQL generator for the view
+        """
+        return IQLGenerator(llm=llm)
 
     async def ask(
-        self, query: str, llm_client: LLMClient, event_tracker: EventTracker, n_retries: int = 3, dry_run: bool = False
+        self,
+        query: str,
+        llm: LLM,
+        event_tracker: EventTracker,
+        n_retries: int = 3,
+        dry_run: bool = False,
+        llm_options: Optional[LLMOptions] = None,
     ) -> ViewExecutionResult:
         """
-        Executes the query and returns the result. It generates the SQL query from the natural language query and
-        executes it against the database. It retries the process in case of errors.
+        Executes the query and returns the result. It generates the IQL query from the natural language query\
+        and applies the filters to the view. It retries the process in case of errors.
 
         Args:
             query: The natural language query to execute.
-            llm_client: The LLM client used to execute the query.
+            llm: The LLM used to execute the query.
             event_tracker: The event tracker used to audit the query execution.
             n_retries: The number of retries to execute the query in case of errors.
             dry_run: If True, the query will not be used to fetch data from the datasource.
+            llm_options: Options to use for the LLM.
 
         Returns:
             The result of the query.
-
-        Raises:
-            Text2SQLError: If the text2sql query generation fails after n_retries.
         """
+        iql_generator = self.get_iql_generator(llm)
+        filter_list = self.list_filters()
 
-        conversation = text2sql_prompt
-        sql, rows = None, None
-        exceptions = []
+        iql_filters, conversation = await iql_generator.generate_iql(
+            question=query,
+            filters=filter_list,
+            event_tracker=event_tracker,
+            llm_options=llm_options,
+        )
 
         for _ in range(n_retries):
-            # We want to catch all exceptions to retry the process.
-            # pylint: disable=broad-except
             try:
-                sql, conversation = await self._generate_sql(query, conversation, llm_client, event_tracker)
-
-                if dry_run:
-                    return ViewExecutionResult(results=[], context={"sql": sql})
-
-                rows = await self._execute_sql(sql)
+                filters = await IQLQuery.parse(iql_filters, filter_list, event_tracker=event_tracker)
+                await self.apply_filters(filters)
                 break
-            except Exception as e:
-                conversation = conversation.add_user_message(f"Query is invalid! Error: {e}")
-                exceptions.append(e)
+            except (IQLError, ValueError) as e:
+                conversation = iql_generator.add_error_msg(conversation, [e])
+                iql_filters, conversation = await iql_generator.generate_iql(
+                    question=query,
+                    filters=filter_list,
+                    event_tracker=event_tracker,
+                    conversation=conversation,
+                    llm_options=llm_options,
+                )
                 continue
 
-        if rows is None:
-            raise Text2SQLError("Text2SQL query generation failed", exceptions=exceptions) from exceptions[-1]
+        result = self.execute(dry_run=dry_run)
+        result.context["iql"] = iql_filters
 
-        # The underscore is used by sqlalchemy to avoid conflicts with column names
-        # pylint: disable=protected-access
-        return ViewExecutionResult(
-            results=[dict(row._mapping) for row in rows],
-            context={
-                "sql": sql,
-            },
-        )
+        return result
 
-    async def _generate_sql(
-        self, query: str, conversation: PromptTemplate, llm_client: LLMClient, event_tracker: EventTracker
-    ) -> Tuple[str, PromptTemplate]:
-        response = await llm_client.text_generation(
-            template=conversation,
-            fmt={"tables": self._get_tables_context(), "dialect": self._engine.dialect.name, "question": query},
-            event_tracker=event_tracker,
-        )
+    @abc.abstractmethod
+    def list_filters(self) -> List[ExposedFunction]:
+        """
+
+        Returns:
+            Filters defined inside the View.
+        """
+
+    @abc.abstractmethod
+    async def apply_filters(self, filters: IQLQuery) -> None:
+        """
+        Applies the chosen filters to the view.
+
+        Args:
+            filters: [IQLQuery](../../concepts/iql.md) object representing the filters to apply
+        """
+
+    @abc.abstractmethod
+    def execute(self, dry_run: bool = False) -> ViewExecutionResult:
+        """
+        Executes the query and returns the result.
 
-        conversation = conversation.add_assistant_message(response)
+        Args:
+            dry_run: if True, should only generate the query without executing it
+        """
 
-        response = response.split("```sql")[-1].strip("\n")
-        response = response.replace("```", "")
-        return response, conversation
-
-    async def _execute_sql(self, sql: str) -> Iterable:
-        with self._engine.connect() as conn:
-            return conn.execute(text(sql)).fetchall()
-
-    def _get_tables_context(self) -> str:
-        context = ""
-        for table in self._config.tables.values():
-            context += f"{table.ddl}\n"
+    def list_similarity_indexes(self) -> Dict[AbstractSimilarityIndex, List[IndexLocation]]:
+        """
+        Lists all the similarity indexes used by the view.
 
-        return context
+        Returns:
+            Mapping of similarity indexes to their locations in the (view_name, filter_name, argument_name) format.
+        """
+        indexes = defaultdict(list)
+        filters = self.list_filters()
+        for filter_ in filters:
+            for param in filter_.parameters:
+                if param.similarity_index:
+                    indexes[param.similarity_index].append((self.__class__.__name__, filter_.name, param.name))
+        return indexes
```

### Comparing `dbally-0.1.0/src/dbally/views/methods_base.py` & `dbally-0.2.0/src/dbally/views/methods_base.py`

 * *Files identical despite different names*

### Comparing `dbally-0.1.0/src/dbally/views/pandas_base.py` & `dbally-0.2.0/src/dbally/views/pandas_base.py`

 * *Files identical despite different names*

### Comparing `dbally-0.1.0/src/dbally/views/sqlalchemy_base.py` & `dbally-0.2.0/src/dbally/views/sqlalchemy_base.py`

 * *Files identical despite different names*

### Comparing `dbally-0.1.0/src/dbally.egg-info/PKG-INFO` & `dbally-0.2.0/src/dbally.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbally
-Version: 0.1.0
+Version: 0.2.0
 Summary: "Efficient, consistent and secure library for querying structured data with natural language"
 Author: deepsense.ai
 Author-email: contact@deepsense.ai
 License: MIT
 Project-URL: Documentation, https://db-ally.deepsense.ai/
 Project-URL: Source, https://github.com/deepsense-ai/db-ally
 Classifier: Development Status :: 2 - Pre-Alpha
@@ -22,39 +22,38 @@
 License-File: LICENSE
 Requires-Dist: pandas~=2.0.3
 Requires-Dist: python-dotenv>=0.5.1
 Requires-Dist: SQLAlchemy==2.0.25
 Requires-Dist: tabulate>=0.9.0
 Requires-Dist: click~=8.1.7
 Requires-Dist: numpy>=1.24.0
-Provides-Extra: openai
-Requires-Dist: openai>=1.10.0; extra == "openai"
-Requires-Dist: tiktoken>=0.6.0; extra == "openai"
+Provides-Extra: litellm
+Requires-Dist: litellm>=1.37.9; extra == "litellm"
 Provides-Extra: faiss
 Requires-Dist: faiss-cpu>=1.8.0; extra == "faiss"
+Provides-Extra: chromadb
+Requires-Dist: chromadb>=0.4.24; extra == "chromadb"
+Provides-Extra: langsmith
+Requires-Dist: langsmith~=0.1.57; extra == "langsmith"
 Provides-Extra: examples
 Requires-Dist: pydantic~=2.6.0; extra == "examples"
 Requires-Dist: pydantic_settings~=2.1.0; extra == "examples"
 Requires-Dist: psycopg2-binary~=2.9.9; extra == "examples"
-Provides-Extra: langsmith
-Requires-Dist: langsmith>=0.0.87; extra == "langsmith"
-Provides-Extra: transformers
-Requires-Dist: transformers>=4.37.1; extra == "transformers"
 Provides-Extra: benchmark
 Requires-Dist: asyncpg~=0.28.0; extra == "benchmark"
 Requires-Dist: eval-type-backport~=0.1.3; extra == "benchmark"
 Requires-Dist: hydra-core~=1.3.2; extra == "benchmark"
 Requires-Dist: loguru~=0.7.0; extra == "benchmark"
 Requires-Dist: neptune~=1.6.3; extra == "benchmark"
 Requires-Dist: pydantic~=2.6.1; extra == "benchmark"
 Requires-Dist: pydantic-core~=2.16.2; extra == "benchmark"
 Requires-Dist: pydantic-settings~=2.0.3; extra == "benchmark"
 Requires-Dist: psycopg2-binary~=2.9.9; extra == "benchmark"
-Provides-Extra: chromadb
-Requires-Dist: chromadb>=0.4.24; extra == "chromadb"
+Provides-Extra: elasticsearch
+Requires-Dist: elasticsearch==8.13.1; extra == "elasticsearch"
 
 # <h1 align="center">db-ally</h1>
 
 <p align="center">
     <em>Efficient, consistent and secure library for querying structured data with natural language</em>
 </p>
 
@@ -81,15 +80,15 @@
 
 In db-ally, developers define their use cases by implementing [**views**](https://db-ally.deepsense.ai/concepts/views) and **filters**. A list of possible filters is presented to the LLM in terms of [**IQL**](https://db-ally.deepsense.ai/concepts/iql) (Intermediate Query Language). Views are grouped and registered within a [**collection**](https://db-ally.deepsense.ai/concepts/views), which then serves as an entry point for asking questions in natural language.
 
 This is a basic implementation of a db-ally view for an example HR application, which retrieves candidates from an SQL database:
 
 ```python
 from dbally import decorators, SqlAlchemyBaseView, create_collection
-from dbally.llm_client.openai_client import OpenAIClient
+from dbally.llms.litellm import LiteLLM
 from sqlalchemy import create_engine
 
 class CandidateView(SqlAlchemyBaseView):
     """
     A view for retrieving candidates from the database.
     """
 
@@ -103,15 +102,15 @@
     def from_country(self, country: str):
         """
         Filter candidates from a specific country.
         """
         return Candidate.country == country
 
 engine = create_engine('sqlite:///candidates.db')
-llm = OpenAIClient(model_name="gpt-3.5-turbo")
+llm = LiteLLM(model_name="gpt-3.5-turbo")
 my_collection = create_collection("collection_name", llm)
 my_collection.add(CandidateView, lambda: CandidateView(engine))
 
 my_collection.ask("Find candidates from United States")
 ```
 
 For a concrete step-by-step example on how to use db-ally, go to [Quickstart](https://db-ally.deepsense.ai/quickstart/) guide. For a more learning-oriented experience, check our db-ally [Tutorial](https://db-ally.deepsense.ai/tutorials/tutorial_1).
@@ -132,20 +131,20 @@
 
 ```bash
 pip install dbally
 ```
 
 Additionally, you can install one of our extensions to use specific features.
 
-* `dbally[openai]`: Use [OpenAI's models](https://platform.openai.com/docs/models)
+* `dbally[litellm]`: Use [100+ LLMs](https://docs.litellm.ai/docs/providers)
 * `dbally[faiss]`: Use [Faiss](https://github.com/facebookresearch/faiss) indexes for similarity search
 * `dbally[langsmith]`: Use [LangSmith](https://www.langchain.com/langsmith) for query tracking
 
 ```bash
-pip install dbally[openai,faiss,langsmith]
+pip install dbally[litellm,faiss,langsmith]
 ```
 
 ## License
 
 db-ally is released under MIT license.
 
 ## How db-ally documentation is organized
```

### Comparing `dbally-0.1.0/src/dbally.egg-info/SOURCES.txt` & `dbally-0.2.0/src/dbally.egg-info/SOURCES.txt`

 * *Files 11% similar despite different names*

```diff
@@ -3,15 +3,17 @@
 README.md
 pyproject.toml
 setup.cfg
 setup.py
 src/py.typed
 src/dbally/__init__.py
 src/dbally/__version__.py
+src/dbally/_exceptions.py
 src/dbally/_main.py
+src/dbally/_types.py
 src/dbally/collection.py
 src/dbally/py.typed
 src/dbally.egg-info/PKG-INFO
 src/dbally.egg-info/SOURCES.txt
 src/dbally.egg-info/dependency_links.txt
 src/dbally.egg-info/entry_points.txt
 src/dbally.egg-info/not-zip-safe
@@ -26,65 +28,67 @@
 src/dbally/audit/event_handlers/__init__.py
 src/dbally/audit/event_handlers/base.py
 src/dbally/audit/event_handlers/cli_event_handler.py
 src/dbally/audit/event_handlers/langsmith_event_handler.py
 src/dbally/data_models/__init__.py
 src/dbally/data_models/audit.py
 src/dbally/data_models/execution_result.py
-src/dbally/data_models/llm_options.py
-src/dbally/data_models/prompts/__init__.py
-src/dbally/data_models/prompts/common_validation_utils.py
-src/dbally/data_models/prompts/iql_prompt_template.py
-src/dbally/data_models/prompts/nl_responder_prompt_template.py
-src/dbally/data_models/prompts/prompt_template.py
-src/dbally/data_models/prompts/query_explainer_prompt_template.py
-src/dbally/data_models/prompts/view_selector_prompt_template.py
-src/dbally/embedding_client/__init__.py
-src/dbally/embedding_client/base.py
-src/dbally/embedding_client/openai.py
+src/dbally/embeddings/__init__.py
+src/dbally/embeddings/_exceptions.py
+src/dbally/embeddings/base.py
+src/dbally/embeddings/litellm.py
 src/dbally/iql/__init__.py
 src/dbally/iql/_exceptions.py
 src/dbally/iql/_processor.py
 src/dbally/iql/_query.py
 src/dbally/iql/_type_validators.py
 src/dbally/iql/syntax.py
 src/dbally/iql_generator/__init__.py
 src/dbally/iql_generator/iql_generator.py
-src/dbally/llm_client/__init__.py
-src/dbally/llm_client/base.py
-src/dbally/llm_client/openai_client.py
+src/dbally/iql_generator/iql_prompt_template.py
+src/dbally/llms/__init__.py
+src/dbally/llms/base.py
+src/dbally/llms/litellm.py
+src/dbally/llms/clients/__init__.py
+src/dbally/llms/clients/_exceptions.py
+src/dbally/llms/clients/base.py
+src/dbally/llms/clients/litellm.py
 src/dbally/nl_responder/__init__.py
 src/dbally/nl_responder/nl_responder.py
-src/dbally/nl_responder/token_counters.py
+src/dbally/nl_responder/nl_responder_prompt_template.py
+src/dbally/nl_responder/query_explainer_prompt_template.py
 src/dbally/prompts/__init__.py
-src/dbally/prompts/prompt_builder.py
+src/dbally/prompts/common_validation_utils.py
+src/dbally/prompts/prompt_template.py
 src/dbally/similarity/__init__.py
 src/dbally/similarity/chroma_store.py
-src/dbally/similarity/detector.py
+src/dbally/similarity/elastic_vector_search.py
+src/dbally/similarity/elasticsearch_store.py
 src/dbally/similarity/faiss_store.py
 src/dbally/similarity/fetcher.py
 src/dbally/similarity/index.py
 src/dbally/similarity/sqlalchemy_base.py
 src/dbally/similarity/store.py
 src/dbally/utils/__init__.py
 src/dbally/utils/errors.py
 src/dbally/view_selection/__init__.py
 src/dbally/view_selection/base.py
 src/dbally/view_selection/llm_view_selector.py
 src/dbally/view_selection/random_view_selector.py
+src/dbally/view_selection/view_selector_prompt_template.py
 src/dbally/views/__init__.py
 src/dbally/views/base.py
 src/dbally/views/decorators.py
 src/dbally/views/exposed_functions.py
 src/dbally/views/methods_base.py
 src/dbally/views/pandas_base.py
 src/dbally/views/sqlalchemy_base.py
 src/dbally/views/structured.py
 src/dbally/views/freeform/__init__.py
 src/dbally/views/freeform/text2sql/__init__.py
-src/dbally/views/freeform/text2sql/_autodiscovery.py
-src/dbally/views/freeform/text2sql/_config.py
-src/dbally/views/freeform/text2sql/_errors.py
-src/dbally/views/freeform/text2sql/_view.py
+src/dbally/views/freeform/text2sql/config.py
+src/dbally/views/freeform/text2sql/errors.py
+src/dbally/views/freeform/text2sql/view.py
 src/dbally_cli/__init__.py
 src/dbally_cli/main.py
-src/dbally_cli/similarity.py
+src/dbally_codegen/__init__.py
+src/dbally_codegen/autodiscovery.py
```

### Comparing `dbally-0.1.0/src/dbally.egg-info/requires.txt` & `dbally-0.2.0/src/dbally.egg-info/requires.txt`

 * *Files 22% similar despite different names*

```diff
@@ -15,24 +15,23 @@
 pydantic-core~=2.16.2
 pydantic-settings~=2.0.3
 psycopg2-binary~=2.9.9
 
 [chromadb]
 chromadb>=0.4.24
 
+[elasticsearch]
+elasticsearch==8.13.1
+
 [examples]
 pydantic~=2.6.0
 pydantic_settings~=2.1.0
 psycopg2-binary~=2.9.9
 
 [faiss]
 faiss-cpu>=1.8.0
 
 [langsmith]
-langsmith>=0.0.87
-
-[openai]
-openai>=1.10.0
-tiktoken>=0.6.0
+langsmith~=0.1.57
 
-[transformers]
-transformers>=4.37.1
+[litellm]
+litellm>=1.37.9
```

