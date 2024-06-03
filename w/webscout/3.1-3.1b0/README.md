# Comparing `tmp/webscout-3.1.tar.gz` & `tmp/webscout-3.1b0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "webscout-3.1.tar", last modified: Mon Jun  3 13:28:42 2024, max compression
+gzip compressed data, was "webscout-3.1b0.tar", last modified: Sat Jun  1 14:42:42 2024, max compression
```

## Comparing `webscout-3.1.tar` & `webscout-3.1b0.tar`

### file list

```diff
@@ -1,81 +1,81 @@
-drwxrwxrwx   0        0        0        0 2024-06-03 13:28:42.378647 webscout-3.1/
-drwxrwxrwx   0        0        0        0 2024-06-03 13:28:39.716333 webscout-3.1/DeepWEBS/
--rw-rw-rw-   0        0        0        0 2024-06-01 08:19:23.000000 webscout-3.1/DeepWEBS/__init__.py
-drwxrwxrwx   0        0        0        0 2024-06-03 13:28:39.751354 webscout-3.1/DeepWEBS/documents/
--rw-rw-rw-   0        0        0        0 2024-06-01 08:19:23.000000 webscout-3.1/DeepWEBS/documents/__init__.py
--rw-rw-rw-   0        0        0     4049 2024-06-01 08:19:23.000000 webscout-3.1/DeepWEBS/documents/query_results_extractor.py
--rw-rw-rw-   0        0        0     5272 2024-06-01 08:19:23.000000 webscout-3.1/DeepWEBS/documents/webpage_content_extractor.py
-drwxrwxrwx   0        0        0        0 2024-06-03 13:28:39.901910 webscout-3.1/DeepWEBS/networks/
--rw-rw-rw-   0        0        0        0 2024-06-01 08:19:23.000000 webscout-3.1/DeepWEBS/networks/__init__.py
--rw-rw-rw-   0        0        0     3183 2024-06-01 08:19:23.000000 webscout-3.1/DeepWEBS/networks/filepath_converter.py
--rw-rw-rw-   0        0        0     1966 2024-06-01 08:19:23.000000 webscout-3.1/DeepWEBS/networks/google_searcher.py
--rw-rw-rw-   0        0        0      726 2024-06-01 08:19:23.000000 webscout-3.1/DeepWEBS/networks/network_configs.py
--rw-rw-rw-   0        0        0     3590 2024-06-01 08:19:23.000000 webscout-3.1/DeepWEBS/networks/webpage_fetcher.py
-drwxrwxrwx   0        0        0        0 2024-06-03 13:28:39.978769 webscout-3.1/DeepWEBS/utilsdw/
--rw-rw-rw-   0        0        0        0 2024-06-01 08:19:23.000000 webscout-3.1/DeepWEBS/utilsdw/__init__.py
--rw-rw-rw-   0        0        0     2472 2024-06-01 08:19:23.000000 webscout-3.1/DeepWEBS/utilsdw/enver.py
--rw-rw-rw-   0        0        0     8174 2024-06-01 08:19:23.000000 webscout-3.1/DeepWEBS/utilsdw/logger.py
--rw-rw-rw-   0        0        0     3150 2024-06-01 08:19:23.000000 webscout-3.1/LICENSE.md
--rw-rw-rw-   0        0        0    66275 2024-06-03 13:28:42.343096 webscout-3.1/PKG-INFO
--rw-rw-rw-   0        0        0    63703 2024-06-03 13:25:28.000000 webscout-3.1/README.md
--rw-rw-rw-   0        0        0       42 2024-06-03 13:28:42.378647 webscout-3.1/setup.cfg
--rw-rw-rw-   0        0        0     2816 2024-06-03 13:19:07.000000 webscout-3.1/setup.py
-drwxrwxrwx   0        0        0        0 2024-06-03 13:28:40.678854 webscout-3.1/webscout/
--rw-rw-rw-   0        0        0    18246 2024-06-01 08:19:23.000000 webscout-3.1/webscout/AIauto.py
--rw-rw-rw-   0        0        0     4710 2024-06-01 08:19:23.000000 webscout-3.1/webscout/AIbase.py
--rw-rw-rw-   0        0        0    33272 2024-06-01 08:19:23.000000 webscout-3.1/webscout/AIutel.py
--rw-rw-rw-   0        0        0     7332 2024-06-01 08:19:23.000000 webscout-3.1/webscout/DWEBS.py
--rw-rw-rw-   0        0        0     4184 2024-06-01 08:19:23.000000 webscout-3.1/webscout/LLM.py
-drwxrwxrwx   0        0        0        0 2024-06-03 13:28:41.034110 webscout-3.1/webscout/Local/
--rw-rw-rw-   0        0        0      238 2024-06-03 11:17:16.000000 webscout-3.1/webscout/Local/__init__.py
--rw-rw-rw-   0        0        0       83 2024-06-03 13:18:51.000000 webscout-3.1/webscout/Local/_version.py
--rw-rw-rw-   0        0        0    18994 2024-06-01 08:19:23.000000 webscout-3.1/webscout/Local/formats.py
--rw-rw-rw-   0        0        0    30710 2024-06-01 08:19:23.000000 webscout-3.1/webscout/Local/model.py
--rw-rw-rw-   0        0        0    35744 2024-06-01 15:17:24.000000 webscout-3.1/webscout/Local/rawdog.py
--rw-rw-rw-   0        0        0     4372 2024-06-01 08:19:23.000000 webscout-3.1/webscout/Local/samplers.py
--rw-rw-rw-   0        0        0    27408 2024-06-01 12:08:36.000000 webscout-3.1/webscout/Local/thread.py
--rw-rw-rw-   0        0        0     6197 2024-06-01 08:19:23.000000 webscout-3.1/webscout/Local/utils.py
-drwxrwxrwx   0        0        0        0 2024-06-03 13:28:42.098531 webscout-3.1/webscout/Provider/
--rw-rw-rw-   0        0        0     8416 2024-06-01 08:19:23.000000 webscout-3.1/webscout/Provider/BasedGPT.py
--rw-rw-rw-   0        0        0     8552 2024-06-01 08:19:23.000000 webscout-3.1/webscout/Provider/Berlin4h.py
--rw-rw-rw-   0        0        0    17182 2024-06-01 08:19:23.000000 webscout-3.1/webscout/Provider/Blackboxai.py
--rw-rw-rw-   0        0        0     8570 2024-06-01 08:19:23.000000 webscout-3.1/webscout/Provider/ChatGPTUK.py
--rw-rw-rw-   0        0        0     8711 2024-06-01 08:19:23.000000 webscout-3.1/webscout/Provider/Cohere.py
--rw-rw-rw-   0        0        0     8451 2024-06-01 08:19:24.000000 webscout-3.1/webscout/Provider/Gemini.py
--rw-rw-rw-   0        0        0    21094 2024-06-01 08:19:24.000000 webscout-3.1/webscout/Provider/Groq.py
--rw-rw-rw-   0        0        0    15806 2024-06-01 08:19:24.000000 webscout-3.1/webscout/Provider/Koboldai.py
--rw-rw-rw-   0        0        0    19987 2024-06-01 08:19:24.000000 webscout-3.1/webscout/Provider/Leo.py
--rw-rw-rw-   0        0        0    17525 2024-06-01 08:19:24.000000 webscout-3.1/webscout/Provider/Llama2.py
--rw-rw-rw-   0        0        0    18890 2024-06-01 08:19:24.000000 webscout-3.1/webscout/Provider/OpenGPT.py
--rw-rw-rw-   0        0        0    20617 2024-06-01 08:19:24.000000 webscout-3.1/webscout/Provider/Openai.py
--rw-rw-rw-   0        0        0     8826 2024-06-01 08:19:24.000000 webscout-3.1/webscout/Provider/Perplexity.py
--rw-rw-rw-   0        0        0    19907 2024-06-01 08:19:24.000000 webscout-3.1/webscout/Provider/Phind.py
--rw-rw-rw-   0        0        0     7510 2024-06-01 08:19:24.000000 webscout-3.1/webscout/Provider/Poe.py
--rw-rw-rw-   0        0        0     8917 2024-06-01 08:19:24.000000 webscout-3.1/webscout/Provider/Reka.py
--rw-rw-rw-   0        0        0    11616 2024-06-01 08:19:24.000000 webscout-3.1/webscout/Provider/ThinkAnyAI.py
--rw-rw-rw-   0        0        0     9039 2024-06-01 08:19:24.000000 webscout-3.1/webscout/Provider/Xjai.py
--rw-rw-rw-   0        0        0    19875 2024-06-01 08:19:24.000000 webscout-3.1/webscout/Provider/Yepchat.py
--rw-rw-rw-   0        0        0     7976 2024-06-01 08:19:24.000000 webscout-3.1/webscout/Provider/Youchat.py
--rw-rw-rw-   0        0        0     1457 2024-06-01 08:19:24.000000 webscout-3.1/webscout/Provider/__init__.py
--rw-rw-rw-   0        0        0     1856 2024-06-01 08:19:24.000000 webscout-3.1/webscout/__init__.py
--rw-rw-rw-   0        0        0      126 2024-06-01 08:19:24.000000 webscout-3.1/webscout/__main__.py
--rw-rw-rw-   0        0        0      684 2024-06-01 08:19:24.000000 webscout-3.1/webscout/async_providers.py
--rw-rw-rw-   0        0        0    18743 2024-06-01 08:19:24.000000 webscout-3.1/webscout/cli.py
--rw-rw-rw-   0        0        0      498 2024-06-01 08:19:24.000000 webscout-3.1/webscout/exceptions.py
--rw-rw-rw-   0        0        0    24487 2024-06-01 08:19:24.000000 webscout-3.1/webscout/g4f.py
--rw-rw-rw-   0        0        0      692 2024-06-01 08:19:24.000000 webscout-3.1/webscout/models.py
--rw-rw-rw-   0        0        0     5896 2024-06-01 08:19:24.000000 webscout-3.1/webscout/tempid.py
--rw-rw-rw-   0        0        0    20622 2024-06-01 08:19:24.000000 webscout-3.1/webscout/transcriber.py
--rw-rw-rw-   0        0        0     2603 2024-06-01 08:19:24.000000 webscout-3.1/webscout/utils.py
--rw-rw-rw-   0        0        0       23 2024-06-03 13:19:06.000000 webscout-3.1/webscout/version.py
--rw-rw-rw-   0        0        0      967 2024-06-01 08:19:24.000000 webscout-3.1/webscout/voice.py
--rw-rw-rw-   0        0        0    85324 2024-06-01 08:19:24.000000 webscout-3.1/webscout/webai.py
--rw-rw-rw-   0        0        0    42650 2024-06-01 08:19:24.000000 webscout-3.1/webscout/webscout_search.py
--rw-rw-rw-   0        0        0    14471 2024-06-01 08:19:24.000000 webscout-3.1/webscout/webscout_search_async.py
-drwxrwxrwx   0        0        0        0 2024-06-03 13:28:42.325098 webscout-3.1/webscout.egg-info/
--rw-rw-rw-   0        0        0    66275 2024-06-03 13:28:38.000000 webscout-3.1/webscout.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1852 2024-06-03 13:28:39.000000 webscout-3.1/webscout.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-06-03 13:28:38.000000 webscout-3.1/webscout.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       73 2024-06-03 13:28:38.000000 webscout-3.1/webscout.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      433 2024-06-03 13:28:38.000000 webscout-3.1/webscout.egg-info/requires.txt
--rw-rw-rw-   0        0        0       18 2024-06-03 13:28:38.000000 webscout-3.1/webscout.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-06-01 14:42:42.894606 webscout-3.1b0/
+drwxrwxrwx   0        0        0        0 2024-06-01 14:42:41.789608 webscout-3.1b0/DeepWEBS/
+-rw-rw-rw-   0        0        0        0 2024-06-01 08:19:23.000000 webscout-3.1b0/DeepWEBS/__init__.py
+drwxrwxrwx   0        0        0        0 2024-06-01 14:42:41.815612 webscout-3.1b0/DeepWEBS/documents/
+-rw-rw-rw-   0        0        0        0 2024-06-01 08:19:23.000000 webscout-3.1b0/DeepWEBS/documents/__init__.py
+-rw-rw-rw-   0        0        0     4049 2024-06-01 08:19:23.000000 webscout-3.1b0/DeepWEBS/documents/query_results_extractor.py
+-rw-rw-rw-   0        0        0     5272 2024-06-01 08:19:23.000000 webscout-3.1b0/DeepWEBS/documents/webpage_content_extractor.py
+drwxrwxrwx   0        0        0        0 2024-06-01 14:42:41.855611 webscout-3.1b0/DeepWEBS/networks/
+-rw-rw-rw-   0        0        0        0 2024-06-01 08:19:23.000000 webscout-3.1b0/DeepWEBS/networks/__init__.py
+-rw-rw-rw-   0        0        0     3183 2024-06-01 08:19:23.000000 webscout-3.1b0/DeepWEBS/networks/filepath_converter.py
+-rw-rw-rw-   0        0        0     1966 2024-06-01 08:19:23.000000 webscout-3.1b0/DeepWEBS/networks/google_searcher.py
+-rw-rw-rw-   0        0        0      726 2024-06-01 08:19:23.000000 webscout-3.1b0/DeepWEBS/networks/network_configs.py
+-rw-rw-rw-   0        0        0     3590 2024-06-01 08:19:23.000000 webscout-3.1b0/DeepWEBS/networks/webpage_fetcher.py
+drwxrwxrwx   0        0        0        0 2024-06-01 14:42:41.872602 webscout-3.1b0/DeepWEBS/utilsdw/
+-rw-rw-rw-   0        0        0        0 2024-06-01 08:19:23.000000 webscout-3.1b0/DeepWEBS/utilsdw/__init__.py
+-rw-rw-rw-   0        0        0     2472 2024-06-01 08:19:23.000000 webscout-3.1b0/DeepWEBS/utilsdw/enver.py
+-rw-rw-rw-   0        0        0     8174 2024-06-01 08:19:23.000000 webscout-3.1b0/DeepWEBS/utilsdw/logger.py
+-rw-rw-rw-   0        0        0     3150 2024-06-01 08:19:23.000000 webscout-3.1b0/LICENSE.md
+-rw-rw-rw-   0        0        0    61996 2024-06-01 14:42:42.886078 webscout-3.1b0/PKG-INFO
+-rw-rw-rw-   0        0        0    59422 2024-06-01 08:19:23.000000 webscout-3.1b0/README.md
+-rw-rw-rw-   0        0        0       42 2024-06-01 14:42:42.894606 webscout-3.1b0/setup.cfg
+-rw-rw-rw-   0        0        0     2821 2024-06-01 14:41:51.000000 webscout-3.1b0/setup.py
+drwxrwxrwx   0        0        0        0 2024-06-01 14:42:42.154900 webscout-3.1b0/webscout/
+-rw-rw-rw-   0        0        0    18246 2024-06-01 08:19:23.000000 webscout-3.1b0/webscout/AIauto.py
+-rw-rw-rw-   0        0        0     4710 2024-06-01 08:19:23.000000 webscout-3.1b0/webscout/AIbase.py
+-rw-rw-rw-   0        0        0    33272 2024-06-01 08:19:23.000000 webscout-3.1b0/webscout/AIutel.py
+-rw-rw-rw-   0        0        0     7332 2024-06-01 08:19:23.000000 webscout-3.1b0/webscout/DWEBS.py
+-rw-rw-rw-   0        0        0     4184 2024-06-01 08:19:23.000000 webscout-3.1b0/webscout/LLM.py
+drwxrwxrwx   0        0        0        0 2024-06-01 14:42:42.327493 webscout-3.1b0/webscout/Local/
+-rw-rw-rw-   0        0        0      217 2024-06-01 08:19:23.000000 webscout-3.1b0/webscout/Local/__init__.py
+-rw-rw-rw-   0        0        0       83 2024-06-01 08:19:23.000000 webscout-3.1b0/webscout/Local/_version.py
+-rw-rw-rw-   0        0        0    18994 2024-06-01 08:19:23.000000 webscout-3.1b0/webscout/Local/formats.py
+-rw-rw-rw-   0        0        0    30710 2024-06-01 08:19:23.000000 webscout-3.1b0/webscout/Local/model.py
+-rw-rw-rw-   0        0        0    35595 2024-06-01 12:09:04.000000 webscout-3.1b0/webscout/Local/rawdog.py
+-rw-rw-rw-   0        0        0     4372 2024-06-01 08:19:23.000000 webscout-3.1b0/webscout/Local/samplers.py
+-rw-rw-rw-   0        0        0    27408 2024-06-01 12:08:36.000000 webscout-3.1b0/webscout/Local/thread.py
+-rw-rw-rw-   0        0        0     6197 2024-06-01 08:19:23.000000 webscout-3.1b0/webscout/Local/utils.py
+drwxrwxrwx   0        0        0        0 2024-06-01 14:42:42.839047 webscout-3.1b0/webscout/Provider/
+-rw-rw-rw-   0        0        0     8416 2024-06-01 08:19:23.000000 webscout-3.1b0/webscout/Provider/BasedGPT.py
+-rw-rw-rw-   0        0        0     8552 2024-06-01 08:19:23.000000 webscout-3.1b0/webscout/Provider/Berlin4h.py
+-rw-rw-rw-   0        0        0    17182 2024-06-01 08:19:23.000000 webscout-3.1b0/webscout/Provider/Blackboxai.py
+-rw-rw-rw-   0        0        0     8570 2024-06-01 08:19:23.000000 webscout-3.1b0/webscout/Provider/ChatGPTUK.py
+-rw-rw-rw-   0        0        0     8711 2024-06-01 08:19:23.000000 webscout-3.1b0/webscout/Provider/Cohere.py
+-rw-rw-rw-   0        0        0     8451 2024-06-01 08:19:24.000000 webscout-3.1b0/webscout/Provider/Gemini.py
+-rw-rw-rw-   0        0        0    21094 2024-06-01 08:19:24.000000 webscout-3.1b0/webscout/Provider/Groq.py
+-rw-rw-rw-   0        0        0    15806 2024-06-01 08:19:24.000000 webscout-3.1b0/webscout/Provider/Koboldai.py
+-rw-rw-rw-   0        0        0    19987 2024-06-01 08:19:24.000000 webscout-3.1b0/webscout/Provider/Leo.py
+-rw-rw-rw-   0        0        0    17525 2024-06-01 08:19:24.000000 webscout-3.1b0/webscout/Provider/Llama2.py
+-rw-rw-rw-   0        0        0    18890 2024-06-01 08:19:24.000000 webscout-3.1b0/webscout/Provider/OpenGPT.py
+-rw-rw-rw-   0        0        0    20617 2024-06-01 08:19:24.000000 webscout-3.1b0/webscout/Provider/Openai.py
+-rw-rw-rw-   0        0        0     8826 2024-06-01 08:19:24.000000 webscout-3.1b0/webscout/Provider/Perplexity.py
+-rw-rw-rw-   0        0        0    19907 2024-06-01 08:19:24.000000 webscout-3.1b0/webscout/Provider/Phind.py
+-rw-rw-rw-   0        0        0     7510 2024-06-01 08:19:24.000000 webscout-3.1b0/webscout/Provider/Poe.py
+-rw-rw-rw-   0        0        0     8917 2024-06-01 08:19:24.000000 webscout-3.1b0/webscout/Provider/Reka.py
+-rw-rw-rw-   0        0        0    11616 2024-06-01 08:19:24.000000 webscout-3.1b0/webscout/Provider/ThinkAnyAI.py
+-rw-rw-rw-   0        0        0     9039 2024-06-01 08:19:24.000000 webscout-3.1b0/webscout/Provider/Xjai.py
+-rw-rw-rw-   0        0        0    19875 2024-06-01 08:19:24.000000 webscout-3.1b0/webscout/Provider/Yepchat.py
+-rw-rw-rw-   0        0        0     7976 2024-06-01 08:19:24.000000 webscout-3.1b0/webscout/Provider/Youchat.py
+-rw-rw-rw-   0        0        0     1457 2024-06-01 08:19:24.000000 webscout-3.1b0/webscout/Provider/__init__.py
+-rw-rw-rw-   0        0        0     1856 2024-06-01 08:19:24.000000 webscout-3.1b0/webscout/__init__.py
+-rw-rw-rw-   0        0        0      126 2024-06-01 08:19:24.000000 webscout-3.1b0/webscout/__main__.py
+-rw-rw-rw-   0        0        0      684 2024-06-01 08:19:24.000000 webscout-3.1b0/webscout/async_providers.py
+-rw-rw-rw-   0        0        0    18743 2024-06-01 08:19:24.000000 webscout-3.1b0/webscout/cli.py
+-rw-rw-rw-   0        0        0      498 2024-06-01 08:19:24.000000 webscout-3.1b0/webscout/exceptions.py
+-rw-rw-rw-   0        0        0    24487 2024-06-01 08:19:24.000000 webscout-3.1b0/webscout/g4f.py
+-rw-rw-rw-   0        0        0      692 2024-06-01 08:19:24.000000 webscout-3.1b0/webscout/models.py
+-rw-rw-rw-   0        0        0     5896 2024-06-01 08:19:24.000000 webscout-3.1b0/webscout/tempid.py
+-rw-rw-rw-   0        0        0    20622 2024-06-01 08:19:24.000000 webscout-3.1b0/webscout/transcriber.py
+-rw-rw-rw-   0        0        0     2603 2024-06-01 08:19:24.000000 webscout-3.1b0/webscout/utils.py
+-rw-rw-rw-   0        0        0       23 2024-06-01 08:19:24.000000 webscout-3.1b0/webscout/version.py
+-rw-rw-rw-   0        0        0      967 2024-06-01 08:19:24.000000 webscout-3.1b0/webscout/voice.py
+-rw-rw-rw-   0        0        0    85324 2024-06-01 08:19:24.000000 webscout-3.1b0/webscout/webai.py
+-rw-rw-rw-   0        0        0    42650 2024-06-01 08:19:24.000000 webscout-3.1b0/webscout/webscout_search.py
+-rw-rw-rw-   0        0        0    14471 2024-06-01 08:19:24.000000 webscout-3.1b0/webscout/webscout_search_async.py
+drwxrwxrwx   0        0        0        0 2024-06-01 14:42:42.859052 webscout-3.1b0/webscout.egg-info/
+-rw-rw-rw-   0        0        0    61996 2024-06-01 14:42:40.000000 webscout-3.1b0/webscout.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1852 2024-06-01 14:42:41.000000 webscout-3.1b0/webscout.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-06-01 14:42:40.000000 webscout-3.1b0/webscout.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       73 2024-06-01 14:42:40.000000 webscout-3.1b0/webscout.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      433 2024-06-01 14:42:40.000000 webscout-3.1b0/webscout.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       18 2024-06-01 14:42:40.000000 webscout-3.1b0/webscout.egg-info/top_level.txt
```

### Comparing `webscout-3.1/DeepWEBS/documents/query_results_extractor.py` & `webscout-3.1b0/DeepWEBS/documents/query_results_extractor.py`

 * *Files identical despite different names*

### Comparing `webscout-3.1/DeepWEBS/documents/webpage_content_extractor.py` & `webscout-3.1b0/DeepWEBS/documents/webpage_content_extractor.py`

 * *Files identical despite different names*

### Comparing `webscout-3.1/DeepWEBS/networks/filepath_converter.py` & `webscout-3.1b0/DeepWEBS/networks/filepath_converter.py`

 * *Files identical despite different names*

### Comparing `webscout-3.1/DeepWEBS/networks/google_searcher.py` & `webscout-3.1b0/DeepWEBS/networks/google_searcher.py`

 * *Files identical despite different names*

### Comparing `webscout-3.1/DeepWEBS/networks/network_configs.py` & `webscout-3.1b0/DeepWEBS/networks/network_configs.py`

 * *Files identical despite different names*

### Comparing `webscout-3.1/DeepWEBS/networks/webpage_fetcher.py` & `webscout-3.1b0/DeepWEBS/networks/webpage_fetcher.py`

 * *Files identical despite different names*

### Comparing `webscout-3.1/DeepWEBS/utilsdw/enver.py` & `webscout-3.1b0/DeepWEBS/utilsdw/enver.py`

 * *Files identical despite different names*

### Comparing `webscout-3.1/DeepWEBS/utilsdw/logger.py` & `webscout-3.1b0/DeepWEBS/utilsdw/logger.py`

 * *Files identical despite different names*

### Comparing `webscout-3.1/LICENSE.md` & `webscout-3.1b0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `webscout-3.1/PKG-INFO` & `webscout-3.1b0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: webscout
-Version: 3.1
+Version: 3.1b0
 Summary: Search for anything using Google, DuckDuckGo, phind.com, Contains AI models, can transcribe yt videos, temporary email and phone number generation, has TTS support, webai (terminal gpt and open interpreter) and offline LLMs
 Author: OEvortex
 Author-email: helpingai5@gmail.com
 License: HelpingAI Simplified Universal License
 Project-URL: Documentation, https://github.com/OE-LUCIFER/Webscout/wiki
 Project-URL: Source, https://github.com/OE-LUCIFER/Webscout
 Project-URL: Tracker, https://github.com/OE-LUCIFER/Webscout/issues
@@ -139,15 +139,14 @@
     - [13. `ThinkAny` - AI search engine](#13-thinkany---ai-search-engine)
     - [14. `chatgptuk` - Chat with gemini-pro](#14-chatgptuk---chat-with-gemini-pro)
     - [15. `poe`- chat with poe](#15-poe--chat-with-poe)
     - [16. `BasedGPT` - chat with GPT](#16-basedgpt---chat-with-gpt)
     - [`LLM`](#llm)
     - [`Local-LLM` webscout can now run GGUF models](#local-llm-webscout-can-now-run-gguf-models)
     - [`Function-calling-local-llm`](#function-calling-local-llm)
-    - [`Local-rawdog`](#local-rawdog)
     - [`LLM` with internet](#llm-with-internet)
     - [LLM with deepwebs](#llm-with-deepwebs)
   - [`Webai` - terminal gpt and a open interpeter](#webai---terminal-gpt-and-a-open-interpeter)
 
 ## Install
 ```python
 pip install -U webscout
