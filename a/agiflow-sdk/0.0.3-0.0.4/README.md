# Comparing `tmp/agiflow_sdk-0.0.3.tar.gz` & `tmp/agiflow_sdk-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "agiflow_sdk-0.0.3.tar", max compression
+gzip compressed data, was "agiflow_sdk-0.0.4.tar", max compression
```

## Comparing `agiflow_sdk-0.0.3.tar` & `agiflow_sdk-0.0.4.tar`

### file list

```diff
@@ -1,264 +1,265 @@
--rw-r--r--   0        0        0      394 2024-06-02 02:24:45.176730 agiflow_sdk-0.0.3/README.md
--rw-r--r--   0        0        0     5480 2024-06-02 02:24:45.177105 agiflow_sdk-0.0.3/agiflow/__init__.py
--rw-r--r--   0        0        0      889 2024-06-02 02:24:45.178092 agiflow_sdk-0.0.3/agiflow/config/__init__.py
--rw-r--r--   0        0        0     1838 2024-06-02 02:24:45.178403 agiflow_sdk-0.0.3/agiflow/config/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0      274 2024-06-02 02:24:45.178660 agiflow_sdk-0.0.3/agiflow/config/__pycache__/constants.cpython-311.pyc
--rw-r--r--   0        0        0     1451 2024-06-02 02:24:45.178841 agiflow_sdk-0.0.3/agiflow/config/__pycache__/environment_vars.cpython-311.pyc
--rw-r--r--   0        0        0       72 2024-06-02 02:24:45.179100 agiflow_sdk-0.0.3/agiflow/config/constants.py
--rw-r--r--   0        0        0     1338 2024-06-02 02:24:45.179350 agiflow_sdk-0.0.3/agiflow/config/environment_vars.py
--rw-r--r--   0        0        0     6148 2024-06-02 02:24:45.179714 agiflow_sdk-0.0.3/agiflow/opentelemetry/.DS_Store
--rw-r--r--   0        0        0     1037 2024-06-02 02:24:45.180029 agiflow_sdk-0.0.3/agiflow/opentelemetry/__init__.py
--rw-r--r--   0        0        0     1379 2024-06-02 02:24:45.180588 agiflow_sdk-0.0.3/agiflow/opentelemetry/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0     4092 2024-06-02 02:24:45.180858 agiflow_sdk-0.0.3/agiflow/opentelemetry/__pycache__/trace_store.cpython-311.pyc
--rw-r--r--   0        0        0      223 2024-06-02 02:24:45.181102 agiflow_sdk-0.0.3/agiflow/opentelemetry/__pycache__/version.cpython-311.pyc
--rw-r--r--   0        0        0     1112 2024-06-02 02:24:45.181463 agiflow_sdk-0.0.3/agiflow/opentelemetry/context/__init__.py
--rw-r--r--   0        0        0     1289 2024-06-02 02:24:45.181798 agiflow_sdk-0.0.3/agiflow/opentelemetry/context/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0     1682 2024-06-02 02:24:45.181979 agiflow_sdk-0.0.3/agiflow/opentelemetry/context/__pycache__/constants.cpython-311.pyc
--rw-r--r--   0        0        0     2868 2024-06-02 02:24:45.182221 agiflow_sdk-0.0.3/agiflow/opentelemetry/context/__pycache__/context.cpython-311.pyc
--rw-r--r--   0        0        0     2653 2024-06-02 02:24:45.182452 agiflow_sdk-0.0.3/agiflow/opentelemetry/context/__pycache__/context_propagation.cpython-311.pyc
--rw-r--r--   0        0        0     2105 2024-06-02 02:24:45.182688 agiflow_sdk-0.0.3/agiflow/opentelemetry/context/__pycache__/set_span_from_context.cpython-311.pyc
--rw-r--r--   0        0        0     2101 2024-06-02 02:24:45.183005 agiflow_sdk-0.0.3/agiflow/opentelemetry/context/__pycache__/span_from_context.cpython-311.pyc
--rw-r--r--   0        0        0      673 2024-06-02 02:24:45.183246 agiflow_sdk-0.0.3/agiflow/opentelemetry/context/constants.py
--rw-r--r--   0        0        0     1231 2024-06-02 02:24:45.183544 agiflow_sdk-0.0.3/agiflow/opentelemetry/context/context.py
--rw-r--r--   0        0        0     1644 2024-06-02 02:24:45.183785 agiflow_sdk-0.0.3/agiflow/opentelemetry/context/context_propagation.py
--rw-r--r--   0        0        0     1285 2024-06-02 02:24:45.184012 agiflow_sdk-0.0.3/agiflow/opentelemetry/context/span_from_context.py
--rw-r--r--   0        0        0     1583 2024-06-02 02:24:45.184357 agiflow_sdk-0.0.3/agiflow/opentelemetry/convention/__init__.py
--rw-r--r--   0        0        0     2184 2024-06-02 02:24:45.184637 agiflow_sdk-0.0.3/agiflow/opentelemetry/convention/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0     2922 2024-06-02 02:24:45.184871 agiflow_sdk-0.0.3/agiflow/opentelemetry/convention/__pycache__/agiflow_attributes.cpython-311.pyc
--rw-r--r--   0        0        0     7800 2024-06-02 02:24:45.185109 agiflow_sdk-0.0.3/agiflow/opentelemetry/convention/__pycache__/constants.cpython-311.pyc
--rw-r--r--   0        0        0     3106 2024-06-02 02:24:45.185374 agiflow_sdk-0.0.3/agiflow/opentelemetry/convention/__pycache__/database_span_attributes.cpython-311.pyc
--rw-r--r--   0        0        0     1665 2024-06-02 02:24:45.185630 agiflow_sdk-0.0.3/agiflow/opentelemetry/convention/__pycache__/framework_span_attributes.cpython-311.pyc
--rw-r--r--   0        0        0     7042 2024-06-02 02:24:45.185924 agiflow_sdk-0.0.3/agiflow/opentelemetry/convention/__pycache__/llm_span_attributes.cpython-311.pyc
--rw-r--r--   0        0        0     2477 2024-06-02 02:24:45.186179 agiflow_sdk-0.0.3/agiflow/opentelemetry/convention/agiflow_attributes.py
--rw-r--r--   0        0        0     3893 2024-06-02 02:24:45.186406 agiflow_sdk-0.0.3/agiflow/opentelemetry/convention/constants.py
--rw-r--r--   0        0        0     2279 2024-06-02 02:24:45.186640 agiflow_sdk-0.0.3/agiflow/opentelemetry/convention/database_span_attributes.py
--rw-r--r--   0        0        0      875 2024-06-02 02:24:45.186857 agiflow_sdk-0.0.3/agiflow/opentelemetry/convention/framework_span_attributes.py
--rw-r--r--   0        0        0     6050 2024-06-02 02:24:45.187048 agiflow_sdk-0.0.3/agiflow/opentelemetry/convention/llm_span_attributes.py
--rw-r--r--   0        0        0    10305 2024-06-02 02:24:45.187394 agiflow_sdk-0.0.3/agiflow/opentelemetry/instrumentation/__init__.py
--rw-r--r--   0        0        0    13104 2024-06-02 02:24:45.187698 agiflow_sdk-0.0.3/agiflow/opentelemetry/instrumentation/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0      154 2024-06-02 02:24:45.188077 agiflow_sdk-0.0.3/agiflow/opentelemetry/instrumentation/anthropic/__init__.py
--rw-r--r--   0        0        0      398 2024-06-02 02:24:45.188291 agiflow_sdk-0.0.3/agiflow/opentelemetry/instrumentation/anthropic/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0     2946 2024-06-02 02:24:45.188421 agiflow_sdk-0.0.3/agiflow/opentelemetry/instrumentation/anthropic/__pycache__/instrumentation.cpython-311.pyc
--rw-r--r--   0        0        0      158 2024-06-02 02:24:45.188726 agiflow_sdk-0.0.3/agiflow/opentelemetry/instrumentation/anthropic/hooks/__init__.py
--rw-r--r--   0        0        0      409 2024-06-02 02:24:45.188941 agiflow_sdk-0.0.3/agiflow/opentelemetry/instrumentation/anthropic/hooks/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0     2606 2024-06-02 02:24:45.189178 agiflow_sdk-0.0.3/agiflow/opentelemetry/instrumentation/anthropic/hooks/__pycache__/base.cpython-311.pyc
--rw-r--r--   0        0        0     9937 2024-06-02 02:24:45.189374 agiflow_sdk-0.0.3/agiflow/opentelemetry/instrumentation/anthropic/hooks/__pycache__/message_create.cpython-311.pyc
--rw-r--r--   0        0        0     1581 2024-06-02 02:24:45.189679 agiflow_sdk-0.0.3/agiflow/opentelemetry/instrumentation/anthropic/hooks/base.py
--rw-r--r--   0        0        0     7481 2024-06-02 02:24:45.189915 agiflow_sdk-0.0.3/agiflow/opentelemetry/instrumentation/anthropic/hooks/message_create.py
--rw-r--r--   0        0        0     1730 2024-06-02 02:24:45.190162 agiflow_sdk-0.0.3/agiflow/opentelemetry/instrumentation/anthropic/instrumentation.py
--rw-r--r--   0        0        0      145 2024-06-02 02:24:45.190471 agiflow_sdk-0.0.3/agiflow/opentelemetry/instrumentation/chroma/__init__.py
--rw-r--r--   0        0        0      389 2024-06-02 02:24:45.190767 agiflow_sdk-0.0.3/agiflow/opentelemetry/instrumentation/chroma/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0     3196 2024-06-02 02:24:45.191004 agiflow_sdk-0.0.3/agiflow/opentelemetry/instrumentation/chroma/__pycache__/instrumentation.cpython-311.pyc
--rw-r--r--   0        0        0      157 2024-06-02 02:24:45.191313 agiflow_sdk-0.0.3/agiflow/opentelemetry/instrumentation/chroma/hooks/__init__.py
--rw-r--r--   0        0        0      405 2024-06-02 02:24:45.191523 agiflow_sdk-0.0.3/agiflow/opentelemetry/instrumentation/chroma/hooks/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0     2297 2024-06-02 02:24:45.191673 agiflow_sdk-0.0.3/agiflow/opentelemetry/instrumentation/chroma/hooks/__pycache__/base.cpython-311.pyc
--rw-r--r--   0        0        0    16999 2024-06-02 02:24:45.191847 agiflow_sdk-0.0.3/agiflow/opentelemetry/instrumentation/chroma/hooks/__pycache__/collection_call.cpython-311.pyc
--rw-r--r--   0        0        0     1385 2024-06-02 02:24:45.192093 agiflow_sdk-0.0.3/agiflow/opentelemetry/instrumentation/chroma/hooks/base.py
--rw-r--r--   0        0        0    10704 2024-06-02 02:24:45.192326 agiflow_sdk-0.0.3/agiflow/opentelemetry/instrumentation/chroma/hooks/collection_call.py
--rw-r--r--   0        0        0     1910 2024-06-02 02:24:45.192645 agiflow_sdk-0.0.3/agiflow/opentelemetry/instrumentation/chroma/instrumentation.py
--rw-r--r--   0        0        0      145 2024-06-02 02:24:45.192945 agiflow_sdk-0.0.3/agiflow/opentelemetry/instrumentation/cohere/__init__.py
--rw-r--r--   0        0        0      389 2024-06-02 02:24:45.193150 agiflow_sdk-0.0.3/agiflow/opentelemetry/instrumentation/cohere/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0     3487 2024-06-02 02:24:45.193289 agiflow_sdk-0.0.3/agiflow/opentelemetry/instrumentation/cohere/__pycache__/instrumentation.cpython-311.pyc
--rw-r--r--   0        0        0      511 2024-06-02 02:24:45.193664 agiflow_sdk-0.0.3/agiflow/opentelemetry/instrumentation/cohere/hooks/__init__.py
--rw-r--r--   0        0        0      809 2024-06-02 02:24:45.193885 agiflow_sdk-0.0.3/agiflow/opentelemetry/instrumentation/cohere/hooks/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0     2247 2024-06-02 02:24:45.194026 agiflow_sdk-0.0.3/agiflow/opentelemetry/instrumentation/cohere/hooks/__pycache__/base.cpython-311.pyc
--rw-r--r--   0        0        0     8362 2024-06-02 02:24:45.194263 agiflow_sdk-0.0.3/agiflow/opentelemetry/instrumentation/cohere/hooks/__pycache__/base_chat.cpython-311.pyc
--rw-r--r--   0        0        0     6177 2024-06-02 02:24:45.194475 agiflow_sdk-0.0.3/agiflow/opentelemetry/instrumentation/cohere/hooks/__pycache__/chat_create.cpython-311.pyc
--rw-r--r--   0        0        0     7073 2024-06-02 02:24:45.194688 agiflow_sdk-0.0.3/agiflow/opentelemetry/instrumentation/cohere/hooks/__pycache__/chat_stream.cpython-311.pyc
--rw-r--r--   0        0        0     5336 2024-06-02 02:24:45.194819 agiflow_sdk-0.0.3/agiflow/opentelemetry/instrumentation/cohere/hooks/__pycache__/embed.cpython-311.pyc
--rw-r--r--   0        0        0     5930 2024-06-02 02:24:45.194958 agiflow_sdk-0.0.3/agiflow/opentelemetry/instrumentation/cohere/hooks/__pycache__/rerank.cpython-311.pyc
--rw-r--r--   0        0        0     1328 2024-06-02 02:24:45.195180 agiflow_sdk-0.0.3/agiflow/opentelemetry/instrumentation/cohere/hooks/base.py
--rw-r--r--   0        0        0     5765 2024-06-02 02:24:45.195426 agiflow_sdk-0.0.3/agiflow/opentelemetry/instrumentation/cohere/hooks/base_chat.py
--rw-r--r--   0        0        0     4975 2024-06-02 02:24:45.195653 agiflow_sdk-0.0.3/agiflow/opentelemetry/instrumentation/cohere/hooks/chat_create.py
--rw-r--r--   0        0        0     7065 2024-06-02 02:24:45.195877 agiflow_sdk-0.0.3/agiflow/opentelemetry/instrumentation/cohere/hooks/chat_stream.py
--rw-r--r--   0        0        0     3919 2024-06-02 02:24:45.196098 agiflow_sdk-0.0.3/agiflow/opentelemetry/instrumentation/cohere/hooks/embed.py
--rw-r--r--   0        0        0     4364 2024-06-02 02:24:45.196324 agiflow_sdk-0.0.3/agiflow/opentelemetry/instrumentation/cohere/hooks/rerank.py
--rw-r--r--   0        0        0     2425 2024-06-02 02:24:45.196558 agiflow_sdk-0.0.3/agiflow/opentelemetry/instrumentation/cohere/instrumentation.py
--rw-r--r--   0        0        0      391 2024-06-02 02:24:45.196851 agiflow_sdk-0.0.3/agiflow/opentelemetry/instrumentation/constants/__init__.py
--rw-r--r--   0        0        0      649 2024-06-02 02:24:45.197064 agiflow_sdk-0.0.3/agiflow/opentelemetry/instrumentation/constants/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0      346 2024-06-02 02:24:45.197300 agiflow_sdk-0.0.3/agiflow/opentelemetry/instrumentation/constants/__pycache__/anthropic.cpython-311.pyc
--rw-r--r--   0        0        0     1014 2024-06-02 02:24:45.197436 agiflow_sdk-0.0.3/agiflow/opentelemetry/instrumentation/constants/__pycache__/chroma.cpython-311.pyc
--rw-r--r--   0        0        0      595 2024-06-02 02:24:45.197572 agiflow_sdk-0.0.3/agiflow/opentelemetry/instrumentation/constants/__pycache__/cohere.cpython-311.pyc
--rw-r--r--   0        0        0      902 2024-06-02 02:24:45.197820 agiflow_sdk-0.0.3/agiflow/opentelemetry/instrumentation/constants/__pycache__/common.cpython-311.pyc
--rw-r--r--   0        0        0     1074 2024-06-02 02:24:45.198055 agiflow_sdk-0.0.3/agiflow/opentelemetry/instrumentation/constants/__pycache__/openai.cpython-311.pyc
--rw-r--r--   0        0        0      126 2024-06-02 02:24:45.198291 agiflow_sdk-0.0.3/agiflow/opentelemetry/instrumentation/constants/anthropic.py
--rw-r--r--   0        0        0      972 2024-06-02 02:24:45.198543 agiflow_sdk-0.0.3/agiflow/opentelemetry/instrumentation/constants/chroma.py
--rw-r--r--   0        0        0      577 2024-06-02 02:24:45.198766 agiflow_sdk-0.0.3/agiflow/opentelemetry/instrumentation/constants/cohere.py
--rw-r--r--   0        0        0      750 2024-06-02 02:24:45.198931 agiflow_sdk-0.0.3/agiflow/opentelemetry/instrumentation/constants/common.py
--rw-r--r--   0        0        0      134 2024-06-02 02:24:45.199148 agiflow_sdk-0.0.3/agiflow/opentelemetry/instrumentation/constants/groq.py
--rw-r--r--   0        0        0     1054 2024-06-02 02:24:45.199366 agiflow_sdk-0.0.3/agiflow/opentelemetry/instrumentation/constants/openai.py
--rw-r--r--   0        0        0      490 2024-06-02 02:24:45.199585 agiflow_sdk-0.0.3/agiflow/opentelemetry/instrumentation/constants/pinecone.py
--rw-r--r--   0        0        0     2016 2024-06-02 02:24:45.199833 agiflow_sdk-0.0.3/agiflow/opentelemetry/instrumentation/constants/qdrant.py
--rw-r--r--   0        0        0     1518 2024-06-02 02:24:45.200069 agiflow_sdk-0.0.3/agiflow/opentelemetry/instrumentation/constants/weaviate.py
--rw-r--r--   0        0        0      139 2024-06-02 02:24:45.200388 agiflow_sdk-0.0.3/agiflow/opentelemetry/instrumentation/groq/__init__.py
--rw-r--r--   0        0        0      156 2024-06-02 02:24:45.200707 agiflow_sdk-0.0.3/agiflow/opentelemetry/instrumentation/groq/hooks/__init__.py
--rw-r--r--   0        0        0     1934 2024-06-02 02:24:45.200941 agiflow_sdk-0.0.3/agiflow/opentelemetry/instrumentation/groq/hooks/base.py
--rw-r--r--   0        0        0    12481 2024-06-02 02:24:45.201219 agiflow_sdk-0.0.3/agiflow/opentelemetry/instrumentation/groq/hooks/chat_completion.py
--rw-r--r--   0        0        0     1993 2024-06-02 02:24:45.201499 agiflow_sdk-0.0.3/agiflow/opentelemetry/instrumentation/groq/instrumentation.py
--rw-r--r--   0        0        0     6148 2024-06-02 02:24:45.201810 agiflow_sdk-0.0.3/agiflow/opentelemetry/instrumentation/langchain/.DS_Store
--rw-r--r--   0        0        0      154 2024-06-02 02:24:45.202026 agiflow_sdk-0.0.3/agiflow/opentelemetry/instrumentation/langchain/__init__.py
--rw-r--r--   0        0        0      398 2024-06-02 02:24:45.202308 agiflow_sdk-0.0.3/agiflow/opentelemetry/instrumentation/langchain/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0     3233 2024-06-02 02:24:45.202521 agiflow_sdk-0.0.3/agiflow/opentelemetry/instrumentation/langchain/__pycache__/instrumentation.cpython-311.pyc
--rw-r--r--   0        0        0     4136 2024-06-02 02:24:45.202756 agiflow_sdk-0.0.3/agiflow/opentelemetry/instrumentation/langchain/__pycache__/patch.cpython-311.pyc
--rw-r--r--   0        0        0      252 2024-06-02 02:24:45.203071 agiflow_sdk-0.0.3/agiflow/opentelemetry/instrumentation/langchain/hooks/__init__.py
--rw-r--r--   0        0        0      532 2024-06-02 02:24:45.203366 agiflow_sdk-0.0.3/agiflow/opentelemetry/instrumentation/langchain/hooks/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0     2313 2024-06-02 02:24:45.203583 agiflow_sdk-0.0.3/agiflow/opentelemetry/instrumentation/langchain/hooks/__pycache__/base.cpython-311.pyc
--rw-r--r--   0        0        0     7286 2024-06-02 02:24:45.203799 agiflow_sdk-0.0.3/agiflow/opentelemetry/instrumentation/langchain/hooks/__pycache__/chat.cpython-311.pyc
--rw-r--r--   0        0        0     3122 2024-06-02 02:24:45.204033 agiflow_sdk-0.0.3/agiflow/opentelemetry/instrumentation/langchain/hooks/__pycache__/generic.cpython-311.pyc
--rw-r--r--   0        0        0     1384 2024-06-02 02:24:45.204253 agiflow_sdk-0.0.3/agiflow/opentelemetry/instrumentation/langchain/hooks/base.py
--rw-r--r--   0        0        0     5021 2024-06-02 02:24:45.204488 agiflow_sdk-0.0.3/agiflow/opentelemetry/instrumentation/langchain/hooks/chat.py
--rw-r--r--   0        0        0     1741 2024-06-02 02:24:45.204708 agiflow_sdk-0.0.3/agiflow/opentelemetry/instrumentation/langchain/hooks/generic.py
--rw-r--r--   0        0        0     2232 2024-06-02 02:24:45.204940 agiflow_sdk-0.0.3/agiflow/opentelemetry/instrumentation/langchain/instrumentation.py
--rw-r--r--   0        0        0     6148 2024-06-02 02:24:45.205242 agiflow_sdk-0.0.3/agiflow/opentelemetry/instrumentation/langchain_community/.DS_Store
--rw-r--r--   0        0        0      182 2024-06-02 02:24:45.205448 agiflow_sdk-0.0.3/agiflow/opentelemetry/instrumentation/langchain_community/__init__.py
--rw-r--r--   0        0        0      427 2024-06-02 02:24:45.205740 agiflow_sdk-0.0.3/agiflow/opentelemetry/instrumentation/langchain_community/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0     3462 2024-06-02 02:24:45.205974 agiflow_sdk-0.0.3/agiflow/opentelemetry/instrumentation/langchain_community/__pycache__/instrumentation.cpython-311.pyc
--rw-r--r--   0        0        0    11425 2024-06-02 02:24:45.206220 agiflow_sdk-0.0.3/agiflow/opentelemetry/instrumentation/langchain_community/__pycache__/patch.cpython-311.pyc
--rw-r--r--   0        0        0     6148 2024-06-02 02:24:45.206631 agiflow_sdk-0.0.3/agiflow/opentelemetry/instrumentation/langchain_community/hooks/.DS_Store
--rw-r--r--   0        0        0      141 2024-06-02 02:24:45.206854 agiflow_sdk-0.0.3/agiflow/opentelemetry/instrumentation/langchain_community/hooks/__init__.py
--rw-r--r--   0        0        0      404 2024-06-02 02:24:45.207102 agiflow_sdk-0.0.3/agiflow/opentelemetry/instrumentation/langchain_community/hooks/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0     2481 2024-06-02 02:24:45.207324 agiflow_sdk-0.0.3/agiflow/opentelemetry/instrumentation/langchain_community/hooks/__pycache__/base.cpython-311.pyc
--rw-r--r--   0        0        0     6863 2024-06-02 02:24:45.207545 agiflow_sdk-0.0.3/agiflow/opentelemetry/instrumentation/langchain_community/hooks/__pycache__/chat.cpython-311.pyc
--rw-r--r--   0        0        0     3163 2024-06-02 02:24:45.207723 agiflow_sdk-0.0.3/agiflow/opentelemetry/instrumentation/langchain_community/hooks/__pycache__/generic.cpython-311.pyc
--rw-r--r--   0        0        0     5119 2024-06-02 02:24:45.207943 agiflow_sdk-0.0.3/agiflow/opentelemetry/instrumentation/langchain_community/hooks/__pycache__/llm.cpython-311.pyc
--rw-r--r--   0        0        0     1499 2024-06-02 02:24:45.208164 agiflow_sdk-0.0.3/agiflow/opentelemetry/instrumentation/langchain_community/hooks/base.py
--rw-r--r--   0        0        0     1769 2024-06-02 02:24:45.208348 agiflow_sdk-0.0.3/agiflow/opentelemetry/instrumentation/langchain_community/hooks/generic.py
--rw-r--r--   0        0        0     3005 2024-06-02 02:24:45.208575 agiflow_sdk-0.0.3/agiflow/opentelemetry/instrumentation/langchain_community/instrumentation.py
--rw-r--r--   0        0        0     6148 2024-06-02 02:24:45.208867 agiflow_sdk-0.0.3/agiflow/opentelemetry/instrumentation/langchain_core/.DS_Store
--rw-r--r--   0        0        0      167 2024-06-02 02:24:45.209076 agiflow_sdk-0.0.3/agiflow/opentelemetry/instrumentation/langchain_core/__init__.py
--rw-r--r--   0        0        0      412 2024-06-02 02:24:45.209362 agiflow_sdk-0.0.3/agiflow/opentelemetry/instrumentation/langchain_core/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0     3928 2024-06-02 02:24:45.209532 agiflow_sdk-0.0.3/agiflow/opentelemetry/instrumentation/langchain_core/__pycache__/instrumentation.cpython-311.pyc
--rw-r--r--   0        0        0     8316 2024-06-02 02:24:45.209754 agiflow_sdk-0.0.3/agiflow/opentelemetry/instrumentation/langchain_core/__pycache__/patch.cpython-311.pyc
--rw-r--r--   0        0        0      390 2024-06-02 02:24:45.210145 agiflow_sdk-0.0.3/agiflow/opentelemetry/instrumentation/langchain_core/hooks/__init__.py
--rw-r--r--   0        0        0      693 2024-06-02 02:24:45.210447 agiflow_sdk-0.0.3/agiflow/opentelemetry/instrumentation/langchain_core/hooks/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0     2558 2024-06-02 02:24:45.210621 agiflow_sdk-0.0.3/agiflow/opentelemetry/instrumentation/langchain_core/hooks/__pycache__/base.cpython-311.pyc
--rw-r--r--   0        0        0     3573 2024-06-02 02:24:45.210855 agiflow_sdk-0.0.3/agiflow/opentelemetry/instrumentation/langchain_core/hooks/__pycache__/generic.cpython-311.pyc
--rw-r--r--   0        0        0     5208 2024-06-02 02:24:45.211082 agiflow_sdk-0.0.3/agiflow/opentelemetry/instrumentation/langchain_core/hooks/__pycache__/llm.cpython-311.pyc
--rw-r--r--   0        0        0     4692 2024-06-02 02:24:45.211311 agiflow_sdk-0.0.3/agiflow/opentelemetry/instrumentation/langchain_core/hooks/__pycache__/runnable.cpython-311.pyc
--rw-r--r--   0        0        0     1533 2024-06-02 02:24:45.211547 agiflow_sdk-0.0.3/agiflow/opentelemetry/instrumentation/langchain_core/hooks/base.py
--rw-r--r--   0        0        0     2152 2024-06-02 02:24:45.211778 agiflow_sdk-0.0.3/agiflow/opentelemetry/instrumentation/langchain_core/hooks/generic.py
--rw-r--r--   0        0        0     3178 2024-06-02 02:24:45.212000 agiflow_sdk-0.0.3/agiflow/opentelemetry/instrumentation/langchain_core/hooks/llm.py
--rw-r--r--   0        0        0     3248 2024-06-02 02:24:45.212220 agiflow_sdk-0.0.3/agiflow/opentelemetry/instrumentation/langchain_core/hooks/runnable.py
--rw-r--r--   0        0        0     3346 2024-06-02 02:24:45.212446 agiflow_sdk-0.0.3/agiflow/opentelemetry/instrumentation/langchain_core/instrumentation.py
--rw-r--r--   0        0        0      154 2024-06-02 02:24:45.212730 agiflow_sdk-0.0.3/agiflow/opentelemetry/instrumentation/langgraph/__init__.py
--rw-r--r--   0        0        0      146 2024-06-02 02:24:45.213004 agiflow_sdk-0.0.3/agiflow/opentelemetry/instrumentation/langgraph/hooks/__init__.py
--rw-r--r--   0        0        0     1343 2024-06-02 02:24:45.213226 agiflow_sdk-0.0.3/agiflow/opentelemetry/instrumentation/langgraph/hooks/base.py
--rw-r--r--   0        0        0     3352 2024-06-02 02:24:45.213449 agiflow_sdk-0.0.3/agiflow/opentelemetry/instrumentation/langgraph/hooks/graph_call.py
--rw-r--r--   0        0        0     2873 2024-06-02 02:24:45.213680 agiflow_sdk-0.0.3/agiflow/opentelemetry/instrumentation/langgraph/instrumentation.py
--rw-r--r--   0        0        0      157 2024-06-02 02:24:45.213973 agiflow_sdk-0.0.3/agiflow/opentelemetry/instrumentation/llamaindex/__init__.py
--rw-r--r--   0        0        0      140 2024-06-02 02:24:45.214172 agiflow_sdk-0.0.3/agiflow/opentelemetry/instrumentation/llamaindex/hooks/__init__.py
--rw-r--r--   0        0        0     1347 2024-06-02 02:24:45.214392 agiflow_sdk-0.0.3/agiflow/opentelemetry/instrumentation/llamaindex/hooks/base.py
--rw-r--r--   0        0        0     1718 2024-06-02 02:24:45.214719 agiflow_sdk-0.0.3/agiflow/opentelemetry/instrumentation/llamaindex/hooks/generic.py
--rw-r--r--   0        0        0     2944 2024-06-02 02:24:45.214962 agiflow_sdk-0.0.3/agiflow/opentelemetry/instrumentation/llamaindex/instrumentation.py
--rw-r--r--   0        0        0     6148 2024-06-02 02:24:45.215250 agiflow_sdk-0.0.3/agiflow/opentelemetry/instrumentation/openai/.DS_Store
--rw-r--r--   0        0        0      145 2024-06-02 02:24:45.215475 agiflow_sdk-0.0.3/agiflow/opentelemetry/instrumentation/openai/__init__.py
--rw-r--r--   0        0        0      389 2024-06-02 02:24:45.215762 agiflow_sdk-0.0.3/agiflow/opentelemetry/instrumentation/openai/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0     3659 2024-06-02 02:24:45.215985 agiflow_sdk-0.0.3/agiflow/opentelemetry/instrumentation/openai/__pycache__/instrumentation.cpython-311.pyc
--rw-r--r--   0        0        0    20526 2024-06-02 02:24:45.216324 agiflow_sdk-0.0.3/agiflow/opentelemetry/instrumentation/openai/__pycache__/patch.cpython-311.pyc
--rw-r--r--   0        0        0     6148 2024-06-02 02:24:45.216648 agiflow_sdk-0.0.3/agiflow/opentelemetry/instrumentation/openai/hooks/.DS_Store
--rw-r--r--   0        0        0      424 2024-06-02 02:24:45.216858 agiflow_sdk-0.0.3/agiflow/opentelemetry/instrumentation/openai/hooks/__init__.py
--rw-r--r--   0        0        0      699 2024-06-02 02:24:45.217090 agiflow_sdk-0.0.3/agiflow/opentelemetry/instrumentation/openai/hooks/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0     4035 2024-06-02 02:24:45.217297 agiflow_sdk-0.0.3/agiflow/opentelemetry/instrumentation/openai/hooks/__pycache__/base.cpython-311.pyc
--rw-r--r--   0        0        0     4744 2024-06-02 02:24:45.217526 agiflow_sdk-0.0.3/agiflow/opentelemetry/instrumentation/openai/hooks/__pycache__/base_llm.cpython-311.pyc
--rw-r--r--   0        0        0    12171 2024-06-02 02:24:45.217777 agiflow_sdk-0.0.3/agiflow/opentelemetry/instrumentation/openai/hooks/__pycache__/chat_completion.cpython-311.pyc
--rw-r--r--   0        0        0    11736 2024-06-02 02:24:45.218089 agiflow_sdk-0.0.3/agiflow/opentelemetry/instrumentation/openai/hooks/__pycache__/completion.cpython-311.pyc
--rw-r--r--   0        0        0     3391 2024-06-02 02:24:45.218334 agiflow_sdk-0.0.3/agiflow/opentelemetry/instrumentation/openai/hooks/__pycache__/embedding.cpython-311.pyc
--rw-r--r--   0        0        0     3885 2024-06-02 02:24:45.218498 agiflow_sdk-0.0.3/agiflow/opentelemetry/instrumentation/openai/hooks/__pycache__/image_generate.cpython-311.pyc
--rw-r--r--   0        0        0     2374 2024-06-02 02:24:45.218685 agiflow_sdk-0.0.3/agiflow/opentelemetry/instrumentation/openai/hooks/__pycache__/utils.cpython-311.pyc
--rw-r--r--   0        0        0     2474 2024-06-02 02:24:45.218904 agiflow_sdk-0.0.3/agiflow/opentelemetry/instrumentation/openai/hooks/base.py
--rw-r--r--   0        0        0     3115 2024-06-02 02:24:45.219079 agiflow_sdk-0.0.3/agiflow/opentelemetry/instrumentation/openai/hooks/base_llm.py
--rw-r--r--   0        0        0    10648 2024-06-02 02:24:45.219381 agiflow_sdk-0.0.3/agiflow/opentelemetry/instrumentation/openai/hooks/chat_completion.py
--rw-r--r--   0        0        0     2257 2024-06-02 02:24:45.219729 agiflow_sdk-0.0.3/agiflow/opentelemetry/instrumentation/openai/hooks/embedding.py
--rw-r--r--   0        0        0     2555 2024-06-02 02:24:45.219988 agiflow_sdk-0.0.3/agiflow/opentelemetry/instrumentation/openai/hooks/image_generate.py
--rw-r--r--   0        0        0     2211 2024-06-02 02:24:45.220201 agiflow_sdk-0.0.3/agiflow/opentelemetry/instrumentation/openai/hooks/utils.py
--rw-r--r--   0        0        0     2910 2024-06-02 02:24:45.220519 agiflow_sdk-0.0.3/agiflow/opentelemetry/instrumentation/openai/instrumentation.py
--rw-r--r--   0        0        0      151 2024-06-02 02:24:45.220974 agiflow_sdk-0.0.3/agiflow/opentelemetry/instrumentation/pinecone/__init__.py
--rw-r--r--   0        0        0      137 2024-06-02 02:24:45.221301 agiflow_sdk-0.0.3/agiflow/opentelemetry/instrumentation/pinecone/hooks/__init__.py
--rw-r--r--   0        0        0     1396 2024-06-02 02:24:45.221529 agiflow_sdk-0.0.3/agiflow/opentelemetry/instrumentation/pinecone/hooks/base.py
--rw-r--r--   0        0        0     6892 2024-06-02 02:24:45.221810 agiflow_sdk-0.0.3/agiflow/opentelemetry/instrumentation/pinecone/hooks/generic.py
--rw-r--r--   0        0        0     2019 2024-06-02 02:24:45.222069 agiflow_sdk-0.0.3/agiflow/opentelemetry/instrumentation/pinecone/instrumentation.py
--rw-r--r--   0        0        0      145 2024-06-02 02:24:45.222389 agiflow_sdk-0.0.3/agiflow/opentelemetry/instrumentation/qdrant/__init__.py
--rw-r--r--   0        0        0      152 2024-06-02 02:24:45.222691 agiflow_sdk-0.0.3/agiflow/opentelemetry/instrumentation/qdrant/hooks/__init__.py
--rw-r--r--   0        0        0     1388 2024-06-02 02:24:45.222972 agiflow_sdk-0.0.3/agiflow/opentelemetry/instrumentation/qdrant/hooks/base.py
--rw-r--r--   0        0        0     3113 2024-06-02 02:24:45.223188 agiflow_sdk-0.0.3/agiflow/opentelemetry/instrumentation/qdrant/hooks/collection.py
--rw-r--r--   0        0        0     1913 2024-06-02 02:24:45.223402 agiflow_sdk-0.0.3/agiflow/opentelemetry/instrumentation/qdrant/instrumentation.py
--rw-r--r--   0        0        0     2309 2024-06-02 02:24:45.223723 agiflow_sdk-0.0.3/agiflow/opentelemetry/instrumentation/utils/__init__.py
--rw-r--r--   0        0        0     2790 2024-06-02 02:24:45.224020 agiflow_sdk-0.0.3/agiflow/opentelemetry/instrumentation/utils/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0    17396 2024-06-02 02:24:45.224369 agiflow_sdk-0.0.3/agiflow/opentelemetry/instrumentation/utils/__pycache__/wrapper.cpython-311.pyc
--rw-r--r--   0        0        0    11559 2024-06-02 02:24:45.224654 agiflow_sdk-0.0.3/agiflow/opentelemetry/instrumentation/utils/wrapper.py
--rw-r--r--   0        0        0      151 2024-06-02 02:24:45.225213 agiflow_sdk-0.0.3/agiflow/opentelemetry/instrumentation/weaviate/__init__.py
--rw-r--r--   0        0        0      306 2024-06-02 02:24:45.225573 agiflow_sdk-0.0.3/agiflow/opentelemetry/instrumentation/weaviate/hooks/__init__.py
--rw-r--r--   0        0        0     1396 2024-06-02 02:24:45.225826 agiflow_sdk-0.0.3/agiflow/opentelemetry/instrumentation/weaviate/hooks/base.py
--rw-r--r--   0        0        0     1776 2024-06-02 02:24:45.226061 agiflow_sdk-0.0.3/agiflow/opentelemetry/instrumentation/weaviate/hooks/generic_collection.py
--rw-r--r--   0        0        0     4091 2024-06-02 02:24:45.226343 agiflow_sdk-0.0.3/agiflow/opentelemetry/instrumentation/weaviate/hooks/generic_query.py
--rw-r--r--   0        0        0     2754 2024-06-02 02:24:45.226607 agiflow_sdk-0.0.3/agiflow/opentelemetry/instrumentation/weaviate/instrumentation.py
--rw-r--r--   0        0        0      144 2024-06-02 02:24:45.227121 agiflow_sdk-0.0.3/agiflow/opentelemetry/span_processors/__init__.py
--rw-r--r--   0        0        0      376 2024-06-02 02:24:45.227476 agiflow_sdk-0.0.3/agiflow/opentelemetry/span_processors/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0     4786 2024-06-02 02:24:45.227744 agiflow_sdk-0.0.3/agiflow/opentelemetry/span_processors/__pycache__/thread_pool_span_processor.cpython-311.pyc
--rw-r--r--   0        0        0     2347 2024-06-02 02:24:45.227998 agiflow_sdk-0.0.3/agiflow/opentelemetry/span_processors/thread_pool_span_processor.py
--rw-r--r--   0        0        0      644 2024-06-02 02:24:45.228330 agiflow_sdk-0.0.3/agiflow/opentelemetry/trace_decorators/__init__.py
--rw-r--r--   0        0        0      910 2024-06-02 02:24:45.228696 agiflow_sdk-0.0.3/agiflow/opentelemetry/trace_decorators/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0     1831 2024-06-02 02:24:45.228938 agiflow_sdk-0.0.3/agiflow/opentelemetry/trace_decorators/__pycache__/helper.cpython-311.pyc
--rw-r--r--   0        0        0     4548 2024-06-02 02:24:45.229175 agiflow_sdk-0.0.3/agiflow/opentelemetry/trace_decorators/__pycache__/task.cpython-311.pyc
--rw-r--r--   0        0        0     3260 2024-06-02 02:24:45.229393 agiflow_sdk-0.0.3/agiflow/opentelemetry/trace_decorators/__pycache__/workflow.cpython-311.pyc
--rw-r--r--   0        0        0    18659 2024-06-02 02:24:45.229722 agiflow_sdk-0.0.3/agiflow/opentelemetry/trace_decorators/__pycache__/wrapper.cpython-311.pyc
--rw-r--r--   0        0        0     1657 2024-06-02 02:24:45.229960 agiflow_sdk-0.0.3/agiflow/opentelemetry/trace_decorators/helper.py
--rw-r--r--   0        0        0     3514 2024-06-02 02:24:45.230178 agiflow_sdk-0.0.3/agiflow/opentelemetry/trace_decorators/task.py
--rw-r--r--   0        0        0     2174 2024-06-02 02:24:45.230377 agiflow_sdk-0.0.3/agiflow/opentelemetry/trace_decorators/workflow.py
--rw-r--r--   0        0        0    14099 2024-06-02 02:24:45.230649 agiflow_sdk-0.0.3/agiflow/opentelemetry/trace_decorators/wrapper.py
--rw-r--r--   0        0        0      115 2024-06-02 02:24:45.231275 agiflow_sdk-0.0.3/agiflow/opentelemetry/trace_exporter/__init__.py
--rw-r--r--   0        0        0      349 2024-06-02 02:24:45.231623 agiflow_sdk-0.0.3/agiflow/opentelemetry/trace_exporter/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0     2687 2024-06-02 02:24:45.231898 agiflow_sdk-0.0.3/agiflow/opentelemetry/trace_exporter/__pycache__/config.cpython-311.pyc
--rw-r--r--   0        0        0     9661 2024-06-02 02:24:45.232184 agiflow_sdk-0.0.3/agiflow/opentelemetry/trace_exporter/__pycache__/json.cpython-311.pyc
--rw-r--r--   0        0        0      238 2024-06-02 02:24:45.232429 agiflow_sdk-0.0.3/agiflow/opentelemetry/trace_exporter/__pycache__/version.cpython-311.pyc
--rw-r--r--   0        0        0     2757 2024-06-02 02:24:45.232711 agiflow_sdk-0.0.3/agiflow/opentelemetry/trace_exporter/config.py
--rw-r--r--   0        0        0     7123 2024-06-02 02:24:45.232979 agiflow_sdk-0.0.3/agiflow/opentelemetry/trace_exporter/json.py
--rw-r--r--   0        0        0       22 2024-06-02 02:24:45.233143 agiflow_sdk-0.0.3/agiflow/opentelemetry/trace_exporter/version.py
--rw-r--r--   0        0        0       99 2024-06-02 02:24:45.233497 agiflow_sdk-0.0.3/agiflow/opentelemetry/trace_sampler/__init__.py
--rw-r--r--   0        0        0      342 2024-06-02 02:24:45.233851 agiflow_sdk-0.0.3/agiflow/opentelemetry/trace_sampler/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0     1787 2024-06-02 02:24:45.234098 agiflow_sdk-0.0.3/agiflow/opentelemetry/trace_sampler/__pycache__/no_sampler.cpython-311.pyc
--rw-r--r--   0        0        0      862 2024-06-02 02:24:45.234365 agiflow_sdk-0.0.3/agiflow/opentelemetry/trace_sampler/no_sampler.py
--rw-r--r--   0        0        0     3160 2024-06-02 02:24:45.234631 agiflow_sdk-0.0.3/agiflow/opentelemetry/trace_store.py
--rw-r--r--   0        0        0     6148 2024-06-02 02:24:45.234998 agiflow_sdk-0.0.3/agiflow/opentelemetry/tracing/.DS_Store
--rw-r--r--   0        0        0      182 2024-06-02 02:24:45.235165 agiflow_sdk-0.0.3/agiflow/opentelemetry/tracing/__init__.py
--rw-r--r--   0        0        0      437 2024-06-02 02:24:45.235472 agiflow_sdk-0.0.3/agiflow/opentelemetry/tracing/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0     1979 2024-06-02 02:24:45.235723 agiflow_sdk-0.0.3/agiflow/opentelemetry/tracing/__pycache__/content_allow_list.cpython-311.pyc
--rw-r--r--   0        0        0     1978 2024-06-02 02:24:45.235897 agiflow_sdk-0.0.3/agiflow/opentelemetry/tracing/__pycache__/content_alow_list.cpython-311.pyc
--rw-r--r--   0        0        0     5230 2024-06-02 02:24:45.236070 agiflow_sdk-0.0.3/agiflow/opentelemetry/tracing/__pycache__/context.cpython-311.pyc
--rw-r--r--   0        0        0      897 2024-06-02 02:24:45.236233 agiflow_sdk-0.0.3/agiflow/opentelemetry/tracing/__pycache__/context_manager.cpython-311.pyc
--rw-r--r--   0        0        0     1507 2024-06-02 02:24:45.236485 agiflow_sdk-0.0.3/agiflow/opentelemetry/tracing/__pycache__/context_propagation.cpython-311.pyc
--rw-r--r--   0        0        0     2581 2024-06-02 02:24:45.236696 agiflow_sdk-0.0.3/agiflow/opentelemetry/tracing/__pycache__/span_from_context.cpython-311.pyc
--rw-r--r--   0        0        0    10065 2024-06-02 02:24:45.236950 agiflow_sdk-0.0.3/agiflow/opentelemetry/tracing/__pycache__/tracing.cpython-311.pyc
--rw-r--r--   0        0        0      846 2024-06-02 02:24:45.237242 agiflow_sdk-0.0.3/agiflow/opentelemetry/tracing/content_allow_list.py
--rw-r--r--   0        0        0      307 2024-06-02 02:24:45.237394 agiflow_sdk-0.0.3/agiflow/opentelemetry/tracing/context_manager.py
--rw-r--r--   0        0        0     7265 2024-06-02 02:24:45.237615 agiflow_sdk-0.0.3/agiflow/opentelemetry/tracing/tracing.py
--rw-r--r--   0        0        0      813 2024-06-02 02:24:45.237931 agiflow_sdk-0.0.3/agiflow/opentelemetry/types/__init__.py
--rw-r--r--   0        0        0     1865 2024-06-02 02:24:45.238251 agiflow_sdk-0.0.3/agiflow/opentelemetry/types/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0     6148 2024-06-02 02:24:45.238921 agiflow_sdk-0.0.3/agiflow/opentelemetry/utils/.DS_Store
--rw-r--r--   0        0        0      340 2024-06-02 02:24:45.239185 agiflow_sdk-0.0.3/agiflow/opentelemetry/utils/__init__.py
--rw-r--r--   0        0        0      521 2024-06-02 02:24:45.239490 agiflow_sdk-0.0.3/agiflow/opentelemetry/utils/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0     3447 2024-06-02 02:24:45.239717 agiflow_sdk-0.0.3/agiflow/opentelemetry/utils/__pycache__/llm.cpython-311.pyc
--rw-r--r--   0        0        0     2240 2024-06-02 02:24:45.239964 agiflow_sdk-0.0.3/agiflow/opentelemetry/utils/llm.py
--rw-r--r--   0        0        0       71 2024-06-02 02:24:45.240315 agiflow_sdk-0.0.3/agiflow/services/__init__.py
--rw-r--r--   0        0        0      297 2024-06-02 02:24:45.240606 agiflow_sdk-0.0.3/agiflow/services/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0     5452 2024-06-02 02:24:45.240790 agiflow_sdk-0.0.3/agiflow/services/__pycache__/fetch.cpython-311.pyc
--rw-r--r--   0        0        0     2731 2024-06-02 02:24:45.241057 agiflow_sdk-0.0.3/agiflow/services/fetch.py
--rw-r--r--   0        0        0     2522 2024-06-02 02:24:45.241399 agiflow_sdk-0.0.3/agiflow/telemetry/__init__.py
--rw-r--r--   0        0        0     4829 2024-06-02 02:24:45.241613 agiflow_sdk-0.0.3/agiflow/telemetry/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0     6148 2024-06-02 02:24:45.241817 agiflow_sdk-0.0.3/agiflow/utils/.DS_Store
--rw-r--r--   0        0        0      444 2024-06-02 02:24:45.242025 agiflow_sdk-0.0.3/agiflow/utils/__init__.py
--rw-r--r--   0        0        0      728 2024-06-02 02:24:45.242317 agiflow_sdk-0.0.3/agiflow/utils/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0      532 2024-06-02 02:24:45.242558 agiflow_sdk-0.0.3/agiflow/utils/__pycache__/assertion.cpython-311.pyc
--rw-r--r--   0        0        0     1923 2024-06-02 02:24:45.242796 agiflow_sdk-0.0.3/agiflow/utils/__pycache__/debugging.cpython-311.pyc
--rw-r--r--   0        0        0     1719 2024-06-02 02:24:45.243023 agiflow_sdk-0.0.3/agiflow/utils/__pycache__/error.cpython-311.pyc
--rw-r--r--   0        0        0     3268 2024-06-02 02:24:45.243178 agiflow_sdk-0.0.3/agiflow/utils/__pycache__/llm.cpython-311.pyc
--rw-r--r--   0        0        0     4718 2024-06-02 02:24:45.243396 agiflow_sdk-0.0.3/agiflow/utils/__pycache__/string.cpython-311.pyc
--rw-r--r--   0        0        0      583 2024-06-02 02:24:45.243621 agiflow_sdk-0.0.3/agiflow/utils/__pycache__/time.cpython-311.pyc
--rw-r--r--   0        0        0      207 2024-06-02 02:24:45.243871 agiflow_sdk-0.0.3/agiflow/utils/assertion.py
--rw-r--r--   0        0        0      580 2024-06-02 02:24:45.244088 agiflow_sdk-0.0.3/agiflow/utils/debugging.py
--rw-r--r--   0        0        0      847 2024-06-02 02:24:45.244311 agiflow_sdk-0.0.3/agiflow/utils/error.py
--rw-r--r--   0        0        0     1965 2024-06-02 02:24:45.244521 agiflow_sdk-0.0.3/agiflow/utils/string.py
--rw-r--r--   0        0        0      264 2024-06-02 02:24:45.244732 agiflow_sdk-0.0.3/agiflow/utils/time.py
--rw-r--r--   0        0        0       22 2024-06-02 02:24:45.244854 agiflow_sdk-0.0.3/agiflow/version.py
--rw-r--r--   0        0        0     1106 2024-06-02 02:24:45.251875 agiflow_sdk-0.0.3/pyproject.toml
--rw-r--r--   0        0        0     1760 1970-01-01 00:00:00.000000 agiflow_sdk-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0      394 2024-06-03 06:05:41.412058 agiflow_sdk-0.0.4/README.md
+-rw-r--r--   0        0        0       64 2024-06-03 06:05:41.412517 agiflow_sdk-0.0.4/agiflow/__init__.py
+-rw-r--r--   0        0        0     5480 2024-06-03 06:05:41.414321 agiflow_sdk-0.0.4/agiflow/agiflow.py
+-rw-r--r--   0        0        0      889 2024-06-03 06:05:41.414824 agiflow_sdk-0.0.4/agiflow/config/__init__.py
+-rw-r--r--   0        0        0     1838 2024-06-03 06:05:41.415501 agiflow_sdk-0.0.4/agiflow/config/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0      274 2024-06-03 06:05:41.415679 agiflow_sdk-0.0.4/agiflow/config/__pycache__/constants.cpython-311.pyc
+-rw-r--r--   0        0        0     1451 2024-06-03 06:05:41.415979 agiflow_sdk-0.0.4/agiflow/config/__pycache__/environment_vars.cpython-311.pyc
+-rw-r--r--   0        0        0       72 2024-06-03 06:05:41.416167 agiflow_sdk-0.0.4/agiflow/config/constants.py
+-rw-r--r--   0        0        0     1338 2024-06-03 06:05:41.416400 agiflow_sdk-0.0.4/agiflow/config/environment_vars.py
+-rw-r--r--   0        0        0     6148 2024-06-03 06:05:41.416762 agiflow_sdk-0.0.4/agiflow/opentelemetry/.DS_Store
+-rw-r--r--   0        0        0     1037 2024-06-03 06:05:41.417092 agiflow_sdk-0.0.4/agiflow/opentelemetry/__init__.py
+-rw-r--r--   0        0        0     1379 2024-06-03 06:05:41.417890 agiflow_sdk-0.0.4/agiflow/opentelemetry/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0     4092 2024-06-03 06:05:41.418277 agiflow_sdk-0.0.4/agiflow/opentelemetry/__pycache__/trace_store.cpython-311.pyc
+-rw-r--r--   0        0        0      223 2024-06-03 06:05:41.418700 agiflow_sdk-0.0.4/agiflow/opentelemetry/__pycache__/version.cpython-311.pyc
+-rw-r--r--   0        0        0     1218 2024-06-03 06:05:41.419039 agiflow_sdk-0.0.4/agiflow/opentelemetry/context/__init__.py
+-rw-r--r--   0        0        0     1363 2024-06-03 06:05:41.419592 agiflow_sdk-0.0.4/agiflow/opentelemetry/context/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0     1790 2024-06-03 06:05:41.419739 agiflow_sdk-0.0.4/agiflow/opentelemetry/context/__pycache__/constants.cpython-311.pyc
+-rw-r--r--   0        0        0     2868 2024-06-03 06:05:41.420055 agiflow_sdk-0.0.4/agiflow/opentelemetry/context/__pycache__/context.cpython-311.pyc
+-rw-r--r--   0        0        0     3327 2024-06-03 06:05:41.420253 agiflow_sdk-0.0.4/agiflow/opentelemetry/context/__pycache__/context_propagation.cpython-311.pyc
+-rw-r--r--   0        0        0     2105 2024-06-03 06:05:41.420617 agiflow_sdk-0.0.4/agiflow/opentelemetry/context/__pycache__/set_span_from_context.cpython-311.pyc
+-rw-r--r--   0        0        0     2101 2024-06-03 06:05:41.420953 agiflow_sdk-0.0.4/agiflow/opentelemetry/context/__pycache__/span_from_context.cpython-311.pyc
+-rw-r--r--   0        0        0      740 2024-06-03 06:05:41.421160 agiflow_sdk-0.0.4/agiflow/opentelemetry/context/constants.py
+-rw-r--r--   0        0        0     1231 2024-06-03 06:05:41.421419 agiflow_sdk-0.0.4/agiflow/opentelemetry/context/context.py
+-rw-r--r--   0        0        0     2139 2024-06-03 06:05:41.421686 agiflow_sdk-0.0.4/agiflow/opentelemetry/context/context_propagation.py
+-rw-r--r--   0        0        0     1285 2024-06-03 06:05:41.421908 agiflow_sdk-0.0.4/agiflow/opentelemetry/context/span_from_context.py
+-rw-r--r--   0        0        0     1583 2024-06-03 06:05:41.422360 agiflow_sdk-0.0.4/agiflow/opentelemetry/convention/__init__.py
+-rw-r--r--   0        0        0     2184 2024-06-03 06:05:41.422694 agiflow_sdk-0.0.4/agiflow/opentelemetry/convention/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0     2922 2024-06-03 06:05:41.422883 agiflow_sdk-0.0.4/agiflow/opentelemetry/convention/__pycache__/agiflow_attributes.cpython-311.pyc
+-rw-r--r--   0        0        0     7800 2024-06-03 06:05:41.423114 agiflow_sdk-0.0.4/agiflow/opentelemetry/convention/__pycache__/constants.cpython-311.pyc
+-rw-r--r--   0        0        0     3106 2024-06-03 06:05:41.423254 agiflow_sdk-0.0.4/agiflow/opentelemetry/convention/__pycache__/database_span_attributes.cpython-311.pyc
+-rw-r--r--   0        0        0     1665 2024-06-03 06:05:41.423590 agiflow_sdk-0.0.4/agiflow/opentelemetry/convention/__pycache__/framework_span_attributes.cpython-311.pyc
+-rw-r--r--   0        0        0     7042 2024-06-03 06:05:41.423727 agiflow_sdk-0.0.4/agiflow/opentelemetry/convention/__pycache__/llm_span_attributes.cpython-311.pyc
+-rw-r--r--   0        0        0     2477 2024-06-03 06:05:41.423906 agiflow_sdk-0.0.4/agiflow/opentelemetry/convention/agiflow_attributes.py
+-rw-r--r--   0        0        0     3893 2024-06-03 06:05:41.424041 agiflow_sdk-0.0.4/agiflow/opentelemetry/convention/constants.py
+-rw-r--r--   0        0        0     2279 2024-06-03 06:05:41.424175 agiflow_sdk-0.0.4/agiflow/opentelemetry/convention/database_span_attributes.py
+-rw-r--r--   0        0        0      875 2024-06-03 06:05:41.424403 agiflow_sdk-0.0.4/agiflow/opentelemetry/convention/framework_span_attributes.py
+-rw-r--r--   0        0        0     6050 2024-06-03 06:05:41.424653 agiflow_sdk-0.0.4/agiflow/opentelemetry/convention/llm_span_attributes.py
+-rw-r--r--   0        0        0    10305 2024-06-03 06:05:41.424919 agiflow_sdk-0.0.4/agiflow/opentelemetry/instrumentation/__init__.py
+-rw-r--r--   0        0        0    13104 2024-06-03 06:05:41.425367 agiflow_sdk-0.0.4/agiflow/opentelemetry/instrumentation/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0      154 2024-06-03 06:05:41.425742 agiflow_sdk-0.0.4/agiflow/opentelemetry/instrumentation/anthropic/__init__.py
+-rw-r--r--   0        0        0      398 2024-06-03 06:05:41.426523 agiflow_sdk-0.0.4/agiflow/opentelemetry/instrumentation/anthropic/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0     2946 2024-06-03 06:05:41.426662 agiflow_sdk-0.0.4/agiflow/opentelemetry/instrumentation/anthropic/__pycache__/instrumentation.cpython-311.pyc
+-rw-r--r--   0        0        0      158 2024-06-03 06:05:41.426910 agiflow_sdk-0.0.4/agiflow/opentelemetry/instrumentation/anthropic/hooks/__init__.py
+-rw-r--r--   0        0        0      409 2024-06-03 06:05:41.427164 agiflow_sdk-0.0.4/agiflow/opentelemetry/instrumentation/anthropic/hooks/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0     2606 2024-06-03 06:05:41.427307 agiflow_sdk-0.0.4/agiflow/opentelemetry/instrumentation/anthropic/hooks/__pycache__/base.cpython-311.pyc
+-rw-r--r--   0        0        0     9937 2024-06-03 06:05:41.427467 agiflow_sdk-0.0.4/agiflow/opentelemetry/instrumentation/anthropic/hooks/__pycache__/message_create.cpython-311.pyc
+-rw-r--r--   0        0        0     1581 2024-06-03 06:05:41.427720 agiflow_sdk-0.0.4/agiflow/opentelemetry/instrumentation/anthropic/hooks/base.py
+-rw-r--r--   0        0        0     7481 2024-06-03 06:05:41.427945 agiflow_sdk-0.0.4/agiflow/opentelemetry/instrumentation/anthropic/hooks/message_create.py
+-rw-r--r--   0        0        0     1730 2024-06-03 06:05:41.428153 agiflow_sdk-0.0.4/agiflow/opentelemetry/instrumentation/anthropic/instrumentation.py
+-rw-r--r--   0        0        0      145 2024-06-03 06:05:41.428426 agiflow_sdk-0.0.4/agiflow/opentelemetry/instrumentation/chroma/__init__.py
+-rw-r--r--   0        0        0      389 2024-06-03 06:05:41.429120 agiflow_sdk-0.0.4/agiflow/opentelemetry/instrumentation/chroma/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0     3196 2024-06-03 06:05:41.429322 agiflow_sdk-0.0.4/agiflow/opentelemetry/instrumentation/chroma/__pycache__/instrumentation.cpython-311.pyc
+-rw-r--r--   0        0        0      157 2024-06-03 06:05:41.429552 agiflow_sdk-0.0.4/agiflow/opentelemetry/instrumentation/chroma/hooks/__init__.py
+-rw-r--r--   0        0        0      405 2024-06-03 06:05:41.429778 agiflow_sdk-0.0.4/agiflow/opentelemetry/instrumentation/chroma/hooks/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0     2297 2024-06-03 06:05:41.430014 agiflow_sdk-0.0.4/agiflow/opentelemetry/instrumentation/chroma/hooks/__pycache__/base.cpython-311.pyc
+-rw-r--r--   0        0        0    16999 2024-06-03 06:05:41.430395 agiflow_sdk-0.0.4/agiflow/opentelemetry/instrumentation/chroma/hooks/__pycache__/collection_call.cpython-311.pyc
+-rw-r--r--   0        0        0     1385 2024-06-03 06:05:41.430558 agiflow_sdk-0.0.4/agiflow/opentelemetry/instrumentation/chroma/hooks/base.py
+-rw-r--r--   0        0        0    10704 2024-06-03 06:05:41.430702 agiflow_sdk-0.0.4/agiflow/opentelemetry/instrumentation/chroma/hooks/collection_call.py
+-rw-r--r--   0        0        0     1910 2024-06-03 06:05:41.430938 agiflow_sdk-0.0.4/agiflow/opentelemetry/instrumentation/chroma/instrumentation.py
+-rw-r--r--   0        0        0      145 2024-06-03 06:05:41.431172 agiflow_sdk-0.0.4/agiflow/opentelemetry/instrumentation/cohere/__init__.py
+-rw-r--r--   0        0        0      389 2024-06-03 06:05:41.432049 agiflow_sdk-0.0.4/agiflow/opentelemetry/instrumentation/cohere/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0     3487 2024-06-03 06:05:41.432194 agiflow_sdk-0.0.4/agiflow/opentelemetry/instrumentation/cohere/__pycache__/instrumentation.cpython-311.pyc
+-rw-r--r--   0        0        0      511 2024-06-03 06:05:41.432537 agiflow_sdk-0.0.4/agiflow/opentelemetry/instrumentation/cohere/hooks/__init__.py
+-rw-r--r--   0        0        0      809 2024-06-03 06:05:41.432797 agiflow_sdk-0.0.4/agiflow/opentelemetry/instrumentation/cohere/hooks/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0     2247 2024-06-03 06:05:41.432946 agiflow_sdk-0.0.4/agiflow/opentelemetry/instrumentation/cohere/hooks/__pycache__/base.cpython-311.pyc
+-rw-r--r--   0        0        0     8362 2024-06-03 06:05:41.433095 agiflow_sdk-0.0.4/agiflow/opentelemetry/instrumentation/cohere/hooks/__pycache__/base_chat.cpython-311.pyc
+-rw-r--r--   0        0        0     6177 2024-06-03 06:05:41.433320 agiflow_sdk-0.0.4/agiflow/opentelemetry/instrumentation/cohere/hooks/__pycache__/chat_create.cpython-311.pyc
+-rw-r--r--   0        0        0     7073 2024-06-03 06:05:41.433467 agiflow_sdk-0.0.4/agiflow/opentelemetry/instrumentation/cohere/hooks/__pycache__/chat_stream.cpython-311.pyc
+-rw-r--r--   0        0        0     5336 2024-06-03 06:05:41.433606 agiflow_sdk-0.0.4/agiflow/opentelemetry/instrumentation/cohere/hooks/__pycache__/embed.cpython-311.pyc
+-rw-r--r--   0        0        0     5930 2024-06-03 06:05:41.433737 agiflow_sdk-0.0.4/agiflow/opentelemetry/instrumentation/cohere/hooks/__pycache__/rerank.cpython-311.pyc
+-rw-r--r--   0        0        0     1328 2024-06-03 06:05:41.433895 agiflow_sdk-0.0.4/agiflow/opentelemetry/instrumentation/cohere/hooks/base.py
+-rw-r--r--   0        0        0     5765 2024-06-03 06:05:41.434039 agiflow_sdk-0.0.4/agiflow/opentelemetry/instrumentation/cohere/hooks/base_chat.py
+-rw-r--r--   0        0        0     4975 2024-06-03 06:05:41.434168 agiflow_sdk-0.0.4/agiflow/opentelemetry/instrumentation/cohere/hooks/chat_create.py
+-rw-r--r--   0        0        0     7065 2024-06-03 06:05:41.434297 agiflow_sdk-0.0.4/agiflow/opentelemetry/instrumentation/cohere/hooks/chat_stream.py
+-rw-r--r--   0        0        0     3919 2024-06-03 06:05:41.434436 agiflow_sdk-0.0.4/agiflow/opentelemetry/instrumentation/cohere/hooks/embed.py
+-rw-r--r--   0        0        0     4364 2024-06-03 06:05:41.434567 agiflow_sdk-0.0.4/agiflow/opentelemetry/instrumentation/cohere/hooks/rerank.py
+-rw-r--r--   0        0        0     2425 2024-06-03 06:05:41.434716 agiflow_sdk-0.0.4/agiflow/opentelemetry/instrumentation/cohere/instrumentation.py
+-rw-r--r--   0        0        0      391 2024-06-03 06:05:41.435061 agiflow_sdk-0.0.4/agiflow/opentelemetry/instrumentation/constants/__init__.py
+-rw-r--r--   0        0        0      649 2024-06-03 06:05:41.435613 agiflow_sdk-0.0.4/agiflow/opentelemetry/instrumentation/constants/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0      346 2024-06-03 06:05:41.435875 agiflow_sdk-0.0.4/agiflow/opentelemetry/instrumentation/constants/__pycache__/anthropic.cpython-311.pyc
+-rw-r--r--   0        0        0     1014 2024-06-03 06:05:41.436026 agiflow_sdk-0.0.4/agiflow/opentelemetry/instrumentation/constants/__pycache__/chroma.cpython-311.pyc
+-rw-r--r--   0        0        0      595 2024-06-03 06:05:41.436173 agiflow_sdk-0.0.4/agiflow/opentelemetry/instrumentation/constants/__pycache__/cohere.cpython-311.pyc
+-rw-r--r--   0        0        0      902 2024-06-03 06:05:41.436412 agiflow_sdk-0.0.4/agiflow/opentelemetry/instrumentation/constants/__pycache__/common.cpython-311.pyc
+-rw-r--r--   0        0        0     1074 2024-06-03 06:05:41.436638 agiflow_sdk-0.0.4/agiflow/opentelemetry/instrumentation/constants/__pycache__/openai.cpython-311.pyc
+-rw-r--r--   0        0        0      126 2024-06-03 06:05:41.436885 agiflow_sdk-0.0.4/agiflow/opentelemetry/instrumentation/constants/anthropic.py
+-rw-r--r--   0        0        0      972 2024-06-03 06:05:41.437021 agiflow_sdk-0.0.4/agiflow/opentelemetry/instrumentation/constants/chroma.py
+-rw-r--r--   0        0        0      577 2024-06-03 06:05:41.437150 agiflow_sdk-0.0.4/agiflow/opentelemetry/instrumentation/constants/cohere.py
+-rw-r--r--   0        0        0      750 2024-06-03 06:05:41.437337 agiflow_sdk-0.0.4/agiflow/opentelemetry/instrumentation/constants/common.py
+-rw-r--r--   0        0        0      134 2024-06-03 06:05:41.437471 agiflow_sdk-0.0.4/agiflow/opentelemetry/instrumentation/constants/groq.py
+-rw-r--r--   0        0        0     1054 2024-06-03 06:05:41.437695 agiflow_sdk-0.0.4/agiflow/opentelemetry/instrumentation/constants/openai.py
+-rw-r--r--   0        0        0      490 2024-06-03 06:05:41.437825 agiflow_sdk-0.0.4/agiflow/opentelemetry/instrumentation/constants/pinecone.py
+-rw-r--r--   0        0        0     2016 2024-06-03 06:05:41.437956 agiflow_sdk-0.0.4/agiflow/opentelemetry/instrumentation/constants/qdrant.py
+-rw-r--r--   0        0        0     1518 2024-06-03 06:05:41.438190 agiflow_sdk-0.0.4/agiflow/opentelemetry/instrumentation/constants/weaviate.py
+-rw-r--r--   0        0        0      139 2024-06-03 06:05:41.438552 agiflow_sdk-0.0.4/agiflow/opentelemetry/instrumentation/groq/__init__.py
+-rw-r--r--   0        0        0      156 2024-06-03 06:05:41.438767 agiflow_sdk-0.0.4/agiflow/opentelemetry/instrumentation/groq/hooks/__init__.py
+-rw-r--r--   0        0        0     1934 2024-06-03 06:05:41.438916 agiflow_sdk-0.0.4/agiflow/opentelemetry/instrumentation/groq/hooks/base.py
+-rw-r--r--   0        0        0    12481 2024-06-03 06:05:41.439078 agiflow_sdk-0.0.4/agiflow/opentelemetry/instrumentation/groq/hooks/chat_completion.py
+-rw-r--r--   0        0        0     1993 2024-06-03 06:05:41.439259 agiflow_sdk-0.0.4/agiflow/opentelemetry/instrumentation/groq/instrumentation.py
+-rw-r--r--   0        0        0     6148 2024-06-03 06:05:41.439706 agiflow_sdk-0.0.4/agiflow/opentelemetry/instrumentation/langchain/.DS_Store
+-rw-r--r--   0        0        0      154 2024-06-03 06:05:41.439849 agiflow_sdk-0.0.4/agiflow/opentelemetry/instrumentation/langchain/__init__.py
+-rw-r--r--   0        0        0      398 2024-06-03 06:05:41.440237 agiflow_sdk-0.0.4/agiflow/opentelemetry/instrumentation/langchain/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0     3233 2024-06-03 06:05:41.440535 agiflow_sdk-0.0.4/agiflow/opentelemetry/instrumentation/langchain/__pycache__/instrumentation.cpython-311.pyc
+-rw-r--r--   0        0        0     4136 2024-06-03 06:05:41.440888 agiflow_sdk-0.0.4/agiflow/opentelemetry/instrumentation/langchain/__pycache__/patch.cpython-311.pyc
+-rw-r--r--   0        0        0      252 2024-06-03 06:05:41.441276 agiflow_sdk-0.0.4/agiflow/opentelemetry/instrumentation/langchain/hooks/__init__.py
+-rw-r--r--   0        0        0      532 2024-06-03 06:05:41.441747 agiflow_sdk-0.0.4/agiflow/opentelemetry/instrumentation/langchain/hooks/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0     2313 2024-06-03 06:05:41.441903 agiflow_sdk-0.0.4/agiflow/opentelemetry/instrumentation/langchain/hooks/__pycache__/base.cpython-311.pyc
+-rw-r--r--   0        0        0     7286 2024-06-03 06:05:41.442050 agiflow_sdk-0.0.4/agiflow/opentelemetry/instrumentation/langchain/hooks/__pycache__/chat.cpython-311.pyc
+-rw-r--r--   0        0        0     3122 2024-06-03 06:05:41.442293 agiflow_sdk-0.0.4/agiflow/opentelemetry/instrumentation/langchain/hooks/__pycache__/generic.cpython-311.pyc
+-rw-r--r--   0        0        0     1384 2024-06-03 06:05:41.442449 agiflow_sdk-0.0.4/agiflow/opentelemetry/instrumentation/langchain/hooks/base.py
+-rw-r--r--   0        0        0     5021 2024-06-03 06:05:41.442597 agiflow_sdk-0.0.4/agiflow/opentelemetry/instrumentation/langchain/hooks/chat.py
+-rw-r--r--   0        0        0     1741 2024-06-03 06:05:41.442839 agiflow_sdk-0.0.4/agiflow/opentelemetry/instrumentation/langchain/hooks/generic.py
+-rw-r--r--   0        0        0     2232 2024-06-03 06:05:41.442987 agiflow_sdk-0.0.4/agiflow/opentelemetry/instrumentation/langchain/instrumentation.py
+-rw-r--r--   0        0        0     6148 2024-06-03 06:05:41.443400 agiflow_sdk-0.0.4/agiflow/opentelemetry/instrumentation/langchain_community/.DS_Store
+-rw-r--r--   0        0        0      182 2024-06-03 06:05:41.443636 agiflow_sdk-0.0.4/agiflow/opentelemetry/instrumentation/langchain_community/__init__.py
+-rw-r--r--   0        0        0      427 2024-06-03 06:05:41.443862 agiflow_sdk-0.0.4/agiflow/opentelemetry/instrumentation/langchain_community/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0     3462 2024-06-03 06:05:41.443997 agiflow_sdk-0.0.4/agiflow/opentelemetry/instrumentation/langchain_community/__pycache__/instrumentation.cpython-311.pyc
+-rw-r--r--   0        0        0    11425 2024-06-03 06:05:41.444345 agiflow_sdk-0.0.4/agiflow/opentelemetry/instrumentation/langchain_community/__pycache__/patch.cpython-311.pyc
+-rw-r--r--   0        0        0     6148 2024-06-03 06:05:41.444880 agiflow_sdk-0.0.4/agiflow/opentelemetry/instrumentation/langchain_community/hooks/.DS_Store
+-rw-r--r--   0        0        0      141 2024-06-03 06:05:41.445007 agiflow_sdk-0.0.4/agiflow/opentelemetry/instrumentation/langchain_community/hooks/__init__.py
+-rw-r--r--   0        0        0      404 2024-06-03 06:05:41.445483 agiflow_sdk-0.0.4/agiflow/opentelemetry/instrumentation/langchain_community/hooks/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0     2481 2024-06-03 06:05:41.445724 agiflow_sdk-0.0.4/agiflow/opentelemetry/instrumentation/langchain_community/hooks/__pycache__/base.cpython-311.pyc
+-rw-r--r--   0        0        0     6863 2024-06-03 06:05:41.446022 agiflow_sdk-0.0.4/agiflow/opentelemetry/instrumentation/langchain_community/hooks/__pycache__/chat.cpython-311.pyc
+-rw-r--r--   0        0        0     3163 2024-06-03 06:05:41.446194 agiflow_sdk-0.0.4/agiflow/opentelemetry/instrumentation/langchain_community/hooks/__pycache__/generic.cpython-311.pyc
+-rw-r--r--   0        0        0     5119 2024-06-03 06:05:41.446495 agiflow_sdk-0.0.4/agiflow/opentelemetry/instrumentation/langchain_community/hooks/__pycache__/llm.cpython-311.pyc
+-rw-r--r--   0        0        0     1499 2024-06-03 06:05:41.446635 agiflow_sdk-0.0.4/agiflow/opentelemetry/instrumentation/langchain_community/hooks/base.py
+-rw-r--r--   0        0        0     1769 2024-06-03 06:05:41.446777 agiflow_sdk-0.0.4/agiflow/opentelemetry/instrumentation/langchain_community/hooks/generic.py
+-rw-r--r--   0        0        0     3005 2024-06-03 06:05:41.446925 agiflow_sdk-0.0.4/agiflow/opentelemetry/instrumentation/langchain_community/instrumentation.py
+-rw-r--r--   0        0        0     6148 2024-06-03 06:05:41.447349 agiflow_sdk-0.0.4/agiflow/opentelemetry/instrumentation/langchain_core/.DS_Store
+-rw-r--r--   0        0        0      167 2024-06-03 06:05:41.447482 agiflow_sdk-0.0.4/agiflow/opentelemetry/instrumentation/langchain_core/__init__.py
+-rw-r--r--   0        0        0      412 2024-06-03 06:05:41.447699 agiflow_sdk-0.0.4/agiflow/opentelemetry/instrumentation/langchain_core/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0     3928 2024-06-03 06:05:41.447837 agiflow_sdk-0.0.4/agiflow/opentelemetry/instrumentation/langchain_core/__pycache__/instrumentation.cpython-311.pyc
+-rw-r--r--   0        0        0     8316 2024-06-03 06:05:41.448068 agiflow_sdk-0.0.4/agiflow/opentelemetry/instrumentation/langchain_core/__pycache__/patch.cpython-311.pyc
+-rw-r--r--   0        0        0      390 2024-06-03 06:05:41.448485 agiflow_sdk-0.0.4/agiflow/opentelemetry/instrumentation/langchain_core/hooks/__init__.py
+-rw-r--r--   0        0        0      693 2024-06-03 06:05:41.448717 agiflow_sdk-0.0.4/agiflow/opentelemetry/instrumentation/langchain_core/hooks/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0     2558 2024-06-03 06:05:41.448857 agiflow_sdk-0.0.4/agiflow/opentelemetry/instrumentation/langchain_core/hooks/__pycache__/base.cpython-311.pyc
+-rw-r--r--   0        0        0     3573 2024-06-03 06:05:41.449088 agiflow_sdk-0.0.4/agiflow/opentelemetry/instrumentation/langchain_core/hooks/__pycache__/generic.cpython-311.pyc
+-rw-r--r--   0        0        0     5208 2024-06-03 06:05:41.449222 agiflow_sdk-0.0.4/agiflow/opentelemetry/instrumentation/langchain_core/hooks/__pycache__/llm.cpython-311.pyc
+-rw-r--r--   0        0        0     4692 2024-06-03 06:05:41.449552 agiflow_sdk-0.0.4/agiflow/opentelemetry/instrumentation/langchain_core/hooks/__pycache__/runnable.cpython-311.pyc
+-rw-r--r--   0        0        0     1533 2024-06-03 06:05:41.449806 agiflow_sdk-0.0.4/agiflow/opentelemetry/instrumentation/langchain_core/hooks/base.py
+-rw-r--r--   0        0        0     2152 2024-06-03 06:05:41.449938 agiflow_sdk-0.0.4/agiflow/opentelemetry/instrumentation/langchain_core/hooks/generic.py
+-rw-r--r--   0        0        0     3178 2024-06-03 06:05:41.450124 agiflow_sdk-0.0.4/agiflow/opentelemetry/instrumentation/langchain_core/hooks/llm.py
+-rw-r--r--   0        0        0     3248 2024-06-03 06:05:41.450261 agiflow_sdk-0.0.4/agiflow/opentelemetry/instrumentation/langchain_core/hooks/runnable.py
+-rw-r--r--   0        0        0     3346 2024-06-03 06:05:41.450417 agiflow_sdk-0.0.4/agiflow/opentelemetry/instrumentation/langchain_core/instrumentation.py
+-rw-r--r--   0        0        0      154 2024-06-03 06:05:41.450911 agiflow_sdk-0.0.4/agiflow/opentelemetry/instrumentation/langgraph/__init__.py
+-rw-r--r--   0        0        0      146 2024-06-03 06:05:41.451140 agiflow_sdk-0.0.4/agiflow/opentelemetry/instrumentation/langgraph/hooks/__init__.py
+-rw-r--r--   0        0        0     1343 2024-06-03 06:05:41.451283 agiflow_sdk-0.0.4/agiflow/opentelemetry/instrumentation/langgraph/hooks/base.py
+-rw-r--r--   0        0        0     3352 2024-06-03 06:05:41.451409 agiflow_sdk-0.0.4/agiflow/opentelemetry/instrumentation/langgraph/hooks/graph_call.py
+-rw-r--r--   0        0        0     2873 2024-06-03 06:05:41.451560 agiflow_sdk-0.0.4/agiflow/opentelemetry/instrumentation/langgraph/instrumentation.py
+-rw-r--r--   0        0        0      157 2024-06-03 06:05:41.451861 agiflow_sdk-0.0.4/agiflow/opentelemetry/instrumentation/llamaindex/__init__.py
+-rw-r--r--   0        0        0      140 2024-06-03 06:05:41.452087 agiflow_sdk-0.0.4/agiflow/opentelemetry/instrumentation/llamaindex/hooks/__init__.py
+-rw-r--r--   0        0        0     1347 2024-06-03 06:05:41.452241 agiflow_sdk-0.0.4/agiflow/opentelemetry/instrumentation/llamaindex/hooks/base.py
+-rw-r--r--   0        0        0     1718 2024-06-03 06:05:41.452379 agiflow_sdk-0.0.4/agiflow/opentelemetry/instrumentation/llamaindex/hooks/generic.py
+-rw-r--r--   0        0        0     2944 2024-06-03 06:05:41.452553 agiflow_sdk-0.0.4/agiflow/opentelemetry/instrumentation/llamaindex/instrumentation.py
+-rw-r--r--   0        0        0     6148 2024-06-03 06:05:41.452909 agiflow_sdk-0.0.4/agiflow/opentelemetry/instrumentation/openai/.DS_Store
+-rw-r--r--   0        0        0      145 2024-06-03 06:05:41.453083 agiflow_sdk-0.0.4/agiflow/opentelemetry/instrumentation/openai/__init__.py
+-rw-r--r--   0        0        0      389 2024-06-03 06:05:41.453320 agiflow_sdk-0.0.4/agiflow/opentelemetry/instrumentation/openai/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0     3659 2024-06-03 06:05:41.453451 agiflow_sdk-0.0.4/agiflow/opentelemetry/instrumentation/openai/__pycache__/instrumentation.cpython-311.pyc
+-rw-r--r--   0        0        0    20526 2024-06-03 06:05:41.454059 agiflow_sdk-0.0.4/agiflow/opentelemetry/instrumentation/openai/__pycache__/patch.cpython-311.pyc
+-rw-r--r--   0        0        0     6148 2024-06-03 06:05:41.454586 agiflow_sdk-0.0.4/agiflow/opentelemetry/instrumentation/openai/hooks/.DS_Store
+-rw-r--r--   0        0        0      424 2024-06-03 06:05:41.454719 agiflow_sdk-0.0.4/agiflow/opentelemetry/instrumentation/openai/hooks/__init__.py
+-rw-r--r--   0        0        0      699 2024-06-03 06:05:41.456812 agiflow_sdk-0.0.4/agiflow/opentelemetry/instrumentation/openai/hooks/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0     4035 2024-06-03 06:05:41.456990 agiflow_sdk-0.0.4/agiflow/opentelemetry/instrumentation/openai/hooks/__pycache__/base.cpython-311.pyc
+-rw-r--r--   0        0        0     4744 2024-06-03 06:05:41.457303 agiflow_sdk-0.0.4/agiflow/opentelemetry/instrumentation/openai/hooks/__pycache__/base_llm.cpython-311.pyc
+-rw-r--r--   0        0        0    12171 2024-06-03 06:05:41.457481 agiflow_sdk-0.0.4/agiflow/opentelemetry/instrumentation/openai/hooks/__pycache__/chat_completion.cpython-311.pyc
+-rw-r--r--   0        0        0    11736 2024-06-03 06:05:41.458012 agiflow_sdk-0.0.4/agiflow/opentelemetry/instrumentation/openai/hooks/__pycache__/completion.cpython-311.pyc
+-rw-r--r--   0        0        0     3391 2024-06-03 06:05:41.458360 agiflow_sdk-0.0.4/agiflow/opentelemetry/instrumentation/openai/hooks/__pycache__/embedding.cpython-311.pyc
+-rw-r--r--   0        0        0     3885 2024-06-03 06:05:41.458541 agiflow_sdk-0.0.4/agiflow/opentelemetry/instrumentation/openai/hooks/__pycache__/image_generate.cpython-311.pyc
+-rw-r--r--   0        0        0     2374 2024-06-03 06:05:41.458731 agiflow_sdk-0.0.4/agiflow/opentelemetry/instrumentation/openai/hooks/__pycache__/utils.cpython-311.pyc
+-rw-r--r--   0        0        0     2474 2024-06-03 06:05:41.458908 agiflow_sdk-0.0.4/agiflow/opentelemetry/instrumentation/openai/hooks/base.py
+-rw-r--r--   0        0        0     3115 2024-06-03 06:05:41.459151 agiflow_sdk-0.0.4/agiflow/opentelemetry/instrumentation/openai/hooks/base_llm.py
+-rw-r--r--   0        0        0    10648 2024-06-03 06:05:41.459315 agiflow_sdk-0.0.4/agiflow/opentelemetry/instrumentation/openai/hooks/chat_completion.py
+-rw-r--r--   0        0        0     2257 2024-06-03 06:05:41.459821 agiflow_sdk-0.0.4/agiflow/opentelemetry/instrumentation/openai/hooks/embedding.py
+-rw-r--r--   0        0        0     2555 2024-06-03 06:05:41.460077 agiflow_sdk-0.0.4/agiflow/opentelemetry/instrumentation/openai/hooks/image_generate.py
+-rw-r--r--   0        0        0     2211 2024-06-03 06:05:41.460239 agiflow_sdk-0.0.4/agiflow/opentelemetry/instrumentation/openai/hooks/utils.py
+-rw-r--r--   0        0        0     2910 2024-06-03 06:05:41.460411 agiflow_sdk-0.0.4/agiflow/opentelemetry/instrumentation/openai/instrumentation.py
+-rw-r--r--   0        0        0      151 2024-06-03 06:05:41.460834 agiflow_sdk-0.0.4/agiflow/opentelemetry/instrumentation/pinecone/__init__.py
+-rw-r--r--   0        0        0      137 2024-06-03 06:05:41.461063 agiflow_sdk-0.0.4/agiflow/opentelemetry/instrumentation/pinecone/hooks/__init__.py
+-rw-r--r--   0        0        0     1396 2024-06-03 06:05:41.461197 agiflow_sdk-0.0.4/agiflow/opentelemetry/instrumentation/pinecone/hooks/base.py
+-rw-r--r--   0        0        0     6892 2024-06-03 06:05:41.461331 agiflow_sdk-0.0.4/agiflow/opentelemetry/instrumentation/pinecone/hooks/generic.py
+-rw-r--r--   0        0        0     2019 2024-06-03 06:05:41.461477 agiflow_sdk-0.0.4/agiflow/opentelemetry/instrumentation/pinecone/instrumentation.py
+-rw-r--r--   0        0        0      145 2024-06-03 06:05:41.461711 agiflow_sdk-0.0.4/agiflow/opentelemetry/instrumentation/qdrant/__init__.py
+-rw-r--r--   0        0        0      152 2024-06-03 06:05:41.461912 agiflow_sdk-0.0.4/agiflow/opentelemetry/instrumentation/qdrant/hooks/__init__.py
+-rw-r--r--   0        0        0     1388 2024-06-03 06:05:41.462043 agiflow_sdk-0.0.4/agiflow/opentelemetry/instrumentation/qdrant/hooks/base.py
+-rw-r--r--   0        0        0     3113 2024-06-03 06:05:41.462178 agiflow_sdk-0.0.4/agiflow/opentelemetry/instrumentation/qdrant/hooks/collection.py
+-rw-r--r--   0        0        0     1913 2024-06-03 06:05:41.462314 agiflow_sdk-0.0.4/agiflow/opentelemetry/instrumentation/qdrant/instrumentation.py
+-rw-r--r--   0        0        0     2309 2024-06-03 06:05:41.462545 agiflow_sdk-0.0.4/agiflow/opentelemetry/instrumentation/utils/__init__.py
+-rw-r--r--   0        0        0     2790 2024-06-03 06:05:41.462885 agiflow_sdk-0.0.4/agiflow/opentelemetry/instrumentation/utils/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0    17396 2024-06-03 06:05:41.463247 agiflow_sdk-0.0.4/agiflow/opentelemetry/instrumentation/utils/__pycache__/wrapper.cpython-311.pyc
+-rw-r--r--   0        0        0    11559 2024-06-03 06:05:41.463408 agiflow_sdk-0.0.4/agiflow/opentelemetry/instrumentation/utils/wrapper.py
+-rw-r--r--   0        0        0      151 2024-06-03 06:05:41.464045 agiflow_sdk-0.0.4/agiflow/opentelemetry/instrumentation/weaviate/__init__.py
+-rw-r--r--   0        0        0      306 2024-06-03 06:05:41.464335 agiflow_sdk-0.0.4/agiflow/opentelemetry/instrumentation/weaviate/hooks/__init__.py
+-rw-r--r--   0        0        0     1396 2024-06-03 06:05:41.464496 agiflow_sdk-0.0.4/agiflow/opentelemetry/instrumentation/weaviate/hooks/base.py
+-rw-r--r--   0        0        0     1776 2024-06-03 06:05:41.464670 agiflow_sdk-0.0.4/agiflow/opentelemetry/instrumentation/weaviate/hooks/generic_collection.py
+-rw-r--r--   0        0        0     4091 2024-06-03 06:05:41.464817 agiflow_sdk-0.0.4/agiflow/opentelemetry/instrumentation/weaviate/hooks/generic_query.py
+-rw-r--r--   0        0        0     2754 2024-06-03 06:05:41.465004 agiflow_sdk-0.0.4/agiflow/opentelemetry/instrumentation/weaviate/instrumentation.py
+-rw-r--r--   0        0        0      144 2024-06-03 06:05:41.465457 agiflow_sdk-0.0.4/agiflow/opentelemetry/span_processors/__init__.py
+-rw-r--r--   0        0        0      376 2024-06-03 06:05:41.466056 agiflow_sdk-0.0.4/agiflow/opentelemetry/span_processors/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0     5123 2024-06-03 06:05:41.466324 agiflow_sdk-0.0.4/agiflow/opentelemetry/span_processors/__pycache__/thread_pool_span_processor.cpython-311.pyc
+-rw-r--r--   0        0        0     2544 2024-06-03 06:05:41.466610 agiflow_sdk-0.0.4/agiflow/opentelemetry/span_processors/thread_pool_span_processor.py
+-rw-r--r--   0        0        0      644 2024-06-03 06:05:41.466926 agiflow_sdk-0.0.4/agiflow/opentelemetry/trace_decorators/__init__.py
+-rw-r--r--   0        0        0      910 2024-06-03 06:05:41.467498 agiflow_sdk-0.0.4/agiflow/opentelemetry/trace_decorators/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0     1383 2024-06-03 06:05:41.467757 agiflow_sdk-0.0.4/agiflow/opentelemetry/trace_decorators/__pycache__/helper.cpython-311.pyc
+-rw-r--r--   0        0        0     4548 2024-06-03 06:05:41.467975 agiflow_sdk-0.0.4/agiflow/opentelemetry/trace_decorators/__pycache__/task.cpython-311.pyc
+-rw-r--r--   0        0        0     3461 2024-06-03 06:05:41.468329 agiflow_sdk-0.0.4/agiflow/opentelemetry/trace_decorators/__pycache__/workflow.cpython-311.pyc
+-rw-r--r--   0        0        0    19398 2024-06-03 06:05:41.468711 agiflow_sdk-0.0.4/agiflow/opentelemetry/trace_decorators/__pycache__/wrapper.cpython-311.pyc
+-rw-r--r--   0        0        0     1650 2024-06-03 06:05:41.468999 agiflow_sdk-0.0.4/agiflow/opentelemetry/trace_decorators/helper.py
+-rw-r--r--   0        0        0     3514 2024-06-03 06:05:41.469243 agiflow_sdk-0.0.4/agiflow/opentelemetry/trace_decorators/task.py
+-rw-r--r--   0        0        0     2241 2024-06-03 06:05:41.469499 agiflow_sdk-0.0.4/agiflow/opentelemetry/trace_decorators/workflow.py
+-rw-r--r--   0        0        0    15064 2024-06-03 06:05:41.469740 agiflow_sdk-0.0.4/agiflow/opentelemetry/trace_decorators/wrapper.py
+-rw-r--r--   0        0        0      115 2024-06-03 06:05:41.470099 agiflow_sdk-0.0.4/agiflow/opentelemetry/trace_exporter/__init__.py
+-rw-r--r--   0        0        0      349 2024-06-03 06:05:41.470425 agiflow_sdk-0.0.4/agiflow/opentelemetry/trace_exporter/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0     2687 2024-06-03 06:05:41.470653 agiflow_sdk-0.0.4/agiflow/opentelemetry/trace_exporter/__pycache__/config.cpython-311.pyc
+-rw-r--r--   0        0        0     9661 2024-06-03 06:05:41.470914 agiflow_sdk-0.0.4/agiflow/opentelemetry/trace_exporter/__pycache__/json.cpython-311.pyc
+-rw-r--r--   0        0        0      238 2024-06-03 06:05:41.471145 agiflow_sdk-0.0.4/agiflow/opentelemetry/trace_exporter/__pycache__/version.cpython-311.pyc
+-rw-r--r--   0        0        0     2757 2024-06-03 06:05:41.471379 agiflow_sdk-0.0.4/agiflow/opentelemetry/trace_exporter/config.py
+-rw-r--r--   0        0        0     7123 2024-06-03 06:05:41.471616 agiflow_sdk-0.0.4/agiflow/opentelemetry/trace_exporter/json.py
+-rw-r--r--   0        0        0       22 2024-06-03 06:05:41.471738 agiflow_sdk-0.0.4/agiflow/opentelemetry/trace_exporter/version.py
+-rw-r--r--   0        0        0       99 2024-06-03 06:05:41.472143 agiflow_sdk-0.0.4/agiflow/opentelemetry/trace_sampler/__init__.py
+-rw-r--r--   0        0        0      342 2024-06-03 06:05:41.472503 agiflow_sdk-0.0.4/agiflow/opentelemetry/trace_sampler/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0     1787 2024-06-03 06:05:41.472741 agiflow_sdk-0.0.4/agiflow/opentelemetry/trace_sampler/__pycache__/no_sampler.cpython-311.pyc
+-rw-r--r--   0        0        0      862 2024-06-03 06:05:41.472991 agiflow_sdk-0.0.4/agiflow/opentelemetry/trace_sampler/no_sampler.py
+-rw-r--r--   0        0        0     3160 2024-06-03 06:05:41.473320 agiflow_sdk-0.0.4/agiflow/opentelemetry/trace_store.py
+-rw-r--r--   0        0        0     6148 2024-06-03 06:05:41.473786 agiflow_sdk-0.0.4/agiflow/opentelemetry/tracing/.DS_Store
+-rw-r--r--   0        0        0      182 2024-06-03 06:05:41.473962 agiflow_sdk-0.0.4/agiflow/opentelemetry/tracing/__init__.py
+-rw-r--r--   0        0        0      437 2024-06-03 06:05:41.474292 agiflow_sdk-0.0.4/agiflow/opentelemetry/tracing/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0     1979 2024-06-03 06:05:41.474519 agiflow_sdk-0.0.4/agiflow/opentelemetry/tracing/__pycache__/content_allow_list.cpython-311.pyc
+-rw-r--r--   0        0        0     1978 2024-06-03 06:05:41.474657 agiflow_sdk-0.0.4/agiflow/opentelemetry/tracing/__pycache__/content_alow_list.cpython-311.pyc
+-rw-r--r--   0        0        0     5230 2024-06-03 06:05:41.474795 agiflow_sdk-0.0.4/agiflow/opentelemetry/tracing/__pycache__/context.cpython-311.pyc
+-rw-r--r--   0        0        0      897 2024-06-03 06:05:41.474922 agiflow_sdk-0.0.4/agiflow/opentelemetry/tracing/__pycache__/context_manager.cpython-311.pyc
+-rw-r--r--   0        0        0     1507 2024-06-03 06:05:41.475149 agiflow_sdk-0.0.4/agiflow/opentelemetry/tracing/__pycache__/context_propagation.cpython-311.pyc
+-rw-r--r--   0        0        0     2581 2024-06-03 06:05:41.475342 agiflow_sdk-0.0.4/agiflow/opentelemetry/tracing/__pycache__/span_from_context.cpython-311.pyc
+-rw-r--r--   0        0        0    10065 2024-06-03 06:05:41.475565 agiflow_sdk-0.0.4/agiflow/opentelemetry/tracing/__pycache__/tracing.cpython-311.pyc
+-rw-r--r--   0        0        0      846 2024-06-03 06:05:41.475844 agiflow_sdk-0.0.4/agiflow/opentelemetry/tracing/content_allow_list.py
+-rw-r--r--   0        0        0      307 2024-06-03 06:05:41.476054 agiflow_sdk-0.0.4/agiflow/opentelemetry/tracing/context_manager.py
+-rw-r--r--   0        0        0     7265 2024-06-03 06:05:41.476272 agiflow_sdk-0.0.4/agiflow/opentelemetry/tracing/tracing.py
+-rw-r--r--   0        0        0      813 2024-06-03 06:05:41.476558 agiflow_sdk-0.0.4/agiflow/opentelemetry/types/__init__.py
+-rw-r--r--   0        0        0     1865 2024-06-03 06:05:41.476962 agiflow_sdk-0.0.4/agiflow/opentelemetry/types/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0     6148 2024-06-03 06:05:41.477297 agiflow_sdk-0.0.4/agiflow/opentelemetry/utils/.DS_Store
+-rw-r--r--   0        0        0      340 2024-06-03 06:05:41.477424 agiflow_sdk-0.0.4/agiflow/opentelemetry/utils/__init__.py
+-rw-r--r--   0        0        0      521 2024-06-03 06:05:41.478103 agiflow_sdk-0.0.4/agiflow/opentelemetry/utils/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0     3447 2024-06-03 06:05:41.478316 agiflow_sdk-0.0.4/agiflow/opentelemetry/utils/__pycache__/llm.cpython-311.pyc
+-rw-r--r--   0        0        0     2240 2024-06-03 06:05:41.478481 agiflow_sdk-0.0.4/agiflow/opentelemetry/utils/llm.py
+-rw-r--r--   0        0        0       71 2024-06-03 06:05:41.478746 agiflow_sdk-0.0.4/agiflow/services/__init__.py
+-rw-r--r--   0        0        0      297 2024-06-03 06:05:41.478969 agiflow_sdk-0.0.4/agiflow/services/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0     5452 2024-06-03 06:05:41.479106 agiflow_sdk-0.0.4/agiflow/services/__pycache__/fetch.cpython-311.pyc
+-rw-r--r--   0        0        0     2731 2024-06-03 06:05:41.479241 agiflow_sdk-0.0.4/agiflow/services/fetch.py
+-rw-r--r--   0        0        0     2522 2024-06-03 06:05:41.479459 agiflow_sdk-0.0.4/agiflow/telemetry/__init__.py
+-rw-r--r--   0        0        0     4829 2024-06-03 06:05:41.479677 agiflow_sdk-0.0.4/agiflow/telemetry/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0     6148 2024-06-03 06:05:41.480130 agiflow_sdk-0.0.4/agiflow/utils/.DS_Store
+-rw-r--r--   0        0        0      444 2024-06-03 06:05:41.480283 agiflow_sdk-0.0.4/agiflow/utils/__init__.py
+-rw-r--r--   0        0        0      728 2024-06-03 06:05:41.480498 agiflow_sdk-0.0.4/agiflow/utils/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0      532 2024-06-03 06:05:41.480739 agiflow_sdk-0.0.4/agiflow/utils/__pycache__/assertion.cpython-311.pyc
+-rw-r--r--   0        0        0     1923 2024-06-03 06:05:41.480879 agiflow_sdk-0.0.4/agiflow/utils/__pycache__/debugging.cpython-311.pyc
+-rw-r--r--   0        0        0     1719 2024-06-03 06:05:41.481013 agiflow_sdk-0.0.4/agiflow/utils/__pycache__/error.cpython-311.pyc
+-rw-r--r--   0        0        0     3268 2024-06-03 06:05:41.481246 agiflow_sdk-0.0.4/agiflow/utils/__pycache__/llm.cpython-311.pyc
+-rw-r--r--   0        0        0     4718 2024-06-03 06:05:41.481389 agiflow_sdk-0.0.4/agiflow/utils/__pycache__/string.cpython-311.pyc
+-rw-r--r--   0        0        0      583 2024-06-03 06:05:41.481522 agiflow_sdk-0.0.4/agiflow/utils/__pycache__/time.cpython-311.pyc
+-rw-r--r--   0        0        0      207 2024-06-03 06:05:41.481757 agiflow_sdk-0.0.4/agiflow/utils/assertion.py
+-rw-r--r--   0        0        0      580 2024-06-03 06:05:41.481884 agiflow_sdk-0.0.4/agiflow/utils/debugging.py
+-rw-r--r--   0        0        0      847 2024-06-03 06:05:41.482020 agiflow_sdk-0.0.4/agiflow/utils/error.py
+-rw-r--r--   0        0        0     1965 2024-06-03 06:05:41.482142 agiflow_sdk-0.0.4/agiflow/utils/string.py
+-rw-r--r--   0        0        0      264 2024-06-03 06:05:41.482273 agiflow_sdk-0.0.4/agiflow/utils/time.py
+-rw-r--r--   0        0        0       22 2024-06-03 06:05:41.482399 agiflow_sdk-0.0.4/agiflow/version.py
+-rw-r--r--   0        0        0     1106 2024-06-03 06:05:41.488768 agiflow_sdk-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0     1760 1970-01-01 00:00:00.000000 agiflow_sdk-0.0.4/PKG-INFO
```

### Comparing `agiflow_sdk-0.0.3/agiflow/__init__.py` & `agiflow_sdk-0.0.4/agiflow/agiflow.py`

 * *Files identical despite different names*

### Comparing `agiflow_sdk-0.0.3/agiflow/config/__init__.py` & `agiflow_sdk-0.0.4/agiflow/config/__init__.py`

 * *Files identical despite different names*

### Comparing `agiflow_sdk-0.0.3/agiflow/config/__pycache__/__init__.cpython-311.pyc` & `agiflow_sdk-0.0.4/agiflow/config/__pycache__/__init__.cpython-311.pyc`

 * *Files 2% similar despite different names*

#### Python bytecode

```diff
@@ -1,9 +1,9 @@
 magic:    0xa70d0d0a
-moddate:  0xe6bc5b66 (Sun Jun  2 00:29:26 2024 UTC)
+moddate:  0x47d85b66 (Sun Jun  2 02:26:15 2024 UTC)
 files sz: 889
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 2
    flags     : 0
    code
```

### Comparing `agiflow_sdk-0.0.3/agiflow/config/__pycache__/environment_vars.cpython-311.pyc` & `agiflow_sdk-0.0.4/agiflow/config/__pycache__/environment_vars.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `agiflow_sdk-0.0.3/agiflow/config/environment_vars.py` & `agiflow_sdk-0.0.4/agiflow/config/environment_vars.py`

 * *Files identical despite different names*

### Comparing `agiflow_sdk-0.0.3/agiflow/opentelemetry/.DS_Store` & `agiflow_sdk-0.0.4/agiflow/opentelemetry/.DS_Store`

 * *Files identical despite different names*

### Comparing `agiflow_sdk-0.0.3/agiflow/opentelemetry/__init__.py` & `agiflow_sdk-0.0.4/agiflow/opentelemetry/__init__.py`

 * *Files identical despite different names*

### Comparing `agiflow_sdk-0.0.3/agiflow/opentelemetry/__pycache__/__init__.cpython-311.pyc` & `agiflow_sdk-0.0.4/agiflow/opentelemetry/__pycache__/__init__.cpython-311.pyc`

 * *Files 4% similar despite different names*

#### Python bytecode

```diff
@@ -1,9 +1,9 @@
 magic:    0xa70d0d0a
-moddate:  0x39b55b66 (Sat Jun  1 23:56:41 2024 UTC)
+moddate:  0x47d85b66 (Sun Jun  2 02:26:15 2024 UTC)
 files sz: 1037
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 2
    flags     : 0
    code
```

### Comparing `agiflow_sdk-0.0.3/agiflow/opentelemetry/__pycache__/trace_store.cpython-311.pyc` & `agiflow_sdk-0.0.4/agiflow/opentelemetry/__pycache__/trace_store.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `agiflow_sdk-0.0.3/agiflow/opentelemetry/context/__init__.py` & `agiflow_sdk-0.0.4/agiflow/opentelemetry/context/__init__.py`

 * *Files 23% similar despite different names*

```diff
@@ -15,15 +15,16 @@
 )
 from agiflow.opentelemetry.context.span_from_context import (
   set_workflow_name_from_context,
   set_prompt_attributes_from_context,
 )
 from agiflow.opentelemetry.context.context_propagation import (
   get_trace_context_from_carrier,
-  get_carrier_from_trace_context
+  get_carrier_from_trace_context,
+  extract_association_properties_from_http_headers,
 )
 
 __all__ = [
   'ContextKeys',
   'PromptSettings',
   'AssociationProperties',
   'set_association_properties',
@@ -34,8 +35,9 @@
   'get_correlation_id',
   'get_association_properties',
   'get_prompt_settings',
   'set_workflow_name_from_context',
   'set_prompt_attributes_from_context',
   'get_trace_context_from_carrier',
   'get_carrier_from_trace_context',
+  'extract_association_properties_from_http_headers'
 ]
```

### Comparing `agiflow_sdk-0.0.3/agiflow/opentelemetry/context/__pycache__/__init__.cpython-311.pyc` & `agiflow_sdk-0.0.4/agiflow/opentelemetry/context/__pycache__/__init__.cpython-311.pyc`

 * *Files 12% similar despite different names*

#### Python bytecode

```diff
@@ -1,20 +1,20 @@
 magic:    0xa70d0d0a
-moddate:  0x43985a66 (Sat Jun  1 03:40:51 2024 UTC)
-files sz: 1112
+moddate:  0x6a425c66 (Sun Jun  2 09:59:06 2024 UTC)
+files sz: 1218
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 2
    flags     : 0
    code
       0x9700640064016c006d015a016d025a026d035a030100640064026c046d
       055a056d065a066d075a076d085a086d095a096d0a5a0a6d0b5a0b6d0c5a
       0c0100640064036c0d6d0e5a0e6d0f5a0f0100640064046c106d115a116d
-      125a12010067006405a2015a1364065300
+      125a126d135a13010067006405a2015a1464065300
      0           0 RESUME                   0
    
      1           2 LOAD_CONST               0 (0)
                  4 LOAD_CONST               1 (('ContextKeys', 'PromptSettings', 'AssociationProperties'))
                  6 IMPORT_NAME              0 (agiflow.opentelemetry.context.constants)
                  8 IMPORT_FROM              1 (ContextKeys)
                 10 STORE_NAME               1 (ContextKeys)
@@ -51,37 +51,39 @@
                 68 IMPORT_FROM             14 (set_workflow_name_from_context)
                 70 STORE_NAME              14 (set_workflow_name_from_context)
                 72 IMPORT_FROM             15 (set_prompt_attributes_from_context)
                 74 STORE_NAME              15 (set_prompt_attributes_from_context)
                 76 POP_TOP
    
     20          78 LOAD_CONST               0 (0)
-                80 LOAD_CONST               4 (('get_trace_context_from_carrier', 'get_carrier_from_trace_context'))
+                80 LOAD_CONST               4 (('get_trace_context_from_carrier', 'get_carrier_from_trace_context', 'extract_association_properties_from_http_headers'))
                 82 IMPORT_NAME             16 (agiflow.opentelemetry.context.context_propagation)
                 84 IMPORT_FROM             17 (get_trace_context_from_carrier)
                 86 STORE_NAME              17 (get_trace_context_from_carrier)
                 88 IMPORT_FROM             18 (get_carrier_from_trace_context)
                 90 STORE_NAME              18 (get_carrier_from_trace_context)
-                92 POP_TOP
+                92 IMPORT_FROM             19 (extract_association_properties_from_http_headers)
+                94 STORE_NAME              19 (extract_association_properties_from_http_headers)
+                96 POP_TOP
    
-    25          94 BUILD_LIST               0
-                96 LOAD_CONST               5 (('ContextKeys', 'PromptSettings', 'AssociationProperties', 'set_association_properties', 'set_workflow_name', 'set_prompt_settings_context', 'set_override_enable_context_tracing', 'get_workflow_name', 'get_correlation_id', 'get_association_properties', 'get_prompt_settings', 'set_workflow_name_from_context', 'set_prompt_attributes_from_context', 'get_trace_context_from_carrier', 'get_carrier_from_trace_context'))
-                98 LIST_EXTEND              1
-               100 STORE_NAME              19 (__all__)
-               102 LOAD_CONST               6 (None)
-               104 RETURN_VALUE
+    26          98 BUILD_LIST               0
+               100 LOAD_CONST               5 (('ContextKeys', 'PromptSettings', 'AssociationProperties', 'set_association_properties', 'set_workflow_name', 'set_prompt_settings_context', 'set_override_enable_context_tracing', 'get_workflow_name', 'get_correlation_id', 'get_association_properties', 'get_prompt_settings', 'set_workflow_name_from_context', 'set_prompt_attributes_from_context', 'get_trace_context_from_carrier', 'get_carrier_from_trace_context', 'extract_association_properties_from_http_headers'))
+               102 LIST_EXTEND              1
+               104 STORE_NAME              20 (__all__)
+               106 LOAD_CONST               6 (None)
+               108 RETURN_VALUE
    consts
       0
       ('ContextKeys', 'PromptSettings', 'AssociationProperties')
       ('set_association_properties', 'set_workflow_name', 'set_prompt_settings_context', 'set_override_enable_context_tracing', 'get_workflow_name', 'get_correlation_id', 'get_association_properties', 'get_prompt_settings')
       ('set_workflow_name_from_context', 'set_prompt_attributes_from_context')
-      ('get_trace_context_from_carrier', 'get_carrier_from_trace_context')
-      ('ContextKeys', 'PromptSettings', 'AssociationProperties', 'set_association_properties', 'set_workflow_name', 'set_prompt_settings_context', 'set_override_enable_context_tracing', 'get_workflow_name', 'get_correlation_id', 'get_association_properties', 'get_prompt_settings', 'set_workflow_name_from_context', 'set_prompt_attributes_from_context', 'get_trace_context_from_carrier', 'get_carrier_from_trace_context')
+      ('get_trace_context_from_carrier', 'get_carrier_from_trace_context', 'extract_association_properties_from_http_headers')
+      ('ContextKeys', 'PromptSettings', 'AssociationProperties', 'set_association_properties', 'set_workflow_name', 'set_prompt_settings_context', 'set_override_enable_context_tracing', 'get_workflow_name', 'get_correlation_id', 'get_association_properties', 'get_prompt_settings', 'set_workflow_name_from_context', 'set_prompt_attributes_from_context', 'get_trace_context_from_carrier', 'get_carrier_from_trace_context', 'extract_association_properties_from_http_headers')
       None
-   names      ('agiflow.opentelemetry.context.constants', 'ContextKeys', 'PromptSettings', 'AssociationProperties', 'agiflow.opentelemetry.context.context', 'set_association_properties', 'set_workflow_name', 'set_prompt_settings_context', 'set_override_enable_context_tracing', 'get_workflow_name', 'get_correlation_id', 'get_association_properties', 'get_prompt_settings', 'agiflow.opentelemetry.context.span_from_context', 'set_workflow_name_from_context', 'set_prompt_attributes_from_context', 'agiflow.opentelemetry.context.context_propagation', 'get_trace_context_from_carrier', 'get_carrier_from_trace_context', '__all__')
+   names      ('agiflow.opentelemetry.context.constants', 'ContextKeys', 'PromptSettings', 'AssociationProperties', 'agiflow.opentelemetry.context.context', 'set_association_properties', 'set_workflow_name', 'set_prompt_settings_context', 'set_override_enable_context_tracing', 'get_workflow_name', 'get_correlation_id', 'get_association_properties', 'get_prompt_settings', 'agiflow.opentelemetry.context.span_from_context', 'set_workflow_name_from_context', 'set_prompt_attributes_from_context', 'agiflow.opentelemetry.context.context_propagation', 'get_trace_context_from_carrier', 'get_carrier_from_trace_context', 'extract_association_properties_from_http_headers', '__all__')
    varnames   ()
    freevars   ()
    cellvars   ()
    filename   '/Users/vuongngo/workspace/agiflow/packages/python/agiflow-sdk/agiflow/opentelemetry/context/__init__.py'
    name       '<module>'
    firstlineno 1
-   lnotab 0x00ff02011405280a10041005
+   lnotab 0x00ff02011405280a10041406
```

### Comparing `agiflow_sdk-0.0.3/agiflow/opentelemetry/context/__pycache__/constants.cpython-311.pyc` & `agiflow_sdk-0.0.4/agiflow/opentelemetry/context/__pycache__/constants.cpython-311.pyc`

 * *Files 24% similar despite different names*

#### Python bytecode

```diff
@@ -1,10 +1,10 @@
 magic:    0xa70d0d0a
-moddate:  0x43985a66 (Sat Jun  1 03:40:51 2024 UTC)
-files sz: 673
+moddate:  0x6a425c66 (Sun Jun  2 09:59:06 2024 UTC)
+files sz: 740
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 5
    flags     : 0
    code
       0x9700640064016c006d015a016d025a0201000200470064028400640365
@@ -38,17 +38,17 @@
                 52 MAKE_FUNCTION            0
                 54 LOAD_CONST               5 ('AssociationProperties')
                 56 LOAD_NAME                1 (TypedDict)
                 58 PRECALL                  3
                 62 CALL                     3
                 72 STORE_NAME               4 (AssociationProperties)
    
-    18          74 PUSH_NULL
+    20          74 PUSH_NULL
                 76 LOAD_BUILD_CLASS
-                78 LOAD_CONST               6 (<code object ContextKeys, file "/Users/vuongngo/workspace/agiflow/packages/python/agiflow-sdk/agiflow/opentelemetry/context/constants.py", line 18>)
+                78 LOAD_CONST               6 (<code object ContextKeys, file "/Users/vuongngo/workspace/agiflow/packages/python/agiflow-sdk/agiflow/opentelemetry/context/constants.py", line 20>)
                 80 MAKE_FUNCTION            0
                 82 LOAD_CONST               7 ('ContextKeys')
                 84 PRECALL                  2
                 88 CALL                     2
                 98 STORE_NAME               5 (ContextKeys)
                100 LOAD_CONST               8 (None)
                102 RETURN_VALUE
@@ -130,15 +130,17 @@
          argcount  : 0
          nlocals   : 0
          stacksize : 3
          flags     : 0
          code
             0x970065005a0164005a0255006503650419000000000000000000650564
             013c0000006503650419000000000000000000650564023c000000650365
-            0419000000000000000000650564033c00000064045300
+            0419000000000000000000650564033c0000006503650419000000000000
+            000000650564043c0000006503650619000000000000000000650564053c
+            00000064065300
           12           0 RESUME                   0
                        2 LOAD_NAME                0 (__name__)
                        4 STORE_NAME               1 (__module__)
                        6 LOAD_CONST               0 ('AssociationProperties')
                        8 STORE_NAME               2 (__qualname__)
                       10 SETUP_ANNOTATIONS
          
@@ -158,58 +160,74 @@
          
           15          56 LOAD_NAME                3 (NotRequired)
                       58 LOAD_NAME                4 (str)
                       60 BINARY_SUBSCR
                       70 LOAD_NAME                5 (__annotations__)
                       72 LOAD_CONST               3 ('user_id')
                       74 STORE_SUBSCR
-                      78 LOAD_CONST               4 (None)
-                      80 RETURN_VALUE
+         
+          16          78 LOAD_NAME                3 (NotRequired)
+                      80 LOAD_NAME                4 (str)
+                      82 BINARY_SUBSCR
+                      92 LOAD_NAME                5 (__annotations__)
+                      94 LOAD_CONST               4 ('session_id')
+                      96 STORE_SUBSCR
+         
+          17         100 LOAD_NAME                3 (NotRequired)
+                     102 LOAD_NAME                6 (bool)
+                     104 BINARY_SUBSCR
+                     114 LOAD_NAME                5 (__annotations__)
+                     116 LOAD_CONST               5 ('auto_trace')
+                     118 STORE_SUBSCR
+                     122 LOAD_CONST               6 (None)
+                     124 RETURN_VALUE
          consts
             'AssociationProperties'
             'action_id'
             'task_id'
             'user_id'
+            'session_id'
+            'auto_trace'
             None
-         names      ('__name__', '__module__', '__qualname__', 'NotRequired', 'str', '__annotations__')
+         names      ('__name__', '__module__', '__qualname__', 'NotRequired', 'str', '__annotations__', 'bool')
          varnames   ()
          freevars   ()
          cellvars   ()
          filename   '/Users/vuongngo/workspace/agiflow/packages/python/agiflow-sdk/agiflow/opentelemetry/context/constants.py'
          name       'AssociationProperties'
          firstlineno 12
-         lnotab 0x0c0116011601
+         lnotab 0x0c011601160116011601
       'AssociationProperties'
       code
          argcount  : 0
          nlocals   : 0
          stacksize : 1
          flags     : 0
          code
             0x970065005a0164005a0264015a0364025a0464035a0564045a0664055a
             0764065300
-          18           0 RESUME                   0
+          20           0 RESUME                   0
                        2 LOAD_NAME                0 (__name__)
                        4 STORE_NAME               1 (__module__)
                        6 LOAD_CONST               0 ('ContextKeys')
                        8 STORE_NAME               2 (__qualname__)
          
-          19          10 LOAD_CONST               1 ('correlation_id')
+          21          10 LOAD_CONST               1 ('correlation_id')
                       12 STORE_NAME               3 (CORRELATION_ID)
          
-          20          14 LOAD_CONST               2 ('association_properties')
+          22          14 LOAD_CONST               2 ('association_properties')
                       16 STORE_NAME               4 (ASSOCIATION_PROPERTIES)
          
-          21          18 LOAD_CONST               3 ('workflow_name')
+          23          18 LOAD_CONST               3 ('workflow_name')
                       20 STORE_NAME               5 (WORKFLOW_NAME)
          
-          23          22 LOAD_CONST               4 ('prompt_settings')
+          25          22 LOAD_CONST               4 ('prompt_settings')
                       24 STORE_NAME               6 (PROMPT_SETTINGS)
          
-          26          26 LOAD_CONST               5 ('override_enable_content_tracing')
+          28          26 LOAD_CONST               5 ('override_enable_content_tracing')
                       28 STORE_NAME               7 (OVERRIDE_ENABLE_CONTENT_TRACING)
                       30 LOAD_CONST               6 (None)
                       32 RETURN_VALUE
          consts
             'ContextKeys'
             'correlation_id'
             'association_properties'
@@ -219,19 +237,19 @@
             None
          names      ('__name__', '__module__', '__qualname__', 'CORRELATION_ID', 'ASSOCIATION_PROPERTIES', 'WORKFLOW_NAME', 'PROMPT_SETTINGS', 'OVERRIDE_ENABLE_CONTENT_TRACING')
          varnames   ()
          freevars   ()
          cellvars   ()
          filename   '/Users/vuongngo/workspace/agiflow/packages/python/agiflow-sdk/agiflow/opentelemetry/context/constants.py'
          name       'ContextKeys'
-         firstlineno 18
+         firstlineno 20
          lnotab 0x0a010401040104020403
       'ContextKeys'
       None
    names      ('typing', 'TypedDict', 'NotRequired', 'PromptSettings', 'AssociationProperties', 'ContextKeys')
    varnames   ()
    freevars   ()
    cellvars   ()
    filename   '/Users/vuongngo/workspace/agiflow/packages/python/agiflow-sdk/agiflow/opentelemetry/context/constants.py'
    name       '<module>'
    firstlineno 1
-   lnotab 0x00ff020110031c081c06
+   lnotab 0x00ff020110031c081c08
```

### Comparing `agiflow_sdk-0.0.3/agiflow/opentelemetry/context/__pycache__/context.cpython-311.pyc` & `agiflow_sdk-0.0.4/agiflow/opentelemetry/context/__pycache__/context.cpython-311.pyc`

 * *Files 1% similar despite different names*

#### Python bytecode

```diff
@@ -1,9 +1,9 @@
 magic:    0xa70d0d0a
-moddate:  0x950c5b66 (Sat Jun  1 11:57:09 2024 UTC)
+moddate:  0x47d85b66 (Sun Jun  2 02:26:15 2024 UTC)
 files sz: 1231
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 4
    flags     : 0
    code
```

### Comparing `agiflow_sdk-0.0.3/agiflow/opentelemetry/context/__pycache__/context_propagation.cpython-311.pyc` & `agiflow_sdk-0.0.4/agiflow/opentelemetry/context/__pycache__/context_propagation.cpython-311.pyc`

 * *Files 16% similar despite different names*

#### Python bytecode

```diff
@@ -1,54 +1,70 @@
 magic:    0xa70d0d0a
-moddate:  0x84ae5b66 (Sat Jun  1 23:28:04 2024 UTC)
-files sz: 1644
+moddate:  0x6a425c66 (Sun Jun  2 09:59:06 2024 UTC)
+files sz: 2139
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 2
    flags     : 0
    code
-      0x9700640064016c006d015a010100640064026c026d035a036d045a0401
-      00640064036c056d065a060100640484005a07640584005a0864065300
+      0x9700640064016c006d015a010100640064026c026d035a030100640064
+      036c046d055a056d065a060100640064046c076d085a080100640584005a
+      09640684005a0a640765016602640884045a0b64095300
      0           0 RESUME                   0
    
      1           2 LOAD_CONST               0 (0)
-                 4 LOAD_CONST               1 (('TraceContextTextMapPropagator',))
-                 6 IMPORT_NAME              0 (opentelemetry.trace.propagation.tracecontext)
-                 8 IMPORT_FROM              1 (TraceContextTextMapPropagator)
-                10 STORE_NAME               1 (TraceContextTextMapPropagator)
+                 4 LOAD_CONST               1 (('Any',))
+                 6 IMPORT_NAME              0 (typing)
+                 8 IMPORT_FROM              1 (Any)
+                10 STORE_NAME               1 (Any)
                 12 POP_TOP
    
      2          14 LOAD_CONST               0 (0)
-                16 LOAD_CONST               2 (('get_current', 'set_value'))
-                18 IMPORT_NAME              2 (opentelemetry.context)
-                20 IMPORT_FROM              3 (get_current)
-                22 STORE_NAME               3 (get_current)
-                24 IMPORT_FROM              4 (set_value)
-                26 STORE_NAME               4 (set_value)
-                28 POP_TOP
+                16 LOAD_CONST               2 (('TraceContextTextMapPropagator',))
+                18 IMPORT_NAME              2 (opentelemetry.trace.propagation.tracecontext)
+                20 IMPORT_FROM              3 (TraceContextTextMapPropagator)
+                22 STORE_NAME               3 (TraceContextTextMapPropagator)
+                24 POP_TOP
    
-     3          30 LOAD_CONST               0 (0)
-                32 LOAD_CONST               3 (('ContextKeys',))
-                34 IMPORT_NAME              5 (agiflow.opentelemetry.context)
-                36 IMPORT_FROM              6 (ContextKeys)
-                38 STORE_NAME               6 (ContextKeys)
+     3          26 LOAD_CONST               0 (0)
+                28 LOAD_CONST               3 (('get_current', 'set_value'))
+                30 IMPORT_NAME              4 (opentelemetry.context)
+                32 IMPORT_FROM              5 (get_current)
+                34 STORE_NAME               5 (get_current)
+                36 IMPORT_FROM              6 (set_value)
+                38 STORE_NAME               6 (set_value)
                 40 POP_TOP
    
-     6          42 LOAD_CONST               4 (<code object get_carrier_from_trace_context, file "/Users/vuongngo/workspace/agiflow/packages/python/agiflow-sdk/agiflow/opentelemetry/context/context_propagation.py", line 6>)
-                44 MAKE_FUNCTION            0
-                46 STORE_NAME               7 (get_carrier_from_trace_context)
+     4          42 LOAD_CONST               0 (0)
+                44 LOAD_CONST               4 (('ContextKeys',))
+                46 IMPORT_NAME              7 (agiflow.opentelemetry.context.constants)
+                48 IMPORT_FROM              8 (ContextKeys)
+                50 STORE_NAME               8 (ContextKeys)
+                52 POP_TOP
    
-    17          48 LOAD_CONST               5 (<code object get_trace_context_from_carrier, file "/Users/vuongngo/workspace/agiflow/packages/python/agiflow-sdk/agiflow/opentelemetry/context/context_propagation.py", line 17>)
-                50 MAKE_FUNCTION            0
-                52 STORE_NAME               8 (get_trace_context_from_carrier)
-                54 LOAD_CONST               6 (None)
-                56 RETURN_VALUE
+     7          54 LOAD_CONST               5 (<code object get_carrier_from_trace_context, file "/Users/vuongngo/workspace/agiflow/packages/python/agiflow-sdk/agiflow/opentelemetry/context/context_propagation.py", line 7>)
+                56 MAKE_FUNCTION            0
+                58 STORE_NAME               9 (get_carrier_from_trace_context)
+   
+    18          60 LOAD_CONST               6 (<code object get_trace_context_from_carrier, file "/Users/vuongngo/workspace/agiflow/packages/python/agiflow-sdk/agiflow/opentelemetry/context/context_propagation.py", line 18>)
+                62 MAKE_FUNCTION            0
+                64 STORE_NAME              10 (get_trace_context_from_carrier)
+   
+    36          66 LOAD_CONST               7 ('headers')
+                68 LOAD_NAME                1 (Any)
+                70 BUILD_TUPLE              2
+                72 LOAD_CONST               8 (<code object extract_association_properties_from_http_headers, file "/Users/vuongngo/workspace/agiflow/packages/python/agiflow-sdk/agiflow/opentelemetry/context/context_propagation.py", line 36>)
+                74 MAKE_FUNCTION            4 (annotations)
+                76 STORE_NAME              11 (extract_association_properties_from_http_headers)
+                78 LOAD_CONST               9 (None)
+                80 RETURN_VALUE
    consts
       0
+      ('Any',)
       ('TraceContextTextMapPropagator',)
       ('get_current', 'set_value')
       ('ContextKeys',)
       code
          argcount  : 0
          nlocals   : 2
          stacksize : 4
@@ -66,92 +82,92 @@
             000000000000003c0000007c01a003000000000000000000000000000000
             00000000007408000000000000000000006a0700000000000000006900a6
             020000ab0200000000000000007c007408000000000000000000006a0700
             000000000000003c0000007c01a003000000000000000000000000000000
             00000000007408000000000000000000006a0800000000000000006900a6
             020000ab0200000000000000007c007408000000000000000000006a0800
             000000000000003c0000007c005300
-           6           0 RESUME                   0
+           7           0 RESUME                   0
          
-           7           2 BUILD_MAP                0
+           8           2 BUILD_MAP                0
                        4 STORE_FAST               0 (carrier)
          
-           8           6 LOAD_GLOBAL              1 (NULL + get_current)
+           9           6 LOAD_GLOBAL              1 (NULL + get_current)
                       18 PRECALL                  0
                       22 CALL                     0
                       32 STORE_FAST               1 (context)
          
-           9          34 LOAD_GLOBAL              3 (NULL + TraceContextTextMapPropagator)
+          10          34 LOAD_GLOBAL              3 (NULL + TraceContextTextMapPropagator)
                       46 PRECALL                  0
                       50 CALL                     0
                       60 LOAD_METHOD              2 (inject)
                       82 LOAD_FAST                0 (carrier)
                       84 PRECALL                  1
                       88 CALL                     1
                       98 POP_TOP
          
-          10         100 LOAD_FAST                1 (context)
+          11         100 LOAD_FAST                1 (context)
                      102 LOAD_METHOD              3 (get)
                      124 LOAD_GLOBAL              8 (ContextKeys)
                      136 LOAD_ATTR                5 (ASSOCIATION_PROPERTIES)
                      146 BUILD_MAP                0
                      148 PRECALL                  2
                      152 CALL                     2
                      162 LOAD_FAST                0 (carrier)
                      164 LOAD_GLOBAL              8 (ContextKeys)
                      176 LOAD_ATTR                5 (ASSOCIATION_PROPERTIES)
                      186 STORE_SUBSCR
          
-          11         190 LOAD_FAST                1 (context)
+          12         190 LOAD_FAST                1 (context)
                      192 LOAD_METHOD              3 (get)
                      214 LOAD_GLOBAL              8 (ContextKeys)
                      226 LOAD_ATTR                6 (PROMPT_SETTINGS)
                      236 BUILD_MAP                0
                      238 PRECALL                  2
                      242 CALL                     2
                      252 LOAD_FAST                0 (carrier)
                      254 LOAD_GLOBAL              8 (ContextKeys)
                      266 LOAD_ATTR                6 (PROMPT_SETTINGS)
                      276 STORE_SUBSCR
          
-          12         280 LOAD_FAST                1 (context)
+          13         280 LOAD_FAST                1 (context)
                      282 LOAD_METHOD              3 (get)
                      304 LOAD_GLOBAL              8 (ContextKeys)
                      316 LOAD_ATTR                7 (WORKFLOW_NAME)
                      326 BUILD_MAP                0
                      328 PRECALL                  2
                      332 CALL                     2
                      342 LOAD_FAST                0 (carrier)
                      344 LOAD_GLOBAL              8 (ContextKeys)
                      356 LOAD_ATTR                7 (WORKFLOW_NAME)
                      366 STORE_SUBSCR
          
-          13         370 LOAD_FAST                1 (context)
+          14         370 LOAD_FAST                1 (context)
                      372 LOAD_METHOD              3 (get)
                      394 LOAD_GLOBAL              8 (ContextKeys)
                      406 LOAD_ATTR                8 (OVERRIDE_ENABLE_CONTENT_TRACING)
                      416 BUILD_MAP                0
                      418 PRECALL                  2
                      422 CALL                     2
                      432 LOAD_FAST                0 (carrier)
                      434 LOAD_GLOBAL              8 (ContextKeys)
                      446 LOAD_ATTR                8 (OVERRIDE_ENABLE_CONTENT_TRACING)
                      456 STORE_SUBSCR
          
-          14         460 LOAD_FAST                0 (carrier)
+          15         460 LOAD_FAST                0 (carrier)
                      462 RETURN_VALUE
          consts
             None
          names      ('get_current', 'TraceContextTextMapPropagator', 'inject', 'get', 'ContextKeys', 'ASSOCIATION_PROPERTIES', 'PROMPT_SETTINGS', 'WORKFLOW_NAME', 'OVERRIDE_ENABLE_CONTENT_TRACING')
          varnames   ('carrier', 'context')
          freevars   ()
          cellvars   ()
          filename   '/Users/vuongngo/workspace/agiflow/packages/python/agiflow-sdk/agiflow/opentelemetry/context/context_propagation.py'
          name       'get_carrier_from_trace_context'
-         firstlineno 6
+         firstlineno 7
          lnotab 0x020104011c0142015a015a015a015a01
       code
          argcount  : 1
          nlocals   : 2
          stacksize : 6
          flags     : 3
          code
@@ -177,137 +193,222 @@
             0100000000000000007c01a6030000ab0300000000000000007d017c00a0
             020000000000000000000000000000000000000000740600000000000000
             0000006a080000000000000000a6010000ab010000000000000000723874
             0b000000000000000000007406000000000000000000006a080000000000
             0000007c00a0020000000000000000000000000000000000000000740600
             0000000000000000006a080000000000000000a6010000ab010000000000
             0000007c01a6030000ab0300000000000000007d017c015300
-          17           0 RESUME                   0
+          18           0 RESUME                   0
          
-          18           2 LOAD_GLOBAL              1 (NULL + TraceContextTextMapPropagator)
+          19           2 LOAD_GLOBAL              1 (NULL + TraceContextTextMapPropagator)
                       14 PRECALL                  0
                       18 CALL                     0
                       28 LOAD_METHOD              1 (extract)
                       50 LOAD_FAST                0 (carrier)
                       52 PRECALL                  1
                       56 CALL                     1
                       66 STORE_FAST               1 (ctx)
          
-          19          68 LOAD_FAST                0 (carrier)
+          20          68 LOAD_FAST                0 (carrier)
                       70 EXTENDED_ARG             1
                       72 POP_JUMP_FORWARD_IF_NONE   348 (to 770)
          
-          20          74 LOAD_FAST                0 (carrier)
+          21          74 LOAD_FAST                0 (carrier)
                       76 LOAD_METHOD              2 (get)
                       98 LOAD_GLOBAL              6 (ContextKeys)
                      110 LOAD_ATTR                4 (ASSOCIATION_PROPERTIES)
                      120 PRECALL                  1
                      124 CALL                     1
                      134 POP_JUMP_FORWARD_IF_FALSE    56 (to 248)
          
-          21         136 LOAD_GLOBAL             11 (NULL + set_value)
+          22         136 LOAD_GLOBAL             11 (NULL + set_value)
                      148 LOAD_GLOBAL              6 (ContextKeys)
                      160 LOAD_ATTR                4 (ASSOCIATION_PROPERTIES)
                      170 LOAD_FAST                0 (carrier)
                      172 LOAD_METHOD              2 (get)
                      194 LOAD_GLOBAL              6 (ContextKeys)
                      206 LOAD_ATTR                4 (ASSOCIATION_PROPERTIES)
                      216 PRECALL                  1
                      220 CALL                     1
                      230 LOAD_FAST                1 (ctx)
                      232 PRECALL                  3
                      236 CALL                     3
                      246 STORE_FAST               1 (ctx)
          
-          22     >>  248 LOAD_FAST                0 (carrier)
+          23     >>  248 LOAD_FAST                0 (carrier)
                      250 LOAD_METHOD              2 (get)
                      272 LOAD_GLOBAL              6 (ContextKeys)
                      284 LOAD_ATTR                6 (PROMPT_SETTINGS)
                      294 PRECALL                  1
                      298 CALL                     1
                      308 POP_JUMP_FORWARD_IF_FALSE    56 (to 422)
          
-          23         310 LOAD_GLOBAL             11 (NULL + set_value)
+          24         310 LOAD_GLOBAL             11 (NULL + set_value)
                      322 LOAD_GLOBAL              6 (ContextKeys)
                      334 LOAD_ATTR                6 (PROMPT_SETTINGS)
                      344 LOAD_FAST                0 (carrier)
                      346 LOAD_METHOD              2 (get)
                      368 LOAD_GLOBAL              6 (ContextKeys)
                      380 LOAD_ATTR                6 (PROMPT_SETTINGS)
                      390 PRECALL                  1
                      394 CALL                     1
                      404 LOAD_FAST                1 (ctx)
                      406 PRECALL                  3
                      410 CALL                     3
                      420 STORE_FAST               1 (ctx)
          
-          24     >>  422 LOAD_FAST                0 (carrier)
+          25     >>  422 LOAD_FAST                0 (carrier)
                      424 LOAD_METHOD              2 (get)
                      446 LOAD_GLOBAL              6 (ContextKeys)
                      458 LOAD_ATTR                7 (WORKFLOW_NAME)
                      468 PRECALL                  1
                      472 CALL                     1
                      482 POP_JUMP_FORWARD_IF_FALSE    56 (to 596)
          
-          25         484 LOAD_GLOBAL             11 (NULL + set_value)
+          26         484 LOAD_GLOBAL             11 (NULL + set_value)
                      496 LOAD_GLOBAL              6 (ContextKeys)
                      508 LOAD_ATTR                7 (WORKFLOW_NAME)
                      518 LOAD_FAST                0 (carrier)
                      520 LOAD_METHOD              2 (get)
                      542 LOAD_GLOBAL              6 (ContextKeys)
                      554 LOAD_ATTR                7 (WORKFLOW_NAME)
                      564 PRECALL                  1
                      568 CALL                     1
                      578 LOAD_FAST                1 (ctx)
                      580 PRECALL                  3
                      584 CALL                     3
                      594 STORE_FAST               1 (ctx)
          
-          26     >>  596 LOAD_FAST                0 (carrier)
+          27     >>  596 LOAD_FAST                0 (carrier)
                      598 LOAD_METHOD              2 (get)
                      620 LOAD_GLOBAL              6 (ContextKeys)
                      632 LOAD_ATTR                8 (OVERRIDE_ENABLE_CONTENT_TRACING)
                      642 PRECALL                  1
                      646 CALL                     1
                      656 POP_JUMP_FORWARD_IF_FALSE    56 (to 770)
          
-          27         658 LOAD_GLOBAL             11 (NULL + set_value)
+          28         658 LOAD_GLOBAL             11 (NULL + set_value)
          
-          28         670 LOAD_GLOBAL              6 (ContextKeys)
+          29         670 LOAD_GLOBAL              6 (ContextKeys)
                      682 LOAD_ATTR                8 (OVERRIDE_ENABLE_CONTENT_TRACING)
          
-          29         692 LOAD_FAST                0 (carrier)
+          30         692 LOAD_FAST                0 (carrier)
                      694 LOAD_METHOD              2 (get)
                      716 LOAD_GLOBAL              6 (ContextKeys)
                      728 LOAD_ATTR                8 (OVERRIDE_ENABLE_CONTENT_TRACING)
                      738 PRECALL                  1
                      742 CALL                     1
          
-          30         752 LOAD_FAST                1 (ctx)
+          31         752 LOAD_FAST                1 (ctx)
          
-          27         754 PRECALL                  3
+          28         754 PRECALL                  3
                      758 CALL                     3
                      768 STORE_FAST               1 (ctx)
          
-          32     >>  770 LOAD_FAST                1 (ctx)
+          33     >>  770 LOAD_FAST                1 (ctx)
                      772 RETURN_VALUE
          consts
             None
          names      ('TraceContextTextMapPropagator', 'extract', 'get', 'ContextKeys', 'ASSOCIATION_PROPERTIES', 'set_value', 'PROMPT_SETTINGS', 'WORKFLOW_NAME', 'OVERRIDE_ENABLE_CONTENT_TRACING')
          varnames   ('carrier', 'ctx')
          freevars   ()
          cellvars   ()
          filename   '/Users/vuongngo/workspace/agiflow/packages/python/agiflow-sdk/agiflow/opentelemetry/context/context_propagation.py'
          name       'get_trace_context_from_carrier'
-         firstlineno 17
+         firstlineno 18
          lnotab
             0x0201420106013e0170013e0170013e0170013e010c0116013c0102fd10
             05
+      'headers'
+      code
+         argcount  : 1
+         nlocals   : 4
+         stacksize : 4
+         flags     : 3
+         code
+            0x97007401000000000000000000007c006401a6020000ab020000000000
+            000000724269007d017c00a0010000000000000000000000000000000000
+            0000006402a6010000ab0100000000000000007d027c00a0010000000000
+            0000000000000000000000000000006403a6010000ab0100000000000000
+            007d037c0281057c027c0164043c0000007c03810f7c0364056b02000000
+            00720b64067c0164073c00000064005300640053006400530064005300
+          36           0 RESUME                   0
+         
+          37           2 LOAD_GLOBAL              1 (NULL + hasattr)
+                      14 LOAD_FAST                0 (headers)
+                      16 LOAD_CONST               1 ('get')
+                      18 PRECALL                  2
+                      22 CALL                     2
+                      32 POP_JUMP_FORWARD_IF_FALSE    66 (to 166)
+         
+          38          34 BUILD_MAP                0
+                      36 STORE_FAST               1 (association_properties)
+         
+          39          38 LOAD_FAST                0 (headers)
+                      40 LOAD_METHOD              1 (get)
+                      62 LOAD_CONST               2 ('x-agiflow-action-id')
+                      64 PRECALL                  1
+                      68 CALL                     1
+                      78 STORE_FAST               2 (action_id)
+         
+          40          80 LOAD_FAST                0 (headers)
+                      82 LOAD_METHOD              1 (get)
+                     104 LOAD_CONST               3 ('x-agiflow-auto-trace')
+                     106 PRECALL                  1
+                     110 CALL                     1
+                     120 STORE_FAST               3 (auto_trace)
+         
+          42         122 LOAD_FAST                2 (action_id)
+                     124 POP_JUMP_FORWARD_IF_NONE     5 (to 136)
+         
+          43         126 LOAD_FAST                2 (action_id)
+                     128 LOAD_FAST                1 (association_properties)
+                     130 LOAD_CONST               4 ('action_id')
+                     132 STORE_SUBSCR
+         
+          45     >>  136 LOAD_FAST                3 (auto_trace)
+                     138 POP_JUMP_FORWARD_IF_NONE    15 (to 170)
+                     140 LOAD_FAST                3 (auto_trace)
+                     142 LOAD_CONST               5 ('true')
+                     144 COMPARE_OP               2 (==)
+                     150 POP_JUMP_FORWARD_IF_FALSE    11 (to 174)
+         
+          46         152 LOAD_CONST               6 (True)
+                     154 LOAD_FAST                1 (association_properties)
+                     156 LOAD_CONST               7 ('auto_trace')
+                     158 STORE_SUBSCR
+                     162 LOAD_CONST               0 (None)
+                     164 RETURN_VALUE
+         
+          37     >>  166 LOAD_CONST               0 (None)
+                     168 RETURN_VALUE
+         
+          45     >>  170 LOAD_CONST               0 (None)
+                     172 RETURN_VALUE
+                 >>  174 LOAD_CONST               0 (None)
+                     176 RETURN_VALUE
+         consts
+            None
+            'get'
+            'x-agiflow-action-id'
+            'x-agiflow-auto-trace'
+            'action_id'
+            'true'
+            True
+            'auto_trace'
+         names      ('hasattr', 'get')
+         varnames   ('headers', 'association_properties', 'action_id', 'auto_trace')
+         freevars   ()
+         cellvars   ()
+         filename   '/Users/vuongngo/workspace/agiflow/packages/python/agiflow-sdk/agiflow/opentelemetry/context/context_propagation.py'
+         name       'extract_association_properties_from_http_headers'
+         firstlineno 36
+         lnotab 0x0201200104012a012a0204010a0210010ef70408
       None
-   names      ('opentelemetry.trace.propagation.tracecontext', 'TraceContextTextMapPropagator', 'opentelemetry.context', 'get_current', 'set_value', 'agiflow.opentelemetry.context', 'ContextKeys', 'get_carrier_from_trace_context', 'get_trace_context_from_carrier')
+   names      ('typing', 'Any', 'opentelemetry.trace.propagation.tracecontext', 'TraceContextTextMapPropagator', 'opentelemetry.context', 'get_current', 'set_value', 'agiflow.opentelemetry.context.constants', 'ContextKeys', 'get_carrier_from_trace_context', 'get_trace_context_from_carrier', 'extract_association_properties_from_http_headers')
    varnames   ()
    freevars   ()
    cellvars   ()
    filename   '/Users/vuongngo/workspace/agiflow/packages/python/agiflow-sdk/agiflow/opentelemetry/context/context_propagation.py'
    name       '<module>'
    firstlineno 1
-   lnotab 0x00ff02010c0110010c03060b
+   lnotab 0x00ff02010c010c0110010c03060b0612
```

### Comparing `agiflow_sdk-0.0.3/agiflow/opentelemetry/context/__pycache__/set_span_from_context.cpython-311.pyc` & `agiflow_sdk-0.0.4/agiflow/opentelemetry/context/__pycache__/set_span_from_context.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `agiflow_sdk-0.0.3/agiflow/opentelemetry/context/__pycache__/span_from_context.cpython-311.pyc` & `agiflow_sdk-0.0.4/agiflow/opentelemetry/context/__pycache__/span_from_context.cpython-311.pyc`

 * *Files 6% similar despite different names*

#### Python bytecode

```diff
@@ -1,9 +1,9 @@
 magic:    0xa70d0d0a
-moddate:  0x6c095b66 (Sat Jun  1 11:43:40 2024 UTC)
+moddate:  0x47d85b66 (Sun Jun  2 02:26:15 2024 UTC)
 files sz: 1285
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 4
    flags     : 0
    code
```

### Comparing `agiflow_sdk-0.0.3/agiflow/opentelemetry/context/constants.py` & `agiflow_sdk-0.0.4/agiflow/opentelemetry/context/constants.py`

 * *Files 24% similar despite different names*

```diff
@@ -9,14 +9,16 @@
     template_variables: NotRequired[dict]
 
 
 class AssociationProperties(TypedDict):
     action_id: NotRequired[str]
     task_id: NotRequired[str]
     user_id: NotRequired[str]
+    session_id: NotRequired[str]
+    auto_trace: NotRequired[bool]
 
 
 class ContextKeys:
     CORRELATION_ID = "correlation_id"
     ASSOCIATION_PROPERTIES = "association_properties"
     WORKFLOW_NAME = "workflow_name"
     # Prompts
```

### Comparing `agiflow_sdk-0.0.3/agiflow/opentelemetry/context/context.py` & `agiflow_sdk-0.0.4/agiflow/opentelemetry/context/context.py`

 * *Files identical despite different names*

### Comparing `agiflow_sdk-0.0.3/agiflow/opentelemetry/context/context_propagation.py` & `agiflow_sdk-0.0.4/agiflow/opentelemetry/context/context_propagation.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,11 @@
+from typing import Any
 from opentelemetry.trace.propagation.tracecontext import TraceContextTextMapPropagator
 from opentelemetry.context import get_current, set_value
-from agiflow.opentelemetry.context import ContextKeys
+from agiflow.opentelemetry.context.constants import ContextKeys
 
 
 def get_carrier_from_trace_context():
     carrier = {}
     context = get_current()
     TraceContextTextMapPropagator().inject(carrier)
     carrier[ContextKeys.ASSOCIATION_PROPERTIES] = context.get(ContextKeys.ASSOCIATION_PROPERTIES, {})
@@ -26,7 +27,20 @@
         if carrier.get(ContextKeys.OVERRIDE_ENABLE_CONTENT_TRACING):
             ctx = set_value(
               ContextKeys.OVERRIDE_ENABLE_CONTENT_TRACING,
               carrier.get(ContextKeys.OVERRIDE_ENABLE_CONTENT_TRACING),
               ctx
             )
     return ctx
+
+
+def extract_association_properties_from_http_headers(headers: Any):
+    if hasattr(headers, 'get'):
+        association_properties = {}
+        action_id = headers.get('x-agiflow-action-id')
+        auto_trace = headers.get('x-agiflow-auto-trace')
+
+        if action_id is not None:
+            association_properties['action_id'] = action_id
+
+        if auto_trace is not None and auto_trace == 'true':
+            association_properties['auto_trace'] = True
```

### Comparing `agiflow_sdk-0.0.3/agiflow/opentelemetry/context/span_from_context.py` & `agiflow_sdk-0.0.4/agiflow/opentelemetry/context/span_from_context.py`

 * *Files identical despite different names*

### Comparing `agiflow_sdk-0.0.3/agiflow/opentelemetry/convention/__init__.py` & `agiflow_sdk-0.0.4/agiflow/opentelemetry/convention/__init__.py`

 * *Files identical despite different names*

### Comparing `agiflow_sdk-0.0.3/agiflow/opentelemetry/convention/__pycache__/__init__.cpython-311.pyc` & `agiflow_sdk-0.0.4/agiflow/opentelemetry/convention/__pycache__/__init__.cpython-311.pyc`

 * *Files 2% similar despite different names*

#### Python bytecode

```diff
@@ -1,9 +1,9 @@
 magic:    0xa70d0d0a
-moddate:  0x4f935b66 (Sat Jun  1 21:31:59 2024 UTC)
+moddate:  0x47d85b66 (Sun Jun  2 02:26:15 2024 UTC)
 files sz: 1583
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 8
    flags     : 0
    code
```

### Comparing `agiflow_sdk-0.0.3/agiflow/opentelemetry/convention/__pycache__/agiflow_attributes.cpython-311.pyc` & `agiflow_sdk-0.0.4/agiflow/opentelemetry/convention/__pycache__/agiflow_attributes.cpython-311.pyc`

 * *Files 1% similar despite different names*

#### Python bytecode

```diff
@@ -1,9 +1,9 @@
 magic:    0xa70d0d0a
-moddate:  0x43985a66 (Sat Jun  1 03:40:51 2024 UTC)
+moddate:  0x47d85b66 (Sun Jun  2 02:26:15 2024 UTC)
 files sz: 2477
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 5
    flags     : 16777216
    code
```

### Comparing `agiflow_sdk-0.0.3/agiflow/opentelemetry/convention/__pycache__/constants.cpython-311.pyc` & `agiflow_sdk-0.0.4/agiflow/opentelemetry/convention/__pycache__/constants.cpython-311.pyc`

 * *Files 1% similar despite different names*

#### Python bytecode

```diff
@@ -1,9 +1,9 @@
 magic:    0xa70d0d0a
-moddate:  0x46d95a66 (Sat Jun  1 08:18:14 2024 UTC)
+moddate:  0x47d85b66 (Sun Jun  2 02:26:15 2024 UTC)
 files sz: 3893
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 6
    flags     : 0
    code
```

### Comparing `agiflow_sdk-0.0.3/agiflow/opentelemetry/convention/__pycache__/database_span_attributes.cpython-311.pyc` & `agiflow_sdk-0.0.4/agiflow/opentelemetry/convention/__pycache__/database_span_attributes.cpython-311.pyc`

 * *Files 5% similar despite different names*

#### Python bytecode

```diff
@@ -1,9 +1,9 @@
 magic:    0xa70d0d0a
-moddate:  0x7bd05a66 (Sat Jun  1 07:40:43 2024 UTC)
+moddate:  0x47d85b66 (Sun Jun  2 02:26:15 2024 UTC)
 files sz: 2279
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 5
    flags     : 16777216
    code
```

### Comparing `agiflow_sdk-0.0.3/agiflow/opentelemetry/convention/__pycache__/framework_span_attributes.cpython-311.pyc` & `agiflow_sdk-0.0.4/agiflow/opentelemetry/convention/__pycache__/framework_span_attributes.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `agiflow_sdk-0.0.3/agiflow/opentelemetry/convention/__pycache__/llm_span_attributes.cpython-311.pyc` & `agiflow_sdk-0.0.4/agiflow/opentelemetry/convention/__pycache__/llm_span_attributes.cpython-311.pyc`

 * *Files 2% similar despite different names*

#### Python bytecode

```diff
@@ -1,9 +1,9 @@
 magic:    0xa70d0d0a
-moddate:  0x43985a66 (Sat Jun  1 03:40:51 2024 UTC)
+moddate:  0x47d85b66 (Sun Jun  2 02:26:15 2024 UTC)
 files sz: 6050
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 5
    flags     : 16777216
    code
```

### Comparing `agiflow_sdk-0.0.3/agiflow/opentelemetry/convention/agiflow_attributes.py` & `agiflow_sdk-0.0.4/agiflow/opentelemetry/convention/agiflow_attributes.py`

 * *Files identical despite different names*

### Comparing `agiflow_sdk-0.0.3/agiflow/opentelemetry/convention/constants.py` & `agiflow_sdk-0.0.4/agiflow/opentelemetry/convention/constants.py`

 * *Files identical despite different names*

### Comparing `agiflow_sdk-0.0.3/agiflow/opentelemetry/convention/database_span_attributes.py` & `agiflow_sdk-0.0.4/agiflow/opentelemetry/convention/database_span_attributes.py`

 * *Files identical despite different names*

### Comparing `agiflow_sdk-0.0.3/agiflow/opentelemetry/convention/framework_span_attributes.py` & `agiflow_sdk-0.0.4/agiflow/opentelemetry/convention/framework_span_attributes.py`

 * *Files identical despite different names*

### Comparing `agiflow_sdk-0.0.3/agiflow/opentelemetry/convention/llm_span_attributes.py` & `agiflow_sdk-0.0.4/agiflow/opentelemetry/convention/llm_span_attributes.py`

 * *Files identical despite different names*

### Comparing `agiflow_sdk-0.0.3/agiflow/opentelemetry/instrumentation/__init__.py` & `agiflow_sdk-0.0.4/agiflow/opentelemetry/instrumentation/__init__.py`

 * *Files identical despite different names*

### Comparing `agiflow_sdk-0.0.3/agiflow/opentelemetry/instrumentation/__pycache__/__init__.cpython-311.pyc` & `agiflow_sdk-0.0.4/agiflow/opentelemetry/instrumentation/__pycache__/__init__.cpython-311.pyc`

 * *Files 1% similar despite different names*

#### Python bytecode

```diff
@@ -1,9 +1,9 @@
 magic:    0xa70d0d0a
-moddate:  0x8a935b66 (Sat Jun  1 21:32:58 2024 UTC)
+moddate:  0x47d85b66 (Sun Jun  2 02:26:15 2024 UTC)
 files sz: 10305
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 26
    flags     : 0
    code
```

### Comparing `agiflow_sdk-0.0.3/agiflow/opentelemetry/instrumentation/anthropic/__pycache__/instrumentation.cpython-311.pyc` & `agiflow_sdk-0.0.4/agiflow/opentelemetry/instrumentation/anthropic/__pycache__/instrumentation.cpython-311.pyc`

 * *Files 6% similar despite different names*

#### Python bytecode

```diff
@@ -1,9 +1,9 @@
 magic:    0xa70d0d0a
-moddate:  0x46ba5a66 (Sat Jun  1 06:05:58 2024 UTC)
+moddate:  0x47d85b66 (Sun Jun  2 02:26:15 2024 UTC)
 files sz: 1730
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 5
    flags     : 0
    code
```

### Comparing `agiflow_sdk-0.0.3/agiflow/opentelemetry/instrumentation/anthropic/hooks/__pycache__/base.cpython-311.pyc` & `agiflow_sdk-0.0.4/agiflow/opentelemetry/instrumentation/anthropic/hooks/__pycache__/base.cpython-311.pyc`

 * *Files 3% similar despite different names*

#### Python bytecode

```diff
@@ -1,9 +1,9 @@
 magic:    0xa70d0d0a
-moddate:  0x02995a66 (Sat Jun  1 03:44:02 2024 UTC)
+moddate:  0x47d85b66 (Sun Jun  2 02:26:15 2024 UTC)
 files sz: 1581
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 5
    flags     : 0
    code
```

### Comparing `agiflow_sdk-0.0.3/agiflow/opentelemetry/instrumentation/anthropic/hooks/__pycache__/message_create.cpython-311.pyc` & `agiflow_sdk-0.0.4/agiflow/opentelemetry/instrumentation/anthropic/hooks/__pycache__/message_create.cpython-311.pyc`

 * *Files 0% similar despite different names*

#### Python bytecode

```diff
@@ -1,9 +1,9 @@
 magic:    0xa70d0d0a
-moddate:  0x43985a66 (Sat Jun  1 03:40:51 2024 UTC)
+moddate:  0x47d85b66 (Sun Jun  2 02:26:15 2024 UTC)
 files sz: 7481
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 5
    flags     : 0
    code
```

### Comparing `agiflow_sdk-0.0.3/agiflow/opentelemetry/instrumentation/anthropic/hooks/base.py` & `agiflow_sdk-0.0.4/agiflow/opentelemetry/instrumentation/anthropic/hooks/base.py`

 * *Files identical despite different names*

### Comparing `agiflow_sdk-0.0.3/agiflow/opentelemetry/instrumentation/anthropic/hooks/message_create.py` & `agiflow_sdk-0.0.4/agiflow/opentelemetry/instrumentation/anthropic/hooks/message_create.py`

 * *Files identical despite different names*

### Comparing `agiflow_sdk-0.0.3/agiflow/opentelemetry/instrumentation/anthropic/instrumentation.py` & `agiflow_sdk-0.0.4/agiflow/opentelemetry/instrumentation/anthropic/instrumentation.py`

 * *Files identical despite different names*

### Comparing `agiflow_sdk-0.0.3/agiflow/opentelemetry/instrumentation/chroma/__pycache__/instrumentation.cpython-311.pyc` & `agiflow_sdk-0.0.4/agiflow/opentelemetry/instrumentation/chroma/__pycache__/instrumentation.cpython-311.pyc`

 * *Files 2% similar despite different names*

#### Python bytecode

```diff
@@ -1,9 +1,9 @@
 magic:    0xa70d0d0a
-moddate:  0xe4d85a66 (Sat Jun  1 08:16:36 2024 UTC)
+moddate:  0x47d85b66 (Sun Jun  2 02:26:15 2024 UTC)
 files sz: 1910
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 5
    flags     : 0
    code
```

### Comparing `agiflow_sdk-0.0.3/agiflow/opentelemetry/instrumentation/chroma/hooks/__pycache__/base.cpython-311.pyc` & `agiflow_sdk-0.0.4/agiflow/opentelemetry/instrumentation/chroma/hooks/__pycache__/base.cpython-311.pyc`

 * *Files 0% similar despite different names*

#### Python bytecode

```diff
@@ -1,9 +1,9 @@
 magic:    0xa70d0d0a
-moddate:  0x4ad95a66 (Sat Jun  1 08:18:18 2024 UTC)
+moddate:  0x47d85b66 (Sun Jun  2 02:26:15 2024 UTC)
 files sz: 1385
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 5
    flags     : 0
    code
```

### Comparing `agiflow_sdk-0.0.3/agiflow/opentelemetry/instrumentation/chroma/hooks/__pycache__/collection_call.cpython-311.pyc` & `agiflow_sdk-0.0.4/agiflow/opentelemetry/instrumentation/chroma/hooks/__pycache__/collection_call.cpython-311.pyc`

 * *Files 0% similar despite different names*

#### Python bytecode

```diff
@@ -1,9 +1,9 @@
 magic:    0xa70d0d0a
-moddate:  0x2dd95a66 (Sat Jun  1 08:17:49 2024 UTC)
+moddate:  0x47d85b66 (Sun Jun  2 02:26:15 2024 UTC)
 files sz: 10704
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 5
    flags     : 0
    code
```

### Comparing `agiflow_sdk-0.0.3/agiflow/opentelemetry/instrumentation/chroma/hooks/base.py` & `agiflow_sdk-0.0.4/agiflow/opentelemetry/instrumentation/chroma/hooks/base.py`

 * *Files identical despite different names*

### Comparing `agiflow_sdk-0.0.3/agiflow/opentelemetry/instrumentation/chroma/hooks/collection_call.py` & `agiflow_sdk-0.0.4/agiflow/opentelemetry/instrumentation/chroma/hooks/collection_call.py`

 * *Files identical despite different names*

### Comparing `agiflow_sdk-0.0.3/agiflow/opentelemetry/instrumentation/chroma/instrumentation.py` & `agiflow_sdk-0.0.4/agiflow/opentelemetry/instrumentation/chroma/instrumentation.py`

 * *Files identical despite different names*

### Comparing `agiflow_sdk-0.0.3/agiflow/opentelemetry/instrumentation/cohere/__pycache__/instrumentation.cpython-311.pyc` & `agiflow_sdk-0.0.4/agiflow/opentelemetry/instrumentation/cohere/__pycache__/instrumentation.cpython-311.pyc`

 * *Files 3% similar despite different names*

#### Python bytecode

```diff
@@ -1,9 +1,9 @@
 magic:    0xa70d0d0a
-moddate:  0x6cd95a66 (Sat Jun  1 08:18:52 2024 UTC)
+moddate:  0x47d85b66 (Sun Jun  2 02:26:15 2024 UTC)
 files sz: 2425
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 5
    flags     : 0
    code
```

### Comparing `agiflow_sdk-0.0.3/agiflow/opentelemetry/instrumentation/cohere/hooks/__pycache__/__init__.cpython-311.pyc` & `agiflow_sdk-0.0.4/agiflow/opentelemetry/instrumentation/cohere/hooks/__pycache__/__init__.cpython-311.pyc`

 * *Files 1% similar despite different names*

#### Python bytecode

```diff
@@ -1,9 +1,9 @@
 magic:    0xa70d0d0a
-moddate:  0x07dd5a66 (Sat Jun  1 08:34:15 2024 UTC)
+moddate:  0x47d85b66 (Sun Jun  2 02:26:15 2024 UTC)
 files sz: 511
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 2
    flags     : 0
    code
```

### Comparing `agiflow_sdk-0.0.3/agiflow/opentelemetry/instrumentation/cohere/hooks/__pycache__/base.cpython-311.pyc` & `agiflow_sdk-0.0.4/agiflow/opentelemetry/instrumentation/cohere/hooks/__pycache__/base.cpython-311.pyc`

 * *Files 1% similar despite different names*

#### Python bytecode

```diff
@@ -1,9 +1,9 @@
 magic:    0xa70d0d0a
-moddate:  0x7ad95a66 (Sat Jun  1 08:19:06 2024 UTC)
+moddate:  0x47d85b66 (Sun Jun  2 02:26:15 2024 UTC)
 files sz: 1328
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 5
    flags     : 0
    code
```

### Comparing `agiflow_sdk-0.0.3/agiflow/opentelemetry/instrumentation/cohere/hooks/__pycache__/base_chat.cpython-311.pyc` & `agiflow_sdk-0.0.4/agiflow/opentelemetry/instrumentation/cohere/hooks/__pycache__/base_chat.cpython-311.pyc`

 * *Files 0% similar despite different names*

#### Python bytecode

```diff
@@ -1,9 +1,9 @@
 magic:    0xa70d0d0a
-moddate:  0x1eb75a66 (Sat Jun  1 05:52:30 2024 UTC)
+moddate:  0x47d85b66 (Sun Jun  2 02:26:15 2024 UTC)
 files sz: 5765
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 5
    flags     : 0
    code
```

### Comparing `agiflow_sdk-0.0.3/agiflow/opentelemetry/instrumentation/cohere/hooks/__pycache__/chat_create.cpython-311.pyc` & `agiflow_sdk-0.0.4/agiflow/opentelemetry/instrumentation/cohere/hooks/__pycache__/chat_create.cpython-311.pyc`

 * *Files 0% similar despite different names*

#### Python bytecode

```diff
@@ -1,9 +1,9 @@
 magic:    0xa70d0d0a
-moddate:  0x9dd95a66 (Sat Jun  1 08:19:41 2024 UTC)
+moddate:  0x47d85b66 (Sun Jun  2 02:26:15 2024 UTC)
 files sz: 4975
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 5
    flags     : 0
    code
```

### Comparing `agiflow_sdk-0.0.3/agiflow/opentelemetry/instrumentation/cohere/hooks/__pycache__/chat_stream.cpython-311.pyc` & `agiflow_sdk-0.0.4/agiflow/opentelemetry/instrumentation/cohere/hooks/__pycache__/chat_stream.cpython-311.pyc`

 * *Files 1% similar despite different names*

#### Python bytecode

```diff
@@ -1,9 +1,9 @@
 magic:    0xa70d0d0a
-moddate:  0x00b75a66 (Sat Jun  1 05:52:00 2024 UTC)
+moddate:  0x47d85b66 (Sun Jun  2 02:26:15 2024 UTC)
 files sz: 7065
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 5
    flags     : 0
    code
```

### Comparing `agiflow_sdk-0.0.3/agiflow/opentelemetry/instrumentation/cohere/hooks/__pycache__/embed.cpython-311.pyc` & `agiflow_sdk-0.0.4/agiflow/opentelemetry/instrumentation/cohere/hooks/__pycache__/embed.cpython-311.pyc`

 * *Files 1% similar despite different names*

#### Python bytecode

```diff
@@ -1,9 +1,9 @@
 magic:    0xa70d0d0a
-moddate:  0xe7b65a66 (Sat Jun  1 05:51:35 2024 UTC)
+moddate:  0x47d85b66 (Sun Jun  2 02:26:15 2024 UTC)
 files sz: 3919
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 5
    flags     : 0
    code
```

### Comparing `agiflow_sdk-0.0.3/agiflow/opentelemetry/instrumentation/cohere/hooks/__pycache__/rerank.cpython-311.pyc` & `agiflow_sdk-0.0.4/agiflow/opentelemetry/instrumentation/cohere/hooks/__pycache__/rerank.cpython-311.pyc`

 * *Files 1% similar despite different names*

#### Python bytecode

```diff
@@ -1,9 +1,9 @@
 magic:    0xa70d0d0a
-moddate:  0xd9b65a66 (Sat Jun  1 05:51:21 2024 UTC)
+moddate:  0x47d85b66 (Sun Jun  2 02:26:15 2024 UTC)
 files sz: 4364
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 5
    flags     : 0
    code
```

### Comparing `agiflow_sdk-0.0.3/agiflow/opentelemetry/instrumentation/cohere/hooks/base.py` & `agiflow_sdk-0.0.4/agiflow/opentelemetry/instrumentation/cohere/hooks/base.py`

 * *Files identical despite different names*

### Comparing `agiflow_sdk-0.0.3/agiflow/opentelemetry/instrumentation/cohere/hooks/base_chat.py` & `agiflow_sdk-0.0.4/agiflow/opentelemetry/instrumentation/cohere/hooks/base_chat.py`

 * *Files identical despite different names*

### Comparing `agiflow_sdk-0.0.3/agiflow/opentelemetry/instrumentation/cohere/hooks/chat_create.py` & `agiflow_sdk-0.0.4/agiflow/opentelemetry/instrumentation/cohere/hooks/chat_create.py`

 * *Files identical despite different names*

### Comparing `agiflow_sdk-0.0.3/agiflow/opentelemetry/instrumentation/cohere/hooks/chat_stream.py` & `agiflow_sdk-0.0.4/agiflow/opentelemetry/instrumentation/cohere/hooks/chat_stream.py`

 * *Files identical despite different names*

### Comparing `agiflow_sdk-0.0.3/agiflow/opentelemetry/instrumentation/cohere/hooks/embed.py` & `agiflow_sdk-0.0.4/agiflow/opentelemetry/instrumentation/cohere/hooks/embed.py`

 * *Files identical despite different names*

### Comparing `agiflow_sdk-0.0.3/agiflow/opentelemetry/instrumentation/cohere/hooks/rerank.py` & `agiflow_sdk-0.0.4/agiflow/opentelemetry/instrumentation/cohere/hooks/rerank.py`

 * *Files identical despite different names*

### Comparing `agiflow_sdk-0.0.3/agiflow/opentelemetry/instrumentation/cohere/instrumentation.py` & `agiflow_sdk-0.0.4/agiflow/opentelemetry/instrumentation/cohere/instrumentation.py`

 * *Files identical despite different names*

### Comparing `agiflow_sdk-0.0.3/agiflow/opentelemetry/instrumentation/constants/__pycache__/__init__.cpython-311.pyc` & `agiflow_sdk-0.0.4/agiflow/opentelemetry/instrumentation/constants/__pycache__/__init__.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `agiflow_sdk-0.0.3/agiflow/opentelemetry/instrumentation/constants/__pycache__/chroma.cpython-311.pyc` & `agiflow_sdk-0.0.4/agiflow/opentelemetry/instrumentation/constants/__pycache__/chroma.cpython-311.pyc`

 * *Files 9% similar despite different names*

#### Python bytecode

```diff
@@ -1,9 +1,9 @@
 magic:    0xa70d0d0a
-moddate:  0x9d9a5a66 (Sat Jun  1 03:50:53 2024 UTC)
+moddate:  0x47d85b66 (Sun Jun  2 02:26:15 2024 UTC)
 files sz: 972
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 11
    flags     : 0
    code
```

### Comparing `agiflow_sdk-0.0.3/agiflow/opentelemetry/instrumentation/constants/__pycache__/cohere.cpython-311.pyc` & `agiflow_sdk-0.0.4/agiflow/opentelemetry/instrumentation/constants/__pycache__/cohere.cpython-311.pyc`

 * *Files 20% similar despite different names*

#### Python bytecode

```diff
@@ -1,9 +1,9 @@
 magic:    0xa70d0d0a
-moddate:  0x77aa5a66 (Sat Jun  1 04:58:31 2024 UTC)
+moddate:  0x47d85b66 (Sun Jun  2 02:26:15 2024 UTC)
 files sz: 577
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 7
    flags     : 0
    code
```

### Comparing `agiflow_sdk-0.0.3/agiflow/opentelemetry/instrumentation/constants/__pycache__/common.cpython-311.pyc` & `agiflow_sdk-0.0.4/agiflow/opentelemetry/instrumentation/constants/__pycache__/common.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `agiflow_sdk-0.0.3/agiflow/opentelemetry/instrumentation/constants/__pycache__/openai.cpython-311.pyc` & `agiflow_sdk-0.0.4/agiflow/opentelemetry/instrumentation/constants/__pycache__/openai.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `agiflow_sdk-0.0.3/agiflow/opentelemetry/instrumentation/constants/chroma.py` & `agiflow_sdk-0.0.4/agiflow/opentelemetry/instrumentation/constants/chroma.py`

 * *Files identical despite different names*

### Comparing `agiflow_sdk-0.0.3/agiflow/opentelemetry/instrumentation/constants/cohere.py` & `agiflow_sdk-0.0.4/agiflow/opentelemetry/instrumentation/constants/cohere.py`

 * *Files identical despite different names*

### Comparing `agiflow_sdk-0.0.3/agiflow/opentelemetry/instrumentation/constants/common.py` & `agiflow_sdk-0.0.4/agiflow/opentelemetry/instrumentation/constants/common.py`

 * *Files identical despite different names*

### Comparing `agiflow_sdk-0.0.3/agiflow/opentelemetry/instrumentation/constants/openai.py` & `agiflow_sdk-0.0.4/agiflow/opentelemetry/instrumentation/constants/openai.py`

 * *Files identical despite different names*

### Comparing `agiflow_sdk-0.0.3/agiflow/opentelemetry/instrumentation/constants/qdrant.py` & `agiflow_sdk-0.0.4/agiflow/opentelemetry/instrumentation/constants/qdrant.py`

 * *Files identical despite different names*

### Comparing `agiflow_sdk-0.0.3/agiflow/opentelemetry/instrumentation/constants/weaviate.py` & `agiflow_sdk-0.0.4/agiflow/opentelemetry/instrumentation/constants/weaviate.py`

 * *Files identical despite different names*

### Comparing `agiflow_sdk-0.0.3/agiflow/opentelemetry/instrumentation/groq/hooks/base.py` & `agiflow_sdk-0.0.4/agiflow/opentelemetry/instrumentation/groq/hooks/base.py`

 * *Files identical despite different names*

### Comparing `agiflow_sdk-0.0.3/agiflow/opentelemetry/instrumentation/groq/hooks/chat_completion.py` & `agiflow_sdk-0.0.4/agiflow/opentelemetry/instrumentation/groq/hooks/chat_completion.py`

 * *Files identical despite different names*

### Comparing `agiflow_sdk-0.0.3/agiflow/opentelemetry/instrumentation/groq/instrumentation.py` & `agiflow_sdk-0.0.4/agiflow/opentelemetry/instrumentation/groq/instrumentation.py`

 * *Files identical despite different names*

### Comparing `agiflow_sdk-0.0.3/agiflow/opentelemetry/instrumentation/langchain/.DS_Store` & `agiflow_sdk-0.0.4/agiflow/opentelemetry/instrumentation/langchain/.DS_Store`

 * *Files identical despite different names*

### Comparing `agiflow_sdk-0.0.3/agiflow/opentelemetry/instrumentation/langchain/__pycache__/instrumentation.cpython-311.pyc` & `agiflow_sdk-0.0.4/agiflow/opentelemetry/instrumentation/langchain/__pycache__/instrumentation.cpython-311.pyc`

 * *Files 0% similar despite different names*

#### Python bytecode

```diff
@@ -1,9 +1,9 @@
 magic:    0xa70d0d0a
-moddate:  0x2cb45b66 (Sat Jun  1 23:52:12 2024 UTC)
+moddate:  0x47d85b66 (Sun Jun  2 02:26:15 2024 UTC)
 files sz: 2232
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 5
    flags     : 0
    code
```

### Comparing `agiflow_sdk-0.0.3/agiflow/opentelemetry/instrumentation/langchain/__pycache__/patch.cpython-311.pyc` & `agiflow_sdk-0.0.4/agiflow/opentelemetry/instrumentation/langchain/__pycache__/patch.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `agiflow_sdk-0.0.3/agiflow/opentelemetry/instrumentation/langchain/hooks/__pycache__/__init__.cpython-311.pyc` & `agiflow_sdk-0.0.4/agiflow/opentelemetry/instrumentation/langchain/hooks/__pycache__/__init__.cpython-311.pyc`

 * *Files 2% similar despite different names*

#### Python bytecode

```diff
@@ -1,9 +1,9 @@
 magic:    0xa70d0d0a
-moddate:  0x4add5a66 (Sat Jun  1 08:35:22 2024 UTC)
+moddate:  0x47d85b66 (Sun Jun  2 02:26:15 2024 UTC)
 files sz: 252
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 2
    flags     : 0
    code
```

### Comparing `agiflow_sdk-0.0.3/agiflow/opentelemetry/instrumentation/langchain/hooks/__pycache__/base.cpython-311.pyc` & `agiflow_sdk-0.0.4/agiflow/opentelemetry/instrumentation/langchain/hooks/__pycache__/base.cpython-311.pyc`

 * *Files 1% similar despite different names*

#### Python bytecode

```diff
@@ -1,9 +1,9 @@
 magic:    0xa70d0d0a
-moddate:  0x21b45b66 (Sat Jun  1 23:52:01 2024 UTC)
+moddate:  0x47d85b66 (Sun Jun  2 02:26:15 2024 UTC)
 files sz: 1384
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 5
    flags     : 0
    code
```

### Comparing `agiflow_sdk-0.0.3/agiflow/opentelemetry/instrumentation/langchain/hooks/__pycache__/chat.cpython-311.pyc` & `agiflow_sdk-0.0.4/agiflow/opentelemetry/instrumentation/langchain/hooks/__pycache__/chat.cpython-311.pyc`

 * *Files 1% similar despite different names*

#### Python bytecode

```diff
@@ -1,9 +1,9 @@
 magic:    0xa70d0d0a
-moddate:  0x3bd65b66 (Sun Jun  2 02:17:31 2024 UTC)
+moddate:  0x47d85b66 (Sun Jun  2 02:26:15 2024 UTC)
 files sz: 5021
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 5
    flags     : 0
    code
```

### Comparing `agiflow_sdk-0.0.3/agiflow/opentelemetry/instrumentation/langchain/hooks/__pycache__/generic.cpython-311.pyc` & `agiflow_sdk-0.0.4/agiflow/opentelemetry/instrumentation/langchain/hooks/__pycache__/generic.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `agiflow_sdk-0.0.3/agiflow/opentelemetry/instrumentation/langchain/hooks/base.py` & `agiflow_sdk-0.0.4/agiflow/opentelemetry/instrumentation/langchain/hooks/base.py`

 * *Files identical despite different names*

### Comparing `agiflow_sdk-0.0.3/agiflow/opentelemetry/instrumentation/langchain/hooks/chat.py` & `agiflow_sdk-0.0.4/agiflow/opentelemetry/instrumentation/langchain/hooks/chat.py`

 * *Files identical despite different names*

### Comparing `agiflow_sdk-0.0.3/agiflow/opentelemetry/instrumentation/langchain/hooks/generic.py` & `agiflow_sdk-0.0.4/agiflow/opentelemetry/instrumentation/langchain/hooks/generic.py`

 * *Files identical despite different names*

### Comparing `agiflow_sdk-0.0.3/agiflow/opentelemetry/instrumentation/langchain/instrumentation.py` & `agiflow_sdk-0.0.4/agiflow/opentelemetry/instrumentation/langchain/instrumentation.py`

 * *Files identical despite different names*

### Comparing `agiflow_sdk-0.0.3/agiflow/opentelemetry/instrumentation/langchain_community/.DS_Store` & `agiflow_sdk-0.0.4/agiflow/opentelemetry/instrumentation/langchain_community/.DS_Store`

 * *Files identical despite different names*

### Comparing `agiflow_sdk-0.0.3/agiflow/opentelemetry/instrumentation/langchain_community/__pycache__/instrumentation.cpython-311.pyc` & `agiflow_sdk-0.0.4/agiflow/opentelemetry/instrumentation/langchain_community/__pycache__/instrumentation.cpython-311.pyc`

 * *Files 2% similar despite different names*

#### Python bytecode

```diff
@@ -1,9 +1,9 @@
 magic:    0xa70d0d0a
-moddate:  0x4fb45b66 (Sat Jun  1 23:52:47 2024 UTC)
+moddate:  0x47d85b66 (Sun Jun  2 02:26:15 2024 UTC)
 files sz: 3005
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 5
    flags     : 0
    code
```

### Comparing `agiflow_sdk-0.0.3/agiflow/opentelemetry/instrumentation/langchain_community/__pycache__/patch.cpython-311.pyc` & `agiflow_sdk-0.0.4/agiflow/opentelemetry/instrumentation/langchain_community/__pycache__/patch.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `agiflow_sdk-0.0.3/agiflow/opentelemetry/instrumentation/langchain_community/hooks/.DS_Store` & `agiflow_sdk-0.0.4/agiflow/opentelemetry/instrumentation/langchain_community/hooks/.DS_Store`

 * *Files identical despite different names*

### Comparing `agiflow_sdk-0.0.3/agiflow/opentelemetry/instrumentation/langchain_community/hooks/__pycache__/base.cpython-311.pyc` & `agiflow_sdk-0.0.4/agiflow/opentelemetry/instrumentation/langchain_community/hooks/__pycache__/base.cpython-311.pyc`

 * *Files 1% similar despite different names*

#### Python bytecode

```diff
@@ -1,9 +1,9 @@
 magic:    0xa70d0d0a
-moddate:  0x4db45b66 (Sat Jun  1 23:52:45 2024 UTC)
+moddate:  0x47d85b66 (Sun Jun  2 02:26:15 2024 UTC)
 files sz: 1499
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 5
    flags     : 0
    code
```

### Comparing `agiflow_sdk-0.0.3/agiflow/opentelemetry/instrumentation/langchain_community/hooks/__pycache__/chat.cpython-311.pyc` & `agiflow_sdk-0.0.4/agiflow/opentelemetry/instrumentation/langchain_community/hooks/__pycache__/chat.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `agiflow_sdk-0.0.3/agiflow/opentelemetry/instrumentation/langchain_community/hooks/__pycache__/generic.cpython-311.pyc` & `agiflow_sdk-0.0.4/agiflow/opentelemetry/instrumentation/langchain_community/hooks/__pycache__/generic.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `agiflow_sdk-0.0.3/agiflow/opentelemetry/instrumentation/langchain_community/hooks/__pycache__/llm.cpython-311.pyc` & `agiflow_sdk-0.0.4/agiflow/opentelemetry/instrumentation/langchain_community/hooks/__pycache__/llm.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `agiflow_sdk-0.0.3/agiflow/opentelemetry/instrumentation/langchain_community/hooks/base.py` & `agiflow_sdk-0.0.4/agiflow/opentelemetry/instrumentation/langchain_community/hooks/base.py`

 * *Files identical despite different names*

### Comparing `agiflow_sdk-0.0.3/agiflow/opentelemetry/instrumentation/langchain_community/hooks/generic.py` & `agiflow_sdk-0.0.4/agiflow/opentelemetry/instrumentation/langchain_community/hooks/generic.py`

 * *Files identical despite different names*

### Comparing `agiflow_sdk-0.0.3/agiflow/opentelemetry/instrumentation/langchain_community/instrumentation.py` & `agiflow_sdk-0.0.4/agiflow/opentelemetry/instrumentation/langchain_community/instrumentation.py`

 * *Files identical despite different names*

### Comparing `agiflow_sdk-0.0.3/agiflow/opentelemetry/instrumentation/langchain_core/.DS_Store` & `agiflow_sdk-0.0.4/agiflow/opentelemetry/instrumentation/langchain_core/.DS_Store`

 * *Files identical despite different names*

### Comparing `agiflow_sdk-0.0.3/agiflow/opentelemetry/instrumentation/langchain_core/__pycache__/instrumentation.cpython-311.pyc` & `agiflow_sdk-0.0.4/agiflow/opentelemetry/instrumentation/langchain_core/__pycache__/instrumentation.cpython-311.pyc`

 * *Files 2% similar despite different names*

#### Python bytecode

```diff
@@ -1,9 +1,9 @@
 magic:    0xa70d0d0a
-moddate:  0x71b45b66 (Sat Jun  1 23:53:21 2024 UTC)
+moddate:  0x47d85b66 (Sun Jun  2 02:26:15 2024 UTC)
 files sz: 3346
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 5
    flags     : 0
    code
```

### Comparing `agiflow_sdk-0.0.3/agiflow/opentelemetry/instrumentation/langchain_core/__pycache__/patch.cpython-311.pyc` & `agiflow_sdk-0.0.4/agiflow/opentelemetry/instrumentation/langchain_core/__pycache__/patch.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `agiflow_sdk-0.0.3/agiflow/opentelemetry/instrumentation/langchain_core/hooks/__pycache__/__init__.cpython-311.pyc` & `agiflow_sdk-0.0.4/agiflow/opentelemetry/instrumentation/langchain_core/hooks/__pycache__/__init__.cpython-311.pyc`

 * *Files 15% similar despite different names*

#### Python bytecode

```diff
@@ -1,9 +1,9 @@
 magic:    0xa70d0d0a
-moddate:  0x99dd5a66 (Sat Jun  1 08:36:41 2024 UTC)
+moddate:  0x47d85b66 (Sun Jun  2 02:26:15 2024 UTC)
 files sz: 390
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 2
    flags     : 0
    code
```

### Comparing `agiflow_sdk-0.0.3/agiflow/opentelemetry/instrumentation/langchain_core/hooks/__pycache__/base.cpython-311.pyc` & `agiflow_sdk-0.0.4/agiflow/opentelemetry/instrumentation/langchain_core/hooks/__pycache__/base.cpython-311.pyc`

 * *Files 1% similar despite different names*

#### Python bytecode

```diff
@@ -1,9 +1,9 @@
 magic:    0xa70d0d0a
-moddate:  0x67b45b66 (Sat Jun  1 23:53:11 2024 UTC)
+moddate:  0x47d85b66 (Sun Jun  2 02:26:15 2024 UTC)
 files sz: 1533
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 5
    flags     : 0
    code
```

### Comparing `agiflow_sdk-0.0.3/agiflow/opentelemetry/instrumentation/langchain_core/hooks/__pycache__/generic.cpython-311.pyc` & `agiflow_sdk-0.0.4/agiflow/opentelemetry/instrumentation/langchain_core/hooks/__pycache__/generic.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `agiflow_sdk-0.0.3/agiflow/opentelemetry/instrumentation/langchain_core/hooks/__pycache__/llm.cpython-311.pyc` & `agiflow_sdk-0.0.4/agiflow/opentelemetry/instrumentation/langchain_core/hooks/__pycache__/llm.cpython-311.pyc`

 * *Files 0% similar despite different names*

#### Python bytecode

```diff
@@ -1,9 +1,9 @@
 magic:    0xa70d0d0a
-moddate:  0x9ed65b66 (Sun Jun  2 02:19:10 2024 UTC)
+moddate:  0x47d85b66 (Sun Jun  2 02:26:15 2024 UTC)
 files sz: 3178
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 5
    flags     : 0
    code
```

### Comparing `agiflow_sdk-0.0.3/agiflow/opentelemetry/instrumentation/langchain_core/hooks/__pycache__/runnable.cpython-311.pyc` & `agiflow_sdk-0.0.4/agiflow/opentelemetry/instrumentation/langchain_core/hooks/__pycache__/runnable.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `agiflow_sdk-0.0.3/agiflow/opentelemetry/instrumentation/langchain_core/hooks/base.py` & `agiflow_sdk-0.0.4/agiflow/opentelemetry/instrumentation/langchain_core/hooks/base.py`

 * *Files identical despite different names*

### Comparing `agiflow_sdk-0.0.3/agiflow/opentelemetry/instrumentation/langchain_core/hooks/generic.py` & `agiflow_sdk-0.0.4/agiflow/opentelemetry/instrumentation/langchain_core/hooks/generic.py`

 * *Files identical despite different names*

### Comparing `agiflow_sdk-0.0.3/agiflow/opentelemetry/instrumentation/langchain_core/hooks/llm.py` & `agiflow_sdk-0.0.4/agiflow/opentelemetry/instrumentation/langchain_core/hooks/llm.py`

 * *Files identical despite different names*

### Comparing `agiflow_sdk-0.0.3/agiflow/opentelemetry/instrumentation/langchain_core/hooks/runnable.py` & `agiflow_sdk-0.0.4/agiflow/opentelemetry/instrumentation/langchain_core/hooks/runnable.py`

 * *Files identical despite different names*

### Comparing `agiflow_sdk-0.0.3/agiflow/opentelemetry/instrumentation/langchain_core/instrumentation.py` & `agiflow_sdk-0.0.4/agiflow/opentelemetry/instrumentation/langchain_core/instrumentation.py`

 * *Files identical despite different names*

### Comparing `agiflow_sdk-0.0.3/agiflow/opentelemetry/instrumentation/langgraph/hooks/base.py` & `agiflow_sdk-0.0.4/agiflow/opentelemetry/instrumentation/langgraph/hooks/base.py`

 * *Files identical despite different names*

### Comparing `agiflow_sdk-0.0.3/agiflow/opentelemetry/instrumentation/langgraph/hooks/graph_call.py` & `agiflow_sdk-0.0.4/agiflow/opentelemetry/instrumentation/langgraph/hooks/graph_call.py`

 * *Files identical despite different names*

### Comparing `agiflow_sdk-0.0.3/agiflow/opentelemetry/instrumentation/langgraph/instrumentation.py` & `agiflow_sdk-0.0.4/agiflow/opentelemetry/instrumentation/langgraph/instrumentation.py`

 * *Files identical despite different names*

### Comparing `agiflow_sdk-0.0.3/agiflow/opentelemetry/instrumentation/llamaindex/hooks/base.py` & `agiflow_sdk-0.0.4/agiflow/opentelemetry/instrumentation/llamaindex/hooks/base.py`

 * *Files identical despite different names*

### Comparing `agiflow_sdk-0.0.3/agiflow/opentelemetry/instrumentation/llamaindex/hooks/generic.py` & `agiflow_sdk-0.0.4/agiflow/opentelemetry/instrumentation/llamaindex/hooks/generic.py`

 * *Files identical despite different names*

### Comparing `agiflow_sdk-0.0.3/agiflow/opentelemetry/instrumentation/llamaindex/instrumentation.py` & `agiflow_sdk-0.0.4/agiflow/opentelemetry/instrumentation/llamaindex/instrumentation.py`

 * *Files identical despite different names*

### Comparing `agiflow_sdk-0.0.3/agiflow/opentelemetry/instrumentation/openai/.DS_Store` & `agiflow_sdk-0.0.4/agiflow/opentelemetry/instrumentation/openai/.DS_Store`

 * *Files identical despite different names*

### Comparing `agiflow_sdk-0.0.3/agiflow/opentelemetry/instrumentation/openai/__pycache__/instrumentation.cpython-311.pyc` & `agiflow_sdk-0.0.4/agiflow/opentelemetry/instrumentation/openai/__pycache__/instrumentation.cpython-311.pyc`

 * *Files 2% similar despite different names*

#### Python bytecode

```diff
@@ -1,9 +1,9 @@
 magic:    0xa70d0d0a
-moddate:  0x70ba5a66 (Sat Jun  1 06:06:40 2024 UTC)
+moddate:  0x47d85b66 (Sun Jun  2 02:26:15 2024 UTC)
 files sz: 2910
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 5
    flags     : 0
    code
```

### Comparing `agiflow_sdk-0.0.3/agiflow/opentelemetry/instrumentation/openai/__pycache__/patch.cpython-311.pyc` & `agiflow_sdk-0.0.4/agiflow/opentelemetry/instrumentation/openai/__pycache__/patch.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `agiflow_sdk-0.0.3/agiflow/opentelemetry/instrumentation/openai/hooks/.DS_Store` & `agiflow_sdk-0.0.4/agiflow/opentelemetry/instrumentation/openai/hooks/.DS_Store`

 * *Files identical despite different names*

### Comparing `agiflow_sdk-0.0.3/agiflow/opentelemetry/instrumentation/openai/hooks/__pycache__/__init__.cpython-311.pyc` & `agiflow_sdk-0.0.4/agiflow/opentelemetry/instrumentation/openai/hooks/__pycache__/__init__.cpython-311.pyc`

 * *Files 2% similar despite different names*

#### Python bytecode

```diff
@@ -1,9 +1,9 @@
 magic:    0xa70d0d0a
-moddate:  0x0ade5a66 (Sat Jun  1 08:38:34 2024 UTC)
+moddate:  0x47d85b66 (Sun Jun  2 02:26:15 2024 UTC)
 files sz: 424
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 2
    flags     : 0
    code
```

### Comparing `agiflow_sdk-0.0.3/agiflow/opentelemetry/instrumentation/openai/hooks/__pycache__/base.cpython-311.pyc` & `agiflow_sdk-0.0.4/agiflow/opentelemetry/instrumentation/openai/hooks/__pycache__/base.cpython-311.pyc`

 * *Files 1% similar despite different names*

#### Python bytecode

```diff
@@ -1,9 +1,9 @@
 magic:    0xa70d0d0a
-moddate:  0xc8d65b66 (Sun Jun  2 02:19:52 2024 UTC)
+moddate:  0x47d85b66 (Sun Jun  2 02:26:15 2024 UTC)
 files sz: 2474
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 5
    flags     : 0
    code
```

### Comparing `agiflow_sdk-0.0.3/agiflow/opentelemetry/instrumentation/openai/hooks/__pycache__/base_llm.cpython-311.pyc` & `agiflow_sdk-0.0.4/agiflow/opentelemetry/instrumentation/openai/hooks/__pycache__/base_llm.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `agiflow_sdk-0.0.3/agiflow/opentelemetry/instrumentation/openai/hooks/__pycache__/chat_completion.cpython-311.pyc` & `agiflow_sdk-0.0.4/agiflow/opentelemetry/instrumentation/openai/hooks/__pycache__/chat_completion.cpython-311.pyc`

 * *Files 1% similar despite different names*

#### Python bytecode

```diff
@@ -1,9 +1,9 @@
 magic:    0xa70d0d0a
-moddate:  0x43985a66 (Sat Jun  1 03:40:51 2024 UTC)
+moddate:  0x47d85b66 (Sun Jun  2 02:26:15 2024 UTC)
 files sz: 10648
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 5
    flags     : 0
    code
```

### Comparing `agiflow_sdk-0.0.3/agiflow/opentelemetry/instrumentation/openai/hooks/__pycache__/completion.cpython-311.pyc` & `agiflow_sdk-0.0.4/agiflow/opentelemetry/instrumentation/openai/hooks/__pycache__/completion.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `agiflow_sdk-0.0.3/agiflow/opentelemetry/instrumentation/openai/hooks/__pycache__/embedding.cpython-311.pyc` & `agiflow_sdk-0.0.4/agiflow/opentelemetry/instrumentation/openai/hooks/__pycache__/embedding.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `agiflow_sdk-0.0.3/agiflow/opentelemetry/instrumentation/openai/hooks/__pycache__/image_generate.cpython-311.pyc` & `agiflow_sdk-0.0.4/agiflow/opentelemetry/instrumentation/openai/hooks/__pycache__/image_generate.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `agiflow_sdk-0.0.3/agiflow/opentelemetry/instrumentation/openai/hooks/__pycache__/utils.cpython-311.pyc` & `agiflow_sdk-0.0.4/agiflow/opentelemetry/instrumentation/openai/hooks/__pycache__/utils.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `agiflow_sdk-0.0.3/agiflow/opentelemetry/instrumentation/openai/hooks/base.py` & `agiflow_sdk-0.0.4/agiflow/opentelemetry/instrumentation/openai/hooks/base.py`

 * *Files identical despite different names*

### Comparing `agiflow_sdk-0.0.3/agiflow/opentelemetry/instrumentation/openai/hooks/base_llm.py` & `agiflow_sdk-0.0.4/agiflow/opentelemetry/instrumentation/openai/hooks/base_llm.py`

 * *Files identical despite different names*

### Comparing `agiflow_sdk-0.0.3/agiflow/opentelemetry/instrumentation/openai/hooks/chat_completion.py` & `agiflow_sdk-0.0.4/agiflow/opentelemetry/instrumentation/openai/hooks/chat_completion.py`

 * *Files identical despite different names*

### Comparing `agiflow_sdk-0.0.3/agiflow/opentelemetry/instrumentation/openai/hooks/embedding.py` & `agiflow_sdk-0.0.4/agiflow/opentelemetry/instrumentation/openai/hooks/embedding.py`

 * *Files identical despite different names*

### Comparing `agiflow_sdk-0.0.3/agiflow/opentelemetry/instrumentation/openai/hooks/image_generate.py` & `agiflow_sdk-0.0.4/agiflow/opentelemetry/instrumentation/openai/hooks/image_generate.py`

 * *Files identical despite different names*

### Comparing `agiflow_sdk-0.0.3/agiflow/opentelemetry/instrumentation/openai/hooks/utils.py` & `agiflow_sdk-0.0.4/agiflow/opentelemetry/instrumentation/openai/hooks/utils.py`

 * *Files identical despite different names*

### Comparing `agiflow_sdk-0.0.3/agiflow/opentelemetry/instrumentation/openai/instrumentation.py` & `agiflow_sdk-0.0.4/agiflow/opentelemetry/instrumentation/openai/instrumentation.py`

 * *Files identical despite different names*

### Comparing `agiflow_sdk-0.0.3/agiflow/opentelemetry/instrumentation/pinecone/hooks/base.py` & `agiflow_sdk-0.0.4/agiflow/opentelemetry/instrumentation/pinecone/hooks/base.py`

 * *Files identical despite different names*

### Comparing `agiflow_sdk-0.0.3/agiflow/opentelemetry/instrumentation/pinecone/hooks/generic.py` & `agiflow_sdk-0.0.4/agiflow/opentelemetry/instrumentation/pinecone/hooks/generic.py`

 * *Files identical despite different names*

### Comparing `agiflow_sdk-0.0.3/agiflow/opentelemetry/instrumentation/pinecone/instrumentation.py` & `agiflow_sdk-0.0.4/agiflow/opentelemetry/instrumentation/pinecone/instrumentation.py`

 * *Files identical despite different names*

### Comparing `agiflow_sdk-0.0.3/agiflow/opentelemetry/instrumentation/qdrant/hooks/base.py` & `agiflow_sdk-0.0.4/agiflow/opentelemetry/instrumentation/qdrant/hooks/base.py`

 * *Files identical despite different names*

### Comparing `agiflow_sdk-0.0.3/agiflow/opentelemetry/instrumentation/qdrant/hooks/collection.py` & `agiflow_sdk-0.0.4/agiflow/opentelemetry/instrumentation/qdrant/hooks/collection.py`

 * *Files identical despite different names*

### Comparing `agiflow_sdk-0.0.3/agiflow/opentelemetry/instrumentation/qdrant/instrumentation.py` & `agiflow_sdk-0.0.4/agiflow/opentelemetry/instrumentation/qdrant/instrumentation.py`

 * *Files identical despite different names*

### Comparing `agiflow_sdk-0.0.3/agiflow/opentelemetry/instrumentation/utils/__init__.py` & `agiflow_sdk-0.0.4/agiflow/opentelemetry/instrumentation/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `agiflow_sdk-0.0.3/agiflow/opentelemetry/instrumentation/utils/__pycache__/__init__.cpython-311.pyc` & `agiflow_sdk-0.0.4/agiflow/opentelemetry/instrumentation/utils/__pycache__/__init__.cpython-311.pyc`

 * *Files 1% similar despite different names*

#### Python bytecode

```diff
@@ -1,9 +1,9 @@
 magic:    0xa70d0d0a
-moddate:  0x08b45b66 (Sat Jun  1 23:51:36 2024 UTC)
+moddate:  0x47d85b66 (Sun Jun  2 02:26:15 2024 UTC)
 files sz: 2309
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 8
    flags     : 0
    code
```

### Comparing `agiflow_sdk-0.0.3/agiflow/opentelemetry/instrumentation/utils/__pycache__/wrapper.cpython-311.pyc` & `agiflow_sdk-0.0.4/agiflow/opentelemetry/instrumentation/utils/__pycache__/wrapper.cpython-311.pyc`

 * *Files 0% similar despite different names*

#### Python bytecode

```diff
@@ -1,9 +1,9 @@
 magic:    0xa70d0d0a
-moddate:  0x08c15b66 (Sun Jun  2 00:47:04 2024 UTC)
+moddate:  0x47d85b66 (Sun Jun  2 02:26:15 2024 UTC)
 files sz: 11559
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 10
    flags     : 0
    code
```

### Comparing `agiflow_sdk-0.0.3/agiflow/opentelemetry/instrumentation/utils/wrapper.py` & `agiflow_sdk-0.0.4/agiflow/opentelemetry/instrumentation/utils/wrapper.py`

 * *Files identical despite different names*

### Comparing `agiflow_sdk-0.0.3/agiflow/opentelemetry/instrumentation/weaviate/hooks/base.py` & `agiflow_sdk-0.0.4/agiflow/opentelemetry/instrumentation/weaviate/hooks/base.py`

 * *Files identical despite different names*

### Comparing `agiflow_sdk-0.0.3/agiflow/opentelemetry/instrumentation/weaviate/hooks/generic_collection.py` & `agiflow_sdk-0.0.4/agiflow/opentelemetry/instrumentation/weaviate/hooks/generic_collection.py`

 * *Files identical despite different names*

### Comparing `agiflow_sdk-0.0.3/agiflow/opentelemetry/instrumentation/weaviate/hooks/generic_query.py` & `agiflow_sdk-0.0.4/agiflow/opentelemetry/instrumentation/weaviate/hooks/generic_query.py`

 * *Files identical despite different names*

### Comparing `agiflow_sdk-0.0.3/agiflow/opentelemetry/instrumentation/weaviate/instrumentation.py` & `agiflow_sdk-0.0.4/agiflow/opentelemetry/instrumentation/weaviate/instrumentation.py`

 * *Files identical despite different names*

### Comparing `agiflow_sdk-0.0.3/agiflow/opentelemetry/span_processors/__pycache__/thread_pool_span_processor.cpython-311.pyc` & `agiflow_sdk-0.0.4/agiflow/opentelemetry/span_processors/__pycache__/thread_pool_span_processor.cpython-311.pyc`

 * *Files 10% similar despite different names*

#### Python bytecode

```diff
@@ -1,22 +1,22 @@
 magic:    0xa70d0d0a
-moddate:  0x11d75b66 (Sun Jun  2 02:21:05 2024 UTC)
-files sz: 2347
+moddate:  0xf5105d66 (Mon Jun  3 00:40:21 2024 UTC)
+files sz: 2544
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 5
    flags     : 0
    code
       0x9700640064016c005a00640064016c015a01640064026c026d035a036d
       045a046d055a050100640064036c066d075a070100640064046c086d095a
       096d0a5a0a6d0b5a0b6d0c5a0c6d0d5a0d0100640064056c0e6d0f5a0f01
-      00640064066c106d115a110100020065006a1200000000000000006513a6
-      010000ab0100000000000000005a14020047006407840064086503a60300
-      00ab0300000000000000005a1564015300
+      00640064066c106d115a110100640064016c125a12020065006a13000000
+      00000000006514a6010000ab0100000000000000005a1502004700640784
+      0064086503a6030000ab0300000000000000005a1664015300
      0           0 RESUME                   0
    
      1           2 LOAD_CONST               0 (0)
                  4 LOAD_CONST               1 (None)
                  6 IMPORT_NAME              0 (logging)
                  8 STORE_NAME               0 (logging)
    
@@ -68,33 +68,38 @@
     14          90 LOAD_CONST               0 (0)
                 92 LOAD_CONST               6 (('Pool',))
                 94 IMPORT_NAME             16 (multiprocessing.dummy)
                 96 IMPORT_FROM             17 (Pool)
                 98 STORE_NAME              17 (Pool)
                100 POP_TOP
    
-    16         102 PUSH_NULL
-               104 LOAD_NAME                0 (logging)
-               106 LOAD_ATTR               18 (getLogger)
-               116 LOAD_NAME               19 (__name__)
-               118 PRECALL                  1
-               122 CALL                     1
-               132 STORE_NAME              20 (logger)
+    15         102 LOAD_CONST               0 (0)
+               104 LOAD_CONST               1 (None)
+               106 IMPORT_NAME             18 (atexit)
+               108 STORE_NAME              18 (atexit)
    
-    19         134 PUSH_NULL
-               136 LOAD_BUILD_CLASS
-               138 LOAD_CONST               7 (<code object ThreadPoolSpanProcessor, file "/Users/vuongngo/workspace/agiflow/packages/python/agiflow-sdk/agiflow/opentelemetry/span_processors/thread_pool_span_processor.py", line 19>)
-               140 MAKE_FUNCTION            0
-               142 LOAD_CONST               8 ('ThreadPoolSpanProcessor')
-               144 LOAD_NAME                3 (SpanProcessor)
-               146 PRECALL                  3
-               150 CALL                     3
-               160 STORE_NAME              21 (ThreadPoolSpanProcessor)
-               162 LOAD_CONST               1 (None)
-               164 RETURN_VALUE
+    17         110 PUSH_NULL
+               112 LOAD_NAME                0 (logging)
+               114 LOAD_ATTR               19 (getLogger)
+               124 LOAD_NAME               20 (__name__)
+               126 PRECALL                  1
+               130 CALL                     1
+               140 STORE_NAME              21 (logger)
+   
+    20         142 PUSH_NULL
+               144 LOAD_BUILD_CLASS
+               146 LOAD_CONST               7 (<code object ThreadPoolSpanProcessor, file "/Users/vuongngo/workspace/agiflow/packages/python/agiflow-sdk/agiflow/opentelemetry/span_processors/thread_pool_span_processor.py", line 20>)
+               148 MAKE_FUNCTION            0
+               150 LOAD_CONST               8 ('ThreadPoolSpanProcessor')
+               152 LOAD_NAME                3 (SpanProcessor)
+               154 PRECALL                  3
+               158 CALL                     3
+               168 STORE_NAME              22 (ThreadPoolSpanProcessor)
+               170 LOAD_CONST               1 (None)
+               172 RETURN_VALUE
    consts
       0
       None
       ('SpanProcessor', 'ReadableSpan', 'Span')
       ('SpanExporter',)
       ('_SUPPRESS_INSTRUMENTATION_KEY', 'Context', 'attach', 'detach', 'set_value')
       ('deque',)
@@ -106,175 +111,223 @@
          flags     : 0
          code
             0x970065005a0164005a0264015a03090009000900641264046504660264
             0584055a050900641364076506640865076a080000000000000000650919
             000000000000000000640964066606640a84055a0a6407650b6409640666
             04640b84045a0c6414640c84045a0d640d84005a0e6415640f650f640965
             106604641084055a11641184005a1264065300
-          19           0 RESUME                   0
+          20           0 RESUME                   0
                        2 LOAD_NAME                0 (__name__)
                        4 STORE_NAME               1 (__module__)
                        6 LOAD_CONST               0 ('ThreadPoolSpanProcessor')
                        8 STORE_NAME               2 (__qualname__)
          
-          20          10 LOAD_CONST               1 ('ThreaPoolSpanProcessor implementation.\n\n    ThreadPoolSpanProcessor is an implementation of `SpanProcessor` that\n    send and forget remote request using threadpool instead of long-running thread.\n\n    Replace BatchSpanProcessor with this in serverless environment if the long-running\n    thread do not consistently send telemetry data and you cannot use SimpleSpanProcessor\n    as it increase the latency of you application.\n    ')
+          21          10 LOAD_CONST               1 ('ThreaPoolSpanProcessor implementation.\n\n    ThreadPoolSpanProcessor is an implementation of `SpanProcessor` that\n    send and forget remote request using threadpool instead of long-running thread.\n\n    Replace BatchSpanProcessor with this in serverless environment if the long-running\n    thread do not consistently send telemetry data and you cannot use SimpleSpanProcessor\n    as it increase the latency of you application.\n    ')
                       12 STORE_NAME               3 (__doc__)
          
-          33          14 NOP
+          34          14 NOP
          
-          34          16 NOP
+          35          16 NOP
          
-          35          18 NOP
+          36          18 NOP
          
-          30          20 LOAD_CONST              18 ((10, 4, 10))
+          31          20 LOAD_CONST              18 ((10, 4, 10))
                       22 LOAD_CONST               4 ('span_exporter')
          
-          32          24 LOAD_NAME                4 (SpanExporter)
+          33          24 LOAD_NAME                4 (SpanExporter)
          
-          30          26 BUILD_TUPLE              2
-                      28 LOAD_CONST               5 (<code object __init__, file "/Users/vuongngo/workspace/agiflow/packages/python/agiflow-sdk/agiflow/opentelemetry/span_processors/thread_pool_span_processor.py", line 30>)
+          31          26 BUILD_TUPLE              2
+                      28 LOAD_CONST               5 (<code object __init__, file "/Users/vuongngo/workspace/agiflow/packages/python/agiflow-sdk/agiflow/opentelemetry/span_processors/thread_pool_span_processor.py", line 31>)
                       30 MAKE_FUNCTION            5 (defaults, annotations)
                       32 STORE_NAME               5 (__init__)
          
-          46          34 NOP
+          52          34 NOP
          
-          43          36 LOAD_CONST              19 ((None,))
+          49          36 LOAD_CONST              19 ((None,))
                       38 LOAD_CONST               7 ('span')
          
-          45          40 LOAD_NAME                6 (Span)
+          51          40 LOAD_NAME                6 (Span)
          
-          43          42 LOAD_CONST               8 ('parent_context')
+          49          42 LOAD_CONST               8 ('parent_context')
          
-          46          44 LOAD_NAME                7 (typing)
+          52          44 LOAD_NAME                7 (typing)
                       46 LOAD_ATTR                8 (Optional)
                       56 LOAD_NAME                9 (Context)
                       58 BINARY_SUBSCR
          
-          43          68 LOAD_CONST               9 ('return')
+          49          68 LOAD_CONST               9 ('return')
          
-          47          70 LOAD_CONST               6 (None)
+          53          70 LOAD_CONST               6 (None)
          
-          43          72 BUILD_TUPLE              6
-                      74 LOAD_CONST              10 (<code object on_start, file "/Users/vuongngo/workspace/agiflow/packages/python/agiflow-sdk/agiflow/opentelemetry/span_processors/thread_pool_span_processor.py", line 43>)
+          49          72 BUILD_TUPLE              6
+                      74 LOAD_CONST              10 (<code object on_start, file "/Users/vuongngo/workspace/agiflow/packages/python/agiflow-sdk/agiflow/opentelemetry/span_processors/thread_pool_span_processor.py", line 49>)
                       76 MAKE_FUNCTION            5 (defaults, annotations)
                       78 STORE_NAME              10 (on_start)
          
-          50          80 LOAD_CONST               7 ('span')
+          56          80 LOAD_CONST               7 ('span')
                       82 LOAD_NAME               11 (ReadableSpan)
                       84 LOAD_CONST               9 ('return')
                       86 LOAD_CONST               6 (None)
                       88 BUILD_TUPLE              4
-                      90 LOAD_CONST              11 (<code object on_end, file "/Users/vuongngo/workspace/agiflow/packages/python/agiflow-sdk/agiflow/opentelemetry/span_processors/thread_pool_span_processor.py", line 50>)
+                      90 LOAD_CONST              11 (<code object on_end, file "/Users/vuongngo/workspace/agiflow/packages/python/agiflow-sdk/agiflow/opentelemetry/span_processors/thread_pool_span_processor.py", line 56>)
                       92 MAKE_FUNCTION            4 (annotations)
                       94 STORE_NAME              12 (on_end)
          
-          58          96 LOAD_CONST              20 (('return', None))
-                      98 LOAD_CONST              12 (<code object shutdown, file "/Users/vuongngo/workspace/agiflow/packages/python/agiflow-sdk/agiflow/opentelemetry/span_processors/thread_pool_span_processor.py", line 58>)
+          64          96 LOAD_CONST              20 (('return', None))
+                      98 LOAD_CONST              12 (<code object shutdown, file "/Users/vuongngo/workspace/agiflow/packages/python/agiflow-sdk/agiflow/opentelemetry/span_processors/thread_pool_span_processor.py", line 64>)
                      100 MAKE_FUNCTION            4 (annotations)
                      102 STORE_NAME              13 (shutdown)
          
-          61         104 LOAD_CONST              13 (<code object _export, file "/Users/vuongngo/workspace/agiflow/packages/python/agiflow-sdk/agiflow/opentelemetry/span_processors/thread_pool_span_processor.py", line 61>)
+          67         104 LOAD_CONST              13 (<code object _export, file "/Users/vuongngo/workspace/agiflow/packages/python/agiflow-sdk/agiflow/opentelemetry/span_processors/thread_pool_span_processor.py", line 67>)
                      106 MAKE_FUNCTION            0
                      108 STORE_NAME              14 (_export)
          
-          64         110 LOAD_CONST              21 ((30000,))
+          70         110 LOAD_CONST              21 ((30000,))
                      112 LOAD_CONST              15 ('timeout_millis')
                      114 LOAD_NAME               15 (int)
                      116 LOAD_CONST               9 ('return')
                      118 LOAD_NAME               16 (bool)
                      120 BUILD_TUPLE              4
-                     122 LOAD_CONST              16 (<code object force_flush, file "/Users/vuongngo/workspace/agiflow/packages/python/agiflow-sdk/agiflow/opentelemetry/span_processors/thread_pool_span_processor.py", line 64>)
+                     122 LOAD_CONST              16 (<code object force_flush, file "/Users/vuongngo/workspace/agiflow/packages/python/agiflow-sdk/agiflow/opentelemetry/span_processors/thread_pool_span_processor.py", line 70>)
                      124 MAKE_FUNCTION            5 (defaults, annotations)
                      126 STORE_NAME              17 (force_flush)
          
-          71         128 LOAD_CONST              17 (<code object wait_for_flush, file "/Users/vuongngo/workspace/agiflow/packages/python/agiflow-sdk/agiflow/opentelemetry/span_processors/thread_pool_span_processor.py", line 71>)
+          77         128 LOAD_CONST              17 (<code object wait_for_flush, file "/Users/vuongngo/workspace/agiflow/packages/python/agiflow-sdk/agiflow/opentelemetry/span_processors/thread_pool_span_processor.py", line 77>)
                      130 MAKE_FUNCTION            0
                      132 STORE_NAME              18 (wait_for_flush)
                      134 LOAD_CONST               6 (None)
                      136 RETURN_VALUE
          consts
             'ThreadPoolSpanProcessor'
             'ThreaPoolSpanProcessor implementation.\n\n    ThreadPoolSpanProcessor is an implementation of `SpanProcessor` that\n    send and forget remote request using threadpool instead of long-running thread.\n\n    Replace BatchSpanProcessor with this in serverless environment if the long-running\n    thread do not consistently send telemetry data and you cannot use SimpleSpanProcessor\n    as it increase the latency of you application.\n    '
             10
             4
             'span_exporter'
             code
                argcount  : 5
-               nlocals   : 5
+               nlocals   : 6
                stacksize : 4
                flags     : 3
                code
                   0x97007401000000000000000000007c03a6010000ab0100000000000000
                   007c005f0100000000000000007c027c005f020000000000000000740700
                   00000000000000000067007c04a6020000ab0200000000000000007c005f
                   0400000000000000007c017c005f05000000000000000067007c005f0600
-                  0000000000000064005300
-                30           0 RESUME                   0
+                  000000000000000900740f000000000000000000006a0800000000000000
+                  007c006a090000000000000000a6010000ab010000000000000000010064
+                  0053002300741400000000000000000000240072257d0574160000000000
+                  0000000000a00c00000000000000000000000000000000000000007c05a6
+                  010000ab0100000000000000000100590064007d057e056400530064007d
+                  057e0577017700780359007701
+                31           0 RESUME                   0
                
-                37           2 LOAD_GLOBAL              1 (NULL + Pool)
+                38           2 LOAD_GLOBAL              1 (NULL + Pool)
                             14 LOAD_FAST                3 (pool_size)
                             16 PRECALL                  1
                             20 CALL                     1
                             30 LOAD_FAST                0 (self)
                             32 STORE_ATTR               1 (pool)
                
-                38          42 LOAD_FAST                2 (max_queue_size)
+                39          42 LOAD_FAST                2 (max_queue_size)
                             44 LOAD_FAST                0 (self)
                             46 STORE_ATTR               2 (max_queue_size)
                
-                39          56 LOAD_GLOBAL              7 (NULL + deque)
+                40          56 LOAD_GLOBAL              7 (NULL + deque)
                             68 BUILD_LIST               0
                             70 LOAD_FAST                4 (pool_queue_size)
                             72 PRECALL                  2
                             76 CALL                     2
                             86 LOAD_FAST                0 (self)
                             88 STORE_ATTR               4 (futures)
                
-                40          98 LOAD_FAST                1 (span_exporter)
+                41          98 LOAD_FAST                1 (span_exporter)
                            100 LOAD_FAST                0 (self)
                            102 STORE_ATTR               5 (span_exporter)
                
-                41         112 BUILD_LIST               0
+                42         112 BUILD_LIST               0
                            114 LOAD_FAST                0 (self)
                            116 STORE_ATTR               6 (queue)
-                           126 LOAD_CONST               0 (None)
-                           128 RETURN_VALUE
+               
+                44         126 NOP
+               
+                45         128 LOAD_GLOBAL             15 (NULL + atexit)
+                           140 LOAD_ATTR                8 (register)
+                           150 LOAD_FAST                0 (self)
+                           152 LOAD_ATTR                9 (wait_for_flush)
+                           162 PRECALL                  1
+                           166 CALL                     1
+                           176 POP_TOP
+                           178 LOAD_CONST               0 (None)
+                           180 RETURN_VALUE
+                       >>  182 PUSH_EXC_INFO
+               
+                46         184 LOAD_GLOBAL             20 (Exception)
+                           196 CHECK_EXC_MATCH
+                           198 POP_JUMP_FORWARD_IF_FALSE    37 (to 274)
+                           200 STORE_FAST               5 (e)
+               
+                47         202 LOAD_GLOBAL             22 (logger)
+                           214 LOAD_METHOD             12 (warn)
+                           236 LOAD_FAST                5 (e)
+                           238 PRECALL                  1
+                           242 CALL                     1
+                           252 POP_TOP
+                           254 POP_EXCEPT
+                           256 LOAD_CONST               0 (None)
+                           258 STORE_FAST               5 (e)
+                           260 DELETE_FAST              5 (e)
+                           262 LOAD_CONST               0 (None)
+                           264 RETURN_VALUE
+                       >>  266 LOAD_CONST               0 (None)
+                           268 STORE_FAST               5 (e)
+                           270 DELETE_FAST              5 (e)
+                           272 RERAISE                  1
+               
+                46     >>  274 RERAISE                  0
+                       >>  276 COPY                     3
+                           278 POP_EXCEPT
+                           280 RERAISE                  1
+               ExceptionTable:
+                 128 to 176 -> 182 [0]
+                 182 to 200 -> 276 [1] lasti
+                 202 to 252 -> 266 [1] lasti
+                 266 to 274 -> 276 [1] lasti
                consts
                   None
-               names      ('Pool', 'pool', 'max_queue_size', 'deque', 'futures', 'span_exporter', 'queue')
-               varnames   ('self', 'span_exporter', 'max_queue_size', 'pool_size', 'pool_queue_size')
+               names      ('Pool', 'pool', 'max_queue_size', 'deque', 'futures', 'span_exporter', 'queue', 'atexit', 'register', 'wait_for_flush', 'Exception', 'logger', 'warn')
+               varnames   ('self', 'span_exporter', 'max_queue_size', 'pool_size', 'pool_queue_size', 'e')
                freevars   ()
                cellvars   ()
                filename   '/Users/vuongngo/workspace/agiflow/packages/python/agiflow-sdk/agiflow/opentelemetry/span_processors/thread_pool_span_processor.py'
                name       '__init__'
-               firstlineno 30
-               lnotab 0x020728010e012a010e01
+               firstlineno 31
+               lnotab 0x020728010e012a010e010e0202013801120148ff
             None
             'span'
             'parent_context'
             'return'
             code
                argcount  : 3
                nlocals   : 3
                stacksize : 1
                flags     : 3
                code 0x970064005300
-                43           0 RESUME                   0
+                49           0 RESUME                   0
                
-                48           2 LOAD_CONST               0 (None)
+                54           2 LOAD_CONST               0 (None)
                              4 RETURN_VALUE
                consts
                   None
                names      ()
                varnames   ('self', 'span', 'parent_context')
                freevars   ()
                cellvars   ()
                filename   '/Users/vuongngo/workspace/agiflow/packages/python/agiflow-sdk/agiflow/opentelemetry/span_processors/thread_pool_span_processor.py'
                name       'on_start'
-               firstlineno 43
+               firstlineno 49
                lnotab 0x0205
             code
                argcount  : 2
                nlocals   : 3
                stacksize : 6
                flags     : 3
                code
@@ -286,45 +339,45 @@
                   00ab0100000000000000007c006a0600000000000000006b020000000072
                   447c006a070000000000000000a004000000000000000000000000000000
                   00000000007c006a080000000000000000a0090000000000000000000000
                   0000000000000000007c006a0a00000000000000007c006a030000000000
                   000000a6020000ab020000000000000000a6010000ab0100000000000000
                   00010067007c005f0300000000000000007417000000000000000000007c
                   02a6010000ab010000000000000000010064005300
-                50           0 RESUME                   0
+                56           0 RESUME                   0
                
-                51           2 LOAD_GLOBAL              1 (NULL + attach)
+                57           2 LOAD_GLOBAL              1 (NULL + attach)
                             14 LOAD_GLOBAL              3 (NULL + set_value)
                             26 LOAD_GLOBAL              4 (_SUPPRESS_INSTRUMENTATION_KEY)
                             38 LOAD_CONST               1 (True)
                             40 PRECALL                  2
                             44 CALL                     2
                             54 PRECALL                  1
                             58 CALL                     1
                             68 STORE_FAST               2 (token)
                
-                52          70 LOAD_FAST                0 (self)
+                58          70 LOAD_FAST                0 (self)
                             72 LOAD_ATTR                3 (queue)
                             82 LOAD_METHOD              4 (append)
                            104 LOAD_FAST                1 (span)
                            106 PRECALL                  1
                            110 CALL                     1
                            120 POP_TOP
                
-                53         122 LOAD_GLOBAL             11 (NULL + len)
+                59         122 LOAD_GLOBAL             11 (NULL + len)
                            134 LOAD_FAST                0 (self)
                            136 LOAD_ATTR                3 (queue)
                            146 PRECALL                  1
                            150 CALL                     1
                            160 LOAD_FAST                0 (self)
                            162 LOAD_ATTR                6 (max_queue_size)
                            172 COMPARE_OP               2 (==)
                            178 POP_JUMP_FORWARD_IF_FALSE    68 (to 316)
                
-                54         180 LOAD_FAST                0 (self)
+                60         180 LOAD_FAST                0 (self)
                            182 LOAD_ATTR                7 (futures)
                            192 LOAD_METHOD              4 (append)
                            214 LOAD_FAST                0 (self)
                            216 LOAD_ATTR                8 (pool)
                            226 LOAD_METHOD              9 (apply_async)
                            248 LOAD_FAST                0 (self)
                            250 LOAD_ATTR               10 (_export)
@@ -332,19 +385,19 @@
                            262 LOAD_ATTR                3 (queue)
                            272 PRECALL                  2
                            276 CALL                     2
                            286 PRECALL                  1
                            290 CALL                     1
                            300 POP_TOP
                
-                55         302 BUILD_LIST               0
+                61         302 BUILD_LIST               0
                            304 LOAD_FAST                0 (self)
                            306 STORE_ATTR               3 (queue)
                
-                56     >>  316 LOAD_GLOBAL             23 (NULL + detach)
+                62     >>  316 LOAD_GLOBAL             23 (NULL + detach)
                            328 LOAD_FAST                2 (token)
                            330 PRECALL                  1
                            334 CALL                     1
                            344 POP_TOP
                            346 LOAD_CONST               0 (None)
                            348 RETURN_VALUE
                consts
@@ -352,27 +405,27 @@
                   True
                names      ('attach', 'set_value', '_SUPPRESS_INSTRUMENTATION_KEY', 'queue', 'append', 'len', 'max_queue_size', 'futures', 'pool', 'apply_async', '_export', 'detach')
                varnames   ('self', 'span', 'token')
                freevars   ()
                cellvars   ()
                filename   '/Users/vuongngo/workspace/agiflow/packages/python/agiflow-sdk/agiflow/opentelemetry/span_processors/thread_pool_span_processor.py'
                name       'on_end'
-               firstlineno 50
+               firstlineno 56
                lnotab 0x0201440134013a017a010e01
             code
                argcount  : 1
                nlocals   : 1
                stacksize : 2
                flags     : 3
                code
                   0x97007c006a000000000000000000a00100000000000000000000000000
                   00000000000000a6000000ab000000000000000000010064005300
-                58           0 RESUME                   0
+                64           0 RESUME                   0
                
-                59           2 LOAD_FAST                0 (self)
+                65           2 LOAD_FAST                0 (self)
                              4 LOAD_ATTR                0 (span_exporter)
                             14 LOAD_METHOD              1 (shutdown)
                             36 PRECALL                  0
                             40 CALL                     0
                             50 POP_TOP
                             52 LOAD_CONST               0 (None)
                             54 RETURN_VALUE
@@ -380,27 +433,27 @@
                   None
                names      ('span_exporter', 'shutdown')
                varnames   ('self',)
                freevars   ()
                cellvars   ()
                filename   '/Users/vuongngo/workspace/agiflow/packages/python/agiflow-sdk/agiflow/opentelemetry/span_processors/thread_pool_span_processor.py'
                name       'shutdown'
-               firstlineno 58
+               firstlineno 64
                lnotab 0x0201
             code
                argcount  : 1
                nlocals   : 2
                stacksize : 3
                flags     : 7
                code
                   0x97007c006a000000000000000000a00100000000000000000000000000
                   000000000000007c01a6010000ab010000000000000000010064005300
-                61           0 RESUME                   0
+                67           0 RESUME                   0
                
-                62           2 LOAD_FAST                0 (self)
+                68           2 LOAD_FAST                0 (self)
                              4 LOAD_ATTR                0 (span_exporter)
                             14 LOAD_METHOD              1 (export)
                             36 LOAD_FAST                1 (seq)
                             38 PRECALL                  1
                             42 CALL                     1
                             52 POP_TOP
                             54 LOAD_CONST               0 (None)
@@ -409,15 +462,15 @@
                   None
                names      ('span_exporter', 'export')
                varnames   ('self', 'seq')
                freevars   ()
                cellvars   ()
                filename   '/Users/vuongngo/workspace/agiflow/packages/python/agiflow-sdk/agiflow/opentelemetry/span_processors/thread_pool_span_processor.py'
                name       '_export'
-               firstlineno 61
+               firstlineno 67
                lnotab 0x0201
             30000
             'timeout_millis'
             code
                argcount  : 2
                nlocals   : 2
                stacksize : 6
@@ -426,26 +479,26 @@
                   0x97007401000000000000000000007c006a010000000000000000a60100
                   00ab01000000000000000064016b030000000072447c006a020000000000
                   000000a00300000000000000000000000000000000000000007c006a0400
                   00000000000000a00500000000000000000000000000000000000000007c
                   006a0600000000000000007c006a010000000000000000a6020000ab0200
                   00000000000000a6010000ab010000000000000000010067007c005f0100
                   0000000000000064025300
-                64           0 RESUME                   0
+                70           0 RESUME                   0
                
-                65           2 LOAD_GLOBAL              1 (NULL + len)
+                71           2 LOAD_GLOBAL              1 (NULL + len)
                             14 LOAD_FAST                0 (self)
                             16 LOAD_ATTR                1 (queue)
                             26 PRECALL                  1
                             30 CALL                     1
                             40 LOAD_CONST               1 (0)
                             42 COMPARE_OP               3 (!=)
                             48 POP_JUMP_FORWARD_IF_FALSE    68 (to 186)
                
-                66          50 LOAD_FAST                0 (self)
+                72          50 LOAD_FAST                0 (self)
                             52 LOAD_ATTR                2 (futures)
                             62 LOAD_METHOD              3 (append)
                             84 LOAD_FAST                0 (self)
                             86 LOAD_ATTR                4 (pool)
                             96 LOAD_METHOD              5 (apply_async)
                            118 LOAD_FAST                0 (self)
                            120 LOAD_ATTR                6 (_export)
@@ -453,31 +506,31 @@
                            132 LOAD_ATTR                1 (queue)
                            142 PRECALL                  2
                            146 CALL                     2
                            156 PRECALL                  1
                            160 CALL                     1
                            170 POP_TOP
                
-                67         172 BUILD_LIST               0
+                73         172 BUILD_LIST               0
                            174 LOAD_FAST                0 (self)
                            176 STORE_ATTR               1 (queue)
                
-                69     >>  186 LOAD_CONST               2 (True)
+                75     >>  186 LOAD_CONST               2 (True)
                            188 RETURN_VALUE
                consts
                   None
                   0
                   True
                names      ('len', 'queue', 'futures', 'append', 'pool', 'apply_async', '_export')
                varnames   ('self', 'timeout_millis')
                freevars   ()
                cellvars   ()
                filename   '/Users/vuongngo/workspace/agiflow/packages/python/agiflow-sdk/agiflow/opentelemetry/span_processors/thread_pool_span_processor.py'
                name       'force_flush'
-               firstlineno 64
+               firstlineno 70
                lnotab 0x020130017a010e02
             code
                argcount  : 1
                nlocals   : 4
                stacksize : 4
                flags     : 3
                code
@@ -485,47 +538,47 @@
                   0000000000000000000000000000000000a6000000ab0000000000000000
                   007d02740400000000000000000000a00300000000000000000000000000
                   000000000000007c02a6010000ab01000000000000000001008c316e3123
                   00740800000000000000000000240072247d037404000000000000000000
                   00a00500000000000000000000000000000000000000007c03a6010000ab
                   0100000000000000000100590064007d037e036e0864007d037e03770177
                   0078035900770167007c005f00000000000000000064005300
-                71           0 RESUME                   0
+                77           0 RESUME                   0
                
-                72           2 NOP
+                78           2 NOP
                
-                73           4 LOAD_FAST                0 (self)
+                79           4 LOAD_FAST                0 (self)
                              6 LOAD_ATTR                0 (futures)
                             16 GET_ITER
                        >>   18 FOR_ITER                48 (to 116)
                             20 STORE_FAST               1 (future)
                
-                74          22 LOAD_FAST                1 (future)
+                80          22 LOAD_FAST                1 (future)
                             24 LOAD_METHOD              1 (get)
                             46 PRECALL                  0
                             50 CALL                     0
                             60 STORE_FAST               2 (res)
                
-                75          62 LOAD_GLOBAL              4 (logger)
+                81          62 LOAD_GLOBAL              4 (logger)
                             74 LOAD_METHOD              3 (info)
                             96 LOAD_FAST                2 (res)
                             98 PRECALL                  1
                            102 CALL                     1
                            112 POP_TOP
                            114 JUMP_BACKWARD           49 (to 18)
                
-                73     >>  116 JUMP_FORWARD            49 (to 216)
+                79     >>  116 JUMP_FORWARD            49 (to 216)
                        >>  118 PUSH_EXC_INFO
                
-                76         120 LOAD_GLOBAL              8 (Exception)
+                82         120 LOAD_GLOBAL              8 (Exception)
                            132 CHECK_EXC_MATCH
                            134 POP_JUMP_FORWARD_IF_FALSE    36 (to 208)
                            136 STORE_FAST               3 (e)
                
-                77         138 LOAD_GLOBAL              4 (logger)
+                83         138 LOAD_GLOBAL              4 (logger)
                            150 LOAD_METHOD              5 (error)
                            172 LOAD_FAST                3 (e)
                            174 PRECALL                  1
                            178 CALL                     1
                            188 POP_TOP
                            190 POP_EXCEPT
                            192 LOAD_CONST               0 (None)
@@ -533,20 +586,20 @@
                            196 DELETE_FAST              3 (e)
                            198 JUMP_FORWARD             8 (to 216)
                        >>  200 LOAD_CONST               0 (None)
                            202 STORE_FAST               3 (e)
                            204 DELETE_FAST              3 (e)
                            206 RERAISE                  1
                
-                76     >>  208 RERAISE                  0
+                82     >>  208 RERAISE                  0
                        >>  210 COPY                     3
                            212 POP_EXCEPT
                            214 RERAISE                  1
                
-                79     >>  216 BUILD_LIST               0
+                85     >>  216 BUILD_LIST               0
                            218 LOAD_FAST                0 (self)
                            220 STORE_ATTR               0 (futures)
                            230 LOAD_CONST               0 (None)
                            232 RETURN_VALUE
                ExceptionTable:
                  4 to 114 -> 118 [0]
                  118 to 136 -> 210 [1] lasti
@@ -556,32 +609,32 @@
                   None
                names      ('futures', 'get', 'logger', 'info', 'Exception', 'error')
                varnames   ('self', 'future', 'res', 'e')
                freevars   ()
                cellvars   ()
                filename   '/Users/vuongngo/workspace/agiflow/packages/python/agiflow-sdk/agiflow/opentelemetry/span_processors/thread_pool_span_processor.py'
                name       'wait_for_flush'
-               firstlineno 71
+               firstlineno 77
                lnotab 0x020102011201280136fe0403120146ff0803
             (10, 4, 10)
             (None,)
             ('return', None)
             (30000,)
          names      ('__name__', '__module__', '__qualname__', '__doc__', 'SpanExporter', '__init__', 'Span', 'typing', 'Optional', 'Context', 'on_start', 'ReadableSpan', 'on_end', 'shutdown', '_export', 'int', 'bool', 'force_flush', 'wait_for_flush')
          varnames   ()
          freevars   ()
          cellvars   ()
          filename   '/Users/vuongngo/workspace/agiflow/packages/python/agiflow-sdk/agiflow/opentelemetry/span_processors/thread_pool_span_processor.py'
          name       'ThreadPoolSpanProcessor'
-         firstlineno 19
+         firstlineno 20
          lnotab
-            0x0a01040d0201020102fb040202fe081002fd040202fe020318fd020402
+            0x0a01040d0201020102fb040202fe081502fd040202fe020318fd020402
             fc08071008080306031207
       'ThreadPoolSpanProcessor'
-   names      ('logging', 'typing', 'opentelemetry.sdk.trace', 'SpanProcessor', 'ReadableSpan', 'Span', 'opentelemetry.sdk.trace.export', 'SpanExporter', 'opentelemetry.context', '_SUPPRESS_INSTRUMENTATION_KEY', 'Context', 'attach', 'detach', 'set_value', 'collections', 'deque', 'multiprocessing.dummy', 'Pool', 'getLogger', '__name__', 'logger', 'ThreadPoolSpanProcessor')
+   names      ('logging', 'typing', 'opentelemetry.sdk.trace', 'SpanProcessor', 'ReadableSpan', 'Span', 'opentelemetry.sdk.trace.export', 'SpanExporter', 'opentelemetry.context', '_SUPPRESS_INSTRUMENTATION_KEY', 'Context', 'attach', 'detach', 'set_value', 'collections', 'deque', 'multiprocessing.dummy', 'Pool', 'atexit', 'getLogger', '__name__', 'logger', 'ThreadPoolSpanProcessor')
    varnames   ()
    freevars   ()
    cellvars   ()
    filename   '/Users/vuongngo/workspace/agiflow/packages/python/agiflow-sdk/agiflow/opentelemetry/span_processors/thread_pool_span_processor.py'
    name       '<module>'
    firstlineno 1
-   lnotab 0x00ff02010801080214010c011c070c010c022003
+   lnotab 0x00ff02010801080214010c011c070c010c0108022003
```

### Comparing `agiflow_sdk-0.0.3/agiflow/opentelemetry/span_processors/thread_pool_span_processor.py` & `agiflow_sdk-0.0.4/agiflow/opentelemetry/span_processors/thread_pool_span_processor.py`

 * *Files 8% similar despite different names*

```diff
@@ -8,14 +8,15 @@
     Context,
     attach,
     detach,
     set_value,
 )
 from collections import deque
 from multiprocessing.dummy import Pool
+import atexit
 
 logger = logging.getLogger(__name__)
 
 
 class ThreadPoolSpanProcessor(SpanProcessor):
     """ThreaPoolSpanProcessor implementation.
 
@@ -35,14 +36,19 @@
         pool_queue_size=10
     ):
         self.pool = Pool(pool_size)
         self.max_queue_size = max_queue_size
         self.futures = deque([], pool_queue_size)
         self.span_exporter = span_exporter
         self.queue = []
+        # Wait for all requests to be finished before shutdown
+        try:
+            atexit.register(self.wait_for_flush)
+        except Exception as e:
+            logger.warn(e)
 
     def on_start(
         self,
         span: Span,
         parent_context: typing.Optional[Context] = None
     ) -> None:
         pass
```

### Comparing `agiflow_sdk-0.0.3/agiflow/opentelemetry/trace_decorators/__init__.py` & `agiflow_sdk-0.0.4/agiflow/opentelemetry/trace_decorators/__init__.py`

 * *Files identical despite different names*

### Comparing `agiflow_sdk-0.0.3/agiflow/opentelemetry/trace_decorators/__pycache__/__init__.cpython-311.pyc` & `agiflow_sdk-0.0.4/agiflow/opentelemetry/trace_decorators/__pycache__/__init__.cpython-311.pyc`

 * *Files 1% similar despite different names*

#### Python bytecode

```diff
@@ -1,9 +1,9 @@
 magic:    0xa70d0d0a
-moddate:  0x1d945b66 (Sat Jun  1 21:35:25 2024 UTC)
+moddate:  0x47d85b66 (Sun Jun  2 02:26:15 2024 UTC)
 files sz: 644
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 2
    flags     : 0
    code
```

### Comparing `agiflow_sdk-0.0.3/agiflow/opentelemetry/trace_decorators/__pycache__/helper.cpython-311.pyc` & `agiflow_sdk-0.0.4/agiflow/opentelemetry/trace_decorators/__pycache__/helper.cpython-311.pyc`

 * *Files 21% similar despite different names*

#### Python bytecode

```diff
@@ -1,177 +1,160 @@
 magic:    0xa70d0d0a
-moddate:  0xeb065b66 (Sat Jun  1 11:32:59 2024 UTC)
-files sz: 1657
+moddate:  0x6a425c66 (Sun Jun  2 09:59:06 2024 UTC)
+files sz: 1650
 code
    argcount  : 0
    nlocals   : 0
-   stacksize : 6
+   stacksize : 5
    flags     : 0
    code
-      0x9700640064016c006d015a016d025a026d035a036d045a040100640064
-      026c056d065a066d075a070100640064036c086d095a0901000200470064
-      04840064056504a6030000ab0300000000000000005a0a02004700640684
-      006407650aa6030000ab0300000000000000005a0b09000900640c640965
-      02650c19000000000000000000640a650265071900000000000000000066
-      04640b84055a0d64085300
+      0x9700640064016c006d015a016d025a026d035a030100640064026c046d
+      055a056d065a060100020047006403840064046503a6030000ab03000000
+      00000000005a07020047006405840064066507a6030000ab030000000000
+      0000005a0864075300
      0           0 RESUME                   0
    
      1           2 LOAD_CONST               0 (0)
-                 4 LOAD_CONST               1 (('NotRequired', 'Optional', 'Callable', 'TypedDict'))
+                 4 LOAD_CONST               1 (('NotRequired', 'Callable', 'TypedDict'))
                  6 IMPORT_NAME              0 (typing)
                  8 IMPORT_FROM              1 (NotRequired)
                 10 STORE_NAME               1 (NotRequired)
-                12 IMPORT_FROM              2 (Optional)
-                14 STORE_NAME               2 (Optional)
-                16 IMPORT_FROM              3 (Callable)
-                18 STORE_NAME               3 (Callable)
-                20 IMPORT_FROM              4 (TypedDict)
-                22 STORE_NAME               4 (TypedDict)
-                24 POP_TOP
-   
-     2          26 LOAD_CONST               0 (0)
-                28 LOAD_CONST               2 (('set_prompt_settings_context', 'PromptSettings'))
-                30 IMPORT_NAME              5 (agiflow.opentelemetry.context)
-                32 IMPORT_FROM              6 (set_prompt_settings_context)
-                34 STORE_NAME               6 (set_prompt_settings_context)
-                36 IMPORT_FROM              7 (PromptSettings)
-                38 STORE_NAME               7 (PromptSettings)
-                40 POP_TOP
-   
-     3          42 LOAD_CONST               0 (0)
-                44 LOAD_CONST               3 (('AgiflowSpanAttributes',))
-                46 IMPORT_NAME              8 (agiflow.opentelemetry.convention)
-                48 IMPORT_FROM              9 (AgiflowSpanAttributes)
-                50 STORE_NAME               9 (AgiflowSpanAttributes)
-                52 POP_TOP
-   
-     6          54 PUSH_NULL
-                56 LOAD_BUILD_CLASS
-                58 LOAD_CONST               4 (<code object SharedKwargs, file "/Users/vuongngo/workspace/agiflow/packages/python/agiflow-sdk/agiflow/opentelemetry/trace_decorators/helper.py", line 6>)
-                60 MAKE_FUNCTION            0
-                62 LOAD_CONST               5 ('SharedKwargs')
-                64 LOAD_NAME                4 (TypedDict)
-                66 PRECALL                  3
-                70 CALL                     3
-                80 STORE_NAME              10 (SharedKwargs)
-   
-    16          82 PUSH_NULL
-                84 LOAD_BUILD_CLASS
-                86 LOAD_CONST               6 (<code object SharedKwargsWithHooks, file "/Users/vuongngo/workspace/agiflow/packages/python/agiflow-sdk/agiflow/opentelemetry/trace_decorators/helper.py", line 16>)
-                88 MAKE_FUNCTION            0
-                90 LOAD_CONST               7 ('SharedKwargsWithHooks')
-                92 LOAD_NAME               10 (SharedKwargs)
-                94 PRECALL                  3
-                98 CALL                     3
-               108 STORE_NAME              11 (SharedKwargsWithHooks)
-   
-    33         110 NOP
-   
-    34         112 NOP
-   
-    31         114 LOAD_CONST              12 ((None, None))
-               116 LOAD_CONST               9 ('description')
-   
-    33         118 LOAD_NAME                2 (Optional)
-               120 LOAD_NAME               12 (str)
-               122 BINARY_SUBSCR
-   
-    31         132 LOAD_CONST              10 ('prompt_settings')
-   
-    34         134 LOAD_NAME                2 (Optional)
-               136 LOAD_NAME                7 (PromptSettings)
-               138 BINARY_SUBSCR
-   
-    31         148 BUILD_TUPLE              4
-               150 LOAD_CONST              11 (<code object add_extra_spans, file "/Users/vuongngo/workspace/agiflow/packages/python/agiflow-sdk/agiflow/opentelemetry/trace_decorators/helper.py", line 31>)
-               152 MAKE_FUNCTION            5 (defaults, annotations)
-               154 STORE_NAME              13 (add_extra_spans)
-               156 LOAD_CONST               8 (None)
-               158 RETURN_VALUE
+                12 IMPORT_FROM              2 (Callable)
+                14 STORE_NAME               2 (Callable)
+                16 IMPORT_FROM              3 (TypedDict)
+                18 STORE_NAME               3 (TypedDict)
+                20 POP_TOP
+   
+     2          22 LOAD_CONST               0 (0)
+                24 LOAD_CONST               2 (('PromptSettings', 'AssociationProperties'))
+                26 IMPORT_NAME              4 (agiflow.opentelemetry.context)
+                28 IMPORT_FROM              5 (PromptSettings)
+                30 STORE_NAME               5 (PromptSettings)
+                32 IMPORT_FROM              6 (AssociationProperties)
+                34 STORE_NAME               6 (AssociationProperties)
+                36 POP_TOP
+   
+     5          38 PUSH_NULL
+                40 LOAD_BUILD_CLASS
+                42 LOAD_CONST               3 (<code object SharedKwargs, file "/Users/vuongngo/workspace/agiflow/packages/python/agiflow-sdk/agiflow/opentelemetry/trace_decorators/helper.py", line 5>)
+                44 MAKE_FUNCTION            0
+                46 LOAD_CONST               4 ('SharedKwargs')
+                48 LOAD_NAME                3 (TypedDict)
+                50 PRECALL                  3
+                54 CALL                     3
+                64 STORE_NAME               7 (SharedKwargs)
+   
+    20          66 PUSH_NULL
+                68 LOAD_BUILD_CLASS
+                70 LOAD_CONST               5 (<code object SharedKwargsWithHooks, file "/Users/vuongngo/workspace/agiflow/packages/python/agiflow-sdk/agiflow/opentelemetry/trace_decorators/helper.py", line 20>)
+                72 MAKE_FUNCTION            0
+                74 LOAD_CONST               6 ('SharedKwargsWithHooks')
+                76 LOAD_NAME                7 (SharedKwargs)
+                78 PRECALL                  3
+                82 CALL                     3
+                92 STORE_NAME               8 (SharedKwargsWithHooks)
+                94 LOAD_CONST               7 (None)
+                96 RETURN_VALUE
    consts
       0
-      ('NotRequired', 'Optional', 'Callable', 'TypedDict')
-      ('set_prompt_settings_context', 'PromptSettings')
-      ('AgiflowSpanAttributes',)
+      ('NotRequired', 'Callable', 'TypedDict')
+      ('PromptSettings', 'AssociationProperties')
       code
          argcount  : 0
          nlocals   : 0
          stacksize : 3
          flags     : 0
          code
             0x970065005a0164005a0255006503650419000000000000000000650564
-            013c0000006503650619000000000000000000650564023c000000640353
-            00
-           6           0 RESUME                   0
+            013c00000065036506190000000000000000006503650719000000000000
+            0000007a070000650564023c000000650365081900000000000000000065
+            036507190000000000000000007a070000650564033c00000064045300
+           5           0 RESUME                   0
                        2 LOAD_NAME                0 (__name__)
                        4 STORE_NAME               1 (__module__)
                        6 LOAD_CONST               0 ('SharedKwargs')
                        8 STORE_NAME               2 (__qualname__)
                       10 SETUP_ANNOTATIONS
          
-           9          12 LOAD_NAME                3 (NotRequired)
+           8          12 LOAD_NAME                3 (NotRequired)
                       14 LOAD_NAME                4 (str)
                       16 BINARY_SUBSCR
                       26 LOAD_NAME                5 (__annotations__)
                       28 LOAD_CONST               1 ('description')
                       30 STORE_SUBSCR
          
           13          34 LOAD_NAME                3 (NotRequired)
                       36 LOAD_NAME                6 (PromptSettings)
                       38 BINARY_SUBSCR
-                      48 LOAD_NAME                5 (__annotations__)
-                      50 LOAD_CONST               2 ('prompt_settings')
-                      52 STORE_SUBSCR
-                      56 LOAD_CONST               3 (None)
-                      58 RETURN_VALUE
+                      48 LOAD_NAME                3 (NotRequired)
+                      50 LOAD_NAME                7 (Callable)
+                      52 BINARY_SUBSCR
+                      62 BINARY_OP                7 (|)
+                      66 LOAD_NAME                5 (__annotations__)
+                      68 LOAD_CONST               2 ('prompt_settings')
+                      70 STORE_SUBSCR
+         
+          17          74 LOAD_NAME                3 (NotRequired)
+                      76 LOAD_NAME                8 (AssociationProperties)
+                      78 BINARY_SUBSCR
+                      88 LOAD_NAME                3 (NotRequired)
+                      90 LOAD_NAME                7 (Callable)
+                      92 BINARY_SUBSCR
+                     102 BINARY_OP                7 (|)
+                     106 LOAD_NAME                5 (__annotations__)
+                     108 LOAD_CONST               3 ('association_properties')
+                     110 STORE_SUBSCR
+                     114 LOAD_CONST               4 (None)
+                     116 RETURN_VALUE
          consts
             'SharedKwargs'
             'description'
             'prompt_settings'
+            'association_properties'
             None
-         names      ('__name__', '__module__', '__qualname__', 'NotRequired', 'str', '__annotations__', 'PromptSettings')
+         names      ('__name__', '__module__', '__qualname__', 'NotRequired', 'str', '__annotations__', 'PromptSettings', 'Callable', 'AssociationProperties')
          varnames   ()
          freevars   ()
          cellvars   ()
          filename   '/Users/vuongngo/workspace/agiflow/packages/python/agiflow-sdk/agiflow/opentelemetry/trace_decorators/helper.py'
          name       'SharedKwargs'
-         firstlineno 6
-         lnotab 0x0c031604
+         firstlineno 5
+         lnotab 0x0c0316052804
       'SharedKwargs'
       code
          argcount  : 0
          nlocals   : 0
          stacksize : 3
          flags     : 0
          code
             0x970065005a0164005a0255006503650419000000000000000000650564
             013c0000006503650419000000000000000000650564023c000000650365
             0419000000000000000000650564033c00000064045300
-          16           0 RESUME                   0
+          20           0 RESUME                   0
                        2 LOAD_NAME                0 (__name__)
                        4 STORE_NAME               1 (__module__)
                        6 LOAD_CONST               0 ('SharedKwargsWithHooks')
                        8 STORE_NAME               2 (__qualname__)
                       10 SETUP_ANNOTATIONS
          
-          20          12 LOAD_NAME                3 (NotRequired)
+          24          12 LOAD_NAME                3 (NotRequired)
                       14 LOAD_NAME                4 (Callable)
                       16 BINARY_SUBSCR
                       26 LOAD_NAME                5 (__annotations__)
                       28 LOAD_CONST               1 ('input_serializer')
                       30 STORE_SUBSCR
          
-          24          34 LOAD_NAME                3 (NotRequired)
+          28          34 LOAD_NAME                3 (NotRequired)
                       36 LOAD_NAME                4 (Callable)
                       38 BINARY_SUBSCR
                       48 LOAD_NAME                5 (__annotations__)
                       50 LOAD_CONST               2 ('output_serializer')
                       52 STORE_SUBSCR
          
-          28          56 LOAD_NAME                3 (NotRequired)
+          32          56 LOAD_NAME                3 (NotRequired)
                       58 LOAD_NAME                4 (Callable)
                       60 BINARY_SUBSCR
                       70 LOAD_NAME                5 (__annotations__)
                       72 LOAD_CONST               3 ('context_parser')
                       74 STORE_SUBSCR
                       78 LOAD_CONST               4 (None)
                       80 RETURN_VALUE
@@ -183,69 +166,19 @@
             None
          names      ('__name__', '__module__', '__qualname__', 'NotRequired', 'Callable', '__annotations__')
          varnames   ()
          freevars   ()
          cellvars   ()
          filename   '/Users/vuongngo/workspace/agiflow/packages/python/agiflow-sdk/agiflow/opentelemetry/trace_decorators/helper.py'
          name       'SharedKwargsWithHooks'
-         firstlineno 16
+         firstlineno 20
          lnotab 0x0c0416041604
       'SharedKwargsWithHooks'
       None
-      'description'
-      'prompt_settings'
-      code
-         argcount  : 3
-         nlocals   : 3
-         stacksize : 4
-         flags     : 3
-         code
-            0x97007c0181207c00a00000000000000000000000000000000000000000
-            007402000000000000000000006a0200000000000000007c01a6020000ab
-            02000000000000000001007c0281117407000000000000000000007c02a6
-            010000ab01000000000000000001006400530064005300
-          31           0 RESUME                   0
-         
-          36           2 LOAD_FAST                1 (description)
-                       4 POP_JUMP_FORWARD_IF_NONE    32 (to 70)
-         
-          37           6 LOAD_FAST                0 (span)
-                       8 LOAD_METHOD              0 (set_attribute)
-                      30 LOAD_GLOBAL              2 (AgiflowSpanAttributes)
-                      42 LOAD_ATTR                2 (AGIFLOW_ENTITY_DESCRIPTION)
-                      52 LOAD_FAST                1 (description)
-                      54 PRECALL                  2
-                      58 CALL                     2
-                      68 POP_TOP
-         
-          39     >>   70 LOAD_FAST                2 (prompt_settings)
-                      72 POP_JUMP_FORWARD_IF_NONE    17 (to 108)
-         
-          40          74 LOAD_GLOBAL              7 (NULL + set_prompt_settings_context)
-                      86 LOAD_FAST                2 (prompt_settings)
-                      88 PRECALL                  1
-                      92 CALL                     1
-                     102 POP_TOP
-                     104 LOAD_CONST               0 (None)
-                     106 RETURN_VALUE
-         
-          39     >>  108 LOAD_CONST               0 (None)
-                     110 RETURN_VALUE
-         consts
-            None
-         names      ('set_attribute', 'AgiflowSpanAttributes', 'AGIFLOW_ENTITY_DESCRIPTION', 'set_prompt_settings_context')
-         varnames   ('span', 'description', 'prompt_settings')
-         freevars   ()
-         cellvars   ()
-         filename   '/Users/vuongngo/workspace/agiflow/packages/python/agiflow-sdk/agiflow/opentelemetry/trace_decorators/helper.py'
-         name       'add_extra_spans'
-         firstlineno 31
-         lnotab 0x020504014002040122ff
-      (None, None)
-   names      ('typing', 'NotRequired', 'Optional', 'Callable', 'TypedDict', 'agiflow.opentelemetry.context', 'set_prompt_settings_context', 'PromptSettings', 'agiflow.opentelemetry.convention', 'AgiflowSpanAttributes', 'SharedKwargs', 'SharedKwargsWithHooks', 'str', 'add_extra_spans')
+   names      ('typing', 'NotRequired', 'Callable', 'TypedDict', 'agiflow.opentelemetry.context', 'PromptSettings', 'AssociationProperties', 'SharedKwargs', 'SharedKwargsWithHooks')
    varnames   ()
    freevars   ()
    cellvars   ()
    filename   '/Users/vuongngo/workspace/agiflow/packages/python/agiflow-sdk/agiflow/opentelemetry/trace_decorators/helper.py'
    name       '<module>'
    firstlineno 1
-   lnotab 0x00ff0201180110010c031c0a1c11020102fd04020efe02030efd
+   lnotab 0x00ff0201140110031c0f
```

### Comparing `agiflow_sdk-0.0.3/agiflow/opentelemetry/trace_decorators/__pycache__/task.cpython-311.pyc` & `agiflow_sdk-0.0.4/agiflow/opentelemetry/trace_decorators/__pycache__/task.cpython-311.pyc`

 * *Files 0% similar despite different names*

#### Python bytecode

```diff
@@ -1,9 +1,9 @@
 magic:    0xa70d0d0a
-moddate:  0x43985a66 (Sat Jun  1 03:40:51 2024 UTC)
+moddate:  0x47d85b66 (Sun Jun  2 02:26:15 2024 UTC)
 files sz: 3514
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 10
    flags     : 0
    code
```

### Comparing `agiflow_sdk-0.0.3/agiflow/opentelemetry/trace_decorators/__pycache__/workflow.cpython-311.pyc` & `agiflow_sdk-0.0.4/agiflow/opentelemetry/trace_decorators/__pycache__/workflow.cpython-311.pyc`

 * *Files 17% similar despite different names*

#### Python bytecode

```diff
@@ -1,10 +1,10 @@
 magic:    0xa70d0d0a
-moddate:  0x43985a66 (Sat Jun  1 03:40:51 2024 UTC)
-files sz: 2174
+moddate:  0x220c5d66 (Mon Jun  3 00:19:46 2024 UTC)
+files sz: 2241
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 8
    flags     : 0
    code
       0x9700640064016c006d015a016d025a020100640064026c036d045a046d
@@ -79,73 +79,73 @@
                104 MAKE_FUNCTION            0
                106 LOAD_CONST               8 ('WorkflowSpanCapture')
                108 LOAD_NAME               11 (BaseSpanCapture)
                110 PRECALL                  3
                114 CALL                     3
                124 STORE_NAME              18 (WorkflowSpanCapture)
    
-    33         126 LOAD_CONST               9 (None)
+    37         126 LOAD_CONST               9 (None)
    
-    34         128 LOAD_CONST               9 (None)
+    38         128 LOAD_CONST               9 (None)
    
-    35         130 LOAD_NAME               17 (SpanKind)
+    39         130 LOAD_NAME               17 (SpanKind)
                132 LOAD_ATTR               19 (INTERNAL)
    
-    32         142 BUILD_TUPLE              3
+    36         142 BUILD_TUPLE              3
                144 LOAD_CONST              10 ('name')
    
-    33         146 LOAD_NAME                1 (Optional)
+    37         146 LOAD_NAME                1 (Optional)
                148 LOAD_NAME               20 (str)
                150 BINARY_SUBSCR
    
-    32         160 LOAD_CONST              11 ('method_name')
+    36         160 LOAD_CONST              11 ('method_name')
    
-    34         162 LOAD_NAME                1 (Optional)
+    38         162 LOAD_NAME                1 (Optional)
                164 LOAD_NAME               20 (str)
                166 BINARY_SUBSCR
    
-    32         176 LOAD_CONST              12 ('kwargs')
+    36         176 LOAD_CONST              12 ('kwargs')
    
-    36         178 LOAD_NAME                2 (Unpack)
+    40         178 LOAD_NAME                2 (Unpack)
                180 LOAD_NAME                9 (SharedKwargsWithHooks)
                182 BINARY_SUBSCR
    
-    32         192 BUILD_TUPLE              6
-               194 LOAD_CONST              13 (<code object workflow, file "/Users/vuongngo/workspace/agiflow/packages/python/agiflow-sdk/agiflow/opentelemetry/trace_decorators/workflow.py", line 32>)
+    36         192 BUILD_TUPLE              6
+               194 LOAD_CONST              13 (<code object workflow, file "/Users/vuongngo/workspace/agiflow/packages/python/agiflow-sdk/agiflow/opentelemetry/trace_decorators/workflow.py", line 36>)
                196 MAKE_FUNCTION            5 (defaults, annotations)
                198 STORE_NAME              21 (workflow)
    
-    57         200 LOAD_CONST               9 (None)
+    61         200 LOAD_CONST               9 (None)
    
-    58         202 LOAD_CONST               9 (None)
+    62         202 LOAD_CONST               9 (None)
    
-    59         204 LOAD_NAME               17 (SpanKind)
+    63         204 LOAD_NAME               17 (SpanKind)
                206 LOAD_ATTR               19 (INTERNAL)
    
-    56         216 BUILD_TUPLE              3
+    60         216 BUILD_TUPLE              3
                218 LOAD_CONST              10 ('name')
    
-    57         220 LOAD_NAME                1 (Optional)
+    61         220 LOAD_NAME                1 (Optional)
                222 LOAD_NAME               20 (str)
                224 BINARY_SUBSCR
    
-    56         234 LOAD_CONST              11 ('method_name')
+    60         234 LOAD_CONST              11 ('method_name')
    
-    58         236 LOAD_NAME                1 (Optional)
+    62         236 LOAD_NAME                1 (Optional)
                238 LOAD_NAME               20 (str)
                240 BINARY_SUBSCR
    
-    56         250 LOAD_CONST              12 ('kwargs')
+    60         250 LOAD_CONST              12 ('kwargs')
    
-    60         252 LOAD_NAME                2 (Unpack)
+    64         252 LOAD_NAME                2 (Unpack)
                254 LOAD_NAME                9 (SharedKwargsWithHooks)
                256 BINARY_SUBSCR
    
-    56         266 BUILD_TUPLE              6
-               268 LOAD_CONST              14 (<code object aworkflow, file "/Users/vuongngo/workspace/agiflow/packages/python/agiflow-sdk/agiflow/opentelemetry/trace_decorators/workflow.py", line 56>)
+    60         266 BUILD_TUPLE              6
+               268 LOAD_CONST              14 (<code object aworkflow, file "/Users/vuongngo/workspace/agiflow/packages/python/agiflow-sdk/agiflow/opentelemetry/trace_decorators/workflow.py", line 60>)
                270 MAKE_FUNCTION            5 (defaults, annotations)
                272 STORE_NAME              22 (aworkflow)
                274 LOAD_CONST               9 (None)
                276 RETURN_VALUE
    consts
       0
       ('Optional', 'Unpack')
@@ -157,15 +157,16 @@
       code
          argcount  : 0
          nlocals   : 0
          stacksize : 2
          flags     : 0
          code
             0x8700970065005a0164005a0288006601640184085a0388006601640284
-            085a04880078015a055300
+            085a04650564038400a6000000ab0000000000000000005a06880078015a
+            075300
                        0 MAKE_CELL                0 (__class__)
          
           19           2 RESUME                   0
                        4 LOAD_NAME                0 (__name__)
                        6 STORE_NAME               1 (__module__)
                        8 LOAD_CONST               0 ('WorkflowSpanCapture')
                       10 STORE_NAME               2 (__qualname__)
@@ -177,18 +178,28 @@
                       20 STORE_NAME               3 (__init__)
          
           25          22 LOAD_CLOSURE             0 (__class__)
                       24 BUILD_TUPLE              1
                       26 LOAD_CONST               2 (<code object capture_input, file "/Users/vuongngo/workspace/agiflow/packages/python/agiflow-sdk/agiflow/opentelemetry/trace_decorators/workflow.py", line 25>)
                       28 MAKE_FUNCTION            8 (closure)
                       30 STORE_NAME               4 (capture_input)
-                      32 LOAD_CLOSURE             0 (__class__)
-                      34 COPY                     1
-                      36 STORE_NAME               5 (__classcell__)
-                      38 RETURN_VALUE
+         
+          31          32 LOAD_NAME                5 (staticmethod)
+         
+          32          34 LOAD_CONST               3 (<code object is_flush_on_exit, file "/Users/vuongngo/workspace/agiflow/packages/python/agiflow-sdk/agiflow/opentelemetry/trace_decorators/workflow.py", line 31>)
+                      36 MAKE_FUNCTION            0
+         
+          31          38 PRECALL                  0
+                      42 CALL                     0
+         
+          32          52 STORE_NAME               6 (is_flush_on_exit)
+                      54 LOAD_CLOSURE             0 (__class__)
+                      56 COPY                     1
+                      58 STORE_NAME               7 (__classcell__)
+                      60 RETURN_VALUE
          consts
             'WorkflowSpanCapture'
             code
                argcount  : 1
                nlocals   : 4
                stacksize : 5
                flags     : 15
@@ -281,22 +292,43 @@
                varnames   ('self',)
                freevars   ('__class__',)
                cellvars   ()
                filename   '/Users/vuongngo/workspace/agiflow/packages/python/agiflow-sdk/agiflow/opentelemetry/trace_decorators/workflow.py'
                name       'capture_input'
                firstlineno 25
                lnotab 0x04014001180122ff
-         names      ('__name__', '__module__', '__qualname__', '__init__', 'capture_input', '__classcell__')
+            code
+               argcount  : 0
+               nlocals   : 0
+               stacksize : 1
+               flags     : 3
+               code 0x970064015300
+                31           0 RESUME                   0
+               
+                33           2 LOAD_CONST               1 (True)
+                             4 RETURN_VALUE
+               consts
+                  None
+                  True
+               names      ()
+               varnames   ()
+               freevars   ()
+               cellvars   ()
+               filename   '/Users/vuongngo/workspace/agiflow/packages/python/agiflow-sdk/agiflow/opentelemetry/trace_decorators/workflow.py'
+               name       'is_flush_on_exit'
+               firstlineno 31
+               lnotab 0x0202
+         names      ('__name__', '__module__', '__qualname__', '__init__', 'capture_input', 'staticmethod', 'is_flush_on_exit', '__classcell__')
          varnames   ()
          freevars   ()
          cellvars   ('__class__',)
          filename   '/Users/vuongngo/workspace/agiflow/packages/python/agiflow-sdk/agiflow/opentelemetry/trace_decorators/workflow.py'
          name       'WorkflowSpanCapture'
          firstlineno 19
-         lnotab 0x0c010a05
+         lnotab 0x0c010a050a06020104ff0e01
       'WorkflowSpanCapture'
       None
       'name'
       'method_name'
       'kwargs'
       code
          argcount  : 3
@@ -305,148 +337,148 @@
          flags     : 11
          code
             0x97007c01802074010000000000000000000064027c0074020000000000
             00000000006a0200000000000000007c0274060000000000000000000064
             019c047c03a4018e01530074090000000000000000000064027c00740200
             0000000000000000006a0200000000000000007c02740600000000000000
             00000064019c047c03a4018e015300
-          32           0 RESUME                   0
+          36           0 RESUME                   0
          
-          38           2 LOAD_FAST                1 (method_name)
+          42           2 LOAD_FAST                1 (method_name)
                        4 POP_JUMP_FORWARD_IF_NOT_NONE    32 (to 70)
          
-          39           6 LOAD_GLOBAL              1 (NULL + decorate_method)
+          43           6 LOAD_GLOBAL              1 (NULL + decorate_method)
                       18 LOAD_CONST               2 (())
          
-          40          20 LOAD_FAST                0 (name)
+          44          20 LOAD_FAST                0 (name)
          
-          41          22 LOAD_GLOBAL              2 (AgiflowServiceTypes)
+          45          22 LOAD_GLOBAL              2 (AgiflowServiceTypes)
                       34 LOAD_ATTR                2 (WORKFLOW)
          
-          42          44 LOAD_FAST                2 (span_kind)
+          46          44 LOAD_FAST                2 (span_kind)
          
-          43          46 LOAD_GLOBAL              6 (WorkflowSpanCapture)
+          47          46 LOAD_GLOBAL              6 (WorkflowSpanCapture)
          
-          39          58 LOAD_CONST               1 (('name', 'tlp_service_type', 'span_kind', 'SpanCapture'))
+          43          58 LOAD_CONST               1 (('name', 'tlp_service_type', 'span_kind', 'SpanCapture'))
                       60 BUILD_CONST_KEY_MAP      4
          
-          44          62 LOAD_FAST                3 (kwargs)
+          48          62 LOAD_FAST                3 (kwargs)
          
-          39          64 DICT_MERGE               1
+          43          64 DICT_MERGE               1
                       66 CALL_FUNCTION_EX         1
                       68 RETURN_VALUE
          
-          47     >>   70 LOAD_GLOBAL              9 (NULL + decorate_class_method)
+          51     >>   70 LOAD_GLOBAL              9 (NULL + decorate_class_method)
                       82 LOAD_CONST               2 (())
          
-          48          84 LOAD_FAST                0 (name)
+          52          84 LOAD_FAST                0 (name)
          
-          49          86 LOAD_GLOBAL              2 (AgiflowServiceTypes)
+          53          86 LOAD_GLOBAL              2 (AgiflowServiceTypes)
                       98 LOAD_ATTR                2 (WORKFLOW)
          
-          50         108 LOAD_FAST                2 (span_kind)
+          54         108 LOAD_FAST                2 (span_kind)
          
-          51         110 LOAD_GLOBAL              6 (WorkflowSpanCapture)
+          55         110 LOAD_GLOBAL              6 (WorkflowSpanCapture)
          
-          47         122 LOAD_CONST               1 (('name', 'tlp_service_type', 'span_kind', 'SpanCapture'))
+          51         122 LOAD_CONST               1 (('name', 'tlp_service_type', 'span_kind', 'SpanCapture'))
                      124 BUILD_CONST_KEY_MAP      4
          
-          52         126 LOAD_FAST                3 (kwargs)
+          56         126 LOAD_FAST                3 (kwargs)
          
-          47         128 DICT_MERGE               1
+          51         128 DICT_MERGE               1
                      130 CALL_FUNCTION_EX         1
                      132 RETURN_VALUE
          consts
             None
             ('name', 'tlp_service_type', 'span_kind', 'SpanCapture')
             ()
          names      ('decorate_method', 'AgiflowServiceTypes', 'WORKFLOW', 'WorkflowSpanCapture', 'decorate_class_method')
          varnames   ('name', 'method_name', 'span_kind', 'kwargs')
          freevars   ()
          cellvars   ()
          filename   '/Users/vuongngo/workspace/agiflow/packages/python/agiflow-sdk/agiflow/opentelemetry/trace_decorators/workflow.py'
          name       'workflow'
-         firstlineno 32
+         firstlineno 36
          lnotab
             0x020604010e010201160102010cfc040502fb06080e010201160102010c
             fc040502fb
       code
          argcount  : 3
          nlocals   : 4
          stacksize : 8
          flags     : 11
          code
             0x97007c01802074010000000000000000000064027c0074020000000000
             00000000006a0200000000000000007c0274060000000000000000000064
             019c047c03a4018e01530074090000000000000000000064027c00740200
             0000000000000000006a0200000000000000007c02740600000000000000
             00000064019c047c03a4018e015300
-          56           0 RESUME                   0
+          60           0 RESUME                   0
          
-          62           2 LOAD_FAST                1 (method_name)
+          66           2 LOAD_FAST                1 (method_name)
                        4 POP_JUMP_FORWARD_IF_NOT_NONE    32 (to 70)
          
-          63           6 LOAD_GLOBAL              1 (NULL + adecorate_method)
+          67           6 LOAD_GLOBAL              1 (NULL + adecorate_method)
                       18 LOAD_CONST               2 (())
          
-          64          20 LOAD_FAST                0 (name)
+          68          20 LOAD_FAST                0 (name)
          
-          65          22 LOAD_GLOBAL              2 (AgiflowServiceTypes)
+          69          22 LOAD_GLOBAL              2 (AgiflowServiceTypes)
                       34 LOAD_ATTR                2 (WORKFLOW)
          
-          66          44 LOAD_FAST                2 (span_kind)
+          70          44 LOAD_FAST                2 (span_kind)
          
-          67          46 LOAD_GLOBAL              6 (WorkflowSpanCapture)
+          71          46 LOAD_GLOBAL              6 (WorkflowSpanCapture)
          
-          63          58 LOAD_CONST               1 (('name', 'tlp_service_type', 'span_kind', 'SpanCapture'))
+          67          58 LOAD_CONST               1 (('name', 'tlp_service_type', 'span_kind', 'SpanCapture'))
                       60 BUILD_CONST_KEY_MAP      4
          
-          68          62 LOAD_FAST                3 (kwargs)
+          72          62 LOAD_FAST                3 (kwargs)
          
-          63          64 DICT_MERGE               1
+          67          64 DICT_MERGE               1
                       66 CALL_FUNCTION_EX         1
                       68 RETURN_VALUE
          
-          71     >>   70 LOAD_GLOBAL              9 (NULL + adecorate_class_method)
+          75     >>   70 LOAD_GLOBAL              9 (NULL + adecorate_class_method)
                       82 LOAD_CONST               2 (())
          
-          72          84 LOAD_FAST                0 (name)
+          76          84 LOAD_FAST                0 (name)
          
-          73          86 LOAD_GLOBAL              2 (AgiflowServiceTypes)
+          77          86 LOAD_GLOBAL              2 (AgiflowServiceTypes)
                       98 LOAD_ATTR                2 (WORKFLOW)
          
-          74         108 LOAD_FAST                2 (span_kind)
+          78         108 LOAD_FAST                2 (span_kind)
          
-          75         110 LOAD_GLOBAL              6 (WorkflowSpanCapture)
+          79         110 LOAD_GLOBAL              6 (WorkflowSpanCapture)
          
-          71         122 LOAD_CONST               1 (('name', 'tlp_service_type', 'span_kind', 'SpanCapture'))
+          75         122 LOAD_CONST               1 (('name', 'tlp_service_type', 'span_kind', 'SpanCapture'))
                      124 BUILD_CONST_KEY_MAP      4
          
-          76         126 LOAD_FAST                3 (kwargs)
+          80         126 LOAD_FAST                3 (kwargs)
          
-          71         128 DICT_MERGE               1
+          75         128 DICT_MERGE               1
                      130 CALL_FUNCTION_EX         1
                      132 RETURN_VALUE
          consts
             None
             ('name', 'tlp_service_type', 'span_kind', 'SpanCapture')
             ()
          names      ('adecorate_method', 'AgiflowServiceTypes', 'WORKFLOW', 'WorkflowSpanCapture', 'adecorate_class_method')
          varnames   ('name', 'method_name', 'span_kind', 'kwargs')
          freevars   ()
          cellvars   ()
          filename   '/Users/vuongngo/workspace/agiflow/packages/python/agiflow-sdk/agiflow/opentelemetry/trace_decorators/workflow.py'
          name       'aworkflow'
-         firstlineno 56
+         firstlineno 60
          lnotab
             0x020604010e010201160102010cfc040502fb06080e010201160102010c
             fc040502fb
    names      ('typing', 'Optional', 'Unpack', 'agiflow.opentelemetry.convention', 'SpanAttributes', 'AgiflowServiceTypes', 'agiflow.opentelemetry.context', 'set_workflow_name', 'agiflow.opentelemetry.trace_decorators.helper', 'SharedKwargsWithHooks', 'agiflow.opentelemetry.trace_decorators.wrapper', 'BaseSpanCapture', 'decorate_method', 'decorate_class_method', 'adecorate_method', 'adecorate_class_method', 'opentelemetry.trace', 'SpanKind', 'WorkflowSpanCapture', 'INTERNAL', 'str', 'workflow', 'aworkflow')
    varnames   ()
    freevars   ()
    cellvars   ()
    filename   '/Users/vuongngo/workspace/agiflow/packages/python/agiflow-sdk/agiflow/opentelemetry/trace_decorators/workflow.py'
    name       '<module>'
    firstlineno 1
    lnotab
-      0x00ff0201100210020c010c031c070c031c0e020102010cfd04010eff02
+      0x00ff0201100210020c010c031c070c031c12020102010cfd04010eff02
       020efe02040efc0819020102010cfd04010eff02020efe02040efc
```

### Comparing `agiflow_sdk-0.0.3/agiflow/opentelemetry/trace_decorators/__pycache__/wrapper.cpython-311.pyc` & `agiflow_sdk-0.0.4/agiflow/opentelemetry/trace_decorators/__pycache__/wrapper.cpython-311.pyc`

 * *Files 10% similar despite different names*

#### Python bytecode

```diff
@@ -1,41 +1,41 @@
 magic:    0xa70d0d0a
-moddate:  0x2bd75b66 (Sun Jun  2 02:21:31 2024 UTC)
-files sz: 14099
+moddate:  0x7c105d66 (Mon Jun  3 00:38:20 2024 UTC)
+files sz: 15064
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 10
    flags     : 0
    code
       0x9700640064016c006d015a010100640064026c026d035a030100640064
       036c045a04640064046c056d065a066d075a076d085a086d095a096d0a5a
       0a6d0b5a0b0100640064056c0c6d0d5a0d0100640064066c0e6d0f5a0f01
-      00640064076c106d115a110100640064086c126d135a136d145a146d155a
-      156d165a160100640064096c176d185a1801006400640a6c196d1a5a1a01
-      006400640b6c1b6d1c5a1c01006400640c6c1d6d1e5a1e6d1f5a1f010064
-      00640d6c206d215a216d225a2201006400640e6c236d245a240100640064
-      0f6c256d265a266d275a276d285a286d295a296d2a5a2a6d2b5a2b6d2c5a
-      2c0100640064106c2d6d2e5a2e6d2f5a2f0100020065096411a6010000ab
-      0100000000000000005a30020065046a3100000000000000006532a60100
-      00ab0100000000000000005a33020047006412840064136501650a653019
-      000000000000000000a6040000ab0400000000000000005a340200470064
-      14840064156534a6030000ab0300000000000000005a35640365116a3600
-      0000000000000065146a3700000000000000006535660464166508653819
-      000000000000000000641765086511190000000000000000006418650b65
-      1e190000000000000000006606641984055a39640365116a360000000000
-      00000065146a370000000000000000653566046416650865381900000000
-      0000000000641765086511190000000000000000006418650b651e190000
-      000000000000006606641a84055a3a65116a36000000000000000065146a
-      370000000000000000653566036416650865381900000000000000000064
-      1b653864176508651119000000000000000000641c650b651e1900000000
-      00000000006608641d84055a3b65116a36000000000000000065146a3700
-      000000000000006535660364166508653819000000000000000000641b65
-      3864176508651119000000000000000000641c650b651e19000000000000
-      0000006608641e84055a3c64035300
+      00640064076c106d115a110100640064086c126d135a130100640064096c
+      146d155a156d165a166d175a176d185a1801006400640a6c196d1a5a1a01
+      006400640b6c1b6d1c5a1c01006400640c6c1d6d1e5a1e01006400640d6c
+      1f6d205a2001006400640e6c216d225a226d235a2301006400640f6c246d
+      255a250100640064106c266d275a276d285a286d295a296d2a5a2a6d2b5a
+      2b6d2c5a2c6d2d5a2d0100640064116c2e6d2f5a2f6d305a300100020065
+      096412a6010000ab0100000000000000005a31020065046a320000000000
+      0000006533a6010000ab0100000000000000005a34020047006413840064
+      146501650a653119000000000000000000a6040000ab0400000000000000
+      005a35020047006415840064166535a6030000ab0300000000000000005a
+      36640365136a37000000000000000065166a380000000000000000653666
+      046417650865391900000000000000000064186508651319000000000000
+      0000006419650b6520190000000000000000006606641a84055a3a640365
+      136a37000000000000000065166a38000000000000000065366604641765
+      086539190000000000000000006418650865131900000000000000000064
+      19650b6520190000000000000000006606641b84055a3b65136a37000000
+      000000000065166a38000000000000000065366603641765086539190000
+      00000000000000641c653964186508651319000000000000000000641d65
+      0b6520190000000000000000006608641e84055a3c65136a370000000000
+      00000065166a380000000000000000653666036417650865391900000000
+      0000000000641c653964186508651319000000000000000000641d650b65
+      20190000000000000000006608641f84055a3d64035300
      0           0 RESUME                   0
    
      1           2 LOAD_CONST               0 (0)
                  4 LOAD_CONST               1 (('ABC',))
                  6 IMPORT_NAME              0 (abc)
                  8 IMPORT_FROM              1 (ABC)
                 10 STORE_NAME               1 (ABC)
@@ -81,300 +81,306 @@
                 80 LOAD_CONST               6 (('SpanAttributes',))
                 82 IMPORT_NAME             14 (agiflow.opentelemetry.convention)
                 84 IMPORT_FROM             15 (SpanAttributes)
                 86 STORE_NAME              15 (SpanAttributes)
                 88 POP_TOP
    
      7          90 LOAD_CONST               0 (0)
-                92 LOAD_CONST               7 (('AgiflowServiceTypes',))
-                94 IMPORT_NAME             16 (agiflow.opentelemetry.convention.constants)
-                96 IMPORT_FROM             17 (AgiflowServiceTypes)
-                98 STORE_NAME              17 (AgiflowServiceTypes)
+                92 LOAD_CONST               7 (('AgiflowSpanAttributes',))
+                94 IMPORT_NAME             16 (agiflow.opentelemetry.convention.agiflow_attributes)
+                96 IMPORT_FROM             17 (AgiflowSpanAttributes)
+                98 STORE_NAME              17 (AgiflowSpanAttributes)
                100 POP_TOP
    
      8         102 LOAD_CONST               0 (0)
-               104 LOAD_CONST               8 (('Span', 'SpanKind', 'Status', 'StatusCode'))
-               106 IMPORT_NAME             18 (opentelemetry.trace)
-               108 IMPORT_FROM             19 (Span)
-               110 STORE_NAME              19 (Span)
-               112 IMPORT_FROM             20 (SpanKind)
-               114 STORE_NAME              20 (SpanKind)
-               116 IMPORT_FROM             21 (Status)
-               118 STORE_NAME              21 (Status)
-               120 IMPORT_FROM             22 (StatusCode)
-               122 STORE_NAME              22 (StatusCode)
-               124 POP_TOP
-   
-     9         126 LOAD_CONST               0 (0)
-               128 LOAD_CONST               9 (('AGIFLOW_ADDITIONAL_SPAN_ATTRIBUTES_KEY',))
-               130 IMPORT_NAME             23 (agiflow.opentelemetry.instrumentation.constants.common)
-               132 IMPORT_FROM             24 (AGIFLOW_ADDITIONAL_SPAN_ATTRIBUTES_KEY)
-               134 STORE_NAME              24 (AGIFLOW_ADDITIONAL_SPAN_ATTRIBUTES_KEY)
+               104 LOAD_CONST               8 (('AgiflowServiceTypes',))
+               106 IMPORT_NAME             18 (agiflow.opentelemetry.convention.constants)
+               108 IMPORT_FROM             19 (AgiflowServiceTypes)
+               110 STORE_NAME              19 (AgiflowServiceTypes)
+               112 POP_TOP
+   
+     9         114 LOAD_CONST               0 (0)
+               116 LOAD_CONST               9 (('Span', 'SpanKind', 'Status', 'StatusCode'))
+               118 IMPORT_NAME             20 (opentelemetry.trace)
+               120 IMPORT_FROM             21 (Span)
+               122 STORE_NAME              21 (Span)
+               124 IMPORT_FROM             22 (SpanKind)
+               126 STORE_NAME              22 (SpanKind)
+               128 IMPORT_FROM             23 (Status)
+               130 STORE_NAME              23 (Status)
+               132 IMPORT_FROM             24 (StatusCode)
+               134 STORE_NAME              24 (StatusCode)
                136 POP_TOP
    
-    12         138 LOAD_CONST               0 (0)
-               140 LOAD_CONST              10 (('baggage',))
-               142 IMPORT_NAME             25 (opentelemetry)
-               144 IMPORT_FROM             26 (baggage)
-               146 STORE_NAME              26 (baggage)
+    10         138 LOAD_CONST               0 (0)
+               140 LOAD_CONST              10 (('AGIFLOW_ADDITIONAL_SPAN_ATTRIBUTES_KEY',))
+               142 IMPORT_NAME             25 (agiflow.opentelemetry.instrumentation.constants.common)
+               144 IMPORT_FROM             26 (AGIFLOW_ADDITIONAL_SPAN_ATTRIBUTES_KEY)
+               146 STORE_NAME              26 (AGIFLOW_ADDITIONAL_SPAN_ATTRIBUTES_KEY)
                148 POP_TOP
    
     13         150 LOAD_CONST               0 (0)
-               152 LOAD_CONST              11 (('__version__',))
-               154 IMPORT_NAME             27 (agiflow.version)
-               156 IMPORT_FROM             28 (__version__)
-               158 STORE_NAME              28 (__version__)
+               152 LOAD_CONST              11 (('baggage',))
+               154 IMPORT_NAME             27 (opentelemetry)
+               156 IMPORT_FROM             28 (baggage)
+               158 STORE_NAME              28 (baggage)
                160 POP_TOP
    
     14         162 LOAD_CONST               0 (0)
-               164 LOAD_CONST              12 (('SharedKwargsWithHooks', 'add_extra_spans'))
-               166 IMPORT_NAME             29 (agiflow.opentelemetry.trace_decorators.helper)
-               168 IMPORT_FROM             30 (SharedKwargsWithHooks)
-               170 STORE_NAME              30 (SharedKwargsWithHooks)
-               172 IMPORT_FROM             31 (add_extra_spans)
-               174 STORE_NAME              31 (add_extra_spans)
-               176 POP_TOP
-   
-    18         178 LOAD_CONST               0 (0)
-               180 LOAD_CONST              13 (('get_tracer', 'TracerWrapper'))
-               182 IMPORT_NAME             32 (agiflow.opentelemetry.tracing)
-               184 IMPORT_FROM             33 (get_tracer)
-               186 STORE_NAME              33 (get_tracer)
-               188 IMPORT_FROM             34 (TracerWrapper)
-               190 STORE_NAME              34 (TracerWrapper)
-               192 POP_TOP
-   
-    19         194 LOAD_CONST               0 (0)
-               196 LOAD_CONST              14 (('should_send_prompts',))
-               198 IMPORT_NAME             35 (agiflow.opentelemetry.utils)
-               200 IMPORT_FROM             36 (should_send_prompts)
-               202 STORE_NAME              36 (should_send_prompts)
-               204 POP_TOP
-   
-    22         206 LOAD_CONST               0 (0)
-               208 LOAD_CONST              15 (('get_trace_context_from_carrier', 'set_association_properties', 'set_prompt_settings_context', 'set_prompt_attributes_from_context', 'set_workflow_name', 'set_override_enable_context_tracing', 'ContextKeys'))
-               210 IMPORT_NAME             37 (agiflow.opentelemetry.context)
-               212 IMPORT_FROM             38 (get_trace_context_from_carrier)
-               214 STORE_NAME              38 (get_trace_context_from_carrier)
-               216 IMPORT_FROM             39 (set_association_properties)
-               218 STORE_NAME              39 (set_association_properties)
-               220 IMPORT_FROM             40 (set_prompt_settings_context)
-               222 STORE_NAME              40 (set_prompt_settings_context)
-               224 IMPORT_FROM             41 (set_prompt_attributes_from_context)
-               226 STORE_NAME              41 (set_prompt_attributes_from_context)
-               228 IMPORT_FROM             42 (set_workflow_name)
-               230 STORE_NAME              42 (set_workflow_name)
-               232 IMPORT_FROM             43 (set_override_enable_context_tracing)
-               234 STORE_NAME              43 (set_override_enable_context_tracing)
-               236 IMPORT_FROM             44 (ContextKeys)
-               238 STORE_NAME              44 (ContextKeys)
-               240 POP_TOP
-   
-    31         242 LOAD_CONST               0 (0)
-               244 LOAD_CONST              16 (('serialise_to_json', 'camel_to_snake'))
-               246 IMPORT_NAME             45 (agiflow.utils)
-               248 IMPORT_FROM             46 (serialise_to_json)
-               250 STORE_NAME              46 (serialise_to_json)
-               252 IMPORT_FROM             47 (camel_to_snake)
-               254 STORE_NAME              47 (camel_to_snake)
-               256 POP_TOP
-   
-    36         258 PUSH_NULL
-               260 LOAD_NAME                9 (TypeVar)
-               262 LOAD_CONST              17 ('R')
-               264 PRECALL                  1
-               268 CALL                     1
-               278 STORE_NAME              48 (R)
-   
-    37         280 PUSH_NULL
-               282 LOAD_NAME                4 (logging)
-               284 LOAD_ATTR               49 (getLogger)
-               294 LOAD_NAME               50 (__name__)
-               296 PRECALL                  1
-               300 CALL                     1
-               310 STORE_NAME              51 (logger)
-   
-    40         312 PUSH_NULL
-               314 LOAD_BUILD_CLASS
-               316 LOAD_CONST              18 (<code object AbstractSpanCapture, file "/Users/vuongngo/workspace/agiflow/packages/python/agiflow-sdk/agiflow/opentelemetry/trace_decorators/wrapper.py", line 40>)
-               318 MAKE_FUNCTION            0
-               320 LOAD_CONST              19 ('AbstractSpanCapture')
-               322 LOAD_NAME                1 (ABC)
-               324 LOAD_NAME               10 (Generic)
-               326 LOAD_NAME               48 (R)
-               328 BINARY_SUBSCR
-               338 PRECALL                  4
-               342 CALL                     4
-               352 STORE_NAME              52 (AbstractSpanCapture)
-   
-    80         354 PUSH_NULL
-               356 LOAD_BUILD_CLASS
-               358 LOAD_CONST              20 (<code object BaseSpanCapture, file "/Users/vuongngo/workspace/agiflow/packages/python/agiflow-sdk/agiflow/opentelemetry/trace_decorators/wrapper.py", line 80>)
-               360 MAKE_FUNCTION            0
-               362 LOAD_CONST              21 ('BaseSpanCapture')
-               364 LOAD_NAME               52 (AbstractSpanCapture)
-               366 PRECALL                  3
-               370 CALL                     3
-               380 STORE_NAME              53 (BaseSpanCapture)
-   
-   231         382 LOAD_CONST               3 (None)
-   
-   232         384 LOAD_NAME               17 (AgiflowServiceTypes)
-               386 LOAD_ATTR               54 (TASK)
-   
-   233         396 LOAD_NAME               20 (SpanKind)
-               398 LOAD_ATTR               55 (INTERNAL)
-   
-   234         408 LOAD_NAME               53 (BaseSpanCapture)
-   
-   230         410 BUILD_TUPLE              4
-               412 LOAD_CONST              22 ('name')
-   
-   231         414 LOAD_NAME                8 (Optional)
-               416 LOAD_NAME               56 (str)
-               418 BINARY_SUBSCR
-   
-   230         428 LOAD_CONST              23 ('tlp_service_type')
-   
-   232         430 LOAD_NAME                8 (Optional)
-               432 LOAD_NAME               17 (AgiflowServiceTypes)
-               434 BINARY_SUBSCR
-   
-   230         444 LOAD_CONST              24 ('config')
-   
-   235         446 LOAD_NAME               11 (Unpack)
-               448 LOAD_NAME               30 (SharedKwargsWithHooks)
-               450 BINARY_SUBSCR
-   
-   230         460 BUILD_TUPLE              6
-               462 LOAD_CONST              25 (<code object decorate_method, file "/Users/vuongngo/workspace/agiflow/packages/python/agiflow-sdk/agiflow/opentelemetry/trace_decorators/wrapper.py", line 230>)
-               464 MAKE_FUNCTION            5 (defaults, annotations)
-               466 STORE_NAME              57 (decorate_method)
-   
-   298         468 LOAD_CONST               3 (None)
-   
-   299         470 LOAD_NAME               17 (AgiflowServiceTypes)
-               472 LOAD_ATTR               54 (TASK)
-   
-   300         482 LOAD_NAME               20 (SpanKind)
-               484 LOAD_ATTR               55 (INTERNAL)
-   
-   301         494 LOAD_NAME               53 (BaseSpanCapture)
-   
-   297         496 BUILD_TUPLE              4
-               498 LOAD_CONST              22 ('name')
-   
-   298         500 LOAD_NAME                8 (Optional)
-               502 LOAD_NAME               56 (str)
-               504 BINARY_SUBSCR
-   
-   297         514 LOAD_CONST              23 ('tlp_service_type')
-   
-   299         516 LOAD_NAME                8 (Optional)
-               518 LOAD_NAME               17 (AgiflowServiceTypes)
-               520 BINARY_SUBSCR
-   
-   297         530 LOAD_CONST              24 ('config')
-   
-   302         532 LOAD_NAME               11 (Unpack)
-               534 LOAD_NAME               30 (SharedKwargsWithHooks)
-               536 BINARY_SUBSCR
-   
-   297         546 BUILD_TUPLE              6
-               548 LOAD_CONST              26 (<code object adecorate_method, file "/Users/vuongngo/workspace/agiflow/packages/python/agiflow-sdk/agiflow/opentelemetry/trace_decorators/wrapper.py", line 297>)
-               550 MAKE_FUNCTION            5 (defaults, annotations)
-               552 STORE_NAME              58 (adecorate_method)
-   
-   368         554 LOAD_NAME               17 (AgiflowServiceTypes)
-               556 LOAD_ATTR               54 (TASK)
-   
-   369         566 LOAD_NAME               20 (SpanKind)
-               568 LOAD_ATTR               55 (INTERNAL)
-   
-   370         578 LOAD_NAME               53 (BaseSpanCapture)
-   
-   365         580 BUILD_TUPLE              3
-               582 LOAD_CONST              22 ('name')
-   
-   366         584 LOAD_NAME                8 (Optional)
-               586 LOAD_NAME               56 (str)
-               588 BINARY_SUBSCR
-   
-   365         598 LOAD_CONST              27 ('method_name')
-   
-   367         600 LOAD_NAME               56 (str)
-   
-   365         602 LOAD_CONST              23 ('tlp_service_type')
-   
-   368         604 LOAD_NAME                8 (Optional)
-               606 LOAD_NAME               17 (AgiflowServiceTypes)
-               608 BINARY_SUBSCR
-   
-   365         618 LOAD_CONST              28 ('kwargs')
-   
-   371         620 LOAD_NAME               11 (Unpack)
-               622 LOAD_NAME               30 (SharedKwargsWithHooks)
-               624 BINARY_SUBSCR
-   
-   365         634 BUILD_TUPLE              8
-               636 LOAD_CONST              29 (<code object decorate_class_method, file "/Users/vuongngo/workspace/agiflow/packages/python/agiflow-sdk/agiflow/opentelemetry/trace_decorators/wrapper.py", line 365>)
-               638 MAKE_FUNCTION            5 (defaults, annotations)
-               640 STORE_NAME              59 (decorate_class_method)
-   
-   395         642 LOAD_NAME               17 (AgiflowServiceTypes)
-               644 LOAD_ATTR               54 (TASK)
-   
-   396         654 LOAD_NAME               20 (SpanKind)
-               656 LOAD_ATTR               55 (INTERNAL)
-   
-   397         666 LOAD_NAME               53 (BaseSpanCapture)
-   
-   392         668 BUILD_TUPLE              3
-               670 LOAD_CONST              22 ('name')
-   
-   393         672 LOAD_NAME                8 (Optional)
-               674 LOAD_NAME               56 (str)
-               676 BINARY_SUBSCR
-   
-   392         686 LOAD_CONST              27 ('method_name')
-   
-   394         688 LOAD_NAME               56 (str)
-   
-   392         690 LOAD_CONST              23 ('tlp_service_type')
-   
-   395         692 LOAD_NAME                8 (Optional)
-               694 LOAD_NAME               17 (AgiflowServiceTypes)
-               696 BINARY_SUBSCR
-   
-   392         706 LOAD_CONST              28 ('kwargs')
-   
-   398         708 LOAD_NAME               11 (Unpack)
-               710 LOAD_NAME               30 (SharedKwargsWithHooks)
-               712 BINARY_SUBSCR
-   
-   392         722 BUILD_TUPLE              8
-               724 LOAD_CONST              30 (<code object adecorate_class_method, file "/Users/vuongngo/workspace/agiflow/packages/python/agiflow-sdk/agiflow/opentelemetry/trace_decorators/wrapper.py", line 392>)
-               726 MAKE_FUNCTION            5 (defaults, annotations)
-               728 STORE_NAME              60 (adecorate_class_method)
-               730 LOAD_CONST               3 (None)
-               732 RETURN_VALUE
+               164 LOAD_CONST              12 (('__version__',))
+               166 IMPORT_NAME             29 (agiflow.version)
+               168 IMPORT_FROM             30 (__version__)
+               170 STORE_NAME              30 (__version__)
+               172 POP_TOP
+   
+    15         174 LOAD_CONST               0 (0)
+               176 LOAD_CONST              13 (('SharedKwargsWithHooks',))
+               178 IMPORT_NAME             31 (agiflow.opentelemetry.trace_decorators.helper)
+               180 IMPORT_FROM             32 (SharedKwargsWithHooks)
+               182 STORE_NAME              32 (SharedKwargsWithHooks)
+               184 POP_TOP
+   
+    18         186 LOAD_CONST               0 (0)
+               188 LOAD_CONST              14 (('get_tracer', 'TracerWrapper'))
+               190 IMPORT_NAME             33 (agiflow.opentelemetry.tracing)
+               192 IMPORT_FROM             34 (get_tracer)
+               194 STORE_NAME              34 (get_tracer)
+               196 IMPORT_FROM             35 (TracerWrapper)
+               198 STORE_NAME              35 (TracerWrapper)
+               200 POP_TOP
+   
+    19         202 LOAD_CONST               0 (0)
+               204 LOAD_CONST              15 (('should_send_prompts',))
+               206 IMPORT_NAME             36 (agiflow.opentelemetry.utils)
+               208 IMPORT_FROM             37 (should_send_prompts)
+               210 STORE_NAME              37 (should_send_prompts)
+               212 POP_TOP
+   
+    22         214 LOAD_CONST               0 (0)
+               216 LOAD_CONST              16 (('get_trace_context_from_carrier', 'set_association_properties', 'set_prompt_settings_context', 'set_prompt_attributes_from_context', 'set_workflow_name', 'set_override_enable_context_tracing', 'ContextKeys'))
+               218 IMPORT_NAME             38 (agiflow.opentelemetry.context)
+               220 IMPORT_FROM             39 (get_trace_context_from_carrier)
+               222 STORE_NAME              39 (get_trace_context_from_carrier)
+               224 IMPORT_FROM             40 (set_association_properties)
+               226 STORE_NAME              40 (set_association_properties)
+               228 IMPORT_FROM             41 (set_prompt_settings_context)
+               230 STORE_NAME              41 (set_prompt_settings_context)
+               232 IMPORT_FROM             42 (set_prompt_attributes_from_context)
+               234 STORE_NAME              42 (set_prompt_attributes_from_context)
+               236 IMPORT_FROM             43 (set_workflow_name)
+               238 STORE_NAME              43 (set_workflow_name)
+               240 IMPORT_FROM             44 (set_override_enable_context_tracing)
+               242 STORE_NAME              44 (set_override_enable_context_tracing)
+               244 IMPORT_FROM             45 (ContextKeys)
+               246 STORE_NAME              45 (ContextKeys)
+               248 POP_TOP
+   
+    31         250 LOAD_CONST               0 (0)
+               252 LOAD_CONST              17 (('serialise_to_json', 'camel_to_snake'))
+               254 IMPORT_NAME             46 (agiflow.utils)
+               256 IMPORT_FROM             47 (serialise_to_json)
+               258 STORE_NAME              47 (serialise_to_json)
+               260 IMPORT_FROM             48 (camel_to_snake)
+               262 STORE_NAME              48 (camel_to_snake)
+               264 POP_TOP
+   
+    36         266 PUSH_NULL
+               268 LOAD_NAME                9 (TypeVar)
+               270 LOAD_CONST              18 ('R')
+               272 PRECALL                  1
+               276 CALL                     1
+               286 STORE_NAME              49 (R)
+   
+    37         288 PUSH_NULL
+               290 LOAD_NAME                4 (logging)
+               292 LOAD_ATTR               50 (getLogger)
+               302 LOAD_NAME               51 (__name__)
+               304 PRECALL                  1
+               308 CALL                     1
+               318 STORE_NAME              52 (logger)
+   
+    40         320 PUSH_NULL
+               322 LOAD_BUILD_CLASS
+               324 LOAD_CONST              19 (<code object AbstractSpanCapture, file "/Users/vuongngo/workspace/agiflow/packages/python/agiflow-sdk/agiflow/opentelemetry/trace_decorators/wrapper.py", line 40>)
+               326 MAKE_FUNCTION            0
+               328 LOAD_CONST              20 ('AbstractSpanCapture')
+               330 LOAD_NAME                1 (ABC)
+               332 LOAD_NAME               10 (Generic)
+               334 LOAD_NAME               49 (R)
+               336 BINARY_SUBSCR
+               346 PRECALL                  4
+               350 CALL                     4
+               360 STORE_NAME              53 (AbstractSpanCapture)
+   
+    80         362 PUSH_NULL
+               364 LOAD_BUILD_CLASS
+               366 LOAD_CONST              21 (<code object BaseSpanCapture, file "/Users/vuongngo/workspace/agiflow/packages/python/agiflow-sdk/agiflow/opentelemetry/trace_decorators/wrapper.py", line 80>)
+               368 MAKE_FUNCTION            0
+               370 LOAD_CONST              22 ('BaseSpanCapture')
+               372 LOAD_NAME               53 (AbstractSpanCapture)
+               374 PRECALL                  3
+               378 CALL                     3
+               388 STORE_NAME              54 (BaseSpanCapture)
+   
+   252         390 LOAD_CONST               3 (None)
+   
+   253         392 LOAD_NAME               19 (AgiflowServiceTypes)
+               394 LOAD_ATTR               55 (TASK)
+   
+   254         404 LOAD_NAME               22 (SpanKind)
+               406 LOAD_ATTR               56 (INTERNAL)
+   
+   255         416 LOAD_NAME               54 (BaseSpanCapture)
+   
+   251         418 BUILD_TUPLE              4
+               420 LOAD_CONST              23 ('name')
+   
+   252         422 LOAD_NAME                8 (Optional)
+               424 LOAD_NAME               57 (str)
+               426 BINARY_SUBSCR
+   
+   251         436 LOAD_CONST              24 ('tlp_service_type')
+   
+   253         438 LOAD_NAME                8 (Optional)
+               440 LOAD_NAME               19 (AgiflowServiceTypes)
+               442 BINARY_SUBSCR
+   
+   251         452 LOAD_CONST              25 ('config')
+   
+   256         454 LOAD_NAME               11 (Unpack)
+               456 LOAD_NAME               32 (SharedKwargsWithHooks)
+               458 BINARY_SUBSCR
+   
+   251         468 BUILD_TUPLE              6
+               470 LOAD_CONST              26 (<code object decorate_method, file "/Users/vuongngo/workspace/agiflow/packages/python/agiflow-sdk/agiflow/opentelemetry/trace_decorators/wrapper.py", line 251>)
+               472 MAKE_FUNCTION            5 (defaults, annotations)
+               474 STORE_NAME              58 (decorate_method)
+   
+   320         476 LOAD_CONST               3 (None)
+   
+   321         478 LOAD_NAME               19 (AgiflowServiceTypes)
+               480 LOAD_ATTR               55 (TASK)
+   
+   322         490 LOAD_NAME               22 (SpanKind)
+               492 LOAD_ATTR               56 (INTERNAL)
+   
+   323         502 LOAD_NAME               54 (BaseSpanCapture)
+   
+   319         504 BUILD_TUPLE              4
+               506 LOAD_CONST              23 ('name')
+   
+   320         508 LOAD_NAME                8 (Optional)
+               510 LOAD_NAME               57 (str)
+               512 BINARY_SUBSCR
+   
+   319         522 LOAD_CONST              24 ('tlp_service_type')
+   
+   321         524 LOAD_NAME                8 (Optional)
+               526 LOAD_NAME               19 (AgiflowServiceTypes)
+               528 BINARY_SUBSCR
+   
+   319         538 LOAD_CONST              25 ('config')
+   
+   324         540 LOAD_NAME               11 (Unpack)
+               542 LOAD_NAME               32 (SharedKwargsWithHooks)
+               544 BINARY_SUBSCR
+   
+   319         554 BUILD_TUPLE              6
+               556 LOAD_CONST              27 (<code object adecorate_method, file "/Users/vuongngo/workspace/agiflow/packages/python/agiflow-sdk/agiflow/opentelemetry/trace_decorators/wrapper.py", line 319>)
+               558 MAKE_FUNCTION            5 (defaults, annotations)
+               560 STORE_NAME              59 (adecorate_method)
+   
+   390         562 LOAD_NAME               19 (AgiflowServiceTypes)
+               564 LOAD_ATTR               55 (TASK)
+   
+   391         574 LOAD_NAME               22 (SpanKind)
+               576 LOAD_ATTR               56 (INTERNAL)
+   
+   392         586 LOAD_NAME               54 (BaseSpanCapture)
+   
+   387         588 BUILD_TUPLE              3
+               590 LOAD_CONST              23 ('name')
+   
+   388         592 LOAD_NAME                8 (Optional)
+               594 LOAD_NAME               57 (str)
+               596 BINARY_SUBSCR
+   
+   387         606 LOAD_CONST              28 ('method_name')
+   
+   389         608 LOAD_NAME               57 (str)
+   
+   387         610 LOAD_CONST              24 ('tlp_service_type')
+   
+   390         612 LOAD_NAME                8 (Optional)
+               614 LOAD_NAME               19 (AgiflowServiceTypes)
+               616 BINARY_SUBSCR
+   
+   387         626 LOAD_CONST              29 ('kwargs')
+   
+   393         628 LOAD_NAME               11 (Unpack)
+               630 LOAD_NAME               32 (SharedKwargsWithHooks)
+               632 BINARY_SUBSCR
+   
+   387         642 BUILD_TUPLE              8
+               644 LOAD_CONST              30 (<code object decorate_class_method, file "/Users/vuongngo/workspace/agiflow/packages/python/agiflow-sdk/agiflow/opentelemetry/trace_decorators/wrapper.py", line 387>)
+               646 MAKE_FUNCTION            5 (defaults, annotations)
+               648 STORE_NAME              60 (decorate_class_method)
+   
+   417         650 LOAD_NAME               19 (AgiflowServiceTypes)
+               652 LOAD_ATTR               55 (TASK)
+   
+   418         662 LOAD_NAME               22 (SpanKind)
+               664 LOAD_ATTR               56 (INTERNAL)
+   
+   419         674 LOAD_NAME               54 (BaseSpanCapture)
+   
+   414         676 BUILD_TUPLE              3
+               678 LOAD_CONST              23 ('name')
+   
+   415         680 LOAD_NAME                8 (Optional)
+               682 LOAD_NAME               57 (str)
+               684 BINARY_SUBSCR
+   
+   414         694 LOAD_CONST              28 ('method_name')
+   
+   416         696 LOAD_NAME               57 (str)
+   
+   414         698 LOAD_CONST              24 ('tlp_service_type')
+   
+   417         700 LOAD_NAME                8 (Optional)
+               702 LOAD_NAME               19 (AgiflowServiceTypes)
+               704 BINARY_SUBSCR
+   
+   414         714 LOAD_CONST              29 ('kwargs')
+   
+   420         716 LOAD_NAME               11 (Unpack)
+               718 LOAD_NAME               32 (SharedKwargsWithHooks)
+               720 BINARY_SUBSCR
+   
+   414         730 BUILD_TUPLE              8
+               732 LOAD_CONST              31 (<code object adecorate_class_method, file "/Users/vuongngo/workspace/agiflow/packages/python/agiflow-sdk/agiflow/opentelemetry/trace_decorators/wrapper.py", line 414>)
+               734 MAKE_FUNCTION            5 (defaults, annotations)
+               736 STORE_NAME              61 (adecorate_class_method)
+               738 LOAD_CONST               3 (None)
+               740 RETURN_VALUE
    consts
       0
       ('ABC',)
       ('wraps',)
       None
       ('Any', 'Dict', 'Optional', 'TypeVar', 'Generic', 'Unpack')
       ('set_workflow_name_from_context',)
       ('SpanAttributes',)
+      ('AgiflowSpanAttributes',)
       ('AgiflowServiceTypes',)
       ('Span', 'SpanKind', 'Status', 'StatusCode')
       ('AGIFLOW_ADDITIONAL_SPAN_ATTRIBUTES_KEY',)
       ('baggage',)
       ('__version__',)
-      ('SharedKwargsWithHooks', 'add_extra_spans')
+      ('SharedKwargsWithHooks',)
       ('get_tracer', 'TracerWrapper')
       ('should_send_prompts',)
       ('get_trace_context_from_carrier', 'set_association_properties', 'set_prompt_settings_context', 'set_prompt_attributes_from_context', 'set_workflow_name', 'set_override_enable_context_tracing', 'ContextKeys')
       ('serialise_to_json', 'camel_to_snake')
       'R'
       code
          argcount  : 0
@@ -565,19 +571,19 @@
             0x970065005a0164005a02550064015a036504650564023c000000650665
             0719000000000000000000650564033c0000006508650564043c00000065
             08650564053c0000006509650564063c0000006508650564073c00000065
             08650564083c000000650a650b6508660219000000000000000000650564
             093c0000006506650b190000000000000000006505640a3c000000640b65
             076a0c0000000000000000640b640b640c9c04640a6506650b1900000000
             000000000064036506650719000000000000000000640665096606640d84
-            065a0d650e640b65076a0c0000000000000000640b6603640a6506650b19
-            000000000000000000640e65066507190000000000000000006407650866
-            06640f8405a6000000ab0000000000000000005a0f650e64108400a60000
-            00ab0000000000000000005a10641184005a11641284005a12641384005a
-            13640b5300
+            065a0d650e640e8400a6000000ab0000000000000000005a0f650e640b65
+            076a0c0000000000000000640b6603640a6506650b190000000000000000
+            00640f650665071900000000000000000064076508660664108405a60000
+            00ab0000000000000000005a10650e64118400a6000000ab000000000000
+            0000005a11641284005a12641384005a13641484005a14640b5300
           80           0 RESUME                   0
                        2 LOAD_NAME                0 (__name__)
                        4 STORE_NAME               1 (__module__)
                        6 LOAD_CONST               0 ('BaseSpanCapture')
                        8 STORE_NAME               2 (__qualname__)
                       10 SETUP_ANNOTATIONS
          
@@ -667,70 +673,80 @@
           95         204 BUILD_TUPLE              6
                      206 LOAD_CONST              13 (<code object __init__, file "/Users/vuongngo/workspace/agiflow/packages/python/agiflow-sdk/agiflow/opentelemetry/trace_decorators/wrapper.py", line 95>)
                      208 MAKE_FUNCTION            6 (kwdefaults, annotations)
                      210 STORE_NAME              13 (__init__)
          
          120         212 LOAD_NAME               14 (staticmethod)
          
-         122         214 LOAD_CONST              11 (None)
+         121         214 LOAD_CONST              14 (<code object is_flush_on_exit, file "/Users/vuongngo/workspace/agiflow/packages/python/agiflow-sdk/agiflow/opentelemetry/trace_decorators/wrapper.py", line 120>)
+                     216 MAKE_FUNCTION            0
          
-         123         216 LOAD_NAME                7 (AgiflowServiceTypes)
-                     218 LOAD_ATTR               12 (TASK)
+         120         218 PRECALL                  0
+                     222 CALL                     0
          
-         124         228 LOAD_CONST              11 (None)
+         121         232 STORE_NAME              15 (is_flush_on_exit)
          
-         121         230 BUILD_TUPLE              3
-                     232 LOAD_CONST              10 ('name')
+         124         234 LOAD_NAME               14 (staticmethod)
          
-         122         234 LOAD_NAME                6 (Optional)
-                     236 LOAD_NAME               11 (str)
-                     238 BINARY_SUBSCR
+         126         236 LOAD_CONST              11 (None)
          
-         121         248 LOAD_CONST              14 ('tlp_service_type')
+         127         238 LOAD_NAME                7 (AgiflowServiceTypes)
+                     240 LOAD_ATTR               12 (TASK)
          
-         123         250 LOAD_NAME                6 (Optional)
-                     252 LOAD_NAME                7 (AgiflowServiceTypes)
-                     254 BINARY_SUBSCR
+         128         250 LOAD_CONST              11 (None)
          
-         121         264 LOAD_CONST               7 ('instance')
+         125         252 BUILD_TUPLE              3
+                     254 LOAD_CONST              10 ('name')
          
-         124         266 LOAD_NAME                8 (Any)
+         126         256 LOAD_NAME                6 (Optional)
+                     258 LOAD_NAME               11 (str)
+                     260 BINARY_SUBSCR
          
-         121         268 BUILD_TUPLE              6
-                     270 LOAD_CONST              15 (<code object get_span_name, file "/Users/vuongngo/workspace/agiflow/packages/python/agiflow-sdk/agiflow/opentelemetry/trace_decorators/wrapper.py", line 120>)
-                     272 MAKE_FUNCTION            5 (defaults, annotations)
+         125         270 LOAD_CONST              15 ('tlp_service_type')
          
-         120         274 PRECALL                  0
-                     278 CALL                     0
+         127         272 LOAD_NAME                6 (Optional)
+                     274 LOAD_NAME                7 (AgiflowServiceTypes)
+                     276 BINARY_SUBSCR
          
-         121         288 STORE_NAME              15 (get_span_name)
+         125         286 LOAD_CONST               7 ('instance')
          
-         135         290 LOAD_NAME               14 (staticmethod)
+         128         288 LOAD_NAME                8 (Any)
          
-         136         292 LOAD_CONST              16 (<code object get_service_type, file "/Users/vuongngo/workspace/agiflow/packages/python/agiflow-sdk/agiflow/opentelemetry/trace_decorators/wrapper.py", line 135>)
-                     294 MAKE_FUNCTION            0
+         125         290 BUILD_TUPLE              6
+                     292 LOAD_CONST              16 (<code object get_span_name, file "/Users/vuongngo/workspace/agiflow/packages/python/agiflow-sdk/agiflow/opentelemetry/trace_decorators/wrapper.py", line 124>)
+                     294 MAKE_FUNCTION            5 (defaults, annotations)
          
-         135         296 PRECALL                  0
+         124         296 PRECALL                  0
                      300 CALL                     0
          
-         136         310 STORE_NAME              16 (get_service_type)
+         125         310 STORE_NAME              16 (get_span_name)
          
-         142         312 LOAD_CONST              17 (<code object set_span_attribute, file "/Users/vuongngo/workspace/agiflow/packages/python/agiflow-sdk/agiflow/opentelemetry/trace_decorators/wrapper.py", line 142>)
-                     314 MAKE_FUNCTION            0
-                     316 STORE_NAME              17 (set_span_attribute)
-         
-         153         318 LOAD_CONST              18 (<code object capture_input, file "/Users/vuongngo/workspace/agiflow/packages/python/agiflow-sdk/agiflow/opentelemetry/trace_decorators/wrapper.py", line 153>)
-                     320 MAKE_FUNCTION            0
-                     322 STORE_NAME              18 (capture_input)
-         
-         207         324 LOAD_CONST              19 (<code object capture_output, file "/Users/vuongngo/workspace/agiflow/packages/python/agiflow-sdk/agiflow/opentelemetry/trace_decorators/wrapper.py", line 207>)
-                     326 MAKE_FUNCTION            0
-                     328 STORE_NAME              19 (capture_output)
-                     330 LOAD_CONST              11 (None)
-                     332 RETURN_VALUE
+         139         312 LOAD_NAME               14 (staticmethod)
+         
+         140         314 LOAD_CONST              17 (<code object get_service_type, file "/Users/vuongngo/workspace/agiflow/packages/python/agiflow-sdk/agiflow/opentelemetry/trace_decorators/wrapper.py", line 139>)
+                     316 MAKE_FUNCTION            0
+         
+         139         318 PRECALL                  0
+                     322 CALL                     0
+         
+         140         332 STORE_NAME              17 (get_service_type)
+         
+         146         334 LOAD_CONST              18 (<code object set_span_attribute, file "/Users/vuongngo/workspace/agiflow/packages/python/agiflow-sdk/agiflow/opentelemetry/trace_decorators/wrapper.py", line 146>)
+                     336 MAKE_FUNCTION            0
+                     338 STORE_NAME              18 (set_span_attribute)
+         
+         157         340 LOAD_CONST              19 (<code object capture_input, file "/Users/vuongngo/workspace/agiflow/packages/python/agiflow-sdk/agiflow/opentelemetry/trace_decorators/wrapper.py", line 157>)
+                     342 MAKE_FUNCTION            0
+                     344 STORE_NAME              19 (capture_input)
+         
+         228         346 LOAD_CONST              20 (<code object capture_output, file "/Users/vuongngo/workspace/agiflow/packages/python/agiflow-sdk/agiflow/opentelemetry/trace_decorators/wrapper.py", line 228>)
+                     348 MAKE_FUNCTION            0
+                     350 STORE_NAME              20 (capture_output)
+                     352 LOAD_CONST              11 (None)
+                     354 RETURN_VALUE
          consts
             'BaseSpanCapture'
             '\n    Store shared props.\n    Required to implement hooks to add to trace to span\n    '
             'span'
             'service_type'
             'args'
             'kwargs'
@@ -845,516 +861,611 @@
                varnames   ('self', 'name', 'service_type', 'span', 'instance', 'context', 'config', 'args', 'kwargs', 'extra_attributes')
                freevars   ()
                cellvars   ()
                filename   '/Users/vuongngo/workspace/agiflow/packages/python/agiflow-sdk/agiflow/opentelemetry/trace_decorators/wrapper.py'
                name       '__init__'
                firstlineno 95
                lnotab 0x020b0e010e010e010e010e010e010e010e0140014a0140013201
+            code
+               argcount  : 0
+               nlocals   : 0
+               stacksize : 1
+               flags     : 3
+               code 0x970064015300
+               120           0 RESUME                   0
+               
+               122           2 LOAD_CONST               1 (False)
+                             4 RETURN_VALUE
+               consts
+                  None
+                  False
+               names      ()
+               varnames   ()
+               freevars   ()
+               cellvars   ()
+               filename   '/Users/vuongngo/workspace/agiflow/packages/python/agiflow-sdk/agiflow/opentelemetry/trace_decorators/wrapper.py'
+               name       'is_flush_on_exit'
+               firstlineno 120
+               lnotab 0x0202
             'tlp_service_type'
             code
                argcount  : 3
                nlocals   : 5
                stacksize : 3
                flags     : 3
                code
                   0x97007c017018740000000000000000000000a001000000000000000000
                   0000000000000000000000a6000000ab0000000000000000007d037c0072
                   077c009b0064017c039b009d036e0b7c026a0200000000000000009b0064
                   017c039b009d037d047c047c0366025300
-               120           0 RESUME                   0
+               124           0 RESUME                   0
                
-               126           2 LOAD_FAST                1 (tlp_service_type)
+               130           2 LOAD_FAST                1 (tlp_service_type)
                              4 JUMP_IF_TRUE_OR_POP     24 (to 54)
                              6 LOAD_GLOBAL              0 (BaseSpanCapture)
                             18 LOAD_METHOD              1 (get_service_type)
                             40 PRECALL                  0
                             44 CALL                     0
                        >>   54 STORE_FAST               3 (service_type)
                
-               130          56 LOAD_FAST                0 (name)
+               134          56 LOAD_FAST                0 (name)
                
-               129          58 POP_JUMP_FORWARD_IF_FALSE     7 (to 74)
+               133          58 POP_JUMP_FORWARD_IF_FALSE     7 (to 74)
                             60 LOAD_FAST                0 (name)
                             62 FORMAT_VALUE             0
                             64 LOAD_CONST               1 ('.')
                             66 LOAD_FAST                3 (service_type)
                             68 FORMAT_VALUE             0
                             70 BUILD_STRING             3
                             72 JUMP_FORWARD            11 (to 96)
                
-               131     >>   74 LOAD_FAST                2 (instance)
+               135     >>   74 LOAD_FAST                2 (instance)
                             76 LOAD_ATTR                2 (__name__)
                             86 FORMAT_VALUE             0
                             88 LOAD_CONST               1 ('.')
                             90 LOAD_FAST                3 (service_type)
                             92 FORMAT_VALUE             0
                             94 BUILD_STRING             3
                
-               128     >>   96 STORE_FAST               4 (span_name)
+               132     >>   96 STORE_FAST               4 (span_name)
                
-               133          98 LOAD_FAST                4 (span_name)
+               137          98 LOAD_FAST                4 (span_name)
                            100 LOAD_FAST                3 (service_type)
                            102 BUILD_TUPLE              2
                            104 RETURN_VALUE
                consts
                   None
                   '.'
                names      ('BaseSpanCapture', 'get_service_type', '__name__')
                varnames   ('name', 'tlp_service_type', 'instance', 'service_type', 'span_name')
                freevars   ()
                cellvars   ()
                filename   '/Users/vuongngo/workspace/agiflow/packages/python/agiflow-sdk/agiflow/opentelemetry/trace_decorators/wrapper.py'
                name       'get_span_name'
-               firstlineno 120
+               firstlineno 124
                lnotab 0x0206360402ff100216fd0205
             code
                argcount  : 0
                nlocals   : 0
                stacksize : 1
                flags     : 3
                code 0x97007400000000000000000000006a0100000000000000005300
-               135           0 RESUME                   0
+               139           0 RESUME                   0
                
-               140           2 LOAD_GLOBAL              0 (AgiflowServiceTypes)
+               144           2 LOAD_GLOBAL              0 (AgiflowServiceTypes)
                             14 LOAD_ATTR                1 (TASK)
                             24 RETURN_VALUE
                consts
                   '\n        Override this method if span kind is different\n        '
                names      ('AgiflowServiceTypes', 'TASK')
                varnames   ()
                freevars   ()
                cellvars   ()
                filename   '/Users/vuongngo/workspace/agiflow/packages/python/agiflow-sdk/agiflow/opentelemetry/trace_decorators/wrapper.py'
                name       'get_service_type'
-               firstlineno 135
+               firstlineno 139
                lnotab 0x0205
             code
                argcount  : 3
                nlocals   : 3
                stacksize : 4
                flags     : 3
                code
-                  0x97007c006a000000000000000000a00100000000000000000000000000
-                  00000000000000a6000000ab000000000000000000724f74050000000000
-                  00000000007c016401a6020000ab02000000000000000072227c006a0000
-                  00000000000000a00300000000000000000000000000000000000000007c
-                  016a0400000000000000007c02a6020000ab020000000000000000010064
-                  0253007c006a000000000000000000a00300000000000000000000000000
-                  000000000000007c017c02a6020000ab0200000000000000000100640253
-                  0064025300
-               142           0 RESUME                   0
-               
-               147           2 LOAD_FAST                0 (self)
-                             4 LOAD_ATTR                0 (span)
-                            14 LOAD_METHOD              1 (is_recording)
-                            36 PRECALL                  0
-                            40 CALL                     0
-                            50 POP_JUMP_FORWARD_IF_FALSE    79 (to 210)
-               
-               148          52 LOAD_GLOBAL              5 (NULL + hasattr)
-                            64 LOAD_FAST                1 (field)
-                            66 LOAD_CONST               1 ('value')
-                            68 PRECALL                  2
-                            72 CALL                     2
-                            82 POP_JUMP_FORWARD_IF_FALSE    34 (to 152)
-               
-               149          84 LOAD_FAST                0 (self)
-                            86 LOAD_ATTR                0 (span)
-                            96 LOAD_METHOD              3 (set_attribute)
-                           118 LOAD_FAST                1 (field)
-                           120 LOAD_ATTR                4 (value)
-                           130 LOAD_FAST                2 (value)
-                           132 PRECALL                  2
-                           136 CALL                     2
-                           146 POP_TOP
-                           148 LOAD_CONST               2 (None)
-                           150 RETURN_VALUE
-               
-               151     >>  152 LOAD_FAST                0 (self)
-                           154 LOAD_ATTR                0 (span)
-                           164 LOAD_METHOD              3 (set_attribute)
-                           186 LOAD_FAST                1 (field)
-                           188 LOAD_FAST                2 (value)
-                           190 PRECALL                  2
-                           194 CALL                     2
-                           204 POP_TOP
-                           206 LOAD_CONST               2 (None)
-                           208 RETURN_VALUE
+                  0x97007c0281687c006a000000000000000000a001000000000000000000
+                  0000000000000000000000a6000000ab0000000000000000007251740500
+                  0000000000000000007c016402a6020000ab02000000000000000072227c
+                  006a000000000000000000a0030000000000000000000000000000000000
+                  0000007c016a0400000000000000007c02a6020000ab0200000000000000
+                  000100640153007c006a000000000000000000a003000000000000000000
+                  00000000000000000000007c017c02a6020000ab02000000000000000001
+                  00640153006401530064015300
+               146           0 RESUME                   0
+               
+               151           2 LOAD_FAST                2 (value)
+                             4 POP_JUMP_FORWARD_IF_NONE   104 (to 214)
+                             6 LOAD_FAST                0 (self)
+                             8 LOAD_ATTR                0 (span)
+                            18 LOAD_METHOD              1 (is_recording)
+                            40 PRECALL                  0
+                            44 CALL                     0
+                            54 POP_JUMP_FORWARD_IF_FALSE    81 (to 218)
                
-               147     >>  210 LOAD_CONST               2 (None)
+               152          56 LOAD_GLOBAL              5 (NULL + hasattr)
+                            68 LOAD_FAST                1 (field)
+                            70 LOAD_CONST               2 ('value')
+                            72 PRECALL                  2
+                            76 CALL                     2
+                            86 POP_JUMP_FORWARD_IF_FALSE    34 (to 156)
+               
+               153          88 LOAD_FAST                0 (self)
+                            90 LOAD_ATTR                0 (span)
+                           100 LOAD_METHOD              3 (set_attribute)
+                           122 LOAD_FAST                1 (field)
+                           124 LOAD_ATTR                4 (value)
+                           134 LOAD_FAST                2 (value)
+                           136 PRECALL                  2
+                           140 CALL                     2
+                           150 POP_TOP
+                           152 LOAD_CONST               1 (None)
+                           154 RETURN_VALUE
+               
+               155     >>  156 LOAD_FAST                0 (self)
+                           158 LOAD_ATTR                0 (span)
+                           168 LOAD_METHOD              3 (set_attribute)
+                           190 LOAD_FAST                1 (field)
+                           192 LOAD_FAST                2 (value)
+                           194 PRECALL                  2
+                           198 CALL                     2
+                           208 POP_TOP
+                           210 LOAD_CONST               1 (None)
                            212 RETURN_VALUE
+               
+               151     >>  214 LOAD_CONST               1 (None)
+                           216 RETURN_VALUE
+                       >>  218 LOAD_CONST               1 (None)
+                           220 RETURN_VALUE
                consts
                   '\n        Using this method to set single attribute\n        which field is an enum\n        '
-                  'value'
                   None
+                  'value'
                names      ('span', 'is_recording', 'hasattr', 'set_attribute', 'value')
                varnames   ('self', 'field', 'value')
                freevars   ()
                cellvars   ()
                filename   '/Users/vuongngo/workspace/agiflow/packages/python/agiflow-sdk/agiflow/opentelemetry/trace_decorators/wrapper.py'
                name       'set_span_attribute'
-               firstlineno 142
-               lnotab 0x02053201200144023afc
+               firstlineno 146
+               lnotab 0x02053601200144023afc
             code
                argcount  : 1
-               nlocals   : 10
-               stacksize : 7
+               nlocals   : 12
+               stacksize : 6
                flags     : 3
                code
                   0x97007c006a00000000000000000072257c00a001000000000000000000
                   00000000000000000000007404000000000000000000006a030000000000
                   0000007c006a000000000000000000a6020000ab02000000000000000001
-                  007c006a04000000000000000090018162740b000000000000000000007c
-                  006a0400000000000000006401a6020000ab020000000000000000900172
-                  4c7c006a040000000000000000a006000000000000000000000000000000
-                  0000000000740e000000000000000000006a080000000000000000a60100
-                  00ab0100000000000000007d017c0181537413000000000000000000007c
-                  01a6010000ab01000000000000000001007c01a00a000000000000000000
-                  0000000000000000000000a6000000ab00000000000000000044005d2f5c
-                  0200007d027d037c006a0b0000000000000000a00c000000000000000000
-                  00000000000000000000007404000000000000000000006a0d0000000000
-                  0000009b0064027c029b009d037c03a6020000ab02000000000000000001
-                  008c307c006a040000000000000000a00600000000000000000000000000
-                  00000000000000740e000000000000000000006a0e0000000000000000a6
-                  010000ab0100000000000000007d047c048129741f000000000000000000
-                  007c04a6010000ab01000000000000000001007421000000000000000000
-                  007c006a0b00000000000000007c006a040000000000000000a6020000ab
-                  02000000000000000001007c006a040000000000000000a0060000000000
-                  000000000000000000000000000000740e000000000000000000006a1100
-                  00000000000000a6010000ab0100000000000000007d057c058129742500
-                  0000000000000000007c05a6010000ab0100000000000000000100742700
-                  0000000000000000007c006a0b00000000000000007c006a040000000000
-                  000000a6020000ab02000000000000000001007c006a0400000000000000
-                  00a0060000000000000000000000000000000000000000740e0000000000
-                  00000000006a140000000000000000a6010000ab0100000000000000007d
-                  067c06810f742b000000000000000000007c06a6010000ab010000000000
-                  0000000100742d000000000000000000007c006a0b00000000000000007c
-                  006a170000000000000000a0060000000000000000000000000000000000
-                  0000006403a6010000ab0100000000000000007c006a1700000000000000
-                  00a00600000000000000000000000000000000000000006404a6010000ab
-                  010000000000000000ac05a6030000ab0300000000000000000100090074
-                  3100000000000000000000a6000000ab00000000000000000072a264067d
-                  077c006a170000000000000000a006000000000000000000000000000000
-                  00000000006407a6010000ab0100000000000000007d087c088122743300
-                  0000000000000000007c08a6010000ab010000000000000000721302007c
-                  087c006a1a000000000000000069007c006a1b0000000000000000a4018e
-                  017d076e1c7439000000000000000000007c006a1a00000000000000007c
-                  006a1b000000000000000064089c02a6010000ab0100000000000000007d
-                  07743b000000000000000000007c07743c00000000000000000000a60200
-                  00ab020000000000000000730f7439000000000000000000007c07a60100
-                  00ab0100000000000000007d077c00a00100000000000000000000000000
-                  000000000000007404000000000000000000006a1f00000000000000007c
-                  07a6020000ab020000000000000000010064005300640053002300744000
-                  000000000000000000240072257d09744200000000000000000000a02200
-                  000000000000000000000000000000000000007c09a6010000ab01000000
-                  00000000000100590064007d097e096400530064007d097e097701770078
-                  0359007701
-               153           0 RESUME                   0
+                  0064007d0164007d027c006a04000000000000000081e1740b0000000000
+                  00000000007c006a0400000000000000006401a6020000ab020000000000
+                  00000072cc7c006a040000000000000000a0060000000000000000000000
+                  000000000000000000740e000000000000000000006a0800000000000000
+                  00a6010000ab0100000000000000007d027c006a040000000000000000a0
+                  060000000000000000000000000000000000000000740e00000000000000
+                  0000006a090000000000000000a6010000ab0100000000000000007d017c
+                  006a040000000000000000a0060000000000000000000000000000000000
+                  000000740e000000000000000000006a0a0000000000000000a6010000ab
+                  0100000000000000007d037c0381297417000000000000000000007c03a6
+                  010000ab01000000000000000001007419000000000000000000007c006a
+                  0d00000000000000007c006a040000000000000000a6020000ab02000000
+                  000000000001007c006a040000000000000000a006000000000000000000
+                  0000000000000000000000740e000000000000000000006a0e0000000000
+                  000000a6010000ab0100000000000000007d047c04810f741f0000000000
+                  00000000007c04a6010000ab01000000000000000001007c00a001000000
+                  00000000000000000000000000000000007420000000000000000000006a
+                  1100000000000000007c006a120000000000000000a00600000000000000
+                  000000000000000000000000006402a6010000ab010000000000000000a6
+                  020000ab02000000000000000001007c006a120000000000000000a00600
+                  000000000000000000000000000000000000006403a6010000ab01000000
+                  00000000007d057c0581247427000000000000000000007c05a6010000ab
+                  010000000000000000721302007c057c006a14000000000000000069007c
+                  006a150000000000000000a4018e017d016e027c057d017c006a12000000
+                  0000000000a00600000000000000000000000000000000000000006404a6
+                  010000ab0100000000000000007d067c0681247427000000000000000000
+                  007c06a6010000ab010000000000000000721302007c067c006a14000000
+                  000000000069007c006a150000000000000000a4018e017d026e027c067d
+                  027c018129742d000000000000000000007c01a6010000ab010000000000
+                  0000000100742f000000000000000000007c006a0d00000000000000007c
+                  006a040000000000000000a6020000ab02000000000000000001007c0281
+                  537431000000000000000000007c02a6010000ab01000000000000000001
+                  007c02a0190000000000000000000000000000000000000000a6000000ab
+                  00000000000000000044005d2f5c0200007d077d087c006a0d0000000000
+                  000000a01a00000000000000000000000000000000000000007404000000
+                  000000000000006a1b00000000000000009b0064057c079b009d037c08a6
+                  020000ab02000000000000000001008c3009007439000000000000000000
+                  00a6000000ab00000000000000000072a264067d097c006a120000000000
+                  000000a00600000000000000000000000000000000000000006407a60100
+                  00ab0100000000000000007d0a7c0a81227427000000000000000000007c
+                  0aa6010000ab010000000000000000721302007c0a7c006a140000000000
+                  00000069007c006a150000000000000000a4018e017d096e1c743b000000
+                  000000000000007c006a1400000000000000007c006a1500000000000000
+                  0064089c02a6010000ab0100000000000000007d09743d00000000000000
+                  0000007c09743e00000000000000000000a6020000ab0200000000000000
+                  00730f743b000000000000000000007c09a6010000ab0100000000000000
+                  007d097c00a0010000000000000000000000000000000000000000740400
+                  0000000000000000006a2000000000000000007c09a6020000ab02000000
+                  000000000001006400530064005300230074420000000000000000000024
+                  0072257d0b744400000000000000000000a0230000000000000000000000
+                  0000000000000000007c0ba6010000ab0100000000000000000100590064
+                  007d0b7e0b6400530064007d0b7e0b77017700780359007701
+               157           0 RESUME                   0
                
-               154           2 LOAD_FAST                0 (self)
+               158           2 LOAD_FAST                0 (self)
                              4 LOAD_ATTR                0 (name)
                             14 POP_JUMP_FORWARD_IF_FALSE    37 (to 90)
                
-               155          16 LOAD_FAST                0 (self)
+               159          16 LOAD_FAST                0 (self)
                             18 LOAD_METHOD              1 (set_span_attribute)
                             40 LOAD_GLOBAL              4 (SpanAttributes)
                             52 LOAD_ATTR                3 (AGIFLOW_ENTITY_NAME)
                             62 LOAD_FAST                0 (self)
                             64 LOAD_ATTR                0 (name)
                             74 PRECALL                  2
                             78 CALL                     2
                             88 POP_TOP
                
-               158     >>   90 LOAD_FAST                0 (self)
-                            92 LOAD_ATTR                4 (context)
-                           102 EXTENDED_ARG             1
-                           104 POP_JUMP_FORWARD_IF_NONE   354 (to 814)
-                           106 LOAD_GLOBAL             11 (NULL + hasattr)
-                           118 LOAD_FAST                0 (self)
-                           120 LOAD_ATTR                4 (context)
-                           130 LOAD_CONST               1 ('get')
-                           132 PRECALL                  2
-                           136 CALL                     2
-                           146 EXTENDED_ARG             1
-                           148 POP_JUMP_FORWARD_IF_FALSE   332 (to 814)
-               
-               159         150 LOAD_FAST                0 (self)
-                           152 LOAD_ATTR                4 (context)
-                           162 LOAD_METHOD              6 (get)
-                           184 LOAD_GLOBAL             14 (ContextKeys)
-                           196 LOAD_ATTR                8 (ASSOCIATION_PROPERTIES)
-                           206 PRECALL                  1
-                           210 CALL                     1
-                           220 STORE_FAST               1 (association_properties)
-               
-               160         222 LOAD_FAST                1 (association_properties)
-                           224 POP_JUMP_FORWARD_IF_NONE    83 (to 392)
-               
-               161         226 LOAD_GLOBAL             19 (NULL + set_association_properties)
-                           238 LOAD_FAST                1 (association_properties)
-                           240 PRECALL                  1
-                           244 CALL                     1
-                           254 POP_TOP
-               
-               162         256 LOAD_FAST                1 (association_properties)
-                           258 LOAD_METHOD             10 (items)
-                           280 PRECALL                  0
-                           284 CALL                     0
-                           294 GET_ITER
-                       >>  296 FOR_ITER                47 (to 392)
-                           298 UNPACK_SEQUENCE          2
-                           302 STORE_FAST               2 (key)
-                           304 STORE_FAST               3 (value)
-               
-               163         306 LOAD_FAST                0 (self)
-                           308 LOAD_ATTR               11 (span)
-                           318 LOAD_METHOD             12 (set_attribute)
-               
-               164         340 LOAD_GLOBAL              4 (SpanAttributes)
-                           352 LOAD_ATTR               13 (AGIFLOW_ASSOCIATION_PROPERTIES)
-                           362 FORMAT_VALUE             0
-                           364 LOAD_CONST               2 ('.')
-                           366 LOAD_FAST                2 (key)
-                           368 FORMAT_VALUE             0
-                           370 BUILD_STRING             3
-                           372 LOAD_FAST                3 (value)
-               
-               163         374 PRECALL                  2
-                           378 CALL                     2
-                           388 POP_TOP
-                           390 JUMP_BACKWARD           48 (to 296)
-               
-               167     >>  392 LOAD_FAST                0 (self)
-                           394 LOAD_ATTR                4 (context)
-                           404 LOAD_METHOD              6 (get)
-                           426 LOAD_GLOBAL             14 (ContextKeys)
-                           438 LOAD_ATTR               14 (PROMPT_SETTINGS)
-                           448 PRECALL                  1
-                           452 CALL                     1
-                           462 STORE_FAST               4 (prompt_settings)
-               
-               168         464 LOAD_FAST                4 (prompt_settings)
-                           466 POP_JUMP_FORWARD_IF_NONE    41 (to 550)
-               
-               169         468 LOAD_GLOBAL             31 (NULL + set_prompt_settings_context)
-                           480 LOAD_FAST                4 (prompt_settings)
-                           482 PRECALL                  1
-                           486 CALL                     1
-                           496 POP_TOP
-               
-               170         498 LOAD_GLOBAL             33 (NULL + set_prompt_attributes_from_context)
-                           510 LOAD_FAST                0 (self)
-                           512 LOAD_ATTR               11 (span)
-                           522 LOAD_FAST                0 (self)
-                           524 LOAD_ATTR                4 (context)
-                           534 PRECALL                  2
-                           538 CALL                     2
-                           548 POP_TOP
-               
-               172     >>  550 LOAD_FAST                0 (self)
-                           552 LOAD_ATTR                4 (context)
-                           562 LOAD_METHOD              6 (get)
-                           584 LOAD_GLOBAL             14 (ContextKeys)
-                           596 LOAD_ATTR               17 (WORKFLOW_NAME)
-                           606 PRECALL                  1
-                           610 CALL                     1
-                           620 STORE_FAST               5 (workflow_name)
-               
-               173         622 LOAD_FAST                5 (workflow_name)
-                           624 POP_JUMP_FORWARD_IF_NONE    41 (to 708)
-               
-               174         626 LOAD_GLOBAL             37 (NULL + set_workflow_name)
-                           638 LOAD_FAST                5 (workflow_name)
-                           640 PRECALL                  1
-                           644 CALL                     1
-                           654 POP_TOP
-               
-               175         656 LOAD_GLOBAL             39 (NULL + set_workflow_name_from_context)
-                           668 LOAD_FAST                0 (self)
-                           670 LOAD_ATTR               11 (span)
-                           680 LOAD_FAST                0 (self)
-                           682 LOAD_ATTR                4 (context)
-                           692 PRECALL                  2
-                           696 CALL                     2
-                           706 POP_TOP
-               
-               177     >>  708 LOAD_FAST                0 (self)
-                           710 LOAD_ATTR                4 (context)
-                           720 LOAD_METHOD              6 (get)
-                           742 LOAD_GLOBAL             14 (ContextKeys)
-                           754 LOAD_ATTR               20 (OVERRIDE_ENABLE_CONTENT_TRACING)
-                           764 PRECALL                  1
-                           768 CALL                     1
-                           778 STORE_FAST               6 (content_tracing)
-               
-               178         780 LOAD_FAST                6 (content_tracing)
-                           782 POP_JUMP_FORWARD_IF_NONE    15 (to 814)
-               
-               179         784 LOAD_GLOBAL             43 (NULL + set_override_enable_context_tracing)
-                           796 LOAD_FAST                6 (content_tracing)
-                           798 PRECALL                  1
-                           802 CALL                     1
-                           812 POP_TOP
-               
-               181     >>  814 LOAD_GLOBAL             45 (NULL + add_extra_spans)
-               
-               182         826 LOAD_FAST                0 (self)
-                           828 LOAD_ATTR               11 (span)
-               
-               183         838 LOAD_FAST                0 (self)
-                           840 LOAD_ATTR               23 (config)
-                           850 LOAD_METHOD              6 (get)
-                           872 LOAD_CONST               3 ('description')
-                           874 PRECALL                  1
-                           878 CALL                     1
-               
-               184         888 LOAD_FAST                0 (self)
-                           890 LOAD_ATTR               23 (config)
-                           900 LOAD_METHOD              6 (get)
-                           922 LOAD_CONST               4 ('prompt_settings')
-                           924 PRECALL                  1
-                           928 CALL                     1
-               
-               181         938 KW_NAMES                 5
-                           940 PRECALL                  3
-                           944 CALL                     3
-                           954 POP_TOP
-               
-               187         956 NOP
-               
-               188         958 LOAD_GLOBAL             49 (NULL + should_send_prompts)
-                           970 PRECALL                  0
-                           974 CALL                     0
-                           984 POP_JUMP_FORWARD_IF_FALSE   162 (to 1310)
-               
-               189         986 LOAD_CONST               6 ('')
-                           988 STORE_FAST               7 (input)
-               
-               190         990 LOAD_FAST                0 (self)
-                           992 LOAD_ATTR               23 (config)
-                          1002 LOAD_METHOD              6 (get)
-                          1024 LOAD_CONST               7 ('input_serializer')
-                          1026 PRECALL                  1
-                          1030 CALL                     1
-                          1040 STORE_FAST               8 (input_serializer)
-               
-               192        1042 LOAD_FAST                8 (input_serializer)
-                          1044 POP_JUMP_FORWARD_IF_NONE    34 (to 1114)
-                          1046 LOAD_GLOBAL             51 (NULL + callable)
-                          1058 LOAD_FAST                8 (input_serializer)
-                          1060 PRECALL                  1
-                          1064 CALL                     1
-                          1074 POP_JUMP_FORWARD_IF_FALSE    19 (to 1114)
-               
-               193        1076 PUSH_NULL
-                          1078 LOAD_FAST                8 (input_serializer)
-                          1080 LOAD_FAST                0 (self)
-                          1082 LOAD_ATTR               26 (args)
-                          1092 BUILD_MAP                0
-                          1094 LOAD_FAST                0 (self)
-                          1096 LOAD_ATTR               27 (kwargs)
-                          1106 DICT_MERGE               1
-                          1108 CALL_FUNCTION_EX         1
-                          1110 STORE_FAST               7 (input)
-                          1112 JUMP_FORWARD            28 (to 1170)
-               
-               195     >> 1114 LOAD_GLOBAL             57 (NULL + serialise_to_json)
-                          1126 LOAD_FAST                0 (self)
-                          1128 LOAD_ATTR               26 (args)
-                          1138 LOAD_FAST                0 (self)
-                          1140 LOAD_ATTR               27 (kwargs)
-                          1150 LOAD_CONST               8 (('args', 'kwargs'))
-                          1152 BUILD_CONST_KEY_MAP      2
-                          1154 PRECALL                  1
-                          1158 CALL                     1
-                          1168 STORE_FAST               7 (input)
-               
-               197     >> 1170 LOAD_GLOBAL             59 (NULL + isinstance)
-                          1182 LOAD_FAST                7 (input)
-                          1184 LOAD_GLOBAL             60 (str)
-                          1196 PRECALL                  2
-                          1200 CALL                     2
-                          1210 POP_JUMP_FORWARD_IF_TRUE    15 (to 1242)
-               
-               198        1212 LOAD_GLOBAL             57 (NULL + serialise_to_json)
-                          1224 LOAD_FAST                7 (input)
-                          1226 PRECALL                  1
-                          1230 CALL                     1
-                          1240 STORE_FAST               7 (input)
-               
-               200     >> 1242 LOAD_FAST                0 (self)
-                          1244 LOAD_METHOD              1 (set_span_attribute)
-               
-               201        1266 LOAD_GLOBAL              4 (SpanAttributes)
-                          1278 LOAD_ATTR               31 (AGIFLOW_ENTITY_INPUT)
-               
-               202        1288 LOAD_FAST                7 (input)
-               
-               200        1290 PRECALL                  2
-                          1294 CALL                     2
-                          1304 POP_TOP
-                          1306 LOAD_CONST               0 (None)
-                          1308 RETURN_VALUE
-               
-               188     >> 1310 LOAD_CONST               0 (None)
-                          1312 RETURN_VALUE
-                       >> 1314 PUSH_EXC_INFO
-               
-               204        1316 LOAD_GLOBAL             64 (TypeError)
-                          1328 CHECK_EXC_MATCH
-                          1330 POP_JUMP_FORWARD_IF_FALSE    37 (to 1406)
-                          1332 STORE_FAST               9 (e)
-               
-               205        1334 LOAD_GLOBAL             66 (logger)
-                          1346 LOAD_METHOD             34 (error)
-                          1368 LOAD_FAST                9 (e)
-                          1370 PRECALL                  1
-                          1374 CALL                     1
-                          1384 POP_TOP
-                          1386 POP_EXCEPT
-                          1388 LOAD_CONST               0 (None)
-                          1390 STORE_FAST               9 (e)
-                          1392 DELETE_FAST              9 (e)
-                          1394 LOAD_CONST               0 (None)
-                          1396 RETURN_VALUE
-                       >> 1398 LOAD_CONST               0 (None)
-                          1400 STORE_FAST               9 (e)
-                          1402 DELETE_FAST              9 (e)
-                          1404 RERAISE                  1
-               
-               204     >> 1406 RERAISE                  0
-                       >> 1408 COPY                     3
-                          1410 POP_EXCEPT
-                          1412 RERAISE                  1
+               161     >>   90 LOAD_CONST               0 (None)
+                            92 STORE_FAST               1 (prompt_settings)
+               
+               162          94 LOAD_CONST               0 (None)
+                            96 STORE_FAST               2 (association_properties)
+               
+               164          98 LOAD_FAST                0 (self)
+                           100 LOAD_ATTR                4 (context)
+                           110 POP_JUMP_FORWARD_IF_NONE   225 (to 562)
+                           112 LOAD_GLOBAL             11 (NULL + hasattr)
+                           124 LOAD_FAST                0 (self)
+                           126 LOAD_ATTR                4 (context)
+                           136 LOAD_CONST               1 ('get')
+                           138 PRECALL                  2
+                           142 CALL                     2
+                           152 POP_JUMP_FORWARD_IF_FALSE   204 (to 562)
+               
+               165         154 LOAD_FAST                0 (self)
+                           156 LOAD_ATTR                4 (context)
+                           166 LOAD_METHOD              6 (get)
+                           188 LOAD_GLOBAL             14 (ContextKeys)
+                           200 LOAD_ATTR                8 (ASSOCIATION_PROPERTIES)
+                           210 PRECALL                  1
+                           214 CALL                     1
+                           224 STORE_FAST               2 (association_properties)
+               
+               166         226 LOAD_FAST                0 (self)
+                           228 LOAD_ATTR                4 (context)
+                           238 LOAD_METHOD              6 (get)
+                           260 LOAD_GLOBAL             14 (ContextKeys)
+                           272 LOAD_ATTR                9 (PROMPT_SETTINGS)
+                           282 PRECALL                  1
+                           286 CALL                     1
+                           296 STORE_FAST               1 (prompt_settings)
+               
+               168         298 LOAD_FAST                0 (self)
+                           300 LOAD_ATTR                4 (context)
+                           310 LOAD_METHOD              6 (get)
+                           332 LOAD_GLOBAL             14 (ContextKeys)
+                           344 LOAD_ATTR               10 (WORKFLOW_NAME)
+                           354 PRECALL                  1
+                           358 CALL                     1
+                           368 STORE_FAST               3 (workflow_name)
+               
+               169         370 LOAD_FAST                3 (workflow_name)
+                           372 POP_JUMP_FORWARD_IF_NONE    41 (to 456)
+               
+               170         374 LOAD_GLOBAL             23 (NULL + set_workflow_name)
+                           386 LOAD_FAST                3 (workflow_name)
+                           388 PRECALL                  1
+                           392 CALL                     1
+                           402 POP_TOP
+               
+               171         404 LOAD_GLOBAL             25 (NULL + set_workflow_name_from_context)
+                           416 LOAD_FAST                0 (self)
+                           418 LOAD_ATTR               13 (span)
+                           428 LOAD_FAST                0 (self)
+                           430 LOAD_ATTR                4 (context)
+                           440 PRECALL                  2
+                           444 CALL                     2
+                           454 POP_TOP
+               
+               173     >>  456 LOAD_FAST                0 (self)
+                           458 LOAD_ATTR                4 (context)
+                           468 LOAD_METHOD              6 (get)
+                           490 LOAD_GLOBAL             14 (ContextKeys)
+                           502 LOAD_ATTR               14 (OVERRIDE_ENABLE_CONTENT_TRACING)
+                           512 PRECALL                  1
+                           516 CALL                     1
+                           526 STORE_FAST               4 (content_tracing)
+               
+               174         528 LOAD_FAST                4 (content_tracing)
+                           530 POP_JUMP_FORWARD_IF_NONE    15 (to 562)
+               
+               175         532 LOAD_GLOBAL             31 (NULL + set_override_enable_context_tracing)
+                           544 LOAD_FAST                4 (content_tracing)
+                           546 PRECALL                  1
+                           550 CALL                     1
+                           560 POP_TOP
+               
+               177     >>  562 LOAD_FAST                0 (self)
+                           564 LOAD_METHOD              1 (set_span_attribute)
+               
+               178         586 LOAD_GLOBAL             32 (AgiflowSpanAttributes)
+                           598 LOAD_ATTR               17 (AGIFLOW_ENTITY_DESCRIPTION)
+               
+               179         608 LOAD_FAST                0 (self)
+                           610 LOAD_ATTR               18 (config)
+                           620 LOAD_METHOD              6 (get)
+                           642 LOAD_CONST               2 ('description')
+                           644 PRECALL                  1
+                           648 CALL                     1
+               
+               177         658 PRECALL                  2
+                           662 CALL                     2
+                           672 POP_TOP
+               
+               182         674 LOAD_FAST                0 (self)
+                           676 LOAD_ATTR               18 (config)
+                           686 LOAD_METHOD              6 (get)
+                           708 LOAD_CONST               3 ('prompt_settings')
+                           710 PRECALL                  1
+                           714 CALL                     1
+                           724 STORE_FAST               5 (prompt_settings_config)
+               
+               183         726 LOAD_FAST                5 (prompt_settings_config)
+                           728 POP_JUMP_FORWARD_IF_NONE    36 (to 802)
+               
+               184         730 LOAD_GLOBAL             39 (NULL + callable)
+                           742 LOAD_FAST                5 (prompt_settings_config)
+                           744 PRECALL                  1
+                           748 CALL                     1
+                           758 POP_JUMP_FORWARD_IF_FALSE    19 (to 798)
+               
+               185         760 PUSH_NULL
+                           762 LOAD_FAST                5 (prompt_settings_config)
+                           764 LOAD_FAST                0 (self)
+                           766 LOAD_ATTR               20 (args)
+                           776 BUILD_MAP                0
+                           778 LOAD_FAST                0 (self)
+                           780 LOAD_ATTR               21 (kwargs)
+                           790 DICT_MERGE               1
+                           792 CALL_FUNCTION_EX         1
+                           794 STORE_FAST               1 (prompt_settings)
+                           796 JUMP_FORWARD             2 (to 802)
+               
+               187     >>  798 LOAD_FAST                5 (prompt_settings_config)
+                           800 STORE_FAST               1 (prompt_settings)
+               
+               189     >>  802 LOAD_FAST                0 (self)
+                           804 LOAD_ATTR               18 (config)
+                           814 LOAD_METHOD              6 (get)
+                           836 LOAD_CONST               4 ('association_properties')
+                           838 PRECALL                  1
+                           842 CALL                     1
+                           852 STORE_FAST               6 (association_properties_config)
+               
+               190         854 LOAD_FAST                6 (association_properties_config)
+                           856 POP_JUMP_FORWARD_IF_NONE    36 (to 930)
+               
+               191         858 LOAD_GLOBAL             39 (NULL + callable)
+                           870 LOAD_FAST                6 (association_properties_config)
+                           872 PRECALL                  1
+                           876 CALL                     1
+                           886 POP_JUMP_FORWARD_IF_FALSE    19 (to 926)
+               
+               192         888 PUSH_NULL
+                           890 LOAD_FAST                6 (association_properties_config)
+                           892 LOAD_FAST                0 (self)
+                           894 LOAD_ATTR               20 (args)
+                           904 BUILD_MAP                0
+                           906 LOAD_FAST                0 (self)
+                           908 LOAD_ATTR               21 (kwargs)
+                           918 DICT_MERGE               1
+                           920 CALL_FUNCTION_EX         1
+                           922 STORE_FAST               2 (association_properties)
+                           924 JUMP_FORWARD             2 (to 930)
+               
+               194     >>  926 LOAD_FAST                6 (association_properties_config)
+                           928 STORE_FAST               2 (association_properties)
+               
+               196     >>  930 LOAD_FAST                1 (prompt_settings)
+                           932 POP_JUMP_FORWARD_IF_NONE    41 (to 1016)
+               
+               197         934 LOAD_GLOBAL             45 (NULL + set_prompt_settings_context)
+                           946 LOAD_FAST                1 (prompt_settings)
+                           948 PRECALL                  1
+                           952 CALL                     1
+                           962 POP_TOP
+               
+               198         964 LOAD_GLOBAL             47 (NULL + set_prompt_attributes_from_context)
+                           976 LOAD_FAST                0 (self)
+                           978 LOAD_ATTR               13 (span)
+                           988 LOAD_FAST                0 (self)
+                           990 LOAD_ATTR                4 (context)
+                          1000 PRECALL                  2
+                          1004 CALL                     2
+                          1014 POP_TOP
+               
+               200     >> 1016 LOAD_FAST                2 (association_properties)
+                          1018 POP_JUMP_FORWARD_IF_NONE    83 (to 1186)
+               
+               201        1020 LOAD_GLOBAL             49 (NULL + set_association_properties)
+                          1032 LOAD_FAST                2 (association_properties)
+                          1034 PRECALL                  1
+                          1038 CALL                     1
+                          1048 POP_TOP
+               
+               202        1050 LOAD_FAST                2 (association_properties)
+                          1052 LOAD_METHOD             25 (items)
+                          1074 PRECALL                  0
+                          1078 CALL                     0
+                          1088 GET_ITER
+                       >> 1090 FOR_ITER                47 (to 1186)
+                          1092 UNPACK_SEQUENCE          2
+                          1096 STORE_FAST               7 (key)
+                          1098 STORE_FAST               8 (value)
+               
+               203        1100 LOAD_FAST                0 (self)
+                          1102 LOAD_ATTR               13 (span)
+                          1112 LOAD_METHOD             26 (set_attribute)
+               
+               204        1134 LOAD_GLOBAL              4 (SpanAttributes)
+                          1146 LOAD_ATTR               27 (AGIFLOW_ASSOCIATION_PROPERTIES)
+                          1156 FORMAT_VALUE             0
+                          1158 LOAD_CONST               5 ('.')
+                          1160 LOAD_FAST                7 (key)
+                          1162 FORMAT_VALUE             0
+                          1164 BUILD_STRING             3
+               
+               205        1166 LOAD_FAST                8 (value)
+               
+               203        1168 PRECALL                  2
+                          1172 CALL                     2
+                          1182 POP_TOP
+                          1184 JUMP_BACKWARD           48 (to 1090)
+               
+               208     >> 1186 NOP
+               
+               209        1188 LOAD_GLOBAL             57 (NULL + should_send_prompts)
+                          1200 PRECALL                  0
+                          1204 CALL                     0
+                          1214 POP_JUMP_FORWARD_IF_FALSE   162 (to 1540)
+               
+               210        1216 LOAD_CONST               6 ('')
+                          1218 STORE_FAST               9 (input)
+               
+               211        1220 LOAD_FAST                0 (self)
+                          1222 LOAD_ATTR               18 (config)
+                          1232 LOAD_METHOD              6 (get)
+                          1254 LOAD_CONST               7 ('input_serializer')
+                          1256 PRECALL                  1
+                          1260 CALL                     1
+                          1270 STORE_FAST              10 (input_serializer)
+               
+               213        1272 LOAD_FAST               10 (input_serializer)
+                          1274 POP_JUMP_FORWARD_IF_NONE    34 (to 1344)
+                          1276 LOAD_GLOBAL             39 (NULL + callable)
+                          1288 LOAD_FAST               10 (input_serializer)
+                          1290 PRECALL                  1
+                          1294 CALL                     1
+                          1304 POP_JUMP_FORWARD_IF_FALSE    19 (to 1344)
+               
+               214        1306 PUSH_NULL
+                          1308 LOAD_FAST               10 (input_serializer)
+                          1310 LOAD_FAST                0 (self)
+                          1312 LOAD_ATTR               20 (args)
+                          1322 BUILD_MAP                0
+                          1324 LOAD_FAST                0 (self)
+                          1326 LOAD_ATTR               21 (kwargs)
+                          1336 DICT_MERGE               1
+                          1338 CALL_FUNCTION_EX         1
+                          1340 STORE_FAST               9 (input)
+                          1342 JUMP_FORWARD            28 (to 1400)
+               
+               216     >> 1344 LOAD_GLOBAL             59 (NULL + serialise_to_json)
+                          1356 LOAD_FAST                0 (self)
+                          1358 LOAD_ATTR               20 (args)
+                          1368 LOAD_FAST                0 (self)
+                          1370 LOAD_ATTR               21 (kwargs)
+                          1380 LOAD_CONST               8 (('args', 'kwargs'))
+                          1382 BUILD_CONST_KEY_MAP      2
+                          1384 PRECALL                  1
+                          1388 CALL                     1
+                          1398 STORE_FAST               9 (input)
+               
+               218     >> 1400 LOAD_GLOBAL             61 (NULL + isinstance)
+                          1412 LOAD_FAST                9 (input)
+                          1414 LOAD_GLOBAL             62 (str)
+                          1426 PRECALL                  2
+                          1430 CALL                     2
+                          1440 POP_JUMP_FORWARD_IF_TRUE    15 (to 1472)
+               
+               219        1442 LOAD_GLOBAL             59 (NULL + serialise_to_json)
+                          1454 LOAD_FAST                9 (input)
+                          1456 PRECALL                  1
+                          1460 CALL                     1
+                          1470 STORE_FAST               9 (input)
+               
+               221     >> 1472 LOAD_FAST                0 (self)
+                          1474 LOAD_METHOD              1 (set_span_attribute)
+               
+               222        1496 LOAD_GLOBAL              4 (SpanAttributes)
+                          1508 LOAD_ATTR               32 (AGIFLOW_ENTITY_INPUT)
+               
+               223        1518 LOAD_FAST                9 (input)
+               
+               221        1520 PRECALL                  2
+                          1524 CALL                     2
+                          1534 POP_TOP
+                          1536 LOAD_CONST               0 (None)
+                          1538 RETURN_VALUE
+               
+               209     >> 1540 LOAD_CONST               0 (None)
+                          1542 RETURN_VALUE
+                       >> 1544 PUSH_EXC_INFO
+               
+               225        1546 LOAD_GLOBAL             66 (TypeError)
+                          1558 CHECK_EXC_MATCH
+                          1560 POP_JUMP_FORWARD_IF_FALSE    37 (to 1636)
+                          1562 STORE_FAST              11 (e)
+               
+               226        1564 LOAD_GLOBAL             68 (logger)
+                          1576 LOAD_METHOD             35 (error)
+                          1598 LOAD_FAST               11 (e)
+                          1600 PRECALL                  1
+                          1604 CALL                     1
+                          1614 POP_TOP
+                          1616 POP_EXCEPT
+                          1618 LOAD_CONST               0 (None)
+                          1620 STORE_FAST              11 (e)
+                          1622 DELETE_FAST             11 (e)
+                          1624 LOAD_CONST               0 (None)
+                          1626 RETURN_VALUE
+                       >> 1628 LOAD_CONST               0 (None)
+                          1630 STORE_FAST              11 (e)
+                          1632 DELETE_FAST             11 (e)
+                          1634 RERAISE                  1
+               
+               225     >> 1636 RERAISE                  0
+                       >> 1638 COPY                     3
+                          1640 POP_EXCEPT
+                          1642 RERAISE                  1
                ExceptionTable:
-                 958 to 1304 -> 1314 [0]
-                 1314 to 1332 -> 1408 [1] lasti
-                 1334 to 1384 -> 1398 [1] lasti
-                 1398 to 1406 -> 1408 [1] lasti
+                 1188 to 1534 -> 1544 [0]
+                 1544 to 1562 -> 1638 [1] lasti
+                 1564 to 1614 -> 1628 [1] lasti
+                 1628 to 1636 -> 1638 [1] lasti
                consts
                   None
                   'get'
-                  '.'
                   'description'
                   'prompt_settings'
-                  ('description', 'prompt_settings')
+                  'association_properties'
+                  '.'
                   ''
                   'input_serializer'
                   ('args', 'kwargs')
-               names      ('name', 'set_span_attribute', 'SpanAttributes', 'AGIFLOW_ENTITY_NAME', 'context', 'hasattr', 'get', 'ContextKeys', 'ASSOCIATION_PROPERTIES', 'set_association_properties', 'items', 'span', 'set_attribute', 'AGIFLOW_ASSOCIATION_PROPERTIES', 'PROMPT_SETTINGS', 'set_prompt_settings_context', 'set_prompt_attributes_from_context', 'WORKFLOW_NAME', 'set_workflow_name', 'set_workflow_name_from_context', 'OVERRIDE_ENABLE_CONTENT_TRACING', 'set_override_enable_context_tracing', 'add_extra_spans', 'config', 'should_send_prompts', 'callable', 'args', 'kwargs', 'serialise_to_json', 'isinstance', 'str', 'AGIFLOW_ENTITY_INPUT', 'TypeError', 'logger', 'error')
-               varnames   ('self', 'association_properties', 'key', 'value', 'prompt_settings', 'workflow_name', 'content_tracing', 'input', 'input_serializer', 'e')
+               names      ('name', 'set_span_attribute', 'SpanAttributes', 'AGIFLOW_ENTITY_NAME', 'context', 'hasattr', 'get', 'ContextKeys', 'ASSOCIATION_PROPERTIES', 'PROMPT_SETTINGS', 'WORKFLOW_NAME', 'set_workflow_name', 'set_workflow_name_from_context', 'span', 'OVERRIDE_ENABLE_CONTENT_TRACING', 'set_override_enable_context_tracing', 'AgiflowSpanAttributes', 'AGIFLOW_ENTITY_DESCRIPTION', 'config', 'callable', 'args', 'kwargs', 'set_prompt_settings_context', 'set_prompt_attributes_from_context', 'set_association_properties', 'items', 'set_attribute', 'AGIFLOW_ASSOCIATION_PROPERTIES', 'should_send_prompts', 'serialise_to_json', 'isinstance', 'str', 'AGIFLOW_ENTITY_INPUT', 'TypeError', 'logger', 'error')
+               varnames   ('self', 'prompt_settings', 'association_properties', 'workflow_name', 'content_tracing', 'prompt_settings_config', 'association_properties_config', 'key', 'value', 'input', 'input_serializer', 'e')
                freevars   ()
                cellvars   ()
                filename   '/Users/vuongngo/workspace/agiflow/packages/python/agiflow-sdk/agiflow/opentelemetry/trace_decorators/wrapper.py'
                name       'capture_input'
-               firstlineno 153
+               firstlineno 157
                lnotab
-                  0x02010e014a033c01480104011e013201220122ff1204480104011e0134
-                  02480104011e013402480104011e020c010c01320132fd120602011c0104
-                  0134022201260238022a011e021801160102fe14f40610120148ff
+                  0x02010e014a0204010402380148014802480104011e013402480104011e
+                  021801160132fe1005340104011e0126020402340104011e012602040204
+                  011e01340204011e0132012201200102fe120502011c0104013402220126
+                  0238022a011e021801160102fe14f40610120148ff
             code
                argcount  : 2
                nlocals   : 5
                stacksize : 5
                flags     : 3
                code
                   0x97000900740100000000000000000000a6000000ab0000000000000000
@@ -1368,104 +1479,104 @@
                   00730f740d000000000000000000007c01a6010000ab0100000000000000
                   007d027c00a0090000000000000000000000000000000000000000741400
                   0000000000000000006a0b00000000000000007c02a6020000ab02000000
                   000000000001006400530064005300230074180000000000000000000024
                   0072257d04741a00000000000000000000a00e0000000000000000000000
                   0000000000000000007c04a6010000ab0100000000000000000100590064
                   007d047e046400530064007d047e0477017700780359007701
-               207           0 RESUME                   0
+               228           0 RESUME                   0
                
-               208           2 NOP
+               229           2 NOP
                
-               209           4 LOAD_GLOBAL              1 (NULL + should_send_prompts)
+               230           4 LOAD_GLOBAL              1 (NULL + should_send_prompts)
                             16 PRECALL                  0
                             20 CALL                     0
                             30 POP_JUMP_FORWARD_IF_FALSE   154 (to 340)
                
-               210          32 LOAD_CONST               1 ('')
+               231          32 LOAD_CONST               1 ('')
                             34 STORE_FAST               2 (output)
                
-               211          36 LOAD_FAST                0 (self)
+               232          36 LOAD_FAST                0 (self)
                             38 LOAD_ATTR                1 (config)
                             48 LOAD_METHOD              2 (get)
                             70 LOAD_CONST               2 ('output_serializer')
                             72 PRECALL                  1
                             76 CALL                     1
                             86 STORE_FAST               3 (output_serializer)
                
-               212          88 LOAD_FAST                3 (output_serializer)
+               233          88 LOAD_FAST                3 (output_serializer)
                             90 POP_JUMP_FORWARD_IF_NONE    35 (to 162)
                             92 LOAD_GLOBAL              7 (NULL + callable)
                            104 LOAD_FAST                3 (output_serializer)
                            106 PRECALL                  1
                            110 CALL                     1
                            120 POP_JUMP_FORWARD_IF_FALSE    20 (to 162)
                
-               213         122 PUSH_NULL
+               234         122 PUSH_NULL
                            124 LOAD_FAST                3 (output_serializer)
                            126 LOAD_FAST                0 (self)
                            128 LOAD_ATTR                4 (args)
                            138 LOAD_CONST               3 ('result')
                            140 LOAD_FAST                1 (result)
                            142 BUILD_MAP                1
                            144 LOAD_FAST                0 (self)
                            146 LOAD_ATTR                5 (kwargs)
                            156 DICT_MERGE               1
                            158 CALL_FUNCTION_EX         1
                            160 STORE_FAST               2 (output)
                
-               214     >>  162 LOAD_FAST                1 (result)
+               235     >>  162 LOAD_FAST                1 (result)
                            164 POP_JUMP_FORWARD_IF_NONE    17 (to 200)
                
-               215         166 LOAD_FAST                3 (output_serializer)
+               236         166 LOAD_FAST                3 (output_serializer)
                            168 POP_JUMP_FORWARD_IF_TRUE    15 (to 200)
                
-               216         170 LOAD_GLOBAL             13 (NULL + serialise_to_json)
+               237         170 LOAD_GLOBAL             13 (NULL + serialise_to_json)
                            182 LOAD_FAST                1 (result)
                            184 PRECALL                  1
                            188 CALL                     1
                            198 STORE_FAST               2 (output)
                
-               218     >>  200 LOAD_GLOBAL             15 (NULL + isinstance)
+               239     >>  200 LOAD_GLOBAL             15 (NULL + isinstance)
                            212 LOAD_FAST                2 (output)
                            214 LOAD_GLOBAL             16 (str)
                            226 PRECALL                  2
                            230 CALL                     2
                            240 POP_JUMP_FORWARD_IF_TRUE    15 (to 272)
                
-               219         242 LOAD_GLOBAL             13 (NULL + serialise_to_json)
+               240         242 LOAD_GLOBAL             13 (NULL + serialise_to_json)
                            254 LOAD_FAST                1 (result)
                            256 PRECALL                  1
                            260 CALL                     1
                            270 STORE_FAST               2 (output)
                
-               221     >>  272 LOAD_FAST                0 (self)
+               242     >>  272 LOAD_FAST                0 (self)
                            274 LOAD_METHOD              9 (set_span_attribute)
                
-               222         296 LOAD_GLOBAL             20 (SpanAttributes)
+               243         296 LOAD_GLOBAL             20 (SpanAttributes)
                            308 LOAD_ATTR               11 (AGIFLOW_ENTITY_OUTPUT)
                
-               223         318 LOAD_FAST                2 (output)
+               244         318 LOAD_FAST                2 (output)
                
-               221         320 PRECALL                  2
+               242         320 PRECALL                  2
                            324 CALL                     2
                            334 POP_TOP
                            336 LOAD_CONST               0 (None)
                            338 RETURN_VALUE
                
-               209     >>  340 LOAD_CONST               0 (None)
+               230     >>  340 LOAD_CONST               0 (None)
                            342 RETURN_VALUE
                        >>  344 PUSH_EXC_INFO
                
-               226         346 LOAD_GLOBAL             24 (TypeError)
+               247         346 LOAD_GLOBAL             24 (TypeError)
                            358 CHECK_EXC_MATCH
                            360 POP_JUMP_FORWARD_IF_FALSE    37 (to 436)
                            362 STORE_FAST               4 (e)
                
-               227         364 LOAD_GLOBAL             26 (logger)
+               248         364 LOAD_GLOBAL             26 (logger)
                            376 LOAD_METHOD             14 (error)
                            398 LOAD_FAST                4 (e)
                            400 PRECALL                  1
                            404 CALL                     1
                            414 POP_TOP
                            416 POP_EXCEPT
                            418 LOAD_CONST               0 (None)
@@ -1474,15 +1585,15 @@
                            424 LOAD_CONST               0 (None)
                            426 RETURN_VALUE
                        >>  428 LOAD_CONST               0 (None)
                            430 STORE_FAST               4 (e)
                            432 DELETE_FAST              4 (e)
                            434 RERAISE                  1
                
-               226     >>  436 RERAISE                  0
+               247     >>  436 RERAISE                  0
                        >>  438 COPY                     3
                            440 POP_EXCEPT
                            442 RERAISE                  1
                ExceptionTable:
                  4 to 334 -> 344 [0]
                  344 to 362 -> 438 [1] lasti
                  364 to 414 -> 428 [1] lasti
@@ -1494,29 +1605,30 @@
                   'result'
                names      ('should_send_prompts', 'config', 'get', 'callable', 'args', 'kwargs', 'serialise_to_json', 'isinstance', 'str', 'set_span_attribute', 'SpanAttributes', 'AGIFLOW_ENTITY_OUTPUT', 'TypeError', 'logger', 'error')
                varnames   ('self', 'result', 'output', 'output_serializer', 'e')
                freevars   ()
                cellvars   ()
                filename   '/Users/vuongngo/workspace/agiflow/packages/python/agiflow-sdk/agiflow/opentelemetry/trace_decorators/wrapper.py'
                name       'capture_output'
-               firstlineno 207
+               firstlineno 228
                lnotab
                   0x020102011c010401340122012801040104011e022a011e021801160102
                   fe14f40611120148ff
-         names      ('__name__', '__module__', '__qualname__', '__doc__', 'Span', '__annotations__', 'Optional', 'AgiflowServiceTypes', 'Any', 'SharedKwargsWithHooks', 'Dict', 'str', 'TASK', '__init__', 'staticmethod', 'get_span_name', 'get_service_type', 'set_span_attribute', 'capture_input', 'capture_output')
+         names      ('__name__', '__module__', '__qualname__', '__doc__', 'Span', '__annotations__', 'Optional', 'AgiflowServiceTypes', 'Any', 'SharedKwargsWithHooks', 'Dict', 'str', 'TASK', '__init__', 'staticmethod', 'is_flush_on_exit', 'get_span_name', 'get_service_type', 'set_span_attribute', 'capture_input', 'capture_output')
          varnames   ()
          freevars   ()
          cellvars   ()
          filename   '/Users/vuongngo/workspace/agiflow/packages/python/agiflow-sdk/agiflow/opentelemetry/trace_decorators/wrapper.py'
          name       'BaseSpanCapture'
          firstlineno 80
          lnotab
             0x0c0104040a0116010a010a010a010a010a011a01160502010c02020102
-            f906030efd02040efc020802f80819020202010c0102fd04010eff02020e
-            fe020302fd06ff0e01020e020104ff0e010206060b0636
+            f906030efd02040efc020802f80819020104ff0e010203020202010c0102
+            fd04010eff02020efe020302fd06ff0e01020e020104ff0e010206060b06
+            47
       'BaseSpanCapture'
       'name'
       'tlp_service_type'
       'config'
       code
          argcount  : 4
          nlocals   : 6
@@ -1527,27 +1639,27 @@
             057c055300
                        0 MAKE_CELL                0 (name)
                        2 MAKE_CELL                1 (tlp_service_type)
                        4 MAKE_CELL                2 (span_kind)
                        6 MAKE_CELL                3 (SpanCapture)
                        8 MAKE_CELL                4 (config)
          
-         230          10 RESUME                   0
+         251          10 RESUME                   0
          
-         237          12 LOAD_CLOSURE             3 (SpanCapture)
+         258          12 LOAD_CLOSURE             3 (SpanCapture)
                       14 LOAD_CLOSURE             4 (config)
                       16 LOAD_CLOSURE             0 (name)
                       18 LOAD_CLOSURE             2 (span_kind)
                       20 LOAD_CLOSURE             1 (tlp_service_type)
                       22 BUILD_TUPLE              5
-                      24 LOAD_CONST               1 (<code object decorate, file "/Users/vuongngo/workspace/agiflow/packages/python/agiflow-sdk/agiflow/opentelemetry/trace_decorators/wrapper.py", line 237>)
+                      24 LOAD_CONST               1 (<code object decorate, file "/Users/vuongngo/workspace/agiflow/packages/python/agiflow-sdk/agiflow/opentelemetry/trace_decorators/wrapper.py", line 258>)
                       26 MAKE_FUNCTION            8 (closure)
                       28 STORE_FAST               5 (decorate)
          
-         294          30 LOAD_FAST                5 (decorate)
+         316          30 LOAD_FAST                5 (decorate)
                       32 RETURN_VALUE
          consts
             None
             code
                argcount  : 1
                nlocals   : 2
                stacksize : 7
@@ -1555,37 +1667,37 @@
                code
                   0x9505870097007401000000000000000000008900a6010000ab01000000
                   0000000000880288038800880488058806660664018408a6000000ab0000
                   000000000000007d017c015300
                              0 COPY_FREE_VARS           5
                              2 MAKE_CELL                0 (fn)
                
-               237           4 RESUME                   0
+               258           4 RESUME                   0
                
-               238           6 LOAD_GLOBAL              1 (NULL + wraps)
+               259           6 LOAD_GLOBAL              1 (NULL + wraps)
                             18 LOAD_DEREF               0 (fn)
                             20 PRECALL                  1
                             24 CALL                     1
                
-               239          34 LOAD_CLOSURE             2 (SpanCapture)
+               260          34 LOAD_CLOSURE             2 (SpanCapture)
                             36 LOAD_CLOSURE             3 (config)
                             38 LOAD_CLOSURE             0 (fn)
                             40 LOAD_CLOSURE             4 (name)
                             42 LOAD_CLOSURE             5 (span_kind)
                             44 LOAD_CLOSURE             6 (tlp_service_type)
                             46 BUILD_TUPLE              6
-                            48 LOAD_CONST               1 (<code object wrap, file "/Users/vuongngo/workspace/agiflow/packages/python/agiflow-sdk/agiflow/opentelemetry/trace_decorators/wrapper.py", line 238>)
+                            48 LOAD_CONST               1 (<code object wrap, file "/Users/vuongngo/workspace/agiflow/packages/python/agiflow-sdk/agiflow/opentelemetry/trace_decorators/wrapper.py", line 259>)
                             50 MAKE_FUNCTION            8 (closure)
                
-               238          52 PRECALL                  0
+               259          52 PRECALL                  0
                             56 CALL                     0
                
-               239          66 STORE_FAST               1 (wrap)
+               260          66 STORE_FAST               1 (wrap)
                
-               292          68 LOAD_FAST                1 (wrap)
+               314          68 LOAD_FAST                1 (wrap)
                             70 RETURN_VALUE
                consts
                   None
                   code
                      argcount  : 0
                      nlocals   : 12
                      stacksize : 12
@@ -1595,392 +1707,399 @@
                         00ab00000000000000000073080200890e7c0069007c01a4018e01530089
                         0ca0020000000000000000000000000000000000000000890f8911890eac
                         01a6030000ab0300000000000000005c0200007d027d03890da003000000
                         00000000000000000000000000000000006402a6010000ab010000000000
                         0000007d0464007d057c0481267409000000000000000000007c04a60100
                         00ab010000000000000000721702007c047c0069007c01a4018e017d0674
                         0b000000000000000000007c06a6010000ab0100000000000000007d0574
-                        0d00000000000000000000a6000000ab00000000000000000035007d077c
-                        07a00700000000000000000000000000000000000000007c0289107c05ac
-                        03a6030000ab03000000000000000035007d080200890c7c00890f7c037c
-                        08890e890d7c0564049c067c01a4018e017d097411000000000000000000
-                        007c096405a6020000ab0200000000000000007228740900000000000000
-                        0000007c096a090000000000000000a6010000ab01000000000000000072
-                        147c09a0090000000000000000000000000000000000000000a6000000ab
-                        000000000000000000010009000200890e7c0069007c01a4018e017d0a74
-                        11000000000000000000007c096406a6020000ab02000000000000000072
-                        297409000000000000000000007c096a0a0000000000000000a6010000ab
-                        01000000000000000072157c09a00a000000000000000000000000000000
-                        00000000007c0aa6010000ab01000000000000000001007c08a00b000000
-                        0000000000000000000000000000000000a6000000ab0000000000000000
-                        0072337c08a00c0000000000000000000000000000000000000000741a00
-                        0000000000000000006a0e0000000000000000a6010000ab010000000000
-                        00000001007c08a00f0000000000000000000000000000000000000000a6
-                        000000ab00000000000000000001007c0a6302640064006400a6020000ab
-                        02000000000000000001006302640064006400a6020000ab020000000000
-                        000000010053002300742000000000000000000000240072557d0b7c08a0
-                        1100000000000000000000000000000000000000007c0ba6010000ab0100
-                        0000000000000001007c08a00c0000000000000000000000000000000000
-                        000000742500000000000000000000741a000000000000000000006a1300
-                        000000000000007429000000000000000000007c0ba6010000ab01000000
-                        0000000000a6020000ab020000000000000000a6010000ab010000000000
-                        0000000100820064007d0b7e0b7701770078035900770123003100730477
-                        0278035900770101005900010001000900640064006400a6020000ab0200
-                        000000000000000100640053002300310073047702780359007701010059
-                        000100010064005300
+                        0d00000000000000000000890ca007000000000000000000000000000000
+                        0000000000a6000000ab000000000000000000ac03a6010000ab01000000
+                        000000000035007d077c07a0080000000000000000000000000000000000
+                        0000007c0289107c05ac04a6030000ab03000000000000000035007d0802
+                        00890c7c00890f7c037c08890e890d7c0564059c067c01a4018e017d0974
+                        13000000000000000000007c096406a6020000ab02000000000000000072
+                        287409000000000000000000007c096a0a0000000000000000a6010000ab
+                        01000000000000000072147c09a00a000000000000000000000000000000
+                        0000000000a6000000ab000000000000000000010009000200890e7c0069
+                        007c01a4018e017d0a7413000000000000000000007c096407a6020000ab
+                        02000000000000000072297409000000000000000000007c096a0b000000
+                        0000000000a6010000ab01000000000000000072157c09a00b0000000000
+                        0000000000000000000000000000007c0aa6010000ab0100000000000000
+                        0001007c08a00c0000000000000000000000000000000000000000a60000
+                        00ab00000000000000000072337c08a00d00000000000000000000000000
+                        00000000000000741c000000000000000000006a0f0000000000000000a6
+                        010000ab01000000000000000001007c08a0100000000000000000000000
+                        000000000000000000a6000000ab00000000000000000001007c0a630264
+                        0064006400a6020000ab02000000000000000001006302640064006400a6
+                        020000ab0200000000000000000100530023007422000000000000000000
+                        00240072557d0b7c08a01200000000000000000000000000000000000000
+                        007c0ba6010000ab01000000000000000001007c08a00d00000000000000
+                        00000000000000000000000000742700000000000000000000741c000000
+                        000000000000006a140000000000000000742b000000000000000000007c
+                        0ba6010000ab010000000000000000a6020000ab020000000000000000a6
+                        010000ab0100000000000000000100820064007d0b7e0b77017700780359
+                        007701230031007304770278035900770101005900010001000900640064
+                        006400a6020000ab02000000000000000001006400530023003100730477
+                        02780359007701010059000100010064005300
                                    0 COPY_FREE_VARS           6
                      
-                     238           2 RESUME                   0
+                     259           2 RESUME                   0
                      
-                     240           4 LOAD_GLOBAL              1 (NULL + TracerWrapper)
+                     261           4 LOAD_GLOBAL              1 (NULL + TracerWrapper)
                                   16 LOAD_ATTR                1 (verify_initialized)
                                   26 PRECALL                  0
                                   30 CALL                     0
                                   40 POP_JUMP_FORWARD_IF_TRUE     8 (to 58)
                      
-                     241          42 PUSH_NULL
+                     262          42 PUSH_NULL
                                   44 LOAD_DEREF              14 (fn)
                                   46 LOAD_FAST                0 (args)
                                   48 BUILD_MAP                0
                                   50 LOAD_FAST                1 (kwargs)
                                   52 DICT_MERGE               1
                                   54 CALL_FUNCTION_EX         1
                                   56 RETURN_VALUE
                      
-                     243     >>   58 LOAD_DEREF              12 (SpanCapture)
+                     264     >>   58 LOAD_DEREF              12 (SpanCapture)
                                   60 LOAD_METHOD              2 (get_span_name)
                      
-                     244          82 LOAD_DEREF              15 (name)
+                     265          82 LOAD_DEREF              15 (name)
                      
-                     245          84 LOAD_DEREF              17 (tlp_service_type)
+                     266          84 LOAD_DEREF              17 (tlp_service_type)
                      
-                     246          86 LOAD_DEREF              14 (fn)
+                     267          86 LOAD_DEREF              14 (fn)
                      
-                     243          88 KW_NAMES                 1
+                     264          88 KW_NAMES                 1
                                   90 PRECALL                  3
                                   94 CALL                     3
                                  104 UNPACK_SEQUENCE          2
                                  108 STORE_FAST               2 (span_name)
                                  110 STORE_FAST               3 (service_type)
                      
-                     249         112 LOAD_DEREF              13 (config)
+                     270         112 LOAD_DEREF              13 (config)
                                  114 LOAD_METHOD              3 (get)
                                  136 LOAD_CONST               2 ('context_parser')
                                  138 PRECALL                  1
                                  142 CALL                     1
                                  152 STORE_FAST               4 (context_parser)
                      
-                     250         154 LOAD_CONST               0 (None)
+                     271         154 LOAD_CONST               0 (None)
                                  156 STORE_FAST               5 (context)
                      
-                     251         158 LOAD_FAST                4 (context_parser)
+                     272         158 LOAD_FAST                4 (context_parser)
                                  160 POP_JUMP_FORWARD_IF_NONE    38 (to 238)
                                  162 LOAD_GLOBAL              9 (NULL + callable)
                                  174 LOAD_FAST                4 (context_parser)
                                  176 PRECALL                  1
                                  180 CALL                     1
                                  190 POP_JUMP_FORWARD_IF_FALSE    23 (to 238)
                      
-                     252         192 PUSH_NULL
+                     273         192 PUSH_NULL
                                  194 LOAD_FAST                4 (context_parser)
                                  196 LOAD_FAST                0 (args)
                                  198 BUILD_MAP                0
                                  200 LOAD_FAST                1 (kwargs)
                                  202 DICT_MERGE               1
                                  204 CALL_FUNCTION_EX         1
                                  206 STORE_FAST               6 (carrier)
                      
-                     253         208 LOAD_GLOBAL             11 (NULL + get_trace_context_from_carrier)
+                     274         208 LOAD_GLOBAL             11 (NULL + get_trace_context_from_carrier)
                                  220 LOAD_FAST                6 (carrier)
                                  222 PRECALL                  1
                                  226 CALL                     1
                                  236 STORE_FAST               5 (context)
                      
-                     255     >>  238 LOAD_GLOBAL             13 (NULL + get_tracer)
-                                 250 PRECALL                  0
-                                 254 CALL                     0
-                                 264 BEFORE_WITH
-                                 266 STORE_FAST               7 (tracer)
-                     
-                     256         268 LOAD_FAST                7 (tracer)
-                                 270 LOAD_METHOD              7 (start_as_current_span)
-                                 292 LOAD_FAST                2 (span_name)
-                                 294 LOAD_DEREF              16 (span_kind)
-                                 296 LOAD_FAST                5 (context)
-                                 298 KW_NAMES                 3
-                                 300 PRECALL                  3
-                                 304 CALL                     3
-                                 314 BEFORE_WITH
-                                 316 STORE_FAST               8 (span)
-                     
-                     257         318 PUSH_NULL
-                                 320 LOAD_DEREF              12 (SpanCapture)
-                     
-                     258         322 LOAD_FAST                0 (args)
-                     
-                     259         324 LOAD_DEREF              15 (name)
-                     
-                     260         326 LOAD_FAST                3 (service_type)
-                     
-                     261         328 LOAD_FAST                8 (span)
-                     
-                     262         330 LOAD_DEREF              14 (fn)
-                     
-                     263         332 LOAD_DEREF              13 (config)
-                     
-                     264         334 LOAD_FAST                5 (context)
-                     
-                     257         336 LOAD_CONST               4 (('name', 'service_type', 'span', 'instance', 'config', 'context'))
-                                 338 BUILD_CONST_KEY_MAP      6
-                     
-                     265         340 LOAD_FAST                1 (kwargs)
-                     
-                     257         342 DICT_MERGE               1
-                                 344 CALL_FUNCTION_EX         1
-                                 346 STORE_FAST               9 (span_capture)
-                     
-                     267         348 LOAD_GLOBAL             17 (NULL + hasattr)
-                                 360 LOAD_FAST                9 (span_capture)
-                                 362 LOAD_CONST               5 ('capture_input')
-                                 364 PRECALL                  2
-                                 368 CALL                     2
-                                 378 POP_JUMP_FORWARD_IF_FALSE    40 (to 460)
-                                 380 LOAD_GLOBAL              9 (NULL + callable)
-                                 392 LOAD_FAST                9 (span_capture)
-                                 394 LOAD_ATTR                9 (capture_input)
-                                 404 PRECALL                  1
-                                 408 CALL                     1
-                                 418 POP_JUMP_FORWARD_IF_FALSE    20 (to 460)
-                     
-                     268         420 LOAD_FAST                9 (span_capture)
-                                 422 LOAD_METHOD              9 (capture_input)
-                                 444 PRECALL                  0
-                                 448 CALL                     0
-                                 458 POP_TOP
-                     
-                     270     >>  460 NOP
-                     
-                     271         462 PUSH_NULL
-                                 464 LOAD_DEREF              14 (fn)
-                                 466 LOAD_FAST                0 (args)
-                                 468 BUILD_MAP                0
-                                 470 LOAD_FAST                1 (kwargs)
-                                 472 DICT_MERGE               1
-                                 474 CALL_FUNCTION_EX         1
-                                 476 STORE_FAST              10 (res)
-                     
-                     273         478 LOAD_GLOBAL             17 (NULL + hasattr)
-                                 490 LOAD_FAST                9 (span_capture)
-                                 492 LOAD_CONST               6 ('capture_output')
-                                 494 PRECALL                  2
-                                 498 CALL                     2
-                                 508 POP_JUMP_FORWARD_IF_FALSE    41 (to 592)
-                                 510 LOAD_GLOBAL              9 (NULL + callable)
-                                 522 LOAD_FAST                9 (span_capture)
-                                 524 LOAD_ATTR               10 (capture_output)
-                                 534 PRECALL                  1
-                                 538 CALL                     1
-                                 548 POP_JUMP_FORWARD_IF_FALSE    21 (to 592)
-                     
-                     274         550 LOAD_FAST                9 (span_capture)
-                                 552 LOAD_METHOD             10 (capture_output)
-                                 574 LOAD_FAST               10 (res)
-                                 576 PRECALL                  1
-                                 580 CALL                     1
-                                 590 POP_TOP
-                     
-                     276     >>  592 LOAD_FAST                8 (span)
-                                 594 LOAD_METHOD             11 (is_recording)
-                                 616 PRECALL                  0
-                                 620 CALL                     0
-                                 630 POP_JUMP_FORWARD_IF_FALSE    51 (to 734)
-                     
-                     277         632 LOAD_FAST                8 (span)
-                                 634 LOAD_METHOD             12 (set_status)
-                                 656 LOAD_GLOBAL             26 (StatusCode)
-                                 668 LOAD_ATTR               14 (OK)
-                                 678 PRECALL                  1
-                                 682 CALL                     1
-                                 692 POP_TOP
-                     
-                     278         694 LOAD_FAST                8 (span)
-                                 696 LOAD_METHOD             15 (end)
-                                 718 PRECALL                  0
-                                 722 CALL                     0
+                     276     >>  238 LOAD_GLOBAL             13 (NULL + get_tracer)
+                                 250 LOAD_DEREF              12 (SpanCapture)
+                                 252 LOAD_METHOD              7 (is_flush_on_exit)
+                                 274 PRECALL                  0
+                                 278 CALL                     0
+                                 288 KW_NAMES                 3
+                                 290 PRECALL                  1
+                                 294 CALL                     1
+                                 304 BEFORE_WITH
+                                 306 STORE_FAST               7 (tracer)
+                     
+                     277         308 LOAD_FAST                7 (tracer)
+                                 310 LOAD_METHOD              8 (start_as_current_span)
+                                 332 LOAD_FAST                2 (span_name)
+                                 334 LOAD_DEREF              16 (span_kind)
+                                 336 LOAD_FAST                5 (context)
+                                 338 KW_NAMES                 4
+                                 340 PRECALL                  3
+                                 344 CALL                     3
+                                 354 BEFORE_WITH
+                                 356 STORE_FAST               8 (span)
+                     
+                     278         358 PUSH_NULL
+                                 360 LOAD_DEREF              12 (SpanCapture)
+                     
+                     279         362 LOAD_FAST                0 (args)
+                     
+                     280         364 LOAD_DEREF              15 (name)
+                     
+                     281         366 LOAD_FAST                3 (service_type)
+                     
+                     282         368 LOAD_FAST                8 (span)
+                     
+                     283         370 LOAD_DEREF              14 (fn)
+                     
+                     284         372 LOAD_DEREF              13 (config)
+                     
+                     285         374 LOAD_FAST                5 (context)
+                     
+                     278         376 LOAD_CONST               5 (('name', 'service_type', 'span', 'instance', 'config', 'context'))
+                                 378 BUILD_CONST_KEY_MAP      6
+                     
+                     286         380 LOAD_FAST                1 (kwargs)
+                     
+                     278         382 DICT_MERGE               1
+                                 384 CALL_FUNCTION_EX         1
+                                 386 STORE_FAST               9 (span_capture)
+                     
+                     288         388 LOAD_GLOBAL             19 (NULL + hasattr)
+                                 400 LOAD_FAST                9 (span_capture)
+                                 402 LOAD_CONST               6 ('capture_input')
+                                 404 PRECALL                  2
+                                 408 CALL                     2
+                                 418 POP_JUMP_FORWARD_IF_FALSE    40 (to 500)
+                                 420 LOAD_GLOBAL              9 (NULL + callable)
+                                 432 LOAD_FAST                9 (span_capture)
+                                 434 LOAD_ATTR               10 (capture_input)
+                                 444 PRECALL                  1
+                                 448 CALL                     1
+                                 458 POP_JUMP_FORWARD_IF_FALSE    20 (to 500)
+                     
+                     289         460 LOAD_FAST                9 (span_capture)
+                                 462 LOAD_METHOD             10 (capture_input)
+                                 484 PRECALL                  0
+                                 488 CALL                     0
+                                 498 POP_TOP
+                     
+                     291     >>  500 NOP
+                     
+                     292         502 PUSH_NULL
+                                 504 LOAD_DEREF              14 (fn)
+                                 506 LOAD_FAST                0 (args)
+                                 508 BUILD_MAP                0
+                                 510 LOAD_FAST                1 (kwargs)
+                                 512 DICT_MERGE               1
+                                 514 CALL_FUNCTION_EX         1
+                                 516 STORE_FAST              10 (res)
+                     
+                     294         518 LOAD_GLOBAL             19 (NULL + hasattr)
+                                 530 LOAD_FAST                9 (span_capture)
+                                 532 LOAD_CONST               7 ('capture_output')
+                                 534 PRECALL                  2
+                                 538 CALL                     2
+                                 548 POP_JUMP_FORWARD_IF_FALSE    41 (to 632)
+                                 550 LOAD_GLOBAL              9 (NULL + callable)
+                                 562 LOAD_FAST                9 (span_capture)
+                                 564 LOAD_ATTR               11 (capture_output)
+                                 574 PRECALL                  1
+                                 578 CALL                     1
+                                 588 POP_JUMP_FORWARD_IF_FALSE    21 (to 632)
+                     
+                     295         590 LOAD_FAST                9 (span_capture)
+                                 592 LOAD_METHOD             11 (capture_output)
+                                 614 LOAD_FAST               10 (res)
+                                 616 PRECALL                  1
+                                 620 CALL                     1
+                                 630 POP_TOP
+                     
+                     297     >>  632 LOAD_FAST                8 (span)
+                                 634 LOAD_METHOD             12 (is_recording)
+                                 656 PRECALL                  0
+                                 660 CALL                     0
+                                 670 POP_JUMP_FORWARD_IF_FALSE    51 (to 774)
+                     
+                     299         672 LOAD_FAST                8 (span)
+                                 674 LOAD_METHOD             13 (set_status)
+                                 696 LOAD_GLOBAL             28 (StatusCode)
+                                 708 LOAD_ATTR               15 (OK)
+                                 718 PRECALL                  1
+                                 722 CALL                     1
                                  732 POP_TOP
                      
-                     280     >>  734 LOAD_FAST               10 (res)
+                     300         734 LOAD_FAST                8 (span)
+                                 736 LOAD_METHOD             16 (end)
+                                 758 PRECALL                  0
+                                 762 CALL                     0
+                                 772 POP_TOP
                      
-                     256         736 SWAP                     2
-                                 738 LOAD_CONST               0 (None)
-                                 740 LOAD_CONST               0 (None)
-                                 742 LOAD_CONST               0 (None)
-                                 744 PRECALL                  2
-                                 748 CALL                     2
-                                 758 POP_TOP
-                     
-                     255         760 SWAP                     2
-                                 762 LOAD_CONST               0 (None)
-                                 764 LOAD_CONST               0 (None)
-                                 766 LOAD_CONST               0 (None)
-                                 768 PRECALL                  2
-                                 772 CALL                     2
-                                 782 POP_TOP
-                                 784 RETURN_VALUE
-                             >>  786 PUSH_EXC_INFO
-                     
-                     282         788 LOAD_GLOBAL             32 (Exception)
-                                 800 CHECK_EXC_MATCH
-                                 802 POP_JUMP_FORWARD_IF_FALSE    85 (to 974)
-                                 804 STORE_FAST              11 (err)
-                     
-                     284         806 LOAD_FAST                8 (span)
-                                 808 LOAD_METHOD             17 (record_exception)
-                                 830 LOAD_FAST               11 (err)
-                                 832 PRECALL                  1
-                                 836 CALL                     1
-                                 846 POP_TOP
-                     
-                     287         848 LOAD_FAST                8 (span)
-                                 850 LOAD_METHOD             12 (set_status)
-                                 872 LOAD_GLOBAL             37 (NULL + Status)
-                                 884 LOAD_GLOBAL             26 (StatusCode)
-                                 896 LOAD_ATTR               19 (ERROR)
-                                 906 LOAD_GLOBAL             41 (NULL + str)
-                                 918 LOAD_FAST               11 (err)
-                                 920 PRECALL                  1
-                                 924 CALL                     1
-                                 934 PRECALL                  2
-                                 938 CALL                     2
-                                 948 PRECALL                  1
-                                 952 CALL                     1
-                                 962 POP_TOP
-                     
-                     290         964 RAISE_VARARGS            0
-                             >>  966 LOAD_CONST               0 (None)
-                                 968 STORE_FAST              11 (err)
-                                 970 DELETE_FAST             11 (err)
-                                 972 RERAISE                  1
-                     
-                     282     >>  974 RERAISE                  0
-                             >>  976 COPY                     3
-                                 978 POP_EXCEPT
-                                 980 RERAISE                  1
-                     
-                     256     >>  982 PUSH_EXC_INFO
-                                 984 WITH_EXCEPT_START
-                                 986 POP_JUMP_FORWARD_IF_TRUE     4 (to 996)
-                                 988 RERAISE                  2
-                             >>  990 COPY                     3
-                                 992 POP_EXCEPT
-                                 994 RERAISE                  1
-                             >>  996 POP_TOP
-                                 998 POP_EXCEPT
-                                1000 POP_TOP
+                     302     >>  774 LOAD_FAST               10 (res)
+                     
+                     277         776 SWAP                     2
+                                 778 LOAD_CONST               0 (None)
+                                 780 LOAD_CONST               0 (None)
+                                 782 LOAD_CONST               0 (None)
+                                 784 PRECALL                  2
+                                 788 CALL                     2
+                                 798 POP_TOP
+                     
+                     276         800 SWAP                     2
+                                 802 LOAD_CONST               0 (None)
+                                 804 LOAD_CONST               0 (None)
+                                 806 LOAD_CONST               0 (None)
+                                 808 PRECALL                  2
+                                 812 CALL                     2
+                                 822 POP_TOP
+                                 824 RETURN_VALUE
+                             >>  826 PUSH_EXC_INFO
+                     
+                     304         828 LOAD_GLOBAL             34 (Exception)
+                                 840 CHECK_EXC_MATCH
+                                 842 POP_JUMP_FORWARD_IF_FALSE    85 (to 1014)
+                                 844 STORE_FAST              11 (err)
+                     
+                     306         846 LOAD_FAST                8 (span)
+                                 848 LOAD_METHOD             18 (record_exception)
+                                 870 LOAD_FAST               11 (err)
+                                 872 PRECALL                  1
+                                 876 CALL                     1
+                                 886 POP_TOP
+                     
+                     309         888 LOAD_FAST                8 (span)
+                                 890 LOAD_METHOD             13 (set_status)
+                                 912 LOAD_GLOBAL             39 (NULL + Status)
+                                 924 LOAD_GLOBAL             28 (StatusCode)
+                                 936 LOAD_ATTR               20 (ERROR)
+                                 946 LOAD_GLOBAL             43 (NULL + str)
+                                 958 LOAD_FAST               11 (err)
+                                 960 PRECALL                  1
+                                 964 CALL                     1
+                                 974 PRECALL                  2
+                                 978 CALL                     2
+                                 988 PRECALL                  1
+                                 992 CALL                     1
                                 1002 POP_TOP
-                                1004 NOP
                      
-                     255        1006 LOAD_CONST               0 (None)
-                                1008 LOAD_CONST               0 (None)
-                                1010 LOAD_CONST               0 (None)
-                                1012 PRECALL                  2
-                                1016 CALL                     2
-                                1026 POP_TOP
-                                1028 LOAD_CONST               0 (None)
-                                1030 RETURN_VALUE
-                             >> 1032 PUSH_EXC_INFO
-                                1034 WITH_EXCEPT_START
-                                1036 POP_JUMP_FORWARD_IF_TRUE     4 (to 1046)
-                                1038 RERAISE                  2
-                             >> 1040 COPY                     3
-                                1042 POP_EXCEPT
-                                1044 RERAISE                  1
-                             >> 1046 POP_TOP
-                                1048 POP_EXCEPT
-                                1050 POP_TOP
-                                1052 POP_TOP
-                                1054 LOAD_CONST               0 (None)
-                                1056 RETURN_VALUE
+                     312        1004 RAISE_VARARGS            0
+                             >> 1006 LOAD_CONST               0 (None)
+                                1008 STORE_FAST              11 (err)
+                                1010 DELETE_FAST             11 (err)
+                                1012 RERAISE                  1
+                     
+                     304     >> 1014 RERAISE                  0
+                             >> 1016 COPY                     3
+                                1018 POP_EXCEPT
+                                1020 RERAISE                  1
+                     
+                     277     >> 1022 PUSH_EXC_INFO
+                                1024 WITH_EXCEPT_START
+                                1026 POP_JUMP_FORWARD_IF_TRUE     4 (to 1036)
+                                1028 RERAISE                  2
+                             >> 1030 COPY                     3
+                                1032 POP_EXCEPT
+                                1034 RERAISE                  1
+                             >> 1036 POP_TOP
+                                1038 POP_EXCEPT
+                                1040 POP_TOP
+                                1042 POP_TOP
+                                1044 NOP
+                     
+                     276        1046 LOAD_CONST               0 (None)
+                                1048 LOAD_CONST               0 (None)
+                                1050 LOAD_CONST               0 (None)
+                                1052 PRECALL                  2
+                                1056 CALL                     2
+                                1066 POP_TOP
+                                1068 LOAD_CONST               0 (None)
+                                1070 RETURN_VALUE
+                             >> 1072 PUSH_EXC_INFO
+                                1074 WITH_EXCEPT_START
+                                1076 POP_JUMP_FORWARD_IF_TRUE     4 (to 1086)
+                                1078 RERAISE                  2
+                             >> 1080 COPY                     3
+                                1082 POP_EXCEPT
+                                1084 RERAISE                  1
+                             >> 1086 POP_TOP
+                                1088 POP_EXCEPT
+                                1090 POP_TOP
+                                1092 POP_TOP
+                                1094 LOAD_CONST               0 (None)
+                                1096 RETURN_VALUE
                      ExceptionTable:
-                       266 to 314 -> 1032 [1] lasti
-                       316 to 458 -> 982 [2] lasti
-                       462 to 734 -> 786 [2]
-                       736 to 758 -> 1032 [1] lasti
-                       786 to 804 -> 976 [3] lasti
-                       806 to 964 -> 966 [3] lasti
-                       966 to 974 -> 976 [3] lasti
-                       976 to 980 -> 982 [2] lasti
-                       982 to 988 -> 990 [4] lasti
-                       990 to 994 -> 1032 [1] lasti
-                       996 to 996 -> 990 [4] lasti
-                       998 to 1002 -> 1032 [1] lasti
-                       1032 to 1038 -> 1040 [3] lasti
-                       1046 to 1046 -> 1040 [3] lasti
+                       306 to 354 -> 1072 [1] lasti
+                       356 to 498 -> 1022 [2] lasti
+                       502 to 774 -> 826 [2]
+                       776 to 798 -> 1072 [1] lasti
+                       826 to 844 -> 1016 [3] lasti
+                       846 to 1004 -> 1006 [3] lasti
+                       1006 to 1014 -> 1016 [3] lasti
+                       1016 to 1020 -> 1022 [2] lasti
+                       1022 to 1028 -> 1030 [4] lasti
+                       1030 to 1034 -> 1072 [1] lasti
+                       1036 to 1036 -> 1030 [4] lasti
+                       1038 to 1042 -> 1072 [1] lasti
+                       1072 to 1078 -> 1080 [3] lasti
+                       1086 to 1086 -> 1080 [3] lasti
                      consts
                         None
                         ('name', 'tlp_service_type', 'instance')
                         'context_parser'
+                        ('flush_on_exit',)
                         ('kind', 'context')
                         ('name', 'service_type', 'span', 'instance', 'config', 'context')
                         'capture_input'
                         'capture_output'
-                     names      ('TracerWrapper', 'verify_initialized', 'get_span_name', 'get', 'callable', 'get_trace_context_from_carrier', 'get_tracer', 'start_as_current_span', 'hasattr', 'capture_input', 'capture_output', 'is_recording', 'set_status', 'StatusCode', 'OK', 'end', 'Exception', 'record_exception', 'Status', 'ERROR', 'str')
+                     names      ('TracerWrapper', 'verify_initialized', 'get_span_name', 'get', 'callable', 'get_trace_context_from_carrier', 'get_tracer', 'is_flush_on_exit', 'start_as_current_span', 'hasattr', 'capture_input', 'capture_output', 'is_recording', 'set_status', 'StatusCode', 'OK', 'end', 'Exception', 'record_exception', 'Status', 'ERROR', 'str')
                      varnames   ('args', 'kwargs', 'span_name', 'service_type', 'context_parser', 'context', 'carrier', 'tracer', 'span', 'span_capture', 'res', 'err')
                      freevars   ('SpanCapture', 'config', 'fn', 'name', 'span_kind', 'tlp_service_type')
                      cellvars   ()
                      filename   '/Users/vuongngo/workspace/agiflow/packages/python/agiflow-sdk/agiflow/opentelemetry/trace_decorators/wrapper.py'
                      name       'wrap'
-                     firstlineno 238
+                     firstlineno 259
                      lnotab
-                        0x04022601100218010201020102fd18062a010401220110011e021e0132
+                        0x04022601100218010201020102fd18062a010401220110011e02460132
                         01040102010201020102010201020102f9040802f8060a48012802020110
-                        0248012a0228013e01280202e818ff1c1b12022a0374030af808e618ff
+                        0248012a0228023e01280202e718ff1c1c12022a0374030af808e518ff
                names      ('wraps',)
                varnames   ('fn', 'wrap')
                freevars   ('SpanCapture', 'config', 'name', 'span_kind', 'tlp_service_type')
                cellvars   ('fn',)
                filename   '/Users/vuongngo/workspace/agiflow/packages/python/agiflow-sdk/agiflow/opentelemetry/trace_decorators/wrapper.py'
                name       'decorate'
-               firstlineno 237
-               lnotab 0x06011c0112ff0e010235
+               firstlineno 258
+               lnotab 0x06011c0112ff0e010236
          names      ()
          varnames   ('name', 'tlp_service_type', 'span_kind', 'SpanCapture', 'config', 'decorate')
          freevars   ()
          cellvars   ('name', 'tlp_service_type', 'span_kind', 'SpanCapture', 'config')
          filename   '/Users/vuongngo/workspace/agiflow/packages/python/agiflow-sdk/agiflow/opentelemetry/trace_decorators/wrapper.py'
          name       'decorate_method'
-         firstlineno 230
-         lnotab 0x0c071239
+         firstlineno 251
+         lnotab 0x0c07123a
       code
          argcount  : 4
          nlocals   : 6
          stacksize : 5
          flags     : 11
          code
             0x870087018702870387049700880388048800880288016605640184087d
             057c055300
                        0 MAKE_CELL                0 (name)
                        2 MAKE_CELL                1 (tlp_service_type)
                        4 MAKE_CELL                2 (span_kind)
                        6 MAKE_CELL                3 (SpanCapture)
                        8 MAKE_CELL                4 (config)
          
-         297          10 RESUME                   0
+         319          10 RESUME                   0
          
-         304          12 LOAD_CLOSURE             3 (SpanCapture)
+         326          12 LOAD_CLOSURE             3 (SpanCapture)
                       14 LOAD_CLOSURE             4 (config)
                       16 LOAD_CLOSURE             0 (name)
                       18 LOAD_CLOSURE             2 (span_kind)
                       20 LOAD_CLOSURE             1 (tlp_service_type)
                       22 BUILD_TUPLE              5
-                      24 LOAD_CONST               1 (<code object decorate, file "/Users/vuongngo/workspace/agiflow/packages/python/agiflow-sdk/agiflow/opentelemetry/trace_decorators/wrapper.py", line 304>)
+                      24 LOAD_CONST               1 (<code object decorate, file "/Users/vuongngo/workspace/agiflow/packages/python/agiflow-sdk/agiflow/opentelemetry/trace_decorators/wrapper.py", line 326>)
                       26 MAKE_FUNCTION            8 (closure)
                       28 STORE_FAST               5 (decorate)
          
-         362          30 LOAD_FAST                5 (decorate)
+         384          30 LOAD_FAST                5 (decorate)
                       32 RETURN_VALUE
          consts
             None
             code
                argcount  : 1
                nlocals   : 2
                stacksize : 7
@@ -1988,37 +2107,37 @@
                code
                   0x9505870097007401000000000000000000008900a6010000ab01000000
                   0000000000880288038800880488058806660664018408a6000000ab0000
                   000000000000007d017c015300
                              0 COPY_FREE_VARS           5
                              2 MAKE_CELL                0 (fn)
                
-               304           4 RESUME                   0
+               326           4 RESUME                   0
                
-               305           6 LOAD_GLOBAL              1 (NULL + wraps)
+               327           6 LOAD_GLOBAL              1 (NULL + wraps)
                             18 LOAD_DEREF               0 (fn)
                             20 PRECALL                  1
                             24 CALL                     1
                
-               306          34 LOAD_CLOSURE             2 (SpanCapture)
+               328          34 LOAD_CLOSURE             2 (SpanCapture)
                             36 LOAD_CLOSURE             3 (config)
                             38 LOAD_CLOSURE             0 (fn)
                             40 LOAD_CLOSURE             4 (name)
                             42 LOAD_CLOSURE             5 (span_kind)
                             44 LOAD_CLOSURE             6 (tlp_service_type)
                             46 BUILD_TUPLE              6
-                            48 LOAD_CONST               1 (<code object wrap, file "/Users/vuongngo/workspace/agiflow/packages/python/agiflow-sdk/agiflow/opentelemetry/trace_decorators/wrapper.py", line 305>)
+                            48 LOAD_CONST               1 (<code object wrap, file "/Users/vuongngo/workspace/agiflow/packages/python/agiflow-sdk/agiflow/opentelemetry/trace_decorators/wrapper.py", line 327>)
                             50 MAKE_FUNCTION            8 (closure)
                
-               305          52 PRECALL                  0
+               327          52 PRECALL                  0
                             56 CALL                     0
                
-               306          66 STORE_FAST               1 (wrap)
+               328          66 STORE_FAST               1 (wrap)
                
-               360          68 LOAD_FAST                1 (wrap)
+               382          68 LOAD_FAST                1 (wrap)
                             70 RETURN_VALUE
                consts
                   None
                   code
                      argcount  : 0
                      nlocals   : 12
                      stacksize : 12
@@ -2028,381 +2147,388 @@
                         00a6000000ab00000000000000000073080200890e7c0069007c01a4018e
                         015300890ca0020000000000000000000000000000000000000000890f89
                         11890eac01a6030000ab0300000000000000005c0200007d027d03890da0
                         0300000000000000000000000000000000000000006402a6010000ab0100
                         000000000000007d0464007d057c0481267409000000000000000000007c
                         04a6010000ab010000000000000000721702007c047c0069007c01a4018e
                         017d06740b000000000000000000007c06a6010000ab0100000000000000
-                        007d05740d00000000000000000000a6000000ab00000000000000000035
-                        007d077c07a00700000000000000000000000000000000000000007c0289
-                        107c05ac03a6030000ab03000000000000000035007d080200890c7c0089
-                        0f7c037c08890e890d7c0564049c067c01a4018e017d0974110000000000
-                        00000000007c096405a6020000ab02000000000000000072287409000000
-                        000000000000007c096a090000000000000000a6010000ab010000000000
-                        00000072147c09a0090000000000000000000000000000000000000000a6
-                        000000ab000000000000000000010009000200890e7c0069007c01a4018e
-                        01830064007b035600970386047d0a7411000000000000000000007c0964
-                        06a6020000ab02000000000000000072297409000000000000000000007c
-                        096a0a0000000000000000a6010000ab01000000000000000072157c09a0
-                        0a00000000000000000000000000000000000000007c0aa6010000ab0100
-                        0000000000000001007c08a00b0000000000000000000000000000000000
-                        000000a6000000ab00000000000000000072337c08a00c00000000000000
-                        00000000000000000000000000741a000000000000000000006a0e000000
-                        0000000000a6010000ab01000000000000000001007c08a00f0000000000
-                        000000000000000000000000000000a6000000ab00000000000000000001
-                        007c0a6302640064006400a6020000ab0200000000000000000100630264
-                        0064006400a6020000ab0200000000000000000100530023007420000000
-                        00000000000000240072697d0b7c08a01100000000000000000000000000
-                        000000000000007c0ba6010000ab01000000000000000001007c08a00c00
-                        000000000000000000000000000000000000007425000000000000000000
-                        00741a000000000000000000006a13000000000000000074290000000000
-                        00000000007c0ba6010000ab010000000000000000a6020000ab02000000
-                        0000000000a6010000ab01000000000000000001007c08a00f0000000000
-                        000000000000000000000000000000a6000000ab00000000000000000001
-                        00820064007d0b7e0b770177007803590077012300310073047702780359
-                        00770101005900010001000900640064006400a6020000ab020000000000
-                        000000010064005300230031007304770278035900770101005900010001
-                        0064005300
+                        007d05740d00000000000000000000890ca0070000000000000000000000
+                        000000000000000000a6000000ab000000000000000000ac03a6010000ab
+                        01000000000000000035007d077c07a00800000000000000000000000000
+                        000000000000007c0289107c05ac04a6030000ab03000000000000000035
+                        007d080200890c7c00890f7c037c08890e890d7c0564059c067c01a4018e
+                        017d097413000000000000000000007c096406a6020000ab020000000000
+                        00000072287409000000000000000000007c096a0a0000000000000000a6
+                        010000ab01000000000000000072147c09a00a0000000000000000000000
+                        000000000000000000a6000000ab00000000000000000001000900020089
+                        0e7c0069007c01a4018e01830064007b035600970386047d0a7413000000
+                        000000000000007c096407a6020000ab0200000000000000007229740900
+                        0000000000000000007c096a0b0000000000000000a6010000ab01000000
+                        000000000072157c09a00b00000000000000000000000000000000000000
+                        007c0aa6010000ab01000000000000000001007c08a00c00000000000000
+                        00000000000000000000000000a6000000ab00000000000000000072337c
+                        08a00d0000000000000000000000000000000000000000741c0000000000
+                        00000000006a0f0000000000000000a6010000ab01000000000000000001
+                        007c08a0100000000000000000000000000000000000000000a6000000ab
+                        00000000000000000001007c0a6302640064006400a6020000ab02000000
+                        000000000001006302640064006400a6020000ab02000000000000000001
+                        0053002300742200000000000000000000240072697d0b7c08a012000000
+                        00000000000000000000000000000000007c0ba6010000ab010000000000
+                        00000001007c08a00d000000000000000000000000000000000000000074
+                        2700000000000000000000741c000000000000000000006a140000000000
+                        000000742b000000000000000000007c0ba6010000ab0100000000000000
+                        00a6020000ab020000000000000000a6010000ab01000000000000000001
+                        007c08a0100000000000000000000000000000000000000000a6000000ab
+                        0000000000000000000100820064007d0b7e0b7701770078035900770123
+                        0031007304770278035900770101005900010001000900640064006400a6
+                        020000ab0200000000000000000100640053002300310073047702780359
+                        007701010059000100010064005300
                                    0 COPY_FREE_VARS           6
                      
-                     305           2 RETURN_GENERATOR
+                     327           2 RETURN_GENERATOR
                                    4 POP_TOP
                                    6 RESUME                   0
                      
-                     307           8 LOAD_GLOBAL              1 (NULL + TracerWrapper)
+                     329           8 LOAD_GLOBAL              1 (NULL + TracerWrapper)
                                   20 LOAD_ATTR                1 (verify_initialized)
                                   30 PRECALL                  0
                                   34 CALL                     0
                                   44 POP_JUMP_FORWARD_IF_TRUE     8 (to 62)
                      
-                     308          46 PUSH_NULL
+                     330          46 PUSH_NULL
                                   48 LOAD_DEREF              14 (fn)
                                   50 LOAD_FAST                0 (args)
                                   52 BUILD_MAP                0
                                   54 LOAD_FAST                1 (kwargs)
                                   56 DICT_MERGE               1
                                   58 CALL_FUNCTION_EX         1
                                   60 RETURN_VALUE
                      
-                     310     >>   62 LOAD_DEREF              12 (SpanCapture)
+                     332     >>   62 LOAD_DEREF              12 (SpanCapture)
                                   64 LOAD_METHOD              2 (get_span_name)
                      
-                     311          86 LOAD_DEREF              15 (name)
+                     333          86 LOAD_DEREF              15 (name)
                      
-                     312          88 LOAD_DEREF              17 (tlp_service_type)
+                     334          88 LOAD_DEREF              17 (tlp_service_type)
                      
-                     313          90 LOAD_DEREF              14 (fn)
+                     335          90 LOAD_DEREF              14 (fn)
                      
-                     310          92 KW_NAMES                 1
+                     332          92 KW_NAMES                 1
                                   94 PRECALL                  3
                                   98 CALL                     3
                                  108 UNPACK_SEQUENCE          2
                                  112 STORE_FAST               2 (span_name)
                                  114 STORE_FAST               3 (service_type)
                      
-                     316         116 LOAD_DEREF              13 (config)
+                     338         116 LOAD_DEREF              13 (config)
                                  118 LOAD_METHOD              3 (get)
                                  140 LOAD_CONST               2 ('context_parser')
                                  142 PRECALL                  1
                                  146 CALL                     1
                                  156 STORE_FAST               4 (context_parser)
                      
-                     317         158 LOAD_CONST               0 (None)
+                     339         158 LOAD_CONST               0 (None)
                                  160 STORE_FAST               5 (context)
                      
-                     318         162 LOAD_FAST                4 (context_parser)
+                     340         162 LOAD_FAST                4 (context_parser)
                                  164 POP_JUMP_FORWARD_IF_NONE    38 (to 242)
                                  166 LOAD_GLOBAL              9 (NULL + callable)
                                  178 LOAD_FAST                4 (context_parser)
                                  180 PRECALL                  1
                                  184 CALL                     1
                                  194 POP_JUMP_FORWARD_IF_FALSE    23 (to 242)
                      
-                     319         196 PUSH_NULL
+                     341         196 PUSH_NULL
                                  198 LOAD_FAST                4 (context_parser)
                                  200 LOAD_FAST                0 (args)
                                  202 BUILD_MAP                0
                                  204 LOAD_FAST                1 (kwargs)
                                  206 DICT_MERGE               1
                                  208 CALL_FUNCTION_EX         1
                                  210 STORE_FAST               6 (carrier)
                      
-                     320         212 LOAD_GLOBAL             11 (NULL + get_trace_context_from_carrier)
+                     342         212 LOAD_GLOBAL             11 (NULL + get_trace_context_from_carrier)
                                  224 LOAD_FAST                6 (carrier)
                                  226 PRECALL                  1
                                  230 CALL                     1
                                  240 STORE_FAST               5 (context)
                      
-                     322     >>  242 LOAD_GLOBAL             13 (NULL + get_tracer)
-                                 254 PRECALL                  0
-                                 258 CALL                     0
-                                 268 BEFORE_WITH
-                                 270 STORE_FAST               7 (tracer)
-                     
-                     323         272 LOAD_FAST                7 (tracer)
-                                 274 LOAD_METHOD              7 (start_as_current_span)
-                                 296 LOAD_FAST                2 (span_name)
-                                 298 LOAD_DEREF              16 (span_kind)
-                                 300 LOAD_FAST                5 (context)
-                                 302 KW_NAMES                 3
-                                 304 PRECALL                  3
-                                 308 CALL                     3
-                                 318 BEFORE_WITH
-                                 320 STORE_FAST               8 (span)
-                     
-                     324         322 PUSH_NULL
-                                 324 LOAD_DEREF              12 (SpanCapture)
-                     
-                     325         326 LOAD_FAST                0 (args)
-                     
-                     326         328 LOAD_DEREF              15 (name)
-                     
-                     327         330 LOAD_FAST                3 (service_type)
-                     
-                     328         332 LOAD_FAST                8 (span)
-                     
-                     329         334 LOAD_DEREF              14 (fn)
-                     
-                     330         336 LOAD_DEREF              13 (config)
-                     
-                     331         338 LOAD_FAST                5 (context)
-                     
-                     324         340 LOAD_CONST               4 (('name', 'service_type', 'span', 'instance', 'config', 'context'))
-                                 342 BUILD_CONST_KEY_MAP      6
-                     
-                     332         344 LOAD_FAST                1 (kwargs)
-                     
-                     324         346 DICT_MERGE               1
-                                 348 CALL_FUNCTION_EX         1
-                                 350 STORE_FAST               9 (span_capture)
-                     
-                     334         352 LOAD_GLOBAL             17 (NULL + hasattr)
-                                 364 LOAD_FAST                9 (span_capture)
-                                 366 LOAD_CONST               5 ('capture_input')
-                                 368 PRECALL                  2
-                                 372 CALL                     2
-                                 382 POP_JUMP_FORWARD_IF_FALSE    40 (to 464)
-                                 384 LOAD_GLOBAL              9 (NULL + callable)
-                                 396 LOAD_FAST                9 (span_capture)
-                                 398 LOAD_ATTR                9 (capture_input)
-                                 408 PRECALL                  1
-                                 412 CALL                     1
-                                 422 POP_JUMP_FORWARD_IF_FALSE    20 (to 464)
-                     
-                     335         424 LOAD_FAST                9 (span_capture)
-                                 426 LOAD_METHOD              9 (capture_input)
-                                 448 PRECALL                  0
-                                 452 CALL                     0
-                                 462 POP_TOP
-                     
-                     337     >>  464 NOP
-                     
-                     338         466 PUSH_NULL
-                                 468 LOAD_DEREF              14 (fn)
-                                 470 LOAD_FAST                0 (args)
-                                 472 BUILD_MAP                0
-                                 474 LOAD_FAST                1 (kwargs)
-                                 476 DICT_MERGE               1
-                                 478 CALL_FUNCTION_EX         1
-                                 480 GET_AWAITABLE            0
-                                 482 LOAD_CONST               0 (None)
-                             >>  484 SEND                     3 (to 492)
-                                 486 YIELD_VALUE
-                                 488 RESUME                   3
-                                 490 JUMP_BACKWARD_NO_INTERRUPT     4 (to 484)
-                             >>  492 STORE_FAST              10 (res)
-                     
-                     340         494 LOAD_GLOBAL             17 (NULL + hasattr)
-                                 506 LOAD_FAST                9 (span_capture)
-                                 508 LOAD_CONST               6 ('capture_output')
-                                 510 PRECALL                  2
-                                 514 CALL                     2
-                                 524 POP_JUMP_FORWARD_IF_FALSE    41 (to 608)
-                                 526 LOAD_GLOBAL              9 (NULL + callable)
-                                 538 LOAD_FAST                9 (span_capture)
-                                 540 LOAD_ATTR               10 (capture_output)
-                                 550 PRECALL                  1
-                                 554 CALL                     1
-                                 564 POP_JUMP_FORWARD_IF_FALSE    21 (to 608)
-                     
-                     341         566 LOAD_FAST                9 (span_capture)
-                                 568 LOAD_METHOD             10 (capture_output)
-                                 590 LOAD_FAST               10 (res)
-                                 592 PRECALL                  1
-                                 596 CALL                     1
-                                 606 POP_TOP
-                     
-                     343     >>  608 LOAD_FAST                8 (span)
-                                 610 LOAD_METHOD             11 (is_recording)
-                                 632 PRECALL                  0
-                                 636 CALL                     0
-                                 646 POP_JUMP_FORWARD_IF_FALSE    51 (to 750)
-                     
-                     344         648 LOAD_FAST                8 (span)
-                                 650 LOAD_METHOD             12 (set_status)
-                                 672 LOAD_GLOBAL             26 (StatusCode)
-                                 684 LOAD_ATTR               14 (OK)
-                                 694 PRECALL                  1
-                                 698 CALL                     1
-                                 708 POP_TOP
-                     
-                     345         710 LOAD_FAST                8 (span)
-                                 712 LOAD_METHOD             15 (end)
-                                 734 PRECALL                  0
-                                 738 CALL                     0
+                     344     >>  242 LOAD_GLOBAL             13 (NULL + get_tracer)
+                                 254 LOAD_DEREF              12 (SpanCapture)
+                                 256 LOAD_METHOD              7 (is_flush_on_exit)
+                                 278 PRECALL                  0
+                                 282 CALL                     0
+                                 292 KW_NAMES                 3
+                                 294 PRECALL                  1
+                                 298 CALL                     1
+                                 308 BEFORE_WITH
+                                 310 STORE_FAST               7 (tracer)
+                     
+                     345         312 LOAD_FAST                7 (tracer)
+                                 314 LOAD_METHOD              8 (start_as_current_span)
+                                 336 LOAD_FAST                2 (span_name)
+                                 338 LOAD_DEREF              16 (span_kind)
+                                 340 LOAD_FAST                5 (context)
+                                 342 KW_NAMES                 4
+                                 344 PRECALL                  3
+                                 348 CALL                     3
+                                 358 BEFORE_WITH
+                                 360 STORE_FAST               8 (span)
+                     
+                     346         362 PUSH_NULL
+                                 364 LOAD_DEREF              12 (SpanCapture)
+                     
+                     347         366 LOAD_FAST                0 (args)
+                     
+                     348         368 LOAD_DEREF              15 (name)
+                     
+                     349         370 LOAD_FAST                3 (service_type)
+                     
+                     350         372 LOAD_FAST                8 (span)
+                     
+                     351         374 LOAD_DEREF              14 (fn)
+                     
+                     352         376 LOAD_DEREF              13 (config)
+                     
+                     353         378 LOAD_FAST                5 (context)
+                     
+                     346         380 LOAD_CONST               5 (('name', 'service_type', 'span', 'instance', 'config', 'context'))
+                                 382 BUILD_CONST_KEY_MAP      6
+                     
+                     354         384 LOAD_FAST                1 (kwargs)
+                     
+                     346         386 DICT_MERGE               1
+                                 388 CALL_FUNCTION_EX         1
+                                 390 STORE_FAST               9 (span_capture)
+                     
+                     356         392 LOAD_GLOBAL             19 (NULL + hasattr)
+                                 404 LOAD_FAST                9 (span_capture)
+                                 406 LOAD_CONST               6 ('capture_input')
+                                 408 PRECALL                  2
+                                 412 CALL                     2
+                                 422 POP_JUMP_FORWARD_IF_FALSE    40 (to 504)
+                                 424 LOAD_GLOBAL              9 (NULL + callable)
+                                 436 LOAD_FAST                9 (span_capture)
+                                 438 LOAD_ATTR               10 (capture_input)
+                                 448 PRECALL                  1
+                                 452 CALL                     1
+                                 462 POP_JUMP_FORWARD_IF_FALSE    20 (to 504)
+                     
+                     357         464 LOAD_FAST                9 (span_capture)
+                                 466 LOAD_METHOD             10 (capture_input)
+                                 488 PRECALL                  0
+                                 492 CALL                     0
+                                 502 POP_TOP
+                     
+                     359     >>  504 NOP
+                     
+                     360         506 PUSH_NULL
+                                 508 LOAD_DEREF              14 (fn)
+                                 510 LOAD_FAST                0 (args)
+                                 512 BUILD_MAP                0
+                                 514 LOAD_FAST                1 (kwargs)
+                                 516 DICT_MERGE               1
+                                 518 CALL_FUNCTION_EX         1
+                                 520 GET_AWAITABLE            0
+                                 522 LOAD_CONST               0 (None)
+                             >>  524 SEND                     3 (to 532)
+                                 526 YIELD_VALUE
+                                 528 RESUME                   3
+                                 530 JUMP_BACKWARD_NO_INTERRUPT     4 (to 524)
+                             >>  532 STORE_FAST              10 (res)
+                     
+                     362         534 LOAD_GLOBAL             19 (NULL + hasattr)
+                                 546 LOAD_FAST                9 (span_capture)
+                                 548 LOAD_CONST               7 ('capture_output')
+                                 550 PRECALL                  2
+                                 554 CALL                     2
+                                 564 POP_JUMP_FORWARD_IF_FALSE    41 (to 648)
+                                 566 LOAD_GLOBAL              9 (NULL + callable)
+                                 578 LOAD_FAST                9 (span_capture)
+                                 580 LOAD_ATTR               11 (capture_output)
+                                 590 PRECALL                  1
+                                 594 CALL                     1
+                                 604 POP_JUMP_FORWARD_IF_FALSE    21 (to 648)
+                     
+                     363         606 LOAD_FAST                9 (span_capture)
+                                 608 LOAD_METHOD             11 (capture_output)
+                                 630 LOAD_FAST               10 (res)
+                                 632 PRECALL                  1
+                                 636 CALL                     1
+                                 646 POP_TOP
+                     
+                     365     >>  648 LOAD_FAST                8 (span)
+                                 650 LOAD_METHOD             12 (is_recording)
+                                 672 PRECALL                  0
+                                 676 CALL                     0
+                                 686 POP_JUMP_FORWARD_IF_FALSE    51 (to 790)
+                     
+                     366         688 LOAD_FAST                8 (span)
+                                 690 LOAD_METHOD             13 (set_status)
+                                 712 LOAD_GLOBAL             28 (StatusCode)
+                                 724 LOAD_ATTR               15 (OK)
+                                 734 PRECALL                  1
+                                 738 CALL                     1
                                  748 POP_TOP
                      
-                     347     >>  750 LOAD_FAST               10 (res)
-                     
-                     323         752 SWAP                     2
-                                 754 LOAD_CONST               0 (None)
-                                 756 LOAD_CONST               0 (None)
-                                 758 LOAD_CONST               0 (None)
-                                 760 PRECALL                  2
-                                 764 CALL                     2
-                                 774 POP_TOP
-                     
-                     322         776 SWAP                     2
-                                 778 LOAD_CONST               0 (None)
-                                 780 LOAD_CONST               0 (None)
-                                 782 LOAD_CONST               0 (None)
-                                 784 PRECALL                  2
-                                 788 CALL                     2
-                                 798 POP_TOP
-                                 800 RETURN_VALUE
-                             >>  802 PUSH_EXC_INFO
-                     
-                     349         804 LOAD_GLOBAL             32 (Exception)
-                                 816 CHECK_EXC_MATCH
-                                 818 POP_JUMP_FORWARD_IF_FALSE   105 (to 1030)
-                                 820 STORE_FAST              11 (err)
-                     
-                     351         822 LOAD_FAST                8 (span)
-                                 824 LOAD_METHOD             17 (record_exception)
-                                 846 LOAD_FAST               11 (err)
-                                 848 PRECALL                  1
-                                 852 CALL                     1
-                                 862 POP_TOP
-                     
-                     354         864 LOAD_FAST                8 (span)
-                                 866 LOAD_METHOD             12 (set_status)
-                                 888 LOAD_GLOBAL             37 (NULL + Status)
-                                 900 LOAD_GLOBAL             26 (StatusCode)
-                                 912 LOAD_ATTR               19 (ERROR)
-                                 922 LOAD_GLOBAL             41 (NULL + str)
-                                 934 LOAD_FAST               11 (err)
-                                 936 PRECALL                  1
-                                 940 CALL                     1
-                                 950 PRECALL                  2
-                                 954 CALL                     2
-                                 964 PRECALL                  1
-                                 968 CALL                     1
-                                 978 POP_TOP
-                     
-                     357         980 LOAD_FAST                8 (span)
-                                 982 LOAD_METHOD             15 (end)
-                                1004 PRECALL                  0
-                                1008 CALL                     0
+                     367         750 LOAD_FAST                8 (span)
+                                 752 LOAD_METHOD             16 (end)
+                                 774 PRECALL                  0
+                                 778 CALL                     0
+                                 788 POP_TOP
+                     
+                     369     >>  790 LOAD_FAST               10 (res)
+                     
+                     345         792 SWAP                     2
+                                 794 LOAD_CONST               0 (None)
+                                 796 LOAD_CONST               0 (None)
+                                 798 LOAD_CONST               0 (None)
+                                 800 PRECALL                  2
+                                 804 CALL                     2
+                                 814 POP_TOP
+                     
+                     344         816 SWAP                     2
+                                 818 LOAD_CONST               0 (None)
+                                 820 LOAD_CONST               0 (None)
+                                 822 LOAD_CONST               0 (None)
+                                 824 PRECALL                  2
+                                 828 CALL                     2
+                                 838 POP_TOP
+                                 840 RETURN_VALUE
+                             >>  842 PUSH_EXC_INFO
+                     
+                     371         844 LOAD_GLOBAL             34 (Exception)
+                                 856 CHECK_EXC_MATCH
+                                 858 POP_JUMP_FORWARD_IF_FALSE   105 (to 1070)
+                                 860 STORE_FAST              11 (err)
+                     
+                     373         862 LOAD_FAST                8 (span)
+                                 864 LOAD_METHOD             18 (record_exception)
+                                 886 LOAD_FAST               11 (err)
+                                 888 PRECALL                  1
+                                 892 CALL                     1
+                                 902 POP_TOP
+                     
+                     376         904 LOAD_FAST                8 (span)
+                                 906 LOAD_METHOD             13 (set_status)
+                                 928 LOAD_GLOBAL             39 (NULL + Status)
+                                 940 LOAD_GLOBAL             28 (StatusCode)
+                                 952 LOAD_ATTR               20 (ERROR)
+                                 962 LOAD_GLOBAL             43 (NULL + str)
+                                 974 LOAD_FAST               11 (err)
+                                 976 PRECALL                  1
+                                 980 CALL                     1
+                                 990 PRECALL                  2
+                                 994 CALL                     2
+                                1004 PRECALL                  1
+                                1008 CALL                     1
                                 1018 POP_TOP
                      
-                     358        1020 RAISE_VARARGS            0
-                             >> 1022 LOAD_CONST               0 (None)
-                                1024 STORE_FAST              11 (err)
-                                1026 DELETE_FAST             11 (err)
-                                1028 RERAISE                  1
-                     
-                     349     >> 1030 RERAISE                  0
-                             >> 1032 COPY                     3
-                                1034 POP_EXCEPT
-                                1036 RERAISE                  1
-                     
-                     323     >> 1038 PUSH_EXC_INFO
-                                1040 WITH_EXCEPT_START
-                                1042 POP_JUMP_FORWARD_IF_TRUE     4 (to 1052)
-                                1044 RERAISE                  2
-                             >> 1046 COPY                     3
-                                1048 POP_EXCEPT
-                                1050 RERAISE                  1
-                             >> 1052 POP_TOP
-                                1054 POP_EXCEPT
-                                1056 POP_TOP
+                     379        1020 LOAD_FAST                8 (span)
+                                1022 LOAD_METHOD             16 (end)
+                                1044 PRECALL                  0
+                                1048 CALL                     0
                                 1058 POP_TOP
-                                1060 NOP
                      
-                     322        1062 LOAD_CONST               0 (None)
-                                1064 LOAD_CONST               0 (None)
-                                1066 LOAD_CONST               0 (None)
-                                1068 PRECALL                  2
-                                1072 CALL                     2
-                                1082 POP_TOP
-                                1084 LOAD_CONST               0 (None)
-                                1086 RETURN_VALUE
-                             >> 1088 PUSH_EXC_INFO
-                                1090 WITH_EXCEPT_START
-                                1092 POP_JUMP_FORWARD_IF_TRUE     4 (to 1102)
-                                1094 RERAISE                  2
-                             >> 1096 COPY                     3
-                                1098 POP_EXCEPT
-                                1100 RERAISE                  1
-                             >> 1102 POP_TOP
-                                1104 POP_EXCEPT
-                                1106 POP_TOP
-                                1108 POP_TOP
-                                1110 LOAD_CONST               0 (None)
-                                1112 RETURN_VALUE
+                     380        1060 RAISE_VARARGS            0
+                             >> 1062 LOAD_CONST               0 (None)
+                                1064 STORE_FAST              11 (err)
+                                1066 DELETE_FAST             11 (err)
+                                1068 RERAISE                  1
+                     
+                     371     >> 1070 RERAISE                  0
+                             >> 1072 COPY                     3
+                                1074 POP_EXCEPT
+                                1076 RERAISE                  1
+                     
+                     345     >> 1078 PUSH_EXC_INFO
+                                1080 WITH_EXCEPT_START
+                                1082 POP_JUMP_FORWARD_IF_TRUE     4 (to 1092)
+                                1084 RERAISE                  2
+                             >> 1086 COPY                     3
+                                1088 POP_EXCEPT
+                                1090 RERAISE                  1
+                             >> 1092 POP_TOP
+                                1094 POP_EXCEPT
+                                1096 POP_TOP
+                                1098 POP_TOP
+                                1100 NOP
+                     
+                     344        1102 LOAD_CONST               0 (None)
+                                1104 LOAD_CONST               0 (None)
+                                1106 LOAD_CONST               0 (None)
+                                1108 PRECALL                  2
+                                1112 CALL                     2
+                                1122 POP_TOP
+                                1124 LOAD_CONST               0 (None)
+                                1126 RETURN_VALUE
+                             >> 1128 PUSH_EXC_INFO
+                                1130 WITH_EXCEPT_START
+                                1132 POP_JUMP_FORWARD_IF_TRUE     4 (to 1142)
+                                1134 RERAISE                  2
+                             >> 1136 COPY                     3
+                                1138 POP_EXCEPT
+                                1140 RERAISE                  1
+                             >> 1142 POP_TOP
+                                1144 POP_EXCEPT
+                                1146 POP_TOP
+                                1148 POP_TOP
+                                1150 LOAD_CONST               0 (None)
+                                1152 RETURN_VALUE
                      ExceptionTable:
-                       270 to 318 -> 1088 [1] lasti
-                       320 to 462 -> 1038 [2] lasti
-                       466 to 750 -> 802 [2]
-                       752 to 774 -> 1088 [1] lasti
-                       802 to 820 -> 1032 [3] lasti
-                       822 to 1020 -> 1022 [3] lasti
-                       1022 to 1030 -> 1032 [3] lasti
-                       1032 to 1036 -> 1038 [2] lasti
-                       1038 to 1044 -> 1046 [4] lasti
-                       1046 to 1050 -> 1088 [1] lasti
-                       1052 to 1052 -> 1046 [4] lasti
-                       1054 to 1058 -> 1088 [1] lasti
-                       1088 to 1094 -> 1096 [3] lasti
-                       1102 to 1102 -> 1096 [3] lasti
+                       310 to 358 -> 1128 [1] lasti
+                       360 to 502 -> 1078 [2] lasti
+                       506 to 790 -> 842 [2]
+                       792 to 814 -> 1128 [1] lasti
+                       842 to 860 -> 1072 [3] lasti
+                       862 to 1060 -> 1062 [3] lasti
+                       1062 to 1070 -> 1072 [3] lasti
+                       1072 to 1076 -> 1078 [2] lasti
+                       1078 to 1084 -> 1086 [4] lasti
+                       1086 to 1090 -> 1128 [1] lasti
+                       1092 to 1092 -> 1086 [4] lasti
+                       1094 to 1098 -> 1128 [1] lasti
+                       1128 to 1134 -> 1136 [3] lasti
+                       1142 to 1142 -> 1136 [3] lasti
                      consts
                         None
                         ('name', 'tlp_service_type', 'instance')
                         'context_parser'
+                        ('flush_on_exit',)
                         ('kind', 'context')
                         ('name', 'service_type', 'span', 'instance', 'config', 'context')
                         'capture_input'
                         'capture_output'
-                     names      ('TracerWrapper', 'verify_initialized', 'get_span_name', 'get', 'callable', 'get_trace_context_from_carrier', 'get_tracer', 'start_as_current_span', 'hasattr', 'capture_input', 'capture_output', 'is_recording', 'set_status', 'StatusCode', 'OK', 'end', 'Exception', 'record_exception', 'Status', 'ERROR', 'str')
+                     names      ('TracerWrapper', 'verify_initialized', 'get_span_name', 'get', 'callable', 'get_trace_context_from_carrier', 'get_tracer', 'is_flush_on_exit', 'start_as_current_span', 'hasattr', 'capture_input', 'capture_output', 'is_recording', 'set_status', 'StatusCode', 'OK', 'end', 'Exception', 'record_exception', 'Status', 'ERROR', 'str')
                      varnames   ('args', 'kwargs', 'span_name', 'service_type', 'context_parser', 'context', 'carrier', 'tracer', 'span', 'span_capture', 'res', 'err')
                      freevars   ('SpanCapture', 'config', 'fn', 'name', 'span_kind', 'tlp_service_type')
                      cellvars   ()
                      filename   '/Users/vuongngo/workspace/agiflow/packages/python/agiflow-sdk/agiflow/opentelemetry/trace_decorators/wrapper.py'
                      name       'wrap'
-                     firstlineno 305
+                     firstlineno 327
                      lnotab
-                        0x08022601100218010201020102fd18062a010401220110011e021e0132
+                        0x08022601100218010201020102fd18062a010401220110011e02460132
                         01040102010201020102010201020102f9040802f8060a4801280202011c
                         0248012a0228013e01280202e818ff1c1b12022a03740328010af708e618
                         ff
                names      ('wraps',)
                varnames   ('fn', 'wrap')
                freevars   ('SpanCapture', 'config', 'name', 'span_kind', 'tlp_service_type')
                cellvars   ('fn',)
                filename   '/Users/vuongngo/workspace/agiflow/packages/python/agiflow-sdk/agiflow/opentelemetry/trace_decorators/wrapper.py'
                name       'decorate'
-               firstlineno 304
+               firstlineno 326
                lnotab 0x06011c0112ff0e010236
          names      ()
          varnames   ('name', 'tlp_service_type', 'span_kind', 'SpanCapture', 'config', 'decorate')
          freevars   ()
          cellvars   ('name', 'tlp_service_type', 'span_kind', 'SpanCapture', 'config')
          filename   '/Users/vuongngo/workspace/agiflow/packages/python/agiflow-sdk/agiflow/opentelemetry/trace_decorators/wrapper.py'
          name       'adecorate_method'
-         firstlineno 297
+         firstlineno 319
          lnotab 0x0c07123a
       'method_name'
       'kwargs'
       code
          argcount  : 5
          nlocals   : 7
          stacksize : 6
@@ -2413,28 +2539,28 @@
                        0 MAKE_CELL                0 (name)
                        2 MAKE_CELL                1 (method_name)
                        4 MAKE_CELL                2 (tlp_service_type)
                        6 MAKE_CELL                3 (span_kind)
                        8 MAKE_CELL                4 (SpanCapture)
                       10 MAKE_CELL                5 (kwargs)
          
-         365          12 RESUME                   0
+         387          12 RESUME                   0
          
-         373          14 LOAD_CLOSURE             4 (SpanCapture)
+         395          14 LOAD_CLOSURE             4 (SpanCapture)
                       16 LOAD_CLOSURE             5 (kwargs)
                       18 LOAD_CLOSURE             1 (method_name)
                       20 LOAD_CLOSURE             0 (name)
                       22 LOAD_CLOSURE             3 (span_kind)
                       24 LOAD_CLOSURE             2 (tlp_service_type)
                       26 BUILD_TUPLE              6
-                      28 LOAD_CONST               1 (<code object decorator, file "/Users/vuongngo/workspace/agiflow/packages/python/agiflow-sdk/agiflow/opentelemetry/trace_decorators/wrapper.py", line 373>)
+                      28 LOAD_CONST               1 (<code object decorator, file "/Users/vuongngo/workspace/agiflow/packages/python/agiflow-sdk/agiflow/opentelemetry/trace_decorators/wrapper.py", line 395>)
                       30 MAKE_FUNCTION            8 (closure)
                       32 STORE_FAST               6 (decorator)
          
-         389          34 LOAD_FAST                6 (decorator)
+         411          34 LOAD_FAST                6 (decorator)
                       36 RETURN_VALUE
          consts
             None
             code
                argcount  : 1
                nlocals   : 3
                stacksize : 13
@@ -2444,92 +2570,92 @@
                   00000000000000a6010000ab0100000000000000007d0174050000000000
                   00000000007c008905a6020000ab0200000000000000007d027407000000
                   000000000000007c008905020074090000000000000000000064027c0189
                   088907890364019c048904a4018e017c02a6010000ab0100000000000000
                   00a6030000ab03000000000000000001007c005300
                              0 COPY_FREE_VARS           6
                
-               373           2 RESUME                   0
+               395           2 RESUME                   0
                
-               374           4 LOAD_DEREF               6 (name)
+               396           4 LOAD_DEREF               6 (name)
                              6 POP_JUMP_FORWARD_IF_FALSE     2 (to 12)
                              8 LOAD_DEREF               6 (name)
                             10 JUMP_FORWARD            19 (to 50)
                        >>   12 LOAD_GLOBAL              1 (NULL + camel_to_snake)
                             24 LOAD_FAST                0 (cls)
                             26 LOAD_ATTR                1 (__name__)
                             36 PRECALL                  1
                             40 CALL                     1
                        >>   50 STORE_FAST               1 (task_name)
                
-               375          52 LOAD_GLOBAL              5 (NULL + getattr)
+               397          52 LOAD_GLOBAL              5 (NULL + getattr)
                             64 LOAD_FAST                0 (cls)
                             66 LOAD_DEREF               5 (method_name)
                             68 PRECALL                  2
                             72 CALL                     2
                             82 STORE_FAST               2 (method)
                
-               376          84 LOAD_GLOBAL              7 (NULL + setattr)
+               398          84 LOAD_GLOBAL              7 (NULL + setattr)
                
-               377          96 LOAD_FAST                0 (cls)
+               399          96 LOAD_FAST                0 (cls)
                
-               378          98 LOAD_DEREF               5 (method_name)
+               400          98 LOAD_DEREF               5 (method_name)
                
-               379         100 PUSH_NULL
+               401         100 PUSH_NULL
                            102 LOAD_GLOBAL              9 (NULL + decorate_method)
                            114 LOAD_CONST               2 (())
                
-               380         116 LOAD_FAST                1 (task_name)
+               402         116 LOAD_FAST                1 (task_name)
                
-               381         118 LOAD_DEREF               8 (tlp_service_type)
+               403         118 LOAD_DEREF               8 (tlp_service_type)
                
-               382         120 LOAD_DEREF               7 (span_kind)
+               404         120 LOAD_DEREF               7 (span_kind)
                
-               383         122 LOAD_DEREF               3 (SpanCapture)
+               405         122 LOAD_DEREF               3 (SpanCapture)
                
-               379         124 LOAD_CONST               1 (('name', 'tlp_service_type', 'span_kind', 'SpanCapture'))
+               401         124 LOAD_CONST               1 (('name', 'tlp_service_type', 'span_kind', 'SpanCapture'))
                            126 BUILD_CONST_KEY_MAP      4
                
-               384         128 LOAD_DEREF               4 (kwargs)
+               406         128 LOAD_DEREF               4 (kwargs)
                
-               379         130 DICT_MERGE               1
+               401         130 DICT_MERGE               1
                            132 CALL_FUNCTION_EX         1
                
-               385         134 LOAD_FAST                2 (method)
+               407         134 LOAD_FAST                2 (method)
                
-               379         136 PRECALL                  1
+               401         136 PRECALL                  1
                            140 CALL                     1
                
-               376         150 PRECALL                  3
+               398         150 PRECALL                  3
                            154 CALL                     3
                            164 POP_TOP
                
-               387         166 LOAD_FAST                0 (cls)
+               409         166 LOAD_FAST                0 (cls)
                            168 RETURN_VALUE
                consts
                   None
                   ('name', 'tlp_service_type', 'span_kind', 'SpanCapture')
                   ()
                names      ('camel_to_snake', '__name__', 'getattr', 'setattr', 'decorate_method')
                varnames   ('cls', 'task_name', 'method')
                freevars   ('SpanCapture', 'kwargs', 'method_name', 'name', 'span_kind', 'tlp_service_type')
                cellvars   ()
                filename   '/Users/vuongngo/workspace/agiflow/packages/python/agiflow-sdk/agiflow/opentelemetry/trace_decorators/wrapper.py'
                name       'decorator'
-               firstlineno 373
+               firstlineno 395
                lnotab
                   0x0401300120010c0102010201100102010201020102fc040502fb040602
                   fa0efd100b
          names      ()
          varnames   ('name', 'method_name', 'tlp_service_type', 'span_kind', 'SpanCapture', 'kwargs', 'decorator')
          freevars   ()
          cellvars   ('name', 'method_name', 'tlp_service_type', 'span_kind', 'SpanCapture', 'kwargs')
          filename   '/Users/vuongngo/workspace/agiflow/packages/python/agiflow-sdk/agiflow/opentelemetry/trace_decorators/wrapper.py'
          name       'decorate_class_method'
-         firstlineno 365
+         firstlineno 387
          lnotab 0x0e081410
       code
          argcount  : 5
          nlocals   : 7
          stacksize : 6
          flags     : 11
          code
@@ -2538,28 +2664,28 @@
                        0 MAKE_CELL                0 (name)
                        2 MAKE_CELL                1 (method_name)
                        4 MAKE_CELL                2 (tlp_service_type)
                        6 MAKE_CELL                3 (span_kind)
                        8 MAKE_CELL                4 (SpanCapture)
                       10 MAKE_CELL                5 (kwargs)
          
-         392          12 RESUME                   0
+         414          12 RESUME                   0
          
-         400          14 LOAD_CLOSURE             4 (SpanCapture)
+         422          14 LOAD_CLOSURE             4 (SpanCapture)
                       16 LOAD_CLOSURE             5 (kwargs)
                       18 LOAD_CLOSURE             1 (method_name)
                       20 LOAD_CLOSURE             0 (name)
                       22 LOAD_CLOSURE             3 (span_kind)
                       24 LOAD_CLOSURE             2 (tlp_service_type)
                       26 BUILD_TUPLE              6
-                      28 LOAD_CONST               1 (<code object decorator, file "/Users/vuongngo/workspace/agiflow/packages/python/agiflow-sdk/agiflow/opentelemetry/trace_decorators/wrapper.py", line 400>)
+                      28 LOAD_CONST               1 (<code object decorator, file "/Users/vuongngo/workspace/agiflow/packages/python/agiflow-sdk/agiflow/opentelemetry/trace_decorators/wrapper.py", line 422>)
                       30 MAKE_FUNCTION            8 (closure)
                       32 STORE_FAST               6 (decorator)
          
-         416          34 LOAD_FAST                6 (decorator)
+         438          34 LOAD_FAST                6 (decorator)
                       36 RETURN_VALUE
          consts
             None
             code
                argcount  : 1
                nlocals   : 3
                stacksize : 13
@@ -2569,99 +2695,99 @@
                   00000000000000a6010000ab0100000000000000007d0174050000000000
                   00000000007c008905a6020000ab0200000000000000007d027407000000
                   000000000000007c008905020074090000000000000000000064027c0189
                   088907890364019c048904a4018e017c02a6010000ab0100000000000000
                   00a6030000ab03000000000000000001007c005300
                              0 COPY_FREE_VARS           6
                
-               400           2 RESUME                   0
+               422           2 RESUME                   0
                
-               401           4 LOAD_DEREF               6 (name)
+               423           4 LOAD_DEREF               6 (name)
                              6 POP_JUMP_FORWARD_IF_FALSE     2 (to 12)
                              8 LOAD_DEREF               6 (name)
                             10 JUMP_FORWARD            19 (to 50)
                        >>   12 LOAD_GLOBAL              1 (NULL + camel_to_snake)
                             24 LOAD_FAST                0 (cls)
                             26 LOAD_ATTR                1 (__name__)
                             36 PRECALL                  1
                             40 CALL                     1
                        >>   50 STORE_FAST               1 (task_name)
                
-               402          52 LOAD_GLOBAL              5 (NULL + getattr)
+               424          52 LOAD_GLOBAL              5 (NULL + getattr)
                             64 LOAD_FAST                0 (cls)
                             66 LOAD_DEREF               5 (method_name)
                             68 PRECALL                  2
                             72 CALL                     2
                             82 STORE_FAST               2 (method)
                
-               403          84 LOAD_GLOBAL              7 (NULL + setattr)
+               425          84 LOAD_GLOBAL              7 (NULL + setattr)
                
-               404          96 LOAD_FAST                0 (cls)
+               426          96 LOAD_FAST                0 (cls)
                
-               405          98 LOAD_DEREF               5 (method_name)
+               427          98 LOAD_DEREF               5 (method_name)
                
-               406         100 PUSH_NULL
+               428         100 PUSH_NULL
                            102 LOAD_GLOBAL              9 (NULL + adecorate_method)
                            114 LOAD_CONST               2 (())
                
-               407         116 LOAD_FAST                1 (task_name)
+               429         116 LOAD_FAST                1 (task_name)
                
-               408         118 LOAD_DEREF               8 (tlp_service_type)
+               430         118 LOAD_DEREF               8 (tlp_service_type)
                
-               409         120 LOAD_DEREF               7 (span_kind)
+               431         120 LOAD_DEREF               7 (span_kind)
                
-               410         122 LOAD_DEREF               3 (SpanCapture)
+               432         122 LOAD_DEREF               3 (SpanCapture)
                
-               406         124 LOAD_CONST               1 (('name', 'tlp_service_type', 'span_kind', 'SpanCapture'))
+               428         124 LOAD_CONST               1 (('name', 'tlp_service_type', 'span_kind', 'SpanCapture'))
                            126 BUILD_CONST_KEY_MAP      4
                
-               411         128 LOAD_DEREF               4 (kwargs)
+               433         128 LOAD_DEREF               4 (kwargs)
                
-               406         130 DICT_MERGE               1
+               428         130 DICT_MERGE               1
                            132 CALL_FUNCTION_EX         1
                
-               412         134 LOAD_FAST                2 (method)
+               434         134 LOAD_FAST                2 (method)
                
-               406         136 PRECALL                  1
+               428         136 PRECALL                  1
                            140 CALL                     1
                
-               403         150 PRECALL                  3
+               425         150 PRECALL                  3
                            154 CALL                     3
                            164 POP_TOP
                
-               414         166 LOAD_FAST                0 (cls)
+               436         166 LOAD_FAST                0 (cls)
                            168 RETURN_VALUE
                consts
                   None
                   ('name', 'tlp_service_type', 'span_kind', 'SpanCapture')
                   ()
                names      ('camel_to_snake', '__name__', 'getattr', 'setattr', 'adecorate_method')
                varnames   ('cls', 'task_name', 'method')
                freevars   ('SpanCapture', 'kwargs', 'method_name', 'name', 'span_kind', 'tlp_service_type')
                cellvars   ()
                filename   '/Users/vuongngo/workspace/agiflow/packages/python/agiflow-sdk/agiflow/opentelemetry/trace_decorators/wrapper.py'
                name       'decorator'
-               firstlineno 400
+               firstlineno 422
                lnotab
                   0x0401300120010c0102010201100102010201020102fc040502fb040602
                   fa0efd100b
          names      ()
          varnames   ('name', 'method_name', 'tlp_service_type', 'span_kind', 'SpanCapture', 'kwargs', 'decorator')
          freevars   ()
          cellvars   ('name', 'method_name', 'tlp_service_type', 'span_kind', 'SpanCapture', 'kwargs')
          filename   '/Users/vuongngo/workspace/agiflow/packages/python/agiflow-sdk/agiflow/opentelemetry/trace_decorators/wrapper.py'
          name       'adecorate_class_method'
-         firstlineno 392
+         firstlineno 414
          lnotab 0x0e081410
-   names      ('abc', 'ABC', 'functools', 'wraps', 'logging', 'typing', 'Any', 'Dict', 'Optional', 'TypeVar', 'Generic', 'Unpack', 'agiflow.opentelemetry.context.span_from_context', 'set_workflow_name_from_context', 'agiflow.opentelemetry.convention', 'SpanAttributes', 'agiflow.opentelemetry.convention.constants', 'AgiflowServiceTypes', 'opentelemetry.trace', 'Span', 'SpanKind', 'Status', 'StatusCode', 'agiflow.opentelemetry.instrumentation.constants.common', 'AGIFLOW_ADDITIONAL_SPAN_ATTRIBUTES_KEY', 'opentelemetry', 'baggage', 'agiflow.version', '__version__', 'agiflow.opentelemetry.trace_decorators.helper', 'SharedKwargsWithHooks', 'add_extra_spans', 'agiflow.opentelemetry.tracing', 'get_tracer', 'TracerWrapper', 'agiflow.opentelemetry.utils', 'should_send_prompts', 'agiflow.opentelemetry.context', 'get_trace_context_from_carrier', 'set_association_properties', 'set_prompt_settings_context', 'set_prompt_attributes_from_context', 'set_workflow_name', 'set_override_enable_context_tracing', 'ContextKeys', 'agiflow.utils', 'serialise_to_json', 'camel_to_snake', 'R', 'getLogger', '__name__', 'logger', 'AbstractSpanCapture', 'BaseSpanCapture', 'TASK', 'INTERNAL', 'str', 'decorate_method', 'adecorate_method', 'decorate_class_method', 'adecorate_class_method')
+   names      ('abc', 'ABC', 'functools', 'wraps', 'logging', 'typing', 'Any', 'Dict', 'Optional', 'TypeVar', 'Generic', 'Unpack', 'agiflow.opentelemetry.context.span_from_context', 'set_workflow_name_from_context', 'agiflow.opentelemetry.convention', 'SpanAttributes', 'agiflow.opentelemetry.convention.agiflow_attributes', 'AgiflowSpanAttributes', 'agiflow.opentelemetry.convention.constants', 'AgiflowServiceTypes', 'opentelemetry.trace', 'Span', 'SpanKind', 'Status', 'StatusCode', 'agiflow.opentelemetry.instrumentation.constants.common', 'AGIFLOW_ADDITIONAL_SPAN_ATTRIBUTES_KEY', 'opentelemetry', 'baggage', 'agiflow.version', '__version__', 'agiflow.opentelemetry.trace_decorators.helper', 'SharedKwargsWithHooks', 'agiflow.opentelemetry.tracing', 'get_tracer', 'TracerWrapper', 'agiflow.opentelemetry.utils', 'should_send_prompts', 'agiflow.opentelemetry.context', 'get_trace_context_from_carrier', 'set_association_properties', 'set_prompt_settings_context', 'set_prompt_attributes_from_context', 'set_workflow_name', 'set_override_enable_context_tracing', 'ContextKeys', 'agiflow.utils', 'serialise_to_json', 'camel_to_snake', 'R', 'getLogger', '__name__', 'logger', 'AbstractSpanCapture', 'BaseSpanCapture', 'TASK', 'INTERNAL', 'str', 'decorate_method', 'adecorate_method', 'decorate_class_method', 'adecorate_class_method')
    varnames   ()
    freevars   ()
    cellvars   ()
    filename   '/Users/vuongngo/workspace/agiflow/packages/python/agiflow-sdk/agiflow/opentelemetry/trace_decorators/wrapper.py'
    name       '<module>'
    firstlineno 1
    lnotab
-      0x00ff02010c010c01080120010c010c010c0118010c030c010c01100410
-      010c0324091005160120032a281c7f001802010c010c0102fc04010eff02
-      020efe02050efb084402010c010c0102fc04010eff02020efe02050efb08
-      470c010c0102fb04010eff020202fe02030efd02060efa081e0c010c0102
-      fb04010eff020202fe02030efd02060efa
+      0x00ff02010c010c01080120010c010c010c010c0118010c030c010c010c
+      0310010c0324091005160120032a281c7f002d02010c010c0102fc04010e
+      ff02020efe02050efb084502010c010c0102fc04010eff02020efe02050e
+      fb08470c010c0102fb04010eff020202fe02030efd02060efa081e0c010c
+      0102fb04010eff020202fe02030efd02060efa
```

### Comparing `agiflow_sdk-0.0.3/agiflow/opentelemetry/trace_decorators/task.py` & `agiflow_sdk-0.0.4/agiflow/opentelemetry/trace_decorators/task.py`

 * *Files identical despite different names*

### Comparing `agiflow_sdk-0.0.3/agiflow/opentelemetry/trace_decorators/workflow.py` & `agiflow_sdk-0.0.4/agiflow/opentelemetry/trace_decorators/workflow.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,14 +24,18 @@
 
     def capture_input(self):
         super().capture_input()
         self.set_span_attribute(
             SpanAttributes.AGIFLOW_SERVICE_TYPE, self.service_type
         )
 
+    @staticmethod
+    def is_flush_on_exit():
+        return True
+
 
 def workflow(
     name: Optional[str] = None,
     method_name: Optional[str] = None,
     span_kind=SpanKind.INTERNAL,
     **kwargs: Unpack[SharedKwargsWithHooks]
 ):
```

### Comparing `agiflow_sdk-0.0.3/agiflow/opentelemetry/trace_decorators/wrapper.py` & `agiflow_sdk-0.0.4/agiflow/opentelemetry/trace_decorators/wrapper.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 from abc import ABC
 from functools import wraps
 import logging
 from typing import Any, Dict, Optional, TypeVar, Generic, Unpack
 from agiflow.opentelemetry.context.span_from_context import set_workflow_name_from_context
 from agiflow.opentelemetry.convention import SpanAttributes
+from agiflow.opentelemetry.convention.agiflow_attributes import AgiflowSpanAttributes
 from agiflow.opentelemetry.convention.constants import AgiflowServiceTypes
 from opentelemetry.trace import Span, SpanKind, Status, StatusCode
 from agiflow.opentelemetry.instrumentation.constants.common import (
     AGIFLOW_ADDITIONAL_SPAN_ATTRIBUTES_KEY,
 )
 from opentelemetry import baggage
 from agiflow.version import __version__
 from agiflow.opentelemetry.trace_decorators.helper import (
     SharedKwargsWithHooks,
-    add_extra_spans
 )
 from agiflow.opentelemetry.tracing import get_tracer, TracerWrapper
 from agiflow.opentelemetry.utils import (
     should_send_prompts,
 )
 from agiflow.opentelemetry.context import (
     get_trace_context_from_carrier,
@@ -114,14 +114,18 @@
         self.set_span_attribute(SpanAttributes.AGIFLOW_SDK_NAME, 'agiflow-python-sdk')
         self.set_span_attribute(SpanAttributes.AGIFLOW_SDK_VERSION, __version__)
         self.set_span_attribute(SpanAttributes.AGIFLOW_SERVICE_NAME, name)
         extra_attributes: Any = baggage.get_baggage(AGIFLOW_ADDITIONAL_SPAN_ATTRIBUTES_KEY)
         self.pydantic_attributes = extra_attributes if extra_attributes is not None else {}
 
     @staticmethod
+    def is_flush_on_exit():
+        return False
+
+    @staticmethod
     def get_span_name(
         name: Optional[str] = None,
         tlp_service_type: Optional[AgiflowServiceTypes] = AgiflowServiceTypes.TASK,
         instance: Any = None,
     ):
         service_type = tlp_service_type or BaseSpanCapture.get_service_type()
 
@@ -140,53 +144,70 @@
         return AgiflowServiceTypes.TASK
 
     def set_span_attribute(self, field, value):
         """
         Using this method to set single attribute
         which field is an enum
         """
-        if self.span.is_recording():
+        if value is not None and self.span.is_recording():
             if hasattr(field, 'value'):
                 self.span.set_attribute(field.value, value)
             else:
                 self.span.set_attribute(field, value)
 
     def capture_input(self):
         if self.name:
             self.set_span_attribute(SpanAttributes.AGIFLOW_ENTITY_NAME, self.name)
 
+        prompt_settings = None
+        association_properties = None
         # Restore context from carrier and apply context to current span attributes
         if self.context is not None and hasattr(self.context, 'get'):
             association_properties = self.context.get(ContextKeys.ASSOCIATION_PROPERTIES)
-            if association_properties is not None:
-                set_association_properties(association_properties)
-                for key, value in association_properties.items():
-                    self.span.set_attribute(
-                          f"{SpanAttributes.AGIFLOW_ASSOCIATION_PROPERTIES}.{key}", value
-                      )
-
             prompt_settings = self.context.get(ContextKeys.PROMPT_SETTINGS)
-            if prompt_settings is not None:
-                set_prompt_settings_context(prompt_settings)
-                set_prompt_attributes_from_context(self.span, self.context)
 
             workflow_name = self.context.get(ContextKeys.WORKFLOW_NAME)
             if workflow_name is not None:
                 set_workflow_name(workflow_name)
                 set_workflow_name_from_context(self.span, self.context)
 
             content_tracing = self.context.get(ContextKeys.OVERRIDE_ENABLE_CONTENT_TRACING)
             if content_tracing is not None:
                 set_override_enable_context_tracing(content_tracing)
 
-        add_extra_spans(
-            self.span,
-            description=self.config.get('description'),
-            prompt_settings=self.config.get('prompt_settings')
-          )
+        self.set_span_attribute(
+          AgiflowSpanAttributes.AGIFLOW_ENTITY_DESCRIPTION,
+          self.config.get('description')
+        )
+
+        prompt_settings_config = self.config.get('prompt_settings')
+        if prompt_settings_config is not None:
+            if callable(prompt_settings_config):
+                prompt_settings = prompt_settings_config(*self.args, **self.kwargs)
+            else:
+                prompt_settings = prompt_settings_config
+
+        association_properties_config = self.config.get('association_properties')
+        if association_properties_config is not None:
+            if callable(association_properties_config):
+                association_properties: Any = association_properties_config(*self.args, **self.kwargs)
+            else:
+                association_properties = association_properties_config
+
+        if prompt_settings is not None:
+            set_prompt_settings_context(prompt_settings)
+            set_prompt_attributes_from_context(self.span, self.context)
+
+        if association_properties is not None:
+            set_association_properties(association_properties)
+            for key, value in association_properties.items():
+                self.span.set_attribute(
+                  f"{SpanAttributes.AGIFLOW_ASSOCIATION_PROPERTIES}.{key}",
+                  value
+                )
 
         try:
             if should_send_prompts():
                 input = ''
                 input_serializer = self.config.get('input_serializer')
 
                 if input_serializer is not None and callable(input_serializer):
@@ -248,15 +269,15 @@
 
             context_parser = config.get('context_parser')
             context = None
             if context_parser is not None and callable(context_parser):
                 carrier = context_parser(*args, **kwargs)
                 context = get_trace_context_from_carrier(carrier)
 
-            with get_tracer() as tracer:
+            with get_tracer(flush_on_exit=SpanCapture.is_flush_on_exit()) as tracer:
                 with tracer.start_as_current_span(span_name, kind=span_kind, context=context) as span:
                     span_capture = SpanCapture(
                       *args,
                       name=name,
                       service_type=service_type,
                       span=span,
                       instance=fn,
@@ -270,14 +291,15 @@
                     try:
                         res = fn(*args, **kwargs)
 
                         if hasattr(span_capture, 'capture_output') and callable(span_capture.capture_output):
                             span_capture.capture_output(res)
 
                         if span.is_recording():
+
                             span.set_status(StatusCode.OK)
                             span.end()
 
                         return res
 
                     except Exception as err:
                         # Record the exception in the span
@@ -315,15 +337,15 @@
 
             context_parser = config.get('context_parser')
             context = None
             if context_parser is not None and callable(context_parser):
                 carrier = context_parser(*args, **kwargs)
                 context = get_trace_context_from_carrier(carrier)
 
-            with get_tracer() as tracer:
+            with get_tracer(flush_on_exit=SpanCapture.is_flush_on_exit()) as tracer:
                 with tracer.start_as_current_span(span_name, kind=span_kind, context=context) as span:
                     span_capture = SpanCapture(
                       *args,
                       name=name,
                       service_type=service_type,
                       span=span,
                       instance=fn,
```

### Comparing `agiflow_sdk-0.0.3/agiflow/opentelemetry/trace_exporter/__pycache__/config.cpython-311.pyc` & `agiflow_sdk-0.0.4/agiflow/opentelemetry/trace_exporter/__pycache__/config.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `agiflow_sdk-0.0.3/agiflow/opentelemetry/trace_exporter/__pycache__/json.cpython-311.pyc` & `agiflow_sdk-0.0.4/agiflow/opentelemetry/trace_exporter/__pycache__/json.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `agiflow_sdk-0.0.3/agiflow/opentelemetry/trace_exporter/config.py` & `agiflow_sdk-0.0.4/agiflow/opentelemetry/trace_exporter/config.py`

 * *Files identical despite different names*

### Comparing `agiflow_sdk-0.0.3/agiflow/opentelemetry/trace_exporter/json.py` & `agiflow_sdk-0.0.4/agiflow/opentelemetry/trace_exporter/json.py`

 * *Files identical despite different names*

### Comparing `agiflow_sdk-0.0.3/agiflow/opentelemetry/trace_sampler/__pycache__/no_sampler.cpython-311.pyc` & `agiflow_sdk-0.0.4/agiflow/opentelemetry/trace_sampler/__pycache__/no_sampler.cpython-311.pyc`

 * *Files 1% similar despite different names*

#### Python bytecode

```diff
@@ -1,9 +1,9 @@
 magic:    0xa70d0d0a
-moddate:  0x3a955b66 (Sat Jun  1 21:40:10 2024 UTC)
+moddate:  0x47d85b66 (Sun Jun  2 02:26:15 2024 UTC)
 files sz: 862
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 5
    flags     : 0
    code
```

### Comparing `agiflow_sdk-0.0.3/agiflow/opentelemetry/trace_sampler/no_sampler.py` & `agiflow_sdk-0.0.4/agiflow/opentelemetry/trace_sampler/no_sampler.py`

 * *Files identical despite different names*

### Comparing `agiflow_sdk-0.0.3/agiflow/opentelemetry/trace_store.py` & `agiflow_sdk-0.0.4/agiflow/opentelemetry/trace_store.py`

 * *Files identical despite different names*

### Comparing `agiflow_sdk-0.0.3/agiflow/opentelemetry/tracing/.DS_Store` & `agiflow_sdk-0.0.4/agiflow/opentelemetry/tracing/.DS_Store`

 * *Files identical despite different names*

### Comparing `agiflow_sdk-0.0.3/agiflow/opentelemetry/tracing/__pycache__/content_allow_list.cpython-311.pyc` & `agiflow_sdk-0.0.4/agiflow/opentelemetry/tracing/__pycache__/content_allow_list.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `agiflow_sdk-0.0.3/agiflow/opentelemetry/tracing/__pycache__/content_alow_list.cpython-311.pyc` & `agiflow_sdk-0.0.4/agiflow/opentelemetry/tracing/__pycache__/content_alow_list.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `agiflow_sdk-0.0.3/agiflow/opentelemetry/tracing/__pycache__/context.cpython-311.pyc` & `agiflow_sdk-0.0.4/agiflow/opentelemetry/tracing/__pycache__/context.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `agiflow_sdk-0.0.3/agiflow/opentelemetry/tracing/__pycache__/context_manager.cpython-311.pyc` & `agiflow_sdk-0.0.4/agiflow/opentelemetry/tracing/__pycache__/context_manager.cpython-311.pyc`

 * *Files 2% similar despite different names*

#### Python bytecode

```diff
@@ -1,9 +1,9 @@
 magic:    0xa70d0d0a
-moddate:  0x02ca5666 (Wed May 29 06:24:02 2024 UTC)
+moddate:  0x87105d66 (Mon Jun  3 00:38:31 2024 UTC)
 files sz: 307
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 4
    flags     : 0
    code
```

### Comparing `agiflow_sdk-0.0.3/agiflow/opentelemetry/tracing/__pycache__/context_propagation.cpython-311.pyc` & `agiflow_sdk-0.0.4/agiflow/opentelemetry/tracing/__pycache__/context_propagation.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `agiflow_sdk-0.0.3/agiflow/opentelemetry/tracing/__pycache__/span_from_context.cpython-311.pyc` & `agiflow_sdk-0.0.4/agiflow/opentelemetry/tracing/__pycache__/span_from_context.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `agiflow_sdk-0.0.3/agiflow/opentelemetry/tracing/__pycache__/tracing.cpython-311.pyc` & `agiflow_sdk-0.0.4/agiflow/opentelemetry/tracing/__pycache__/tracing.cpython-311.pyc`

 * *Files 0% similar despite different names*

#### Python bytecode

```diff
@@ -1,9 +1,9 @@
 magic:    0xa70d0d0a
-moddate:  0x5bd75b66 (Sun Jun  2 02:22:19 2024 UTC)
+moddate:  0x47d85b66 (Sun Jun  2 02:26:15 2024 UTC)
 files sz: 7265
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 6
    flags     : 0
    code
```

### Comparing `agiflow_sdk-0.0.3/agiflow/opentelemetry/tracing/content_allow_list.py` & `agiflow_sdk-0.0.4/agiflow/opentelemetry/tracing/content_allow_list.py`

 * *Files identical despite different names*

### Comparing `agiflow_sdk-0.0.3/agiflow/opentelemetry/tracing/tracing.py` & `agiflow_sdk-0.0.4/agiflow/opentelemetry/tracing/tracing.py`

 * *Files identical despite different names*

### Comparing `agiflow_sdk-0.0.3/agiflow/opentelemetry/types/__init__.py` & `agiflow_sdk-0.0.4/agiflow/opentelemetry/types/__init__.py`

 * *Files identical despite different names*

### Comparing `agiflow_sdk-0.0.3/agiflow/opentelemetry/types/__pycache__/__init__.cpython-311.pyc` & `agiflow_sdk-0.0.4/agiflow/opentelemetry/types/__pycache__/__init__.cpython-311.pyc`

 * *Files 2% similar despite different names*

#### Python bytecode

```diff
@@ -1,9 +1,9 @@
 magic:    0xa70d0d0a
-moddate:  0xb8e45a66 (Sat Jun  1 09:07:04 2024 UTC)
+moddate:  0x47d85b66 (Sun Jun  2 02:26:15 2024 UTC)
 files sz: 813
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 6
    flags     : 0
    code
```

### Comparing `agiflow_sdk-0.0.3/agiflow/opentelemetry/utils/.DS_Store` & `agiflow_sdk-0.0.4/agiflow/opentelemetry/utils/.DS_Store`

 * *Files identical despite different names*

### Comparing `agiflow_sdk-0.0.3/agiflow/opentelemetry/utils/__pycache__/__init__.cpython-311.pyc` & `agiflow_sdk-0.0.4/agiflow/opentelemetry/utils/__pycache__/__init__.cpython-311.pyc`

 * *Files 3% similar despite different names*

#### Python bytecode

```diff
@@ -1,9 +1,9 @@
 magic:    0xa70d0d0a
-moddate:  0xa3e95a66 (Sat Jun  1 09:28:03 2024 UTC)
+moddate:  0x47d85b66 (Sun Jun  2 02:26:15 2024 UTC)
 files sz: 340
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 2
    flags     : 0
    code
```

### Comparing `agiflow_sdk-0.0.3/agiflow/opentelemetry/utils/__pycache__/llm.cpython-311.pyc` & `agiflow_sdk-0.0.4/agiflow/opentelemetry/utils/__pycache__/llm.cpython-311.pyc`

 * *Files 2% similar despite different names*

#### Python bytecode

```diff
@@ -1,9 +1,9 @@
 magic:    0xa70d0d0a
-moddate:  0x58e95a66 (Sat Jun  1 09:26:48 2024 UTC)
+moddate:  0x47d85b66 (Sun Jun  2 02:26:15 2024 UTC)
 files sz: 2240
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 2
    flags     : 0
    code
```

### Comparing `agiflow_sdk-0.0.3/agiflow/opentelemetry/utils/llm.py` & `agiflow_sdk-0.0.4/agiflow/opentelemetry/utils/llm.py`

 * *Files identical despite different names*

### Comparing `agiflow_sdk-0.0.3/agiflow/services/__pycache__/fetch.cpython-311.pyc` & `agiflow_sdk-0.0.4/agiflow/services/__pycache__/fetch.cpython-311.pyc`

 * *Files 0% similar despite different names*

#### Python bytecode

```diff
@@ -1,9 +1,9 @@
 magic:    0xa70d0d0a
-moddate:  0x83d75b66 (Sun Jun  2 02:22:59 2024 UTC)
+moddate:  0x47d85b66 (Sun Jun  2 02:26:15 2024 UTC)
 files sz: 2731
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 8
    flags     : 0
    code
```

### Comparing `agiflow_sdk-0.0.3/agiflow/services/fetch.py` & `agiflow_sdk-0.0.4/agiflow/services/fetch.py`

 * *Files identical despite different names*

### Comparing `agiflow_sdk-0.0.3/agiflow/telemetry/__init__.py` & `agiflow_sdk-0.0.4/agiflow/telemetry/__init__.py`

 * *Files identical despite different names*

### Comparing `agiflow_sdk-0.0.3/agiflow/telemetry/__pycache__/__init__.cpython-311.pyc` & `agiflow_sdk-0.0.4/agiflow/telemetry/__pycache__/__init__.cpython-311.pyc`

 * *Files 0% similar despite different names*

#### Python bytecode

```diff
@@ -1,9 +1,9 @@
 magic:    0xa70d0d0a
-moddate:  0xfd955b66 (Sat Jun  1 21:43:25 2024 UTC)
+moddate:  0x47d85b66 (Sun Jun  2 02:26:15 2024 UTC)
 files sz: 2522
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 4
    flags     : 0
    code
```

### Comparing `agiflow_sdk-0.0.3/agiflow/utils/.DS_Store` & `agiflow_sdk-0.0.4/agiflow/utils/.DS_Store`

 * *Files identical despite different names*

### Comparing `agiflow_sdk-0.0.3/agiflow/utils/__pycache__/__init__.cpython-311.pyc` & `agiflow_sdk-0.0.4/agiflow/utils/__pycache__/__init__.cpython-311.pyc`

 * *Files 0% similar despite different names*

#### Python bytecode

```diff
@@ -1,9 +1,9 @@
 magic:    0xa70d0d0a
-moddate:  0x29ad5b66 (Sat Jun  1 23:22:17 2024 UTC)
+moddate:  0x47d85b66 (Sun Jun  2 02:26:15 2024 UTC)
 files sz: 444
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 2
    flags     : 0
    code
```

### Comparing `agiflow_sdk-0.0.3/agiflow/utils/__pycache__/assertion.cpython-311.pyc` & `agiflow_sdk-0.0.4/agiflow/utils/__pycache__/assertion.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `agiflow_sdk-0.0.3/agiflow/utils/__pycache__/debugging.cpython-311.pyc` & `agiflow_sdk-0.0.4/agiflow/utils/__pycache__/debugging.cpython-311.pyc`

 * *Files 2% similar despite different names*

#### Python bytecode

```diff
@@ -1,9 +1,9 @@
 magic:    0xa70d0d0a
-moddate:  0x5aae5b66 (Sat Jun  1 23:27:22 2024 UTC)
+moddate:  0x47d85b66 (Sun Jun  2 02:26:15 2024 UTC)
 files sz: 580
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 4
    flags     : 0
    code
```

### Comparing `agiflow_sdk-0.0.3/agiflow/utils/__pycache__/error.cpython-311.pyc` & `agiflow_sdk-0.0.4/agiflow/utils/__pycache__/error.cpython-311.pyc`

 * *Files 1% similar despite different names*

#### Python bytecode

```diff
@@ -1,9 +1,9 @@
 magic:    0xa70d0d0a
-moddate:  0x98d75b66 (Sun Jun  2 02:23:20 2024 UTC)
+moddate:  0x47d85b66 (Sun Jun  2 02:26:15 2024 UTC)
 files sz: 847
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 2
    flags     : 0
    code
```

### Comparing `agiflow_sdk-0.0.3/agiflow/utils/__pycache__/llm.cpython-311.pyc` & `agiflow_sdk-0.0.4/agiflow/utils/__pycache__/llm.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `agiflow_sdk-0.0.3/agiflow/utils/__pycache__/string.cpython-311.pyc` & `agiflow_sdk-0.0.4/agiflow/utils/__pycache__/string.cpython-311.pyc`

 * *Files 1% similar despite different names*

#### Python bytecode

```diff
@@ -1,9 +1,9 @@
 magic:    0xa70d0d0a
-moddate:  0xc1af5b66 (Sat Jun  1 23:33:21 2024 UTC)
+moddate:  0x47d85b66 (Sun Jun  2 02:26:15 2024 UTC)
 files sz: 1965
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 4
    flags     : 0
    code
```

### Comparing `agiflow_sdk-0.0.3/agiflow/utils/__pycache__/time.cpython-311.pyc` & `agiflow_sdk-0.0.4/agiflow/utils/__pycache__/time.cpython-311.pyc`

 * *Files 3% similar despite different names*

#### Python bytecode

```diff
@@ -1,9 +1,9 @@
 magic:    0xa70d0d0a
-moddate:  0xa5d75a66 (Sat Jun  1 08:11:17 2024 UTC)
+moddate:  0x47d85b66 (Sun Jun  2 02:26:15 2024 UTC)
 files sz: 264
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 2
    flags     : 0
    code 0x9700640064016c006d005a000100640284005a0164035300
```

### Comparing `agiflow_sdk-0.0.3/agiflow/utils/debugging.py` & `agiflow_sdk-0.0.4/agiflow/utils/debugging.py`

 * *Files identical despite different names*

### Comparing `agiflow_sdk-0.0.3/agiflow/utils/error.py` & `agiflow_sdk-0.0.4/agiflow/utils/error.py`

 * *Files identical despite different names*

### Comparing `agiflow_sdk-0.0.3/agiflow/utils/string.py` & `agiflow_sdk-0.0.4/agiflow/utils/string.py`

 * *Files identical despite different names*

### Comparing `agiflow_sdk-0.0.3/pyproject.toml` & `agiflow_sdk-0.0.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 [tool.coverage.report]
 exclude_lines = [ "if TYPE_CHECKING:" ]
 show_missing = true
 
 [tool.poetry]
 name = "agiflow-sdk"
-version = "0.0.3"
+version = "0.0.4"
 description = "Agiflow Software Development Kit (SDK) for Python"
 authors = [ "Vuong Ngo <vuongngo.pd@gmail.com>" ]
 repository = "https://github.com/agiflowAI/agiflow"
 documentation = "https://docs.agiflow.io/category/python"
 license = "Apache-2.0"
 readme = "README.md"
```

### Comparing `agiflow_sdk-0.0.3/PKG-INFO` & `agiflow_sdk-0.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: agiflow-sdk
-Version: 0.0.3
+Version: 0.0.4
 Summary: Agiflow Software Development Kit (SDK) for Python
 Home-page: https://github.com/agiflowAI/agiflow
 License: Apache-2.0
 Author: Vuong Ngo
 Author-email: vuongngo.pd@gmail.com
 Requires-Python: >=3.9,<4
 Classifier: License :: OSI Approved :: Apache Software License
```