@@ -1242,15 +1241,14 @@
     # Use the mistral_chat method to get the response
     response = llm.chat(messages)
 
     # Print the response
     print("AI: ", response)
 ```
 ### `Local-LLM` webscout can now run GGUF models
-Local LLM's some functions are taken from easy-llama
 ```python
 from webscout.Local.utils import download_model
 from webscout.Local.model import Model
 from webscout.Local.thread import Thread
 from webscout.Local import formats
 # 1. Download the model
 repo_id = "microsoft/Phi-3-mini-4k-instruct-gguf"  # Replace with the desired Hugging Face repo
@@ -1334,101 +1332,14 @@
 
 # Start interacting with the model
 while True:
     user_input = input("You: ")
     response = thread.send(user_input)
     print("Bot: ", response) 
 ```
-### `Local-rawdog`
-```python
-import webscout.Local as ws
-from webscout.Local.rawdog import RawDog
-from webscout.Local.samplers import DefaultSampling
-from webscout.Local.formats import chatml, AdvancedFormat
-from webscout.Local.utils import download_model
-import datetime
-import sys
-import os
-
-repo_id = "YorkieOH10/granite-8b-code-instruct-Q8_0-GGUF" 
-filename = "granite-8b-code-instruct.Q8_0.gguf"
-model_path = download_model(repo_id, filename, token='')
-
-# Load the model using the downloaded path
-model = ws.Model(model_path, n_gpu_layers=10)
-
-rawdog = RawDog()
-
-# Create an AdvancedFormat and modify the system content
-# Use a lambda to generate the prompt dynamically:
-chat_format = AdvancedFormat(chatml)
-#  **Pre-format the intro_prompt string:**
-system_content = f"""
-You are a command-line coding assistant called Rawdog that generates and auto-executes Python scripts.
-
-A typical interaction goes like this:
-1. The user gives you a natural language PROMPT.
-2. You:
-    i. Determine what needs to be done
-    ii. Write a short Python SCRIPT to do it
-    iii. Communicate back to the user by printing to the console in that SCRIPT
-3. The compiler extracts the script and then runs it using exec(). If there will be an exception raised,
- it will be send back to you starting with "PREVIOUS SCRIPT EXCEPTION:".
-4. In case of exception, regenerate error free script.
-
-If you need to review script outputs before completing the task, you can print the word "CONTINUE" at the end of your SCRIPT.
-This can be useful for summarizing documents or technical readouts, reading instructions before
-deciding what to do, or other tasks that require multi-step reasoning.
-A typical 'CONTINUE' interaction looks like this:
-1. The user gives you a natural language PROMPT.
-2. You:
-    i. Determine what needs to be done
-    ii. Determine that you need to see the output of some subprocess call to complete the task
-    iii. Write a short Python SCRIPT to print that and then print the word "CONTINUE"
-3. The compiler
-    i. Checks and runs your SCRIPT
-    ii. Captures the output and appends it to the conversation as "LAST SCRIPT OUTPUT:"
-    iii. Finds the word "CONTINUE" and sends control back to you
-4. You again:
-    i. Look at the original PROMPT + the "LAST SCRIPT OUTPUT:" to determine what needs to be done
-    ii. Write a short Python SCRIPT to do it
-    iii. Communicate back to the user by printing to the console in that SCRIPT
-5. The compiler...
-
-Please follow these conventions carefully:
-- Decline any tasks that seem dangerous, irreversible, or that you don't understand.
-- Always review the full conversation prior to answering and maintain continuity.
-- If asked for information, just print the information clearly and concisely.
-- If asked to do something, print a concise summary of what you've done as confirmation.
-- If asked a question, respond in a friendly, conversational way. Use programmatically-generated and natural language responses as appropriate.
-- If you need clarification, return a SCRIPT that prints your question. In the next interaction, continue based on the user's response.
-- Assume the user would like something concise. For example rather than printing a massive table, filter or summarize it to what's likely of interest.
-- Actively clean up any temporary processes or files you use.
-- When looking through files, use git as available to skip files, and skip hidden files (.env, .git, etc) by default.
-- You can plot anything with matplotlib.
-- ALWAYS Return your SCRIPT inside of a single pair of ``` delimiters. Only the console output of the first such SCRIPT is visible to the user, so make sure that it's complete and don't bother returning anything else.
-"""
-chat_format.override('system_content', lambda: system_content)
-
-thread = ws.Thread(model, format=chat_format, sampler=DefaultSampling)
-
-while True:
-    prompt = input(">: ")
-    if prompt.lower() == "q":
-        break
-
-    response = thread.send(prompt)
-
-    # Process the response using RawDog
-    script_output = rawdog.main(response)
-
-    if script_output:
-        print(script_output)
-
-```
 ### `LLM` with internet
 ```python
 from __future__ import annotations
 from typing import List, Optional
 
 from webscout.LLM import LLM
 from webscout import WEBS
```

#### html2text {}

```diff
@@ -1,26 +1,26 @@
-Metadata-Version: 2.1 Name: webscout Version: 3.1 Summary: Search for anything
-using Google, DuckDuckGo, phind.com, Contains AI models, can transcribe yt
-videos, temporary email and phone number generation, has TTS support, webai
-(terminal gpt and open interpreter) and offline LLMs Author: OEvortex Author-
-email: helpingai5@gmail.com License: HelpingAI Simplified Universal License
-Project-URL: Documentation, https://github.com/OE-LUCIFER/Webscout/wiki
-Project-URL: Source, https://github.com/OE-LUCIFER/Webscout Project-URL:
-Tracker, https://github.com/OE-LUCIFER/Webscout/issues Project-URL: YouTube,
-https://youtube.com/@OEvortex Classifier: Development Status :: 5 - Production/
-Stable Classifier: Intended Audience :: Developers Classifier: License ::
-Other/Proprietary License Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3 Classifier: Programming
-Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
-Language :: Python :: 3.11 Classifier: Programming Language :: Python :: 3.12
-Classifier: Programming Language :: Python :: Implementation :: CPython
-Classifier: Topic :: Internet :: WWW/HTTP :: Indexing/Search Classifier: Topic
-:: Software Development :: Libraries :: Python Modules Description-Content-
-Type: text/markdown License-File: LICENSE.md Requires-Dist:
+Metadata-Version: 2.1 Name: webscout Version: 3.1b0 Summary: Search for
+anything using Google, DuckDuckGo, phind.com, Contains AI models, can
+transcribe yt videos, temporary email and phone number generation, has TTS
+support, webai (terminal gpt and open interpreter) and offline LLMs Author:
+OEvortex Author-email: helpingai5@gmail.com License: HelpingAI Simplified
+Universal License Project-URL: Documentation, https://github.com/OE-LUCIFER/
+Webscout/wiki Project-URL: Source, https://github.com/OE-LUCIFER/Webscout
+Project-URL: Tracker, https://github.com/OE-LUCIFER/Webscout/issues Project-
+URL: YouTube, https://youtube.com/@OEvortex Classifier: Development Status :: 5
+- Production/Stable Classifier: Intended Audience :: Developers Classifier:
+License :: Other/Proprietary License Classifier: Operating System :: OS
+Independent Classifier: Programming Language :: Python :: 3 Classifier:
+Programming Language :: Python :: 3.8 Classifier: Programming Language ::
+Python :: 3.9 Classifier: Programming Language :: Python :: 3.10 Classifier:
+Programming Language :: Python :: 3.11 Classifier: Programming Language ::
+Python :: 3.12 Classifier: Programming Language :: Python :: Implementation ::
+CPython Classifier: Topic :: Internet :: WWW/HTTP :: Indexing/Search
+Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Description-Content-Type: text/markdown License-File: LICENSE.md Requires-Dist:
 docstring_inheritance Requires-Dist: click Requires-Dist: curl_cffi Requires-
 Dist: lxml Requires-Dist: nest-asyncio Requires-Dist: selenium Requires-Dist:
 tqdm Requires-Dist: webdriver-manager Requires-Dist: halo>=0.0.31 Requires-
 Dist: g4f>=0.2.2.3 Requires-Dist: rich Requires-Dist: python-dotenv Requires-
 Dist: beautifulsoup4 Requires-Dist: markdownify Requires-Dist: pydantic
 Requires-Dist: requests Requires-Dist: sse_starlette Requires-Dist: termcolor
 Requires-Dist: tiktoken Requires-Dist: tldextract Requires-Dist: orjson
@@ -76,71 +76,70 @@
  (#11-cohere---chat-with-cohere) - [12. `Xjai` - chat with free gpt 3.5](#12-
    xjai---chat-with-free-gpt-35) - [13. `ThinkAny` - AI search engine](#13-
  thinkany---ai-search-engine) - [14. `chatgptuk` - Chat with gemini-pro](#14-
  chatgptuk---chat-with-gemini-pro) - [15. `poe`- chat with poe](#15-poe--chat-
  with-poe) - [16. `BasedGPT` - chat with GPT](#16-basedgpt---chat-with-gpt) -
   [`LLM`](#llm) - [`Local-LLM` webscout can now run GGUF models](#local-llm-
  webscout-can-now-run-gguf-models) - [`Function-calling-local-llm`](#function-
- calling-local-llm) - [`Local-rawdog`](#local-rawdog) - [`LLM` with internet]
-  (#llm-with-internet) - [LLM with deepwebs](#llm-with-deepwebs) - [`Webai` -
-     terminal gpt and a open interpeter](#webai---terminal-gpt-and-a-open-
-  interpeter) ## Install ```python pip install -U webscout ``` ## CLI version
-```python3 python -m webscout --help ``` | Command | Description | |-----------
---------------------------------|----------------------------------------------
----------------------------------------------------------| | python -m webscout
-answers -k Text | CLI function to perform an answers search using Webscout. | |
- python -m webscout images -k Text | CLI function to perform an images search
-using Webscout. | | python -m webscout maps -k Text | CLI function to perform a
-maps search using Webscout. | | python -m webscout news -k Text | CLI function
- to perform a news search using Webscout. | | python -m webscout suggestions -
-   k Text | CLI function to perform a suggestions search using Webscout. | |
- python -m webscout text -k Text | CLI function to perform a text search using
- Webscout. | | python -m webscout translate -k Text | CLI function to perform
-   translate using Webscout. | | python -m webscout version | A command-line
-   interface command that prints and returns the version of the program. | |
-  python -m webscout videos -k Text | CLI function to perform a videos search
- using DuckDuckGo API. | [Go To TOP](#TOP) ## Regions expand xa-ar for Arabia
-xa-en for Arabia (en) ar-es for Argentina au-en for Australia at-de for Austria
-   be-fr for Belgium (fr) be-nl for Belgium (nl) br-pt for Brazil bg-bg for
-  Bulgaria ca-en for Canada ca-fr for Canada (fr) ct-ca for Catalan cl-es for
-  Chile cn-zh for China co-es for Colombia hr-hr for Croatia cz-cs for Czech
-Republic dk-da for Denmark ee-et for Estonia fi-fi for Finland fr-fr for France
-de-de for Germany gr-el for Greece hk-tzh for Hong Kong hu-hu for Hungary in-en
-for India id-id for Indonesia id-en for Indonesia (en) ie-en for Ireland il-he
-for Israel it-it for Italy jp-jp for Japan kr-kr for Korea lv-lv for Latvia lt-
-lt for Lithuania xl-es for Latin America my-ms for Malaysia my-en for Malaysia
-  (en) mx-es for Mexico nl-nl for Netherlands nz-en for New Zealand no-no for
- Norway pe-es for Peru ph-en for Philippines ph-tl for Philippines (tl) pl-pl
-  for Poland pt-pt for Portugal ro-ro for Romania ru-ru for Russia sg-en for
- Singapore sk-sk for Slovak Republic sl-sl for Slovenia za-en for South Africa
-     es-es for Spain se-sv for Sweden ch-de for Switzerland (de) ch-fr for
-    Switzerland (fr) ch-it for Switzerland (it) tw-tzh for Taiwan th-th for
-Thailand tr-tr for Turkey ua-uk for Ukraine uk-en for United Kingdom us-en for
-   United States ue-es for United States (es) ve-es for Venezuela vn-vi for
- Vietnam wt-wt for No region ___ [Go To TOP](#TOP) ## Tempmail and Temp number
-### Temp number ```python from rich.console import Console from webscout import
- tempid def main(): console = Console() phone = tempid.TemporaryPhoneNumber()
-try: # Get a temporary phone number for a specific country (or random) number =
-   phone.get_number(country="Finland") console.print(f"Your temporary phone
- number: [bold cyan]{number}[/bold cyan]") # Pause execution briefly (replace
-   with your actual logic) # import time module import time time.sleep(30) #
-  Adjust the waiting time as needed # Retrieve and print messages messages =
-  phone.get_messages(number) if messages: # Access individual messages using
-     indexing: console.print(f"[bold green]{messages[0].frm}:[/] {messages
-    [0].content}") # (Add more lines if you expect multiple messages) else:
-console.print("No messages received.") except Exception as e: console.print(f"
- [bold red]An error occurred: {e}") if __name__ == "__main__": main() ``` ###
-    Tempmail ```python import asyncio from rich.console import Console from
-rich.table import Table from rich.text import Text from webscout import tempid
-  async def main() -> None: console = Console() client = tempid.Client() try:
-   domains = await client.get_domains() if not domains: console.print("[bold
-   red]No domains available. Please try again later.") return email = await
-  client.create_email(domain=domains[0].name) console.print(f"Your temporary
-    email: [bold cyan]{email.email}[/bold cyan]") console.print(f"Token for
-    accessing the email: [bold cyan]{email.token}[/bold cyan]") while True:
+  calling-local-llm) - [`LLM` with internet](#llm-with-internet) - [LLM with
+deepwebs](#llm-with-deepwebs) - [`Webai` - terminal gpt and a open interpeter]
+(#webai---terminal-gpt-and-a-open-interpeter) ## Install ```python pip install
+   -U webscout ``` ## CLI version ```python3 python -m webscout --help ``` |
+Command | Description | |-------------------------------------------|----------
+-------------------------------------------------------------------------------
+--------------| | python -m webscout answers -k Text | CLI function to perform
+ an answers search using Webscout. | | python -m webscout images -k Text | CLI
+  function to perform an images search using Webscout. | | python -m webscout
+maps -k Text | CLI function to perform a maps search using Webscout. | | python
+    -m webscout news -k Text | CLI function to perform a news search using
+Webscout. | | python -m webscout suggestions -k Text | CLI function to perform
+a suggestions search using Webscout. | | python -m webscout text -k Text | CLI
+   function to perform a text search using Webscout. | | python -m webscout
+   translate -k Text | CLI function to perform translate using Webscout. | |
+ python -m webscout version | A command-line interface command that prints and
+returns the version of the program. | | python -m webscout videos -k Text | CLI
+ function to perform a videos search using DuckDuckGo API. | [Go To TOP](#TOP)
+ ## Regions expand xa-ar for Arabia xa-en for Arabia (en) ar-es for Argentina
+au-en for Australia at-de for Austria be-fr for Belgium (fr) be-nl for Belgium
+(nl) br-pt for Brazil bg-bg for Bulgaria ca-en for Canada ca-fr for Canada (fr)
+ct-ca for Catalan cl-es for Chile cn-zh for China co-es for Colombia hr-hr for
+Croatia cz-cs for Czech Republic dk-da for Denmark ee-et for Estonia fi-fi for
+  Finland fr-fr for France de-de for Germany gr-el for Greece hk-tzh for Hong
+Kong hu-hu for Hungary in-en for India id-id for Indonesia id-en for Indonesia
+ (en) ie-en for Ireland il-he for Israel it-it for Italy jp-jp for Japan kr-kr
+ for Korea lv-lv for Latvia lt-lt for Lithuania xl-es for Latin America my-ms
+for Malaysia my-en for Malaysia (en) mx-es for Mexico nl-nl for Netherlands nz-
+en for New Zealand no-no for Norway pe-es for Peru ph-en for Philippines ph-tl
+for Philippines (tl) pl-pl for Poland pt-pt for Portugal ro-ro for Romania ru-
+ru for Russia sg-en for Singapore sk-sk for Slovak Republic sl-sl for Slovenia
+za-en for South Africa es-es for Spain se-sv for Sweden ch-de for Switzerland
+ (de) ch-fr for Switzerland (fr) ch-it for Switzerland (it) tw-tzh for Taiwan
+th-th for Thailand tr-tr for Turkey ua-uk for Ukraine uk-en for United Kingdom
+us-en for United States ue-es for United States (es) ve-es for Venezuela vn-vi
+  for Vietnam wt-wt for No region ___ [Go To TOP](#TOP) ## Tempmail and Temp
+number ### Temp number ```python from rich.console import Console from webscout
+             import tempid def main(): console = Console() phone =
+    tempid.TemporaryPhoneNumber() try: # Get a temporary phone number for a
+   specific country (or random) number = phone.get_number(country="Finland")
+console.print(f"Your temporary phone number: [bold cyan]{number}[/bold cyan]")
+# Pause execution briefly (replace with your actual logic) # import time module
+ import time time.sleep(30) # Adjust the waiting time as needed # Retrieve and
+  print messages messages = phone.get_messages(number) if messages: # Access
+   individual messages using indexing: console.print(f"[bold green]{messages
+ [0].frm}:[/] {messages[0].content}") # (Add more lines if you expect multiple
+ messages) else: console.print("No messages received.") except Exception as e:
+ console.print(f"[bold red]An error occurred: {e}") if __name__ == "__main__":
+   main() ``` ### Tempmail ```python import asyncio from rich.console import
+ Console from rich.table import Table from rich.text import Text from webscout
+     import tempid async def main() -> None: console = Console() client =
+   tempid.Client() try: domains = await client.get_domains() if not domains:
+console.print("[bold red]No domains available. Please try again later.") return
+email = await client.create_email(domain=domains[0].name) console.print(f"Your
+ temporary email: [bold cyan]{email.email}[/bold cyan]") console.print(f"Token
+  for accessing the email: [bold cyan]{email.token}[/bold cyan]") while True:
   messages = await client.get_messages(email.email) if messages is not None:
 break if messages: table = Table(show_header=True, header_style="bold magenta")
     table.add_column("From", style="bold cyan") table.add_column("Subject",
  style="bold yellow") table.add_column("Body", style="bold green") for message
  in messages: body_preview = Text(message.body_text if message.body_text else
  "No body") table.add_row(message.email_from or "Unknown", message.subject or
    "No Subject", body_preview) console.print(table) else: console.print("No
@@ -423,32 +422,31 @@
  message from the file with open('system.txt', 'r') as file: system_message =
  file.read() # Initialize the LLM class with the model name and system message
  llm = LLM(model="microsoft/WizardLM-2-8x22B", system_message=system_message)
   while True: # Get the user input user_input = input("User: ") # Define the
  messages to be sent messages = [ {"role": "user", "content": user_input} ] #
 Use the mistral_chat method to get the response response = llm.chat(messages) #
 Print the response print("AI: ", response) ``` ### `Local-LLM` webscout can now
-run GGUF models Local LLM's some functions are taken from easy-llama ```python
-   from webscout.Local.utils import download_model from webscout.Local.model
-   import Model from webscout.Local.thread import Thread from webscout.Local
-  import formats # 1. Download the model repo_id = "microsoft/Phi-3-mini-4k-
-instruct-gguf" # Replace with the desired Hugging Face repo filename = "Phi-3-
-  mini-4k-instruct-q4.gguf" # Replace with the correct filename model_path =
-download_model(repo_id, filename) # 2. Load the model model = Model(model_path,
- n_gpu_layers=4) # 3. Create a Thread for conversation thread = Thread(model,
- formats.phi3) # 4. Start interacting with the model thread.interact() ``` ###
-   `Function-calling-local-llm` ```python from webscout.Local import Model,
-Thread, formats from webscout import DeepWEBS from webscout.Local.utils import
-          download_model from webscout.Local.model import Model from
-  webscout.Local.thread import Thread from webscout.Local import formats from
-   webscout.Local.samplers import SamplerSettings def deepwebs_search(query,
-max_results=5): """Performs a web search using DeepWEBS and returns results as
- JSON.""" deepwebs = DeepWEBS() search_config = DeepWEBS.DeepSearch( queries=
-  [query], max_results=max_results, extract_webpage=False, safe=False, types=
-      ["web"], overwrite_query_html=True, overwrite_webpage_html=True, )
+run GGUF models ```python from webscout.Local.utils import download_model from
+webscout.Local.model import Model from webscout.Local.thread import Thread from
+webscout.Local import formats # 1. Download the model repo_id = "microsoft/Phi-
+3-mini-4k-instruct-gguf" # Replace with the desired Hugging Face repo filename
+    = "Phi-3-mini-4k-instruct-q4.gguf" # Replace with the correct filename
+  model_path = download_model(repo_id, filename) # 2. Load the model model =
+Model(model_path, n_gpu_layers=4) # 3. Create a Thread for conversation thread
+      = Thread(model, formats.phi3) # 4. Start interacting with the model
+     thread.interact() ``` ### `Function-calling-local-llm` ```python from
+webscout.Local import Model, Thread, formats from webscout import DeepWEBS from
+  webscout.Local.utils import download_model from webscout.Local.model import
+   Model from webscout.Local.thread import Thread from webscout.Local import
+formats from webscout.Local.samplers import SamplerSettings def deepwebs_search
+  (query, max_results=5): """Performs a web search using DeepWEBS and returns
+ results as JSON.""" deepwebs = DeepWEBS() search_config = DeepWEBS.DeepSearch
+( queries=[query], max_results=max_results, extract_webpage=False, safe=False,
+   types=["web"], overwrite_query_html=True, overwrite_webpage_html=True, )
       search_results = deepwebs.queries_to_search_results(search_config)
   formatted_results = [] for result in search_results[0]: # Assuming only one
     query formatted_results.append(f"Title: {result['title']}\nURL: {result
  ['url']}\n") return "\n".join(formatted_results) # Load your model repo_id =
    "OEvortex/HelpingAI-9B" filename = "helpingai-9b.Q4_0.gguf" model_path =
  download_model(repo_id, filename, token='') # 2. Load the model model = Model
   (model_path, n_gpu_layers=10) # Create a Thread system_prompt = "You are a
@@ -462,67 +460,15 @@
 "function", "function": { "name": "deepwebs_search", "description": "Performs a
   web search using DeepWEBS and returns the title and URLs of the results.",
  "execute": deepwebs_search, "parameters": { "type": "object", "properties":
 { "query": { "type": "string", "description": "The query to search on the web",
 }, "max_results": { "type": "integer", "description": "Maximum number of search
      results (default: 5)", }, }, "required": ["query"], }, }, }) # Start
  interacting with the model while True: user_input = input("You: ") response =
-    thread.send(user_input) print("Bot: ", response) ``` ### `Local-rawdog`
-```python import webscout.Local as ws from webscout.Local.rawdog import RawDog
-from webscout.Local.samplers import DefaultSampling from webscout.Local.formats
- import chatml, AdvancedFormat from webscout.Local.utils import download_model
-  import datetime import sys import os repo_id = "YorkieOH10/granite-8b-code-
-instruct-Q8_0-GGUF" filename = "granite-8b-code-instruct.Q8_0.gguf" model_path
-   = download_model(repo_id, filename, token='') # Load the model using the
-downloaded path model = ws.Model(model_path, n_gpu_layers=10) rawdog = RawDog()
-  # Create an AdvancedFormat and modify the system content # Use a lambda to
-generate the prompt dynamically: chat_format = AdvancedFormat(chatml) # **Pre-
-format the intro_prompt string:** system_content = f""" You are a command-line
-coding assistant called Rawdog that generates and auto-executes Python scripts.
-A typical interaction goes like this: 1. The user gives you a natural language
-  PROMPT. 2. You: i. Determine what needs to be done ii. Write a short Python
-SCRIPT to do it iii. Communicate back to the user by printing to the console in
-that SCRIPT 3. The compiler extracts the script and then runs it using exec().
-If there will be an exception raised, it will be send back to you starting with
- "PREVIOUS SCRIPT EXCEPTION:". 4. In case of exception, regenerate error free
- script. If you need to review script outputs before completing the task, you
-can print the word "CONTINUE" at the end of your SCRIPT. This can be useful for
-   summarizing documents or technical readouts, reading instructions before
-   deciding what to do, or other tasks that require multi-step reasoning. A
-typical 'CONTINUE' interaction looks like this: 1. The user gives you a natural
-language PROMPT. 2. You: i. Determine what needs to be done ii. Determine that
- you need to see the output of some subprocess call to complete the task iii.
-Write a short Python SCRIPT to print that and then print the word "CONTINUE" 3.
-The compiler i. Checks and runs your SCRIPT ii. Captures the output and appends
-it to the conversation as "LAST SCRIPT OUTPUT:" iii. Finds the word "CONTINUE"
- and sends control back to you 4. You again: i. Look at the original PROMPT +
-the "LAST SCRIPT OUTPUT:" to determine what needs to be done ii. Write a short
-  Python SCRIPT to do it iii. Communicate back to the user by printing to the
-   console in that SCRIPT 5. The compiler... Please follow these conventions
- carefully: - Decline any tasks that seem dangerous, irreversible, or that you
-don't understand. - Always review the full conversation prior to answering and
-  maintain continuity. - If asked for information, just print the information
- clearly and concisely. - If asked to do something, print a concise summary of
-what you've done as confirmation. - If asked a question, respond in a friendly,
-    conversational way. Use programmatically-generated and natural language
-  responses as appropriate. - If you need clarification, return a SCRIPT that
-  prints your question. In the next interaction, continue based on the user's
- response. - Assume the user would like something concise. For example rather
-   than printing a massive table, filter or summarize it to what's likely of
-interest. - Actively clean up any temporary processes or files you use. - When
-  looking through files, use git as available to skip files, and skip hidden
-files (.env, .git, etc) by default. - You can plot anything with matplotlib. -
- ALWAYS Return your SCRIPT inside of a single pair of ``` delimiters. Only the
- console output of the first such SCRIPT is visible to the user, so make sure
-       that it's complete and don't bother returning anything else. """
-    chat_format.override('system_content', lambda: system_content) thread =
-   ws.Thread(model, format=chat_format, sampler=DefaultSampling) while True:
- prompt = input(">: ") if prompt.lower() == "q": break response = thread.send
-   (prompt) # Process the response using RawDog script_output = rawdog.main
- (response) if script_output: print(script_output) ``` ### `LLM` with internet
+ thread.send(user_input) print("Bot: ", response) ``` ### `LLM` with internet
 ```python from __future__ import annotations from typing import List, Optional
     from webscout.LLM import LLM from webscout import WEBS import warnings
 system_message: str = ( "As an AI assistant, I have been designed with advanced
  capabilities, including real-time access to online resources. This enables me
     to enrich our conversations and provide you with informed and accurate
 responses, drawing from a vast array of information. With each interaction, my
  goal is to create a seamless and meaningful connection, offering insights and
```

### Comparing `webscout-3.1/README.md` & `webscout-3.1b0/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -74,15 +74,14 @@
     - [13. `ThinkAny` - AI search engine](#13-thinkany---ai-search-engine)
     - [14. `chatgptuk` - Chat with gemini-pro](#14-chatgptuk---chat-with-gemini-pro)
     - [15. `poe`- chat with poe](#15-poe--chat-with-poe)
     - [16. `BasedGPT` - chat with GPT](#16-basedgpt---chat-with-gpt)
     - [`LLM`](#llm)
     - [`Local-LLM` webscout can now run GGUF models](#local-llm-webscout-can-now-run-gguf-models)
     - [`Function-calling-local-llm`](#function-calling-local-llm)
-    - [`Local-rawdog`](#local-rawdog)
     - [`LLM` with internet](#llm-with-internet)
     - [LLM with deepwebs](#llm-with-deepwebs)
   - [`Webai` - terminal gpt and a open interpeter](#webai---terminal-gpt-and-a-open-interpeter)
 
 ## Install
 ```python
 pip install -U webscout
@@ -1177,15 +1176,14 @@
     # Use the mistral_chat method to get the response
     response = llm.chat(messages)
 
     # Print the response
     print("AI: ", response)
 ```
 ### `Local-LLM` webscout can now run GGUF models
-Local LLM's some functions are taken from easy-llama
 ```python
 from webscout.Local.utils import download_model
 from webscout.Local.model import Model
 from webscout.Local.thread import Thread
 from webscout.Local import formats
 # 1. Download the model
 repo_id = "microsoft/Phi-3-mini-4k-instruct-gguf"  # Replace with the desired Hugging Face repo
@@ -1269,101 +1267,14 @@
 
 # Start interacting with the model
 while True:
     user_input = input("You: ")
     response = thread.send(user_input)
     print("Bot: ", response) 
 ```
-### `Local-rawdog`
-```python
-import webscout.Local as ws
-from webscout.Local.rawdog import RawDog
-from webscout.Local.samplers import DefaultSampling
-from webscout.Local.formats import chatml, AdvancedFormat
-from webscout.Local.utils import download_model
-import datetime
-import sys
-import os
-
-repo_id = "YorkieOH10/granite-8b-code-instruct-Q8_0-GGUF" 
-filename = "granite-8b-code-instruct.Q8_0.gguf"
-model_path = download_model(repo_id, filename, token='')
-
-# Load the model using the downloaded path
-model = ws.Model(model_path, n_gpu_layers=10)
-
-rawdog = RawDog()
-
-# Create an AdvancedFormat and modify the system content
-# Use a lambda to generate the prompt dynamically:
-chat_format = AdvancedFormat(chatml)
-#  **Pre-format the intro_prompt string:**
-system_content = f"""
-You are a command-line coding assistant called Rawdog that generates and auto-executes Python scripts.
-
-A typical interaction goes like this:
-1. The user gives you a natural language PROMPT.
-2. You:
-    i. Determine what needs to be done
-    ii. Write a short Python SCRIPT to do it
-    iii. Communicate back to the user by printing to the console in that SCRIPT
-3. The compiler extracts the script and then runs it using exec(). If there will be an exception raised,
- it will be send back to you starting with "PREVIOUS SCRIPT EXCEPTION:".
-4. In case of exception, regenerate error free script.
-
-If you need to review script outputs before completing the task, you can print the word "CONTINUE" at the end of your SCRIPT.
-This can be useful for summarizing documents or technical readouts, reading instructions before
-deciding what to do, or other tasks that require multi-step reasoning.
-A typical 'CONTINUE' interaction looks like this:
-1. The user gives you a natural language PROMPT.
-2. You:
-    i. Determine what needs to be done
-    ii. Determine that you need to see the output of some subprocess call to complete the task
-    iii. Write a short Python SCRIPT to print that and then print the word "CONTINUE"
-3. The compiler
-    i. Checks and runs your SCRIPT
-    ii. Captures the output and appends it to the conversation as "LAST SCRIPT OUTPUT:"
-    iii. Finds the word "CONTINUE" and sends control back to you
-4. You again:
-    i. Look at the original PROMPT + the "LAST SCRIPT OUTPUT:" to determine what needs to be done
-    ii. Write a short Python SCRIPT to do it
-    iii. Communicate back to the user by printing to the console in that SCRIPT
-5. The compiler...
-
-Please follow these conventions carefully:
-- Decline any tasks that seem dangerous, irreversible, or that you don't understand.
-- Always review the full conversation prior to answering and maintain continuity.
-- If asked for information, just print the information clearly and concisely.
-- If asked to do something, print a concise summary of what you've done as confirmation.
-- If asked a question, respond in a friendly, conversational way. Use programmatically-generated and natural language responses as appropriate.
-- If you need clarification, return a SCRIPT that prints your question. In the next interaction, continue based on the user's response.
-- Assume the user would like something concise. For example rather than printing a massive table, filter or summarize it to what's likely of interest.
-- Actively clean up any temporary processes or files you use.
-- When looking through files, use git as available to skip files, and skip hidden files (.env, .git, etc) by default.
-- You can plot anything with matplotlib.
-- ALWAYS Return your SCRIPT inside of a single pair of ``` delimiters. Only the console output of the first such SCRIPT is visible to the user, so make sure that it's complete and don't bother returning anything else.
-"""
-chat_format.override('system_content', lambda: system_content)
-
-thread = ws.Thread(model, format=chat_format, sampler=DefaultSampling)
-
-while True:
-    prompt = input(">: ")
-    if prompt.lower() == "q":
-        break
-
-    response = thread.send(prompt)
-
-    # Process the response using RawDog
-    script_output = rawdog.main(response)
-
-    if script_output:
-        print(script_output)
-
-```
 ### `LLM` with internet
 ```python
 from __future__ import annotations
 from typing import List, Optional
 
 from webscout.LLM import LLM
 from webscout import WEBS
```

#### html2text {}

```diff
@@ -42,71 +42,70 @@
  (#11-cohere---chat-with-cohere) - [12. `Xjai` - chat with free gpt 3.5](#12-
    xjai---chat-with-free-gpt-35) - [13. `ThinkAny` - AI search engine](#13-
  thinkany---ai-search-engine) - [14. `chatgptuk` - Chat with gemini-pro](#14-
  chatgptuk---chat-with-gemini-pro) - [15. `poe`- chat with poe](#15-poe--chat-
  with-poe) - [16. `BasedGPT` - chat with GPT](#16-basedgpt---chat-with-gpt) -
   [`LLM`](#llm) - [`Local-LLM` webscout can now run GGUF models](#local-llm-
  webscout-can-now-run-gguf-models) - [`Function-calling-local-llm`](#function-
- calling-local-llm) - [`Local-rawdog`](#local-rawdog) - [`LLM` with internet]
-  (#llm-with-internet) - [LLM with deepwebs](#llm-with-deepwebs) - [`Webai` -
-     terminal gpt and a open interpeter](#webai---terminal-gpt-and-a-open-
-  interpeter) ## Install ```python pip install -U webscout ``` ## CLI version
-```python3 python -m webscout --help ``` | Command | Description | |-----------
---------------------------------|----------------------------------------------
----------------------------------------------------------| | python -m webscout
-answers -k Text | CLI function to perform an answers search using Webscout. | |
- python -m webscout images -k Text | CLI function to perform an images search
-using Webscout. | | python -m webscout maps -k Text | CLI function to perform a
-maps search using Webscout. | | python -m webscout news -k Text | CLI function
- to perform a news search using Webscout. | | python -m webscout suggestions -
-   k Text | CLI function to perform a suggestions search using Webscout. | |
- python -m webscout text -k Text | CLI function to perform a text search using
- Webscout. | | python -m webscout translate -k Text | CLI function to perform
-   translate using Webscout. | | python -m webscout version | A command-line
-   interface command that prints and returns the version of the program. | |
-  python -m webscout videos -k Text | CLI function to perform a videos search
- using DuckDuckGo API. | [Go To TOP](#TOP) ## Regions expand xa-ar for Arabia
-xa-en for Arabia (en) ar-es for Argentina au-en for Australia at-de for Austria
-   be-fr for Belgium (fr) be-nl for Belgium (nl) br-pt for Brazil bg-bg for
-  Bulgaria ca-en for Canada ca-fr for Canada (fr) ct-ca for Catalan cl-es for
-  Chile cn-zh for China co-es for Colombia hr-hr for Croatia cz-cs for Czech
-Republic dk-da for Denmark ee-et for Estonia fi-fi for Finland fr-fr for France
-de-de for Germany gr-el for Greece hk-tzh for Hong Kong hu-hu for Hungary in-en
-for India id-id for Indonesia id-en for Indonesia (en) ie-en for Ireland il-he
-for Israel it-it for Italy jp-jp for Japan kr-kr for Korea lv-lv for Latvia lt-
-lt for Lithuania xl-es for Latin America my-ms for Malaysia my-en for Malaysia
-  (en) mx-es for Mexico nl-nl for Netherlands nz-en for New Zealand no-no for
- Norway pe-es for Peru ph-en for Philippines ph-tl for Philippines (tl) pl-pl
-  for Poland pt-pt for Portugal ro-ro for Romania ru-ru for Russia sg-en for
- Singapore sk-sk for Slovak Republic sl-sl for Slovenia za-en for South Africa
-     es-es for Spain se-sv for Sweden ch-de for Switzerland (de) ch-fr for
-    Switzerland (fr) ch-it for Switzerland (it) tw-tzh for Taiwan th-th for
-Thailand tr-tr for Turkey ua-uk for Ukraine uk-en for United Kingdom us-en for
-   United States ue-es for United States (es) ve-es for Venezuela vn-vi for
- Vietnam wt-wt for No region ___ [Go To TOP](#TOP) ## Tempmail and Temp number
-### Temp number ```python from rich.console import Console from webscout import
- tempid def main(): console = Console() phone = tempid.TemporaryPhoneNumber()
-try: # Get a temporary phone number for a specific country (or random) number =
-   phone.get_number(country="Finland") console.print(f"Your temporary phone
- number: [bold cyan]{number}[/bold cyan]") # Pause execution briefly (replace
-   with your actual logic) # import time module import time time.sleep(30) #
-  Adjust the waiting time as needed # Retrieve and print messages messages =
-  phone.get_messages(number) if messages: # Access individual messages using
-     indexing: console.print(f"[bold green]{messages[0].frm}:[/] {messages
-    [0].content}") # (Add more lines if you expect multiple messages) else:
-console.print("No messages received.") except Exception as e: console.print(f"
- [bold red]An error occurred: {e}") if __name__ == "__main__": main() ``` ###
-    Tempmail ```python import asyncio from rich.console import Console from
-rich.table import Table from rich.text import Text from webscout import tempid
-  async def main() -> None: console = Console() client = tempid.Client() try:
-   domains = await client.get_domains() if not domains: console.print("[bold
-   red]No domains available. Please try again later.") return email = await
-  client.create_email(domain=domains[0].name) console.print(f"Your temporary
-    email: [bold cyan]{email.email}[/bold cyan]") console.print(f"Token for
-    accessing the email: [bold cyan]{email.token}[/bold cyan]") while True:
+  calling-local-llm) - [`LLM` with internet](#llm-with-internet) - [LLM with
+deepwebs](#llm-with-deepwebs) - [`Webai` - terminal gpt and a open interpeter]
+(#webai---terminal-gpt-and-a-open-interpeter) ## Install ```python pip install
+   -U webscout ``` ## CLI version ```python3 python -m webscout --help ``` |
+Command | Description | |-------------------------------------------|----------
+-------------------------------------------------------------------------------
+--------------| | python -m webscout answers -k Text | CLI function to perform
+ an answers search using Webscout. | | python -m webscout images -k Text | CLI
+  function to perform an images search using Webscout. | | python -m webscout
+maps -k Text | CLI function to perform a maps search using Webscout. | | python
+    -m webscout news -k Text | CLI function to perform a news search using
+Webscout. | | python -m webscout suggestions -k Text | CLI function to perform
+a suggestions search using Webscout. | | python -m webscout text -k Text | CLI
+   function to perform a text search using Webscout. | | python -m webscout
+   translate -k Text | CLI function to perform translate using Webscout. | |
+ python -m webscout version | A command-line interface command that prints and
+returns the version of the program. | | python -m webscout videos -k Text | CLI
+ function to perform a videos search using DuckDuckGo API. | [Go To TOP](#TOP)
+ ## Regions expand xa-ar for Arabia xa-en for Arabia (en) ar-es for Argentina
+au-en for Australia at-de for Austria be-fr for Belgium (fr) be-nl for Belgium
+(nl) br-pt for Brazil bg-bg for Bulgaria ca-en for Canada ca-fr for Canada (fr)
+ct-ca for Catalan cl-es for Chile cn-zh for China co-es for Colombia hr-hr for
+Croatia cz-cs for Czech Republic dk-da for Denmark ee-et for Estonia fi-fi for
+  Finland fr-fr for France de-de for Germany gr-el for Greece hk-tzh for Hong
+Kong hu-hu for Hungary in-en for India id-id for Indonesia id-en for Indonesia
+ (en) ie-en for Ireland il-he for Israel it-it for Italy jp-jp for Japan kr-kr
+ for Korea lv-lv for Latvia lt-lt for Lithuania xl-es for Latin America my-ms
+for Malaysia my-en for Malaysia (en) mx-es for Mexico nl-nl for Netherlands nz-
+en for New Zealand no-no for Norway pe-es for Peru ph-en for Philippines ph-tl
+for Philippines (tl) pl-pl for Poland pt-pt for Portugal ro-ro for Romania ru-
+ru for Russia sg-en for Singapore sk-sk for Slovak Republic sl-sl for Slovenia
+za-en for South Africa es-es for Spain se-sv for Sweden ch-de for Switzerland
+ (de) ch-fr for Switzerland (fr) ch-it for Switzerland (it) tw-tzh for Taiwan
+th-th for Thailand tr-tr for Turkey ua-uk for Ukraine uk-en for United Kingdom
+us-en for United States ue-es for United States (es) ve-es for Venezuela vn-vi
+  for Vietnam wt-wt for No region ___ [Go To TOP](#TOP) ## Tempmail and Temp
+number ### Temp number ```python from rich.console import Console from webscout
+             import tempid def main(): console = Console() phone =
+    tempid.TemporaryPhoneNumber() try: # Get a temporary phone number for a
+   specific country (or random) number = phone.get_number(country="Finland")
+console.print(f"Your temporary phone number: [bold cyan]{number}[/bold cyan]")
+# Pause execution briefly (replace with your actual logic) # import time module
+ import time time.sleep(30) # Adjust the waiting time as needed # Retrieve and
+  print messages messages = phone.get_messages(number) if messages: # Access
+   individual messages using indexing: console.print(f"[bold green]{messages
+ [0].frm}:[/] {messages[0].content}") # (Add more lines if you expect multiple
+ messages) else: console.print("No messages received.") except Exception as e:
+ console.print(f"[bold red]An error occurred: {e}") if __name__ == "__main__":
+   main() ``` ### Tempmail ```python import asyncio from rich.console import
+ Console from rich.table import Table from rich.text import Text from webscout
+     import tempid async def main() -> None: console = Console() client =
+   tempid.Client() try: domains = await client.get_domains() if not domains:
+console.print("[bold red]No domains available. Please try again later.") return
+email = await client.create_email(domain=domains[0].name) console.print(f"Your
+ temporary email: [bold cyan]{email.email}[/bold cyan]") console.print(f"Token
+  for accessing the email: [bold cyan]{email.token}[/bold cyan]") while True:
   messages = await client.get_messages(email.email) if messages is not None:
 break if messages: table = Table(show_header=True, header_style="bold magenta")
     table.add_column("From", style="bold cyan") table.add_column("Subject",
  style="bold yellow") table.add_column("Body", style="bold green") for message
  in messages: body_preview = Text(message.body_text if message.body_text else
  "No body") table.add_row(message.email_from or "Unknown", message.subject or
    "No Subject", body_preview) console.print(table) else: console.print("No
@@ -389,32 +388,31 @@
  message from the file with open('system.txt', 'r') as file: system_message =
  file.read() # Initialize the LLM class with the model name and system message
  llm = LLM(model="microsoft/WizardLM-2-8x22B", system_message=system_message)
   while True: # Get the user input user_input = input("User: ") # Define the
  messages to be sent messages = [ {"role": "user", "content": user_input} ] #
 Use the mistral_chat method to get the response response = llm.chat(messages) #
 Print the response print("AI: ", response) ``` ### `Local-LLM` webscout can now
-run GGUF models Local LLM's some functions are taken from easy-llama ```python
-   from webscout.Local.utils import download_model from webscout.Local.model
-   import Model from webscout.Local.thread import Thread from webscout.Local
-  import formats # 1. Download the model repo_id = "microsoft/Phi-3-mini-4k-
-instruct-gguf" # Replace with the desired Hugging Face repo filename = "Phi-3-
-  mini-4k-instruct-q4.gguf" # Replace with the correct filename model_path =
-download_model(repo_id, filename) # 2. Load the model model = Model(model_path,
- n_gpu_layers=4) # 3. Create a Thread for conversation thread = Thread(model,
- formats.phi3) # 4. Start interacting with the model thread.interact() ``` ###
-   `Function-calling-local-llm` ```python from webscout.Local import Model,
-Thread, formats from webscout import DeepWEBS from webscout.Local.utils import
-          download_model from webscout.Local.model import Model from
-  webscout.Local.thread import Thread from webscout.Local import formats from
-   webscout.Local.samplers import SamplerSettings def deepwebs_search(query,
-max_results=5): """Performs a web search using DeepWEBS and returns results as
- JSON.""" deepwebs = DeepWEBS() search_config = DeepWEBS.DeepSearch( queries=
-  [query], max_results=max_results, extract_webpage=False, safe=False, types=
-      ["web"], overwrite_query_html=True, overwrite_webpage_html=True, )
+run GGUF models ```python from webscout.Local.utils import download_model from
+webscout.Local.model import Model from webscout.Local.thread import Thread from
+webscout.Local import formats # 1. Download the model repo_id = "microsoft/Phi-
+3-mini-4k-instruct-gguf" # Replace with the desired Hugging Face repo filename
+    = "Phi-3-mini-4k-instruct-q4.gguf" # Replace with the correct filename
+  model_path = download_model(repo_id, filename) # 2. Load the model model =
+Model(model_path, n_gpu_layers=4) # 3. Create a Thread for conversation thread
+      = Thread(model, formats.phi3) # 4. Start interacting with the model
+     thread.interact() ``` ### `Function-calling-local-llm` ```python from
+webscout.Local import Model, Thread, formats from webscout import DeepWEBS from
+  webscout.Local.utils import download_model from webscout.Local.model import
+   Model from webscout.Local.thread import Thread from webscout.Local import
+formats from webscout.Local.samplers import SamplerSettings def deepwebs_search
+  (query, max_results=5): """Performs a web search using DeepWEBS and returns
+ results as JSON.""" deepwebs = DeepWEBS() search_config = DeepWEBS.DeepSearch
+( queries=[query], max_results=max_results, extract_webpage=False, safe=False,
+   types=["web"], overwrite_query_html=True, overwrite_webpage_html=True, )
       search_results = deepwebs.queries_to_search_results(search_config)
   formatted_results = [] for result in search_results[0]: # Assuming only one
     query formatted_results.append(f"Title: {result['title']}\nURL: {result
  ['url']}\n") return "\n".join(formatted_results) # Load your model repo_id =
    "OEvortex/HelpingAI-9B" filename = "helpingai-9b.Q4_0.gguf" model_path =
  download_model(repo_id, filename, token='') # 2. Load the model model = Model
   (model_path, n_gpu_layers=10) # Create a Thread system_prompt = "You are a
@@ -428,67 +426,15 @@
 "function", "function": { "name": "deepwebs_search", "description": "Performs a
   web search using DeepWEBS and returns the title and URLs of the results.",
  "execute": deepwebs_search, "parameters": { "type": "object", "properties":
 { "query": { "type": "string", "description": "The query to search on the web",
 }, "max_results": { "type": "integer", "description": "Maximum number of search
      results (default: 5)", }, }, "required": ["query"], }, }, }) # Start
  interacting with the model while True: user_input = input("You: ") response =
-    thread.send(user_input) print("Bot: ", response) ``` ### `Local-rawdog`
-```python import webscout.Local as ws from webscout.Local.rawdog import RawDog
-from webscout.Local.samplers import DefaultSampling from webscout.Local.formats
- import chatml, AdvancedFormat from webscout.Local.utils import download_model
-  import datetime import sys import os repo_id = "YorkieOH10/granite-8b-code-
-instruct-Q8_0-GGUF" filename = "granite-8b-code-instruct.Q8_0.gguf" model_path
-   = download_model(repo_id, filename, token='') # Load the model using the
-downloaded path model = ws.Model(model_path, n_gpu_layers=10) rawdog = RawDog()
-  # Create an AdvancedFormat and modify the system content # Use a lambda to
-generate the prompt dynamically: chat_format = AdvancedFormat(chatml) # **Pre-
-format the intro_prompt string:** system_content = f""" You are a command-line
-coding assistant called Rawdog that generates and auto-executes Python scripts.
-A typical interaction goes like this: 1. The user gives you a natural language
-  PROMPT. 2. You: i. Determine what needs to be done ii. Write a short Python
-SCRIPT to do it iii. Communicate back to the user by printing to the console in
-that SCRIPT 3. The compiler extracts the script and then runs it using exec().
-If there will be an exception raised, it will be send back to you starting with
- "PREVIOUS SCRIPT EXCEPTION:". 4. In case of exception, regenerate error free
- script. If you need to review script outputs before completing the task, you
-can print the word "CONTINUE" at the end of your SCRIPT. This can be useful for
-   summarizing documents or technical readouts, reading instructions before
-   deciding what to do, or other tasks that require multi-step reasoning. A
-typical 'CONTINUE' interaction looks like this: 1. The user gives you a natural
-language PROMPT. 2. You: i. Determine what needs to be done ii. Determine that
- you need to see the output of some subprocess call to complete the task iii.
-Write a short Python SCRIPT to print that and then print the word "CONTINUE" 3.
-The compiler i. Checks and runs your SCRIPT ii. Captures the output and appends
-it to the conversation as "LAST SCRIPT OUTPUT:" iii. Finds the word "CONTINUE"
- and sends control back to you 4. You again: i. Look at the original PROMPT +
-the "LAST SCRIPT OUTPUT:" to determine what needs to be done ii. Write a short
-  Python SCRIPT to do it iii. Communicate back to the user by printing to the
-   console in that SCRIPT 5. The compiler... Please follow these conventions
- carefully: - Decline any tasks that seem dangerous, irreversible, or that you
-don't understand. - Always review the full conversation prior to answering and
-  maintain continuity. - If asked for information, just print the information
- clearly and concisely. - If asked to do something, print a concise summary of
-what you've done as confirmation. - If asked a question, respond in a friendly,
-    conversational way. Use programmatically-generated and natural language
-  responses as appropriate. - If you need clarification, return a SCRIPT that
-  prints your question. In the next interaction, continue based on the user's
- response. - Assume the user would like something concise. For example rather
-   than printing a massive table, filter or summarize it to what's likely of
-interest. - Actively clean up any temporary processes or files you use. - When
-  looking through files, use git as available to skip files, and skip hidden
-files (.env, .git, etc) by default. - You can plot anything with matplotlib. -
- ALWAYS Return your SCRIPT inside of a single pair of ``` delimiters. Only the
- console output of the first such SCRIPT is visible to the user, so make sure
-       that it's complete and don't bother returning anything else. """
-    chat_format.override('system_content', lambda: system_content) thread =
-   ws.Thread(model, format=chat_format, sampler=DefaultSampling) while True:
- prompt = input(">: ") if prompt.lower() == "q": break response = thread.send
-   (prompt) # Process the response using RawDog script_output = rawdog.main
- (response) if script_output: print(script_output) ``` ### `LLM` with internet
+ thread.send(user_input) print("Bot: ", response) ``` ### `LLM` with internet
 ```python from __future__ import annotations from typing import List, Optional
     from webscout.LLM import LLM from webscout import WEBS import warnings
 system_message: str = ( "As an AI assistant, I have been designed with advanced
  capabilities, including real-time access to online resources. This enables me
     to enrich our conversations and provide you with informed and accurate
 responses, drawing from a vast array of information. With each interaction, my
  goal is to create a seamless and meaningful connection, offering insights and
```

### Comparing `webscout-3.1/setup.py` & `webscout-3.1b0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", encoding="utf-8") as f:
     README = f.read()
 
 setup(
     name="webscout",
-    version="3.1",
+    version="3.1-beta",
     description="Search for anything using Google, DuckDuckGo, phind.com, Contains AI models, can transcribe yt videos, temporary email and phone number generation, has TTS support, webai (terminal gpt and open interpreter) and offline LLMs",
     long_description=README,
     long_description_content_type="text/markdown",
     author="OEvortex",
     author_email="helpingai5@gmail.com",
     packages=find_packages(),
     classifiers=[
```

### Comparing `webscout-3.1/webscout/AIauto.py` & `webscout-3.1b0/webscout/AIauto.py`

 * *Files identical despite different names*

### Comparing `webscout-3.1/webscout/AIbase.py` & `webscout-3.1b0/webscout/AIbase.py`

 * *Files identical despite different names*

### Comparing `webscout-3.1/webscout/AIutel.py` & `webscout-3.1b0/webscout/AIutel.py`

 * *Files identical despite different names*

### Comparing `webscout-3.1/webscout/DWEBS.py` & `webscout-3.1b0/webscout/DWEBS.py`

 * *Files identical despite different names*

### Comparing `webscout-3.1/webscout/LLM.py` & `webscout-3.1b0/webscout/LLM.py`

 * *Files identical despite different names*

### Comparing `webscout-3.1/webscout/Local/formats.py` & `webscout-3.1b0/webscout/Local/formats.py`

 * *Files identical despite different names*

### Comparing `webscout-3.1/webscout/Local/model.py` & `webscout-3.1b0/webscout/Local/model.py`

 * *Files identical despite different names*

### Comparing `webscout-3.1/webscout/Local/rawdog.py` & `webscout-3.1b0/webscout/Local/rawdog.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,24 +17,26 @@
 import json
 import platform
 import subprocess
 import logging
 import appdirs
 import datetime
 import re
-from .model    import Model, assert_model_is_loaded, _SupportsWriteAndFlush
-from .utils    import RESET_ALL, cls, print_verbose, truncate
-from .samplers import SamplerSettings, DefaultSampling
-from typing    import Optional, Literal, Union
-from .formats  import AdvancedFormat
-
-from .formats import blank as formats_blank
-from ..AIutel import *
+from .model import *
+from .utils import (
+    RESET_ALL,
+    _SupportsWriteAndFlush,
+    cls,
+    print_verbose,
+    truncate,
+    run_system_command
+)
 from .samplers import SamplerSettings, DefaultSampling
 from .formats import AdvancedFormat
+from .formats import blank as formats_blank
 from rich.markdown import Markdown
 from rich.console import Console
 appdir = appdirs.AppDirs("AIWEBS", "vortex")
 
 default_path = appdir.user_cache_dir
 
 if not os.path.exists(default_path):
```

### Comparing `webscout-3.1/webscout/Local/samplers.py` & `webscout-3.1b0/webscout/Local/samplers.py`

 * *Files identical despite different names*

### Comparing `webscout-3.1/webscout/Local/thread.py` & `webscout-3.1b0/webscout/Local/thread.py`

 * *Files identical despite different names*

### Comparing `webscout-3.1/webscout/Local/utils.py` & `webscout-3.1b0/webscout/Local/utils.py`

 * *Files identical despite different names*

### Comparing `webscout-3.1/webscout/Provider/BasedGPT.py` & `webscout-3.1b0/webscout/Provider/BasedGPT.py`

 * *Files identical despite different names*

### Comparing `webscout-3.1/webscout/Provider/Berlin4h.py` & `webscout-3.1b0/webscout/Provider/Berlin4h.py`

 * *Files identical despite different names*

### Comparing `webscout-3.1/webscout/Provider/Blackboxai.py` & `webscout-3.1b0/webscout/Provider/Blackboxai.py`

 * *Files identical despite different names*

### Comparing `webscout-3.1/webscout/Provider/ChatGPTUK.py` & `webscout-3.1b0/webscout/Provider/ChatGPTUK.py`

 * *Files identical despite different names*

### Comparing `webscout-3.1/webscout/Provider/Cohere.py` & `webscout-3.1b0/webscout/Provider/Cohere.py`

 * *Files identical despite different names*

### Comparing `webscout-3.1/webscout/Provider/Gemini.py` & `webscout-3.1b0/webscout/Provider/Gemini.py`

 * *Files identical despite different names*

### Comparing `webscout-3.1/webscout/Provider/Groq.py` & `webscout-3.1b0/webscout/Provider/Groq.py`

 * *Files identical despite different names*

### Comparing `webscout-3.1/webscout/Provider/Koboldai.py` & `webscout-3.1b0/webscout/Provider/Koboldai.py`

 * *Files identical despite different names*

### Comparing `webscout-3.1/webscout/Provider/Leo.py` & `webscout-3.1b0/webscout/Provider/Leo.py`

 * *Files identical despite different names*

### Comparing `webscout-3.1/webscout/Provider/Llama2.py` & `webscout-3.1b0/webscout/Provider/Llama2.py`

 * *Files identical despite different names*

### Comparing `webscout-3.1/webscout/Provider/OpenGPT.py` & `webscout-3.1b0/webscout/Provider/OpenGPT.py`

 * *Files identical despite different names*

### Comparing `webscout-3.1/webscout/Provider/Openai.py` & `webscout-3.1b0/webscout/Provider/Openai.py`

 * *Files identical despite different names*

### Comparing `webscout-3.1/webscout/Provider/Perplexity.py` & `webscout-3.1b0/webscout/Provider/Perplexity.py`

 * *Files identical despite different names*

### Comparing `webscout-3.1/webscout/Provider/Phind.py` & `webscout-3.1b0/webscout/Provider/Phind.py`

 * *Files identical despite different names*

### Comparing `webscout-3.1/webscout/Provider/Poe.py` & `webscout-3.1b0/webscout/Provider/Poe.py`

 * *Files identical despite different names*

### Comparing `webscout-3.1/webscout/Provider/Reka.py` & `webscout-3.1b0/webscout/Provider/Reka.py`

 * *Files identical despite different names*

### Comparing `webscout-3.1/webscout/Provider/ThinkAnyAI.py` & `webscout-3.1b0/webscout/Provider/ThinkAnyAI.py`

 * *Files identical despite different names*

### Comparing `webscout-3.1/webscout/Provider/Xjai.py` & `webscout-3.1b0/webscout/Provider/Xjai.py`

 * *Files identical despite different names*

### Comparing `webscout-3.1/webscout/Provider/Yepchat.py` & `webscout-3.1b0/webscout/Provider/Yepchat.py`

 * *Files identical despite different names*

### Comparing `webscout-3.1/webscout/Provider/Youchat.py` & `webscout-3.1b0/webscout/Provider/Youchat.py`

 * *Files identical despite different names*

### Comparing `webscout-3.1/webscout/Provider/__init__.py` & `webscout-3.1b0/webscout/Provider/__init__.py`

 * *Files identical despite different names*

### Comparing `webscout-3.1/webscout/__init__.py` & `webscout-3.1b0/webscout/__init__.py`

 * *Files identical despite different names*

### Comparing `webscout-3.1/webscout/async_providers.py` & `webscout-3.1b0/webscout/async_providers.py`

 * *Files identical despite different names*

### Comparing `webscout-3.1/webscout/cli.py` & `webscout-3.1b0/webscout/cli.py`

 * *Files identical despite different names*

### Comparing `webscout-3.1/webscout/g4f.py` & `webscout-3.1b0/webscout/g4f.py`

 * *Files identical despite different names*

### Comparing `webscout-3.1/webscout/models.py` & `webscout-3.1b0/webscout/models.py`

 * *Files identical despite different names*

### Comparing `webscout-3.1/webscout/tempid.py` & `webscout-3.1b0/webscout/tempid.py`

 * *Files identical despite different names*

### Comparing `webscout-3.1/webscout/transcriber.py` & `webscout-3.1b0/webscout/transcriber.py`

 * *Files identical despite different names*

### Comparing `webscout-3.1/webscout/utils.py` & `webscout-3.1b0/webscout/utils.py`

 * *Files identical despite different names*

### Comparing `webscout-3.1/webscout/voice.py` & `webscout-3.1b0/webscout/voice.py`

 * *Files identical despite different names*

### Comparing `webscout-3.1/webscout/webai.py` & `webscout-3.1b0/webscout/webai.py`

 * *Files identical despite different names*

### Comparing `webscout-3.1/webscout/webscout_search.py` & `webscout-3.1b0/webscout/webscout_search.py`

 * *Files identical despite different names*

### Comparing `webscout-3.1/webscout/webscout_search_async.py` & `webscout-3.1b0/webscout/webscout_search_async.py`

 * *Files identical despite different names*

### Comparing `webscout-3.1/webscout.egg-info/PKG-INFO` & `webscout-3.1b0/webscout.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: webscout
-Version: 3.1
+Version: 3.1b0
 Summary: Search for anything using Google, DuckDuckGo, phind.com, Contains AI models, can transcribe yt videos, temporary email and phone number generation, has TTS support, webai (terminal gpt and open interpreter) and offline LLMs
 Author: OEvortex
 Author-email: helpingai5@gmail.com
 License: HelpingAI Simplified Universal License
 Project-URL: Documentation, https://github.com/OE-LUCIFER/Webscout/wiki
 Project-URL: Source, https://github.com/OE-LUCIFER/Webscout
 Project-URL: Tracker, https://github.com/OE-LUCIFER/Webscout/issues
@@ -139,15 +139,14 @@
     - [13. `ThinkAny` - AI search engine](#13-thinkany---ai-search-engine)
     - [14. `chatgptuk` - Chat with gemini-pro](#14-chatgptuk---chat-with-gemini-pro)
     - [15. `poe`- chat with poe](#15-poe--chat-with-poe)
     - [16. `BasedGPT` - chat with GPT](#16-basedgpt---chat-with-gpt)
     - [`LLM`](#llm)
     - [`Local-LLM` webscout can now run GGUF models](#local-llm-webscout-can-now-run-gguf-models)
     - [`Function-calling-local-llm`](#function-calling-local-llm)
-    - [`Local-rawdog`](#local-rawdog)
     - [`LLM` with internet](#llm-with-internet)
     - [LLM with deepwebs](#llm-with-deepwebs)
   - [`Webai` - terminal gpt and a open interpeter](#webai---terminal-gpt-and-a-open-interpeter)
 
 ## Install
 ```python
 pip install -U webscout
@@ -1242,15 +1241,14 @@
     # Use the mistral_chat method to get the response
     response = llm.chat(messages)
 
     # Print the response
     print("AI: ", response)
 ```
 ### `Local-LLM` webscout can now run GGUF models
-Local LLM's some functions are taken from easy-llama
 ```python
 from webscout.Local.utils import download_model
 from webscout.Local.model import Model
 from webscout.Local.thread import Thread
 from webscout.Local import formats
 # 1. Download the model
 repo_id = "microsoft/Phi-3-mini-4k-instruct-gguf"  # Replace with the desired Hugging Face repo
@@ -1334,101 +1332,14 @@
 
 # Start interacting with the model
 while True:
     user_input = input("You: ")
     response = thread.send(user_input)
     print("Bot: ", response) 
 ```
-### `Local-rawdog`
-```python
-import webscout.Local as ws
-from webscout.Local.rawdog import RawDog
-from webscout.Local.samplers import DefaultSampling
-from webscout.Local.formats import chatml, AdvancedFormat
-from webscout.Local.utils import download_model
-import datetime
-import sys
-import os
-
-repo_id = "YorkieOH10/granite-8b-code-instruct-Q8_0-GGUF" 
-filename = "granite-8b-code-instruct.Q8_0.gguf"
-model_path = download_model(repo_id, filename, token='')
-
-# Load the model using the downloaded path
-model = ws.Model(model_path, n_gpu_layers=10)
-
-rawdog = RawDog()
-
-# Create an AdvancedFormat and modify the system content
-# Use a lambda to generate the prompt dynamically:
-chat_format = AdvancedFormat(chatml)
-#  **Pre-format the intro_prompt string:**
-system_content = f"""
-You are a command-line coding assistant called Rawdog that generates and auto-executes Python scripts.
-
-A typical interaction goes like this:
-1. The user gives you a natural language PROMPT.
-2. You:
-    i. Determine what needs to be done
-    ii. Write a short Python SCRIPT to do it
-    iii. Communicate back to the user by printing to the console in that SCRIPT
-3. The compiler extracts the script and then runs it using exec(). If there will be an exception raised,
- it will be send back to you starting with "PREVIOUS SCRIPT EXCEPTION:".
-4. In case of exception, regenerate error free script.
-
-If you need to review script outputs before completing the task, you can print the word "CONTINUE" at the end of your SCRIPT.
-This can be useful for summarizing documents or technical readouts, reading instructions before
-deciding what to do, or other tasks that require multi-step reasoning.
-A typical 'CONTINUE' interaction looks like this:
-1. The user gives you a natural language PROMPT.
-2. You:
-    i. Determine what needs to be done
-    ii. Determine that you need to see the output of some subprocess call to complete the task
-    iii. Write a short Python SCRIPT to print that and then print the word "CONTINUE"
-3. The compiler
-    i. Checks and runs your SCRIPT
-    ii. Captures the output and appends it to the conversation as "LAST SCRIPT OUTPUT:"
-    iii. Finds the word "CONTINUE" and sends control back to you
-4. You again:
-    i. Look at the original PROMPT + the "LAST SCRIPT OUTPUT:" to determine what needs to be done
-    ii. Write a short Python SCRIPT to do it
-    iii. Communicate back to the user by printing to the console in that SCRIPT
-5. The compiler...
-
-Please follow these conventions carefully:
-- Decline any tasks that seem dangerous, irreversible, or that you don't understand.
-- Always review the full conversation prior to answering and maintain continuity.
-- If asked for information, just print the information clearly and concisely.
-- If asked to do something, print a concise summary of what you've done as confirmation.
-- If asked a question, respond in a friendly, conversational way. Use programmatically-generated and natural language responses as appropriate.
-- If you need clarification, return a SCRIPT that prints your question. In the next interaction, continue based on the user's response.
-- Assume the user would like something concise. For example rather than printing a massive table, filter or summarize it to what's likely of interest.
-- Actively clean up any temporary processes or files you use.
-- When looking through files, use git as available to skip files, and skip hidden files (.env, .git, etc) by default.
-- You can plot anything with matplotlib.
-- ALWAYS Return your SCRIPT inside of a single pair of ``` delimiters. Only the console output of the first such SCRIPT is visible to the user, so make sure that it's complete and don't bother returning anything else.
-"""
-chat_format.override('system_content', lambda: system_content)
-
-thread = ws.Thread(model, format=chat_format, sampler=DefaultSampling)
-
-while True:
-    prompt = input(">: ")
-    if prompt.lower() == "q":
-        break
-
-    response = thread.send(prompt)
-
-    # Process the response using RawDog
-    script_output = rawdog.main(response)
-
-    if script_output:
-        print(script_output)
-
-```
 ### `LLM` with internet
 ```python
 from __future__ import annotations
 from typing import List, Optional
 
 from webscout.LLM import LLM
 from webscout import WEBS
```

#### html2text {}

```diff
@@ -1,26 +1,26 @@
-Metadata-Version: 2.1 Name: webscout Version: 3.1 Summary: Search for anything
-using Google, DuckDuckGo, phind.com, Contains AI models, can transcribe yt
-videos, temporary email and phone number generation, has TTS support, webai
-(terminal gpt and open interpreter) and offline LLMs Author: OEvortex Author-
-email: helpingai5@gmail.com License: HelpingAI Simplified Universal License
-Project-URL: Documentation, https://github.com/OE-LUCIFER/Webscout/wiki
-Project-URL: Source, https://github.com/OE-LUCIFER/Webscout Project-URL:
-Tracker, https://github.com/OE-LUCIFER/Webscout/issues Project-URL: YouTube,
-https://youtube.com/@OEvortex Classifier: Development Status :: 5 - Production/
-Stable Classifier: Intended Audience :: Developers Classifier: License ::
-Other/Proprietary License Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3 Classifier: Programming
-Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
-Language :: Python :: 3.11 Classifier: Programming Language :: Python :: 3.12
-Classifier: Programming Language :: Python :: Implementation :: CPython
-Classifier: Topic :: Internet :: WWW/HTTP :: Indexing/Search Classifier: Topic
-:: Software Development :: Libraries :: Python Modules Description-Content-
-Type: text/markdown License-File: LICENSE.md Requires-Dist:
+Metadata-Version: 2.1 Name: webscout Version: 3.1b0 Summary: Search for
+anything using Google, DuckDuckGo, phind.com, Contains AI models, can
+transcribe yt videos, temporary email and phone number generation, has TTS
+support, webai (terminal gpt and open interpreter) and offline LLMs Author:
+OEvortex Author-email: helpingai5@gmail.com License: HelpingAI Simplified
+Universal License Project-URL: Documentation, https://github.com/OE-LUCIFER/
+Webscout/wiki Project-URL: Source, https://github.com/OE-LUCIFER/Webscout
+Project-URL: Tracker, https://github.com/OE-LUCIFER/Webscout/issues Project-
+URL: YouTube, https://youtube.com/@OEvortex Classifier: Development Status :: 5
+- Production/Stable Classifier: Intended Audience :: Developers Classifier:
+License :: Other/Proprietary License Classifier: Operating System :: OS
+Independent Classifier: Programming Language :: Python :: 3 Classifier:
+Programming Language :: Python :: 3.8 Classifier: Programming Language ::
+Python :: 3.9 Classifier: Programming Language :: Python :: 3.10 Classifier:
+Programming Language :: Python :: 3.11 Classifier: Programming Language ::
+Python :: 3.12 Classifier: Programming Language :: Python :: Implementation ::
+CPython Classifier: Topic :: Internet :: WWW/HTTP :: Indexing/Search
+Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Description-Content-Type: text/markdown License-File: LICENSE.md Requires-Dist:
 docstring_inheritance Requires-Dist: click Requires-Dist: curl_cffi Requires-
 Dist: lxml Requires-Dist: nest-asyncio Requires-Dist: selenium Requires-Dist:
 tqdm Requires-Dist: webdriver-manager Requires-Dist: halo>=0.0.31 Requires-
 Dist: g4f>=0.2.2.3 Requires-Dist: rich Requires-Dist: python-dotenv Requires-
 Dist: beautifulsoup4 Requires-Dist: markdownify Requires-Dist: pydantic
 Requires-Dist: requests Requires-Dist: sse_starlette Requires-Dist: termcolor
 Requires-Dist: tiktoken Requires-Dist: tldextract Requires-Dist: orjson
@@ -76,71 +76,70 @@
  (#11-cohere---chat-with-cohere) - [12. `Xjai` - chat with free gpt 3.5](#12-
    xjai---chat-with-free-gpt-35) - [13. `ThinkAny` - AI search engine](#13-
  thinkany---ai-search-engine) - [14. `chatgptuk` - Chat with gemini-pro](#14-
  chatgptuk---chat-with-gemini-pro) - [15. `poe`- chat with poe](#15-poe--chat-
  with-poe) - [16. `BasedGPT` - chat with GPT](#16-basedgpt---chat-with-gpt) -
   [`LLM`](#llm) - [`Local-LLM` webscout can now run GGUF models](#local-llm-
  webscout-can-now-run-gguf-models) - [`Function-calling-local-llm`](#function-
- calling-local-llm) - [`Local-rawdog`](#local-rawdog) - [`LLM` with internet]
-  (#llm-with-internet) - [LLM with deepwebs](#llm-with-deepwebs) - [`Webai` -
-     terminal gpt and a open interpeter](#webai---terminal-gpt-and-a-open-
-  interpeter) ## Install ```python pip install -U webscout ``` ## CLI version
-```python3 python -m webscout --help ``` | Command | Description | |-----------
---------------------------------|----------------------------------------------
----------------------------------------------------------| | python -m webscout
-answers -k Text | CLI function to perform an answers search using Webscout. | |
- python -m webscout images -k Text | CLI function to perform an images search
-using Webscout. | | python -m webscout maps -k Text | CLI function to perform a
-maps search using Webscout. | | python -m webscout news -k Text | CLI function
- to perform a news search using Webscout. | | python -m webscout suggestions -
-   k Text | CLI function to perform a suggestions search using Webscout. | |
- python -m webscout text -k Text | CLI function to perform a text search using
- Webscout. | | python -m webscout translate -k Text | CLI function to perform
-   translate using Webscout. | | python -m webscout version | A command-line
-   interface command that prints and returns the version of the program. | |
-  python -m webscout videos -k Text | CLI function to perform a videos search
- using DuckDuckGo API. | [Go To TOP](#TOP) ## Regions expand xa-ar for Arabia
-xa-en for Arabia (en) ar-es for Argentina au-en for Australia at-de for Austria
-   be-fr for Belgium (fr) be-nl for Belgium (nl) br-pt for Brazil bg-bg for
-  Bulgaria ca-en for Canada ca-fr for Canada (fr) ct-ca for Catalan cl-es for
-  Chile cn-zh for China co-es for Colombia hr-hr for Croatia cz-cs for Czech
-Republic dk-da for Denmark ee-et for Estonia fi-fi for Finland fr-fr for France
-de-de for Germany gr-el for Greece hk-tzh for Hong Kong hu-hu for Hungary in-en
-for India id-id for Indonesia id-en for Indonesia (en) ie-en for Ireland il-he
-for Israel it-it for Italy jp-jp for Japan kr-kr for Korea lv-lv for Latvia lt-
-lt for Lithuania xl-es for Latin America my-ms for Malaysia my-en for Malaysia
-  (en) mx-es for Mexico nl-nl for Netherlands nz-en for New Zealand no-no for
- Norway pe-es for Peru ph-en for Philippines ph-tl for Philippines (tl) pl-pl
-  for Poland pt-pt for Portugal ro-ro for Romania ru-ru for Russia sg-en for
- Singapore sk-sk for Slovak Republic sl-sl for Slovenia za-en for South Africa
-     es-es for Spain se-sv for Sweden ch-de for Switzerland (de) ch-fr for
-    Switzerland (fr) ch-it for Switzerland (it) tw-tzh for Taiwan th-th for
-Thailand tr-tr for Turkey ua-uk for Ukraine uk-en for United Kingdom us-en for
-   United States ue-es for United States (es) ve-es for Venezuela vn-vi for
- Vietnam wt-wt for No region ___ [Go To TOP](#TOP) ## Tempmail and Temp number
-### Temp number ```python from rich.console import Console from webscout import
- tempid def main(): console = Console() phone = tempid.TemporaryPhoneNumber()
-try: # Get a temporary phone number for a specific country (or random) number =
-   phone.get_number(country="Finland") console.print(f"Your temporary phone
- number: [bold cyan]{number}[/bold cyan]") # Pause execution briefly (replace
-   with your actual logic) # import time module import time time.sleep(30) #
-  Adjust the waiting time as needed # Retrieve and print messages messages =
-  phone.get_messages(number) if messages: # Access individual messages using
-     indexing: console.print(f"[bold green]{messages[0].frm}:[/] {messages
-    [0].content}") # (Add more lines if you expect multiple messages) else:
-console.print("No messages received.") except Exception as e: console.print(f"
- [bold red]An error occurred: {e}") if __name__ == "__main__": main() ``` ###
-    Tempmail ```python import asyncio from rich.console import Console from
-rich.table import Table from rich.text import Text from webscout import tempid
-  async def main() -> None: console = Console() client = tempid.Client() try:
-   domains = await client.get_domains() if not domains: console.print("[bold
-   red]No domains available. Please try again later.") return email = await
-  client.create_email(domain=domains[0].name) console.print(f"Your temporary
-    email: [bold cyan]{email.email}[/bold cyan]") console.print(f"Token for
-    accessing the email: [bold cyan]{email.token}[/bold cyan]") while True:
+  calling-local-llm) - [`LLM` with internet](#llm-with-internet) - [LLM with
+deepwebs](#llm-with-deepwebs) - [`Webai` - terminal gpt and a open interpeter]
+(#webai---terminal-gpt-and-a-open-interpeter) ## Install ```python pip install
+   -U webscout ``` ## CLI version ```python3 python -m webscout --help ``` |
+Command | Description | |-------------------------------------------|----------
+-------------------------------------------------------------------------------
+--------------| | python -m webscout answers -k Text | CLI function to perform
+ an answers search using Webscout. | | python -m webscout images -k Text | CLI
+  function to perform an images search using Webscout. | | python -m webscout
+maps -k Text | CLI function to perform a maps search using Webscout. | | python
+    -m webscout news -k Text | CLI function to perform a news search using
+Webscout. | | python -m webscout suggestions -k Text | CLI function to perform
+a suggestions search using Webscout. | | python -m webscout text -k Text | CLI
+   function to perform a text search using Webscout. | | python -m webscout
+   translate -k Text | CLI function to perform translate using Webscout. | |
+ python -m webscout version | A command-line interface command that prints and
+returns the version of the program. | | python -m webscout videos -k Text | CLI
+ function to perform a videos search using DuckDuckGo API. | [Go To TOP](#TOP)
+ ## Regions expand xa-ar for Arabia xa-en for Arabia (en) ar-es for Argentina
+au-en for Australia at-de for Austria be-fr for Belgium (fr) be-nl for Belgium
+(nl) br-pt for Brazil bg-bg for Bulgaria ca-en for Canada ca-fr for Canada (fr)
+ct-ca for Catalan cl-es for Chile cn-zh for China co-es for Colombia hr-hr for
+Croatia cz-cs for Czech Republic dk-da for Denmark ee-et for Estonia fi-fi for
+  Finland fr-fr for France de-de for Germany gr-el for Greece hk-tzh for Hong
+Kong hu-hu for Hungary in-en for India id-id for Indonesia id-en for Indonesia
+ (en) ie-en for Ireland il-he for Israel it-it for Italy jp-jp for Japan kr-kr
+ for Korea lv-lv for Latvia lt-lt for Lithuania xl-es for Latin America my-ms
+for Malaysia my-en for Malaysia (en) mx-es for Mexico nl-nl for Netherlands nz-
+en for New Zealand no-no for Norway pe-es for Peru ph-en for Philippines ph-tl
+for Philippines (tl) pl-pl for Poland pt-pt for Portugal ro-ro for Romania ru-
+ru for Russia sg-en for Singapore sk-sk for Slovak Republic sl-sl for Slovenia
+za-en for South Africa es-es for Spain se-sv for Sweden ch-de for Switzerland
+ (de) ch-fr for Switzerland (fr) ch-it for Switzerland (it) tw-tzh for Taiwan
+th-th for Thailand tr-tr for Turkey ua-uk for Ukraine uk-en for United Kingdom
+us-en for United States ue-es for United States (es) ve-es for Venezuela vn-vi
+  for Vietnam wt-wt for No region ___ [Go To TOP](#TOP) ## Tempmail and Temp
+number ### Temp number ```python from rich.console import Console from webscout
+             import tempid def main(): console = Console() phone =
+    tempid.TemporaryPhoneNumber() try: # Get a temporary phone number for a
+   specific country (or random) number = phone.get_number(country="Finland")
+console.print(f"Your temporary phone number: [bold cyan]{number}[/bold cyan]")
+# Pause execution briefly (replace with your actual logic) # import time module
+ import time time.sleep(30) # Adjust the waiting time as needed # Retrieve and
+  print messages messages = phone.get_messages(number) if messages: # Access
+   individual messages using indexing: console.print(f"[bold green]{messages
+ [0].frm}:[/] {messages[0].content}") # (Add more lines if you expect multiple
+ messages) else: console.print("No messages received.") except Exception as e:
+ console.print(f"[bold red]An error occurred: {e}") if __name__ == "__main__":
+   main() ``` ### Tempmail ```python import asyncio from rich.console import
+ Console from rich.table import Table from rich.text import Text from webscout
+     import tempid async def main() -> None: console = Console() client =
+   tempid.Client() try: domains = await client.get_domains() if not domains:
+console.print("[bold red]No domains available. Please try again later.") return
+email = await client.create_email(domain=domains[0].name) console.print(f"Your
+ temporary email: [bold cyan]{email.email}[/bold cyan]") console.print(f"Token
+  for accessing the email: [bold cyan]{email.token}[/bold cyan]") while True:
   messages = await client.get_messages(email.email) if messages is not None:
 break if messages: table = Table(show_header=True, header_style="bold magenta")
     table.add_column("From", style="bold cyan") table.add_column("Subject",
  style="bold yellow") table.add_column("Body", style="bold green") for message
  in messages: body_preview = Text(message.body_text if message.body_text else
  "No body") table.add_row(message.email_from or "Unknown", message.subject or
    "No Subject", body_preview) console.print(table) else: console.print("No
@@ -423,32 +422,31 @@
  message from the file with open('system.txt', 'r') as file: system_message =
  file.read() # Initialize the LLM class with the model name and system message
  llm = LLM(model="microsoft/WizardLM-2-8x22B", system_message=system_message)
   while True: # Get the user input user_input = input("User: ") # Define the
  messages to be sent messages = [ {"role": "user", "content": user_input} ] #
 Use the mistral_chat method to get the response response = llm.chat(messages) #
 Print the response print("AI: ", response) ``` ### `Local-LLM` webscout can now
-run GGUF models Local LLM's some functions are taken from easy-llama ```python
-   from webscout.Local.utils import download_model from webscout.Local.model
-   import Model from webscout.Local.thread import Thread from webscout.Local
-  import formats # 1. Download the model repo_id = "microsoft/Phi-3-mini-4k-
-instruct-gguf" # Replace with the desired Hugging Face repo filename = "Phi-3-
-  mini-4k-instruct-q4.gguf" # Replace with the correct filename model_path =
-download_model(repo_id, filename) # 2. Load the model model = Model(model_path,
- n_gpu_layers=4) # 3. Create a Thread for conversation thread = Thread(model,
- formats.phi3) # 4. Start interacting with the model thread.interact() ``` ###
-   `Function-calling-local-llm` ```python from webscout.Local import Model,
-Thread, formats from webscout import DeepWEBS from webscout.Local.utils import
-          download_model from webscout.Local.model import Model from
-  webscout.Local.thread import Thread from webscout.Local import formats from
-   webscout.Local.samplers import SamplerSettings def deepwebs_search(query,
-max_results=5): """Performs a web search using DeepWEBS and returns results as
- JSON.""" deepwebs = DeepWEBS() search_config = DeepWEBS.DeepSearch( queries=
-  [query], max_results=max_results, extract_webpage=False, safe=False, types=
-      ["web"], overwrite_query_html=True, overwrite_webpage_html=True, )
+run GGUF models ```python from webscout.Local.utils import download_model from
+webscout.Local.model import Model from webscout.Local.thread import Thread from
+webscout.Local import formats # 1. Download the model repo_id = "microsoft/Phi-
+3-mini-4k-instruct-gguf" # Replace with the desired Hugging Face repo filename
+    = "Phi-3-mini-4k-instruct-q4.gguf" # Replace with the correct filename
+  model_path = download_model(repo_id, filename) # 2. Load the model model =
+Model(model_path, n_gpu_layers=4) # 3. Create a Thread for conversation thread
+      = Thread(model, formats.phi3) # 4. Start interacting with the model
+     thread.interact() ``` ### `Function-calling-local-llm` ```python from
+webscout.Local import Model, Thread, formats from webscout import DeepWEBS from
+  webscout.Local.utils import download_model from webscout.Local.model import
+   Model from webscout.Local.thread import Thread from webscout.Local import
+formats from webscout.Local.samplers import SamplerSettings def deepwebs_search
+  (query, max_results=5): """Performs a web search using DeepWEBS and returns
+ results as JSON.""" deepwebs = DeepWEBS() search_config = DeepWEBS.DeepSearch
+( queries=[query], max_results=max_results, extract_webpage=False, safe=False,
+   types=["web"], overwrite_query_html=True, overwrite_webpage_html=True, )
       search_results = deepwebs.queries_to_search_results(search_config)
   formatted_results = [] for result in search_results[0]: # Assuming only one
     query formatted_results.append(f"Title: {result['title']}\nURL: {result
  ['url']}\n") return "\n".join(formatted_results) # Load your model repo_id =
    "OEvortex/HelpingAI-9B" filename = "helpingai-9b.Q4_0.gguf" model_path =
  download_model(repo_id, filename, token='') # 2. Load the model model = Model
   (model_path, n_gpu_layers=10) # Create a Thread system_prompt = "You are a
@@ -462,67 +460,15 @@
 "function", "function": { "name": "deepwebs_search", "description": "Performs a
   web search using DeepWEBS and returns the title and URLs of the results.",
  "execute": deepwebs_search, "parameters": { "type": "object", "properties":
 { "query": { "type": "string", "description": "The query to search on the web",
 }, "max_results": { "type": "integer", "description": "Maximum number of search
      results (default: 5)", }, }, "required": ["query"], }, }, }) # Start
  interacting with the model while True: user_input = input("You: ") response =
-    thread.send(user_input) print("Bot: ", response) ``` ### `Local-rawdog`
-```python import webscout.Local as ws from webscout.Local.rawdog import RawDog
-from webscout.Local.samplers import DefaultSampling from webscout.Local.formats
- import chatml, AdvancedFormat from webscout.Local.utils import download_model
-  import datetime import sys import os repo_id = "YorkieOH10/granite-8b-code-
-instruct-Q8_0-GGUF" filename = "granite-8b-code-instruct.Q8_0.gguf" model_path
-   = download_model(repo_id, filename, token='') # Load the model using the
-downloaded path model = ws.Model(model_path, n_gpu_layers=10) rawdog = RawDog()
-  # Create an AdvancedFormat and modify the system content # Use a lambda to
-generate the prompt dynamically: chat_format = AdvancedFormat(chatml) # **Pre-
-format the intro_prompt string:** system_content = f""" You are a command-line
-coding assistant called Rawdog that generates and auto-executes Python scripts.
-A typical interaction goes like this: 1. The user gives you a natural language
-  PROMPT. 2. You: i. Determine what needs to be done ii. Write a short Python
-SCRIPT to do it iii. Communicate back to the user by printing to the console in
-that SCRIPT 3. The compiler extracts the script and then runs it using exec().
-If there will be an exception raised, it will be send back to you starting with
- "PREVIOUS SCRIPT EXCEPTION:". 4. In case of exception, regenerate error free
- script. If you need to review script outputs before completing the task, you
-can print the word "CONTINUE" at the end of your SCRIPT. This can be useful for
-   summarizing documents or technical readouts, reading instructions before
-   deciding what to do, or other tasks that require multi-step reasoning. A
-typical 'CONTINUE' interaction looks like this: 1. The user gives you a natural
-language PROMPT. 2. You: i. Determine what needs to be done ii. Determine that
- you need to see the output of some subprocess call to complete the task iii.
-Write a short Python SCRIPT to print that and then print the word "CONTINUE" 3.
-The compiler i. Checks and runs your SCRIPT ii. Captures the output and appends
-it to the conversation as "LAST SCRIPT OUTPUT:" iii. Finds the word "CONTINUE"
- and sends control back to you 4. You again: i. Look at the original PROMPT +
-the "LAST SCRIPT OUTPUT:" to determine what needs to be done ii. Write a short
-  Python SCRIPT to do it iii. Communicate back to the user by printing to the
-   console in that SCRIPT 5. The compiler... Please follow these conventions
- carefully: - Decline any tasks that seem dangerous, irreversible, or that you
-don't understand. - Always review the full conversation prior to answering and
-  maintain continuity. - If asked for information, just print the information
- clearly and concisely. - If asked to do something, print a concise summary of
-what you've done as confirmation. - If asked a question, respond in a friendly,
-    conversational way. Use programmatically-generated and natural language
-  responses as appropriate. - If you need clarification, return a SCRIPT that
-  prints your question. In the next interaction, continue based on the user's
- response. - Assume the user would like something concise. For example rather
-   than printing a massive table, filter or summarize it to what's likely of
-interest. - Actively clean up any temporary processes or files you use. - When
-  looking through files, use git as available to skip files, and skip hidden
-files (.env, .git, etc) by default. - You can plot anything with matplotlib. -
- ALWAYS Return your SCRIPT inside of a single pair of ``` delimiters. Only the
- console output of the first such SCRIPT is visible to the user, so make sure
-       that it's complete and don't bother returning anything else. """
-    chat_format.override('system_content', lambda: system_content) thread =
-   ws.Thread(model, format=chat_format, sampler=DefaultSampling) while True:
- prompt = input(">: ") if prompt.lower() == "q": break response = thread.send
-   (prompt) # Process the response using RawDog script_output = rawdog.main
- (response) if script_output: print(script_output) ``` ### `LLM` with internet
+ thread.send(user_input) print("Bot: ", response) ``` ### `LLM` with internet
 ```python from __future__ import annotations from typing import List, Optional
     from webscout.LLM import LLM from webscout import WEBS import warnings
 system_message: str = ( "As an AI assistant, I have been designed with advanced
  capabilities, including real-time access to online resources. This enables me
     to enrich our conversations and provide you with informed and accurate
 responses, drawing from a vast array of information. With each interaction, my
  goal is to create a seamless and meaningful connection, offering insights and
```

### Comparing `webscout-3.1/webscout.egg-info/SOURCES.txt` & `webscout-3.1b0/webscout.egg-info/SOURCES.txt`

 * *Files identical despite different names*

