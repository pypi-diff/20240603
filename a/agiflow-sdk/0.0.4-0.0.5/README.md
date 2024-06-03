# Comparing `tmp/agiflow_sdk-0.0.4.tar.gz` & `tmp/agiflow_sdk-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "agiflow_sdk-0.0.4.tar", max compression
+gzip compressed data, was "agiflow_sdk-0.0.5.tar", max compression
```

## Comparing `agiflow_sdk-0.0.4.tar` & `agiflow_sdk-0.0.5.tar`

### file list

```diff
@@ -1,265 +1,265 @@
--rw-r--r--   0        0        0      394 2024-06-03 06:05:41.412058 agiflow_sdk-0.0.4/README.md
--rw-r--r--   0        0        0       64 2024-06-03 06:05:41.412517 agiflow_sdk-0.0.4/agiflow/__init__.py
--rw-r--r--   0        0        0     5480 2024-06-03 06:05:41.414321 agiflow_sdk-0.0.4/agiflow/agiflow.py
--rw-r--r--   0        0        0      889 2024-06-03 06:05:41.414824 agiflow_sdk-0.0.4/agiflow/config/__init__.py
--rw-r--r--   0        0        0     1838 2024-06-03 06:05:41.415501 agiflow_sdk-0.0.4/agiflow/config/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0      274 2024-06-03 06:05:41.415679 agiflow_sdk-0.0.4/agiflow/config/__pycache__/constants.cpython-311.pyc
--rw-r--r--   0        0        0     1451 2024-06-03 06:05:41.415979 agiflow_sdk-0.0.4/agiflow/config/__pycache__/environment_vars.cpython-311.pyc
--rw-r--r--   0        0        0       72 2024-06-03 06:05:41.416167 agiflow_sdk-0.0.4/agiflow/config/constants.py
--rw-r--r--   0        0        0     1338 2024-06-03 06:05:41.416400 agiflow_sdk-0.0.4/agiflow/config/environment_vars.py
--rw-r--r--   0        0        0     6148 2024-06-03 06:05:41.416762 agiflow_sdk-0.0.4/agiflow/opentelemetry/.DS_Store
--rw-r--r--   0        0        0     1037 2024-06-03 06:05:41.417092 agiflow_sdk-0.0.4/agiflow/opentelemetry/__init__.py
--rw-r--r--   0        0        0     1379 2024-06-03 06:05:41.417890 agiflow_sdk-0.0.4/agiflow/opentelemetry/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0     4092 2024-06-03 06:05:41.418277 agiflow_sdk-0.0.4/agiflow/opentelemetry/__pycache__/trace_store.cpython-311.pyc
--rw-r--r--   0        0        0      223 2024-06-03 06:05:41.418700 agiflow_sdk-0.0.4/agiflow/opentelemetry/__pycache__/version.cpython-311.pyc
--rw-r--r--   0        0        0     1218 2024-06-03 06:05:41.419039 agiflow_sdk-0.0.4/agiflow/opentelemetry/context/__init__.py
--rw-r--r--   0        0        0     1363 2024-06-03 06:05:41.419592 agiflow_sdk-0.0.4/agiflow/opentelemetry/context/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0     1790 2024-06-03 06:05:41.419739 agiflow_sdk-0.0.4/agiflow/opentelemetry/context/__pycache__/constants.cpython-311.pyc
--rw-r--r--   0        0        0     2868 2024-06-03 06:05:41.420055 agiflow_sdk-0.0.4/agiflow/opentelemetry/context/__pycache__/context.cpython-311.pyc
--rw-r--r--   0        0        0     3327 2024-06-03 06:05:41.420253 agiflow_sdk-0.0.4/agiflow/opentelemetry/context/__pycache__/context_propagation.cpython-311.pyc
--rw-r--r--   0        0        0     2105 2024-06-03 06:05:41.420617 agiflow_sdk-0.0.4/agiflow/opentelemetry/context/__pycache__/set_span_from_context.cpython-311.pyc
--rw-r--r--   0        0        0     2101 2024-06-03 06:05:41.420953 agiflow_sdk-0.0.4/agiflow/opentelemetry/context/__pycache__/span_from_context.cpython-311.pyc
--rw-r--r--   0        0        0      740 2024-06-03 06:05:41.421160 agiflow_sdk-0.0.4/agiflow/opentelemetry/context/constants.py
--rw-r--r--   0        0        0     1231 2024-06-03 06:05:41.421419 agiflow_sdk-0.0.4/agiflow/opentelemetry/context/context.py
--rw-r--r--   0        0        0     2139 2024-06-03 06:05:41.421686 agiflow_sdk-0.0.4/agiflow/opentelemetry/context/context_propagation.py
--rw-r--r--   0        0        0     1285 2024-06-03 06:05:41.421908 agiflow_sdk-0.0.4/agiflow/opentelemetry/context/span_from_context.py
--rw-r--r--   0        0        0     1583 2024-06-03 06:05:41.422360 agiflow_sdk-0.0.4/agiflow/opentelemetry/convention/__init__.py
--rw-r--r--   0        0        0     2184 2024-06-03 06:05:41.422694 agiflow_sdk-0.0.4/agiflow/opentelemetry/convention/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0     2922 2024-06-03 06:05:41.422883 agiflow_sdk-0.0.4/agiflow/opentelemetry/convention/__pycache__/agiflow_attributes.cpython-311.pyc
--rw-r--r--   0        0        0     7800 2024-06-03 06:05:41.423114 agiflow_sdk-0.0.4/agiflow/opentelemetry/convention/__pycache__/constants.cpython-311.pyc
--rw-r--r--   0        0        0     3106 2024-06-03 06:05:41.423254 agiflow_sdk-0.0.4/agiflow/opentelemetry/convention/__pycache__/database_span_attributes.cpython-311.pyc
--rw-r--r--   0        0        0     1665 2024-06-03 06:05:41.423590 agiflow_sdk-0.0.4/agiflow/opentelemetry/convention/__pycache__/framework_span_attributes.cpython-311.pyc
--rw-r--r--   0        0        0     7042 2024-06-03 06:05:41.423727 agiflow_sdk-0.0.4/agiflow/opentelemetry/convention/__pycache__/llm_span_attributes.cpython-311.pyc
--rw-r--r--   0        0        0     2477 2024-06-03 06:05:41.423906 agiflow_sdk-0.0.4/agiflow/opentelemetry/convention/agiflow_attributes.py
--rw-r--r--   0        0        0     3893 2024-06-03 06:05:41.424041 agiflow_sdk-0.0.4/agiflow/opentelemetry/convention/constants.py
--rw-r--r--   0        0        0     2279 2024-06-03 06:05:41.424175 agiflow_sdk-0.0.4/agiflow/opentelemetry/convention/database_span_attributes.py
--rw-r--r--   0        0        0      875 2024-06-03 06:05:41.424403 agiflow_sdk-0.0.4/agiflow/opentelemetry/convention/framework_span_attributes.py
--rw-r--r--   0        0        0     6050 2024-06-03 06:05:41.424653 agiflow_sdk-0.0.4/agiflow/opentelemetry/convention/llm_span_attributes.py
--rw-r--r--   0        0        0    10305 2024-06-03 06:05:41.424919 agiflow_sdk-0.0.4/agiflow/opentelemetry/instrumentation/__init__.py
--rw-r--r--   0        0        0    13104 2024-06-03 06:05:41.425367 agiflow_sdk-0.0.4/agiflow/opentelemetry/instrumentation/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0      154 2024-06-03 06:05:41.425742 agiflow_sdk-0.0.4/agiflow/opentelemetry/instrumentation/anthropic/__init__.py
--rw-r--r--   0        0        0      398 2024-06-03 06:05:41.426523 agiflow_sdk-0.0.4/agiflow/opentelemetry/instrumentation/anthropic/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0     2946 2024-06-03 06:05:41.426662 agiflow_sdk-0.0.4/agiflow/opentelemetry/instrumentation/anthropic/__pycache__/instrumentation.cpython-311.pyc
--rw-r--r--   0        0        0      158 2024-06-03 06:05:41.426910 agiflow_sdk-0.0.4/agiflow/opentelemetry/instrumentation/anthropic/hooks/__init__.py
--rw-r--r--   0        0        0      409 2024-06-03 06:05:41.427164 agiflow_sdk-0.0.4/agiflow/opentelemetry/instrumentation/anthropic/hooks/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0     2606 2024-06-03 06:05:41.427307 agiflow_sdk-0.0.4/agiflow/opentelemetry/instrumentation/anthropic/hooks/__pycache__/base.cpython-311.pyc
--rw-r--r--   0        0        0     9937 2024-06-03 06:05:41.427467 agiflow_sdk-0.0.4/agiflow/opentelemetry/instrumentation/anthropic/hooks/__pycache__/message_create.cpython-311.pyc
--rw-r--r--   0        0        0     1581 2024-06-03 06:05:41.427720 agiflow_sdk-0.0.4/agiflow/opentelemetry/instrumentation/anthropic/hooks/base.py
--rw-r--r--   0        0        0     7481 2024-06-03 06:05:41.427945 agiflow_sdk-0.0.4/agiflow/opentelemetry/instrumentation/anthropic/hooks/message_create.py
--rw-r--r--   0        0        0     1730 2024-06-03 06:05:41.428153 agiflow_sdk-0.0.4/agiflow/opentelemetry/instrumentation/anthropic/instrumentation.py
--rw-r--r--   0        0        0      145 2024-06-03 06:05:41.428426 agiflow_sdk-0.0.4/agiflow/opentelemetry/instrumentation/chroma/__init__.py
--rw-r--r--   0        0        0      389 2024-06-03 06:05:41.429120 agiflow_sdk-0.0.4/agiflow/opentelemetry/instrumentation/chroma/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0     3196 2024-06-03 06:05:41.429322 agiflow_sdk-0.0.4/agiflow/opentelemetry/instrumentation/chroma/__pycache__/instrumentation.cpython-311.pyc
--rw-r--r--   0        0        0      157 2024-06-03 06:05:41.429552 agiflow_sdk-0.0.4/agiflow/opentelemetry/instrumentation/chroma/hooks/__init__.py
--rw-r--r--   0        0        0      405 2024-06-03 06:05:41.429778 agiflow_sdk-0.0.4/agiflow/opentelemetry/instrumentation/chroma/hooks/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0     2297 2024-06-03 06:05:41.430014 agiflow_sdk-0.0.4/agiflow/opentelemetry/instrumentation/chroma/hooks/__pycache__/base.cpython-311.pyc
--rw-r--r--   0        0        0    16999 2024-06-03 06:05:41.430395 agiflow_sdk-0.0.4/agiflow/opentelemetry/instrumentation/chroma/hooks/__pycache__/collection_call.cpython-311.pyc
--rw-r--r--   0        0        0     1385 2024-06-03 06:05:41.430558 agiflow_sdk-0.0.4/agiflow/opentelemetry/instrumentation/chroma/hooks/base.py
--rw-r--r--   0        0        0    10704 2024-06-03 06:05:41.430702 agiflow_sdk-0.0.4/agiflow/opentelemetry/instrumentation/chroma/hooks/collection_call.py
--rw-r--r--   0        0        0     1910 2024-06-03 06:05:41.430938 agiflow_sdk-0.0.4/agiflow/opentelemetry/instrumentation/chroma/instrumentation.py
--rw-r--r--   0        0        0      145 2024-06-03 06:05:41.431172 agiflow_sdk-0.0.4/agiflow/opentelemetry/instrumentation/cohere/__init__.py
--rw-r--r--   0        0        0      389 2024-06-03 06:05:41.432049 agiflow_sdk-0.0.4/agiflow/opentelemetry/instrumentation/cohere/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0     3487 2024-06-03 06:05:41.432194 agiflow_sdk-0.0.4/agiflow/opentelemetry/instrumentation/cohere/__pycache__/instrumentation.cpython-311.pyc
--rw-r--r--   0        0        0      511 2024-06-03 06:05:41.432537 agiflow_sdk-0.0.4/agiflow/opentelemetry/instrumentation/cohere/hooks/__init__.py
--rw-r--r--   0        0        0      809 2024-06-03 06:05:41.432797 agiflow_sdk-0.0.4/agiflow/opentelemetry/instrumentation/cohere/hooks/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0     2247 2024-06-03 06:05:41.432946 agiflow_sdk-0.0.4/agiflow/opentelemetry/instrumentation/cohere/hooks/__pycache__/base.cpython-311.pyc
--rw-r--r--   0        0        0     8362 2024-06-03 06:05:41.433095 agiflow_sdk-0.0.4/agiflow/opentelemetry/instrumentation/cohere/hooks/__pycache__/base_chat.cpython-311.pyc
--rw-r--r--   0        0        0     6177 2024-06-03 06:05:41.433320 agiflow_sdk-0.0.4/agiflow/opentelemetry/instrumentation/cohere/hooks/__pycache__/chat_create.cpython-311.pyc
--rw-r--r--   0        0        0     7073 2024-06-03 06:05:41.433467 agiflow_sdk-0.0.4/agiflow/opentelemetry/instrumentation/cohere/hooks/__pycache__/chat_stream.cpython-311.pyc
--rw-r--r--   0        0        0     5336 2024-06-03 06:05:41.433606 agiflow_sdk-0.0.4/agiflow/opentelemetry/instrumentation/cohere/hooks/__pycache__/embed.cpython-311.pyc
--rw-r--r--   0        0        0     5930 2024-06-03 06:05:41.433737 agiflow_sdk-0.0.4/agiflow/opentelemetry/instrumentation/cohere/hooks/__pycache__/rerank.cpython-311.pyc
--rw-r--r--   0        0        0     1328 2024-06-03 06:05:41.433895 agiflow_sdk-0.0.4/agiflow/opentelemetry/instrumentation/cohere/hooks/base.py
--rw-r--r--   0        0        0     5765 2024-06-03 06:05:41.434039 agiflow_sdk-0.0.4/agiflow/opentelemetry/instrumentation/cohere/hooks/base_chat.py
--rw-r--r--   0        0        0     4975 2024-06-03 06:05:41.434168 agiflow_sdk-0.0.4/agiflow/opentelemetry/instrumentation/cohere/hooks/chat_create.py
--rw-r--r--   0        0        0     7065 2024-06-03 06:05:41.434297 agiflow_sdk-0.0.4/agiflow/opentelemetry/instrumentation/cohere/hooks/chat_stream.py
--rw-r--r--   0        0        0     3919 2024-06-03 06:05:41.434436 agiflow_sdk-0.0.4/agiflow/opentelemetry/instrumentation/cohere/hooks/embed.py
--rw-r--r--   0        0        0     4364 2024-06-03 06:05:41.434567 agiflow_sdk-0.0.4/agiflow/opentelemetry/instrumentation/cohere/hooks/rerank.py
--rw-r--r--   0        0        0     2425 2024-06-03 06:05:41.434716 agiflow_sdk-0.0.4/agiflow/opentelemetry/instrumentation/cohere/instrumentation.py
--rw-r--r--   0        0        0      391 2024-06-03 06:05:41.435061 agiflow_sdk-0.0.4/agiflow/opentelemetry/instrumentation/constants/__init__.py
--rw-r--r--   0        0        0      649 2024-06-03 06:05:41.435613 agiflow_sdk-0.0.4/agiflow/opentelemetry/instrumentation/constants/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0      346 2024-06-03 06:05:41.435875 agiflow_sdk-0.0.4/agiflow/opentelemetry/instrumentation/constants/__pycache__/anthropic.cpython-311.pyc
--rw-r--r--   0        0        0     1014 2024-06-03 06:05:41.436026 agiflow_sdk-0.0.4/agiflow/opentelemetry/instrumentation/constants/__pycache__/chroma.cpython-311.pyc
--rw-r--r--   0        0        0      595 2024-06-03 06:05:41.436173 agiflow_sdk-0.0.4/agiflow/opentelemetry/instrumentation/constants/__pycache__/cohere.cpython-311.pyc
--rw-r--r--   0        0        0      902 2024-06-03 06:05:41.436412 agiflow_sdk-0.0.4/agiflow/opentelemetry/instrumentation/constants/__pycache__/common.cpython-311.pyc
--rw-r--r--   0        0        0     1074 2024-06-03 06:05:41.436638 agiflow_sdk-0.0.4/agiflow/opentelemetry/instrumentation/constants/__pycache__/openai.cpython-311.pyc
--rw-r--r--   0        0        0      126 2024-06-03 06:05:41.436885 agiflow_sdk-0.0.4/agiflow/opentelemetry/instrumentation/constants/anthropic.py
--rw-r--r--   0        0        0      972 2024-06-03 06:05:41.437021 agiflow_sdk-0.0.4/agiflow/opentelemetry/instrumentation/constants/chroma.py
--rw-r--r--   0        0        0      577 2024-06-03 06:05:41.437150 agiflow_sdk-0.0.4/agiflow/opentelemetry/instrumentation/constants/cohere.py
--rw-r--r--   0        0        0      750 2024-06-03 06:05:41.437337 agiflow_sdk-0.0.4/agiflow/opentelemetry/instrumentation/constants/common.py
--rw-r--r--   0        0        0      134 2024-06-03 06:05:41.437471 agiflow_sdk-0.0.4/agiflow/opentelemetry/instrumentation/constants/groq.py
--rw-r--r--   0        0        0     1054 2024-06-03 06:05:41.437695 agiflow_sdk-0.0.4/agiflow/opentelemetry/instrumentation/constants/openai.py
--rw-r--r--   0        0        0      490 2024-06-03 06:05:41.437825 agiflow_sdk-0.0.4/agiflow/opentelemetry/instrumentation/constants/pinecone.py
--rw-r--r--   0        0        0     2016 2024-06-03 06:05:41.437956 agiflow_sdk-0.0.4/agiflow/opentelemetry/instrumentation/constants/qdrant.py
--rw-r--r--   0        0        0     1518 2024-06-03 06:05:41.438190 agiflow_sdk-0.0.4/agiflow/opentelemetry/instrumentation/constants/weaviate.py
--rw-r--r--   0        0        0      139 2024-06-03 06:05:41.438552 agiflow_sdk-0.0.4/agiflow/opentelemetry/instrumentation/groq/__init__.py
--rw-r--r--   0        0        0      156 2024-06-03 06:05:41.438767 agiflow_sdk-0.0.4/agiflow/opentelemetry/instrumentation/groq/hooks/__init__.py
--rw-r--r--   0        0        0     1934 2024-06-03 06:05:41.438916 agiflow_sdk-0.0.4/agiflow/opentelemetry/instrumentation/groq/hooks/base.py
--rw-r--r--   0        0        0    12481 2024-06-03 06:05:41.439078 agiflow_sdk-0.0.4/agiflow/opentelemetry/instrumentation/groq/hooks/chat_completion.py
--rw-r--r--   0        0        0     1993 2024-06-03 06:05:41.439259 agiflow_sdk-0.0.4/agiflow/opentelemetry/instrumentation/groq/instrumentation.py
--rw-r--r--   0        0        0     6148 2024-06-03 06:05:41.439706 agiflow_sdk-0.0.4/agiflow/opentelemetry/instrumentation/langchain/.DS_Store
--rw-r--r--   0        0        0      154 2024-06-03 06:05:41.439849 agiflow_sdk-0.0.4/agiflow/opentelemetry/instrumentation/langchain/__init__.py
--rw-r--r--   0        0        0      398 2024-06-03 06:05:41.440237 agiflow_sdk-0.0.4/agiflow/opentelemetry/instrumentation/langchain/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0     3233 2024-06-03 06:05:41.440535 agiflow_sdk-0.0.4/agiflow/opentelemetry/instrumentation/langchain/__pycache__/instrumentation.cpython-311.pyc
--rw-r--r--   0        0        0     4136 2024-06-03 06:05:41.440888 agiflow_sdk-0.0.4/agiflow/opentelemetry/instrumentation/langchain/__pycache__/patch.cpython-311.pyc
--rw-r--r--   0        0        0      252 2024-06-03 06:05:41.441276 agiflow_sdk-0.0.4/agiflow/opentelemetry/instrumentation/langchain/hooks/__init__.py
--rw-r--r--   0        0        0      532 2024-06-03 06:05:41.441747 agiflow_sdk-0.0.4/agiflow/opentelemetry/instrumentation/langchain/hooks/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0     2313 2024-06-03 06:05:41.441903 agiflow_sdk-0.0.4/agiflow/opentelemetry/instrumentation/langchain/hooks/__pycache__/base.cpython-311.pyc
--rw-r--r--   0        0        0     7286 2024-06-03 06:05:41.442050 agiflow_sdk-0.0.4/agiflow/opentelemetry/instrumentation/langchain/hooks/__pycache__/chat.cpython-311.pyc
--rw-r--r--   0        0        0     3122 2024-06-03 06:05:41.442293 agiflow_sdk-0.0.4/agiflow/opentelemetry/instrumentation/langchain/hooks/__pycache__/generic.cpython-311.pyc
--rw-r--r--   0        0        0     1384 2024-06-03 06:05:41.442449 agiflow_sdk-0.0.4/agiflow/opentelemetry/instrumentation/langchain/hooks/base.py
--rw-r--r--   0        0        0     5021 2024-06-03 06:05:41.442597 agiflow_sdk-0.0.4/agiflow/opentelemetry/instrumentation/langchain/hooks/chat.py
--rw-r--r--   0        0        0     1741 2024-06-03 06:05:41.442839 agiflow_sdk-0.0.4/agiflow/opentelemetry/instrumentation/langchain/hooks/generic.py
--rw-r--r--   0        0        0     2232 2024-06-03 06:05:41.442987 agiflow_sdk-0.0.4/agiflow/opentelemetry/instrumentation/langchain/instrumentation.py
--rw-r--r--   0        0        0     6148 2024-06-03 06:05:41.443400 agiflow_sdk-0.0.4/agiflow/opentelemetry/instrumentation/langchain_community/.DS_Store
--rw-r--r--   0        0        0      182 2024-06-03 06:05:41.443636 agiflow_sdk-0.0.4/agiflow/opentelemetry/instrumentation/langchain_community/__init__.py
--rw-r--r--   0        0        0      427 2024-06-03 06:05:41.443862 agiflow_sdk-0.0.4/agiflow/opentelemetry/instrumentation/langchain_community/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0     3462 2024-06-03 06:05:41.443997 agiflow_sdk-0.0.4/agiflow/opentelemetry/instrumentation/langchain_community/__pycache__/instrumentation.cpython-311.pyc
--rw-r--r--   0        0        0    11425 2024-06-03 06:05:41.444345 agiflow_sdk-0.0.4/agiflow/opentelemetry/instrumentation/langchain_community/__pycache__/patch.cpython-311.pyc
--rw-r--r--   0        0        0     6148 2024-06-03 06:05:41.444880 agiflow_sdk-0.0.4/agiflow/opentelemetry/instrumentation/langchain_community/hooks/.DS_Store
--rw-r--r--   0        0        0      141 2024-06-03 06:05:41.445007 agiflow_sdk-0.0.4/agiflow/opentelemetry/instrumentation/langchain_community/hooks/__init__.py
--rw-r--r--   0        0        0      404 2024-06-03 06:05:41.445483 agiflow_sdk-0.0.4/agiflow/opentelemetry/instrumentation/langchain_community/hooks/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0     2481 2024-06-03 06:05:41.445724 agiflow_sdk-0.0.4/agiflow/opentelemetry/instrumentation/langchain_community/hooks/__pycache__/base.cpython-311.pyc
--rw-r--r--   0        0        0     6863 2024-06-03 06:05:41.446022 agiflow_sdk-0.0.4/agiflow/opentelemetry/instrumentation/langchain_community/hooks/__pycache__/chat.cpython-311.pyc
--rw-r--r--   0        0        0     3163 2024-06-03 06:05:41.446194 agiflow_sdk-0.0.4/agiflow/opentelemetry/instrumentation/langchain_community/hooks/__pycache__/generic.cpython-311.pyc
--rw-r--r--   0        0        0     5119 2024-06-03 06:05:41.446495 agiflow_sdk-0.0.4/agiflow/opentelemetry/instrumentation/langchain_community/hooks/__pycache__/llm.cpython-311.pyc
--rw-r--r--   0        0        0     1499 2024-06-03 06:05:41.446635 agiflow_sdk-0.0.4/agiflow/opentelemetry/instrumentation/langchain_community/hooks/base.py
--rw-r--r--   0        0        0     1769 2024-06-03 06:05:41.446777 agiflow_sdk-0.0.4/agiflow/opentelemetry/instrumentation/langchain_community/hooks/generic.py
--rw-r--r--   0        0        0     3005 2024-06-03 06:05:41.446925 agiflow_sdk-0.0.4/agiflow/opentelemetry/instrumentation/langchain_community/instrumentation.py
--rw-r--r--   0        0        0     6148 2024-06-03 06:05:41.447349 agiflow_sdk-0.0.4/agiflow/opentelemetry/instrumentation/langchain_core/.DS_Store
--rw-r--r--   0        0        0      167 2024-06-03 06:05:41.447482 agiflow_sdk-0.0.4/agiflow/opentelemetry/instrumentation/langchain_core/__init__.py
--rw-r--r--   0        0        0      412 2024-06-03 06:05:41.447699 agiflow_sdk-0.0.4/agiflow/opentelemetry/instrumentation/langchain_core/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0     3928 2024-06-03 06:05:41.447837 agiflow_sdk-0.0.4/agiflow/opentelemetry/instrumentation/langchain_core/__pycache__/instrumentation.cpython-311.pyc
--rw-r--r--   0        0        0     8316 2024-06-03 06:05:41.448068 agiflow_sdk-0.0.4/agiflow/opentelemetry/instrumentation/langchain_core/__pycache__/patch.cpython-311.pyc
--rw-r--r--   0        0        0      390 2024-06-03 06:05:41.448485 agiflow_sdk-0.0.4/agiflow/opentelemetry/instrumentation/langchain_core/hooks/__init__.py
--rw-r--r--   0        0        0      693 2024-06-03 06:05:41.448717 agiflow_sdk-0.0.4/agiflow/opentelemetry/instrumentation/langchain_core/hooks/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0     2558 2024-06-03 06:05:41.448857 agiflow_sdk-0.0.4/agiflow/opentelemetry/instrumentation/langchain_core/hooks/__pycache__/base.cpython-311.pyc
--rw-r--r--   0        0        0     3573 2024-06-03 06:05:41.449088 agiflow_sdk-0.0.4/agiflow/opentelemetry/instrumentation/langchain_core/hooks/__pycache__/generic.cpython-311.pyc
--rw-r--r--   0        0        0     5208 2024-06-03 06:05:41.449222 agiflow_sdk-0.0.4/agiflow/opentelemetry/instrumentation/langchain_core/hooks/__pycache__/llm.cpython-311.pyc
--rw-r--r--   0        0        0     4692 2024-06-03 06:05:41.449552 agiflow_sdk-0.0.4/agiflow/opentelemetry/instrumentation/langchain_core/hooks/__pycache__/runnable.cpython-311.pyc
--rw-r--r--   0        0        0     1533 2024-06-03 06:05:41.449806 agiflow_sdk-0.0.4/agiflow/opentelemetry/instrumentation/langchain_core/hooks/base.py
--rw-r--r--   0        0        0     2152 2024-06-03 06:05:41.449938 agiflow_sdk-0.0.4/agiflow/opentelemetry/instrumentation/langchain_core/hooks/generic.py
--rw-r--r--   0        0        0     3178 2024-06-03 06:05:41.450124 agiflow_sdk-0.0.4/agiflow/opentelemetry/instrumentation/langchain_core/hooks/llm.py
--rw-r--r--   0        0        0     3248 2024-06-03 06:05:41.450261 agiflow_sdk-0.0.4/agiflow/opentelemetry/instrumentation/langchain_core/hooks/runnable.py
--rw-r--r--   0        0        0     3346 2024-06-03 06:05:41.450417 agiflow_sdk-0.0.4/agiflow/opentelemetry/instrumentation/langchain_core/instrumentation.py
--rw-r--r--   0        0        0      154 2024-06-03 06:05:41.450911 agiflow_sdk-0.0.4/agiflow/opentelemetry/instrumentation/langgraph/__init__.py
--rw-r--r--   0        0        0      146 2024-06-03 06:05:41.451140 agiflow_sdk-0.0.4/agiflow/opentelemetry/instrumentation/langgraph/hooks/__init__.py
--rw-r--r--   0        0        0     1343 2024-06-03 06:05:41.451283 agiflow_sdk-0.0.4/agiflow/opentelemetry/instrumentation/langgraph/hooks/base.py
--rw-r--r--   0        0        0     3352 2024-06-03 06:05:41.451409 agiflow_sdk-0.0.4/agiflow/opentelemetry/instrumentation/langgraph/hooks/graph_call.py
--rw-r--r--   0        0        0     2873 2024-06-03 06:05:41.451560 agiflow_sdk-0.0.4/agiflow/opentelemetry/instrumentation/langgraph/instrumentation.py
--rw-r--r--   0        0        0      157 2024-06-03 06:05:41.451861 agiflow_sdk-0.0.4/agiflow/opentelemetry/instrumentation/llamaindex/__init__.py
--rw-r--r--   0        0        0      140 2024-06-03 06:05:41.452087 agiflow_sdk-0.0.4/agiflow/opentelemetry/instrumentation/llamaindex/hooks/__init__.py
--rw-r--r--   0        0        0     1347 2024-06-03 06:05:41.452241 agiflow_sdk-0.0.4/agiflow/opentelemetry/instrumentation/llamaindex/hooks/base.py
--rw-r--r--   0        0        0     1718 2024-06-03 06:05:41.452379 agiflow_sdk-0.0.4/agiflow/opentelemetry/instrumentation/llamaindex/hooks/generic.py
--rw-r--r--   0        0        0     2944 2024-06-03 06:05:41.452553 agiflow_sdk-0.0.4/agiflow/opentelemetry/instrumentation/llamaindex/instrumentation.py
--rw-r--r--   0        0        0     6148 2024-06-03 06:05:41.452909 agiflow_sdk-0.0.4/agiflow/opentelemetry/instrumentation/openai/.DS_Store
--rw-r--r--   0        0        0      145 2024-06-03 06:05:41.453083 agiflow_sdk-0.0.4/agiflow/opentelemetry/instrumentation/openai/__init__.py
--rw-r--r--   0        0        0      389 2024-06-03 06:05:41.453320 agiflow_sdk-0.0.4/agiflow/opentelemetry/instrumentation/openai/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0     3659 2024-06-03 06:05:41.453451 agiflow_sdk-0.0.4/agiflow/opentelemetry/instrumentation/openai/__pycache__/instrumentation.cpython-311.pyc
--rw-r--r--   0        0        0    20526 2024-06-03 06:05:41.454059 agiflow_sdk-0.0.4/agiflow/opentelemetry/instrumentation/openai/__pycache__/patch.cpython-311.pyc
--rw-r--r--   0        0        0     6148 2024-06-03 06:05:41.454586 agiflow_sdk-0.0.4/agiflow/opentelemetry/instrumentation/openai/hooks/.DS_Store
--rw-r--r--   0        0        0      424 2024-06-03 06:05:41.454719 agiflow_sdk-0.0.4/agiflow/opentelemetry/instrumentation/openai/hooks/__init__.py
--rw-r--r--   0        0        0      699 2024-06-03 06:05:41.456812 agiflow_sdk-0.0.4/agiflow/opentelemetry/instrumentation/openai/hooks/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0     4035 2024-06-03 06:05:41.456990 agiflow_sdk-0.0.4/agiflow/opentelemetry/instrumentation/openai/hooks/__pycache__/base.cpython-311.pyc
--rw-r--r--   0        0        0     4744 2024-06-03 06:05:41.457303 agiflow_sdk-0.0.4/agiflow/opentelemetry/instrumentation/openai/hooks/__pycache__/base_llm.cpython-311.pyc
--rw-r--r--   0        0        0    12171 2024-06-03 06:05:41.457481 agiflow_sdk-0.0.4/agiflow/opentelemetry/instrumentation/openai/hooks/__pycache__/chat_completion.cpython-311.pyc
--rw-r--r--   0        0        0    11736 2024-06-03 06:05:41.458012 agiflow_sdk-0.0.4/agiflow/opentelemetry/instrumentation/openai/hooks/__pycache__/completion.cpython-311.pyc
--rw-r--r--   0        0        0     3391 2024-06-03 06:05:41.458360 agiflow_sdk-0.0.4/agiflow/opentelemetry/instrumentation/openai/hooks/__pycache__/embedding.cpython-311.pyc
--rw-r--r--   0        0        0     3885 2024-06-03 06:05:41.458541 agiflow_sdk-0.0.4/agiflow/opentelemetry/instrumentation/openai/hooks/__pycache__/image_generate.cpython-311.pyc
--rw-r--r--   0        0        0     2374 2024-06-03 06:05:41.458731 agiflow_sdk-0.0.4/agiflow/opentelemetry/instrumentation/openai/hooks/__pycache__/utils.cpython-311.pyc
--rw-r--r--   0        0        0     2474 2024-06-03 06:05:41.458908 agiflow_sdk-0.0.4/agiflow/opentelemetry/instrumentation/openai/hooks/base.py
--rw-r--r--   0        0        0     3115 2024-06-03 06:05:41.459151 agiflow_sdk-0.0.4/agiflow/opentelemetry/instrumentation/openai/hooks/base_llm.py
--rw-r--r--   0        0        0    10648 2024-06-03 06:05:41.459315 agiflow_sdk-0.0.4/agiflow/opentelemetry/instrumentation/openai/hooks/chat_completion.py
--rw-r--r--   0        0        0     2257 2024-06-03 06:05:41.459821 agiflow_sdk-0.0.4/agiflow/opentelemetry/instrumentation/openai/hooks/embedding.py
--rw-r--r--   0        0        0     2555 2024-06-03 06:05:41.460077 agiflow_sdk-0.0.4/agiflow/opentelemetry/instrumentation/openai/hooks/image_generate.py
--rw-r--r--   0        0        0     2211 2024-06-03 06:05:41.460239 agiflow_sdk-0.0.4/agiflow/opentelemetry/instrumentation/openai/hooks/utils.py
--rw-r--r--   0        0        0     2910 2024-06-03 06:05:41.460411 agiflow_sdk-0.0.4/agiflow/opentelemetry/instrumentation/openai/instrumentation.py
--rw-r--r--   0        0        0      151 2024-06-03 06:05:41.460834 agiflow_sdk-0.0.4/agiflow/opentelemetry/instrumentation/pinecone/__init__.py
--rw-r--r--   0        0        0      137 2024-06-03 06:05:41.461063 agiflow_sdk-0.0.4/agiflow/opentelemetry/instrumentation/pinecone/hooks/__init__.py
--rw-r--r--   0        0        0     1396 2024-06-03 06:05:41.461197 agiflow_sdk-0.0.4/agiflow/opentelemetry/instrumentation/pinecone/hooks/base.py
--rw-r--r--   0        0        0     6892 2024-06-03 06:05:41.461331 agiflow_sdk-0.0.4/agiflow/opentelemetry/instrumentation/pinecone/hooks/generic.py
--rw-r--r--   0        0        0     2019 2024-06-03 06:05:41.461477 agiflow_sdk-0.0.4/agiflow/opentelemetry/instrumentation/pinecone/instrumentation.py
--rw-r--r--   0        0        0      145 2024-06-03 06:05:41.461711 agiflow_sdk-0.0.4/agiflow/opentelemetry/instrumentation/qdrant/__init__.py
--rw-r--r--   0        0        0      152 2024-06-03 06:05:41.461912 agiflow_sdk-0.0.4/agiflow/opentelemetry/instrumentation/qdrant/hooks/__init__.py
--rw-r--r--   0        0        0     1388 2024-06-03 06:05:41.462043 agiflow_sdk-0.0.4/agiflow/opentelemetry/instrumentation/qdrant/hooks/base.py
--rw-r--r--   0        0        0     3113 2024-06-03 06:05:41.462178 agiflow_sdk-0.0.4/agiflow/opentelemetry/instrumentation/qdrant/hooks/collection.py
--rw-r--r--   0        0        0     1913 2024-06-03 06:05:41.462314 agiflow_sdk-0.0.4/agiflow/opentelemetry/instrumentation/qdrant/instrumentation.py
--rw-r--r--   0        0        0     2309 2024-06-03 06:05:41.462545 agiflow_sdk-0.0.4/agiflow/opentelemetry/instrumentation/utils/__init__.py
--rw-r--r--   0        0        0     2790 2024-06-03 06:05:41.462885 agiflow_sdk-0.0.4/agiflow/opentelemetry/instrumentation/utils/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0    17396 2024-06-03 06:05:41.463247 agiflow_sdk-0.0.4/agiflow/opentelemetry/instrumentation/utils/__pycache__/wrapper.cpython-311.pyc
--rw-r--r--   0        0        0    11559 2024-06-03 06:05:41.463408 agiflow_sdk-0.0.4/agiflow/opentelemetry/instrumentation/utils/wrapper.py
--rw-r--r--   0        0        0      151 2024-06-03 06:05:41.464045 agiflow_sdk-0.0.4/agiflow/opentelemetry/instrumentation/weaviate/__init__.py
--rw-r--r--   0        0        0      306 2024-06-03 06:05:41.464335 agiflow_sdk-0.0.4/agiflow/opentelemetry/instrumentation/weaviate/hooks/__init__.py
--rw-r--r--   0        0        0     1396 2024-06-03 06:05:41.464496 agiflow_sdk-0.0.4/agiflow/opentelemetry/instrumentation/weaviate/hooks/base.py
--rw-r--r--   0        0        0     1776 2024-06-03 06:05:41.464670 agiflow_sdk-0.0.4/agiflow/opentelemetry/instrumentation/weaviate/hooks/generic_collection.py
--rw-r--r--   0        0        0     4091 2024-06-03 06:05:41.464817 agiflow_sdk-0.0.4/agiflow/opentelemetry/instrumentation/weaviate/hooks/generic_query.py
--rw-r--r--   0        0        0     2754 2024-06-03 06:05:41.465004 agiflow_sdk-0.0.4/agiflow/opentelemetry/instrumentation/weaviate/instrumentation.py
--rw-r--r--   0        0        0      144 2024-06-03 06:05:41.465457 agiflow_sdk-0.0.4/agiflow/opentelemetry/span_processors/__init__.py
--rw-r--r--   0        0        0      376 2024-06-03 06:05:41.466056 agiflow_sdk-0.0.4/agiflow/opentelemetry/span_processors/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0     5123 2024-06-03 06:05:41.466324 agiflow_sdk-0.0.4/agiflow/opentelemetry/span_processors/__pycache__/thread_pool_span_processor.cpython-311.pyc
--rw-r--r--   0        0        0     2544 2024-06-03 06:05:41.466610 agiflow_sdk-0.0.4/agiflow/opentelemetry/span_processors/thread_pool_span_processor.py
--rw-r--r--   0        0        0      644 2024-06-03 06:05:41.466926 agiflow_sdk-0.0.4/agiflow/opentelemetry/trace_decorators/__init__.py
--rw-r--r--   0        0        0      910 2024-06-03 06:05:41.467498 agiflow_sdk-0.0.4/agiflow/opentelemetry/trace_decorators/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0     1383 2024-06-03 06:05:41.467757 agiflow_sdk-0.0.4/agiflow/opentelemetry/trace_decorators/__pycache__/helper.cpython-311.pyc
--rw-r--r--   0        0        0     4548 2024-06-03 06:05:41.467975 agiflow_sdk-0.0.4/agiflow/opentelemetry/trace_decorators/__pycache__/task.cpython-311.pyc
--rw-r--r--   0        0        0     3461 2024-06-03 06:05:41.468329 agiflow_sdk-0.0.4/agiflow/opentelemetry/trace_decorators/__pycache__/workflow.cpython-311.pyc
--rw-r--r--   0        0        0    19398 2024-06-03 06:05:41.468711 agiflow_sdk-0.0.4/agiflow/opentelemetry/trace_decorators/__pycache__/wrapper.cpython-311.pyc
--rw-r--r--   0        0        0     1650 2024-06-03 06:05:41.468999 agiflow_sdk-0.0.4/agiflow/opentelemetry/trace_decorators/helper.py
--rw-r--r--   0        0        0     3514 2024-06-03 06:05:41.469243 agiflow_sdk-0.0.4/agiflow/opentelemetry/trace_decorators/task.py
--rw-r--r--   0        0        0     2241 2024-06-03 06:05:41.469499 agiflow_sdk-0.0.4/agiflow/opentelemetry/trace_decorators/workflow.py
--rw-r--r--   0        0        0    15064 2024-06-03 06:05:41.469740 agiflow_sdk-0.0.4/agiflow/opentelemetry/trace_decorators/wrapper.py
--rw-r--r--   0        0        0      115 2024-06-03 06:05:41.470099 agiflow_sdk-0.0.4/agiflow/opentelemetry/trace_exporter/__init__.py
--rw-r--r--   0        0        0      349 2024-06-03 06:05:41.470425 agiflow_sdk-0.0.4/agiflow/opentelemetry/trace_exporter/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0     2687 2024-06-03 06:05:41.470653 agiflow_sdk-0.0.4/agiflow/opentelemetry/trace_exporter/__pycache__/config.cpython-311.pyc
--rw-r--r--   0        0        0     9661 2024-06-03 06:05:41.470914 agiflow_sdk-0.0.4/agiflow/opentelemetry/trace_exporter/__pycache__/json.cpython-311.pyc
--rw-r--r--   0        0        0      238 2024-06-03 06:05:41.471145 agiflow_sdk-0.0.4/agiflow/opentelemetry/trace_exporter/__pycache__/version.cpython-311.pyc
--rw-r--r--   0        0        0     2757 2024-06-03 06:05:41.471379 agiflow_sdk-0.0.4/agiflow/opentelemetry/trace_exporter/config.py
--rw-r--r--   0        0        0     7123 2024-06-03 06:05:41.471616 agiflow_sdk-0.0.4/agiflow/opentelemetry/trace_exporter/json.py
--rw-r--r--   0        0        0       22 2024-06-03 06:05:41.471738 agiflow_sdk-0.0.4/agiflow/opentelemetry/trace_exporter/version.py
--rw-r--r--   0        0        0       99 2024-06-03 06:05:41.472143 agiflow_sdk-0.0.4/agiflow/opentelemetry/trace_sampler/__init__.py
--rw-r--r--   0        0        0      342 2024-06-03 06:05:41.472503 agiflow_sdk-0.0.4/agiflow/opentelemetry/trace_sampler/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0     1787 2024-06-03 06:05:41.472741 agiflow_sdk-0.0.4/agiflow/opentelemetry/trace_sampler/__pycache__/no_sampler.cpython-311.pyc
--rw-r--r--   0        0        0      862 2024-06-03 06:05:41.472991 agiflow_sdk-0.0.4/agiflow/opentelemetry/trace_sampler/no_sampler.py
--rw-r--r--   0        0        0     3160 2024-06-03 06:05:41.473320 agiflow_sdk-0.0.4/agiflow/opentelemetry/trace_store.py
--rw-r--r--   0        0        0     6148 2024-06-03 06:05:41.473786 agiflow_sdk-0.0.4/agiflow/opentelemetry/tracing/.DS_Store
--rw-r--r--   0        0        0      182 2024-06-03 06:05:41.473962 agiflow_sdk-0.0.4/agiflow/opentelemetry/tracing/__init__.py
--rw-r--r--   0        0        0      437 2024-06-03 06:05:41.474292 agiflow_sdk-0.0.4/agiflow/opentelemetry/tracing/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0     1979 2024-06-03 06:05:41.474519 agiflow_sdk-0.0.4/agiflow/opentelemetry/tracing/__pycache__/content_allow_list.cpython-311.pyc
--rw-r--r--   0        0        0     1978 2024-06-03 06:05:41.474657 agiflow_sdk-0.0.4/agiflow/opentelemetry/tracing/__pycache__/content_alow_list.cpython-311.pyc
--rw-r--r--   0        0        0     5230 2024-06-03 06:05:41.474795 agiflow_sdk-0.0.4/agiflow/opentelemetry/tracing/__pycache__/context.cpython-311.pyc
--rw-r--r--   0        0        0      897 2024-06-03 06:05:41.474922 agiflow_sdk-0.0.4/agiflow/opentelemetry/tracing/__pycache__/context_manager.cpython-311.pyc
--rw-r--r--   0        0        0     1507 2024-06-03 06:05:41.475149 agiflow_sdk-0.0.4/agiflow/opentelemetry/tracing/__pycache__/context_propagation.cpython-311.pyc
--rw-r--r--   0        0        0     2581 2024-06-03 06:05:41.475342 agiflow_sdk-0.0.4/agiflow/opentelemetry/tracing/__pycache__/span_from_context.cpython-311.pyc
--rw-r--r--   0        0        0    10065 2024-06-03 06:05:41.475565 agiflow_sdk-0.0.4/agiflow/opentelemetry/tracing/__pycache__/tracing.cpython-311.pyc
--rw-r--r--   0        0        0      846 2024-06-03 06:05:41.475844 agiflow_sdk-0.0.4/agiflow/opentelemetry/tracing/content_allow_list.py
--rw-r--r--   0        0        0      307 2024-06-03 06:05:41.476054 agiflow_sdk-0.0.4/agiflow/opentelemetry/tracing/context_manager.py
--rw-r--r--   0        0        0     7265 2024-06-03 06:05:41.476272 agiflow_sdk-0.0.4/agiflow/opentelemetry/tracing/tracing.py
--rw-r--r--   0        0        0      813 2024-06-03 06:05:41.476558 agiflow_sdk-0.0.4/agiflow/opentelemetry/types/__init__.py
--rw-r--r--   0        0        0     1865 2024-06-03 06:05:41.476962 agiflow_sdk-0.0.4/agiflow/opentelemetry/types/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0     6148 2024-06-03 06:05:41.477297 agiflow_sdk-0.0.4/agiflow/opentelemetry/utils/.DS_Store
--rw-r--r--   0        0        0      340 2024-06-03 06:05:41.477424 agiflow_sdk-0.0.4/agiflow/opentelemetry/utils/__init__.py
--rw-r--r--   0        0        0      521 2024-06-03 06:05:41.478103 agiflow_sdk-0.0.4/agiflow/opentelemetry/utils/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0     3447 2024-06-03 06:05:41.478316 agiflow_sdk-0.0.4/agiflow/opentelemetry/utils/__pycache__/llm.cpython-311.pyc
--rw-r--r--   0        0        0     2240 2024-06-03 06:05:41.478481 agiflow_sdk-0.0.4/agiflow/opentelemetry/utils/llm.py
--rw-r--r--   0        0        0       71 2024-06-03 06:05:41.478746 agiflow_sdk-0.0.4/agiflow/services/__init__.py
--rw-r--r--   0        0        0      297 2024-06-03 06:05:41.478969 agiflow_sdk-0.0.4/agiflow/services/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0     5452 2024-06-03 06:05:41.479106 agiflow_sdk-0.0.4/agiflow/services/__pycache__/fetch.cpython-311.pyc
--rw-r--r--   0        0        0     2731 2024-06-03 06:05:41.479241 agiflow_sdk-0.0.4/agiflow/services/fetch.py
--rw-r--r--   0        0        0     2522 2024-06-03 06:05:41.479459 agiflow_sdk-0.0.4/agiflow/telemetry/__init__.py
--rw-r--r--   0        0        0     4829 2024-06-03 06:05:41.479677 agiflow_sdk-0.0.4/agiflow/telemetry/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0     6148 2024-06-03 06:05:41.480130 agiflow_sdk-0.0.4/agiflow/utils/.DS_Store
--rw-r--r--   0        0        0      444 2024-06-03 06:05:41.480283 agiflow_sdk-0.0.4/agiflow/utils/__init__.py
--rw-r--r--   0        0        0      728 2024-06-03 06:05:41.480498 agiflow_sdk-0.0.4/agiflow/utils/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0      532 2024-06-03 06:05:41.480739 agiflow_sdk-0.0.4/agiflow/utils/__pycache__/assertion.cpython-311.pyc
--rw-r--r--   0        0        0     1923 2024-06-03 06:05:41.480879 agiflow_sdk-0.0.4/agiflow/utils/__pycache__/debugging.cpython-311.pyc
--rw-r--r--   0        0        0     1719 2024-06-03 06:05:41.481013 agiflow_sdk-0.0.4/agiflow/utils/__pycache__/error.cpython-311.pyc
--rw-r--r--   0        0        0     3268 2024-06-03 06:05:41.481246 agiflow_sdk-0.0.4/agiflow/utils/__pycache__/llm.cpython-311.pyc
--rw-r--r--   0        0        0     4718 2024-06-03 06:05:41.481389 agiflow_sdk-0.0.4/agiflow/utils/__pycache__/string.cpython-311.pyc
--rw-r--r--   0        0        0      583 2024-06-03 06:05:41.481522 agiflow_sdk-0.0.4/agiflow/utils/__pycache__/time.cpython-311.pyc
--rw-r--r--   0        0        0      207 2024-06-03 06:05:41.481757 agiflow_sdk-0.0.4/agiflow/utils/assertion.py
--rw-r--r--   0        0        0      580 2024-06-03 06:05:41.481884 agiflow_sdk-0.0.4/agiflow/utils/debugging.py
--rw-r--r--   0        0        0      847 2024-06-03 06:05:41.482020 agiflow_sdk-0.0.4/agiflow/utils/error.py
--rw-r--r--   0        0        0     1965 2024-06-03 06:05:41.482142 agiflow_sdk-0.0.4/agiflow/utils/string.py
--rw-r--r--   0        0        0      264 2024-06-03 06:05:41.482273 agiflow_sdk-0.0.4/agiflow/utils/time.py
--rw-r--r--   0        0        0       22 2024-06-03 06:05:41.482399 agiflow_sdk-0.0.4/agiflow/version.py
--rw-r--r--   0        0        0     1106 2024-06-03 06:05:41.488768 agiflow_sdk-0.0.4/pyproject.toml
--rw-r--r--   0        0        0     1760 1970-01-01 00:00:00.000000 agiflow_sdk-0.0.4/PKG-INFO
+-rw-r--r--   0        0        0      394 2024-06-03 09:15:32.791219 agiflow_sdk-0.0.5/README.md
+-rw-r--r--   0        0        0       64 2024-06-03 09:15:32.791760 agiflow_sdk-0.0.5/agiflow/__init__.py
+-rw-r--r--   0        0        0     5480 2024-06-03 09:15:32.792935 agiflow_sdk-0.0.5/agiflow/agiflow.py
+-rw-r--r--   0        0        0      889 2024-06-03 09:15:32.793274 agiflow_sdk-0.0.5/agiflow/config/__init__.py
+-rw-r--r--   0        0        0     1838 2024-06-03 09:15:32.793640 agiflow_sdk-0.0.5/agiflow/config/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0      274 2024-06-03 09:15:32.793840 agiflow_sdk-0.0.5/agiflow/config/__pycache__/constants.cpython-311.pyc
+-rw-r--r--   0        0        0     1451 2024-06-03 09:15:32.794043 agiflow_sdk-0.0.5/agiflow/config/__pycache__/environment_vars.cpython-311.pyc
+-rw-r--r--   0        0        0       72 2024-06-03 09:15:32.794226 agiflow_sdk-0.0.5/agiflow/config/constants.py
+-rw-r--r--   0        0        0     1338 2024-06-03 09:15:32.794456 agiflow_sdk-0.0.5/agiflow/config/environment_vars.py
+-rw-r--r--   0        0        0     6148 2024-06-03 09:15:32.794811 agiflow_sdk-0.0.5/agiflow/opentelemetry/.DS_Store
+-rw-r--r--   0        0        0     1037 2024-06-03 09:15:32.795169 agiflow_sdk-0.0.5/agiflow/opentelemetry/__init__.py
+-rw-r--r--   0        0        0     1379 2024-06-03 09:15:32.796271 agiflow_sdk-0.0.5/agiflow/opentelemetry/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0     4092 2024-06-03 09:15:32.796584 agiflow_sdk-0.0.5/agiflow/opentelemetry/__pycache__/trace_store.cpython-311.pyc
+-rw-r--r--   0        0        0      223 2024-06-03 09:15:32.801806 agiflow_sdk-0.0.5/agiflow/opentelemetry/__pycache__/version.cpython-311.pyc
+-rw-r--r--   0        0        0     1218 2024-06-03 09:15:32.802253 agiflow_sdk-0.0.5/agiflow/opentelemetry/context/__init__.py
+-rw-r--r--   0        0        0     1363 2024-06-03 09:15:32.802507 agiflow_sdk-0.0.5/agiflow/opentelemetry/context/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0     1790 2024-06-03 09:15:32.802728 agiflow_sdk-0.0.5/agiflow/opentelemetry/context/__pycache__/constants.cpython-311.pyc
+-rw-r--r--   0        0        0     2868 2024-06-03 09:15:32.803122 agiflow_sdk-0.0.5/agiflow/opentelemetry/context/__pycache__/context.cpython-311.pyc
+-rw-r--r--   0        0        0     3327 2024-06-03 09:15:32.803501 agiflow_sdk-0.0.5/agiflow/opentelemetry/context/__pycache__/context_propagation.cpython-311.pyc
+-rw-r--r--   0        0        0     2105 2024-06-03 09:15:32.803850 agiflow_sdk-0.0.5/agiflow/opentelemetry/context/__pycache__/set_span_from_context.cpython-311.pyc
+-rw-r--r--   0        0        0     2101 2024-06-03 09:15:32.804263 agiflow_sdk-0.0.5/agiflow/opentelemetry/context/__pycache__/span_from_context.cpython-311.pyc
+-rw-r--r--   0        0        0      740 2024-06-03 09:15:32.804580 agiflow_sdk-0.0.5/agiflow/opentelemetry/context/constants.py
+-rw-r--r--   0        0        0     1231 2024-06-03 09:15:32.804843 agiflow_sdk-0.0.5/agiflow/opentelemetry/context/context.py
+-rw-r--r--   0        0        0     2139 2024-06-03 09:15:32.805111 agiflow_sdk-0.0.5/agiflow/opentelemetry/context/context_propagation.py
+-rw-r--r--   0        0        0     1285 2024-06-03 09:15:32.805317 agiflow_sdk-0.0.5/agiflow/opentelemetry/context/span_from_context.py
+-rw-r--r--   0        0        0     1583 2024-06-03 09:15:32.805835 agiflow_sdk-0.0.5/agiflow/opentelemetry/convention/__init__.py
+-rw-r--r--   0        0        0     2184 2024-06-03 09:15:32.806200 agiflow_sdk-0.0.5/agiflow/opentelemetry/convention/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0     2922 2024-06-03 09:15:32.806414 agiflow_sdk-0.0.5/agiflow/opentelemetry/convention/__pycache__/agiflow_attributes.cpython-311.pyc
+-rw-r--r--   0        0        0     7800 2024-06-03 09:15:32.806633 agiflow_sdk-0.0.5/agiflow/opentelemetry/convention/__pycache__/constants.cpython-311.pyc
+-rw-r--r--   0        0        0     3106 2024-06-03 09:15:32.806975 agiflow_sdk-0.0.5/agiflow/opentelemetry/convention/__pycache__/database_span_attributes.cpython-311.pyc
+-rw-r--r--   0        0        0     1665 2024-06-03 09:15:32.807283 agiflow_sdk-0.0.5/agiflow/opentelemetry/convention/__pycache__/framework_span_attributes.cpython-311.pyc
+-rw-r--r--   0        0        0     7042 2024-06-03 09:15:32.807442 agiflow_sdk-0.0.5/agiflow/opentelemetry/convention/__pycache__/llm_span_attributes.cpython-311.pyc
+-rw-r--r--   0        0        0     2477 2024-06-03 09:15:32.807625 agiflow_sdk-0.0.5/agiflow/opentelemetry/convention/agiflow_attributes.py
+-rw-r--r--   0        0        0     3893 2024-06-03 09:15:32.807776 agiflow_sdk-0.0.5/agiflow/opentelemetry/convention/constants.py
+-rw-r--r--   0        0        0     2279 2024-06-03 09:15:32.807931 agiflow_sdk-0.0.5/agiflow/opentelemetry/convention/database_span_attributes.py
+-rw-r--r--   0        0        0      875 2024-06-03 09:15:32.808166 agiflow_sdk-0.0.5/agiflow/opentelemetry/convention/framework_span_attributes.py
+-rw-r--r--   0        0        0     6050 2024-06-03 09:15:32.808441 agiflow_sdk-0.0.5/agiflow/opentelemetry/convention/llm_span_attributes.py
+-rw-r--r--   0        0        0    10305 2024-06-03 09:15:32.808785 agiflow_sdk-0.0.5/agiflow/opentelemetry/instrumentation/__init__.py
+-rw-r--r--   0        0        0    13104 2024-06-03 09:15:32.809123 agiflow_sdk-0.0.5/agiflow/opentelemetry/instrumentation/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0      154 2024-06-03 09:15:32.809508 agiflow_sdk-0.0.5/agiflow/opentelemetry/instrumentation/anthropic/__init__.py
+-rw-r--r--   0        0        0      398 2024-06-03 09:15:32.809761 agiflow_sdk-0.0.5/agiflow/opentelemetry/instrumentation/anthropic/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0     2946 2024-06-03 09:15:32.809909 agiflow_sdk-0.0.5/agiflow/opentelemetry/instrumentation/anthropic/__pycache__/instrumentation.cpython-311.pyc
+-rw-r--r--   0        0        0      158 2024-06-03 09:15:32.810137 agiflow_sdk-0.0.5/agiflow/opentelemetry/instrumentation/anthropic/hooks/__init__.py
+-rw-r--r--   0        0        0      409 2024-06-03 09:15:32.810361 agiflow_sdk-0.0.5/agiflow/opentelemetry/instrumentation/anthropic/hooks/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0     2606 2024-06-03 09:15:32.810497 agiflow_sdk-0.0.5/agiflow/opentelemetry/instrumentation/anthropic/hooks/__pycache__/base.cpython-311.pyc
+-rw-r--r--   0        0        0     9937 2024-06-03 09:15:32.810639 agiflow_sdk-0.0.5/agiflow/opentelemetry/instrumentation/anthropic/hooks/__pycache__/message_create.cpython-311.pyc
+-rw-r--r--   0        0        0     1581 2024-06-03 09:15:32.810841 agiflow_sdk-0.0.5/agiflow/opentelemetry/instrumentation/anthropic/hooks/base.py
+-rw-r--r--   0        0        0     7481 2024-06-03 09:15:32.811058 agiflow_sdk-0.0.5/agiflow/opentelemetry/instrumentation/anthropic/hooks/message_create.py
+-rw-r--r--   0        0        0     1730 2024-06-03 09:15:32.811248 agiflow_sdk-0.0.5/agiflow/opentelemetry/instrumentation/anthropic/instrumentation.py
+-rw-r--r--   0        0        0      145 2024-06-03 09:15:32.811493 agiflow_sdk-0.0.5/agiflow/opentelemetry/instrumentation/chroma/__init__.py
+-rw-r--r--   0        0        0      389 2024-06-03 09:15:32.811943 agiflow_sdk-0.0.5/agiflow/opentelemetry/instrumentation/chroma/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0     3196 2024-06-03 09:15:32.812133 agiflow_sdk-0.0.5/agiflow/opentelemetry/instrumentation/chroma/__pycache__/instrumentation.cpython-311.pyc
+-rw-r--r--   0        0        0      157 2024-06-03 09:15:32.812399 agiflow_sdk-0.0.5/agiflow/opentelemetry/instrumentation/chroma/hooks/__init__.py
+-rw-r--r--   0        0        0      405 2024-06-03 09:15:32.812627 agiflow_sdk-0.0.5/agiflow/opentelemetry/instrumentation/chroma/hooks/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0     2297 2024-06-03 09:15:32.812882 agiflow_sdk-0.0.5/agiflow/opentelemetry/instrumentation/chroma/hooks/__pycache__/base.cpython-311.pyc
+-rw-r--r--   0        0        0    16999 2024-06-03 09:15:32.813087 agiflow_sdk-0.0.5/agiflow/opentelemetry/instrumentation/chroma/hooks/__pycache__/collection_call.cpython-311.pyc
+-rw-r--r--   0        0        0     1385 2024-06-03 09:15:32.813247 agiflow_sdk-0.0.5/agiflow/opentelemetry/instrumentation/chroma/hooks/base.py
+-rw-r--r--   0        0        0    10704 2024-06-03 09:15:32.813398 agiflow_sdk-0.0.5/agiflow/opentelemetry/instrumentation/chroma/hooks/collection_call.py
+-rw-r--r--   0        0        0     1910 2024-06-03 09:15:32.813616 agiflow_sdk-0.0.5/agiflow/opentelemetry/instrumentation/chroma/instrumentation.py
+-rw-r--r--   0        0        0      145 2024-06-03 09:15:32.813848 agiflow_sdk-0.0.5/agiflow/opentelemetry/instrumentation/cohere/__init__.py
+-rw-r--r--   0        0        0      389 2024-06-03 09:15:32.814232 agiflow_sdk-0.0.5/agiflow/opentelemetry/instrumentation/cohere/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0     3487 2024-06-03 09:15:32.814393 agiflow_sdk-0.0.5/agiflow/opentelemetry/instrumentation/cohere/__pycache__/instrumentation.cpython-311.pyc
+-rw-r--r--   0        0        0      511 2024-06-03 09:15:32.814784 agiflow_sdk-0.0.5/agiflow/opentelemetry/instrumentation/cohere/hooks/__init__.py
+-rw-r--r--   0        0        0      809 2024-06-03 09:15:32.815061 agiflow_sdk-0.0.5/agiflow/opentelemetry/instrumentation/cohere/hooks/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0     2247 2024-06-03 09:15:32.815214 agiflow_sdk-0.0.5/agiflow/opentelemetry/instrumentation/cohere/hooks/__pycache__/base.cpython-311.pyc
+-rw-r--r--   0        0        0     8362 2024-06-03 09:15:32.815382 agiflow_sdk-0.0.5/agiflow/opentelemetry/instrumentation/cohere/hooks/__pycache__/base_chat.cpython-311.pyc
+-rw-r--r--   0        0        0     6177 2024-06-03 09:15:32.815573 agiflow_sdk-0.0.5/agiflow/opentelemetry/instrumentation/cohere/hooks/__pycache__/chat_create.cpython-311.pyc
+-rw-r--r--   0        0        0     7073 2024-06-03 09:15:32.815713 agiflow_sdk-0.0.5/agiflow/opentelemetry/instrumentation/cohere/hooks/__pycache__/chat_stream.cpython-311.pyc
+-rw-r--r--   0        0        0     5336 2024-06-03 09:15:32.815853 agiflow_sdk-0.0.5/agiflow/opentelemetry/instrumentation/cohere/hooks/__pycache__/embed.cpython-311.pyc
+-rw-r--r--   0        0        0     5930 2024-06-03 09:15:32.816009 agiflow_sdk-0.0.5/agiflow/opentelemetry/instrumentation/cohere/hooks/__pycache__/rerank.cpython-311.pyc
+-rw-r--r--   0        0        0     1328 2024-06-03 09:15:32.816157 agiflow_sdk-0.0.5/agiflow/opentelemetry/instrumentation/cohere/hooks/base.py
+-rw-r--r--   0        0        0     5765 2024-06-03 09:15:32.816293 agiflow_sdk-0.0.5/agiflow/opentelemetry/instrumentation/cohere/hooks/base_chat.py
+-rw-r--r--   0        0        0     4975 2024-06-03 09:15:32.816429 agiflow_sdk-0.0.5/agiflow/opentelemetry/instrumentation/cohere/hooks/chat_create.py
+-rw-r--r--   0        0        0     7065 2024-06-03 09:15:32.816577 agiflow_sdk-0.0.5/agiflow/opentelemetry/instrumentation/cohere/hooks/chat_stream.py
+-rw-r--r--   0        0        0     3919 2024-06-03 09:15:32.816744 agiflow_sdk-0.0.5/agiflow/opentelemetry/instrumentation/cohere/hooks/embed.py
+-rw-r--r--   0        0        0     4364 2024-06-03 09:15:32.817070 agiflow_sdk-0.0.5/agiflow/opentelemetry/instrumentation/cohere/hooks/rerank.py
+-rw-r--r--   0        0        0     2425 2024-06-03 09:15:32.817300 agiflow_sdk-0.0.5/agiflow/opentelemetry/instrumentation/cohere/instrumentation.py
+-rw-r--r--   0        0        0      391 2024-06-03 09:15:32.817662 agiflow_sdk-0.0.5/agiflow/opentelemetry/instrumentation/constants/__init__.py
+-rw-r--r--   0        0        0      649 2024-06-03 09:15:32.818008 agiflow_sdk-0.0.5/agiflow/opentelemetry/instrumentation/constants/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0      346 2024-06-03 09:15:32.818266 agiflow_sdk-0.0.5/agiflow/opentelemetry/instrumentation/constants/__pycache__/anthropic.cpython-311.pyc
+-rw-r--r--   0        0        0     1014 2024-06-03 09:15:32.818410 agiflow_sdk-0.0.5/agiflow/opentelemetry/instrumentation/constants/__pycache__/chroma.cpython-311.pyc
+-rw-r--r--   0        0        0      595 2024-06-03 09:15:32.818543 agiflow_sdk-0.0.5/agiflow/opentelemetry/instrumentation/constants/__pycache__/cohere.cpython-311.pyc
+-rw-r--r--   0        0        0      902 2024-06-03 09:15:32.818777 agiflow_sdk-0.0.5/agiflow/opentelemetry/instrumentation/constants/__pycache__/common.cpython-311.pyc
+-rw-r--r--   0        0        0     1074 2024-06-03 09:15:32.819021 agiflow_sdk-0.0.5/agiflow/opentelemetry/instrumentation/constants/__pycache__/openai.cpython-311.pyc
+-rw-r--r--   0        0        0      126 2024-06-03 09:15:32.819250 agiflow_sdk-0.0.5/agiflow/opentelemetry/instrumentation/constants/anthropic.py
+-rw-r--r--   0        0        0      972 2024-06-03 09:15:32.819416 agiflow_sdk-0.0.5/agiflow/opentelemetry/instrumentation/constants/chroma.py
+-rw-r--r--   0        0        0      577 2024-06-03 09:15:32.819620 agiflow_sdk-0.0.5/agiflow/opentelemetry/instrumentation/constants/cohere.py
+-rw-r--r--   0        0        0      750 2024-06-03 09:15:32.819840 agiflow_sdk-0.0.5/agiflow/opentelemetry/instrumentation/constants/common.py
+-rw-r--r--   0        0        0      134 2024-06-03 09:15:32.819980 agiflow_sdk-0.0.5/agiflow/opentelemetry/instrumentation/constants/groq.py
+-rw-r--r--   0        0        0     1054 2024-06-03 09:15:32.820212 agiflow_sdk-0.0.5/agiflow/opentelemetry/instrumentation/constants/openai.py
+-rw-r--r--   0        0        0      490 2024-06-03 09:15:32.820356 agiflow_sdk-0.0.5/agiflow/opentelemetry/instrumentation/constants/pinecone.py
+-rw-r--r--   0        0        0     2016 2024-06-03 09:15:32.820488 agiflow_sdk-0.0.5/agiflow/opentelemetry/instrumentation/constants/qdrant.py
+-rw-r--r--   0        0        0     1518 2024-06-03 09:15:32.820617 agiflow_sdk-0.0.5/agiflow/opentelemetry/instrumentation/constants/weaviate.py
+-rw-r--r--   0        0        0      139 2024-06-03 09:15:32.820870 agiflow_sdk-0.0.5/agiflow/opentelemetry/instrumentation/groq/__init__.py
+-rw-r--r--   0        0        0      156 2024-06-03 09:15:32.821087 agiflow_sdk-0.0.5/agiflow/opentelemetry/instrumentation/groq/hooks/__init__.py
+-rw-r--r--   0        0        0     1934 2024-06-03 09:15:32.821232 agiflow_sdk-0.0.5/agiflow/opentelemetry/instrumentation/groq/hooks/base.py
+-rw-r--r--   0        0        0    12481 2024-06-03 09:15:32.821399 agiflow_sdk-0.0.5/agiflow/opentelemetry/instrumentation/groq/hooks/chat_completion.py
+-rw-r--r--   0        0        0     1993 2024-06-03 09:15:32.821606 agiflow_sdk-0.0.5/agiflow/opentelemetry/instrumentation/groq/instrumentation.py
+-rw-r--r--   0        0        0     6148 2024-06-03 09:15:32.822089 agiflow_sdk-0.0.5/agiflow/opentelemetry/instrumentation/langchain/.DS_Store
+-rw-r--r--   0        0        0      154 2024-06-03 09:15:32.822264 agiflow_sdk-0.0.5/agiflow/opentelemetry/instrumentation/langchain/__init__.py
+-rw-r--r--   0        0        0      398 2024-06-03 09:15:32.822591 agiflow_sdk-0.0.5/agiflow/opentelemetry/instrumentation/langchain/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0     3233 2024-06-03 09:15:32.822886 agiflow_sdk-0.0.5/agiflow/opentelemetry/instrumentation/langchain/__pycache__/instrumentation.cpython-311.pyc
+-rw-r--r--   0        0        0     4136 2024-06-03 09:15:32.823130 agiflow_sdk-0.0.5/agiflow/opentelemetry/instrumentation/langchain/__pycache__/patch.cpython-311.pyc
+-rw-r--r--   0        0        0      252 2024-06-03 09:15:32.823381 agiflow_sdk-0.0.5/agiflow/opentelemetry/instrumentation/langchain/hooks/__init__.py
+-rw-r--r--   0        0        0      532 2024-06-03 09:15:32.823608 agiflow_sdk-0.0.5/agiflow/opentelemetry/instrumentation/langchain/hooks/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0     2313 2024-06-03 09:15:32.823745 agiflow_sdk-0.0.5/agiflow/opentelemetry/instrumentation/langchain/hooks/__pycache__/base.cpython-311.pyc
+-rw-r--r--   0        0        0     7286 2024-06-03 09:15:32.823900 agiflow_sdk-0.0.5/agiflow/opentelemetry/instrumentation/langchain/hooks/__pycache__/chat.cpython-311.pyc
+-rw-r--r--   0        0        0     3122 2024-06-03 09:15:32.824157 agiflow_sdk-0.0.5/agiflow/opentelemetry/instrumentation/langchain/hooks/__pycache__/generic.cpython-311.pyc
+-rw-r--r--   0        0        0     1384 2024-06-03 09:15:32.824315 agiflow_sdk-0.0.5/agiflow/opentelemetry/instrumentation/langchain/hooks/base.py
+-rw-r--r--   0        0        0     5021 2024-06-03 09:15:32.824454 agiflow_sdk-0.0.5/agiflow/opentelemetry/instrumentation/langchain/hooks/chat.py
+-rw-r--r--   0        0        0     1741 2024-06-03 09:15:32.824741 agiflow_sdk-0.0.5/agiflow/opentelemetry/instrumentation/langchain/hooks/generic.py
+-rw-r--r--   0        0        0     2232 2024-06-03 09:15:32.824888 agiflow_sdk-0.0.5/agiflow/opentelemetry/instrumentation/langchain/instrumentation.py
+-rw-r--r--   0        0        0     6148 2024-06-03 09:15:32.825327 agiflow_sdk-0.0.5/agiflow/opentelemetry/instrumentation/langchain_community/.DS_Store
+-rw-r--r--   0        0        0      182 2024-06-03 09:15:32.825467 agiflow_sdk-0.0.5/agiflow/opentelemetry/instrumentation/langchain_community/__init__.py
+-rw-r--r--   0        0        0      427 2024-06-03 09:15:32.825684 agiflow_sdk-0.0.5/agiflow/opentelemetry/instrumentation/langchain_community/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0     3462 2024-06-03 09:15:32.825815 agiflow_sdk-0.0.5/agiflow/opentelemetry/instrumentation/langchain_community/__pycache__/instrumentation.cpython-311.pyc
+-rw-r--r--   0        0        0    11425 2024-06-03 09:15:32.826059 agiflow_sdk-0.0.5/agiflow/opentelemetry/instrumentation/langchain_community/__pycache__/patch.cpython-311.pyc
+-rw-r--r--   0        0        0     6148 2024-06-03 09:15:32.826548 agiflow_sdk-0.0.5/agiflow/opentelemetry/instrumentation/langchain_community/hooks/.DS_Store
+-rw-r--r--   0        0        0      141 2024-06-03 09:15:32.826677 agiflow_sdk-0.0.5/agiflow/opentelemetry/instrumentation/langchain_community/hooks/__init__.py
+-rw-r--r--   0        0        0      404 2024-06-03 09:15:32.826939 agiflow_sdk-0.0.5/agiflow/opentelemetry/instrumentation/langchain_community/hooks/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0     2481 2024-06-03 09:15:32.827084 agiflow_sdk-0.0.5/agiflow/opentelemetry/instrumentation/langchain_community/hooks/__pycache__/base.cpython-311.pyc
+-rw-r--r--   0        0        0     6863 2024-06-03 09:15:32.827296 agiflow_sdk-0.0.5/agiflow/opentelemetry/instrumentation/langchain_community/hooks/__pycache__/chat.cpython-311.pyc
+-rw-r--r--   0        0        0     3163 2024-06-03 09:15:32.827470 agiflow_sdk-0.0.5/agiflow/opentelemetry/instrumentation/langchain_community/hooks/__pycache__/generic.cpython-311.pyc
+-rw-r--r--   0        0        0     5119 2024-06-03 09:15:32.827788 agiflow_sdk-0.0.5/agiflow/opentelemetry/instrumentation/langchain_community/hooks/__pycache__/llm.cpython-311.pyc
+-rw-r--r--   0        0        0     1499 2024-06-03 09:15:32.827928 agiflow_sdk-0.0.5/agiflow/opentelemetry/instrumentation/langchain_community/hooks/base.py
+-rw-r--r--   0        0        0     1769 2024-06-03 09:15:32.828056 agiflow_sdk-0.0.5/agiflow/opentelemetry/instrumentation/langchain_community/hooks/generic.py
+-rw-r--r--   0        0        0     3005 2024-06-03 09:15:32.828205 agiflow_sdk-0.0.5/agiflow/opentelemetry/instrumentation/langchain_community/instrumentation.py
+-rw-r--r--   0        0        0     6148 2024-06-03 09:15:32.828612 agiflow_sdk-0.0.5/agiflow/opentelemetry/instrumentation/langchain_core/.DS_Store
+-rw-r--r--   0        0        0      167 2024-06-03 09:15:32.828745 agiflow_sdk-0.0.5/agiflow/opentelemetry/instrumentation/langchain_core/__init__.py
+-rw-r--r--   0        0        0      412 2024-06-03 09:15:32.828957 agiflow_sdk-0.0.5/agiflow/opentelemetry/instrumentation/langchain_core/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0     3928 2024-06-03 09:15:32.829098 agiflow_sdk-0.0.5/agiflow/opentelemetry/instrumentation/langchain_core/__pycache__/instrumentation.cpython-311.pyc
+-rw-r--r--   0        0        0     8316 2024-06-03 09:15:32.829293 agiflow_sdk-0.0.5/agiflow/opentelemetry/instrumentation/langchain_core/__pycache__/patch.cpython-311.pyc
+-rw-r--r--   0        0        0      390 2024-06-03 09:15:32.829557 agiflow_sdk-0.0.5/agiflow/opentelemetry/instrumentation/langchain_core/hooks/__init__.py
+-rw-r--r--   0        0        0      693 2024-06-03 09:15:32.829781 agiflow_sdk-0.0.5/agiflow/opentelemetry/instrumentation/langchain_core/hooks/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0     2558 2024-06-03 09:15:32.829980 agiflow_sdk-0.0.5/agiflow/opentelemetry/instrumentation/langchain_core/hooks/__pycache__/base.cpython-311.pyc
+-rw-r--r--   0        0        0     3573 2024-06-03 09:15:32.830219 agiflow_sdk-0.0.5/agiflow/opentelemetry/instrumentation/langchain_core/hooks/__pycache__/generic.cpython-311.pyc
+-rw-r--r--   0        0        0     5208 2024-06-03 09:15:32.830396 agiflow_sdk-0.0.5/agiflow/opentelemetry/instrumentation/langchain_core/hooks/__pycache__/llm.cpython-311.pyc
+-rw-r--r--   0        0        0     4692 2024-06-03 09:15:32.830702 agiflow_sdk-0.0.5/agiflow/opentelemetry/instrumentation/langchain_core/hooks/__pycache__/runnable.cpython-311.pyc
+-rw-r--r--   0        0        0     1533 2024-06-03 09:15:32.830945 agiflow_sdk-0.0.5/agiflow/opentelemetry/instrumentation/langchain_core/hooks/base.py
+-rw-r--r--   0        0        0     2152 2024-06-03 09:15:32.831075 agiflow_sdk-0.0.5/agiflow/opentelemetry/instrumentation/langchain_core/hooks/generic.py
+-rw-r--r--   0        0        0     3178 2024-06-03 09:15:32.831256 agiflow_sdk-0.0.5/agiflow/opentelemetry/instrumentation/langchain_core/hooks/llm.py
+-rw-r--r--   0        0        0     3248 2024-06-03 09:15:32.831407 agiflow_sdk-0.0.5/agiflow/opentelemetry/instrumentation/langchain_core/hooks/runnable.py
+-rw-r--r--   0        0        0     3346 2024-06-03 09:15:32.831559 agiflow_sdk-0.0.5/agiflow/opentelemetry/instrumentation/langchain_core/instrumentation.py
+-rw-r--r--   0        0        0      154 2024-06-03 09:15:32.831788 agiflow_sdk-0.0.5/agiflow/opentelemetry/instrumentation/langgraph/__init__.py
+-rw-r--r--   0        0        0      146 2024-06-03 09:15:32.832000 agiflow_sdk-0.0.5/agiflow/opentelemetry/instrumentation/langgraph/hooks/__init__.py
+-rw-r--r--   0        0        0     1343 2024-06-03 09:15:32.832130 agiflow_sdk-0.0.5/agiflow/opentelemetry/instrumentation/langgraph/hooks/base.py
+-rw-r--r--   0        0        0     3352 2024-06-03 09:15:32.832262 agiflow_sdk-0.0.5/agiflow/opentelemetry/instrumentation/langgraph/hooks/graph_call.py
+-rw-r--r--   0        0        0     2873 2024-06-03 09:15:32.832409 agiflow_sdk-0.0.5/agiflow/opentelemetry/instrumentation/langgraph/instrumentation.py
+-rw-r--r--   0        0        0      157 2024-06-03 09:15:32.832631 agiflow_sdk-0.0.5/agiflow/opentelemetry/instrumentation/llamaindex/__init__.py
+-rw-r--r--   0        0        0      140 2024-06-03 09:15:32.832831 agiflow_sdk-0.0.5/agiflow/opentelemetry/instrumentation/llamaindex/hooks/__init__.py
+-rw-r--r--   0        0        0     1347 2024-06-03 09:15:32.832966 agiflow_sdk-0.0.5/agiflow/opentelemetry/instrumentation/llamaindex/hooks/base.py
+-rw-r--r--   0        0        0     1718 2024-06-03 09:15:32.833098 agiflow_sdk-0.0.5/agiflow/opentelemetry/instrumentation/llamaindex/hooks/generic.py
+-rw-r--r--   0        0        0     2944 2024-06-03 09:15:32.833588 agiflow_sdk-0.0.5/agiflow/opentelemetry/instrumentation/llamaindex/instrumentation.py
+-rw-r--r--   0        0        0     6148 2024-06-03 09:15:32.833944 agiflow_sdk-0.0.5/agiflow/opentelemetry/instrumentation/openai/.DS_Store
+-rw-r--r--   0        0        0      145 2024-06-03 09:15:32.834087 agiflow_sdk-0.0.5/agiflow/opentelemetry/instrumentation/openai/__init__.py
+-rw-r--r--   0        0        0      389 2024-06-03 09:15:32.834324 agiflow_sdk-0.0.5/agiflow/opentelemetry/instrumentation/openai/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0     3659 2024-06-03 09:15:32.834465 agiflow_sdk-0.0.5/agiflow/opentelemetry/instrumentation/openai/__pycache__/instrumentation.cpython-311.pyc
+-rw-r--r--   0        0        0    20526 2024-06-03 09:15:32.835216 agiflow_sdk-0.0.5/agiflow/opentelemetry/instrumentation/openai/__pycache__/patch.cpython-311.pyc
+-rw-r--r--   0        0        0     6148 2024-06-03 09:15:32.835735 agiflow_sdk-0.0.5/agiflow/opentelemetry/instrumentation/openai/hooks/.DS_Store
+-rw-r--r--   0        0        0      424 2024-06-03 09:15:32.835883 agiflow_sdk-0.0.5/agiflow/opentelemetry/instrumentation/openai/hooks/__init__.py
+-rw-r--r--   0        0        0      699 2024-06-03 09:15:32.836165 agiflow_sdk-0.0.5/agiflow/opentelemetry/instrumentation/openai/hooks/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0     4035 2024-06-03 09:15:32.836300 agiflow_sdk-0.0.5/agiflow/opentelemetry/instrumentation/openai/hooks/__pycache__/base.cpython-311.pyc
+-rw-r--r--   0        0        0     4744 2024-06-03 09:15:32.836543 agiflow_sdk-0.0.5/agiflow/opentelemetry/instrumentation/openai/hooks/__pycache__/base_llm.cpython-311.pyc
+-rw-r--r--   0        0        0    12171 2024-06-03 09:15:32.836694 agiflow_sdk-0.0.5/agiflow/opentelemetry/instrumentation/openai/hooks/__pycache__/chat_completion.cpython-311.pyc
+-rw-r--r--   0        0        0    11736 2024-06-03 09:15:32.837178 agiflow_sdk-0.0.5/agiflow/opentelemetry/instrumentation/openai/hooks/__pycache__/completion.cpython-311.pyc
+-rw-r--r--   0        0        0     3391 2024-06-03 09:15:32.837387 agiflow_sdk-0.0.5/agiflow/opentelemetry/instrumentation/openai/hooks/__pycache__/embedding.cpython-311.pyc
+-rw-r--r--   0        0        0     3885 2024-06-03 09:15:32.838007 agiflow_sdk-0.0.5/agiflow/opentelemetry/instrumentation/openai/hooks/__pycache__/image_generate.cpython-311.pyc
+-rw-r--r--   0        0        0     2374 2024-06-03 09:15:32.838199 agiflow_sdk-0.0.5/agiflow/opentelemetry/instrumentation/openai/hooks/__pycache__/utils.cpython-311.pyc
+-rw-r--r--   0        0        0     2474 2024-06-03 09:15:32.838370 agiflow_sdk-0.0.5/agiflow/opentelemetry/instrumentation/openai/hooks/base.py
+-rw-r--r--   0        0        0     3115 2024-06-03 09:15:32.838620 agiflow_sdk-0.0.5/agiflow/opentelemetry/instrumentation/openai/hooks/base_llm.py
+-rw-r--r--   0        0        0    10648 2024-06-03 09:15:32.838789 agiflow_sdk-0.0.5/agiflow/opentelemetry/instrumentation/openai/hooks/chat_completion.py
+-rw-r--r--   0        0        0     2257 2024-06-03 09:15:32.839139 agiflow_sdk-0.0.5/agiflow/opentelemetry/instrumentation/openai/hooks/embedding.py
+-rw-r--r--   0        0        0     2555 2024-06-03 09:15:32.839337 agiflow_sdk-0.0.5/agiflow/opentelemetry/instrumentation/openai/hooks/image_generate.py
+-rw-r--r--   0        0        0     2211 2024-06-03 09:15:32.839521 agiflow_sdk-0.0.5/agiflow/opentelemetry/instrumentation/openai/hooks/utils.py
+-rw-r--r--   0        0        0     2910 2024-06-03 09:15:32.839717 agiflow_sdk-0.0.5/agiflow/opentelemetry/instrumentation/openai/instrumentation.py
+-rw-r--r--   0        0        0      151 2024-06-03 09:15:32.840110 agiflow_sdk-0.0.5/agiflow/opentelemetry/instrumentation/pinecone/__init__.py
+-rw-r--r--   0        0        0      137 2024-06-03 09:15:32.840393 agiflow_sdk-0.0.5/agiflow/opentelemetry/instrumentation/pinecone/hooks/__init__.py
+-rw-r--r--   0        0        0     1396 2024-06-03 09:15:32.840570 agiflow_sdk-0.0.5/agiflow/opentelemetry/instrumentation/pinecone/hooks/base.py
+-rw-r--r--   0        0        0     6892 2024-06-03 09:15:32.840759 agiflow_sdk-0.0.5/agiflow/opentelemetry/instrumentation/pinecone/hooks/generic.py
+-rw-r--r--   0        0        0     2019 2024-06-03 09:15:32.840949 agiflow_sdk-0.0.5/agiflow/opentelemetry/instrumentation/pinecone/instrumentation.py
+-rw-r--r--   0        0        0      145 2024-06-03 09:15:32.841217 agiflow_sdk-0.0.5/agiflow/opentelemetry/instrumentation/qdrant/__init__.py
+-rw-r--r--   0        0        0      152 2024-06-03 09:15:32.841490 agiflow_sdk-0.0.5/agiflow/opentelemetry/instrumentation/qdrant/hooks/__init__.py
+-rw-r--r--   0        0        0     1388 2024-06-03 09:15:32.841667 agiflow_sdk-0.0.5/agiflow/opentelemetry/instrumentation/qdrant/hooks/base.py
+-rw-r--r--   0        0        0     3113 2024-06-03 09:15:32.841839 agiflow_sdk-0.0.5/agiflow/opentelemetry/instrumentation/qdrant/hooks/collection.py
+-rw-r--r--   0        0        0     1913 2024-06-03 09:15:32.842097 agiflow_sdk-0.0.5/agiflow/opentelemetry/instrumentation/qdrant/instrumentation.py
+-rw-r--r--   0        0        0     2309 2024-06-03 09:15:32.842404 agiflow_sdk-0.0.5/agiflow/opentelemetry/instrumentation/utils/__init__.py
+-rw-r--r--   0        0        0     2790 2024-06-03 09:15:32.842839 agiflow_sdk-0.0.5/agiflow/opentelemetry/instrumentation/utils/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0    17396 2024-06-03 09:15:32.843262 agiflow_sdk-0.0.5/agiflow/opentelemetry/instrumentation/utils/__pycache__/wrapper.cpython-311.pyc
+-rw-r--r--   0        0        0    11559 2024-06-03 09:15:32.843557 agiflow_sdk-0.0.5/agiflow/opentelemetry/instrumentation/utils/wrapper.py
+-rw-r--r--   0        0        0      151 2024-06-03 09:15:32.843983 agiflow_sdk-0.0.5/agiflow/opentelemetry/instrumentation/weaviate/__init__.py
+-rw-r--r--   0        0        0      306 2024-06-03 09:15:32.844245 agiflow_sdk-0.0.5/agiflow/opentelemetry/instrumentation/weaviate/hooks/__init__.py
+-rw-r--r--   0        0        0     1396 2024-06-03 09:15:32.844390 agiflow_sdk-0.0.5/agiflow/opentelemetry/instrumentation/weaviate/hooks/base.py
+-rw-r--r--   0        0        0     1776 2024-06-03 09:15:32.844546 agiflow_sdk-0.0.5/agiflow/opentelemetry/instrumentation/weaviate/hooks/generic_collection.py
+-rw-r--r--   0        0        0     4091 2024-06-03 09:15:32.844753 agiflow_sdk-0.0.5/agiflow/opentelemetry/instrumentation/weaviate/hooks/generic_query.py
+-rw-r--r--   0        0        0     2754 2024-06-03 09:15:32.844963 agiflow_sdk-0.0.5/agiflow/opentelemetry/instrumentation/weaviate/instrumentation.py
+-rw-r--r--   0        0        0      144 2024-06-03 09:15:32.845268 agiflow_sdk-0.0.5/agiflow/opentelemetry/span_processors/__init__.py
+-rw-r--r--   0        0        0      376 2024-06-03 09:15:32.845647 agiflow_sdk-0.0.5/agiflow/opentelemetry/span_processors/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0     5123 2024-06-03 09:15:32.845938 agiflow_sdk-0.0.5/agiflow/opentelemetry/span_processors/__pycache__/thread_pool_span_processor.cpython-311.pyc
+-rw-r--r--   0        0        0     2544 2024-06-03 09:15:32.846182 agiflow_sdk-0.0.5/agiflow/opentelemetry/span_processors/thread_pool_span_processor.py
+-rw-r--r--   0        0        0      644 2024-06-03 09:15:32.846408 agiflow_sdk-0.0.5/agiflow/opentelemetry/trace_decorators/__init__.py
+-rw-r--r--   0        0        0      910 2024-06-03 09:15:32.846702 agiflow_sdk-0.0.5/agiflow/opentelemetry/trace_decorators/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0     1383 2024-06-03 09:15:32.846935 agiflow_sdk-0.0.5/agiflow/opentelemetry/trace_decorators/__pycache__/helper.cpython-311.pyc
+-rw-r--r--   0        0        0     4660 2024-06-03 09:15:32.847152 agiflow_sdk-0.0.5/agiflow/opentelemetry/trace_decorators/__pycache__/task.cpython-311.pyc
+-rw-r--r--   0        0        0     3296 2024-06-03 09:15:32.847372 agiflow_sdk-0.0.5/agiflow/opentelemetry/trace_decorators/__pycache__/workflow.cpython-311.pyc
+-rw-r--r--   0        0        0    19223 2024-06-03 09:15:32.847618 agiflow_sdk-0.0.5/agiflow/opentelemetry/trace_decorators/__pycache__/wrapper.cpython-311.pyc
+-rw-r--r--   0        0        0     1650 2024-06-03 09:15:32.847877 agiflow_sdk-0.0.5/agiflow/opentelemetry/trace_decorators/helper.py
+-rw-r--r--   0        0        0     3964 2024-06-03 09:15:32.848098 agiflow_sdk-0.0.5/agiflow/opentelemetry/trace_decorators/task.py
+-rw-r--r--   0        0        0     2294 2024-06-03 09:15:32.848303 agiflow_sdk-0.0.5/agiflow/opentelemetry/trace_decorators/workflow.py
+-rw-r--r--   0        0        0    15148 2024-06-03 09:15:32.848545 agiflow_sdk-0.0.5/agiflow/opentelemetry/trace_decorators/wrapper.py
+-rw-r--r--   0        0        0      115 2024-06-03 09:15:32.848929 agiflow_sdk-0.0.5/agiflow/opentelemetry/trace_exporter/__init__.py
+-rw-r--r--   0        0        0      349 2024-06-03 09:15:32.849275 agiflow_sdk-0.0.5/agiflow/opentelemetry/trace_exporter/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0     2687 2024-06-03 09:15:32.849513 agiflow_sdk-0.0.5/agiflow/opentelemetry/trace_exporter/__pycache__/config.cpython-311.pyc
+-rw-r--r--   0        0        0     9661 2024-06-03 09:15:32.849769 agiflow_sdk-0.0.5/agiflow/opentelemetry/trace_exporter/__pycache__/json.cpython-311.pyc
+-rw-r--r--   0        0        0      238 2024-06-03 09:15:32.849949 agiflow_sdk-0.0.5/agiflow/opentelemetry/trace_exporter/__pycache__/version.cpython-311.pyc
+-rw-r--r--   0        0        0     2757 2024-06-03 09:15:32.850252 agiflow_sdk-0.0.5/agiflow/opentelemetry/trace_exporter/config.py
+-rw-r--r--   0        0        0     7123 2024-06-03 09:15:32.850525 agiflow_sdk-0.0.5/agiflow/opentelemetry/trace_exporter/json.py
+-rw-r--r--   0        0        0       22 2024-06-03 09:15:32.850684 agiflow_sdk-0.0.5/agiflow/opentelemetry/trace_exporter/version.py
+-rw-r--r--   0        0        0       99 2024-06-03 09:15:32.851035 agiflow_sdk-0.0.5/agiflow/opentelemetry/trace_sampler/__init__.py
+-rw-r--r--   0        0        0      342 2024-06-03 09:15:32.851374 agiflow_sdk-0.0.5/agiflow/opentelemetry/trace_sampler/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0     1787 2024-06-03 09:15:32.851668 agiflow_sdk-0.0.5/agiflow/opentelemetry/trace_sampler/__pycache__/no_sampler.cpython-311.pyc
+-rw-r--r--   0        0        0      862 2024-06-03 09:15:32.851916 agiflow_sdk-0.0.5/agiflow/opentelemetry/trace_sampler/no_sampler.py
+-rw-r--r--   0        0        0     3160 2024-06-03 09:15:32.852301 agiflow_sdk-0.0.5/agiflow/opentelemetry/trace_store.py
+-rw-r--r--   0        0        0     6148 2024-06-03 09:15:32.852817 agiflow_sdk-0.0.5/agiflow/opentelemetry/tracing/.DS_Store
+-rw-r--r--   0        0        0      182 2024-06-03 09:15:32.853034 agiflow_sdk-0.0.5/agiflow/opentelemetry/tracing/__init__.py
+-rw-r--r--   0        0        0      437 2024-06-03 09:15:32.853390 agiflow_sdk-0.0.5/agiflow/opentelemetry/tracing/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0     1979 2024-06-03 09:15:32.853659 agiflow_sdk-0.0.5/agiflow/opentelemetry/tracing/__pycache__/content_allow_list.cpython-311.pyc
+-rw-r--r--   0        0        0     1978 2024-06-03 09:15:32.853865 agiflow_sdk-0.0.5/agiflow/opentelemetry/tracing/__pycache__/content_alow_list.cpython-311.pyc
+-rw-r--r--   0        0        0     5230 2024-06-03 09:15:32.854048 agiflow_sdk-0.0.5/agiflow/opentelemetry/tracing/__pycache__/context.cpython-311.pyc
+-rw-r--r--   0        0        0      897 2024-06-03 09:15:32.854302 agiflow_sdk-0.0.5/agiflow/opentelemetry/tracing/__pycache__/context_manager.cpython-311.pyc
+-rw-r--r--   0        0        0     1507 2024-06-03 09:15:32.854558 agiflow_sdk-0.0.5/agiflow/opentelemetry/tracing/__pycache__/context_propagation.cpython-311.pyc
+-rw-r--r--   0        0        0     2581 2024-06-03 09:15:32.854828 agiflow_sdk-0.0.5/agiflow/opentelemetry/tracing/__pycache__/span_from_context.cpython-311.pyc
+-rw-r--r--   0        0        0    10065 2024-06-03 09:15:32.855086 agiflow_sdk-0.0.5/agiflow/opentelemetry/tracing/__pycache__/tracing.cpython-311.pyc
+-rw-r--r--   0        0        0      846 2024-06-03 09:15:32.855343 agiflow_sdk-0.0.5/agiflow/opentelemetry/tracing/content_allow_list.py
+-rw-r--r--   0        0        0      307 2024-06-03 09:15:32.855603 agiflow_sdk-0.0.5/agiflow/opentelemetry/tracing/context_manager.py
+-rw-r--r--   0        0        0     7265 2024-06-03 09:15:32.855854 agiflow_sdk-0.0.5/agiflow/opentelemetry/tracing/tracing.py
+-rw-r--r--   0        0        0      813 2024-06-03 09:15:32.856241 agiflow_sdk-0.0.5/agiflow/opentelemetry/types/__init__.py
+-rw-r--r--   0        0        0     1865 2024-06-03 09:15:32.856620 agiflow_sdk-0.0.5/agiflow/opentelemetry/types/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0     6148 2024-06-03 09:15:32.857044 agiflow_sdk-0.0.5/agiflow/opentelemetry/utils/.DS_Store
+-rw-r--r--   0        0        0      340 2024-06-03 09:15:32.857212 agiflow_sdk-0.0.5/agiflow/opentelemetry/utils/__init__.py
+-rw-r--r--   0        0        0      521 2024-06-03 09:15:32.857579 agiflow_sdk-0.0.5/agiflow/opentelemetry/utils/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0     3447 2024-06-03 09:15:32.857951 agiflow_sdk-0.0.5/agiflow/opentelemetry/utils/__pycache__/llm.cpython-311.pyc
+-rw-r--r--   0        0        0     2240 2024-06-03 09:15:32.858126 agiflow_sdk-0.0.5/agiflow/opentelemetry/utils/llm.py
+-rw-r--r--   0        0        0       71 2024-06-03 09:15:32.858415 agiflow_sdk-0.0.5/agiflow/services/__init__.py
+-rw-r--r--   0        0        0      297 2024-06-03 09:15:32.858630 agiflow_sdk-0.0.5/agiflow/services/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0     5452 2024-06-03 09:15:32.858769 agiflow_sdk-0.0.5/agiflow/services/__pycache__/fetch.cpython-311.pyc
+-rw-r--r--   0        0        0     2731 2024-06-03 09:15:32.858918 agiflow_sdk-0.0.5/agiflow/services/fetch.py
+-rw-r--r--   0        0        0     2522 2024-06-03 09:15:32.859183 agiflow_sdk-0.0.5/agiflow/telemetry/__init__.py
+-rw-r--r--   0        0        0     4829 2024-06-03 09:15:32.859433 agiflow_sdk-0.0.5/agiflow/telemetry/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0     6148 2024-06-03 09:15:32.859890 agiflow_sdk-0.0.5/agiflow/utils/.DS_Store
+-rw-r--r--   0        0        0      444 2024-06-03 09:15:32.860042 agiflow_sdk-0.0.5/agiflow/utils/__init__.py
+-rw-r--r--   0        0        0      728 2024-06-03 09:15:32.860259 agiflow_sdk-0.0.5/agiflow/utils/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0      532 2024-06-03 09:15:32.860487 agiflow_sdk-0.0.5/agiflow/utils/__pycache__/assertion.cpython-311.pyc
+-rw-r--r--   0        0        0     1923 2024-06-03 09:15:32.860641 agiflow_sdk-0.0.5/agiflow/utils/__pycache__/debugging.cpython-311.pyc
+-rw-r--r--   0        0        0     1719 2024-06-03 09:15:32.860788 agiflow_sdk-0.0.5/agiflow/utils/__pycache__/error.cpython-311.pyc
+-rw-r--r--   0        0        0     3268 2024-06-03 09:15:32.861016 agiflow_sdk-0.0.5/agiflow/utils/__pycache__/llm.cpython-311.pyc
+-rw-r--r--   0        0        0     4718 2024-06-03 09:15:32.861165 agiflow_sdk-0.0.5/agiflow/utils/__pycache__/string.cpython-311.pyc
+-rw-r--r--   0        0        0      583 2024-06-03 09:15:32.861308 agiflow_sdk-0.0.5/agiflow/utils/__pycache__/time.cpython-311.pyc
+-rw-r--r--   0        0        0      207 2024-06-03 09:15:32.861599 agiflow_sdk-0.0.5/agiflow/utils/assertion.py
+-rw-r--r--   0        0        0      580 2024-06-03 09:15:32.861736 agiflow_sdk-0.0.5/agiflow/utils/debugging.py
+-rw-r--r--   0        0        0      847 2024-06-03 09:15:32.861875 agiflow_sdk-0.0.5/agiflow/utils/error.py
+-rw-r--r--   0        0        0     1965 2024-06-03 09:15:32.862037 agiflow_sdk-0.0.5/agiflow/utils/string.py
+-rw-r--r--   0        0        0      264 2024-06-03 09:15:32.862186 agiflow_sdk-0.0.5/agiflow/utils/time.py
+-rw-r--r--   0        0        0       22 2024-06-03 09:15:32.862494 agiflow_sdk-0.0.5/agiflow/version.py
+-rw-r--r--   0        0        0     1106 2024-06-03 09:15:32.870352 agiflow_sdk-0.0.5/pyproject.toml
+-rw-r--r--   0        0        0     1760 1970-01-01 00:00:00.000000 agiflow_sdk-0.0.5/PKG-INFO
```

### Comparing `agiflow_sdk-0.0.4/agiflow/agiflow.py` & `agiflow_sdk-0.0.5/agiflow/agiflow.py`

 * *Files identical despite different names*

### Comparing `agiflow_sdk-0.0.4/agiflow/config/__init__.py` & `agiflow_sdk-0.0.5/agiflow/config/__init__.py`

 * *Files identical despite different names*

### Comparing `agiflow_sdk-0.0.4/agiflow/config/__pycache__/__init__.cpython-311.pyc` & `agiflow_sdk-0.0.5/agiflow/config/__pycache__/__init__.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `agiflow_sdk-0.0.4/agiflow/config/__pycache__/environment_vars.cpython-311.pyc` & `agiflow_sdk-0.0.5/agiflow/config/__pycache__/environment_vars.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `agiflow_sdk-0.0.4/agiflow/config/environment_vars.py` & `agiflow_sdk-0.0.5/agiflow/config/environment_vars.py`

 * *Files identical despite different names*

### Comparing `agiflow_sdk-0.0.4/agiflow/opentelemetry/.DS_Store` & `agiflow_sdk-0.0.5/agiflow/opentelemetry/.DS_Store`

 * *Files identical despite different names*

### Comparing `agiflow_sdk-0.0.4/agiflow/opentelemetry/__init__.py` & `agiflow_sdk-0.0.5/agiflow/opentelemetry/__init__.py`

 * *Files identical despite different names*

### Comparing `agiflow_sdk-0.0.4/agiflow/opentelemetry/__pycache__/__init__.cpython-311.pyc` & `agiflow_sdk-0.0.5/agiflow/opentelemetry/__pycache__/__init__.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `agiflow_sdk-0.0.4/agiflow/opentelemetry/__pycache__/trace_store.cpython-311.pyc` & `agiflow_sdk-0.0.5/agiflow/opentelemetry/__pycache__/trace_store.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `agiflow_sdk-0.0.4/agiflow/opentelemetry/context/__init__.py` & `agiflow_sdk-0.0.5/agiflow/opentelemetry/context/__init__.py`

 * *Files identical despite different names*

### Comparing `agiflow_sdk-0.0.4/agiflow/opentelemetry/context/__pycache__/__init__.cpython-311.pyc` & `agiflow_sdk-0.0.5/agiflow/opentelemetry/context/__pycache__/__init__.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `agiflow_sdk-0.0.4/agiflow/opentelemetry/context/__pycache__/constants.cpython-311.pyc` & `agiflow_sdk-0.0.5/agiflow/opentelemetry/context/__pycache__/constants.cpython-311.pyc`

 * *Files 15% similar despite different names*

#### Python bytecode

```diff
@@ -1,9 +1,9 @@
 magic:    0xa70d0d0a
-moddate:  0x6a425c66 (Sun Jun  2 09:59:06 2024 UTC)
+moddate:  0x2f885d66 (Mon Jun  3 09:09:03 2024 UTC)
 files sz: 740
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 5
    flags     : 0
    code
```

### Comparing `agiflow_sdk-0.0.4/agiflow/opentelemetry/context/__pycache__/context.cpython-311.pyc` & `agiflow_sdk-0.0.5/agiflow/opentelemetry/context/__pycache__/context.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `agiflow_sdk-0.0.4/agiflow/opentelemetry/context/__pycache__/context_propagation.cpython-311.pyc` & `agiflow_sdk-0.0.5/agiflow/opentelemetry/context/__pycache__/context_propagation.cpython-311.pyc`

 * *Files 1% similar despite different names*

#### Python bytecode

```diff
@@ -1,9 +1,9 @@
 magic:    0xa70d0d0a
-moddate:  0x6a425c66 (Sun Jun  2 09:59:06 2024 UTC)
+moddate:  0x2f885d66 (Mon Jun  3 09:09:03 2024 UTC)
 files sz: 2139
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 2
    flags     : 0
    code
```

### Comparing `agiflow_sdk-0.0.4/agiflow/opentelemetry/context/__pycache__/set_span_from_context.cpython-311.pyc` & `agiflow_sdk-0.0.5/agiflow/opentelemetry/context/__pycache__/set_span_from_context.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `agiflow_sdk-0.0.4/agiflow/opentelemetry/context/__pycache__/span_from_context.cpython-311.pyc` & `agiflow_sdk-0.0.5/agiflow/opentelemetry/context/__pycache__/span_from_context.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `agiflow_sdk-0.0.4/agiflow/opentelemetry/context/constants.py` & `agiflow_sdk-0.0.5/agiflow/opentelemetry/context/constants.py`

 * *Files identical despite different names*

### Comparing `agiflow_sdk-0.0.4/agiflow/opentelemetry/context/context.py` & `agiflow_sdk-0.0.5/agiflow/opentelemetry/context/context.py`

 * *Files identical despite different names*

### Comparing `agiflow_sdk-0.0.4/agiflow/opentelemetry/context/context_propagation.py` & `agiflow_sdk-0.0.5/agiflow/opentelemetry/context/context_propagation.py`

 * *Files identical despite different names*

### Comparing `agiflow_sdk-0.0.4/agiflow/opentelemetry/context/span_from_context.py` & `agiflow_sdk-0.0.5/agiflow/opentelemetry/context/span_from_context.py`

 * *Files identical despite different names*

### Comparing `agiflow_sdk-0.0.4/agiflow/opentelemetry/convention/__init__.py` & `agiflow_sdk-0.0.5/agiflow/opentelemetry/convention/__init__.py`

 * *Files identical despite different names*

### Comparing `agiflow_sdk-0.0.4/agiflow/opentelemetry/convention/__pycache__/__init__.cpython-311.pyc` & `agiflow_sdk-0.0.5/agiflow/opentelemetry/convention/__pycache__/__init__.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `agiflow_sdk-0.0.4/agiflow/opentelemetry/convention/__pycache__/agiflow_attributes.cpython-311.pyc` & `agiflow_sdk-0.0.5/agiflow/opentelemetry/convention/__pycache__/agiflow_attributes.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `agiflow_sdk-0.0.4/agiflow/opentelemetry/convention/__pycache__/constants.cpython-311.pyc` & `agiflow_sdk-0.0.5/agiflow/opentelemetry/convention/__pycache__/constants.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `agiflow_sdk-0.0.4/agiflow/opentelemetry/convention/__pycache__/database_span_attributes.cpython-311.pyc` & `agiflow_sdk-0.0.5/agiflow/opentelemetry/convention/__pycache__/database_span_attributes.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `agiflow_sdk-0.0.4/agiflow/opentelemetry/convention/__pycache__/framework_span_attributes.cpython-311.pyc` & `agiflow_sdk-0.0.5/agiflow/opentelemetry/convention/__pycache__/framework_span_attributes.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `agiflow_sdk-0.0.4/agiflow/opentelemetry/convention/__pycache__/llm_span_attributes.cpython-311.pyc` & `agiflow_sdk-0.0.5/agiflow/opentelemetry/convention/__pycache__/llm_span_attributes.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `agiflow_sdk-0.0.4/agiflow/opentelemetry/convention/agiflow_attributes.py` & `agiflow_sdk-0.0.5/agiflow/opentelemetry/convention/agiflow_attributes.py`

 * *Files identical despite different names*

### Comparing `agiflow_sdk-0.0.4/agiflow/opentelemetry/convention/constants.py` & `agiflow_sdk-0.0.5/agiflow/opentelemetry/convention/constants.py`

 * *Files identical despite different names*

### Comparing `agiflow_sdk-0.0.4/agiflow/opentelemetry/convention/database_span_attributes.py` & `agiflow_sdk-0.0.5/agiflow/opentelemetry/convention/database_span_attributes.py`

 * *Files identical despite different names*

### Comparing `agiflow_sdk-0.0.4/agiflow/opentelemetry/convention/framework_span_attributes.py` & `agiflow_sdk-0.0.5/agiflow/opentelemetry/convention/framework_span_attributes.py`

 * *Files identical despite different names*

### Comparing `agiflow_sdk-0.0.4/agiflow/opentelemetry/convention/llm_span_attributes.py` & `agiflow_sdk-0.0.5/agiflow/opentelemetry/convention/llm_span_attributes.py`

 * *Files identical despite different names*

### Comparing `agiflow_sdk-0.0.4/agiflow/opentelemetry/instrumentation/__init__.py` & `agiflow_sdk-0.0.5/agiflow/opentelemetry/instrumentation/__init__.py`

 * *Files identical despite different names*

### Comparing `agiflow_sdk-0.0.4/agiflow/opentelemetry/instrumentation/__pycache__/__init__.cpython-311.pyc` & `agiflow_sdk-0.0.5/agiflow/opentelemetry/instrumentation/__pycache__/__init__.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `agiflow_sdk-0.0.4/agiflow/opentelemetry/instrumentation/anthropic/__pycache__/instrumentation.cpython-311.pyc` & `agiflow_sdk-0.0.5/agiflow/opentelemetry/instrumentation/anthropic/__pycache__/instrumentation.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `agiflow_sdk-0.0.4/agiflow/opentelemetry/instrumentation/anthropic/hooks/__pycache__/base.cpython-311.pyc` & `agiflow_sdk-0.0.5/agiflow/opentelemetry/instrumentation/anthropic/hooks/__pycache__/base.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `agiflow_sdk-0.0.4/agiflow/opentelemetry/instrumentation/anthropic/hooks/__pycache__/message_create.cpython-311.pyc` & `agiflow_sdk-0.0.5/agiflow/opentelemetry/instrumentation/anthropic/hooks/__pycache__/message_create.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `agiflow_sdk-0.0.4/agiflow/opentelemetry/instrumentation/anthropic/hooks/base.py` & `agiflow_sdk-0.0.5/agiflow/opentelemetry/instrumentation/anthropic/hooks/base.py`

 * *Files identical despite different names*

### Comparing `agiflow_sdk-0.0.4/agiflow/opentelemetry/instrumentation/anthropic/hooks/message_create.py` & `agiflow_sdk-0.0.5/agiflow/opentelemetry/instrumentation/anthropic/hooks/message_create.py`

 * *Files identical despite different names*

### Comparing `agiflow_sdk-0.0.4/agiflow/opentelemetry/instrumentation/anthropic/instrumentation.py` & `agiflow_sdk-0.0.5/agiflow/opentelemetry/instrumentation/anthropic/instrumentation.py`

 * *Files identical despite different names*

### Comparing `agiflow_sdk-0.0.4/agiflow/opentelemetry/instrumentation/chroma/__pycache__/instrumentation.cpython-311.pyc` & `agiflow_sdk-0.0.5/agiflow/opentelemetry/instrumentation/chroma/__pycache__/instrumentation.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `agiflow_sdk-0.0.4/agiflow/opentelemetry/instrumentation/chroma/hooks/__pycache__/base.cpython-311.pyc` & `agiflow_sdk-0.0.5/agiflow/opentelemetry/instrumentation/chroma/hooks/__pycache__/base.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `agiflow_sdk-0.0.4/agiflow/opentelemetry/instrumentation/chroma/hooks/__pycache__/collection_call.cpython-311.pyc` & `agiflow_sdk-0.0.5/agiflow/opentelemetry/instrumentation/chroma/hooks/__pycache__/collection_call.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `agiflow_sdk-0.0.4/agiflow/opentelemetry/instrumentation/chroma/hooks/base.py` & `agiflow_sdk-0.0.5/agiflow/opentelemetry/instrumentation/chroma/hooks/base.py`

 * *Files identical despite different names*

### Comparing `agiflow_sdk-0.0.4/agiflow/opentelemetry/instrumentation/chroma/hooks/collection_call.py` & `agiflow_sdk-0.0.5/agiflow/opentelemetry/instrumentation/chroma/hooks/collection_call.py`

 * *Files identical despite different names*

### Comparing `agiflow_sdk-0.0.4/agiflow/opentelemetry/instrumentation/chroma/instrumentation.py` & `agiflow_sdk-0.0.5/agiflow/opentelemetry/instrumentation/chroma/instrumentation.py`

 * *Files identical despite different names*

### Comparing `agiflow_sdk-0.0.4/agiflow/opentelemetry/instrumentation/cohere/__pycache__/instrumentation.cpython-311.pyc` & `agiflow_sdk-0.0.5/agiflow/opentelemetry/instrumentation/cohere/__pycache__/instrumentation.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `agiflow_sdk-0.0.4/agiflow/opentelemetry/instrumentation/cohere/hooks/__pycache__/__init__.cpython-311.pyc` & `agiflow_sdk-0.0.5/agiflow/opentelemetry/instrumentation/cohere/hooks/__pycache__/__init__.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `agiflow_sdk-0.0.4/agiflow/opentelemetry/instrumentation/cohere/hooks/__pycache__/base.cpython-311.pyc` & `agiflow_sdk-0.0.5/agiflow/opentelemetry/instrumentation/cohere/hooks/__pycache__/base.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `agiflow_sdk-0.0.4/agiflow/opentelemetry/instrumentation/cohere/hooks/__pycache__/base_chat.cpython-311.pyc` & `agiflow_sdk-0.0.5/agiflow/opentelemetry/instrumentation/cohere/hooks/__pycache__/base_chat.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `agiflow_sdk-0.0.4/agiflow/opentelemetry/instrumentation/cohere/hooks/__pycache__/chat_create.cpython-311.pyc` & `agiflow_sdk-0.0.5/agiflow/opentelemetry/instrumentation/cohere/hooks/__pycache__/chat_create.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `agiflow_sdk-0.0.4/agiflow/opentelemetry/instrumentation/cohere/hooks/__pycache__/chat_stream.cpython-311.pyc` & `agiflow_sdk-0.0.5/agiflow/opentelemetry/instrumentation/cohere/hooks/__pycache__/chat_stream.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `agiflow_sdk-0.0.4/agiflow/opentelemetry/instrumentation/cohere/hooks/__pycache__/embed.cpython-311.pyc` & `agiflow_sdk-0.0.5/agiflow/opentelemetry/instrumentation/cohere/hooks/__pycache__/embed.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `agiflow_sdk-0.0.4/agiflow/opentelemetry/instrumentation/cohere/hooks/__pycache__/rerank.cpython-311.pyc` & `agiflow_sdk-0.0.5/agiflow/opentelemetry/instrumentation/cohere/hooks/__pycache__/rerank.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `agiflow_sdk-0.0.4/agiflow/opentelemetry/instrumentation/cohere/hooks/base.py` & `agiflow_sdk-0.0.5/agiflow/opentelemetry/instrumentation/cohere/hooks/base.py`

 * *Files identical despite different names*

### Comparing `agiflow_sdk-0.0.4/agiflow/opentelemetry/instrumentation/cohere/hooks/base_chat.py` & `agiflow_sdk-0.0.5/agiflow/opentelemetry/instrumentation/cohere/hooks/base_chat.py`

 * *Files identical despite different names*

### Comparing `agiflow_sdk-0.0.4/agiflow/opentelemetry/instrumentation/cohere/hooks/chat_create.py` & `agiflow_sdk-0.0.5/agiflow/opentelemetry/instrumentation/cohere/hooks/chat_create.py`

 * *Files identical despite different names*

### Comparing `agiflow_sdk-0.0.4/agiflow/opentelemetry/instrumentation/cohere/hooks/chat_stream.py` & `agiflow_sdk-0.0.5/agiflow/opentelemetry/instrumentation/cohere/hooks/chat_stream.py`

 * *Files identical despite different names*

### Comparing `agiflow_sdk-0.0.4/agiflow/opentelemetry/instrumentation/cohere/hooks/embed.py` & `agiflow_sdk-0.0.5/agiflow/opentelemetry/instrumentation/cohere/hooks/embed.py`

 * *Files identical despite different names*

### Comparing `agiflow_sdk-0.0.4/agiflow/opentelemetry/instrumentation/cohere/hooks/rerank.py` & `agiflow_sdk-0.0.5/agiflow/opentelemetry/instrumentation/cohere/hooks/rerank.py`

 * *Files identical despite different names*

### Comparing `agiflow_sdk-0.0.4/agiflow/opentelemetry/instrumentation/cohere/instrumentation.py` & `agiflow_sdk-0.0.5/agiflow/opentelemetry/instrumentation/cohere/instrumentation.py`

 * *Files identical despite different names*

### Comparing `agiflow_sdk-0.0.4/agiflow/opentelemetry/instrumentation/constants/__pycache__/__init__.cpython-311.pyc` & `agiflow_sdk-0.0.5/agiflow/opentelemetry/instrumentation/constants/__pycache__/__init__.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `agiflow_sdk-0.0.4/agiflow/opentelemetry/instrumentation/constants/__pycache__/chroma.cpython-311.pyc` & `agiflow_sdk-0.0.5/agiflow/opentelemetry/instrumentation/constants/__pycache__/chroma.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `agiflow_sdk-0.0.4/agiflow/opentelemetry/instrumentation/constants/__pycache__/cohere.cpython-311.pyc` & `agiflow_sdk-0.0.5/agiflow/opentelemetry/instrumentation/constants/__pycache__/cohere.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `agiflow_sdk-0.0.4/agiflow/opentelemetry/instrumentation/constants/__pycache__/common.cpython-311.pyc` & `agiflow_sdk-0.0.5/agiflow/opentelemetry/instrumentation/constants/__pycache__/common.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `agiflow_sdk-0.0.4/agiflow/opentelemetry/instrumentation/constants/__pycache__/openai.cpython-311.pyc` & `agiflow_sdk-0.0.5/agiflow/opentelemetry/instrumentation/constants/__pycache__/openai.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `agiflow_sdk-0.0.4/agiflow/opentelemetry/instrumentation/constants/chroma.py` & `agiflow_sdk-0.0.5/agiflow/opentelemetry/instrumentation/constants/chroma.py`

 * *Files identical despite different names*

### Comparing `agiflow_sdk-0.0.4/agiflow/opentelemetry/instrumentation/constants/cohere.py` & `agiflow_sdk-0.0.5/agiflow/opentelemetry/instrumentation/constants/cohere.py`

 * *Files identical despite different names*

### Comparing `agiflow_sdk-0.0.4/agiflow/opentelemetry/instrumentation/constants/common.py` & `agiflow_sdk-0.0.5/agiflow/opentelemetry/instrumentation/constants/common.py`

 * *Files identical despite different names*

### Comparing `agiflow_sdk-0.0.4/agiflow/opentelemetry/instrumentation/constants/openai.py` & `agiflow_sdk-0.0.5/agiflow/opentelemetry/instrumentation/constants/openai.py`

 * *Files identical despite different names*

### Comparing `agiflow_sdk-0.0.4/agiflow/opentelemetry/instrumentation/constants/qdrant.py` & `agiflow_sdk-0.0.5/agiflow/opentelemetry/instrumentation/constants/qdrant.py`

 * *Files identical despite different names*

### Comparing `agiflow_sdk-0.0.4/agiflow/opentelemetry/instrumentation/constants/weaviate.py` & `agiflow_sdk-0.0.5/agiflow/opentelemetry/instrumentation/constants/weaviate.py`

 * *Files identical despite different names*

### Comparing `agiflow_sdk-0.0.4/agiflow/opentelemetry/instrumentation/groq/hooks/base.py` & `agiflow_sdk-0.0.5/agiflow/opentelemetry/instrumentation/groq/hooks/base.py`

 * *Files identical despite different names*

### Comparing `agiflow_sdk-0.0.4/agiflow/opentelemetry/instrumentation/groq/hooks/chat_completion.py` & `agiflow_sdk-0.0.5/agiflow/opentelemetry/instrumentation/groq/hooks/chat_completion.py`

 * *Files identical despite different names*

### Comparing `agiflow_sdk-0.0.4/agiflow/opentelemetry/instrumentation/groq/instrumentation.py` & `agiflow_sdk-0.0.5/agiflow/opentelemetry/instrumentation/groq/instrumentation.py`

 * *Files identical despite different names*

### Comparing `agiflow_sdk-0.0.4/agiflow/opentelemetry/instrumentation/langchain/.DS_Store` & `agiflow_sdk-0.0.5/agiflow/opentelemetry/instrumentation/langchain/.DS_Store`

 * *Files identical despite different names*

### Comparing `agiflow_sdk-0.0.4/agiflow/opentelemetry/instrumentation/langchain/__pycache__/instrumentation.cpython-311.pyc` & `agiflow_sdk-0.0.5/agiflow/opentelemetry/instrumentation/langchain/__pycache__/instrumentation.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `agiflow_sdk-0.0.4/agiflow/opentelemetry/instrumentation/langchain/__pycache__/patch.cpython-311.pyc` & `agiflow_sdk-0.0.5/agiflow/opentelemetry/instrumentation/langchain/__pycache__/patch.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `agiflow_sdk-0.0.4/agiflow/opentelemetry/instrumentation/langchain/hooks/__pycache__/__init__.cpython-311.pyc` & `agiflow_sdk-0.0.5/agiflow/opentelemetry/instrumentation/langchain/hooks/__pycache__/__init__.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `agiflow_sdk-0.0.4/agiflow/opentelemetry/instrumentation/langchain/hooks/__pycache__/base.cpython-311.pyc` & `agiflow_sdk-0.0.5/agiflow/opentelemetry/instrumentation/langchain/hooks/__pycache__/base.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `agiflow_sdk-0.0.4/agiflow/opentelemetry/instrumentation/langchain/hooks/__pycache__/chat.cpython-311.pyc` & `agiflow_sdk-0.0.5/agiflow/opentelemetry/instrumentation/langchain/hooks/__pycache__/chat.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `agiflow_sdk-0.0.4/agiflow/opentelemetry/instrumentation/langchain/hooks/__pycache__/generic.cpython-311.pyc` & `agiflow_sdk-0.0.5/agiflow/opentelemetry/instrumentation/langchain/hooks/__pycache__/generic.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `agiflow_sdk-0.0.4/agiflow/opentelemetry/instrumentation/langchain/hooks/base.py` & `agiflow_sdk-0.0.5/agiflow/opentelemetry/instrumentation/langchain/hooks/base.py`

 * *Files identical despite different names*

### Comparing `agiflow_sdk-0.0.4/agiflow/opentelemetry/instrumentation/langchain/hooks/chat.py` & `agiflow_sdk-0.0.5/agiflow/opentelemetry/instrumentation/langchain/hooks/chat.py`

 * *Files identical despite different names*

### Comparing `agiflow_sdk-0.0.4/agiflow/opentelemetry/instrumentation/langchain/hooks/generic.py` & `agiflow_sdk-0.0.5/agiflow/opentelemetry/instrumentation/langchain/hooks/generic.py`

 * *Files identical despite different names*

### Comparing `agiflow_sdk-0.0.4/agiflow/opentelemetry/instrumentation/langchain/instrumentation.py` & `agiflow_sdk-0.0.5/agiflow/opentelemetry/instrumentation/langchain/instrumentation.py`

 * *Files identical despite different names*

### Comparing `agiflow_sdk-0.0.4/agiflow/opentelemetry/instrumentation/langchain_community/.DS_Store` & `agiflow_sdk-0.0.5/agiflow/opentelemetry/instrumentation/langchain_community/.DS_Store`

 * *Files identical despite different names*

### Comparing `agiflow_sdk-0.0.4/agiflow/opentelemetry/instrumentation/langchain_community/__pycache__/instrumentation.cpython-311.pyc` & `agiflow_sdk-0.0.5/agiflow/opentelemetry/instrumentation/langchain_community/__pycache__/instrumentation.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `agiflow_sdk-0.0.4/agiflow/opentelemetry/instrumentation/langchain_community/__pycache__/patch.cpython-311.pyc` & `agiflow_sdk-0.0.5/agiflow/opentelemetry/instrumentation/langchain_community/__pycache__/patch.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `agiflow_sdk-0.0.4/agiflow/opentelemetry/instrumentation/langchain_community/hooks/.DS_Store` & `agiflow_sdk-0.0.5/agiflow/opentelemetry/instrumentation/langchain_community/hooks/.DS_Store`

 * *Files identical despite different names*

### Comparing `agiflow_sdk-0.0.4/agiflow/opentelemetry/instrumentation/langchain_community/hooks/__pycache__/base.cpython-311.pyc` & `agiflow_sdk-0.0.5/agiflow/opentelemetry/instrumentation/langchain_community/hooks/__pycache__/base.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `agiflow_sdk-0.0.4/agiflow/opentelemetry/instrumentation/langchain_community/hooks/__pycache__/chat.cpython-311.pyc` & `agiflow_sdk-0.0.5/agiflow/opentelemetry/instrumentation/langchain_community/hooks/__pycache__/chat.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `agiflow_sdk-0.0.4/agiflow/opentelemetry/instrumentation/langchain_community/hooks/__pycache__/generic.cpython-311.pyc` & `agiflow_sdk-0.0.5/agiflow/opentelemetry/instrumentation/langchain_community/hooks/__pycache__/generic.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `agiflow_sdk-0.0.4/agiflow/opentelemetry/instrumentation/langchain_community/hooks/__pycache__/llm.cpython-311.pyc` & `agiflow_sdk-0.0.5/agiflow/opentelemetry/instrumentation/langchain_community/hooks/__pycache__/llm.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `agiflow_sdk-0.0.4/agiflow/opentelemetry/instrumentation/langchain_community/hooks/base.py` & `agiflow_sdk-0.0.5/agiflow/opentelemetry/instrumentation/langchain_community/hooks/base.py`

 * *Files identical despite different names*

### Comparing `agiflow_sdk-0.0.4/agiflow/opentelemetry/instrumentation/langchain_community/hooks/generic.py` & `agiflow_sdk-0.0.5/agiflow/opentelemetry/instrumentation/langchain_community/hooks/generic.py`

 * *Files identical despite different names*

### Comparing `agiflow_sdk-0.0.4/agiflow/opentelemetry/instrumentation/langchain_community/instrumentation.py` & `agiflow_sdk-0.0.5/agiflow/opentelemetry/instrumentation/langchain_community/instrumentation.py`

 * *Files identical despite different names*

### Comparing `agiflow_sdk-0.0.4/agiflow/opentelemetry/instrumentation/langchain_core/.DS_Store` & `agiflow_sdk-0.0.5/agiflow/opentelemetry/instrumentation/langchain_core/.DS_Store`

 * *Files identical despite different names*

### Comparing `agiflow_sdk-0.0.4/agiflow/opentelemetry/instrumentation/langchain_core/__pycache__/instrumentation.cpython-311.pyc` & `agiflow_sdk-0.0.5/agiflow/opentelemetry/instrumentation/langchain_core/__pycache__/instrumentation.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `agiflow_sdk-0.0.4/agiflow/opentelemetry/instrumentation/langchain_core/__pycache__/patch.cpython-311.pyc` & `agiflow_sdk-0.0.5/agiflow/opentelemetry/instrumentation/langchain_core/__pycache__/patch.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `agiflow_sdk-0.0.4/agiflow/opentelemetry/instrumentation/langchain_core/hooks/__pycache__/__init__.cpython-311.pyc` & `agiflow_sdk-0.0.5/agiflow/opentelemetry/instrumentation/langchain_core/hooks/__pycache__/__init__.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `agiflow_sdk-0.0.4/agiflow/opentelemetry/instrumentation/langchain_core/hooks/__pycache__/base.cpython-311.pyc` & `agiflow_sdk-0.0.5/agiflow/opentelemetry/instrumentation/langchain_core/hooks/__pycache__/base.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `agiflow_sdk-0.0.4/agiflow/opentelemetry/instrumentation/langchain_core/hooks/__pycache__/generic.cpython-311.pyc` & `agiflow_sdk-0.0.5/agiflow/opentelemetry/instrumentation/langchain_core/hooks/__pycache__/generic.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `agiflow_sdk-0.0.4/agiflow/opentelemetry/instrumentation/langchain_core/hooks/__pycache__/llm.cpython-311.pyc` & `agiflow_sdk-0.0.5/agiflow/opentelemetry/instrumentation/langchain_core/hooks/__pycache__/llm.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `agiflow_sdk-0.0.4/agiflow/opentelemetry/instrumentation/langchain_core/hooks/__pycache__/runnable.cpython-311.pyc` & `agiflow_sdk-0.0.5/agiflow/opentelemetry/instrumentation/langchain_core/hooks/__pycache__/runnable.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `agiflow_sdk-0.0.4/agiflow/opentelemetry/instrumentation/langchain_core/hooks/base.py` & `agiflow_sdk-0.0.5/agiflow/opentelemetry/instrumentation/langchain_core/hooks/base.py`

 * *Files identical despite different names*

### Comparing `agiflow_sdk-0.0.4/agiflow/opentelemetry/instrumentation/langchain_core/hooks/generic.py` & `agiflow_sdk-0.0.5/agiflow/opentelemetry/instrumentation/langchain_core/hooks/generic.py`

 * *Files identical despite different names*

### Comparing `agiflow_sdk-0.0.4/agiflow/opentelemetry/instrumentation/langchain_core/hooks/llm.py` & `agiflow_sdk-0.0.5/agiflow/opentelemetry/instrumentation/langchain_core/hooks/llm.py`

 * *Files identical despite different names*

### Comparing `agiflow_sdk-0.0.4/agiflow/opentelemetry/instrumentation/langchain_core/hooks/runnable.py` & `agiflow_sdk-0.0.5/agiflow/opentelemetry/instrumentation/langchain_core/hooks/runnable.py`

 * *Files identical despite different names*

### Comparing `agiflow_sdk-0.0.4/agiflow/opentelemetry/instrumentation/langchain_core/instrumentation.py` & `agiflow_sdk-0.0.5/agiflow/opentelemetry/instrumentation/langchain_core/instrumentation.py`

 * *Files identical despite different names*

### Comparing `agiflow_sdk-0.0.4/agiflow/opentelemetry/instrumentation/langgraph/hooks/base.py` & `agiflow_sdk-0.0.5/agiflow/opentelemetry/instrumentation/langgraph/hooks/base.py`

 * *Files identical despite different names*

### Comparing `agiflow_sdk-0.0.4/agiflow/opentelemetry/instrumentation/langgraph/hooks/graph_call.py` & `agiflow_sdk-0.0.5/agiflow/opentelemetry/instrumentation/langgraph/hooks/graph_call.py`

 * *Files identical despite different names*

### Comparing `agiflow_sdk-0.0.4/agiflow/opentelemetry/instrumentation/langgraph/instrumentation.py` & `agiflow_sdk-0.0.5/agiflow/opentelemetry/instrumentation/langgraph/instrumentation.py`

 * *Files identical despite different names*

### Comparing `agiflow_sdk-0.0.4/agiflow/opentelemetry/instrumentation/llamaindex/hooks/base.py` & `agiflow_sdk-0.0.5/agiflow/opentelemetry/instrumentation/llamaindex/hooks/base.py`

 * *Files identical despite different names*

### Comparing `agiflow_sdk-0.0.4/agiflow/opentelemetry/instrumentation/llamaindex/hooks/generic.py` & `agiflow_sdk-0.0.5/agiflow/opentelemetry/instrumentation/llamaindex/hooks/generic.py`

 * *Files identical despite different names*

### Comparing `agiflow_sdk-0.0.4/agiflow/opentelemetry/instrumentation/llamaindex/instrumentation.py` & `agiflow_sdk-0.0.5/agiflow/opentelemetry/instrumentation/llamaindex/instrumentation.py`

 * *Files identical despite different names*

### Comparing `agiflow_sdk-0.0.4/agiflow/opentelemetry/instrumentation/openai/.DS_Store` & `agiflow_sdk-0.0.5/agiflow/opentelemetry/instrumentation/openai/.DS_Store`

 * *Files identical despite different names*

### Comparing `agiflow_sdk-0.0.4/agiflow/opentelemetry/instrumentation/openai/__pycache__/instrumentation.cpython-311.pyc` & `agiflow_sdk-0.0.5/agiflow/opentelemetry/instrumentation/openai/__pycache__/instrumentation.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `agiflow_sdk-0.0.4/agiflow/opentelemetry/instrumentation/openai/__pycache__/patch.cpython-311.pyc` & `agiflow_sdk-0.0.5/agiflow/opentelemetry/instrumentation/openai/__pycache__/patch.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `agiflow_sdk-0.0.4/agiflow/opentelemetry/instrumentation/openai/hooks/.DS_Store` & `agiflow_sdk-0.0.5/agiflow/opentelemetry/instrumentation/openai/hooks/.DS_Store`

 * *Files identical despite different names*

### Comparing `agiflow_sdk-0.0.4/agiflow/opentelemetry/instrumentation/openai/hooks/__pycache__/__init__.cpython-311.pyc` & `agiflow_sdk-0.0.5/agiflow/opentelemetry/instrumentation/openai/hooks/__pycache__/__init__.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `agiflow_sdk-0.0.4/agiflow/opentelemetry/instrumentation/openai/hooks/__pycache__/base.cpython-311.pyc` & `agiflow_sdk-0.0.5/agiflow/opentelemetry/instrumentation/openai/hooks/__pycache__/base.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `agiflow_sdk-0.0.4/agiflow/opentelemetry/instrumentation/openai/hooks/__pycache__/base_llm.cpython-311.pyc` & `agiflow_sdk-0.0.5/agiflow/opentelemetry/instrumentation/openai/hooks/__pycache__/base_llm.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `agiflow_sdk-0.0.4/agiflow/opentelemetry/instrumentation/openai/hooks/__pycache__/chat_completion.cpython-311.pyc` & `agiflow_sdk-0.0.5/agiflow/opentelemetry/instrumentation/openai/hooks/__pycache__/chat_completion.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `agiflow_sdk-0.0.4/agiflow/opentelemetry/instrumentation/openai/hooks/__pycache__/completion.cpython-311.pyc` & `agiflow_sdk-0.0.5/agiflow/opentelemetry/instrumentation/openai/hooks/__pycache__/completion.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `agiflow_sdk-0.0.4/agiflow/opentelemetry/instrumentation/openai/hooks/__pycache__/embedding.cpython-311.pyc` & `agiflow_sdk-0.0.5/agiflow/opentelemetry/instrumentation/openai/hooks/__pycache__/embedding.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `agiflow_sdk-0.0.4/agiflow/opentelemetry/instrumentation/openai/hooks/__pycache__/image_generate.cpython-311.pyc` & `agiflow_sdk-0.0.5/agiflow/opentelemetry/instrumentation/openai/hooks/__pycache__/image_generate.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `agiflow_sdk-0.0.4/agiflow/opentelemetry/instrumentation/openai/hooks/__pycache__/utils.cpython-311.pyc` & `agiflow_sdk-0.0.5/agiflow/opentelemetry/instrumentation/openai/hooks/__pycache__/utils.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `agiflow_sdk-0.0.4/agiflow/opentelemetry/instrumentation/openai/hooks/base.py` & `agiflow_sdk-0.0.5/agiflow/opentelemetry/instrumentation/openai/hooks/base.py`

 * *Files identical despite different names*

### Comparing `agiflow_sdk-0.0.4/agiflow/opentelemetry/instrumentation/openai/hooks/base_llm.py` & `agiflow_sdk-0.0.5/agiflow/opentelemetry/instrumentation/openai/hooks/base_llm.py`

 * *Files identical despite different names*

### Comparing `agiflow_sdk-0.0.4/agiflow/opentelemetry/instrumentation/openai/hooks/chat_completion.py` & `agiflow_sdk-0.0.5/agiflow/opentelemetry/instrumentation/openai/hooks/chat_completion.py`

 * *Files identical despite different names*

### Comparing `agiflow_sdk-0.0.4/agiflow/opentelemetry/instrumentation/openai/hooks/embedding.py` & `agiflow_sdk-0.0.5/agiflow/opentelemetry/instrumentation/openai/hooks/embedding.py`

 * *Files identical despite different names*

### Comparing `agiflow_sdk-0.0.4/agiflow/opentelemetry/instrumentation/openai/hooks/image_generate.py` & `agiflow_sdk-0.0.5/agiflow/opentelemetry/instrumentation/openai/hooks/image_generate.py`

 * *Files identical despite different names*

### Comparing `agiflow_sdk-0.0.4/agiflow/opentelemetry/instrumentation/openai/hooks/utils.py` & `agiflow_sdk-0.0.5/agiflow/opentelemetry/instrumentation/openai/hooks/utils.py`

 * *Files identical despite different names*

### Comparing `agiflow_sdk-0.0.4/agiflow/opentelemetry/instrumentation/openai/instrumentation.py` & `agiflow_sdk-0.0.5/agiflow/opentelemetry/instrumentation/openai/instrumentation.py`

 * *Files identical despite different names*

### Comparing `agiflow_sdk-0.0.4/agiflow/opentelemetry/instrumentation/pinecone/hooks/base.py` & `agiflow_sdk-0.0.5/agiflow/opentelemetry/instrumentation/pinecone/hooks/base.py`

 * *Files identical despite different names*

### Comparing `agiflow_sdk-0.0.4/agiflow/opentelemetry/instrumentation/pinecone/hooks/generic.py` & `agiflow_sdk-0.0.5/agiflow/opentelemetry/instrumentation/pinecone/hooks/generic.py`

 * *Files identical despite different names*

### Comparing `agiflow_sdk-0.0.4/agiflow/opentelemetry/instrumentation/pinecone/instrumentation.py` & `agiflow_sdk-0.0.5/agiflow/opentelemetry/instrumentation/pinecone/instrumentation.py`

 * *Files identical despite different names*

### Comparing `agiflow_sdk-0.0.4/agiflow/opentelemetry/instrumentation/qdrant/hooks/base.py` & `agiflow_sdk-0.0.5/agiflow/opentelemetry/instrumentation/qdrant/hooks/base.py`

 * *Files identical despite different names*

### Comparing `agiflow_sdk-0.0.4/agiflow/opentelemetry/instrumentation/qdrant/hooks/collection.py` & `agiflow_sdk-0.0.5/agiflow/opentelemetry/instrumentation/qdrant/hooks/collection.py`

 * *Files identical despite different names*

### Comparing `agiflow_sdk-0.0.4/agiflow/opentelemetry/instrumentation/qdrant/instrumentation.py` & `agiflow_sdk-0.0.5/agiflow/opentelemetry/instrumentation/qdrant/instrumentation.py`

 * *Files identical despite different names*

### Comparing `agiflow_sdk-0.0.4/agiflow/opentelemetry/instrumentation/utils/__init__.py` & `agiflow_sdk-0.0.5/agiflow/opentelemetry/instrumentation/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `agiflow_sdk-0.0.4/agiflow/opentelemetry/instrumentation/utils/__pycache__/__init__.cpython-311.pyc` & `agiflow_sdk-0.0.5/agiflow/opentelemetry/instrumentation/utils/__pycache__/__init__.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `agiflow_sdk-0.0.4/agiflow/opentelemetry/instrumentation/utils/__pycache__/wrapper.cpython-311.pyc` & `agiflow_sdk-0.0.5/agiflow/opentelemetry/instrumentation/utils/__pycache__/wrapper.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `agiflow_sdk-0.0.4/agiflow/opentelemetry/instrumentation/utils/wrapper.py` & `agiflow_sdk-0.0.5/agiflow/opentelemetry/instrumentation/utils/wrapper.py`

 * *Files identical despite different names*

### Comparing `agiflow_sdk-0.0.4/agiflow/opentelemetry/instrumentation/weaviate/hooks/base.py` & `agiflow_sdk-0.0.5/agiflow/opentelemetry/instrumentation/weaviate/hooks/base.py`

 * *Files identical despite different names*

### Comparing `agiflow_sdk-0.0.4/agiflow/opentelemetry/instrumentation/weaviate/hooks/generic_collection.py` & `agiflow_sdk-0.0.5/agiflow/opentelemetry/instrumentation/weaviate/hooks/generic_collection.py`

 * *Files identical despite different names*

### Comparing `agiflow_sdk-0.0.4/agiflow/opentelemetry/instrumentation/weaviate/hooks/generic_query.py` & `agiflow_sdk-0.0.5/agiflow/opentelemetry/instrumentation/weaviate/hooks/generic_query.py`

 * *Files identical despite different names*

### Comparing `agiflow_sdk-0.0.4/agiflow/opentelemetry/instrumentation/weaviate/instrumentation.py` & `agiflow_sdk-0.0.5/agiflow/opentelemetry/instrumentation/weaviate/instrumentation.py`

 * *Files identical despite different names*

### Comparing `agiflow_sdk-0.0.4/agiflow/opentelemetry/span_processors/__pycache__/thread_pool_span_processor.cpython-311.pyc` & `agiflow_sdk-0.0.5/agiflow/opentelemetry/span_processors/__pycache__/thread_pool_span_processor.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `agiflow_sdk-0.0.4/agiflow/opentelemetry/span_processors/thread_pool_span_processor.py` & `agiflow_sdk-0.0.5/agiflow/opentelemetry/span_processors/thread_pool_span_processor.py`

 * *Files identical despite different names*

### Comparing `agiflow_sdk-0.0.4/agiflow/opentelemetry/trace_decorators/__init__.py` & `agiflow_sdk-0.0.5/agiflow/opentelemetry/trace_decorators/__init__.py`

 * *Files identical despite different names*

### Comparing `agiflow_sdk-0.0.4/agiflow/opentelemetry/trace_decorators/__pycache__/__init__.cpython-311.pyc` & `agiflow_sdk-0.0.5/agiflow/opentelemetry/trace_decorators/__pycache__/__init__.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `agiflow_sdk-0.0.4/agiflow/opentelemetry/trace_decorators/__pycache__/helper.cpython-311.pyc` & `agiflow_sdk-0.0.5/agiflow/opentelemetry/trace_decorators/__pycache__/helper.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `agiflow_sdk-0.0.4/agiflow/opentelemetry/trace_decorators/__pycache__/task.cpython-311.pyc` & `agiflow_sdk-0.0.5/agiflow/opentelemetry/trace_decorators/__pycache__/task.cpython-311.pyc`

 * *Files 17% similar despite different names*

#### Python bytecode

```diff
@@ -1,37 +1,38 @@
 magic:    0xa70d0d0a
-moddate:  0x47d85b66 (Sun Jun  2 02:26:15 2024 UTC)
-files sz: 3514
+moddate:  0x65895d66 (Mon Jun  3 09:14:13 2024 UTC)
+files sz: 3964
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 10
    flags     : 0
    code
       0x9700640064016c006d015a016d025a020100640064026c036d045a046d
       055a050100640064036c066d075a070100640064046c086d095a096d0a5a
       0a6d0b5a0b6d0c5a0c6d0d5a0d0100640064056c0e6d0f5a0f0100020047
       006406840064076509a6030000ab0300000000000000005a106408640865
-      0f6a11000000000000000065056a12000000000000000066046409650165
-      1319000000000000000000640a6501651319000000000000000000640b65
-      01650519000000000000000000640c650265071900000000000000000066
-      08640d84055a1464086408650f6a11000000000000000065056a12000000
-      0000000000660464096501651319000000000000000000640a6501651319
-      000000000000000000640b6501650519000000000000000000640c650265
-      07190000000000000000006608640e84055a1564086408650f6a11000000
-      0000000000660364096501651319000000000000000000640a6501651319
-      000000000000000000640c65026507190000000000000000006606640f84
-      055a1664086408650f6a1100000000000000006603640965016513190000
-      00000000000000640a6501651319000000000000000000640c6502650719
-      0000000000000000006606641084055a1764086408650f6a110000000000
-      000000660364096501651319000000000000000000640a65016513190000
-      00000000000000640c65026507190000000000000000006606641184055a
-      1864086408650f6a11000000000000000066036409650165131900000000
-      0000000000640a6501651319000000000000000000640c65026507190000
-      000000000000006606641284055a1964085300
+      0f6a11000000000000000065056a12000000000000000064096605640a65
+      01651319000000000000000000640b650165131900000000000000000064
+      0c6501650519000000000000000000640d65026507190000000000000000
+      006608640e84055a1464086408650f6a11000000000000000065056a1200
+      0000000000000064096605640a6501651319000000000000000000640b65
+      01651319000000000000000000640c650165051900000000000000000064
+      0d65026507190000000000000000006608640f84055a1564086408650f6a
+      11000000000000000064096604640a650165131900000000000000000064
+      0b6501651319000000000000000000640d65026507190000000000000000
+      006606641084055a1664086408650f6a1100000000000000006409660464
+      0a6501651319000000000000000000640b65016513190000000000000000
+      00640d65026507190000000000000000006606641184055a176408640865
+      0f6a11000000000000000064096604640a65016513190000000000000000
+      00640b6501651319000000000000000000640d6502650719000000000000
+      0000006606641284055a1864086408650f6a110000000000000000640966
+      04640a6501651319000000000000000000640b6501651319000000000000
+      000000640d65026507190000000000000000006606641384055a19640853
+      00
      0           0 RESUME                   0
    
      1           2 LOAD_CONST               0 (0)
                  4 LOAD_CONST               1 (('Optional', 'Unpack'))
                  6 IMPORT_NAME              0 (typing)
                  8 IMPORT_FROM              1 (Optional)
                 10 STORE_NAME               1 (Optional)
@@ -93,209 +94,221 @@
    
     32         118 LOAD_NAME               15 (SpanKind)
                120 LOAD_ATTR               17 (INTERNAL)
    
     33         130 LOAD_NAME                5 (AgiflowServiceTypes)
                132 LOAD_ATTR               18 (TASK)
    
-    29         142 BUILD_TUPLE              4
-               144 LOAD_CONST               9 ('name')
+    34         142 LOAD_CONST               9 (False)
    
-    30         146 LOAD_NAME                1 (Optional)
-               148 LOAD_NAME               19 (str)
-               150 BINARY_SUBSCR
+    29         144 BUILD_TUPLE              5
+               146 LOAD_CONST              10 ('name')
    
-    29         160 LOAD_CONST              10 ('method_name')
+    30         148 LOAD_NAME                1 (Optional)
+               150 LOAD_NAME               19 (str)
+               152 BINARY_SUBSCR
    
-    31         162 LOAD_NAME                1 (Optional)
-               164 LOAD_NAME               19 (str)
-               166 BINARY_SUBSCR
+    29         162 LOAD_CONST              11 ('method_name')
    
-    29         176 LOAD_CONST              11 ('tlp_service_type')
+    31         164 LOAD_NAME                1 (Optional)
+               166 LOAD_NAME               19 (str)
+               168 BINARY_SUBSCR
    
-    33         178 LOAD_NAME                1 (Optional)
-               180 LOAD_NAME                5 (AgiflowServiceTypes)
-               182 BINARY_SUBSCR
+    29         178 LOAD_CONST              12 ('tlp_service_type')
    
-    29         192 LOAD_CONST              12 ('kwargs')
+    33         180 LOAD_NAME                1 (Optional)
+               182 LOAD_NAME                5 (AgiflowServiceTypes)
+               184 BINARY_SUBSCR
    
-    34         194 LOAD_NAME                2 (Unpack)
-               196 LOAD_NAME                7 (SharedKwargsWithHooks)
-               198 BINARY_SUBSCR
+    29         194 LOAD_CONST              13 ('kwargs')
    
-    29         208 BUILD_TUPLE              8
-               210 LOAD_CONST              13 (<code object task, file "/Users/vuongngo/workspace/agiflow/packages/python/agiflow-sdk/agiflow/opentelemetry/trace_decorators/task.py", line 29>)
-               212 MAKE_FUNCTION            5 (defaults, annotations)
-               214 STORE_NAME              20 (task)
+    35         196 LOAD_NAME                2 (Unpack)
+               198 LOAD_NAME                7 (SharedKwargsWithHooks)
+               200 BINARY_SUBSCR
    
-    57         216 LOAD_CONST               8 (None)
+    29         210 BUILD_TUPLE              8
+               212 LOAD_CONST              14 (<code object task, file "/Users/vuongngo/workspace/agiflow/packages/python/agiflow-sdk/agiflow/opentelemetry/trace_decorators/task.py", line 29>)
+               214 MAKE_FUNCTION            5 (defaults, annotations)
+               216 STORE_NAME              20 (task)
    
-    58         218 LOAD_CONST               8 (None)
+    60         218 LOAD_CONST               8 (None)
    
-    59         220 LOAD_NAME               15 (SpanKind)
-               222 LOAD_ATTR               17 (INTERNAL)
+    61         220 LOAD_CONST               8 (None)
    
-    60         232 LOAD_NAME                5 (AgiflowServiceTypes)
-               234 LOAD_ATTR               18 (TASK)
+    62         222 LOAD_NAME               15 (SpanKind)
+               224 LOAD_ATTR               17 (INTERNAL)
    
-    56         244 BUILD_TUPLE              4
-               246 LOAD_CONST               9 ('name')
+    63         234 LOAD_NAME                5 (AgiflowServiceTypes)
+               236 LOAD_ATTR               18 (TASK)
    
-    57         248 LOAD_NAME                1 (Optional)
-               250 LOAD_NAME               19 (str)
-               252 BINARY_SUBSCR
+    64         246 LOAD_CONST               9 (False)
    
-    56         262 LOAD_CONST              10 ('method_name')
+    59         248 BUILD_TUPLE              5
+               250 LOAD_CONST              10 ('name')
    
-    58         264 LOAD_NAME                1 (Optional)
-               266 LOAD_NAME               19 (str)
-               268 BINARY_SUBSCR
+    60         252 LOAD_NAME                1 (Optional)
+               254 LOAD_NAME               19 (str)
+               256 BINARY_SUBSCR
    
-    56         278 LOAD_CONST              11 ('tlp_service_type')
+    59         266 LOAD_CONST              11 ('method_name')
    
-    60         280 LOAD_NAME                1 (Optional)
-               282 LOAD_NAME                5 (AgiflowServiceTypes)
-               284 BINARY_SUBSCR
+    61         268 LOAD_NAME                1 (Optional)
+               270 LOAD_NAME               19 (str)
+               272 BINARY_SUBSCR
    
-    56         294 LOAD_CONST              12 ('kwargs')
+    59         282 LOAD_CONST              12 ('tlp_service_type')
    
-    61         296 LOAD_NAME                2 (Unpack)
-               298 LOAD_NAME                7 (SharedKwargsWithHooks)
-               300 BINARY_SUBSCR
+    63         284 LOAD_NAME                1 (Optional)
+               286 LOAD_NAME                5 (AgiflowServiceTypes)
+               288 BINARY_SUBSCR
    
-    56         310 BUILD_TUPLE              8
-               312 LOAD_CONST              14 (<code object atask, file "/Users/vuongngo/workspace/agiflow/packages/python/agiflow-sdk/agiflow/opentelemetry/trace_decorators/task.py", line 56>)
-               314 MAKE_FUNCTION            5 (defaults, annotations)
-               316 STORE_NAME              21 (atask)
+    59         298 LOAD_CONST              13 ('kwargs')
    
-    83         318 LOAD_CONST               8 (None)
+    65         300 LOAD_NAME                2 (Unpack)
+               302 LOAD_NAME                7 (SharedKwargsWithHooks)
+               304 BINARY_SUBSCR
    
-    84         320 LOAD_CONST               8 (None)
+    59         314 BUILD_TUPLE              8
+               316 LOAD_CONST              15 (<code object atask, file "/Users/vuongngo/workspace/agiflow/packages/python/agiflow-sdk/agiflow/opentelemetry/trace_decorators/task.py", line 59>)
+               318 MAKE_FUNCTION            5 (defaults, annotations)
+               320 STORE_NAME              21 (atask)
    
-    85         322 LOAD_NAME               15 (SpanKind)
-               324 LOAD_ATTR               17 (INTERNAL)
+    89         322 LOAD_CONST               8 (None)
    
-    82         334 BUILD_TUPLE              3
-               336 LOAD_CONST               9 ('name')
+    90         324 LOAD_CONST               8 (None)
    
-    83         338 LOAD_NAME                1 (Optional)
-               340 LOAD_NAME               19 (str)
-               342 BINARY_SUBSCR
+    91         326 LOAD_NAME               15 (SpanKind)
+               328 LOAD_ATTR               17 (INTERNAL)
    
-    82         352 LOAD_CONST              10 ('method_name')
+    92         338 LOAD_CONST               9 (False)
    
-    84         354 LOAD_NAME                1 (Optional)
-               356 LOAD_NAME               19 (str)
-               358 BINARY_SUBSCR
+    88         340 BUILD_TUPLE              4
+               342 LOAD_CONST              10 ('name')
    
-    82         368 LOAD_CONST              12 ('kwargs')
+    89         344 LOAD_NAME                1 (Optional)
+               346 LOAD_NAME               19 (str)
+               348 BINARY_SUBSCR
    
-    86         370 LOAD_NAME                2 (Unpack)
-               372 LOAD_NAME                7 (SharedKwargsWithHooks)
-               374 BINARY_SUBSCR
+    88         358 LOAD_CONST              11 ('method_name')
    
-    82         384 BUILD_TUPLE              6
-               386 LOAD_CONST              15 (<code object agent, file "/Users/vuongngo/workspace/agiflow/packages/python/agiflow-sdk/agiflow/opentelemetry/trace_decorators/task.py", line 82>)
-               388 MAKE_FUNCTION            5 (defaults, annotations)
-               390 STORE_NAME              22 (agent)
+    90         360 LOAD_NAME                1 (Optional)
+               362 LOAD_NAME               19 (str)
+               364 BINARY_SUBSCR
    
-    98         392 LOAD_CONST               8 (None)
+    88         374 LOAD_CONST              13 ('kwargs')
    
-    99         394 LOAD_CONST               8 (None)
+    93         376 LOAD_NAME                2 (Unpack)
+               378 LOAD_NAME                7 (SharedKwargsWithHooks)
+               380 BINARY_SUBSCR
    
-   100         396 LOAD_NAME               15 (SpanKind)
-               398 LOAD_ATTR               17 (INTERNAL)
+    88         390 BUILD_TUPLE              6
+               392 LOAD_CONST              16 (<code object agent, file "/Users/vuongngo/workspace/agiflow/packages/python/agiflow-sdk/agiflow/opentelemetry/trace_decorators/task.py", line 88>)
+               394 MAKE_FUNCTION            5 (defaults, annotations)
+               396 STORE_NAME              22 (agent)
    
-    97         408 BUILD_TUPLE              3
-               410 LOAD_CONST               9 ('name')
+   106         398 LOAD_CONST               8 (None)
    
-    98         412 LOAD_NAME                1 (Optional)
-               414 LOAD_NAME               19 (str)
-               416 BINARY_SUBSCR
+   107         400 LOAD_CONST               8 (None)
    
-    97         426 LOAD_CONST              10 ('method_name')
+   108         402 LOAD_NAME               15 (SpanKind)
+               404 LOAD_ATTR               17 (INTERNAL)
    
-    99         428 LOAD_NAME                1 (Optional)
-               430 LOAD_NAME               19 (str)
-               432 BINARY_SUBSCR
+   109         414 LOAD_CONST               9 (False)
    
-    97         442 LOAD_CONST              12 ('kwargs')
+   105         416 BUILD_TUPLE              4
+               418 LOAD_CONST              10 ('name')
    
-   101         444 LOAD_NAME                2 (Unpack)
-               446 LOAD_NAME                7 (SharedKwargsWithHooks)
-               448 BINARY_SUBSCR
+   106         420 LOAD_NAME                1 (Optional)
+               422 LOAD_NAME               19 (str)
+               424 BINARY_SUBSCR
    
-    97         458 BUILD_TUPLE              6
-               460 LOAD_CONST              16 (<code object tool, file "/Users/vuongngo/workspace/agiflow/packages/python/agiflow-sdk/agiflow/opentelemetry/trace_decorators/task.py", line 97>)
-               462 MAKE_FUNCTION            5 (defaults, annotations)
-               464 STORE_NAME              23 (tool)
+   105         434 LOAD_CONST              11 ('method_name')
    
-   113         466 LOAD_CONST               8 (None)
+   107         436 LOAD_NAME                1 (Optional)
+               438 LOAD_NAME               19 (str)
+               440 BINARY_SUBSCR
    
-   114         468 LOAD_CONST               8 (None)
+   105         450 LOAD_CONST              13 ('kwargs')
    
-   115         470 LOAD_NAME               15 (SpanKind)
-               472 LOAD_ATTR               17 (INTERNAL)
+   110         452 LOAD_NAME                2 (Unpack)
+               454 LOAD_NAME                7 (SharedKwargsWithHooks)
+               456 BINARY_SUBSCR
    
-   112         482 BUILD_TUPLE              3
-               484 LOAD_CONST               9 ('name')
+   105         466 BUILD_TUPLE              6
+               468 LOAD_CONST              17 (<code object tool, file "/Users/vuongngo/workspace/agiflow/packages/python/agiflow-sdk/agiflow/opentelemetry/trace_decorators/task.py", line 105>)
+               470 MAKE_FUNCTION            5 (defaults, annotations)
+               472 STORE_NAME              23 (tool)
    
-   113         486 LOAD_NAME                1 (Optional)
-               488 LOAD_NAME               19 (str)
-               490 BINARY_SUBSCR
+   123         474 LOAD_CONST               8 (None)
    
-   112         500 LOAD_CONST              10 ('method_name')
+   124         476 LOAD_CONST               8 (None)
    
-   114         502 LOAD_NAME                1 (Optional)
-               504 LOAD_NAME               19 (str)
-               506 BINARY_SUBSCR
+   125         478 LOAD_NAME               15 (SpanKind)
+               480 LOAD_ATTR               17 (INTERNAL)
    
-   112         516 LOAD_CONST              12 ('kwargs')
+   126         490 LOAD_CONST               9 (False)
    
-   116         518 LOAD_NAME                2 (Unpack)
-               520 LOAD_NAME                7 (SharedKwargsWithHooks)
-               522 BINARY_SUBSCR
+   122         492 BUILD_TUPLE              4
+               494 LOAD_CONST              10 ('name')
    
-   112         532 BUILD_TUPLE              6
-               534 LOAD_CONST              17 (<code object aagent, file "/Users/vuongngo/workspace/agiflow/packages/python/agiflow-sdk/agiflow/opentelemetry/trace_decorators/task.py", line 112>)
-               536 MAKE_FUNCTION            5 (defaults, annotations)
-               538 STORE_NAME              24 (aagent)
+   123         496 LOAD_NAME                1 (Optional)
+               498 LOAD_NAME               19 (str)
+               500 BINARY_SUBSCR
    
-   128         540 LOAD_CONST               8 (None)
+   122         510 LOAD_CONST              11 ('method_name')
    
-   129         542 LOAD_CONST               8 (None)
+   124         512 LOAD_NAME                1 (Optional)
+               514 LOAD_NAME               19 (str)
+               516 BINARY_SUBSCR
    
-   130         544 LOAD_NAME               15 (SpanKind)
-               546 LOAD_ATTR               17 (INTERNAL)
+   122         526 LOAD_CONST              13 ('kwargs')
    
-   127         556 BUILD_TUPLE              3
-               558 LOAD_CONST               9 ('name')
+   127         528 LOAD_NAME                2 (Unpack)
+               530 LOAD_NAME                7 (SharedKwargsWithHooks)
+               532 BINARY_SUBSCR
    
-   128         560 LOAD_NAME                1 (Optional)
-               562 LOAD_NAME               19 (str)
-               564 BINARY_SUBSCR
+   122         542 BUILD_TUPLE              6
+               544 LOAD_CONST              18 (<code object aagent, file "/Users/vuongngo/workspace/agiflow/packages/python/agiflow-sdk/agiflow/opentelemetry/trace_decorators/task.py", line 122>)
+               546 MAKE_FUNCTION            5 (defaults, annotations)
+               548 STORE_NAME              24 (aagent)
    
-   127         574 LOAD_CONST              10 ('method_name')
+   140         550 LOAD_CONST               8 (None)
    
-   129         576 LOAD_NAME                1 (Optional)
-               578 LOAD_NAME               19 (str)
-               580 BINARY_SUBSCR
+   141         552 LOAD_CONST               8 (None)
    
-   127         590 LOAD_CONST              12 ('kwargs')
+   142         554 LOAD_NAME               15 (SpanKind)
+               556 LOAD_ATTR               17 (INTERNAL)
    
-   131         592 LOAD_NAME                2 (Unpack)
-               594 LOAD_NAME                7 (SharedKwargsWithHooks)
-               596 BINARY_SUBSCR
+   143         566 LOAD_CONST               9 (False)
    
-   127         606 BUILD_TUPLE              6
-               608 LOAD_CONST              18 (<code object atool, file "/Users/vuongngo/workspace/agiflow/packages/python/agiflow-sdk/agiflow/opentelemetry/trace_decorators/task.py", line 127>)
-               610 MAKE_FUNCTION            5 (defaults, annotations)
-               612 STORE_NAME              25 (atool)
-               614 LOAD_CONST               8 (None)
-               616 RETURN_VALUE
+   139         568 BUILD_TUPLE              4
+               570 LOAD_CONST              10 ('name')
+   
+   140         572 LOAD_NAME                1 (Optional)
+               574 LOAD_NAME               19 (str)
+               576 BINARY_SUBSCR
+   
+   139         586 LOAD_CONST              11 ('method_name')
+   
+   141         588 LOAD_NAME                1 (Optional)
+               590 LOAD_NAME               19 (str)
+               592 BINARY_SUBSCR
+   
+   139         602 LOAD_CONST              13 ('kwargs')
+   
+   144         604 LOAD_NAME                2 (Unpack)
+               606 LOAD_NAME                7 (SharedKwargsWithHooks)
+               608 BINARY_SUBSCR
+   
+   139         618 BUILD_TUPLE              6
+               620 LOAD_CONST              19 (<code object atool, file "/Users/vuongngo/workspace/agiflow/packages/python/agiflow-sdk/agiflow/opentelemetry/trace_decorators/task.py", line 139>)
+               622 MAKE_FUNCTION            5 (defaults, annotations)
+               624 STORE_NAME              25 (atool)
+               626 LOAD_CONST               8 (None)
+               628 RETURN_VALUE
    consts
       0
       ('Optional', 'Unpack')
       ('SpanAttributes', 'AgiflowServiceTypes')
       ('SharedKwargsWithHooks',)
       ('BaseSpanCapture', 'decorate_method', 'decorate_class_method', 'adecorate_method', 'adecorate_class_method')
       ('SpanKind',)
@@ -419,334 +432,352 @@
          cellvars   ('__class__',)
          filename   '/Users/vuongngo/workspace/agiflow/packages/python/agiflow-sdk/agiflow/opentelemetry/trace_decorators/task.py'
          name       'TaskSpanCapture'
          firstlineno 18
          lnotab 0x0c010a03
       'TaskSpanCapture'
       None
+      False
       'name'
       'method_name'
       'tlp_service_type'
       'kwargs'
       code
-         argcount  : 4
-         nlocals   : 5
-         stacksize : 9
+         argcount  : 5
+         nlocals   : 6
+         stacksize : 10
          flags     : 11
          code
-            0x97007c01801674010000000000000000000064037c007c037c02740200
-            00000000000000000064019c047c04a4018e015300740500000000000000
-            00000064037c007c017c037c0274020000000000000000000064029c057c
-            04a4018e015300
+            0x97007c01801774010000000000000000000064037c007c037c02740200
+            0000000000000000007c0464019c057c05a4018e01530074050000000000
+            000000000064037c007c017c037c027402000000000000000000007c0464
+            029c067c05a4018e015300
           29           0 RESUME                   0
          
-          36           2 LOAD_FAST                1 (method_name)
-                       4 POP_JUMP_FORWARD_IF_NOT_NONE    22 (to 50)
+          37           2 LOAD_FAST                1 (method_name)
+                       4 POP_JUMP_FORWARD_IF_NOT_NONE    23 (to 52)
          
-          37           6 LOAD_GLOBAL              1 (NULL + decorate_method)
+          38           6 LOAD_GLOBAL              1 (NULL + decorate_method)
                       18 LOAD_CONST               3 (())
          
-          38          20 LOAD_FAST                0 (name)
+          39          20 LOAD_FAST                0 (name)
+         
+          40          22 LOAD_FAST                3 (tlp_service_type)
          
-          39          22 LOAD_FAST                3 (tlp_service_type)
+          41          24 LOAD_FAST                2 (span_kind)
          
-          40          24 LOAD_FAST                2 (span_kind)
+          42          26 LOAD_GLOBAL              2 (TaskSpanCapture)
          
-          41          26 LOAD_GLOBAL              2 (TaskSpanCapture)
+          43          38 LOAD_FAST                4 (flush_on_exit)
          
-          37          38 LOAD_CONST               1 (('name', 'tlp_service_type', 'span_kind', 'SpanCapture'))
-                      40 BUILD_CONST_KEY_MAP      4
+          38          40 LOAD_CONST               1 (('name', 'tlp_service_type', 'span_kind', 'SpanCapture', 'flush_on_exit'))
+                      42 BUILD_CONST_KEY_MAP      5
          
-          42          42 LOAD_FAST                4 (kwargs)
+          44          44 LOAD_FAST                5 (kwargs)
          
-          37          44 DICT_MERGE               1
-                      46 CALL_FUNCTION_EX         1
-                      48 RETURN_VALUE
+          38          46 DICT_MERGE               1
+                      48 CALL_FUNCTION_EX         1
+                      50 RETURN_VALUE
          
-          45     >>   50 LOAD_GLOBAL              5 (NULL + decorate_class_method)
-                      62 LOAD_CONST               3 (())
+          47     >>   52 LOAD_GLOBAL              5 (NULL + decorate_class_method)
+                      64 LOAD_CONST               3 (())
          
-          46          64 LOAD_FAST                0 (name)
+          48          66 LOAD_FAST                0 (name)
          
-          47          66 LOAD_FAST                1 (method_name)
+          49          68 LOAD_FAST                1 (method_name)
          
-          48          68 LOAD_FAST                3 (tlp_service_type)
+          50          70 LOAD_FAST                3 (tlp_service_type)
          
-          49          70 LOAD_FAST                2 (span_kind)
+          51          72 LOAD_FAST                2 (span_kind)
          
-          50          72 LOAD_GLOBAL              2 (TaskSpanCapture)
+          52          74 LOAD_GLOBAL              2 (TaskSpanCapture)
          
-          45          84 LOAD_CONST               2 (('name', 'method_name', 'tlp_service_type', 'span_kind', 'SpanCapture'))
-                      86 BUILD_CONST_KEY_MAP      5
+          53          86 LOAD_FAST                4 (flush_on_exit)
          
-          51          88 LOAD_FAST                4 (kwargs)
+          47          88 LOAD_CONST               2 (('name', 'method_name', 'tlp_service_type', 'span_kind', 'SpanCapture', 'flush_on_exit'))
+                      90 BUILD_CONST_KEY_MAP      6
          
-          45          90 DICT_MERGE               1
-                      92 CALL_FUNCTION_EX         1
-                      94 RETURN_VALUE
+          54          92 LOAD_FAST                5 (kwargs)
+         
+          47          94 DICT_MERGE               1
+                      96 CALL_FUNCTION_EX         1
+                      98 RETURN_VALUE
          consts
             None
-            ('name', 'tlp_service_type', 'span_kind', 'SpanCapture')
-            ('name', 'method_name', 'tlp_service_type', 'span_kind', 'SpanCapture')
+            ('name', 'tlp_service_type', 'span_kind', 'SpanCapture', 'flush_on_exit')
+            ('name', 'method_name', 'tlp_service_type', 'span_kind', 'SpanCapture', 'flush_on_exit')
             ()
          names      ('decorate_method', 'TaskSpanCapture', 'decorate_class_method')
-         varnames   ('name', 'method_name', 'span_kind', 'tlp_service_type', 'kwargs')
+         varnames   ('name', 'method_name', 'span_kind', 'tlp_service_type', 'flush_on_exit', 'kwargs')
          freevars   ()
          cellvars   ()
          filename   '/Users/vuongngo/workspace/agiflow/packages/python/agiflow-sdk/agiflow/opentelemetry/trace_decorators/task.py'
          name       'task'
          firstlineno 29
          lnotab
-            0x020704010e010201020102010cfc040502fb06080e0102010201020102
-            010cfb040602fa
+            0x020804010e010201020102010c0102fb040602fa06090e010201020102
+            0102010c0102fa040702f9
       code
-         argcount  : 4
-         nlocals   : 5
-         stacksize : 9
+         argcount  : 5
+         nlocals   : 6
+         stacksize : 10
          flags     : 11
          code
-            0x97007c01801674010000000000000000000064037c007c037c02740200
-            00000000000000000064019c047c04a4018e015300740500000000000000
-            00000064037c007c017c037c0274020000000000000000000064029c057c
-            04a4018e015300
-          56           0 RESUME                   0
+            0x97007c01801774010000000000000000000064037c007c037c02740200
+            0000000000000000007c0464019c057c05a4018e01530074050000000000
+            000000000064037c007c017c037c027402000000000000000000007c0464
+            029c067c05a4018e015300
+          59           0 RESUME                   0
          
-          63           2 LOAD_FAST                1 (method_name)
-                       4 POP_JUMP_FORWARD_IF_NOT_NONE    22 (to 50)
+          67           2 LOAD_FAST                1 (method_name)
+                       4 POP_JUMP_FORWARD_IF_NOT_NONE    23 (to 52)
          
-          64           6 LOAD_GLOBAL              1 (NULL + adecorate_method)
+          68           6 LOAD_GLOBAL              1 (NULL + adecorate_method)
                       18 LOAD_CONST               3 (())
          
-          65          20 LOAD_FAST                0 (name)
+          69          20 LOAD_FAST                0 (name)
+         
+          70          22 LOAD_FAST                3 (tlp_service_type)
+         
+          71          24 LOAD_FAST                2 (span_kind)
          
-          66          22 LOAD_FAST                3 (tlp_service_type)
+          72          26 LOAD_GLOBAL              2 (TaskSpanCapture)
          
-          67          24 LOAD_FAST                2 (span_kind)
+          73          38 LOAD_FAST                4 (flush_on_exit)
          
-          68          26 LOAD_GLOBAL              2 (TaskSpanCapture)
+          68          40 LOAD_CONST               1 (('name', 'tlp_service_type', 'span_kind', 'SpanCapture', 'flush_on_exit'))
+                      42 BUILD_CONST_KEY_MAP      5
          
-          64          38 LOAD_CONST               1 (('name', 'tlp_service_type', 'span_kind', 'SpanCapture'))
-                      40 BUILD_CONST_KEY_MAP      4
+          74          44 LOAD_FAST                5 (kwargs)
          
-          69          42 LOAD_FAST                4 (kwargs)
+          68          46 DICT_MERGE               1
+                      48 CALL_FUNCTION_EX         1
+                      50 RETURN_VALUE
          
-          64          44 DICT_MERGE               1
-                      46 CALL_FUNCTION_EX         1
-                      48 RETURN_VALUE
+          77     >>   52 LOAD_GLOBAL              5 (NULL + adecorate_class_method)
+                      64 LOAD_CONST               3 (())
          
-          72     >>   50 LOAD_GLOBAL              5 (NULL + adecorate_class_method)
-                      62 LOAD_CONST               3 (())
+          78          66 LOAD_FAST                0 (name)
          
-          73          64 LOAD_FAST                0 (name)
+          79          68 LOAD_FAST                1 (method_name)
          
-          74          66 LOAD_FAST                1 (method_name)
+          80          70 LOAD_FAST                3 (tlp_service_type)
          
-          75          68 LOAD_FAST                3 (tlp_service_type)
+          81          72 LOAD_FAST                2 (span_kind)
          
-          76          70 LOAD_FAST                2 (span_kind)
+          82          74 LOAD_GLOBAL              2 (TaskSpanCapture)
          
-          77          72 LOAD_GLOBAL              2 (TaskSpanCapture)
+          83          86 LOAD_FAST                4 (flush_on_exit)
          
-          72          84 LOAD_CONST               2 (('name', 'method_name', 'tlp_service_type', 'span_kind', 'SpanCapture'))
-                      86 BUILD_CONST_KEY_MAP      5
+          77          88 LOAD_CONST               2 (('name', 'method_name', 'tlp_service_type', 'span_kind', 'SpanCapture', 'flush_on_exit'))
+                      90 BUILD_CONST_KEY_MAP      6
          
-          78          88 LOAD_FAST                4 (kwargs)
+          84          92 LOAD_FAST                5 (kwargs)
          
-          72          90 DICT_MERGE               1
-                      92 CALL_FUNCTION_EX         1
-                      94 RETURN_VALUE
+          77          94 DICT_MERGE               1
+                      96 CALL_FUNCTION_EX         1
+                      98 RETURN_VALUE
          consts
             None
-            ('name', 'tlp_service_type', 'span_kind', 'SpanCapture')
-            ('name', 'method_name', 'tlp_service_type', 'span_kind', 'SpanCapture')
+            ('name', 'tlp_service_type', 'span_kind', 'SpanCapture', 'flush_on_exit')
+            ('name', 'method_name', 'tlp_service_type', 'span_kind', 'SpanCapture', 'flush_on_exit')
             ()
          names      ('adecorate_method', 'TaskSpanCapture', 'adecorate_class_method')
-         varnames   ('name', 'method_name', 'span_kind', 'tlp_service_type', 'kwargs')
+         varnames   ('name', 'method_name', 'span_kind', 'tlp_service_type', 'flush_on_exit', 'kwargs')
          freevars   ()
          cellvars   ()
          filename   '/Users/vuongngo/workspace/agiflow/packages/python/agiflow-sdk/agiflow/opentelemetry/trace_decorators/task.py'
          name       'atask'
-         firstlineno 56
+         firstlineno 59
          lnotab
-            0x020704010e010201020102010cfc040502fb06080e0102010201020102
-            010cfb040602fa
+            0x020804010e010201020102010c0102fb040602fa06090e010201020102
+            0102010c0102fa040702f9
       code
-         argcount  : 3
-         nlocals   : 4
-         stacksize : 8
+         argcount  : 4
+         nlocals   : 5
+         stacksize : 9
          flags     : 11
          code
             0x970074010000000000000000000064027c007c01740200000000000000
-            0000006a0200000000000000007c0264019c047c03a4018e015300
-          82           0 RESUME                   0
+            0000006a0200000000000000007c027c0364019c057c04a4018e015300
+          88           0 RESUME                   0
          
-          88           2 LOAD_GLOBAL              1 (NULL + task)
+          95           2 LOAD_GLOBAL              1 (NULL + task)
                       14 LOAD_CONST               2 (())
          
-          89          16 LOAD_FAST                0 (name)
+          96          16 LOAD_FAST                0 (name)
          
-          90          18 LOAD_FAST                1 (method_name)
+          97          18 LOAD_FAST                1 (method_name)
          
-          91          20 LOAD_GLOBAL              2 (AgiflowServiceTypes)
+          98          20 LOAD_GLOBAL              2 (AgiflowServiceTypes)
                       32 LOAD_ATTR                2 (AGENT)
          
-          92          42 LOAD_FAST                2 (span_kind)
+          99          42 LOAD_FAST                2 (span_kind)
+         
+         100          44 LOAD_FAST                3 (flush_on_exit)
          
-          88          44 LOAD_CONST               1 (('name', 'method_name', 'tlp_service_type', 'span_kind'))
-                      46 BUILD_CONST_KEY_MAP      4
+          95          46 LOAD_CONST               1 (('name', 'method_name', 'tlp_service_type', 'span_kind', 'flush_on_exit'))
+                      48 BUILD_CONST_KEY_MAP      5
          
-          93          48 LOAD_FAST                3 (kwargs)
+         101          50 LOAD_FAST                4 (kwargs)
          
-          88          50 DICT_MERGE               1
-                      52 CALL_FUNCTION_EX         1
-                      54 RETURN_VALUE
+          95          52 DICT_MERGE               1
+                      54 CALL_FUNCTION_EX         1
+                      56 RETURN_VALUE
          consts
             None
-            ('name', 'method_name', 'tlp_service_type', 'span_kind')
+            ('name', 'method_name', 'tlp_service_type', 'span_kind', 'flush_on_exit')
             ()
          names      ('task', 'AgiflowServiceTypes', 'AGENT')
-         varnames   ('name', 'method_name', 'span_kind', 'kwargs')
+         varnames   ('name', 'method_name', 'span_kind', 'flush_on_exit', 'kwargs')
          freevars   ()
          cellvars   ()
          filename   '/Users/vuongngo/workspace/agiflow/packages/python/agiflow-sdk/agiflow/opentelemetry/trace_decorators/task.py'
          name       'agent'
-         firstlineno 82
-         lnotab 0x02060e0102010201160102fc040502fb
+         firstlineno 88
+         lnotab 0x02070e01020102011601020102fb040602fa
       code
-         argcount  : 3
-         nlocals   : 4
-         stacksize : 8
+         argcount  : 4
+         nlocals   : 5
+         stacksize : 9
          flags     : 11
          code
             0x970074010000000000000000000064027c007c01740200000000000000
-            0000006a0200000000000000007c0264019c047c03a4018e015300
-          97           0 RESUME                   0
+            0000006a0200000000000000007c027c0364019c057c04a4018e015300
+         105           0 RESUME                   0
          
-         103           2 LOAD_GLOBAL              1 (NULL + task)
+         112           2 LOAD_GLOBAL              1 (NULL + task)
                       14 LOAD_CONST               2 (())
          
-         104          16 LOAD_FAST                0 (name)
+         113          16 LOAD_FAST                0 (name)
          
-         105          18 LOAD_FAST                1 (method_name)
+         114          18 LOAD_FAST                1 (method_name)
          
-         106          20 LOAD_GLOBAL              2 (AgiflowServiceTypes)
+         115          20 LOAD_GLOBAL              2 (AgiflowServiceTypes)
                       32 LOAD_ATTR                2 (TOOL)
          
-         107          42 LOAD_FAST                2 (span_kind)
+         116          42 LOAD_FAST                2 (span_kind)
+         
+         117          44 LOAD_FAST                3 (flush_on_exit)
          
-         103          44 LOAD_CONST               1 (('name', 'method_name', 'tlp_service_type', 'span_kind'))
-                      46 BUILD_CONST_KEY_MAP      4
+         112          46 LOAD_CONST               1 (('name', 'method_name', 'tlp_service_type', 'span_kind', 'flush_on_exit'))
+                      48 BUILD_CONST_KEY_MAP      5
          
-         108          48 LOAD_FAST                3 (kwargs)
+         118          50 LOAD_FAST                4 (kwargs)
          
-         103          50 DICT_MERGE               1
-                      52 CALL_FUNCTION_EX         1
-                      54 RETURN_VALUE
+         112          52 DICT_MERGE               1
+                      54 CALL_FUNCTION_EX         1
+                      56 RETURN_VALUE
          consts
             None
-            ('name', 'method_name', 'tlp_service_type', 'span_kind')
+            ('name', 'method_name', 'tlp_service_type', 'span_kind', 'flush_on_exit')
             ()
          names      ('task', 'AgiflowServiceTypes', 'TOOL')
-         varnames   ('name', 'method_name', 'span_kind', 'kwargs')
+         varnames   ('name', 'method_name', 'span_kind', 'flush_on_exit', 'kwargs')
          freevars   ()
          cellvars   ()
          filename   '/Users/vuongngo/workspace/agiflow/packages/python/agiflow-sdk/agiflow/opentelemetry/trace_decorators/task.py'
          name       'tool'
-         firstlineno 97
-         lnotab 0x02060e0102010201160102fc040502fb
+         firstlineno 105
+         lnotab 0x02070e01020102011601020102fb040602fa
       code
-         argcount  : 3
-         nlocals   : 4
-         stacksize : 8
+         argcount  : 4
+         nlocals   : 5
+         stacksize : 9
          flags     : 11
          code
             0x970074010000000000000000000064027c007c01740200000000000000
-            0000006a0200000000000000007c0264019c047c03a4018e015300
-         112           0 RESUME                   0
+            0000006a0200000000000000007c027c0364019c057c04a4018e015300
+         122           0 RESUME                   0
          
-         118           2 LOAD_GLOBAL              1 (NULL + atask)
+         129           2 LOAD_GLOBAL              1 (NULL + atask)
                       14 LOAD_CONST               2 (())
          
-         119          16 LOAD_FAST                0 (name)
+         130          16 LOAD_FAST                0 (name)
          
-         120          18 LOAD_FAST                1 (method_name)
+         131          18 LOAD_FAST                1 (method_name)
          
-         121          20 LOAD_GLOBAL              2 (AgiflowServiceTypes)
+         132          20 LOAD_GLOBAL              2 (AgiflowServiceTypes)
                       32 LOAD_ATTR                2 (AGENT)
          
-         122          42 LOAD_FAST                2 (span_kind)
+         133          42 LOAD_FAST                2 (span_kind)
+         
+         134          44 LOAD_FAST                3 (flush_on_exit)
          
-         118          44 LOAD_CONST               1 (('name', 'method_name', 'tlp_service_type', 'span_kind'))
-                      46 BUILD_CONST_KEY_MAP      4
+         129          46 LOAD_CONST               1 (('name', 'method_name', 'tlp_service_type', 'span_kind', 'flush_on_exit'))
+                      48 BUILD_CONST_KEY_MAP      5
          
-         123          48 LOAD_FAST                3 (kwargs)
+         135          50 LOAD_FAST                4 (kwargs)
          
-         118          50 DICT_MERGE               1
-                      52 CALL_FUNCTION_EX         1
-                      54 RETURN_VALUE
+         129          52 DICT_MERGE               1
+                      54 CALL_FUNCTION_EX         1
+                      56 RETURN_VALUE
          consts
             None
-            ('name', 'method_name', 'tlp_service_type', 'span_kind')
+            ('name', 'method_name', 'tlp_service_type', 'span_kind', 'flush_on_exit')
             ()
          names      ('atask', 'AgiflowServiceTypes', 'AGENT')
-         varnames   ('name', 'method_name', 'span_kind', 'kwargs')
+         varnames   ('name', 'method_name', 'span_kind', 'flush_on_exit', 'kwargs')
          freevars   ()
          cellvars   ()
          filename   '/Users/vuongngo/workspace/agiflow/packages/python/agiflow-sdk/agiflow/opentelemetry/trace_decorators/task.py'
          name       'aagent'
-         firstlineno 112
-         lnotab 0x02060e0102010201160102fc040502fb
+         firstlineno 122
+         lnotab 0x02070e01020102011601020102fb040602fa
       code
-         argcount  : 3
-         nlocals   : 4
-         stacksize : 8
+         argcount  : 4
+         nlocals   : 5
+         stacksize : 9
          flags     : 11
          code
             0x970074010000000000000000000064027c007c01740200000000000000
-            0000006a0200000000000000007c0264019c047c03a4018e015300
-         127           0 RESUME                   0
+            0000006a0200000000000000007c027c0364019c057c04a4018e015300
+         139           0 RESUME                   0
          
-         133           2 LOAD_GLOBAL              1 (NULL + atask)
+         146           2 LOAD_GLOBAL              1 (NULL + atask)
                       14 LOAD_CONST               2 (())
          
-         134          16 LOAD_FAST                0 (name)
+         147          16 LOAD_FAST                0 (name)
          
-         135          18 LOAD_FAST                1 (method_name)
+         148          18 LOAD_FAST                1 (method_name)
          
-         136          20 LOAD_GLOBAL              2 (AgiflowServiceTypes)
+         149          20 LOAD_GLOBAL              2 (AgiflowServiceTypes)
                       32 LOAD_ATTR                2 (TOOL)
          
-         137          42 LOAD_FAST                2 (span_kind)
+         150          42 LOAD_FAST                2 (span_kind)
+         
+         151          44 LOAD_FAST                3 (flush_on_exit)
          
-         133          44 LOAD_CONST               1 (('name', 'method_name', 'tlp_service_type', 'span_kind'))
-                      46 BUILD_CONST_KEY_MAP      4
+         146          46 LOAD_CONST               1 (('name', 'method_name', 'tlp_service_type', 'span_kind', 'flush_on_exit'))
+                      48 BUILD_CONST_KEY_MAP      5
          
-         138          48 LOAD_FAST                3 (kwargs)
+         152          50 LOAD_FAST                4 (kwargs)
          
-         133          50 DICT_MERGE               1
-                      52 CALL_FUNCTION_EX         1
-                      54 RETURN_VALUE
+         146          52 DICT_MERGE               1
+                      54 CALL_FUNCTION_EX         1
+                      56 RETURN_VALUE
          consts
             None
-            ('name', 'method_name', 'tlp_service_type', 'span_kind')
+            ('name', 'method_name', 'tlp_service_type', 'span_kind', 'flush_on_exit')
             ()
          names      ('atask', 'AgiflowServiceTypes', 'TOOL')
-         varnames   ('name', 'method_name', 'span_kind', 'kwargs')
+         varnames   ('name', 'method_name', 'span_kind', 'flush_on_exit', 'kwargs')
          freevars   ()
          cellvars   ()
          filename   '/Users/vuongngo/workspace/agiflow/packages/python/agiflow-sdk/agiflow/opentelemetry/trace_decorators/task.py'
          name       'atool'
-         firstlineno 127
-         lnotab 0x02060e0102010201160102fc040502fb
+         firstlineno 139
+         lnotab 0x02070e01020102011601020102fb040602fa
    names      ('typing', 'Optional', 'Unpack', 'agiflow.opentelemetry.convention', 'SpanAttributes', 'AgiflowServiceTypes', 'agiflow.opentelemetry.trace_decorators.helper', 'SharedKwargsWithHooks', 'agiflow.opentelemetry.trace_decorators.wrapper', 'BaseSpanCapture', 'decorate_method', 'decorate_class_method', 'adecorate_method', 'adecorate_class_method', 'opentelemetry.trace', 'SpanKind', 'TaskSpanCapture', 'INTERNAL', 'TASK', 'str', 'task', 'atask', 'agent', 'tool', 'aagent', 'atool')
    varnames   ()
    freevars   ()
    cellvars   ()
    filename   '/Users/vuongngo/workspace/agiflow/packages/python/agiflow-sdk/agiflow/opentelemetry/trace_decorators/task.py'
    name       '<module>'
    firstlineno 1
    lnotab
-      0x00ff0201100210020c031c070c031c0c020102010c010cfc04010eff02
-      020efe02040efc02050efb081c020102010c010cfc04010eff02020efe02
-      040efc02050efb081b020102010cfd04010eff02020efe02040efc081002
-      0102010cfd04010eff02020efe02040efc0810020102010cfd04010eff02
-      020efe02040efc0810020102010cfd04010eff02020efe02040efc
+      0x00ff0201100210020c031c070c031c0c020102010c010c0102fb04010e
+      ff02020efe02040efc02060efa081f020102010c010c0102fb04010eff02
+      020efe02040efc02060efa081e020102010c0102fc04010eff02020efe02
+      050efb0812020102010c0102fc04010eff02020efe02050efb0812020102
+      010c0102fc04010eff02020efe02050efb0812020102010c0102fc04010e
+      ff02020efe02050efb
```

### Comparing `agiflow_sdk-0.0.4/agiflow/opentelemetry/trace_decorators/__pycache__/workflow.cpython-311.pyc` & `agiflow_sdk-0.0.5/agiflow/opentelemetry/trace_decorators/__pycache__/workflow.cpython-311.pyc`

 * *Files 23% similar despite different names*

#### Python bytecode

```diff
@@ -1,10 +1,10 @@
 magic:    0xa70d0d0a
-moddate:  0x220c5d66 (Mon Jun  3 00:19:46 2024 UTC)
-files sz: 2241
+moddate:  0x97895d66 (Mon Jun  3 09:15:03 2024 UTC)
+files sz: 2294
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
    
-    37         126 LOAD_CONST               9 (None)
+    33         126 LOAD_CONST               9 (None)
    
-    38         128 LOAD_CONST               9 (None)
+    34         128 LOAD_CONST               9 (None)
    
-    39         130 LOAD_NAME               17 (SpanKind)
+    35         130 LOAD_NAME               17 (SpanKind)
                132 LOAD_ATTR               19 (INTERNAL)
    
-    36         142 BUILD_TUPLE              3
+    32         142 BUILD_TUPLE              3
                144 LOAD_CONST              10 ('name')
    
-    37         146 LOAD_NAME                1 (Optional)
+    33         146 LOAD_NAME                1 (Optional)
                148 LOAD_NAME               20 (str)
                150 BINARY_SUBSCR
    
-    36         160 LOAD_CONST              11 ('method_name')
+    32         160 LOAD_CONST              11 ('method_name')
    
-    38         162 LOAD_NAME                1 (Optional)
+    34         162 LOAD_NAME                1 (Optional)
                164 LOAD_NAME               20 (str)
                166 BINARY_SUBSCR
    
-    36         176 LOAD_CONST              12 ('kwargs')
+    32         176 LOAD_CONST              12 ('kwargs')
    
-    40         178 LOAD_NAME                2 (Unpack)
+    36         178 LOAD_NAME                2 (Unpack)
                180 LOAD_NAME                9 (SharedKwargsWithHooks)
                182 BINARY_SUBSCR
    
-    36         192 BUILD_TUPLE              6
-               194 LOAD_CONST              13 (<code object workflow, file "/Users/vuongngo/workspace/agiflow/packages/python/agiflow-sdk/agiflow/opentelemetry/trace_decorators/workflow.py", line 36>)
+    32         192 BUILD_TUPLE              6
+               194 LOAD_CONST              13 (<code object workflow, file "/Users/vuongngo/workspace/agiflow/packages/python/agiflow-sdk/agiflow/opentelemetry/trace_decorators/workflow.py", line 32>)
                196 MAKE_FUNCTION            5 (defaults, annotations)
                198 STORE_NAME              21 (workflow)
    
-    61         200 LOAD_CONST               9 (None)
+    59         200 LOAD_CONST               9 (None)
    
-    62         202 LOAD_CONST               9 (None)
+    60         202 LOAD_CONST               9 (None)
    
-    63         204 LOAD_NAME               17 (SpanKind)
+    61         204 LOAD_NAME               17 (SpanKind)
                206 LOAD_ATTR               19 (INTERNAL)
    
-    60         216 BUILD_TUPLE              3
+    58         216 BUILD_TUPLE              3
                218 LOAD_CONST              10 ('name')
    
-    61         220 LOAD_NAME                1 (Optional)
+    59         220 LOAD_NAME                1 (Optional)
                222 LOAD_NAME               20 (str)
                224 BINARY_SUBSCR
    
-    60         234 LOAD_CONST              11 ('method_name')
+    58         234 LOAD_CONST              11 ('method_name')
    
-    62         236 LOAD_NAME                1 (Optional)
+    60         236 LOAD_NAME                1 (Optional)
                238 LOAD_NAME               20 (str)
                240 BINARY_SUBSCR
    
-    60         250 LOAD_CONST              12 ('kwargs')
+    58         250 LOAD_CONST              12 ('kwargs')
    
-    64         252 LOAD_NAME                2 (Unpack)
+    62         252 LOAD_NAME                2 (Unpack)
                254 LOAD_NAME                9 (SharedKwargsWithHooks)
                256 BINARY_SUBSCR
    
-    60         266 BUILD_TUPLE              6
-               268 LOAD_CONST              14 (<code object aworkflow, file "/Users/vuongngo/workspace/agiflow/packages/python/agiflow-sdk/agiflow/opentelemetry/trace_decorators/workflow.py", line 60>)
+    58         266 BUILD_TUPLE              6
+               268 LOAD_CONST              14 (<code object aworkflow, file "/Users/vuongngo/workspace/agiflow/packages/python/agiflow-sdk/agiflow/opentelemetry/trace_decorators/workflow.py", line 58>)
                270 MAKE_FUNCTION            5 (defaults, annotations)
                272 STORE_NAME              22 (aworkflow)
                274 LOAD_CONST               9 (None)
                276 RETURN_VALUE
    consts
       0
       ('Optional', 'Unpack')
@@ -157,16 +157,15 @@
       code
          argcount  : 0
          nlocals   : 0
          stacksize : 2
          flags     : 0
          code
             0x8700970065005a0164005a0288006601640184085a0388006601640284
-            085a04650564038400a6000000ab0000000000000000005a06880078015a
-            075300
+            085a04880078015a055300
                        0 MAKE_CELL                0 (__class__)
          
           19           2 RESUME                   0
                        4 LOAD_NAME                0 (__name__)
                        6 STORE_NAME               1 (__module__)
                        8 LOAD_CONST               0 ('WorkflowSpanCapture')
                       10 STORE_NAME               2 (__qualname__)
@@ -178,28 +177,18 @@
                       20 STORE_NAME               3 (__init__)
          
           25          22 LOAD_CLOSURE             0 (__class__)
                       24 BUILD_TUPLE              1
                       26 LOAD_CONST               2 (<code object capture_input, file "/Users/vuongngo/workspace/agiflow/packages/python/agiflow-sdk/agiflow/opentelemetry/trace_decorators/workflow.py", line 25>)
                       28 MAKE_FUNCTION            8 (closure)
                       30 STORE_NAME               4 (capture_input)
-         
-          31          32 LOAD_NAME                5 (staticmethod)
-         
-          32          34 LOAD_CONST               3 (<code object is_flush_on_exit, file "/Users/vuongngo/workspace/agiflow/packages/python/agiflow-sdk/agiflow/opentelemetry/trace_decorators/workflow.py", line 31>)
-                      36 MAKE_FUNCTION            0
-         
-          31          38 PRECALL                  0
-                      42 CALL                     0
-         
-          32          52 STORE_NAME               6 (is_flush_on_exit)
-                      54 LOAD_CLOSURE             0 (__class__)
-                      56 COPY                     1
-                      58 STORE_NAME               7 (__classcell__)
-                      60 RETURN_VALUE
+                      32 LOAD_CLOSURE             0 (__class__)
+                      34 COPY                     1
+                      36 STORE_NAME               5 (__classcell__)
+                      38 RETURN_VALUE
          consts
             'WorkflowSpanCapture'
             code
                argcount  : 1
                nlocals   : 4
                stacksize : 5
                flags     : 15
@@ -292,193 +281,182 @@
                varnames   ('self',)
                freevars   ('__class__',)
                cellvars   ()
                filename   '/Users/vuongngo/workspace/agiflow/packages/python/agiflow-sdk/agiflow/opentelemetry/trace_decorators/workflow.py'
                name       'capture_input'
                firstlineno 25
                lnotab 0x04014001180122ff
-            code
-               argcount  : 0
-               nlocals   : 0
-               stacksize : 1
-               flags     : 3
-               code 0x970064015300
-                31           0 RESUME                   0
-               
-                33           2 LOAD_CONST               1 (True)
-                             4 RETURN_VALUE
-               consts
-                  None
-                  True
-               names      ()
-               varnames   ()
-               freevars   ()
-               cellvars   ()
-               filename   '/Users/vuongngo/workspace/agiflow/packages/python/agiflow-sdk/agiflow/opentelemetry/trace_decorators/workflow.py'
-               name       'is_flush_on_exit'
-               firstlineno 31
-               lnotab 0x0202
-         names      ('__name__', '__module__', '__qualname__', '__init__', 'capture_input', 'staticmethod', 'is_flush_on_exit', '__classcell__')
+         names      ('__name__', '__module__', '__qualname__', '__init__', 'capture_input', '__classcell__')
          varnames   ()
          freevars   ()
          cellvars   ('__class__',)
          filename   '/Users/vuongngo/workspace/agiflow/packages/python/agiflow-sdk/agiflow/opentelemetry/trace_decorators/workflow.py'
          name       'WorkflowSpanCapture'
          firstlineno 19
-         lnotab 0x0c010a050a06020104ff0e01
+         lnotab 0x0c010a05
       'WorkflowSpanCapture'
       None
       'name'
       'method_name'
       'kwargs'
       code
          argcount  : 3
          nlocals   : 4
-         stacksize : 8
+         stacksize : 9
          flags     : 11
          code
-            0x97007c01802074010000000000000000000064027c0074020000000000
+            0x97007c01802174010000000000000000000064037c0074020000000000
             00000000006a0200000000000000007c0274060000000000000000000064
-            019c047c03a4018e01530074090000000000000000000064027c00740200
-            0000000000000000006a0200000000000000007c02740600000000000000
-            00000064019c047c03a4018e015300
-          36           0 RESUME                   0
+            0164029c057c03a4018e01530074090000000000000000000064037c0074
+            02000000000000000000006a0200000000000000007c0274060000000000
+            0000000000640164029c057c03a4018e015300
+          32           0 RESUME                   0
          
-          42           2 LOAD_FAST                1 (method_name)
-                       4 POP_JUMP_FORWARD_IF_NOT_NONE    32 (to 70)
+          38           2 LOAD_FAST                1 (method_name)
+                       4 POP_JUMP_FORWARD_IF_NOT_NONE    33 (to 72)
          
-          43           6 LOAD_GLOBAL              1 (NULL + decorate_method)
-                      18 LOAD_CONST               2 (())
+          39           6 LOAD_GLOBAL              1 (NULL + decorate_method)
+                      18 LOAD_CONST               3 (())
          
-          44          20 LOAD_FAST                0 (name)
+          40          20 LOAD_FAST                0 (name)
          
-          45          22 LOAD_GLOBAL              2 (AgiflowServiceTypes)
+          41          22 LOAD_GLOBAL              2 (AgiflowServiceTypes)
                       34 LOAD_ATTR                2 (WORKFLOW)
          
-          46          44 LOAD_FAST                2 (span_kind)
+          42          44 LOAD_FAST                2 (span_kind)
+         
+          43          46 LOAD_GLOBAL              6 (WorkflowSpanCapture)
          
-          47          46 LOAD_GLOBAL              6 (WorkflowSpanCapture)
+          44          58 LOAD_CONST               1 (True)
          
-          43          58 LOAD_CONST               1 (('name', 'tlp_service_type', 'span_kind', 'SpanCapture'))
-                      60 BUILD_CONST_KEY_MAP      4
+          39          60 LOAD_CONST               2 (('name', 'tlp_service_type', 'span_kind', 'SpanCapture', 'flush_on_exit'))
+                      62 BUILD_CONST_KEY_MAP      5
          
-          48          62 LOAD_FAST                3 (kwargs)
+          45          64 LOAD_FAST                3 (kwargs)
          
-          43          64 DICT_MERGE               1
-                      66 CALL_FUNCTION_EX         1
-                      68 RETURN_VALUE
+          39          66 DICT_MERGE               1
+                      68 CALL_FUNCTION_EX         1
+                      70 RETURN_VALUE
          
-          51     >>   70 LOAD_GLOBAL              9 (NULL + decorate_class_method)
-                      82 LOAD_CONST               2 (())
+          48     >>   72 LOAD_GLOBAL              9 (NULL + decorate_class_method)
+                      84 LOAD_CONST               3 (())
          
-          52          84 LOAD_FAST                0 (name)
+          49          86 LOAD_FAST                0 (name)
          
-          53          86 LOAD_GLOBAL              2 (AgiflowServiceTypes)
-                      98 LOAD_ATTR                2 (WORKFLOW)
+          50          88 LOAD_GLOBAL              2 (AgiflowServiceTypes)
+                     100 LOAD_ATTR                2 (WORKFLOW)
          
-          54         108 LOAD_FAST                2 (span_kind)
+          51         110 LOAD_FAST                2 (span_kind)
          
-          55         110 LOAD_GLOBAL              6 (WorkflowSpanCapture)
+          52         112 LOAD_GLOBAL              6 (WorkflowSpanCapture)
          
-          51         122 LOAD_CONST               1 (('name', 'tlp_service_type', 'span_kind', 'SpanCapture'))
-                     124 BUILD_CONST_KEY_MAP      4
+          53         124 LOAD_CONST               1 (True)
          
-          56         126 LOAD_FAST                3 (kwargs)
+          48         126 LOAD_CONST               2 (('name', 'tlp_service_type', 'span_kind', 'SpanCapture', 'flush_on_exit'))
+                     128 BUILD_CONST_KEY_MAP      5
          
-          51         128 DICT_MERGE               1
-                     130 CALL_FUNCTION_EX         1
-                     132 RETURN_VALUE
+          54         130 LOAD_FAST                3 (kwargs)
+         
+          48         132 DICT_MERGE               1
+                     134 CALL_FUNCTION_EX         1
+                     136 RETURN_VALUE
          consts
             None
-            ('name', 'tlp_service_type', 'span_kind', 'SpanCapture')
+            True
+            ('name', 'tlp_service_type', 'span_kind', 'SpanCapture', 'flush_on_exit')
             ()
          names      ('decorate_method', 'AgiflowServiceTypes', 'WORKFLOW', 'WorkflowSpanCapture', 'decorate_class_method')
          varnames   ('name', 'method_name', 'span_kind', 'kwargs')
          freevars   ()
          cellvars   ()
          filename   '/Users/vuongngo/workspace/agiflow/packages/python/agiflow-sdk/agiflow/opentelemetry/trace_decorators/workflow.py'
          name       'workflow'
-         firstlineno 36
+         firstlineno 32
          lnotab
-            0x020604010e010201160102010cfc040502fb06080e010201160102010c
-            fc040502fb
+            0x020604010e010201160102010c0102fb040602fa06090e010201160102
+            010c0102fb040602fa
       code
          argcount  : 3
          nlocals   : 4
-         stacksize : 8
+         stacksize : 9
          flags     : 11
          code
-            0x97007c01802074010000000000000000000064027c0074020000000000
+            0x97007c01802174010000000000000000000064037c0074020000000000
             00000000006a0200000000000000007c0274060000000000000000000064
-            019c047c03a4018e01530074090000000000000000000064027c00740200
-            0000000000000000006a0200000000000000007c02740600000000000000
-            00000064019c047c03a4018e015300
-          60           0 RESUME                   0
+            0164029c057c03a4018e01530074090000000000000000000064037c0074
+            02000000000000000000006a0200000000000000007c0274060000000000
+            0000000000640164029c057c03a4018e015300
+          58           0 RESUME                   0
          
-          66           2 LOAD_FAST                1 (method_name)
-                       4 POP_JUMP_FORWARD_IF_NOT_NONE    32 (to 70)
+          64           2 LOAD_FAST                1 (method_name)
+                       4 POP_JUMP_FORWARD_IF_NOT_NONE    33 (to 72)
          
-          67           6 LOAD_GLOBAL              1 (NULL + adecorate_method)
-                      18 LOAD_CONST               2 (())
+          65           6 LOAD_GLOBAL              1 (NULL + adecorate_method)
+                      18 LOAD_CONST               3 (())
          
-          68          20 LOAD_FAST                0 (name)
+          66          20 LOAD_FAST                0 (name)
          
-          69          22 LOAD_GLOBAL              2 (AgiflowServiceTypes)
+          67          22 LOAD_GLOBAL              2 (AgiflowServiceTypes)
                       34 LOAD_ATTR                2 (WORKFLOW)
          
-          70          44 LOAD_FAST                2 (span_kind)
+          68          44 LOAD_FAST                2 (span_kind)
+         
+          69          46 LOAD_GLOBAL              6 (WorkflowSpanCapture)
+         
+          70          58 LOAD_CONST               1 (True)
          
-          71          46 LOAD_GLOBAL              6 (WorkflowSpanCapture)
+          65          60 LOAD_CONST               2 (('name', 'tlp_service_type', 'span_kind', 'SpanCapture', 'flush_on_exit'))
+                      62 BUILD_CONST_KEY_MAP      5
          
-          67          58 LOAD_CONST               1 (('name', 'tlp_service_type', 'span_kind', 'SpanCapture'))
-                      60 BUILD_CONST_KEY_MAP      4
+          71          64 LOAD_FAST                3 (kwargs)
          
-          72          62 LOAD_FAST                3 (kwargs)
+          65          66 DICT_MERGE               1
+                      68 CALL_FUNCTION_EX         1
+                      70 RETURN_VALUE
          
-          67          64 DICT_MERGE               1
-                      66 CALL_FUNCTION_EX         1
-                      68 RETURN_VALUE
+          74     >>   72 LOAD_GLOBAL              9 (NULL + adecorate_class_method)
+                      84 LOAD_CONST               3 (())
          
-          75     >>   70 LOAD_GLOBAL              9 (NULL + adecorate_class_method)
-                      82 LOAD_CONST               2 (())
+          75          86 LOAD_FAST                0 (name)
          
-          76          84 LOAD_FAST                0 (name)
+          76          88 LOAD_GLOBAL              2 (AgiflowServiceTypes)
+                     100 LOAD_ATTR                2 (WORKFLOW)
          
-          77          86 LOAD_GLOBAL              2 (AgiflowServiceTypes)
-                      98 LOAD_ATTR                2 (WORKFLOW)
+          77         110 LOAD_FAST                2 (span_kind)
          
-          78         108 LOAD_FAST                2 (span_kind)
+          78         112 LOAD_GLOBAL              6 (WorkflowSpanCapture)
          
-          79         110 LOAD_GLOBAL              6 (WorkflowSpanCapture)
+          79         124 LOAD_CONST               1 (True)
          
-          75         122 LOAD_CONST               1 (('name', 'tlp_service_type', 'span_kind', 'SpanCapture'))
-                     124 BUILD_CONST_KEY_MAP      4
+          74         126 LOAD_CONST               2 (('name', 'tlp_service_type', 'span_kind', 'SpanCapture', 'flush_on_exit'))
+                     128 BUILD_CONST_KEY_MAP      5
          
-          80         126 LOAD_FAST                3 (kwargs)
+          80         130 LOAD_FAST                3 (kwargs)
          
-          75         128 DICT_MERGE               1
-                     130 CALL_FUNCTION_EX         1
-                     132 RETURN_VALUE
+          74         132 DICT_MERGE               1
+                     134 CALL_FUNCTION_EX         1
+                     136 RETURN_VALUE
          consts
             None
-            ('name', 'tlp_service_type', 'span_kind', 'SpanCapture')
+            True
+            ('name', 'tlp_service_type', 'span_kind', 'SpanCapture', 'flush_on_exit')
             ()
          names      ('adecorate_method', 'AgiflowServiceTypes', 'WORKFLOW', 'WorkflowSpanCapture', 'adecorate_class_method')
          varnames   ('name', 'method_name', 'span_kind', 'kwargs')
          freevars   ()
          cellvars   ()
          filename   '/Users/vuongngo/workspace/agiflow/packages/python/agiflow-sdk/agiflow/opentelemetry/trace_decorators/workflow.py'
          name       'aworkflow'
-         firstlineno 60
+         firstlineno 58
          lnotab
-            0x020604010e010201160102010cfc040502fb06080e010201160102010c
-            fc040502fb
+            0x020604010e010201160102010c0102fb040602fa06090e010201160102
+            010c0102fb040602fa
    names      ('typing', 'Optional', 'Unpack', 'agiflow.opentelemetry.convention', 'SpanAttributes', 'AgiflowServiceTypes', 'agiflow.opentelemetry.context', 'set_workflow_name', 'agiflow.opentelemetry.trace_decorators.helper', 'SharedKwargsWithHooks', 'agiflow.opentelemetry.trace_decorators.wrapper', 'BaseSpanCapture', 'decorate_method', 'decorate_class_method', 'adecorate_method', 'adecorate_class_method', 'opentelemetry.trace', 'SpanKind', 'WorkflowSpanCapture', 'INTERNAL', 'str', 'workflow', 'aworkflow')
    varnames   ()
    freevars   ()
    cellvars   ()
    filename   '/Users/vuongngo/workspace/agiflow/packages/python/agiflow-sdk/agiflow/opentelemetry/trace_decorators/workflow.py'
    name       '<module>'
    firstlineno 1
    lnotab
-      0x00ff0201100210020c010c031c070c031c12020102010cfd04010eff02
-      020efe02040efc0819020102010cfd04010eff02020efe02040efc
+      0x00ff0201100210020c010c031c070c031c0e020102010cfd04010eff02
+      020efe02040efc081b020102010cfd04010eff02020efe02040efc
```

### Comparing `agiflow_sdk-0.0.4/agiflow/opentelemetry/trace_decorators/__pycache__/wrapper.cpython-311.pyc` & `agiflow_sdk-0.0.5/agiflow/opentelemetry/trace_decorators/__pycache__/wrapper.cpython-311.pyc`

 * *Files 7% similar despite different names*

#### Python bytecode

```diff
@@ -1,10 +1,10 @@
 magic:    0xa70d0d0a
-moddate:  0x7c105d66 (Mon Jun  3 00:38:20 2024 UTC)
-files sz: 15064
+moddate:  0x7d895d66 (Mon Jun  3 09:14:37 2024 UTC)
+files sz: 15148
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 10
    flags     : 0
    code
       0x9700640064016c006d015a010100640064026c026d035a030100640064
@@ -16,26 +16,27 @@
       1f6d205a2001006400640e6c216d225a226d235a2301006400640f6c246d
       255a250100640064106c266d275a276d285a286d295a296d2a5a2a6d2b5a
       2b6d2c5a2c6d2d5a2d0100640064116c2e6d2f5a2f6d305a300100020065
       096412a6010000ab0100000000000000005a31020065046a320000000000
       0000006533a6010000ab0100000000000000005a34020047006413840064
       146501650a653119000000000000000000a6040000ab0400000000000000
       005a35020047006415840064166535a6030000ab0300000000000000005a
-      36640365136a37000000000000000065166a380000000000000000653666
-      046417650865391900000000000000000064186508651319000000000000
-      0000006419650b6520190000000000000000006606641a84055a3a640365
-      136a37000000000000000065166a38000000000000000065366604641765
-      086539190000000000000000006418650865131900000000000000000064
-      19650b6520190000000000000000006606641b84055a3b65136a37000000
-      000000000065166a38000000000000000065366603641765086539190000
-      00000000000000641c653964186508651319000000000000000000641d65
-      0b6520190000000000000000006608641e84055a3c65136a370000000000
-      00000065166a380000000000000000653666036417650865391900000000
-      0000000000641c653964186508651319000000000000000000641d650b65
-      20190000000000000000006608641f84055a3d64035300
+      36640365136a37000000000000000065166a380000000000000000653664
+      176605641865086539190000000000000000006419650865131900000000
+      0000000000641a650b6520190000000000000000006606641b84055a3a64
+      0365136a37000000000000000065166a3800000000000000006536641766
+      056418650865391900000000000000000064196508651319000000000000
+      000000641a650b6520190000000000000000006606641c84055a3b65136a
+      37000000000000000065166a380000000000000000653664176604641865
+      08653919000000000000000000641d653964196508651319000000000000
+      000000641e650b6520190000000000000000006608641f84055a3c65136a
+      37000000000000000065166a380000000000000000653664176604641865
+      08653919000000000000000000641d653964196508651319000000000000
+      000000641e650b6520190000000000000000006608642084055a3d640353
+      00
      0           0 RESUME                   0
    
      1           2 LOAD_CONST               0 (0)
                  4 LOAD_CONST               1 (('ABC',))
                  6 IMPORT_NAME              0 (abc)
                  8 IMPORT_FROM              1 (ABC)
                 10 STORE_NAME               1 (ABC)
@@ -217,155 +218,163 @@
                368 MAKE_FUNCTION            0
                370 LOAD_CONST              22 ('BaseSpanCapture')
                372 LOAD_NAME               53 (AbstractSpanCapture)
                374 PRECALL                  3
                378 CALL                     3
                388 STORE_NAME              54 (BaseSpanCapture)
    
-   252         390 LOAD_CONST               3 (None)
+   248         390 LOAD_CONST               3 (None)
    
-   253         392 LOAD_NAME               19 (AgiflowServiceTypes)
+   249         392 LOAD_NAME               19 (AgiflowServiceTypes)
                394 LOAD_ATTR               55 (TASK)
    
-   254         404 LOAD_NAME               22 (SpanKind)
+   250         404 LOAD_NAME               22 (SpanKind)
                406 LOAD_ATTR               56 (INTERNAL)
    
-   255         416 LOAD_NAME               54 (BaseSpanCapture)
+   251         416 LOAD_NAME               54 (BaseSpanCapture)
    
-   251         418 BUILD_TUPLE              4
-               420 LOAD_CONST              23 ('name')
+   252         418 LOAD_CONST              23 (False)
    
-   252         422 LOAD_NAME                8 (Optional)
-               424 LOAD_NAME               57 (str)
-               426 BINARY_SUBSCR
+   247         420 BUILD_TUPLE              5
+               422 LOAD_CONST              24 ('name')
    
-   251         436 LOAD_CONST              24 ('tlp_service_type')
+   248         424 LOAD_NAME                8 (Optional)
+               426 LOAD_NAME               57 (str)
+               428 BINARY_SUBSCR
    
-   253         438 LOAD_NAME                8 (Optional)
-               440 LOAD_NAME               19 (AgiflowServiceTypes)
-               442 BINARY_SUBSCR
+   247         438 LOAD_CONST              25 ('tlp_service_type')
    
-   251         452 LOAD_CONST              25 ('config')
+   249         440 LOAD_NAME                8 (Optional)
+               442 LOAD_NAME               19 (AgiflowServiceTypes)
+               444 BINARY_SUBSCR
    
-   256         454 LOAD_NAME               11 (Unpack)
-               456 LOAD_NAME               32 (SharedKwargsWithHooks)
-               458 BINARY_SUBSCR
+   247         454 LOAD_CONST              26 ('config')
    
-   251         468 BUILD_TUPLE              6
-               470 LOAD_CONST              26 (<code object decorate_method, file "/Users/vuongngo/workspace/agiflow/packages/python/agiflow-sdk/agiflow/opentelemetry/trace_decorators/wrapper.py", line 251>)
-               472 MAKE_FUNCTION            5 (defaults, annotations)
-               474 STORE_NAME              58 (decorate_method)
+   253         456 LOAD_NAME               11 (Unpack)
+               458 LOAD_NAME               32 (SharedKwargsWithHooks)
+               460 BINARY_SUBSCR
    
-   320         476 LOAD_CONST               3 (None)
+   247         470 BUILD_TUPLE              6
+               472 LOAD_CONST              27 (<code object decorate_method, file "/Users/vuongngo/workspace/agiflow/packages/python/agiflow-sdk/agiflow/opentelemetry/trace_decorators/wrapper.py", line 247>)
+               474 MAKE_FUNCTION            5 (defaults, annotations)
+               476 STORE_NAME              58 (decorate_method)
    
-   321         478 LOAD_NAME               19 (AgiflowServiceTypes)
-               480 LOAD_ATTR               55 (TASK)
+   317         478 LOAD_CONST               3 (None)
    
-   322         490 LOAD_NAME               22 (SpanKind)
-               492 LOAD_ATTR               56 (INTERNAL)
+   318         480 LOAD_NAME               19 (AgiflowServiceTypes)
+               482 LOAD_ATTR               55 (TASK)
    
-   323         502 LOAD_NAME               54 (BaseSpanCapture)
+   319         492 LOAD_NAME               22 (SpanKind)
+               494 LOAD_ATTR               56 (INTERNAL)
    
-   319         504 BUILD_TUPLE              4
-               506 LOAD_CONST              23 ('name')
+   320         504 LOAD_NAME               54 (BaseSpanCapture)
    
-   320         508 LOAD_NAME                8 (Optional)
-               510 LOAD_NAME               57 (str)
-               512 BINARY_SUBSCR
+   321         506 LOAD_CONST              23 (False)
    
-   319         522 LOAD_CONST              24 ('tlp_service_type')
+   316         508 BUILD_TUPLE              5
+               510 LOAD_CONST              24 ('name')
    
-   321         524 LOAD_NAME                8 (Optional)
-               526 LOAD_NAME               19 (AgiflowServiceTypes)
-               528 BINARY_SUBSCR
+   317         512 LOAD_NAME                8 (Optional)
+               514 LOAD_NAME               57 (str)
+               516 BINARY_SUBSCR
    
-   319         538 LOAD_CONST              25 ('config')
+   316         526 LOAD_CONST              25 ('tlp_service_type')
    
-   324         540 LOAD_NAME               11 (Unpack)
-               542 LOAD_NAME               32 (SharedKwargsWithHooks)
-               544 BINARY_SUBSCR
+   318         528 LOAD_NAME                8 (Optional)
+               530 LOAD_NAME               19 (AgiflowServiceTypes)
+               532 BINARY_SUBSCR
    
-   319         554 BUILD_TUPLE              6
-               556 LOAD_CONST              27 (<code object adecorate_method, file "/Users/vuongngo/workspace/agiflow/packages/python/agiflow-sdk/agiflow/opentelemetry/trace_decorators/wrapper.py", line 319>)
-               558 MAKE_FUNCTION            5 (defaults, annotations)
-               560 STORE_NAME              59 (adecorate_method)
+   316         542 LOAD_CONST              26 ('config')
    
-   390         562 LOAD_NAME               19 (AgiflowServiceTypes)
-               564 LOAD_ATTR               55 (TASK)
+   322         544 LOAD_NAME               11 (Unpack)
+               546 LOAD_NAME               32 (SharedKwargsWithHooks)
+               548 BINARY_SUBSCR
    
-   391         574 LOAD_NAME               22 (SpanKind)
-               576 LOAD_ATTR               56 (INTERNAL)
+   316         558 BUILD_TUPLE              6
+               560 LOAD_CONST              28 (<code object adecorate_method, file "/Users/vuongngo/workspace/agiflow/packages/python/agiflow-sdk/agiflow/opentelemetry/trace_decorators/wrapper.py", line 316>)
+               562 MAKE_FUNCTION            5 (defaults, annotations)
+               564 STORE_NAME              59 (adecorate_method)
    
-   392         586 LOAD_NAME               54 (BaseSpanCapture)
+   388         566 LOAD_NAME               19 (AgiflowServiceTypes)
+               568 LOAD_ATTR               55 (TASK)
    
-   387         588 BUILD_TUPLE              3
-               590 LOAD_CONST              23 ('name')
+   389         578 LOAD_NAME               22 (SpanKind)
+               580 LOAD_ATTR               56 (INTERNAL)
    
-   388         592 LOAD_NAME                8 (Optional)
-               594 LOAD_NAME               57 (str)
-               596 BINARY_SUBSCR
+   390         590 LOAD_NAME               54 (BaseSpanCapture)
    
-   387         606 LOAD_CONST              28 ('method_name')
+   391         592 LOAD_CONST              23 (False)
    
-   389         608 LOAD_NAME               57 (str)
+   385         594 BUILD_TUPLE              4
+               596 LOAD_CONST              24 ('name')
    
-   387         610 LOAD_CONST              24 ('tlp_service_type')
+   386         598 LOAD_NAME                8 (Optional)
+               600 LOAD_NAME               57 (str)
+               602 BINARY_SUBSCR
    
-   390         612 LOAD_NAME                8 (Optional)
-               614 LOAD_NAME               19 (AgiflowServiceTypes)
-               616 BINARY_SUBSCR
+   385         612 LOAD_CONST              29 ('method_name')
    
-   387         626 LOAD_CONST              29 ('kwargs')
+   387         614 LOAD_NAME               57 (str)
    
-   393         628 LOAD_NAME               11 (Unpack)
-               630 LOAD_NAME               32 (SharedKwargsWithHooks)
-               632 BINARY_SUBSCR
+   385         616 LOAD_CONST              25 ('tlp_service_type')
    
-   387         642 BUILD_TUPLE              8
-               644 LOAD_CONST              30 (<code object decorate_class_method, file "/Users/vuongngo/workspace/agiflow/packages/python/agiflow-sdk/agiflow/opentelemetry/trace_decorators/wrapper.py", line 387>)
-               646 MAKE_FUNCTION            5 (defaults, annotations)
-               648 STORE_NAME              60 (decorate_class_method)
+   388         618 LOAD_NAME                8 (Optional)
+               620 LOAD_NAME               19 (AgiflowServiceTypes)
+               622 BINARY_SUBSCR
    
-   417         650 LOAD_NAME               19 (AgiflowServiceTypes)
-               652 LOAD_ATTR               55 (TASK)
+   385         632 LOAD_CONST              30 ('kwargs')
    
-   418         662 LOAD_NAME               22 (SpanKind)
-               664 LOAD_ATTR               56 (INTERNAL)
+   392         634 LOAD_NAME               11 (Unpack)
+               636 LOAD_NAME               32 (SharedKwargsWithHooks)
+               638 BINARY_SUBSCR
    
-   419         674 LOAD_NAME               54 (BaseSpanCapture)
+   385         648 BUILD_TUPLE              8
+               650 LOAD_CONST              31 (<code object decorate_class_method, file "/Users/vuongngo/workspace/agiflow/packages/python/agiflow-sdk/agiflow/opentelemetry/trace_decorators/wrapper.py", line 385>)
+               652 MAKE_FUNCTION            5 (defaults, annotations)
+               654 STORE_NAME              60 (decorate_class_method)
    
-   414         676 BUILD_TUPLE              3
-               678 LOAD_CONST              23 ('name')
+   417         656 LOAD_NAME               19 (AgiflowServiceTypes)
+               658 LOAD_ATTR               55 (TASK)
    
-   415         680 LOAD_NAME                8 (Optional)
-               682 LOAD_NAME               57 (str)
-               684 BINARY_SUBSCR
+   418         668 LOAD_NAME               22 (SpanKind)
+               670 LOAD_ATTR               56 (INTERNAL)
    
-   414         694 LOAD_CONST              28 ('method_name')
+   419         680 LOAD_NAME               54 (BaseSpanCapture)
    
-   416         696 LOAD_NAME               57 (str)
+   420         682 LOAD_CONST              23 (False)
    
-   414         698 LOAD_CONST              24 ('tlp_service_type')
+   414         684 BUILD_TUPLE              4
+               686 LOAD_CONST              24 ('name')
    
-   417         700 LOAD_NAME                8 (Optional)
-               702 LOAD_NAME               19 (AgiflowServiceTypes)
-               704 BINARY_SUBSCR
+   415         688 LOAD_NAME                8 (Optional)
+               690 LOAD_NAME               57 (str)
+               692 BINARY_SUBSCR
    
-   414         714 LOAD_CONST              29 ('kwargs')
+   414         702 LOAD_CONST              29 ('method_name')
    
-   420         716 LOAD_NAME               11 (Unpack)
-               718 LOAD_NAME               32 (SharedKwargsWithHooks)
-               720 BINARY_SUBSCR
+   416         704 LOAD_NAME               57 (str)
    
-   414         730 BUILD_TUPLE              8
-               732 LOAD_CONST              31 (<code object adecorate_class_method, file "/Users/vuongngo/workspace/agiflow/packages/python/agiflow-sdk/agiflow/opentelemetry/trace_decorators/wrapper.py", line 414>)
-               734 MAKE_FUNCTION            5 (defaults, annotations)
-               736 STORE_NAME              61 (adecorate_class_method)
-               738 LOAD_CONST               3 (None)
-               740 RETURN_VALUE
+   414         706 LOAD_CONST              25 ('tlp_service_type')
+   
+   417         708 LOAD_NAME                8 (Optional)
+               710 LOAD_NAME               19 (AgiflowServiceTypes)
+               712 BINARY_SUBSCR
+   
+   414         722 LOAD_CONST              30 ('kwargs')
+   
+   421         724 LOAD_NAME               11 (Unpack)
+               726 LOAD_NAME               32 (SharedKwargsWithHooks)
+               728 BINARY_SUBSCR
+   
+   414         738 BUILD_TUPLE              8
+               740 LOAD_CONST              32 (<code object adecorate_class_method, file "/Users/vuongngo/workspace/agiflow/packages/python/agiflow-sdk/agiflow/opentelemetry/trace_decorators/wrapper.py", line 414>)
+               742 MAKE_FUNCTION            5 (defaults, annotations)
+               744 STORE_NAME              61 (adecorate_class_method)
+               746 LOAD_CONST               3 (None)
+               748 RETURN_VALUE
    consts
       0
       ('ABC',)
       ('wraps',)
       None
       ('Any', 'Dict', 'Optional', 'TypeVar', 'Generic', 'Unpack')
       ('set_workflow_name_from_context',)
@@ -571,19 +580,19 @@
             0x970065005a0164005a02550064015a036504650564023c000000650665
             0719000000000000000000650564033c0000006508650564043c00000065
             08650564053c0000006509650564063c0000006508650564073c00000065
             08650564083c000000650a650b6508660219000000000000000000650564
             093c0000006506650b190000000000000000006505640a3c000000640b65
             076a0c0000000000000000640b640b640c9c04640a6506650b1900000000
             000000000064036506650719000000000000000000640665096606640d84
-            065a0d650e640e8400a6000000ab0000000000000000005a0f650e640b65
-            076a0c0000000000000000640b6603640a6506650b190000000000000000
-            00640f650665071900000000000000000064076508660664108405a60000
-            00ab0000000000000000005a10650e64118400a6000000ab000000000000
-            0000005a11641284005a12641384005a13641484005a14640b5300
+            065a0d650e640b65076a0c0000000000000000640b6603640a6506650b19
+            000000000000000000640e65066507190000000000000000006407650866
+            06640f8405a6000000ab0000000000000000005a0f650e64108400a60000
+            00ab0000000000000000005a10641184005a11641284005a12641384005a
+            13640b5300
           80           0 RESUME                   0
                        2 LOAD_NAME                0 (__name__)
                        4 STORE_NAME               1 (__module__)
                        6 LOAD_CONST               0 ('BaseSpanCapture')
                        8 STORE_NAME               2 (__qualname__)
                       10 SETUP_ANNOTATIONS
          
@@ -673,80 +682,70 @@
           95         204 BUILD_TUPLE              6
                      206 LOAD_CONST              13 (<code object __init__, file "/Users/vuongngo/workspace/agiflow/packages/python/agiflow-sdk/agiflow/opentelemetry/trace_decorators/wrapper.py", line 95>)
                      208 MAKE_FUNCTION            6 (kwdefaults, annotations)
                      210 STORE_NAME              13 (__init__)
          
          120         212 LOAD_NAME               14 (staticmethod)
          
-         121         214 LOAD_CONST              14 (<code object is_flush_on_exit, file "/Users/vuongngo/workspace/agiflow/packages/python/agiflow-sdk/agiflow/opentelemetry/trace_decorators/wrapper.py", line 120>)
-                     216 MAKE_FUNCTION            0
+         122         214 LOAD_CONST              11 (None)
          
-         120         218 PRECALL                  0
-                     222 CALL                     0
+         123         216 LOAD_NAME                7 (AgiflowServiceTypes)
+                     218 LOAD_ATTR               12 (TASK)
          
-         121         232 STORE_NAME              15 (is_flush_on_exit)
+         124         228 LOAD_CONST              11 (None)
          
-         124         234 LOAD_NAME               14 (staticmethod)
+         121         230 BUILD_TUPLE              3
+                     232 LOAD_CONST              10 ('name')
          
-         126         236 LOAD_CONST              11 (None)
+         122         234 LOAD_NAME                6 (Optional)
+                     236 LOAD_NAME               11 (str)
+                     238 BINARY_SUBSCR
          
-         127         238 LOAD_NAME                7 (AgiflowServiceTypes)
-                     240 LOAD_ATTR               12 (TASK)
+         121         248 LOAD_CONST              14 ('tlp_service_type')
          
-         128         250 LOAD_CONST              11 (None)
+         123         250 LOAD_NAME                6 (Optional)
+                     252 LOAD_NAME                7 (AgiflowServiceTypes)
+                     254 BINARY_SUBSCR
          
-         125         252 BUILD_TUPLE              3
-                     254 LOAD_CONST              10 ('name')
+         121         264 LOAD_CONST               7 ('instance')
          
-         126         256 LOAD_NAME                6 (Optional)
-                     258 LOAD_NAME               11 (str)
-                     260 BINARY_SUBSCR
+         124         266 LOAD_NAME                8 (Any)
          
-         125         270 LOAD_CONST              15 ('tlp_service_type')
+         121         268 BUILD_TUPLE              6
+                     270 LOAD_CONST              15 (<code object get_span_name, file "/Users/vuongngo/workspace/agiflow/packages/python/agiflow-sdk/agiflow/opentelemetry/trace_decorators/wrapper.py", line 120>)
+                     272 MAKE_FUNCTION            5 (defaults, annotations)
          
-         127         272 LOAD_NAME                6 (Optional)
-                     274 LOAD_NAME                7 (AgiflowServiceTypes)
-                     276 BINARY_SUBSCR
+         120         274 PRECALL                  0
+                     278 CALL                     0
          
-         125         286 LOAD_CONST               7 ('instance')
+         121         288 STORE_NAME              15 (get_span_name)
          
-         128         288 LOAD_NAME                8 (Any)
+         135         290 LOAD_NAME               14 (staticmethod)
          
-         125         290 BUILD_TUPLE              6
-                     292 LOAD_CONST              16 (<code object get_span_name, file "/Users/vuongngo/workspace/agiflow/packages/python/agiflow-sdk/agiflow/opentelemetry/trace_decorators/wrapper.py", line 124>)
-                     294 MAKE_FUNCTION            5 (defaults, annotations)
+         136         292 LOAD_CONST              16 (<code object get_service_type, file "/Users/vuongngo/workspace/agiflow/packages/python/agiflow-sdk/agiflow/opentelemetry/trace_decorators/wrapper.py", line 135>)
+                     294 MAKE_FUNCTION            0
          
-         124         296 PRECALL                  0
+         135         296 PRECALL                  0
                      300 CALL                     0
          
-         125         310 STORE_NAME              16 (get_span_name)
-         
-         139         312 LOAD_NAME               14 (staticmethod)
-         
-         140         314 LOAD_CONST              17 (<code object get_service_type, file "/Users/vuongngo/workspace/agiflow/packages/python/agiflow-sdk/agiflow/opentelemetry/trace_decorators/wrapper.py", line 139>)
-                     316 MAKE_FUNCTION            0
+         136         310 STORE_NAME              16 (get_service_type)
          
-         139         318 PRECALL                  0
-                     322 CALL                     0
-         
-         140         332 STORE_NAME              17 (get_service_type)
-         
-         146         334 LOAD_CONST              18 (<code object set_span_attribute, file "/Users/vuongngo/workspace/agiflow/packages/python/agiflow-sdk/agiflow/opentelemetry/trace_decorators/wrapper.py", line 146>)
-                     336 MAKE_FUNCTION            0
-                     338 STORE_NAME              18 (set_span_attribute)
-         
-         157         340 LOAD_CONST              19 (<code object capture_input, file "/Users/vuongngo/workspace/agiflow/packages/python/agiflow-sdk/agiflow/opentelemetry/trace_decorators/wrapper.py", line 157>)
-                     342 MAKE_FUNCTION            0
-                     344 STORE_NAME              19 (capture_input)
-         
-         228         346 LOAD_CONST              20 (<code object capture_output, file "/Users/vuongngo/workspace/agiflow/packages/python/agiflow-sdk/agiflow/opentelemetry/trace_decorators/wrapper.py", line 228>)
-                     348 MAKE_FUNCTION            0
-                     350 STORE_NAME              20 (capture_output)
-                     352 LOAD_CONST              11 (None)
-                     354 RETURN_VALUE
+         142         312 LOAD_CONST              17 (<code object set_span_attribute, file "/Users/vuongngo/workspace/agiflow/packages/python/agiflow-sdk/agiflow/opentelemetry/trace_decorators/wrapper.py", line 142>)
+                     314 MAKE_FUNCTION            0
+                     316 STORE_NAME              17 (set_span_attribute)
+         
+         153         318 LOAD_CONST              18 (<code object capture_input, file "/Users/vuongngo/workspace/agiflow/packages/python/agiflow-sdk/agiflow/opentelemetry/trace_decorators/wrapper.py", line 153>)
+                     320 MAKE_FUNCTION            0
+                     322 STORE_NAME              18 (capture_input)
+         
+         224         324 LOAD_CONST              19 (<code object capture_output, file "/Users/vuongngo/workspace/agiflow/packages/python/agiflow-sdk/agiflow/opentelemetry/trace_decorators/wrapper.py", line 224>)
+                     326 MAKE_FUNCTION            0
+                     328 STORE_NAME              19 (capture_output)
+                     330 LOAD_CONST              11 (None)
+                     332 RETURN_VALUE
          consts
             'BaseSpanCapture'
             '\n    Store shared props.\n    Required to implement hooks to add to trace to span\n    '
             'span'
             'service_type'
             'args'
             'kwargs'
@@ -861,112 +860,91 @@
                varnames   ('self', 'name', 'service_type', 'span', 'instance', 'context', 'config', 'args', 'kwargs', 'extra_attributes')
                freevars   ()
                cellvars   ()
                filename   '/Users/vuongngo/workspace/agiflow/packages/python/agiflow-sdk/agiflow/opentelemetry/trace_decorators/wrapper.py'
                name       '__init__'
                firstlineno 95
                lnotab 0x020b0e010e010e010e010e010e010e010e0140014a0140013201
-            code
-               argcount  : 0
-               nlocals   : 0
-               stacksize : 1
-               flags     : 3
-               code 0x970064015300
-               120           0 RESUME                   0
-               
-               122           2 LOAD_CONST               1 (False)
-                             4 RETURN_VALUE
-               consts
-                  None
-                  False
-               names      ()
-               varnames   ()
-               freevars   ()
-               cellvars   ()
-               filename   '/Users/vuongngo/workspace/agiflow/packages/python/agiflow-sdk/agiflow/opentelemetry/trace_decorators/wrapper.py'
-               name       'is_flush_on_exit'
-               firstlineno 120
-               lnotab 0x0202
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
-               124           0 RESUME                   0
+               120           0 RESUME                   0
                
-               130           2 LOAD_FAST                1 (tlp_service_type)
+               126           2 LOAD_FAST                1 (tlp_service_type)
                              4 JUMP_IF_TRUE_OR_POP     24 (to 54)
                              6 LOAD_GLOBAL              0 (BaseSpanCapture)
                             18 LOAD_METHOD              1 (get_service_type)
                             40 PRECALL                  0
                             44 CALL                     0
                        >>   54 STORE_FAST               3 (service_type)
                
-               134          56 LOAD_FAST                0 (name)
+               130          56 LOAD_FAST                0 (name)
                
-               133          58 POP_JUMP_FORWARD_IF_FALSE     7 (to 74)
+               129          58 POP_JUMP_FORWARD_IF_FALSE     7 (to 74)
                             60 LOAD_FAST                0 (name)
                             62 FORMAT_VALUE             0
                             64 LOAD_CONST               1 ('.')
                             66 LOAD_FAST                3 (service_type)
                             68 FORMAT_VALUE             0
                             70 BUILD_STRING             3
                             72 JUMP_FORWARD            11 (to 96)
                
-               135     >>   74 LOAD_FAST                2 (instance)
+               131     >>   74 LOAD_FAST                2 (instance)
                             76 LOAD_ATTR                2 (__name__)
                             86 FORMAT_VALUE             0
                             88 LOAD_CONST               1 ('.')
                             90 LOAD_FAST                3 (service_type)
                             92 FORMAT_VALUE             0
                             94 BUILD_STRING             3
                
-               132     >>   96 STORE_FAST               4 (span_name)
+               128     >>   96 STORE_FAST               4 (span_name)
                
-               137          98 LOAD_FAST                4 (span_name)
+               133          98 LOAD_FAST                4 (span_name)
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
-               firstlineno 124
+               firstlineno 120
                lnotab 0x0206360402ff100216fd0205
             code
                argcount  : 0
                nlocals   : 0
                stacksize : 1
                flags     : 3
                code 0x97007400000000000000000000006a0100000000000000005300
-               139           0 RESUME                   0
+               135           0 RESUME                   0
                
-               144           2 LOAD_GLOBAL              0 (AgiflowServiceTypes)
+               140           2 LOAD_GLOBAL              0 (AgiflowServiceTypes)
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
-               firstlineno 139
+               firstlineno 135
                lnotab 0x0205
             code
                argcount  : 3
                nlocals   : 3
                stacksize : 4
                flags     : 3
                code
@@ -974,70 +952,70 @@
                   0000000000000000000000a6000000ab0000000000000000007251740500
                   0000000000000000007c016402a6020000ab02000000000000000072227c
                   006a000000000000000000a0030000000000000000000000000000000000
                   0000007c016a0400000000000000007c02a6020000ab0200000000000000
                   000100640153007c006a000000000000000000a003000000000000000000
                   00000000000000000000007c017c02a6020000ab02000000000000000001
                   00640153006401530064015300
-               146           0 RESUME                   0
+               142           0 RESUME                   0
                
-               151           2 LOAD_FAST                2 (value)
+               147           2 LOAD_FAST                2 (value)
                              4 POP_JUMP_FORWARD_IF_NONE   104 (to 214)
                              6 LOAD_FAST                0 (self)
                              8 LOAD_ATTR                0 (span)
                             18 LOAD_METHOD              1 (is_recording)
                             40 PRECALL                  0
                             44 CALL                     0
                             54 POP_JUMP_FORWARD_IF_FALSE    81 (to 218)
                
-               152          56 LOAD_GLOBAL              5 (NULL + hasattr)
+               148          56 LOAD_GLOBAL              5 (NULL + hasattr)
                             68 LOAD_FAST                1 (field)
                             70 LOAD_CONST               2 ('value')
                             72 PRECALL                  2
                             76 CALL                     2
                             86 POP_JUMP_FORWARD_IF_FALSE    34 (to 156)
                
-               153          88 LOAD_FAST                0 (self)
+               149          88 LOAD_FAST                0 (self)
                             90 LOAD_ATTR                0 (span)
                            100 LOAD_METHOD              3 (set_attribute)
                            122 LOAD_FAST                1 (field)
                            124 LOAD_ATTR                4 (value)
                            134 LOAD_FAST                2 (value)
                            136 PRECALL                  2
                            140 CALL                     2
                            150 POP_TOP
                            152 LOAD_CONST               1 (None)
                            154 RETURN_VALUE
                
-               155     >>  156 LOAD_FAST                0 (self)
+               151     >>  156 LOAD_FAST                0 (self)
                            158 LOAD_ATTR                0 (span)
                            168 LOAD_METHOD              3 (set_attribute)
                            190 LOAD_FAST                1 (field)
                            192 LOAD_FAST                2 (value)
                            194 PRECALL                  2
                            198 CALL                     2
                            208 POP_TOP
                            210 LOAD_CONST               1 (None)
                            212 RETURN_VALUE
                
-               151     >>  214 LOAD_CONST               1 (None)
+               147     >>  214 LOAD_CONST               1 (None)
                            216 RETURN_VALUE
                        >>  218 LOAD_CONST               1 (None)
                            220 RETURN_VALUE
                consts
                   '\n        Using this method to set single attribute\n        which field is an enum\n        '
                   None
                   'value'
                names      ('span', 'is_recording', 'hasattr', 'set_attribute', 'value')
                varnames   ('self', 'field', 'value')
                freevars   ()
                cellvars   ()
                filename   '/Users/vuongngo/workspace/agiflow/packages/python/agiflow-sdk/agiflow/opentelemetry/trace_decorators/wrapper.py'
                name       'set_span_attribute'
-               firstlineno 146
+               firstlineno 142
                lnotab 0x02053601200144023afc
             code
                argcount  : 1
                nlocals   : 12
                stacksize : 6
                flags     : 3
                code
@@ -1092,333 +1070,333 @@
                   00730f743b000000000000000000007c09a6010000ab0100000000000000
                   007d097c00a0010000000000000000000000000000000000000000740400
                   0000000000000000006a2000000000000000007c09a6020000ab02000000
                   000000000001006400530064005300230074420000000000000000000024
                   0072257d0b744400000000000000000000a0230000000000000000000000
                   0000000000000000007c0ba6010000ab0100000000000000000100590064
                   007d0b7e0b6400530064007d0b7e0b77017700780359007701
-               157           0 RESUME                   0
+               153           0 RESUME                   0
                
-               158           2 LOAD_FAST                0 (self)
+               154           2 LOAD_FAST                0 (self)
                              4 LOAD_ATTR                0 (name)
                             14 POP_JUMP_FORWARD_IF_FALSE    37 (to 90)
                
-               159          16 LOAD_FAST                0 (self)
+               155          16 LOAD_FAST                0 (self)
                             18 LOAD_METHOD              1 (set_span_attribute)
                             40 LOAD_GLOBAL              4 (SpanAttributes)
                             52 LOAD_ATTR                3 (AGIFLOW_ENTITY_NAME)
                             62 LOAD_FAST                0 (self)
                             64 LOAD_ATTR                0 (name)
                             74 PRECALL                  2
                             78 CALL                     2
                             88 POP_TOP
                
-               161     >>   90 LOAD_CONST               0 (None)
+               157     >>   90 LOAD_CONST               0 (None)
                             92 STORE_FAST               1 (prompt_settings)
                
-               162          94 LOAD_CONST               0 (None)
+               158          94 LOAD_CONST               0 (None)
                             96 STORE_FAST               2 (association_properties)
                
-               164          98 LOAD_FAST                0 (self)
+               160          98 LOAD_FAST                0 (self)
                            100 LOAD_ATTR                4 (context)
                            110 POP_JUMP_FORWARD_IF_NONE   225 (to 562)
                            112 LOAD_GLOBAL             11 (NULL + hasattr)
                            124 LOAD_FAST                0 (self)
                            126 LOAD_ATTR                4 (context)
                            136 LOAD_CONST               1 ('get')
                            138 PRECALL                  2
                            142 CALL                     2
                            152 POP_JUMP_FORWARD_IF_FALSE   204 (to 562)
                
-               165         154 LOAD_FAST                0 (self)
+               161         154 LOAD_FAST                0 (self)
                            156 LOAD_ATTR                4 (context)
                            166 LOAD_METHOD              6 (get)
                            188 LOAD_GLOBAL             14 (ContextKeys)
                            200 LOAD_ATTR                8 (ASSOCIATION_PROPERTIES)
                            210 PRECALL                  1
                            214 CALL                     1
                            224 STORE_FAST               2 (association_properties)
                
-               166         226 LOAD_FAST                0 (self)
+               162         226 LOAD_FAST                0 (self)
                            228 LOAD_ATTR                4 (context)
                            238 LOAD_METHOD              6 (get)
                            260 LOAD_GLOBAL             14 (ContextKeys)
                            272 LOAD_ATTR                9 (PROMPT_SETTINGS)
                            282 PRECALL                  1
                            286 CALL                     1
                            296 STORE_FAST               1 (prompt_settings)
                
-               168         298 LOAD_FAST                0 (self)
+               164         298 LOAD_FAST                0 (self)
                            300 LOAD_ATTR                4 (context)
                            310 LOAD_METHOD              6 (get)
                            332 LOAD_GLOBAL             14 (ContextKeys)
                            344 LOAD_ATTR               10 (WORKFLOW_NAME)
                            354 PRECALL                  1
                            358 CALL                     1
                            368 STORE_FAST               3 (workflow_name)
                
-               169         370 LOAD_FAST                3 (workflow_name)
+               165         370 LOAD_FAST                3 (workflow_name)
                            372 POP_JUMP_FORWARD_IF_NONE    41 (to 456)
                
-               170         374 LOAD_GLOBAL             23 (NULL + set_workflow_name)
+               166         374 LOAD_GLOBAL             23 (NULL + set_workflow_name)
                            386 LOAD_FAST                3 (workflow_name)
                            388 PRECALL                  1
                            392 CALL                     1
                            402 POP_TOP
                
-               171         404 LOAD_GLOBAL             25 (NULL + set_workflow_name_from_context)
+               167         404 LOAD_GLOBAL             25 (NULL + set_workflow_name_from_context)
                            416 LOAD_FAST                0 (self)
                            418 LOAD_ATTR               13 (span)
                            428 LOAD_FAST                0 (self)
                            430 LOAD_ATTR                4 (context)
                            440 PRECALL                  2
                            444 CALL                     2
                            454 POP_TOP
                
-               173     >>  456 LOAD_FAST                0 (self)
+               169     >>  456 LOAD_FAST                0 (self)
                            458 LOAD_ATTR                4 (context)
                            468 LOAD_METHOD              6 (get)
                            490 LOAD_GLOBAL             14 (ContextKeys)
                            502 LOAD_ATTR               14 (OVERRIDE_ENABLE_CONTENT_TRACING)
                            512 PRECALL                  1
                            516 CALL                     1
                            526 STORE_FAST               4 (content_tracing)
                
-               174         528 LOAD_FAST                4 (content_tracing)
+               170         528 LOAD_FAST                4 (content_tracing)
                            530 POP_JUMP_FORWARD_IF_NONE    15 (to 562)
                
-               175         532 LOAD_GLOBAL             31 (NULL + set_override_enable_context_tracing)
+               171         532 LOAD_GLOBAL             31 (NULL + set_override_enable_context_tracing)
                            544 LOAD_FAST                4 (content_tracing)
                            546 PRECALL                  1
                            550 CALL                     1
                            560 POP_TOP
                
-               177     >>  562 LOAD_FAST                0 (self)
+               173     >>  562 LOAD_FAST                0 (self)
                            564 LOAD_METHOD              1 (set_span_attribute)
                
-               178         586 LOAD_GLOBAL             32 (AgiflowSpanAttributes)
+               174         586 LOAD_GLOBAL             32 (AgiflowSpanAttributes)
                            598 LOAD_ATTR               17 (AGIFLOW_ENTITY_DESCRIPTION)
                
-               179         608 LOAD_FAST                0 (self)
+               175         608 LOAD_FAST                0 (self)
                            610 LOAD_ATTR               18 (config)
                            620 LOAD_METHOD              6 (get)
                            642 LOAD_CONST               2 ('description')
                            644 PRECALL                  1
                            648 CALL                     1
                
-               177         658 PRECALL                  2
+               173         658 PRECALL                  2
                            662 CALL                     2
                            672 POP_TOP
                
-               182         674 LOAD_FAST                0 (self)
+               178         674 LOAD_FAST                0 (self)
                            676 LOAD_ATTR               18 (config)
                            686 LOAD_METHOD              6 (get)
                            708 LOAD_CONST               3 ('prompt_settings')
                            710 PRECALL                  1
                            714 CALL                     1
                            724 STORE_FAST               5 (prompt_settings_config)
                
-               183         726 LOAD_FAST                5 (prompt_settings_config)
+               179         726 LOAD_FAST                5 (prompt_settings_config)
                            728 POP_JUMP_FORWARD_IF_NONE    36 (to 802)
                
-               184         730 LOAD_GLOBAL             39 (NULL + callable)
+               180         730 LOAD_GLOBAL             39 (NULL + callable)
                            742 LOAD_FAST                5 (prompt_settings_config)
                            744 PRECALL                  1
                            748 CALL                     1
                            758 POP_JUMP_FORWARD_IF_FALSE    19 (to 798)
                
-               185         760 PUSH_NULL
+               181         760 PUSH_NULL
                            762 LOAD_FAST                5 (prompt_settings_config)
                            764 LOAD_FAST                0 (self)
                            766 LOAD_ATTR               20 (args)
                            776 BUILD_MAP                0
                            778 LOAD_FAST                0 (self)
                            780 LOAD_ATTR               21 (kwargs)
                            790 DICT_MERGE               1
                            792 CALL_FUNCTION_EX         1
                            794 STORE_FAST               1 (prompt_settings)
                            796 JUMP_FORWARD             2 (to 802)
                
-               187     >>  798 LOAD_FAST                5 (prompt_settings_config)
+               183     >>  798 LOAD_FAST                5 (prompt_settings_config)
                            800 STORE_FAST               1 (prompt_settings)
                
-               189     >>  802 LOAD_FAST                0 (self)
+               185     >>  802 LOAD_FAST                0 (self)
                            804 LOAD_ATTR               18 (config)
                            814 LOAD_METHOD              6 (get)
                            836 LOAD_CONST               4 ('association_properties')
                            838 PRECALL                  1
                            842 CALL                     1
                            852 STORE_FAST               6 (association_properties_config)
                
-               190         854 LOAD_FAST                6 (association_properties_config)
+               186         854 LOAD_FAST                6 (association_properties_config)
                            856 POP_JUMP_FORWARD_IF_NONE    36 (to 930)
                
-               191         858 LOAD_GLOBAL             39 (NULL + callable)
+               187         858 LOAD_GLOBAL             39 (NULL + callable)
                            870 LOAD_FAST                6 (association_properties_config)
                            872 PRECALL                  1
                            876 CALL                     1
                            886 POP_JUMP_FORWARD_IF_FALSE    19 (to 926)
                
-               192         888 PUSH_NULL
+               188         888 PUSH_NULL
                            890 LOAD_FAST                6 (association_properties_config)
                            892 LOAD_FAST                0 (self)
                            894 LOAD_ATTR               20 (args)
                            904 BUILD_MAP                0
                            906 LOAD_FAST                0 (self)
                            908 LOAD_ATTR               21 (kwargs)
                            918 DICT_MERGE               1
                            920 CALL_FUNCTION_EX         1
                            922 STORE_FAST               2 (association_properties)
                            924 JUMP_FORWARD             2 (to 930)
                
-               194     >>  926 LOAD_FAST                6 (association_properties_config)
+               190     >>  926 LOAD_FAST                6 (association_properties_config)
                            928 STORE_FAST               2 (association_properties)
                
-               196     >>  930 LOAD_FAST                1 (prompt_settings)
+               192     >>  930 LOAD_FAST                1 (prompt_settings)
                            932 POP_JUMP_FORWARD_IF_NONE    41 (to 1016)
                
-               197         934 LOAD_GLOBAL             45 (NULL + set_prompt_settings_context)
+               193         934 LOAD_GLOBAL             45 (NULL + set_prompt_settings_context)
                            946 LOAD_FAST                1 (prompt_settings)
                            948 PRECALL                  1
                            952 CALL                     1
                            962 POP_TOP
                
-               198         964 LOAD_GLOBAL             47 (NULL + set_prompt_attributes_from_context)
+               194         964 LOAD_GLOBAL             47 (NULL + set_prompt_attributes_from_context)
                            976 LOAD_FAST                0 (self)
                            978 LOAD_ATTR               13 (span)
                            988 LOAD_FAST                0 (self)
                            990 LOAD_ATTR                4 (context)
                           1000 PRECALL                  2
                           1004 CALL                     2
                           1014 POP_TOP
                
-               200     >> 1016 LOAD_FAST                2 (association_properties)
+               196     >> 1016 LOAD_FAST                2 (association_properties)
                           1018 POP_JUMP_FORWARD_IF_NONE    83 (to 1186)
                
-               201        1020 LOAD_GLOBAL             49 (NULL + set_association_properties)
+               197        1020 LOAD_GLOBAL             49 (NULL + set_association_properties)
                           1032 LOAD_FAST                2 (association_properties)
                           1034 PRECALL                  1
                           1038 CALL                     1
                           1048 POP_TOP
                
-               202        1050 LOAD_FAST                2 (association_properties)
+               198        1050 LOAD_FAST                2 (association_properties)
                           1052 LOAD_METHOD             25 (items)
                           1074 PRECALL                  0
                           1078 CALL                     0
                           1088 GET_ITER
                        >> 1090 FOR_ITER                47 (to 1186)
                           1092 UNPACK_SEQUENCE          2
                           1096 STORE_FAST               7 (key)
                           1098 STORE_FAST               8 (value)
                
-               203        1100 LOAD_FAST                0 (self)
+               199        1100 LOAD_FAST                0 (self)
                           1102 LOAD_ATTR               13 (span)
                           1112 LOAD_METHOD             26 (set_attribute)
                
-               204        1134 LOAD_GLOBAL              4 (SpanAttributes)
+               200        1134 LOAD_GLOBAL              4 (SpanAttributes)
                           1146 LOAD_ATTR               27 (AGIFLOW_ASSOCIATION_PROPERTIES)
                           1156 FORMAT_VALUE             0
                           1158 LOAD_CONST               5 ('.')
                           1160 LOAD_FAST                7 (key)
                           1162 FORMAT_VALUE             0
                           1164 BUILD_STRING             3
                
-               205        1166 LOAD_FAST                8 (value)
+               201        1166 LOAD_FAST                8 (value)
                
-               203        1168 PRECALL                  2
+               199        1168 PRECALL                  2
                           1172 CALL                     2
                           1182 POP_TOP
                           1184 JUMP_BACKWARD           48 (to 1090)
                
-               208     >> 1186 NOP
+               204     >> 1186 NOP
                
-               209        1188 LOAD_GLOBAL             57 (NULL + should_send_prompts)
+               205        1188 LOAD_GLOBAL             57 (NULL + should_send_prompts)
                           1200 PRECALL                  0
                           1204 CALL                     0
                           1214 POP_JUMP_FORWARD_IF_FALSE   162 (to 1540)
                
-               210        1216 LOAD_CONST               6 ('')
+               206        1216 LOAD_CONST               6 ('')
                           1218 STORE_FAST               9 (input)
                
-               211        1220 LOAD_FAST                0 (self)
+               207        1220 LOAD_FAST                0 (self)
                           1222 LOAD_ATTR               18 (config)
                           1232 LOAD_METHOD              6 (get)
                           1254 LOAD_CONST               7 ('input_serializer')
                           1256 PRECALL                  1
                           1260 CALL                     1
                           1270 STORE_FAST              10 (input_serializer)
                
-               213        1272 LOAD_FAST               10 (input_serializer)
+               209        1272 LOAD_FAST               10 (input_serializer)
                           1274 POP_JUMP_FORWARD_IF_NONE    34 (to 1344)
                           1276 LOAD_GLOBAL             39 (NULL + callable)
                           1288 LOAD_FAST               10 (input_serializer)
                           1290 PRECALL                  1
                           1294 CALL                     1
                           1304 POP_JUMP_FORWARD_IF_FALSE    19 (to 1344)
                
-               214        1306 PUSH_NULL
+               210        1306 PUSH_NULL
                           1308 LOAD_FAST               10 (input_serializer)
                           1310 LOAD_FAST                0 (self)
                           1312 LOAD_ATTR               20 (args)
                           1322 BUILD_MAP                0
                           1324 LOAD_FAST                0 (self)
                           1326 LOAD_ATTR               21 (kwargs)
                           1336 DICT_MERGE               1
                           1338 CALL_FUNCTION_EX         1
                           1340 STORE_FAST               9 (input)
                           1342 JUMP_FORWARD            28 (to 1400)
                
-               216     >> 1344 LOAD_GLOBAL             59 (NULL + serialise_to_json)
+               212     >> 1344 LOAD_GLOBAL             59 (NULL + serialise_to_json)
                           1356 LOAD_FAST                0 (self)
                           1358 LOAD_ATTR               20 (args)
                           1368 LOAD_FAST                0 (self)
                           1370 LOAD_ATTR               21 (kwargs)
                           1380 LOAD_CONST               8 (('args', 'kwargs'))
                           1382 BUILD_CONST_KEY_MAP      2
                           1384 PRECALL                  1
                           1388 CALL                     1
                           1398 STORE_FAST               9 (input)
                
-               218     >> 1400 LOAD_GLOBAL             61 (NULL + isinstance)
+               214     >> 1400 LOAD_GLOBAL             61 (NULL + isinstance)
                           1412 LOAD_FAST                9 (input)
                           1414 LOAD_GLOBAL             62 (str)
                           1426 PRECALL                  2
                           1430 CALL                     2
                           1440 POP_JUMP_FORWARD_IF_TRUE    15 (to 1472)
                
-               219        1442 LOAD_GLOBAL             59 (NULL + serialise_to_json)
+               215        1442 LOAD_GLOBAL             59 (NULL + serialise_to_json)
                           1454 LOAD_FAST                9 (input)
                           1456 PRECALL                  1
                           1460 CALL                     1
                           1470 STORE_FAST               9 (input)
                
-               221     >> 1472 LOAD_FAST                0 (self)
+               217     >> 1472 LOAD_FAST                0 (self)
                           1474 LOAD_METHOD              1 (set_span_attribute)
                
-               222        1496 LOAD_GLOBAL              4 (SpanAttributes)
+               218        1496 LOAD_GLOBAL              4 (SpanAttributes)
                           1508 LOAD_ATTR               32 (AGIFLOW_ENTITY_INPUT)
                
-               223        1518 LOAD_FAST                9 (input)
+               219        1518 LOAD_FAST                9 (input)
                
-               221        1520 PRECALL                  2
+               217        1520 PRECALL                  2
                           1524 CALL                     2
                           1534 POP_TOP
                           1536 LOAD_CONST               0 (None)
                           1538 RETURN_VALUE
                
-               209     >> 1540 LOAD_CONST               0 (None)
+               205     >> 1540 LOAD_CONST               0 (None)
                           1542 RETURN_VALUE
                        >> 1544 PUSH_EXC_INFO
                
-               225        1546 LOAD_GLOBAL             66 (TypeError)
+               221        1546 LOAD_GLOBAL             66 (TypeError)
                           1558 CHECK_EXC_MATCH
                           1560 POP_JUMP_FORWARD_IF_FALSE    37 (to 1636)
                           1562 STORE_FAST              11 (e)
                
-               226        1564 LOAD_GLOBAL             68 (logger)
+               222        1564 LOAD_GLOBAL             68 (logger)
                           1576 LOAD_METHOD             35 (error)
                           1598 LOAD_FAST               11 (e)
                           1600 PRECALL                  1
                           1604 CALL                     1
                           1614 POP_TOP
                           1616 POP_EXCEPT
                           1618 LOAD_CONST               0 (None)
@@ -1427,15 +1405,15 @@
                           1624 LOAD_CONST               0 (None)
                           1626 RETURN_VALUE
                        >> 1628 LOAD_CONST               0 (None)
                           1630 STORE_FAST              11 (e)
                           1632 DELETE_FAST             11 (e)
                           1634 RERAISE                  1
                
-               225     >> 1636 RERAISE                  0
+               221     >> 1636 RERAISE                  0
                        >> 1638 COPY                     3
                           1640 POP_EXCEPT
                           1642 RERAISE                  1
                ExceptionTable:
                  1188 to 1534 -> 1544 [0]
                  1544 to 1562 -> 1638 [1] lasti
                  1564 to 1614 -> 1628 [1] lasti
@@ -1452,15 +1430,15 @@
                   ('args', 'kwargs')
                names      ('name', 'set_span_attribute', 'SpanAttributes', 'AGIFLOW_ENTITY_NAME', 'context', 'hasattr', 'get', 'ContextKeys', 'ASSOCIATION_PROPERTIES', 'PROMPT_SETTINGS', 'WORKFLOW_NAME', 'set_workflow_name', 'set_workflow_name_from_context', 'span', 'OVERRIDE_ENABLE_CONTENT_TRACING', 'set_override_enable_context_tracing', 'AgiflowSpanAttributes', 'AGIFLOW_ENTITY_DESCRIPTION', 'config', 'callable', 'args', 'kwargs', 'set_prompt_settings_context', 'set_prompt_attributes_from_context', 'set_association_properties', 'items', 'set_attribute', 'AGIFLOW_ASSOCIATION_PROPERTIES', 'should_send_prompts', 'serialise_to_json', 'isinstance', 'str', 'AGIFLOW_ENTITY_INPUT', 'TypeError', 'logger', 'error')
                varnames   ('self', 'prompt_settings', 'association_properties', 'workflow_name', 'content_tracing', 'prompt_settings_config', 'association_properties_config', 'key', 'value', 'input', 'input_serializer', 'e')
                freevars   ()
                cellvars   ()
                filename   '/Users/vuongngo/workspace/agiflow/packages/python/agiflow-sdk/agiflow/opentelemetry/trace_decorators/wrapper.py'
                name       'capture_input'
-               firstlineno 157
+               firstlineno 153
                lnotab
                   0x02010e014a0204010402380148014802480104011e013402480104011e
                   021801160132fe1005340104011e0126020402340104011e012602040204
                   011e01340204011e0132012201200102fe120502011c0104013402220126
                   0238022a011e021801160102fe14f40610120148ff
             code
                argcount  : 2
@@ -1479,104 +1457,104 @@
                   00730f740d000000000000000000007c01a6010000ab0100000000000000
                   007d027c00a0090000000000000000000000000000000000000000741400
                   0000000000000000006a0b00000000000000007c02a6020000ab02000000
                   000000000001006400530064005300230074180000000000000000000024
                   0072257d04741a00000000000000000000a00e0000000000000000000000
                   0000000000000000007c04a6010000ab0100000000000000000100590064
                   007d047e046400530064007d047e0477017700780359007701
-               228           0 RESUME                   0
+               224           0 RESUME                   0
                
-               229           2 NOP
+               225           2 NOP
                
-               230           4 LOAD_GLOBAL              1 (NULL + should_send_prompts)
+               226           4 LOAD_GLOBAL              1 (NULL + should_send_prompts)
                             16 PRECALL                  0
                             20 CALL                     0
                             30 POP_JUMP_FORWARD_IF_FALSE   154 (to 340)
                
-               231          32 LOAD_CONST               1 ('')
+               227          32 LOAD_CONST               1 ('')
                             34 STORE_FAST               2 (output)
                
-               232          36 LOAD_FAST                0 (self)
+               228          36 LOAD_FAST                0 (self)
                             38 LOAD_ATTR                1 (config)
                             48 LOAD_METHOD              2 (get)
                             70 LOAD_CONST               2 ('output_serializer')
                             72 PRECALL                  1
                             76 CALL                     1
                             86 STORE_FAST               3 (output_serializer)
                
-               233          88 LOAD_FAST                3 (output_serializer)
+               229          88 LOAD_FAST                3 (output_serializer)
                             90 POP_JUMP_FORWARD_IF_NONE    35 (to 162)
                             92 LOAD_GLOBAL              7 (NULL + callable)
                            104 LOAD_FAST                3 (output_serializer)
                            106 PRECALL                  1
                            110 CALL                     1
                            120 POP_JUMP_FORWARD_IF_FALSE    20 (to 162)
                
-               234         122 PUSH_NULL
+               230         122 PUSH_NULL
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
                
-               235     >>  162 LOAD_FAST                1 (result)
+               231     >>  162 LOAD_FAST                1 (result)
                            164 POP_JUMP_FORWARD_IF_NONE    17 (to 200)
                
-               236         166 LOAD_FAST                3 (output_serializer)
+               232         166 LOAD_FAST                3 (output_serializer)
                            168 POP_JUMP_FORWARD_IF_TRUE    15 (to 200)
                
-               237         170 LOAD_GLOBAL             13 (NULL + serialise_to_json)
+               233         170 LOAD_GLOBAL             13 (NULL + serialise_to_json)
                            182 LOAD_FAST                1 (result)
                            184 PRECALL                  1
                            188 CALL                     1
                            198 STORE_FAST               2 (output)
                
-               239     >>  200 LOAD_GLOBAL             15 (NULL + isinstance)
+               235     >>  200 LOAD_GLOBAL             15 (NULL + isinstance)
                            212 LOAD_FAST                2 (output)
                            214 LOAD_GLOBAL             16 (str)
                            226 PRECALL                  2
                            230 CALL                     2
                            240 POP_JUMP_FORWARD_IF_TRUE    15 (to 272)
                
-               240         242 LOAD_GLOBAL             13 (NULL + serialise_to_json)
+               236         242 LOAD_GLOBAL             13 (NULL + serialise_to_json)
                            254 LOAD_FAST                1 (result)
                            256 PRECALL                  1
                            260 CALL                     1
                            270 STORE_FAST               2 (output)
                
-               242     >>  272 LOAD_FAST                0 (self)
+               238     >>  272 LOAD_FAST                0 (self)
                            274 LOAD_METHOD              9 (set_span_attribute)
                
-               243         296 LOAD_GLOBAL             20 (SpanAttributes)
+               239         296 LOAD_GLOBAL             20 (SpanAttributes)
                            308 LOAD_ATTR               11 (AGIFLOW_ENTITY_OUTPUT)
                
-               244         318 LOAD_FAST                2 (output)
+               240         318 LOAD_FAST                2 (output)
                
-               242         320 PRECALL                  2
+               238         320 PRECALL                  2
                            324 CALL                     2
                            334 POP_TOP
                            336 LOAD_CONST               0 (None)
                            338 RETURN_VALUE
                
-               230     >>  340 LOAD_CONST               0 (None)
+               226     >>  340 LOAD_CONST               0 (None)
                            342 RETURN_VALUE
                        >>  344 PUSH_EXC_INFO
                
-               247         346 LOAD_GLOBAL             24 (TypeError)
+               243         346 LOAD_GLOBAL             24 (TypeError)
                            358 CHECK_EXC_MATCH
                            360 POP_JUMP_FORWARD_IF_FALSE    37 (to 436)
                            362 STORE_FAST               4 (e)
                
-               248         364 LOAD_GLOBAL             26 (logger)
+               244         364 LOAD_GLOBAL             26 (logger)
                            376 LOAD_METHOD             14 (error)
                            398 LOAD_FAST                4 (e)
                            400 PRECALL                  1
                            404 CALL                     1
                            414 POP_TOP
                            416 POP_EXCEPT
                            418 LOAD_CONST               0 (None)
@@ -1585,15 +1563,15 @@
                            424 LOAD_CONST               0 (None)
                            426 RETURN_VALUE
                        >>  428 LOAD_CONST               0 (None)
                            430 STORE_FAST               4 (e)
                            432 DELETE_FAST              4 (e)
                            434 RERAISE                  1
                
-               247     >>  436 RERAISE                  0
+               243     >>  436 RERAISE                  0
                        >>  438 COPY                     3
                            440 POP_EXCEPT
                            442 RERAISE                  1
                ExceptionTable:
                  4 to 334 -> 344 [0]
                  344 to 362 -> 438 [1] lasti
                  364 to 414 -> 428 [1] lasti
@@ -1605,1189 +1583,1195 @@
                   'result'
                names      ('should_send_prompts', 'config', 'get', 'callable', 'args', 'kwargs', 'serialise_to_json', 'isinstance', 'str', 'set_span_attribute', 'SpanAttributes', 'AGIFLOW_ENTITY_OUTPUT', 'TypeError', 'logger', 'error')
                varnames   ('self', 'result', 'output', 'output_serializer', 'e')
                freevars   ()
                cellvars   ()
                filename   '/Users/vuongngo/workspace/agiflow/packages/python/agiflow-sdk/agiflow/opentelemetry/trace_decorators/wrapper.py'
                name       'capture_output'
-               firstlineno 228
+               firstlineno 224
                lnotab
                   0x020102011c010401340122012801040104011e022a011e021801160102
                   fe14f40611120148ff
-         names      ('__name__', '__module__', '__qualname__', '__doc__', 'Span', '__annotations__', 'Optional', 'AgiflowServiceTypes', 'Any', 'SharedKwargsWithHooks', 'Dict', 'str', 'TASK', '__init__', 'staticmethod', 'is_flush_on_exit', 'get_span_name', 'get_service_type', 'set_span_attribute', 'capture_input', 'capture_output')
+         names      ('__name__', '__module__', '__qualname__', '__doc__', 'Span', '__annotations__', 'Optional', 'AgiflowServiceTypes', 'Any', 'SharedKwargsWithHooks', 'Dict', 'str', 'TASK', '__init__', 'staticmethod', 'get_span_name', 'get_service_type', 'set_span_attribute', 'capture_input', 'capture_output')
          varnames   ()
          freevars   ()
          cellvars   ()
          filename   '/Users/vuongngo/workspace/agiflow/packages/python/agiflow-sdk/agiflow/opentelemetry/trace_decorators/wrapper.py'
          name       'BaseSpanCapture'
          firstlineno 80
          lnotab
             0x0c0104040a0116010a010a010a010a010a011a01160502010c02020102
-            f906030efd02040efc020802f80819020104ff0e010203020202010c0102
-            fd04010eff02020efe020302fd06ff0e01020e020104ff0e010206060b06
-            47
+            f906030efd02040efc020802f80819020202010c0102fd04010eff02020e
+            fe020302fd06ff0e01020e020104ff0e010206060b0647
       'BaseSpanCapture'
+      False
       'name'
       'tlp_service_type'
       'config'
       code
-         argcount  : 4
-         nlocals   : 6
-         stacksize : 5
+         argcount  : 5
+         nlocals   : 7
+         stacksize : 6
          flags     : 11
          code
-            0x870087018702870387049700880388048800880288016605640184087d
-            057c055300
+            0x8700870187028703870487059700880388058804880088028801660664
+            0184087d067c065300
                        0 MAKE_CELL                0 (name)
                        2 MAKE_CELL                1 (tlp_service_type)
                        4 MAKE_CELL                2 (span_kind)
                        6 MAKE_CELL                3 (SpanCapture)
-                       8 MAKE_CELL                4 (config)
+                       8 MAKE_CELL                4 (flush_on_exit)
+                      10 MAKE_CELL                5 (config)
          
-         251          10 RESUME                   0
+         247          12 RESUME                   0
          
-         258          12 LOAD_CLOSURE             3 (SpanCapture)
-                      14 LOAD_CLOSURE             4 (config)
-                      16 LOAD_CLOSURE             0 (name)
-                      18 LOAD_CLOSURE             2 (span_kind)
-                      20 LOAD_CLOSURE             1 (tlp_service_type)
-                      22 BUILD_TUPLE              5
-                      24 LOAD_CONST               1 (<code object decorate, file "/Users/vuongngo/workspace/agiflow/packages/python/agiflow-sdk/agiflow/opentelemetry/trace_decorators/wrapper.py", line 258>)
-                      26 MAKE_FUNCTION            8 (closure)
-                      28 STORE_FAST               5 (decorate)
+         255          14 LOAD_CLOSURE             3 (SpanCapture)
+                      16 LOAD_CLOSURE             5 (config)
+                      18 LOAD_CLOSURE             4 (flush_on_exit)
+                      20 LOAD_CLOSURE             0 (name)
+                      22 LOAD_CLOSURE             2 (span_kind)
+                      24 LOAD_CLOSURE             1 (tlp_service_type)
+                      26 BUILD_TUPLE              6
+                      28 LOAD_CONST               1 (<code object decorate, file "/Users/vuongngo/workspace/agiflow/packages/python/agiflow-sdk/agiflow/opentelemetry/trace_decorators/wrapper.py", line 255>)
+                      30 MAKE_FUNCTION            8 (closure)
+                      32 STORE_FAST               6 (decorate)
          
-         316          30 LOAD_FAST                5 (decorate)
-                      32 RETURN_VALUE
+         313          34 LOAD_FAST                6 (decorate)
+                      36 RETURN_VALUE
          consts
             None
             code
                argcount  : 1
                nlocals   : 2
-               stacksize : 7
+               stacksize : 8
                flags     : 19
                code
-                  0x9505870097007401000000000000000000008900a6010000ab01000000
-                  0000000000880288038800880488058806660664018408a6000000ab0000
-                  000000000000007d017c015300
-                             0 COPY_FREE_VARS           5
+                  0x9506870097007401000000000000000000008900a6010000ab01000000
+                  00000000008802880388048800880588068807660764018408a6000000ab
+                  0000000000000000007d017c015300
+                             0 COPY_FREE_VARS           6
                              2 MAKE_CELL                0 (fn)
                
-               258           4 RESUME                   0
+               255           4 RESUME                   0
                
-               259           6 LOAD_GLOBAL              1 (NULL + wraps)
+               256           6 LOAD_GLOBAL              1 (NULL + wraps)
                             18 LOAD_DEREF               0 (fn)
                             20 PRECALL                  1
                             24 CALL                     1
                
-               260          34 LOAD_CLOSURE             2 (SpanCapture)
+               257          34 LOAD_CLOSURE             2 (SpanCapture)
                             36 LOAD_CLOSURE             3 (config)
-                            38 LOAD_CLOSURE             0 (fn)
-                            40 LOAD_CLOSURE             4 (name)
-                            42 LOAD_CLOSURE             5 (span_kind)
-                            44 LOAD_CLOSURE             6 (tlp_service_type)
-                            46 BUILD_TUPLE              6
-                            48 LOAD_CONST               1 (<code object wrap, file "/Users/vuongngo/workspace/agiflow/packages/python/agiflow-sdk/agiflow/opentelemetry/trace_decorators/wrapper.py", line 259>)
-                            50 MAKE_FUNCTION            8 (closure)
+                            38 LOAD_CLOSURE             4 (flush_on_exit)
+                            40 LOAD_CLOSURE             0 (fn)
+                            42 LOAD_CLOSURE             5 (name)
+                            44 LOAD_CLOSURE             6 (span_kind)
+                            46 LOAD_CLOSURE             7 (tlp_service_type)
+                            48 BUILD_TUPLE              7
+                            50 LOAD_CONST               1 (<code object wrap, file "/Users/vuongngo/workspace/agiflow/packages/python/agiflow-sdk/agiflow/opentelemetry/trace_decorators/wrapper.py", line 256>)
+                            52 MAKE_FUNCTION            8 (closure)
                
-               259          52 PRECALL                  0
-                            56 CALL                     0
+               256          54 PRECALL                  0
+                            58 CALL                     0
                
-               260          66 STORE_FAST               1 (wrap)
+               257          68 STORE_FAST               1 (wrap)
                
-               314          68 LOAD_FAST                1 (wrap)
-                            70 RETURN_VALUE
+               311          70 LOAD_FAST                1 (wrap)
+                            72 RETURN_VALUE
                consts
                   None
                   code
                      argcount  : 0
                      nlocals   : 12
                      stacksize : 12
                      flags     : 31
                      code
-                        0x950697007401000000000000000000006a010000000000000000a60000
-                        00ab00000000000000000073080200890e7c0069007c01a4018e01530089
-                        0ca0020000000000000000000000000000000000000000890f8911890eac
+                        0x950797007401000000000000000000006a010000000000000000a60000
+                        00ab00000000000000000073080200890f7c0069007c01a4018e01530089
+                        0ca002000000000000000000000000000000000000000089108912890fac
                         01a6030000ab0300000000000000005c0200007d027d03890da003000000
                         00000000000000000000000000000000006402a6010000ab010000000000
                         0000007d0464007d057c0481267409000000000000000000007c04a60100
                         00ab010000000000000000721702007c047c0069007c01a4018e017d0674
                         0b000000000000000000007c06a6010000ab0100000000000000007d0574
-                        0d00000000000000000000890ca007000000000000000000000000000000
-                        0000000000a6000000ab000000000000000000ac03a6010000ab01000000
-                        000000000035007d077c07a0080000000000000000000000000000000000
-                        0000007c0289107c05ac04a6030000ab03000000000000000035007d0802
-                        00890c7c00890f7c037c08890e890d7c0564059c067c01a4018e017d0974
-                        13000000000000000000007c096406a6020000ab02000000000000000072
-                        287409000000000000000000007c096a0a0000000000000000a6010000ab
-                        01000000000000000072147c09a00a000000000000000000000000000000
-                        0000000000a6000000ab000000000000000000010009000200890e7c0069
-                        007c01a4018e017d0a7413000000000000000000007c096407a6020000ab
-                        02000000000000000072297409000000000000000000007c096a0b000000
-                        0000000000a6010000ab01000000000000000072157c09a00b0000000000
-                        0000000000000000000000000000007c0aa6010000ab0100000000000000
-                        0001007c08a00c0000000000000000000000000000000000000000a60000
-                        00ab00000000000000000072337c08a00d00000000000000000000000000
-                        00000000000000741c000000000000000000006a0f0000000000000000a6
-                        010000ab01000000000000000001007c08a0100000000000000000000000
-                        000000000000000000a6000000ab00000000000000000001007c0a630264
-                        0064006400a6020000ab02000000000000000001006302640064006400a6
-                        020000ab0200000000000000000100530023007422000000000000000000
-                        00240072557d0b7c08a01200000000000000000000000000000000000000
-                        007c0ba6010000ab01000000000000000001007c08a00d00000000000000
-                        00000000000000000000000000742700000000000000000000741c000000
-                        000000000000006a140000000000000000742b000000000000000000007c
-                        0ba6010000ab010000000000000000a6020000ab020000000000000000a6
-                        010000ab0100000000000000000100820064007d0b7e0b77017700780359
-                        007701230031007304770278035900770101005900010001000900640064
-                        006400a6020000ab02000000000000000001006400530023003100730477
-                        02780359007701010059000100010064005300
-                                   0 COPY_FREE_VARS           6
+                        0d00000000000000000000890eac03a6010000ab01000000000000000035
+                        007d077c07a00700000000000000000000000000000000000000007c0289
+                        117c05ac04a6030000ab03000000000000000035007d080200890c7c0089
+                        107c037c08890f890d7c0564059c067c01a4018e017d0974110000000000
+                        00000000007c096406a6020000ab02000000000000000072287409000000
+                        000000000000007c096a090000000000000000a6010000ab010000000000
+                        00000072147c09a0090000000000000000000000000000000000000000a6
+                        000000ab000000000000000000010009000200890f7c0069007c01a4018e
+                        017d0a7411000000000000000000007c096407a6020000ab020000000000
+                        00000072297409000000000000000000007c096a0a0000000000000000a6
+                        010000ab01000000000000000072157c09a00a0000000000000000000000
+                        0000000000000000007c0aa6010000ab01000000000000000001007c08a0
+                        0b0000000000000000000000000000000000000000a6000000ab00000000
+                        000000000072337c08a00c00000000000000000000000000000000000000
+                        00741a000000000000000000006a0e0000000000000000a6010000ab0100
+                        0000000000000001007c08a00f0000000000000000000000000000000000
+                        000000a6000000ab00000000000000000001007c0a6302640064006400a6
+                        020000ab02000000000000000001006302640064006400a6020000ab0200
+                        00000000000000010053002300742000000000000000000000240072557d
+                        0b7c08a01100000000000000000000000000000000000000007c0ba60100
+                        00ab01000000000000000001007c08a00c00000000000000000000000000
+                        00000000000000742500000000000000000000741a000000000000000000
+                        006a1300000000000000007429000000000000000000007c0ba6010000ab
+                        010000000000000000a6020000ab020000000000000000a6010000ab0100
+                        000000000000000100820064007d0b7e0b77017700780359007701230031
+                        007304770278035900770101005900010001000900640064006400a60200
+                        00ab02000000000000000001006400530023003100730477027803590077
+                        01010059000100010064005300
+                                   0 COPY_FREE_VARS           7
                      
-                     259           2 RESUME                   0
+                     256           2 RESUME                   0
                      
-                     261           4 LOAD_GLOBAL              1 (NULL + TracerWrapper)
+                     258           4 LOAD_GLOBAL              1 (NULL + TracerWrapper)
                                   16 LOAD_ATTR                1 (verify_initialized)
                                   26 PRECALL                  0
                                   30 CALL                     0
                                   40 POP_JUMP_FORWARD_IF_TRUE     8 (to 58)
                      
-                     262          42 PUSH_NULL
-                                  44 LOAD_DEREF              14 (fn)
+                     259          42 PUSH_NULL
+                                  44 LOAD_DEREF              15 (fn)
                                   46 LOAD_FAST                0 (args)
                                   48 BUILD_MAP                0
                                   50 LOAD_FAST                1 (kwargs)
                                   52 DICT_MERGE               1
                                   54 CALL_FUNCTION_EX         1
                                   56 RETURN_VALUE
                      
-                     264     >>   58 LOAD_DEREF              12 (SpanCapture)
+                     261     >>   58 LOAD_DEREF              12 (SpanCapture)
                                   60 LOAD_METHOD              2 (get_span_name)
                      
-                     265          82 LOAD_DEREF              15 (name)
+                     262          82 LOAD_DEREF              16 (name)
                      
-                     266          84 LOAD_DEREF              17 (tlp_service_type)
+                     263          84 LOAD_DEREF              18 (tlp_service_type)
                      
-                     267          86 LOAD_DEREF              14 (fn)
+                     264          86 LOAD_DEREF              15 (fn)
                      
-                     264          88 KW_NAMES                 1
+                     261          88 KW_NAMES                 1
                                   90 PRECALL                  3
                                   94 CALL                     3
                                  104 UNPACK_SEQUENCE          2
                                  108 STORE_FAST               2 (span_name)
                                  110 STORE_FAST               3 (service_type)
                      
-                     270         112 LOAD_DEREF              13 (config)
+                     267         112 LOAD_DEREF              13 (config)
                                  114 LOAD_METHOD              3 (get)
                                  136 LOAD_CONST               2 ('context_parser')
                                  138 PRECALL                  1
                                  142 CALL                     1
                                  152 STORE_FAST               4 (context_parser)
                      
-                     271         154 LOAD_CONST               0 (None)
+                     268         154 LOAD_CONST               0 (None)
                                  156 STORE_FAST               5 (context)
                      
-                     272         158 LOAD_FAST                4 (context_parser)
+                     269         158 LOAD_FAST                4 (context_parser)
                                  160 POP_JUMP_FORWARD_IF_NONE    38 (to 238)
                                  162 LOAD_GLOBAL              9 (NULL + callable)
                                  174 LOAD_FAST                4 (context_parser)
                                  176 PRECALL                  1
                                  180 CALL                     1
                                  190 POP_JUMP_FORWARD_IF_FALSE    23 (to 238)
                      
-                     273         192 PUSH_NULL
+                     270         192 PUSH_NULL
                                  194 LOAD_FAST                4 (context_parser)
                                  196 LOAD_FAST                0 (args)
                                  198 BUILD_MAP                0
                                  200 LOAD_FAST                1 (kwargs)
                                  202 DICT_MERGE               1
                                  204 CALL_FUNCTION_EX         1
                                  206 STORE_FAST               6 (carrier)
                      
-                     274         208 LOAD_GLOBAL             11 (NULL + get_trace_context_from_carrier)
+                     271         208 LOAD_GLOBAL             11 (NULL + get_trace_context_from_carrier)
                                  220 LOAD_FAST                6 (carrier)
                                  222 PRECALL                  1
                                  226 CALL                     1
                                  236 STORE_FAST               5 (context)
                      
-                     276     >>  238 LOAD_GLOBAL             13 (NULL + get_tracer)
-                                 250 LOAD_DEREF              12 (SpanCapture)
-                                 252 LOAD_METHOD              7 (is_flush_on_exit)
-                                 274 PRECALL                  0
-                                 278 CALL                     0
-                                 288 KW_NAMES                 3
-                                 290 PRECALL                  1
-                                 294 CALL                     1
-                                 304 BEFORE_WITH
-                                 306 STORE_FAST               7 (tracer)
-                     
-                     277         308 LOAD_FAST                7 (tracer)
-                                 310 LOAD_METHOD              8 (start_as_current_span)
-                                 332 LOAD_FAST                2 (span_name)
-                                 334 LOAD_DEREF              16 (span_kind)
-                                 336 LOAD_FAST                5 (context)
-                                 338 KW_NAMES                 4
-                                 340 PRECALL                  3
-                                 344 CALL                     3
-                                 354 BEFORE_WITH
-                                 356 STORE_FAST               8 (span)
-                     
-                     278         358 PUSH_NULL
-                                 360 LOAD_DEREF              12 (SpanCapture)
-                     
-                     279         362 LOAD_FAST                0 (args)
-                     
-                     280         364 LOAD_DEREF              15 (name)
-                     
-                     281         366 LOAD_FAST                3 (service_type)
-                     
-                     282         368 LOAD_FAST                8 (span)
-                     
-                     283         370 LOAD_DEREF              14 (fn)
-                     
-                     284         372 LOAD_DEREF              13 (config)
-                     
-                     285         374 LOAD_FAST                5 (context)
-                     
-                     278         376 LOAD_CONST               5 (('name', 'service_type', 'span', 'instance', 'config', 'context'))
-                                 378 BUILD_CONST_KEY_MAP      6
-                     
-                     286         380 LOAD_FAST                1 (kwargs)
-                     
-                     278         382 DICT_MERGE               1
-                                 384 CALL_FUNCTION_EX         1
-                                 386 STORE_FAST               9 (span_capture)
-                     
-                     288         388 LOAD_GLOBAL             19 (NULL + hasattr)
-                                 400 LOAD_FAST                9 (span_capture)
-                                 402 LOAD_CONST               6 ('capture_input')
-                                 404 PRECALL                  2
-                                 408 CALL                     2
-                                 418 POP_JUMP_FORWARD_IF_FALSE    40 (to 500)
-                                 420 LOAD_GLOBAL              9 (NULL + callable)
-                                 432 LOAD_FAST                9 (span_capture)
-                                 434 LOAD_ATTR               10 (capture_input)
-                                 444 PRECALL                  1
-                                 448 CALL                     1
-                                 458 POP_JUMP_FORWARD_IF_FALSE    20 (to 500)
-                     
-                     289         460 LOAD_FAST                9 (span_capture)
-                                 462 LOAD_METHOD             10 (capture_input)
-                                 484 PRECALL                  0
-                                 488 CALL                     0
-                                 498 POP_TOP
-                     
-                     291     >>  500 NOP
-                     
-                     292         502 PUSH_NULL
-                                 504 LOAD_DEREF              14 (fn)
-                                 506 LOAD_FAST                0 (args)
-                                 508 BUILD_MAP                0
-                                 510 LOAD_FAST                1 (kwargs)
-                                 512 DICT_MERGE               1
-                                 514 CALL_FUNCTION_EX         1
-                                 516 STORE_FAST              10 (res)
-                     
-                     294         518 LOAD_GLOBAL             19 (NULL + hasattr)
-                                 530 LOAD_FAST                9 (span_capture)
-                                 532 LOAD_CONST               7 ('capture_output')
-                                 534 PRECALL                  2
-                                 538 CALL                     2
-                                 548 POP_JUMP_FORWARD_IF_FALSE    41 (to 632)
-                                 550 LOAD_GLOBAL              9 (NULL + callable)
-                                 562 LOAD_FAST                9 (span_capture)
-                                 564 LOAD_ATTR               11 (capture_output)
-                                 574 PRECALL                  1
-                                 578 CALL                     1
-                                 588 POP_JUMP_FORWARD_IF_FALSE    21 (to 632)
-                     
-                     295         590 LOAD_FAST                9 (span_capture)
-                                 592 LOAD_METHOD             11 (capture_output)
-                                 614 LOAD_FAST               10 (res)
-                                 616 PRECALL                  1
-                                 620 CALL                     1
-                                 630 POP_TOP
-                     
-                     297     >>  632 LOAD_FAST                8 (span)
-                                 634 LOAD_METHOD             12 (is_recording)
-                                 656 PRECALL                  0
-                                 660 CALL                     0
-                                 670 POP_JUMP_FORWARD_IF_FALSE    51 (to 774)
-                     
-                     299         672 LOAD_FAST                8 (span)
-                                 674 LOAD_METHOD             13 (set_status)
-                                 696 LOAD_GLOBAL             28 (StatusCode)
-                                 708 LOAD_ATTR               15 (OK)
-                                 718 PRECALL                  1
-                                 722 CALL                     1
-                                 732 POP_TOP
-                     
-                     300         734 LOAD_FAST                8 (span)
-                                 736 LOAD_METHOD             16 (end)
-                                 758 PRECALL                  0
-                                 762 CALL                     0
-                                 772 POP_TOP
-                     
-                     302     >>  774 LOAD_FAST               10 (res)
-                     
-                     277         776 SWAP                     2
-                                 778 LOAD_CONST               0 (None)
-                                 780 LOAD_CONST               0 (None)
-                                 782 LOAD_CONST               0 (None)
-                                 784 PRECALL                  2
-                                 788 CALL                     2
-                                 798 POP_TOP
-                     
-                     276         800 SWAP                     2
-                                 802 LOAD_CONST               0 (None)
-                                 804 LOAD_CONST               0 (None)
-                                 806 LOAD_CONST               0 (None)
-                                 808 PRECALL                  2
-                                 812 CALL                     2
-                                 822 POP_TOP
-                                 824 RETURN_VALUE
-                             >>  826 PUSH_EXC_INFO
-                     
-                     304         828 LOAD_GLOBAL             34 (Exception)
-                                 840 CHECK_EXC_MATCH
-                                 842 POP_JUMP_FORWARD_IF_FALSE    85 (to 1014)
-                                 844 STORE_FAST              11 (err)
-                     
-                     306         846 LOAD_FAST                8 (span)
-                                 848 LOAD_METHOD             18 (record_exception)
-                                 870 LOAD_FAST               11 (err)
-                                 872 PRECALL                  1
-                                 876 CALL                     1
-                                 886 POP_TOP
-                     
-                     309         888 LOAD_FAST                8 (span)
-                                 890 LOAD_METHOD             13 (set_status)
-                                 912 LOAD_GLOBAL             39 (NULL + Status)
-                                 924 LOAD_GLOBAL             28 (StatusCode)
-                                 936 LOAD_ATTR               20 (ERROR)
-                                 946 LOAD_GLOBAL             43 (NULL + str)
-                                 958 LOAD_FAST               11 (err)
-                                 960 PRECALL                  1
-                                 964 CALL                     1
-                                 974 PRECALL                  2
-                                 978 CALL                     2
-                                 988 PRECALL                  1
-                                 992 CALL                     1
-                                1002 POP_TOP
-                     
-                     312        1004 RAISE_VARARGS            0
-                             >> 1006 LOAD_CONST               0 (None)
-                                1008 STORE_FAST              11 (err)
-                                1010 DELETE_FAST             11 (err)
-                                1012 RERAISE                  1
-                     
-                     304     >> 1014 RERAISE                  0
-                             >> 1016 COPY                     3
-                                1018 POP_EXCEPT
-                                1020 RERAISE                  1
-                     
-                     277     >> 1022 PUSH_EXC_INFO
-                                1024 WITH_EXCEPT_START
-                                1026 POP_JUMP_FORWARD_IF_TRUE     4 (to 1036)
-                                1028 RERAISE                  2
-                             >> 1030 COPY                     3
-                                1032 POP_EXCEPT
-                                1034 RERAISE                  1
-                             >> 1036 POP_TOP
-                                1038 POP_EXCEPT
-                                1040 POP_TOP
-                                1042 POP_TOP
-                                1044 NOP
-                     
-                     276        1046 LOAD_CONST               0 (None)
-                                1048 LOAD_CONST               0 (None)
-                                1050 LOAD_CONST               0 (None)
-                                1052 PRECALL                  2
-                                1056 CALL                     2
-                                1066 POP_TOP
-                                1068 LOAD_CONST               0 (None)
-                                1070 RETURN_VALUE
-                             >> 1072 PUSH_EXC_INFO
-                                1074 WITH_EXCEPT_START
-                                1076 POP_JUMP_FORWARD_IF_TRUE     4 (to 1086)
-                                1078 RERAISE                  2
-                             >> 1080 COPY                     3
-                                1082 POP_EXCEPT
-                                1084 RERAISE                  1
-                             >> 1086 POP_TOP
-                                1088 POP_EXCEPT
-                                1090 POP_TOP
-                                1092 POP_TOP
-                                1094 LOAD_CONST               0 (None)
-                                1096 RETURN_VALUE
+                     273     >>  238 LOAD_GLOBAL             13 (NULL + get_tracer)
+                                 250 LOAD_DEREF              14 (flush_on_exit)
+                                 252 KW_NAMES                 3
+                                 254 PRECALL                  1
+                                 258 CALL                     1
+                                 268 BEFORE_WITH
+                                 270 STORE_FAST               7 (tracer)
+                     
+                     274         272 LOAD_FAST                7 (tracer)
+                                 274 LOAD_METHOD              7 (start_as_current_span)
+                                 296 LOAD_FAST                2 (span_name)
+                                 298 LOAD_DEREF              17 (span_kind)
+                                 300 LOAD_FAST                5 (context)
+                                 302 KW_NAMES                 4
+                                 304 PRECALL                  3
+                                 308 CALL                     3
+                                 318 BEFORE_WITH
+                                 320 STORE_FAST               8 (span)
+                     
+                     275         322 PUSH_NULL
+                                 324 LOAD_DEREF              12 (SpanCapture)
+                     
+                     276         326 LOAD_FAST                0 (args)
+                     
+                     277         328 LOAD_DEREF              16 (name)
+                     
+                     278         330 LOAD_FAST                3 (service_type)
+                     
+                     279         332 LOAD_FAST                8 (span)
+                     
+                     280         334 LOAD_DEREF              15 (fn)
+                     
+                     281         336 LOAD_DEREF              13 (config)
+                     
+                     282         338 LOAD_FAST                5 (context)
+                     
+                     275         340 LOAD_CONST               5 (('name', 'service_type', 'span', 'instance', 'config', 'context'))
+                                 342 BUILD_CONST_KEY_MAP      6
+                     
+                     283         344 LOAD_FAST                1 (kwargs)
+                     
+                     275         346 DICT_MERGE               1
+                                 348 CALL_FUNCTION_EX         1
+                                 350 STORE_FAST               9 (span_capture)
+                     
+                     285         352 LOAD_GLOBAL             17 (NULL + hasattr)
+                                 364 LOAD_FAST                9 (span_capture)
+                                 366 LOAD_CONST               6 ('capture_input')
+                                 368 PRECALL                  2
+                                 372 CALL                     2
+                                 382 POP_JUMP_FORWARD_IF_FALSE    40 (to 464)
+                                 384 LOAD_GLOBAL              9 (NULL + callable)
+                                 396 LOAD_FAST                9 (span_capture)
+                                 398 LOAD_ATTR                9 (capture_input)
+                                 408 PRECALL                  1
+                                 412 CALL                     1
+                                 422 POP_JUMP_FORWARD_IF_FALSE    20 (to 464)
+                     
+                     286         424 LOAD_FAST                9 (span_capture)
+                                 426 LOAD_METHOD              9 (capture_input)
+                                 448 PRECALL                  0
+                                 452 CALL                     0
+                                 462 POP_TOP
+                     
+                     288     >>  464 NOP
+                     
+                     289         466 PUSH_NULL
+                                 468 LOAD_DEREF              15 (fn)
+                                 470 LOAD_FAST                0 (args)
+                                 472 BUILD_MAP                0
+                                 474 LOAD_FAST                1 (kwargs)
+                                 476 DICT_MERGE               1
+                                 478 CALL_FUNCTION_EX         1
+                                 480 STORE_FAST              10 (res)
+                     
+                     291         482 LOAD_GLOBAL             17 (NULL + hasattr)
+                                 494 LOAD_FAST                9 (span_capture)
+                                 496 LOAD_CONST               7 ('capture_output')
+                                 498 PRECALL                  2
+                                 502 CALL                     2
+                                 512 POP_JUMP_FORWARD_IF_FALSE    41 (to 596)
+                                 514 LOAD_GLOBAL              9 (NULL + callable)
+                                 526 LOAD_FAST                9 (span_capture)
+                                 528 LOAD_ATTR               10 (capture_output)
+                                 538 PRECALL                  1
+                                 542 CALL                     1
+                                 552 POP_JUMP_FORWARD_IF_FALSE    21 (to 596)
+                     
+                     292         554 LOAD_FAST                9 (span_capture)
+                                 556 LOAD_METHOD             10 (capture_output)
+                                 578 LOAD_FAST               10 (res)
+                                 580 PRECALL                  1
+                                 584 CALL                     1
+                                 594 POP_TOP
+                     
+                     294     >>  596 LOAD_FAST                8 (span)
+                                 598 LOAD_METHOD             11 (is_recording)
+                                 620 PRECALL                  0
+                                 624 CALL                     0
+                                 634 POP_JUMP_FORWARD_IF_FALSE    51 (to 738)
+                     
+                     296         636 LOAD_FAST                8 (span)
+                                 638 LOAD_METHOD             12 (set_status)
+                                 660 LOAD_GLOBAL             26 (StatusCode)
+                                 672 LOAD_ATTR               14 (OK)
+                                 682 PRECALL                  1
+                                 686 CALL                     1
+                                 696 POP_TOP
+                     
+                     297         698 LOAD_FAST                8 (span)
+                                 700 LOAD_METHOD             15 (end)
+                                 722 PRECALL                  0
+                                 726 CALL                     0
+                                 736 POP_TOP
+                     
+                     299     >>  738 LOAD_FAST               10 (res)
+                     
+                     274         740 SWAP                     2
+                                 742 LOAD_CONST               0 (None)
+                                 744 LOAD_CONST               0 (None)
+                                 746 LOAD_CONST               0 (None)
+                                 748 PRECALL                  2
+                                 752 CALL                     2
+                                 762 POP_TOP
+                     
+                     273         764 SWAP                     2
+                                 766 LOAD_CONST               0 (None)
+                                 768 LOAD_CONST               0 (None)
+                                 770 LOAD_CONST               0 (None)
+                                 772 PRECALL                  2
+                                 776 CALL                     2
+                                 786 POP_TOP
+                                 788 RETURN_VALUE
+                             >>  790 PUSH_EXC_INFO
+                     
+                     301         792 LOAD_GLOBAL             32 (Exception)
+                                 804 CHECK_EXC_MATCH
+                                 806 POP_JUMP_FORWARD_IF_FALSE    85 (to 978)
+                                 808 STORE_FAST              11 (err)
+                     
+                     303         810 LOAD_FAST                8 (span)
+                                 812 LOAD_METHOD             17 (record_exception)
+                                 834 LOAD_FAST               11 (err)
+                                 836 PRECALL                  1
+                                 840 CALL                     1
+                                 850 POP_TOP
+                     
+                     306         852 LOAD_FAST                8 (span)
+                                 854 LOAD_METHOD             12 (set_status)
+                                 876 LOAD_GLOBAL             37 (NULL + Status)
+                                 888 LOAD_GLOBAL             26 (StatusCode)
+                                 900 LOAD_ATTR               19 (ERROR)
+                                 910 LOAD_GLOBAL             41 (NULL + str)
+                                 922 LOAD_FAST               11 (err)
+                                 924 PRECALL                  1
+                                 928 CALL                     1
+                                 938 PRECALL                  2
+                                 942 CALL                     2
+                                 952 PRECALL                  1
+                                 956 CALL                     1
+                                 966 POP_TOP
+                     
+                     309         968 RAISE_VARARGS            0
+                             >>  970 LOAD_CONST               0 (None)
+                                 972 STORE_FAST              11 (err)
+                                 974 DELETE_FAST             11 (err)
+                                 976 RERAISE                  1
+                     
+                     301     >>  978 RERAISE                  0
+                             >>  980 COPY                     3
+                                 982 POP_EXCEPT
+                                 984 RERAISE                  1
+                     
+                     274     >>  986 PUSH_EXC_INFO
+                                 988 WITH_EXCEPT_START
+                                 990 POP_JUMP_FORWARD_IF_TRUE     4 (to 1000)
+                                 992 RERAISE                  2
+                             >>  994 COPY                     3
+                                 996 POP_EXCEPT
+                                 998 RERAISE                  1
+                             >> 1000 POP_TOP
+                                1002 POP_EXCEPT
+                                1004 POP_TOP
+                                1006 POP_TOP
+                                1008 NOP
+                     
+                     273        1010 LOAD_CONST               0 (None)
+                                1012 LOAD_CONST               0 (None)
+                                1014 LOAD_CONST               0 (None)
+                                1016 PRECALL                  2
+                                1020 CALL                     2
+                                1030 POP_TOP
+                                1032 LOAD_CONST               0 (None)
+                                1034 RETURN_VALUE
+                             >> 1036 PUSH_EXC_INFO
+                                1038 WITH_EXCEPT_START
+                                1040 POP_JUMP_FORWARD_IF_TRUE     4 (to 1050)
+                                1042 RERAISE                  2
+                             >> 1044 COPY                     3
+                                1046 POP_EXCEPT
+                                1048 RERAISE                  1
+                             >> 1050 POP_TOP
+                                1052 POP_EXCEPT
+                                1054 POP_TOP
+                                1056 POP_TOP
+                                1058 LOAD_CONST               0 (None)
+                                1060 RETURN_VALUE
                      ExceptionTable:
-                       306 to 354 -> 1072 [1] lasti
-                       356 to 498 -> 1022 [2] lasti
-                       502 to 774 -> 826 [2]
-                       776 to 798 -> 1072 [1] lasti
-                       826 to 844 -> 1016 [3] lasti
-                       846 to 1004 -> 1006 [3] lasti
-                       1006 to 1014 -> 1016 [3] lasti
-                       1016 to 1020 -> 1022 [2] lasti
-                       1022 to 1028 -> 1030 [4] lasti
-                       1030 to 1034 -> 1072 [1] lasti
-                       1036 to 1036 -> 1030 [4] lasti
-                       1038 to 1042 -> 1072 [1] lasti
-                       1072 to 1078 -> 1080 [3] lasti
-                       1086 to 1086 -> 1080 [3] lasti
+                       270 to 318 -> 1036 [1] lasti
+                       320 to 462 -> 986 [2] lasti
+                       466 to 738 -> 790 [2]
+                       740 to 762 -> 1036 [1] lasti
+                       790 to 808 -> 980 [3] lasti
+                       810 to 968 -> 970 [3] lasti
+                       970 to 978 -> 980 [3] lasti
+                       980 to 984 -> 986 [2] lasti
+                       986 to 992 -> 994 [4] lasti
+                       994 to 998 -> 1036 [1] lasti
+                       1000 to 1000 -> 994 [4] lasti
+                       1002 to 1006 -> 1036 [1] lasti
+                       1036 to 1042 -> 1044 [3] lasti
+                       1050 to 1050 -> 1044 [3] lasti
                      consts
                         None
                         ('name', 'tlp_service_type', 'instance')
                         'context_parser'
                         ('flush_on_exit',)
                         ('kind', 'context')
                         ('name', 'service_type', 'span', 'instance', 'config', 'context')
                         'capture_input'
                         'capture_output'
-                     names      ('TracerWrapper', 'verify_initialized', 'get_span_name', 'get', 'callable', 'get_trace_context_from_carrier', 'get_tracer', 'is_flush_on_exit', 'start_as_current_span', 'hasattr', 'capture_input', 'capture_output', 'is_recording', 'set_status', 'StatusCode', 'OK', 'end', 'Exception', 'record_exception', 'Status', 'ERROR', 'str')
+                     names      ('TracerWrapper', 'verify_initialized', 'get_span_name', 'get', 'callable', 'get_trace_context_from_carrier', 'get_tracer', 'start_as_current_span', 'hasattr', 'capture_input', 'capture_output', 'is_recording', 'set_status', 'StatusCode', 'OK', 'end', 'Exception', 'record_exception', 'Status', 'ERROR', 'str')
                      varnames   ('args', 'kwargs', 'span_name', 'service_type', 'context_parser', 'context', 'carrier', 'tracer', 'span', 'span_capture', 'res', 'err')
-                     freevars   ('SpanCapture', 'config', 'fn', 'name', 'span_kind', 'tlp_service_type')
+                     freevars   ('SpanCapture', 'config', 'flush_on_exit', 'fn', 'name', 'span_kind', 'tlp_service_type')
                      cellvars   ()
                      filename   '/Users/vuongngo/workspace/agiflow/packages/python/agiflow-sdk/agiflow/opentelemetry/trace_decorators/wrapper.py'
                      name       'wrap'
-                     firstlineno 259
+                     firstlineno 256
                      lnotab
-                        0x04022601100218010201020102fd18062a010401220110011e02460132
+                        0x04022601100218010201020102fd18062a010401220110011e02220132
                         01040102010201020102010201020102f9040802f8060a48012802020110
                         0248012a0228023e01280202e718ff1c1c12022a0374030af808e518ff
                names      ('wraps',)
                varnames   ('fn', 'wrap')
-               freevars   ('SpanCapture', 'config', 'name', 'span_kind', 'tlp_service_type')
+               freevars   ('SpanCapture', 'config', 'flush_on_exit', 'name', 'span_kind', 'tlp_service_type')
                cellvars   ('fn',)
                filename   '/Users/vuongngo/workspace/agiflow/packages/python/agiflow-sdk/agiflow/opentelemetry/trace_decorators/wrapper.py'
                name       'decorate'
-               firstlineno 258
-               lnotab 0x06011c0112ff0e010236
+               firstlineno 255
+               lnotab 0x06011c0114ff0e010236
          names      ()
-         varnames   ('name', 'tlp_service_type', 'span_kind', 'SpanCapture', 'config', 'decorate')
+         varnames   ('name', 'tlp_service_type', 'span_kind', 'SpanCapture', 'flush_on_exit', 'config', 'decorate')
          freevars   ()
-         cellvars   ('name', 'tlp_service_type', 'span_kind', 'SpanCapture', 'config')
+         cellvars   ('name', 'tlp_service_type', 'span_kind', 'SpanCapture', 'flush_on_exit', 'config')
          filename   '/Users/vuongngo/workspace/agiflow/packages/python/agiflow-sdk/agiflow/opentelemetry/trace_decorators/wrapper.py'
          name       'decorate_method'
-         firstlineno 251
-         lnotab 0x0c07123a
+         firstlineno 247
+         lnotab 0x0e08143a
       code
-         argcount  : 4
-         nlocals   : 6
-         stacksize : 5
+         argcount  : 5
+         nlocals   : 7
+         stacksize : 6
          flags     : 11
          code
-            0x870087018702870387049700880388048800880288016605640184087d
-            057c055300
+            0x8700870187028703870487059700880388058804880088028801660664
+            0184087d067c065300
                        0 MAKE_CELL                0 (name)
                        2 MAKE_CELL                1 (tlp_service_type)
                        4 MAKE_CELL                2 (span_kind)
                        6 MAKE_CELL                3 (SpanCapture)
-                       8 MAKE_CELL                4 (config)
+                       8 MAKE_CELL                4 (flush_on_exit)
+                      10 MAKE_CELL                5 (config)
          
-         319          10 RESUME                   0
+         316          12 RESUME                   0
          
-         326          12 LOAD_CLOSURE             3 (SpanCapture)
-                      14 LOAD_CLOSURE             4 (config)
-                      16 LOAD_CLOSURE             0 (name)
-                      18 LOAD_CLOSURE             2 (span_kind)
-                      20 LOAD_CLOSURE             1 (tlp_service_type)
-                      22 BUILD_TUPLE              5
-                      24 LOAD_CONST               1 (<code object decorate, file "/Users/vuongngo/workspace/agiflow/packages/python/agiflow-sdk/agiflow/opentelemetry/trace_decorators/wrapper.py", line 326>)
-                      26 MAKE_FUNCTION            8 (closure)
-                      28 STORE_FAST               5 (decorate)
+         324          14 LOAD_CLOSURE             3 (SpanCapture)
+                      16 LOAD_CLOSURE             5 (config)
+                      18 LOAD_CLOSURE             4 (flush_on_exit)
+                      20 LOAD_CLOSURE             0 (name)
+                      22 LOAD_CLOSURE             2 (span_kind)
+                      24 LOAD_CLOSURE             1 (tlp_service_type)
+                      26 BUILD_TUPLE              6
+                      28 LOAD_CONST               1 (<code object decorate, file "/Users/vuongngo/workspace/agiflow/packages/python/agiflow-sdk/agiflow/opentelemetry/trace_decorators/wrapper.py", line 324>)
+                      30 MAKE_FUNCTION            8 (closure)
+                      32 STORE_FAST               6 (decorate)
          
-         384          30 LOAD_FAST                5 (decorate)
-                      32 RETURN_VALUE
+         382          34 LOAD_FAST                6 (decorate)
+                      36 RETURN_VALUE
          consts
             None
             code
                argcount  : 1
                nlocals   : 2
-               stacksize : 7
+               stacksize : 8
                flags     : 19
                code
-                  0x9505870097007401000000000000000000008900a6010000ab01000000
-                  0000000000880288038800880488058806660664018408a6000000ab0000
-                  000000000000007d017c015300
-                             0 COPY_FREE_VARS           5
+                  0x9506870097007401000000000000000000008900a6010000ab01000000
+                  00000000008802880388048800880588068807660764018408a6000000ab
+                  0000000000000000007d017c015300
+                             0 COPY_FREE_VARS           6
                              2 MAKE_CELL                0 (fn)
                
-               326           4 RESUME                   0
+               324           4 RESUME                   0
                
-               327           6 LOAD_GLOBAL              1 (NULL + wraps)
+               325           6 LOAD_GLOBAL              1 (NULL + wraps)
                             18 LOAD_DEREF               0 (fn)
                             20 PRECALL                  1
                             24 CALL                     1
                
-               328          34 LOAD_CLOSURE             2 (SpanCapture)
+               326          34 LOAD_CLOSURE             2 (SpanCapture)
                             36 LOAD_CLOSURE             3 (config)
-                            38 LOAD_CLOSURE             0 (fn)
-                            40 LOAD_CLOSURE             4 (name)
-                            42 LOAD_CLOSURE             5 (span_kind)
-                            44 LOAD_CLOSURE             6 (tlp_service_type)
-                            46 BUILD_TUPLE              6
-                            48 LOAD_CONST               1 (<code object wrap, file "/Users/vuongngo/workspace/agiflow/packages/python/agiflow-sdk/agiflow/opentelemetry/trace_decorators/wrapper.py", line 327>)
-                            50 MAKE_FUNCTION            8 (closure)
+                            38 LOAD_CLOSURE             4 (flush_on_exit)
+                            40 LOAD_CLOSURE             0 (fn)
+                            42 LOAD_CLOSURE             5 (name)
+                            44 LOAD_CLOSURE             6 (span_kind)
+                            46 LOAD_CLOSURE             7 (tlp_service_type)
+                            48 BUILD_TUPLE              7
+                            50 LOAD_CONST               1 (<code object wrap, file "/Users/vuongngo/workspace/agiflow/packages/python/agiflow-sdk/agiflow/opentelemetry/trace_decorators/wrapper.py", line 325>)
+                            52 MAKE_FUNCTION            8 (closure)
                
-               327          52 PRECALL                  0
-                            56 CALL                     0
+               325          54 PRECALL                  0
+                            58 CALL                     0
                
-               328          66 STORE_FAST               1 (wrap)
+               326          68 STORE_FAST               1 (wrap)
                
-               382          68 LOAD_FAST                1 (wrap)
-                            70 RETURN_VALUE
+               380          70 LOAD_FAST                1 (wrap)
+                            72 RETURN_VALUE
                consts
                   None
                   code
                      argcount  : 0
                      nlocals   : 12
                      stacksize : 12
                      flags     : 159
                      code
-                        0x95064b00010097007401000000000000000000006a0100000000000000
-                        00a6000000ab00000000000000000073080200890e7c0069007c01a4018e
-                        015300890ca0020000000000000000000000000000000000000000890f89
-                        11890eac01a6030000ab0300000000000000005c0200007d027d03890da0
+                        0x95074b00010097007401000000000000000000006a0100000000000000
+                        00a6000000ab00000000000000000073080200890f7c0069007c01a4018e
+                        015300890ca0020000000000000000000000000000000000000000891089
+                        12890fac01a6030000ab0300000000000000005c0200007d027d03890da0
                         0300000000000000000000000000000000000000006402a6010000ab0100
                         000000000000007d0464007d057c0481267409000000000000000000007c
                         04a6010000ab010000000000000000721702007c047c0069007c01a4018e
                         017d06740b000000000000000000007c06a6010000ab0100000000000000
-                        007d05740d00000000000000000000890ca0070000000000000000000000
-                        000000000000000000a6000000ab000000000000000000ac03a6010000ab
-                        01000000000000000035007d077c07a00800000000000000000000000000
-                        000000000000007c0289107c05ac04a6030000ab03000000000000000035
-                        007d080200890c7c00890f7c037c08890e890d7c0564059c067c01a4018e
-                        017d097413000000000000000000007c096406a6020000ab020000000000
-                        00000072287409000000000000000000007c096a0a0000000000000000a6
-                        010000ab01000000000000000072147c09a00a0000000000000000000000
-                        000000000000000000a6000000ab00000000000000000001000900020089
-                        0e7c0069007c01a4018e01830064007b035600970386047d0a7413000000
-                        000000000000007c096407a6020000ab0200000000000000007229740900
-                        0000000000000000007c096a0b0000000000000000a6010000ab01000000
-                        000000000072157c09a00b00000000000000000000000000000000000000
-                        007c0aa6010000ab01000000000000000001007c08a00c00000000000000
-                        00000000000000000000000000a6000000ab00000000000000000072337c
-                        08a00d0000000000000000000000000000000000000000741c0000000000
-                        00000000006a0f0000000000000000a6010000ab01000000000000000001
-                        007c08a0100000000000000000000000000000000000000000a6000000ab
-                        00000000000000000001007c0a6302640064006400a6020000ab02000000
-                        000000000001006302640064006400a6020000ab02000000000000000001
-                        0053002300742200000000000000000000240072697d0b7c08a012000000
-                        00000000000000000000000000000000007c0ba6010000ab010000000000
-                        00000001007c08a00d000000000000000000000000000000000000000074
-                        2700000000000000000000741c000000000000000000006a140000000000
-                        000000742b000000000000000000007c0ba6010000ab0100000000000000
-                        00a6020000ab020000000000000000a6010000ab01000000000000000001
-                        007c08a0100000000000000000000000000000000000000000a6000000ab
-                        0000000000000000000100820064007d0b7e0b7701770078035900770123
-                        0031007304770278035900770101005900010001000900640064006400a6
-                        020000ab0200000000000000000100640053002300310073047702780359
-                        007701010059000100010064005300
-                                   0 COPY_FREE_VARS           6
+                        007d05740d00000000000000000000890eac03a6010000ab010000000000
+                        00000035007d077c07a00700000000000000000000000000000000000000
+                        007c0289117c05ac04a6030000ab03000000000000000035007d08020089
+                        0c7c0089107c037c08890f890d7c0564059c067c01a4018e017d09741100
+                        0000000000000000007c096406a6020000ab020000000000000000722874
+                        09000000000000000000007c096a090000000000000000a6010000ab0100
+                        0000000000000072147c09a0090000000000000000000000000000000000
+                        000000a6000000ab000000000000000000010009000200890f7c0069007c
+                        01a4018e01830064007b035600970386047d0a7411000000000000000000
+                        007c096407a6020000ab0200000000000000007229740900000000000000
+                        0000007c096a0a0000000000000000a6010000ab01000000000000000072
+                        157c09a00a00000000000000000000000000000000000000007c0aa60100
+                        00ab01000000000000000001007c08a00b00000000000000000000000000
+                        00000000000000a6000000ab00000000000000000072337c08a00c000000
+                        0000000000000000000000000000000000741a000000000000000000006a
+                        0e0000000000000000a6010000ab01000000000000000001007c08a00f00
+                        00000000000000000000000000000000000000a6000000ab000000000000
+                        00000001007c0a6302640064006400a6020000ab02000000000000000001
+                        006302640064006400a6020000ab02000000000000000001005300230074
+                        2000000000000000000000240072697d0b7c08a011000000000000000000
+                        00000000000000000000007c0ba6010000ab01000000000000000001007c
+                        08a00c000000000000000000000000000000000000000074250000000000
+                        0000000000741a000000000000000000006a130000000000000000742900
+                        0000000000000000007c0ba6010000ab010000000000000000a6020000ab
+                        020000000000000000a6010000ab01000000000000000001007c08a00f00
+                        00000000000000000000000000000000000000a6000000ab000000000000
+                        0000000100820064007d0b7e0b7701770078035900770123003100730477
+                        0278035900770101005900010001000900640064006400a6020000ab0200
+                        000000000000000100640053002300310073047702780359007701010059
+                        000100010064005300
+                                   0 COPY_FREE_VARS           7
                      
-                     327           2 RETURN_GENERATOR
+                     325           2 RETURN_GENERATOR
                                    4 POP_TOP
                                    6 RESUME                   0
                      
-                     329           8 LOAD_GLOBAL              1 (NULL + TracerWrapper)
+                     327           8 LOAD_GLOBAL              1 (NULL + TracerWrapper)
                                   20 LOAD_ATTR                1 (verify_initialized)
                                   30 PRECALL                  0
                                   34 CALL                     0
                                   44 POP_JUMP_FORWARD_IF_TRUE     8 (to 62)
                      
-                     330          46 PUSH_NULL
-                                  48 LOAD_DEREF              14 (fn)
+                     328          46 PUSH_NULL
+                                  48 LOAD_DEREF              15 (fn)
                                   50 LOAD_FAST                0 (args)
                                   52 BUILD_MAP                0
                                   54 LOAD_FAST                1 (kwargs)
                                   56 DICT_MERGE               1
                                   58 CALL_FUNCTION_EX         1
                                   60 RETURN_VALUE
                      
-                     332     >>   62 LOAD_DEREF              12 (SpanCapture)
+                     330     >>   62 LOAD_DEREF              12 (SpanCapture)
                                   64 LOAD_METHOD              2 (get_span_name)
                      
-                     333          86 LOAD_DEREF              15 (name)
+                     331          86 LOAD_DEREF              16 (name)
                      
-                     334          88 LOAD_DEREF              17 (tlp_service_type)
+                     332          88 LOAD_DEREF              18 (tlp_service_type)
                      
-                     335          90 LOAD_DEREF              14 (fn)
+                     333          90 LOAD_DEREF              15 (fn)
                      
-                     332          92 KW_NAMES                 1
+                     330          92 KW_NAMES                 1
                                   94 PRECALL                  3
                                   98 CALL                     3
                                  108 UNPACK_SEQUENCE          2
                                  112 STORE_FAST               2 (span_name)
                                  114 STORE_FAST               3 (service_type)
                      
-                     338         116 LOAD_DEREF              13 (config)
+                     336         116 LOAD_DEREF              13 (config)
                                  118 LOAD_METHOD              3 (get)
                                  140 LOAD_CONST               2 ('context_parser')
                                  142 PRECALL                  1
                                  146 CALL                     1
                                  156 STORE_FAST               4 (context_parser)
                      
-                     339         158 LOAD_CONST               0 (None)
+                     337         158 LOAD_CONST               0 (None)
                                  160 STORE_FAST               5 (context)
                      
-                     340         162 LOAD_FAST                4 (context_parser)
+                     338         162 LOAD_FAST                4 (context_parser)
                                  164 POP_JUMP_FORWARD_IF_NONE    38 (to 242)
                                  166 LOAD_GLOBAL              9 (NULL + callable)
                                  178 LOAD_FAST                4 (context_parser)
                                  180 PRECALL                  1
                                  184 CALL                     1
                                  194 POP_JUMP_FORWARD_IF_FALSE    23 (to 242)
                      
-                     341         196 PUSH_NULL
+                     339         196 PUSH_NULL
                                  198 LOAD_FAST                4 (context_parser)
                                  200 LOAD_FAST                0 (args)
                                  202 BUILD_MAP                0
                                  204 LOAD_FAST                1 (kwargs)
                                  206 DICT_MERGE               1
                                  208 CALL_FUNCTION_EX         1
                                  210 STORE_FAST               6 (carrier)
                      
-                     342         212 LOAD_GLOBAL             11 (NULL + get_trace_context_from_carrier)
+                     340         212 LOAD_GLOBAL             11 (NULL + get_trace_context_from_carrier)
                                  224 LOAD_FAST                6 (carrier)
                                  226 PRECALL                  1
                                  230 CALL                     1
                                  240 STORE_FAST               5 (context)
                      
-                     344     >>  242 LOAD_GLOBAL             13 (NULL + get_tracer)
-                                 254 LOAD_DEREF              12 (SpanCapture)
-                                 256 LOAD_METHOD              7 (is_flush_on_exit)
-                                 278 PRECALL                  0
-                                 282 CALL                     0
-                                 292 KW_NAMES                 3
-                                 294 PRECALL                  1
-                                 298 CALL                     1
-                                 308 BEFORE_WITH
-                                 310 STORE_FAST               7 (tracer)
-                     
-                     345         312 LOAD_FAST                7 (tracer)
-                                 314 LOAD_METHOD              8 (start_as_current_span)
-                                 336 LOAD_FAST                2 (span_name)
-                                 338 LOAD_DEREF              16 (span_kind)
-                                 340 LOAD_FAST                5 (context)
-                                 342 KW_NAMES                 4
-                                 344 PRECALL                  3
-                                 348 CALL                     3
-                                 358 BEFORE_WITH
-                                 360 STORE_FAST               8 (span)
-                     
-                     346         362 PUSH_NULL
-                                 364 LOAD_DEREF              12 (SpanCapture)
-                     
-                     347         366 LOAD_FAST                0 (args)
-                     
-                     348         368 LOAD_DEREF              15 (name)
-                     
-                     349         370 LOAD_FAST                3 (service_type)
-                     
-                     350         372 LOAD_FAST                8 (span)
-                     
-                     351         374 LOAD_DEREF              14 (fn)
-                     
-                     352         376 LOAD_DEREF              13 (config)
-                     
-                     353         378 LOAD_FAST                5 (context)
-                     
-                     346         380 LOAD_CONST               5 (('name', 'service_type', 'span', 'instance', 'config', 'context'))
-                                 382 BUILD_CONST_KEY_MAP      6
-                     
-                     354         384 LOAD_FAST                1 (kwargs)
-                     
-                     346         386 DICT_MERGE               1
-                                 388 CALL_FUNCTION_EX         1
-                                 390 STORE_FAST               9 (span_capture)
-                     
-                     356         392 LOAD_GLOBAL             19 (NULL + hasattr)
-                                 404 LOAD_FAST                9 (span_capture)
-                                 406 LOAD_CONST               6 ('capture_input')
-                                 408 PRECALL                  2
-                                 412 CALL                     2
-                                 422 POP_JUMP_FORWARD_IF_FALSE    40 (to 504)
-                                 424 LOAD_GLOBAL              9 (NULL + callable)
-                                 436 LOAD_FAST                9 (span_capture)
-                                 438 LOAD_ATTR               10 (capture_input)
-                                 448 PRECALL                  1
-                                 452 CALL                     1
-                                 462 POP_JUMP_FORWARD_IF_FALSE    20 (to 504)
-                     
-                     357         464 LOAD_FAST                9 (span_capture)
-                                 466 LOAD_METHOD             10 (capture_input)
-                                 488 PRECALL                  0
-                                 492 CALL                     0
-                                 502 POP_TOP
-                     
-                     359     >>  504 NOP
-                     
-                     360         506 PUSH_NULL
-                                 508 LOAD_DEREF              14 (fn)
-                                 510 LOAD_FAST                0 (args)
-                                 512 BUILD_MAP                0
-                                 514 LOAD_FAST                1 (kwargs)
-                                 516 DICT_MERGE               1
-                                 518 CALL_FUNCTION_EX         1
-                                 520 GET_AWAITABLE            0
-                                 522 LOAD_CONST               0 (None)
-                             >>  524 SEND                     3 (to 532)
-                                 526 YIELD_VALUE
-                                 528 RESUME                   3
-                                 530 JUMP_BACKWARD_NO_INTERRUPT     4 (to 524)
-                             >>  532 STORE_FAST              10 (res)
-                     
-                     362         534 LOAD_GLOBAL             19 (NULL + hasattr)
-                                 546 LOAD_FAST                9 (span_capture)
-                                 548 LOAD_CONST               7 ('capture_output')
-                                 550 PRECALL                  2
-                                 554 CALL                     2
-                                 564 POP_JUMP_FORWARD_IF_FALSE    41 (to 648)
-                                 566 LOAD_GLOBAL              9 (NULL + callable)
-                                 578 LOAD_FAST                9 (span_capture)
-                                 580 LOAD_ATTR               11 (capture_output)
-                                 590 PRECALL                  1
-                                 594 CALL                     1
-                                 604 POP_JUMP_FORWARD_IF_FALSE    21 (to 648)
-                     
-                     363         606 LOAD_FAST                9 (span_capture)
-                                 608 LOAD_METHOD             11 (capture_output)
-                                 630 LOAD_FAST               10 (res)
-                                 632 PRECALL                  1
-                                 636 CALL                     1
-                                 646 POP_TOP
-                     
-                     365     >>  648 LOAD_FAST                8 (span)
-                                 650 LOAD_METHOD             12 (is_recording)
-                                 672 PRECALL                  0
-                                 676 CALL                     0
-                                 686 POP_JUMP_FORWARD_IF_FALSE    51 (to 790)
-                     
-                     366         688 LOAD_FAST                8 (span)
-                                 690 LOAD_METHOD             13 (set_status)
-                                 712 LOAD_GLOBAL             28 (StatusCode)
-                                 724 LOAD_ATTR               15 (OK)
-                                 734 PRECALL                  1
-                                 738 CALL                     1
-                                 748 POP_TOP
-                     
-                     367         750 LOAD_FAST                8 (span)
-                                 752 LOAD_METHOD             16 (end)
-                                 774 PRECALL                  0
-                                 778 CALL                     0
-                                 788 POP_TOP
-                     
-                     369     >>  790 LOAD_FAST               10 (res)
-                     
-                     345         792 SWAP                     2
-                                 794 LOAD_CONST               0 (None)
-                                 796 LOAD_CONST               0 (None)
-                                 798 LOAD_CONST               0 (None)
-                                 800 PRECALL                  2
-                                 804 CALL                     2
-                                 814 POP_TOP
-                     
-                     344         816 SWAP                     2
-                                 818 LOAD_CONST               0 (None)
-                                 820 LOAD_CONST               0 (None)
-                                 822 LOAD_CONST               0 (None)
-                                 824 PRECALL                  2
-                                 828 CALL                     2
-                                 838 POP_TOP
-                                 840 RETURN_VALUE
-                             >>  842 PUSH_EXC_INFO
-                     
-                     371         844 LOAD_GLOBAL             34 (Exception)
-                                 856 CHECK_EXC_MATCH
-                                 858 POP_JUMP_FORWARD_IF_FALSE   105 (to 1070)
-                                 860 STORE_FAST              11 (err)
-                     
-                     373         862 LOAD_FAST                8 (span)
-                                 864 LOAD_METHOD             18 (record_exception)
-                                 886 LOAD_FAST               11 (err)
-                                 888 PRECALL                  1
-                                 892 CALL                     1
-                                 902 POP_TOP
-                     
-                     376         904 LOAD_FAST                8 (span)
-                                 906 LOAD_METHOD             13 (set_status)
-                                 928 LOAD_GLOBAL             39 (NULL + Status)
-                                 940 LOAD_GLOBAL             28 (StatusCode)
-                                 952 LOAD_ATTR               20 (ERROR)
-                                 962 LOAD_GLOBAL             43 (NULL + str)
-                                 974 LOAD_FAST               11 (err)
-                                 976 PRECALL                  1
-                                 980 CALL                     1
-                                 990 PRECALL                  2
-                                 994 CALL                     2
-                                1004 PRECALL                  1
-                                1008 CALL                     1
-                                1018 POP_TOP
-                     
-                     379        1020 LOAD_FAST                8 (span)
-                                1022 LOAD_METHOD             16 (end)
-                                1044 PRECALL                  0
-                                1048 CALL                     0
-                                1058 POP_TOP
-                     
-                     380        1060 RAISE_VARARGS            0
-                             >> 1062 LOAD_CONST               0 (None)
-                                1064 STORE_FAST              11 (err)
-                                1066 DELETE_FAST             11 (err)
-                                1068 RERAISE                  1
-                     
-                     371     >> 1070 RERAISE                  0
-                             >> 1072 COPY                     3
-                                1074 POP_EXCEPT
-                                1076 RERAISE                  1
-                     
-                     345     >> 1078 PUSH_EXC_INFO
-                                1080 WITH_EXCEPT_START
-                                1082 POP_JUMP_FORWARD_IF_TRUE     4 (to 1092)
-                                1084 RERAISE                  2
-                             >> 1086 COPY                     3
-                                1088 POP_EXCEPT
-                                1090 RERAISE                  1
-                             >> 1092 POP_TOP
-                                1094 POP_EXCEPT
-                                1096 POP_TOP
-                                1098 POP_TOP
-                                1100 NOP
-                     
-                     344        1102 LOAD_CONST               0 (None)
-                                1104 LOAD_CONST               0 (None)
-                                1106 LOAD_CONST               0 (None)
-                                1108 PRECALL                  2
-                                1112 CALL                     2
-                                1122 POP_TOP
-                                1124 LOAD_CONST               0 (None)
-                                1126 RETURN_VALUE
-                             >> 1128 PUSH_EXC_INFO
-                                1130 WITH_EXCEPT_START
-                                1132 POP_JUMP_FORWARD_IF_TRUE     4 (to 1142)
-                                1134 RERAISE                  2
-                             >> 1136 COPY                     3
-                                1138 POP_EXCEPT
-                                1140 RERAISE                  1
-                             >> 1142 POP_TOP
-                                1144 POP_EXCEPT
-                                1146 POP_TOP
-                                1148 POP_TOP
-                                1150 LOAD_CONST               0 (None)
-                                1152 RETURN_VALUE
+                     342     >>  242 LOAD_GLOBAL             13 (NULL + get_tracer)
+                                 254 LOAD_DEREF              14 (flush_on_exit)
+                                 256 KW_NAMES                 3
+                                 258 PRECALL                  1
+                                 262 CALL                     1
+                                 272 BEFORE_WITH
+                                 274 STORE_FAST               7 (tracer)
+                     
+                     343         276 LOAD_FAST                7 (tracer)
+                                 278 LOAD_METHOD              7 (start_as_current_span)
+                                 300 LOAD_FAST                2 (span_name)
+                                 302 LOAD_DEREF              17 (span_kind)
+                                 304 LOAD_FAST                5 (context)
+                                 306 KW_NAMES                 4
+                                 308 PRECALL                  3
+                                 312 CALL                     3
+                                 322 BEFORE_WITH
+                                 324 STORE_FAST               8 (span)
+                     
+                     344         326 PUSH_NULL
+                                 328 LOAD_DEREF              12 (SpanCapture)
+                     
+                     345         330 LOAD_FAST                0 (args)
+                     
+                     346         332 LOAD_DEREF              16 (name)
+                     
+                     347         334 LOAD_FAST                3 (service_type)
+                     
+                     348         336 LOAD_FAST                8 (span)
+                     
+                     349         338 LOAD_DEREF              15 (fn)
+                     
+                     350         340 LOAD_DEREF              13 (config)
+                     
+                     351         342 LOAD_FAST                5 (context)
+                     
+                     344         344 LOAD_CONST               5 (('name', 'service_type', 'span', 'instance', 'config', 'context'))
+                                 346 BUILD_CONST_KEY_MAP      6
+                     
+                     352         348 LOAD_FAST                1 (kwargs)
+                     
+                     344         350 DICT_MERGE               1
+                                 352 CALL_FUNCTION_EX         1
+                                 354 STORE_FAST               9 (span_capture)
+                     
+                     354         356 LOAD_GLOBAL             17 (NULL + hasattr)
+                                 368 LOAD_FAST                9 (span_capture)
+                                 370 LOAD_CONST               6 ('capture_input')
+                                 372 PRECALL                  2
+                                 376 CALL                     2
+                                 386 POP_JUMP_FORWARD_IF_FALSE    40 (to 468)
+                                 388 LOAD_GLOBAL              9 (NULL + callable)
+                                 400 LOAD_FAST                9 (span_capture)
+                                 402 LOAD_ATTR                9 (capture_input)
+                                 412 PRECALL                  1
+                                 416 CALL                     1
+                                 426 POP_JUMP_FORWARD_IF_FALSE    20 (to 468)
+                     
+                     355         428 LOAD_FAST                9 (span_capture)
+                                 430 LOAD_METHOD              9 (capture_input)
+                                 452 PRECALL                  0
+                                 456 CALL                     0
+                                 466 POP_TOP
+                     
+                     357     >>  468 NOP
+                     
+                     358         470 PUSH_NULL
+                                 472 LOAD_DEREF              15 (fn)
+                                 474 LOAD_FAST                0 (args)
+                                 476 BUILD_MAP                0
+                                 478 LOAD_FAST                1 (kwargs)
+                                 480 DICT_MERGE               1
+                                 482 CALL_FUNCTION_EX         1
+                                 484 GET_AWAITABLE            0
+                                 486 LOAD_CONST               0 (None)
+                             >>  488 SEND                     3 (to 496)
+                                 490 YIELD_VALUE
+                                 492 RESUME                   3
+                                 494 JUMP_BACKWARD_NO_INTERRUPT     4 (to 488)
+                             >>  496 STORE_FAST              10 (res)
+                     
+                     360         498 LOAD_GLOBAL             17 (NULL + hasattr)
+                                 510 LOAD_FAST                9 (span_capture)
+                                 512 LOAD_CONST               7 ('capture_output')
+                                 514 PRECALL                  2
+                                 518 CALL                     2
+                                 528 POP_JUMP_FORWARD_IF_FALSE    41 (to 612)
+                                 530 LOAD_GLOBAL              9 (NULL + callable)
+                                 542 LOAD_FAST                9 (span_capture)
+                                 544 LOAD_ATTR               10 (capture_output)
+                                 554 PRECALL                  1
+                                 558 CALL                     1
+                                 568 POP_JUMP_FORWARD_IF_FALSE    21 (to 612)
+                     
+                     361         570 LOAD_FAST                9 (span_capture)
+                                 572 LOAD_METHOD             10 (capture_output)
+                                 594 LOAD_FAST               10 (res)
+                                 596 PRECALL                  1
+                                 600 CALL                     1
+                                 610 POP_TOP
+                     
+                     363     >>  612 LOAD_FAST                8 (span)
+                                 614 LOAD_METHOD             11 (is_recording)
+                                 636 PRECALL                  0
+                                 640 CALL                     0
+                                 650 POP_JUMP_FORWARD_IF_FALSE    51 (to 754)
+                     
+                     364         652 LOAD_FAST                8 (span)
+                                 654 LOAD_METHOD             12 (set_status)
+                                 676 LOAD_GLOBAL             26 (StatusCode)
+                                 688 LOAD_ATTR               14 (OK)
+                                 698 PRECALL                  1
+                                 702 CALL                     1
+                                 712 POP_TOP
+                     
+                     365         714 LOAD_FAST                8 (span)
+                                 716 LOAD_METHOD             15 (end)
+                                 738 PRECALL                  0
+                                 742 CALL                     0
+                                 752 POP_TOP
+                     
+                     367     >>  754 LOAD_FAST               10 (res)
+                     
+                     343         756 SWAP                     2
+                                 758 LOAD_CONST               0 (None)
+                                 760 LOAD_CONST               0 (None)
+                                 762 LOAD_CONST               0 (None)
+                                 764 PRECALL                  2
+                                 768 CALL                     2
+                                 778 POP_TOP
+                     
+                     342         780 SWAP                     2
+                                 782 LOAD_CONST               0 (None)
+                                 784 LOAD_CONST               0 (None)
+                                 786 LOAD_CONST               0 (None)
+                                 788 PRECALL                  2
+                                 792 CALL                     2
+                                 802 POP_TOP
+                                 804 RETURN_VALUE
+                             >>  806 PUSH_EXC_INFO
+                     
+                     369         808 LOAD_GLOBAL             32 (Exception)
+                                 820 CHECK_EXC_MATCH
+                                 822 POP_JUMP_FORWARD_IF_FALSE   105 (to 1034)
+                                 824 STORE_FAST              11 (err)
+                     
+                     371         826 LOAD_FAST                8 (span)
+                                 828 LOAD_METHOD             17 (record_exception)
+                                 850 LOAD_FAST               11 (err)
+                                 852 PRECALL                  1
+                                 856 CALL                     1
+                                 866 POP_TOP
+                     
+                     374         868 LOAD_FAST                8 (span)
+                                 870 LOAD_METHOD             12 (set_status)
+                                 892 LOAD_GLOBAL             37 (NULL + Status)
+                                 904 LOAD_GLOBAL             26 (StatusCode)
+                                 916 LOAD_ATTR               19 (ERROR)
+                                 926 LOAD_GLOBAL             41 (NULL + str)
+                                 938 LOAD_FAST               11 (err)
+                                 940 PRECALL                  1
+                                 944 CALL                     1
+                                 954 PRECALL                  2
+                                 958 CALL                     2
+                                 968 PRECALL                  1
+                                 972 CALL                     1
+                                 982 POP_TOP
+                     
+                     377         984 LOAD_FAST                8 (span)
+                                 986 LOAD_METHOD             15 (end)
+                                1008 PRECALL                  0
+                                1012 CALL                     0
+                                1022 POP_TOP
+                     
+                     378        1024 RAISE_VARARGS            0
+                             >> 1026 LOAD_CONST               0 (None)
+                                1028 STORE_FAST              11 (err)
+                                1030 DELETE_FAST             11 (err)
+                                1032 RERAISE                  1
+                     
+                     369     >> 1034 RERAISE                  0
+                             >> 1036 COPY                     3
+                                1038 POP_EXCEPT
+                                1040 RERAISE                  1
+                     
+                     343     >> 1042 PUSH_EXC_INFO
+                                1044 WITH_EXCEPT_START
+                                1046 POP_JUMP_FORWARD_IF_TRUE     4 (to 1056)
+                                1048 RERAISE                  2
+                             >> 1050 COPY                     3
+                                1052 POP_EXCEPT
+                                1054 RERAISE                  1
+                             >> 1056 POP_TOP
+                                1058 POP_EXCEPT
+                                1060 POP_TOP
+                                1062 POP_TOP
+                                1064 NOP
+                     
+                     342        1066 LOAD_CONST               0 (None)
+                                1068 LOAD_CONST               0 (None)
+                                1070 LOAD_CONST               0 (None)
+                                1072 PRECALL                  2
+                                1076 CALL                     2
+                                1086 POP_TOP
+                                1088 LOAD_CONST               0 (None)
+                                1090 RETURN_VALUE
+                             >> 1092 PUSH_EXC_INFO
+                                1094 WITH_EXCEPT_START
+                                1096 POP_JUMP_FORWARD_IF_TRUE     4 (to 1106)
+                                1098 RERAISE                  2
+                             >> 1100 COPY                     3
+                                1102 POP_EXCEPT
+                                1104 RERAISE                  1
+                             >> 1106 POP_TOP
+                                1108 POP_EXCEPT
+                                1110 POP_TOP
+                                1112 POP_TOP
+                                1114 LOAD_CONST               0 (None)
+                                1116 RETURN_VALUE
                      ExceptionTable:
-                       310 to 358 -> 1128 [1] lasti
-                       360 to 502 -> 1078 [2] lasti
-                       506 to 790 -> 842 [2]
-                       792 to 814 -> 1128 [1] lasti
-                       842 to 860 -> 1072 [3] lasti
-                       862 to 1060 -> 1062 [3] lasti
-                       1062 to 1070 -> 1072 [3] lasti
-                       1072 to 1076 -> 1078 [2] lasti
-                       1078 to 1084 -> 1086 [4] lasti
-                       1086 to 1090 -> 1128 [1] lasti
-                       1092 to 1092 -> 1086 [4] lasti
-                       1094 to 1098 -> 1128 [1] lasti
-                       1128 to 1134 -> 1136 [3] lasti
-                       1142 to 1142 -> 1136 [3] lasti
+                       274 to 322 -> 1092 [1] lasti
+                       324 to 466 -> 1042 [2] lasti
+                       470 to 754 -> 806 [2]
+                       756 to 778 -> 1092 [1] lasti
+                       806 to 824 -> 1036 [3] lasti
+                       826 to 1024 -> 1026 [3] lasti
+                       1026 to 1034 -> 1036 [3] lasti
+                       1036 to 1040 -> 1042 [2] lasti
+                       1042 to 1048 -> 1050 [4] lasti
+                       1050 to 1054 -> 1092 [1] lasti
+                       1056 to 1056 -> 1050 [4] lasti
+                       1058 to 1062 -> 1092 [1] lasti
+                       1092 to 1098 -> 1100 [3] lasti
+                       1106 to 1106 -> 1100 [3] lasti
                      consts
                         None
                         ('name', 'tlp_service_type', 'instance')
                         'context_parser'
                         ('flush_on_exit',)
                         ('kind', 'context')
                         ('name', 'service_type', 'span', 'instance', 'config', 'context')
                         'capture_input'
                         'capture_output'
-                     names      ('TracerWrapper', 'verify_initialized', 'get_span_name', 'get', 'callable', 'get_trace_context_from_carrier', 'get_tracer', 'is_flush_on_exit', 'start_as_current_span', 'hasattr', 'capture_input', 'capture_output', 'is_recording', 'set_status', 'StatusCode', 'OK', 'end', 'Exception', 'record_exception', 'Status', 'ERROR', 'str')
+                     names      ('TracerWrapper', 'verify_initialized', 'get_span_name', 'get', 'callable', 'get_trace_context_from_carrier', 'get_tracer', 'start_as_current_span', 'hasattr', 'capture_input', 'capture_output', 'is_recording', 'set_status', 'StatusCode', 'OK', 'end', 'Exception', 'record_exception', 'Status', 'ERROR', 'str')
                      varnames   ('args', 'kwargs', 'span_name', 'service_type', 'context_parser', 'context', 'carrier', 'tracer', 'span', 'span_capture', 'res', 'err')
-                     freevars   ('SpanCapture', 'config', 'fn', 'name', 'span_kind', 'tlp_service_type')
+                     freevars   ('SpanCapture', 'config', 'flush_on_exit', 'fn', 'name', 'span_kind', 'tlp_service_type')
                      cellvars   ()
                      filename   '/Users/vuongngo/workspace/agiflow/packages/python/agiflow-sdk/agiflow/opentelemetry/trace_decorators/wrapper.py'
                      name       'wrap'
-                     firstlineno 327
+                     firstlineno 325
                      lnotab
-                        0x08022601100218010201020102fd18062a010401220110011e02460132
+                        0x08022601100218010201020102fd18062a010401220110011e02220132
                         01040102010201020102010201020102f9040802f8060a4801280202011c
                         0248012a0228013e01280202e818ff1c1b12022a03740328010af708e618
                         ff
                names      ('wraps',)
                varnames   ('fn', 'wrap')
-               freevars   ('SpanCapture', 'config', 'name', 'span_kind', 'tlp_service_type')
+               freevars   ('SpanCapture', 'config', 'flush_on_exit', 'name', 'span_kind', 'tlp_service_type')
                cellvars   ('fn',)
                filename   '/Users/vuongngo/workspace/agiflow/packages/python/agiflow-sdk/agiflow/opentelemetry/trace_decorators/wrapper.py'
                name       'decorate'
-               firstlineno 326
-               lnotab 0x06011c0112ff0e010236
+               firstlineno 324
+               lnotab 0x06011c0114ff0e010236
          names      ()
-         varnames   ('name', 'tlp_service_type', 'span_kind', 'SpanCapture', 'config', 'decorate')
+         varnames   ('name', 'tlp_service_type', 'span_kind', 'SpanCapture', 'flush_on_exit', 'config', 'decorate')
          freevars   ()
-         cellvars   ('name', 'tlp_service_type', 'span_kind', 'SpanCapture', 'config')
+         cellvars   ('name', 'tlp_service_type', 'span_kind', 'SpanCapture', 'flush_on_exit', 'config')
          filename   '/Users/vuongngo/workspace/agiflow/packages/python/agiflow-sdk/agiflow/opentelemetry/trace_decorators/wrapper.py'
          name       'adecorate_method'
-         firstlineno 319
-         lnotab 0x0c07123a
+         firstlineno 316
+         lnotab 0x0e08143a
       'method_name'
       'kwargs'
       code
-         argcount  : 5
-         nlocals   : 7
-         stacksize : 6
+         argcount  : 6
+         nlocals   : 8
+         stacksize : 7
          flags     : 11
          code
-            0x8700870187028703870487059700880488058801880088038802660664
-            0184087d067c065300
+            0x8700870187028703870487058706970088048805880688018800880388
+            026607640184087d077c075300
                        0 MAKE_CELL                0 (name)
                        2 MAKE_CELL                1 (method_name)
                        4 MAKE_CELL                2 (tlp_service_type)
                        6 MAKE_CELL                3 (span_kind)
                        8 MAKE_CELL                4 (SpanCapture)
-                      10 MAKE_CELL                5 (kwargs)
+                      10 MAKE_CELL                5 (flush_on_exit)
+                      12 MAKE_CELL                6 (kwargs)
          
-         387          12 RESUME                   0
+         385          14 RESUME                   0
          
-         395          14 LOAD_CLOSURE             4 (SpanCapture)
-                      16 LOAD_CLOSURE             5 (kwargs)
-                      18 LOAD_CLOSURE             1 (method_name)
-                      20 LOAD_CLOSURE             0 (name)
-                      22 LOAD_CLOSURE             3 (span_kind)
-                      24 LOAD_CLOSURE             2 (tlp_service_type)
-                      26 BUILD_TUPLE              6
-                      28 LOAD_CONST               1 (<code object decorator, file "/Users/vuongngo/workspace/agiflow/packages/python/agiflow-sdk/agiflow/opentelemetry/trace_decorators/wrapper.py", line 395>)
-                      30 MAKE_FUNCTION            8 (closure)
-                      32 STORE_FAST               6 (decorator)
+         394          16 LOAD_CLOSURE             4 (SpanCapture)
+                      18 LOAD_CLOSURE             5 (flush_on_exit)
+                      20 LOAD_CLOSURE             6 (kwargs)
+                      22 LOAD_CLOSURE             1 (method_name)
+                      24 LOAD_CLOSURE             0 (name)
+                      26 LOAD_CLOSURE             3 (span_kind)
+                      28 LOAD_CLOSURE             2 (tlp_service_type)
+                      30 BUILD_TUPLE              7
+                      32 LOAD_CONST               1 (<code object decorator, file "/Users/vuongngo/workspace/agiflow/packages/python/agiflow-sdk/agiflow/opentelemetry/trace_decorators/wrapper.py", line 394>)
+                      34 MAKE_FUNCTION            8 (closure)
+                      36 STORE_FAST               7 (decorator)
          
-         411          34 LOAD_FAST                6 (decorator)
-                      36 RETURN_VALUE
+         411          38 LOAD_FAST                7 (decorator)
+                      40 RETURN_VALUE
          consts
             None
             code
                argcount  : 1
                nlocals   : 3
-               stacksize : 13
+               stacksize : 14
                flags     : 19
                code
-                  0x950697008906720289066e137401000000000000000000007c006a0100
+                  0x950797008907720289076e137401000000000000000000007c006a0100
                   00000000000000a6010000ab0100000000000000007d0174050000000000
-                  00000000007c008905a6020000ab0200000000000000007d027407000000
-                  000000000000007c008905020074090000000000000000000064027c0189
-                  088907890364019c048904a4018e017c02a6010000ab0100000000000000
-                  00a6030000ab03000000000000000001007c005300
-                             0 COPY_FREE_VARS           6
+                  00000000007c008906a6020000ab0200000000000000007d027407000000
+                  000000000000007c008906020074090000000000000000000064027c0189
+                  0989088903890464019c058905a4018e017c02a6010000ab010000000000
+                  000000a6030000ab03000000000000000001007c005300
+                             0 COPY_FREE_VARS           7
                
-               395           2 RESUME                   0
+               394           2 RESUME                   0
                
-               396           4 LOAD_DEREF               6 (name)
+               395           4 LOAD_DEREF               7 (name)
                              6 POP_JUMP_FORWARD_IF_FALSE     2 (to 12)
-                             8 LOAD_DEREF               6 (name)
+                             8 LOAD_DEREF               7 (name)
                             10 JUMP_FORWARD            19 (to 50)
                        >>   12 LOAD_GLOBAL              1 (NULL + camel_to_snake)
                             24 LOAD_FAST                0 (cls)
                             26 LOAD_ATTR                1 (__name__)
                             36 PRECALL                  1
                             40 CALL                     1
                        >>   50 STORE_FAST               1 (task_name)
                
-               397          52 LOAD_GLOBAL              5 (NULL + getattr)
+               396          52 LOAD_GLOBAL              5 (NULL + getattr)
                             64 LOAD_FAST                0 (cls)
-                            66 LOAD_DEREF               5 (method_name)
+                            66 LOAD_DEREF               6 (method_name)
                             68 PRECALL                  2
                             72 CALL                     2
                             82 STORE_FAST               2 (method)
                
-               398          84 LOAD_GLOBAL              7 (NULL + setattr)
+               397          84 LOAD_GLOBAL              7 (NULL + setattr)
                
-               399          96 LOAD_FAST                0 (cls)
+               398          96 LOAD_FAST                0 (cls)
                
-               400          98 LOAD_DEREF               5 (method_name)
+               399          98 LOAD_DEREF               6 (method_name)
                
-               401         100 PUSH_NULL
+               400         100 PUSH_NULL
                            102 LOAD_GLOBAL              9 (NULL + decorate_method)
                            114 LOAD_CONST               2 (())
                
-               402         116 LOAD_FAST                1 (task_name)
+               401         116 LOAD_FAST                1 (task_name)
                
-               403         118 LOAD_DEREF               8 (tlp_service_type)
+               402         118 LOAD_DEREF               9 (tlp_service_type)
                
-               404         120 LOAD_DEREF               7 (span_kind)
+               403         120 LOAD_DEREF               8 (span_kind)
                
-               405         122 LOAD_DEREF               3 (SpanCapture)
+               404         122 LOAD_DEREF               3 (SpanCapture)
                
-               401         124 LOAD_CONST               1 (('name', 'tlp_service_type', 'span_kind', 'SpanCapture'))
-                           126 BUILD_CONST_KEY_MAP      4
+               405         124 LOAD_DEREF               4 (flush_on_exit)
                
-               406         128 LOAD_DEREF               4 (kwargs)
+               400         126 LOAD_CONST               1 (('name', 'tlp_service_type', 'span_kind', 'SpanCapture', 'flush_on_exit'))
+                           128 BUILD_CONST_KEY_MAP      5
                
-               401         130 DICT_MERGE               1
-                           132 CALL_FUNCTION_EX         1
+               406         130 LOAD_DEREF               5 (kwargs)
                
-               407         134 LOAD_FAST                2 (method)
+               400         132 DICT_MERGE               1
+                           134 CALL_FUNCTION_EX         1
                
-               401         136 PRECALL                  1
-                           140 CALL                     1
+               407         136 LOAD_FAST                2 (method)
                
-               398         150 PRECALL                  3
-                           154 CALL                     3
-                           164 POP_TOP
+               400         138 PRECALL                  1
+                           142 CALL                     1
                
-               409         166 LOAD_FAST                0 (cls)
-                           168 RETURN_VALUE
+               397         152 PRECALL                  3
+                           156 CALL                     3
+                           166 POP_TOP
+               
+               409         168 LOAD_FAST                0 (cls)
+                           170 RETURN_VALUE
                consts
                   None
-                  ('name', 'tlp_service_type', 'span_kind', 'SpanCapture')
+                  ('name', 'tlp_service_type', 'span_kind', 'SpanCapture', 'flush_on_exit')
                   ()
                names      ('camel_to_snake', '__name__', 'getattr', 'setattr', 'decorate_method')
                varnames   ('cls', 'task_name', 'method')
-               freevars   ('SpanCapture', 'kwargs', 'method_name', 'name', 'span_kind', 'tlp_service_type')
+               freevars   ('SpanCapture', 'flush_on_exit', 'kwargs', 'method_name', 'name', 'span_kind', 'tlp_service_type')
                cellvars   ()
                filename   '/Users/vuongngo/workspace/agiflow/packages/python/agiflow-sdk/agiflow/opentelemetry/trace_decorators/wrapper.py'
                name       'decorator'
-               firstlineno 395
+               firstlineno 394
                lnotab
-                  0x0401300120010c0102010201100102010201020102fc040502fb040602
-                  fa0efd100b
+                  0x0401300120010c01020102011001020102010201020102fb040602fa04
+                  0702f90efd100c
          names      ()
-         varnames   ('name', 'method_name', 'tlp_service_type', 'span_kind', 'SpanCapture', 'kwargs', 'decorator')
+         varnames   ('name', 'method_name', 'tlp_service_type', 'span_kind', 'SpanCapture', 'flush_on_exit', 'kwargs', 'decorator')
          freevars   ()
-         cellvars   ('name', 'method_name', 'tlp_service_type', 'span_kind', 'SpanCapture', 'kwargs')
+         cellvars   ('name', 'method_name', 'tlp_service_type', 'span_kind', 'SpanCapture', 'flush_on_exit', 'kwargs')
          filename   '/Users/vuongngo/workspace/agiflow/packages/python/agiflow-sdk/agiflow/opentelemetry/trace_decorators/wrapper.py'
          name       'decorate_class_method'
-         firstlineno 387
-         lnotab 0x0e081410
+         firstlineno 385
+         lnotab 0x10091611
       code
-         argcount  : 5
-         nlocals   : 7
-         stacksize : 6
+         argcount  : 6
+         nlocals   : 8
+         stacksize : 7
          flags     : 11
          code
-            0x8700870187028703870487059700880488058801880088038802660664
-            0184087d067c065300
+            0x8700870187028703870487058706970088048805880688018800880388
+            026607640184087d077c075300
                        0 MAKE_CELL                0 (name)
                        2 MAKE_CELL                1 (method_name)
                        4 MAKE_CELL                2 (tlp_service_type)
                        6 MAKE_CELL                3 (span_kind)
                        8 MAKE_CELL                4 (SpanCapture)
-                      10 MAKE_CELL                5 (kwargs)
+                      10 MAKE_CELL                5 (flush_on_exit)
+                      12 MAKE_CELL                6 (kwargs)
          
-         414          12 RESUME                   0
+         414          14 RESUME                   0
          
-         422          14 LOAD_CLOSURE             4 (SpanCapture)
-                      16 LOAD_CLOSURE             5 (kwargs)
-                      18 LOAD_CLOSURE             1 (method_name)
-                      20 LOAD_CLOSURE             0 (name)
-                      22 LOAD_CLOSURE             3 (span_kind)
-                      24 LOAD_CLOSURE             2 (tlp_service_type)
-                      26 BUILD_TUPLE              6
-                      28 LOAD_CONST               1 (<code object decorator, file "/Users/vuongngo/workspace/agiflow/packages/python/agiflow-sdk/agiflow/opentelemetry/trace_decorators/wrapper.py", line 422>)
-                      30 MAKE_FUNCTION            8 (closure)
-                      32 STORE_FAST               6 (decorator)
+         423          16 LOAD_CLOSURE             4 (SpanCapture)
+                      18 LOAD_CLOSURE             5 (flush_on_exit)
+                      20 LOAD_CLOSURE             6 (kwargs)
+                      22 LOAD_CLOSURE             1 (method_name)
+                      24 LOAD_CLOSURE             0 (name)
+                      26 LOAD_CLOSURE             3 (span_kind)
+                      28 LOAD_CLOSURE             2 (tlp_service_type)
+                      30 BUILD_TUPLE              7
+                      32 LOAD_CONST               1 (<code object decorator, file "/Users/vuongngo/workspace/agiflow/packages/python/agiflow-sdk/agiflow/opentelemetry/trace_decorators/wrapper.py", line 423>)
+                      34 MAKE_FUNCTION            8 (closure)
+                      36 STORE_FAST               7 (decorator)
          
-         438          34 LOAD_FAST                6 (decorator)
-                      36 RETURN_VALUE
+         440          38 LOAD_FAST                7 (decorator)
+                      40 RETURN_VALUE
          consts
             None
             code
                argcount  : 1
                nlocals   : 3
-               stacksize : 13
+               stacksize : 14
                flags     : 19
                code
-                  0x950697008906720289066e137401000000000000000000007c006a0100
+                  0x950797008907720289076e137401000000000000000000007c006a0100
                   00000000000000a6010000ab0100000000000000007d0174050000000000
-                  00000000007c008905a6020000ab0200000000000000007d027407000000
-                  000000000000007c008905020074090000000000000000000064027c0189
-                  088907890364019c048904a4018e017c02a6010000ab0100000000000000
-                  00a6030000ab03000000000000000001007c005300
-                             0 COPY_FREE_VARS           6
+                  00000000007c008906a6020000ab0200000000000000007d027407000000
+                  000000000000007c008906020074090000000000000000000064027c0189
+                  0989088903890464019c058905a4018e017c02a6010000ab010000000000
+                  000000a6030000ab03000000000000000001007c005300
+                             0 COPY_FREE_VARS           7
                
-               422           2 RESUME                   0
+               423           2 RESUME                   0
                
-               423           4 LOAD_DEREF               6 (name)
+               424           4 LOAD_DEREF               7 (name)
                              6 POP_JUMP_FORWARD_IF_FALSE     2 (to 12)
-                             8 LOAD_DEREF               6 (name)
+                             8 LOAD_DEREF               7 (name)
                             10 JUMP_FORWARD            19 (to 50)
                        >>   12 LOAD_GLOBAL              1 (NULL + camel_to_snake)
                             24 LOAD_FAST                0 (cls)
                             26 LOAD_ATTR                1 (__name__)
                             36 PRECALL                  1
                             40 CALL                     1
                        >>   50 STORE_FAST               1 (task_name)
                
-               424          52 LOAD_GLOBAL              5 (NULL + getattr)
+               425          52 LOAD_GLOBAL              5 (NULL + getattr)
                             64 LOAD_FAST                0 (cls)
-                            66 LOAD_DEREF               5 (method_name)
+                            66 LOAD_DEREF               6 (method_name)
                             68 PRECALL                  2
                             72 CALL                     2
                             82 STORE_FAST               2 (method)
                
-               425          84 LOAD_GLOBAL              7 (NULL + setattr)
+               426          84 LOAD_GLOBAL              7 (NULL + setattr)
                
-               426          96 LOAD_FAST                0 (cls)
+               427          96 LOAD_FAST                0 (cls)
                
-               427          98 LOAD_DEREF               5 (method_name)
+               428          98 LOAD_DEREF               6 (method_name)
                
-               428         100 PUSH_NULL
+               429         100 PUSH_NULL
                            102 LOAD_GLOBAL              9 (NULL + adecorate_method)
                            114 LOAD_CONST               2 (())
                
-               429         116 LOAD_FAST                1 (task_name)
+               430         116 LOAD_FAST                1 (task_name)
+               
+               431         118 LOAD_DEREF               9 (tlp_service_type)
                
-               430         118 LOAD_DEREF               8 (tlp_service_type)
+               432         120 LOAD_DEREF               8 (span_kind)
                
-               431         120 LOAD_DEREF               7 (span_kind)
+               433         122 LOAD_DEREF               3 (SpanCapture)
                
-               432         122 LOAD_DEREF               3 (SpanCapture)
+               434         124 LOAD_DEREF               4 (flush_on_exit)
                
-               428         124 LOAD_CONST               1 (('name', 'tlp_service_type', 'span_kind', 'SpanCapture'))
-                           126 BUILD_CONST_KEY_MAP      4
+               429         126 LOAD_CONST               1 (('name', 'tlp_service_type', 'span_kind', 'SpanCapture', 'flush_on_exit'))
+                           128 BUILD_CONST_KEY_MAP      5
                
-               433         128 LOAD_DEREF               4 (kwargs)
+               435         130 LOAD_DEREF               5 (kwargs)
                
-               428         130 DICT_MERGE               1
-                           132 CALL_FUNCTION_EX         1
+               429         132 DICT_MERGE               1
+                           134 CALL_FUNCTION_EX         1
                
-               434         134 LOAD_FAST                2 (method)
+               436         136 LOAD_FAST                2 (method)
                
-               428         136 PRECALL                  1
-                           140 CALL                     1
+               429         138 PRECALL                  1
+                           142 CALL                     1
                
-               425         150 PRECALL                  3
-                           154 CALL                     3
-                           164 POP_TOP
+               426         152 PRECALL                  3
+                           156 CALL                     3
+                           166 POP_TOP
                
-               436         166 LOAD_FAST                0 (cls)
-                           168 RETURN_VALUE
+               438         168 LOAD_FAST                0 (cls)
+                           170 RETURN_VALUE
                consts
                   None
-                  ('name', 'tlp_service_type', 'span_kind', 'SpanCapture')
+                  ('name', 'tlp_service_type', 'span_kind', 'SpanCapture', 'flush_on_exit')
                   ()
                names      ('camel_to_snake', '__name__', 'getattr', 'setattr', 'adecorate_method')
                varnames   ('cls', 'task_name', 'method')
-               freevars   ('SpanCapture', 'kwargs', 'method_name', 'name', 'span_kind', 'tlp_service_type')
+               freevars   ('SpanCapture', 'flush_on_exit', 'kwargs', 'method_name', 'name', 'span_kind', 'tlp_service_type')
                cellvars   ()
                filename   '/Users/vuongngo/workspace/agiflow/packages/python/agiflow-sdk/agiflow/opentelemetry/trace_decorators/wrapper.py'
                name       'decorator'
-               firstlineno 422
+               firstlineno 423
                lnotab
-                  0x0401300120010c0102010201100102010201020102fc040502fb040602
-                  fa0efd100b
+                  0x0401300120010c01020102011001020102010201020102fb040602fa04
+                  0702f90efd100c
          names      ()
-         varnames   ('name', 'method_name', 'tlp_service_type', 'span_kind', 'SpanCapture', 'kwargs', 'decorator')
+         varnames   ('name', 'method_name', 'tlp_service_type', 'span_kind', 'SpanCapture', 'flush_on_exit', 'kwargs', 'decorator')
          freevars   ()
-         cellvars   ('name', 'method_name', 'tlp_service_type', 'span_kind', 'SpanCapture', 'kwargs')
+         cellvars   ('name', 'method_name', 'tlp_service_type', 'span_kind', 'SpanCapture', 'flush_on_exit', 'kwargs')
          filename   '/Users/vuongngo/workspace/agiflow/packages/python/agiflow-sdk/agiflow/opentelemetry/trace_decorators/wrapper.py'
          name       'adecorate_class_method'
          firstlineno 414
-         lnotab 0x0e081410
+         lnotab 0x10091611
    names      ('abc', 'ABC', 'functools', 'wraps', 'logging', 'typing', 'Any', 'Dict', 'Optional', 'TypeVar', 'Generic', 'Unpack', 'agiflow.opentelemetry.context.span_from_context', 'set_workflow_name_from_context', 'agiflow.opentelemetry.convention', 'SpanAttributes', 'agiflow.opentelemetry.convention.agiflow_attributes', 'AgiflowSpanAttributes', 'agiflow.opentelemetry.convention.constants', 'AgiflowServiceTypes', 'opentelemetry.trace', 'Span', 'SpanKind', 'Status', 'StatusCode', 'agiflow.opentelemetry.instrumentation.constants.common', 'AGIFLOW_ADDITIONAL_SPAN_ATTRIBUTES_KEY', 'opentelemetry', 'baggage', 'agiflow.version', '__version__', 'agiflow.opentelemetry.trace_decorators.helper', 'SharedKwargsWithHooks', 'agiflow.opentelemetry.tracing', 'get_tracer', 'TracerWrapper', 'agiflow.opentelemetry.utils', 'should_send_prompts', 'agiflow.opentelemetry.context', 'get_trace_context_from_carrier', 'set_association_properties', 'set_prompt_settings_context', 'set_prompt_attributes_from_context', 'set_workflow_name', 'set_override_enable_context_tracing', 'ContextKeys', 'agiflow.utils', 'serialise_to_json', 'camel_to_snake', 'R', 'getLogger', '__name__', 'logger', 'AbstractSpanCapture', 'BaseSpanCapture', 'TASK', 'INTERNAL', 'str', 'decorate_method', 'adecorate_method', 'decorate_class_method', 'adecorate_class_method')
    varnames   ()
    freevars   ()
    cellvars   ()
    filename   '/Users/vuongngo/workspace/agiflow/packages/python/agiflow-sdk/agiflow/opentelemetry/trace_decorators/wrapper.py'
    name       '<module>'
    firstlineno 1
    lnotab
       0x00ff02010c010c01080120010c010c010c010c0118010c030c010c010c
-      0310010c0324091005160120032a281c7f002d02010c010c0102fc04010e
-      ff02020efe02050efb084502010c010c0102fc04010eff02020efe02050e
-      fb08470c010c0102fb04010eff020202fe02030efd02060efa081e0c010c
-      0102fb04010eff020202fe02030efd02060efa
+      0310010c0324091005160120032a281c7f002902010c010c01020102fb04
+      010eff02020efe02060efa084602010c010c01020102fb04010eff02020e
+      fe02060efa08480c010c01020102fa04010eff020202fe02030efd02070e
+      f908200c010c01020102fa04010eff020202fe02030efd02070ef9
```

### Comparing `agiflow_sdk-0.0.4/agiflow/opentelemetry/trace_decorators/helper.py` & `agiflow_sdk-0.0.5/agiflow/opentelemetry/trace_decorators/helper.py`

 * *Files identical despite different names*

### Comparing `agiflow_sdk-0.0.4/agiflow/opentelemetry/trace_decorators/task.py` & `agiflow_sdk-0.0.5/agiflow/opentelemetry/trace_decorators/task.py`

 * *Files 20% similar despite different names*

```diff
@@ -27,113 +27,127 @@
 
 
 def task(
     name: Optional[str] = None,
     method_name: Optional[str] = None,
     span_kind=SpanKind.INTERNAL,
     tlp_service_type: Optional[AgiflowServiceTypes] = AgiflowServiceTypes.TASK,
+    flush_on_exit=False,
     **kwargs: Unpack[SharedKwargsWithHooks]
 ):
     if method_name is None:
         return decorate_method(
             name=name,
             tlp_service_type=tlp_service_type,
             span_kind=span_kind,
             SpanCapture=TaskSpanCapture,
+            flush_on_exit=flush_on_exit,
             **kwargs
         )
     else:
         return decorate_class_method(
             name=name,
             method_name=method_name,
             tlp_service_type=tlp_service_type,
             span_kind=span_kind,
             SpanCapture=TaskSpanCapture,
+            flush_on_exit=flush_on_exit,
             **kwargs
         )
 
 
 # Async Decorators
 def atask(
     name: Optional[str] = None,
     method_name: Optional[str] = None,
     span_kind=SpanKind.INTERNAL,
     tlp_service_type: Optional[AgiflowServiceTypes] = AgiflowServiceTypes.TASK,
+    flush_on_exit=False,
     **kwargs: Unpack[SharedKwargsWithHooks]
 ):
     if method_name is None:
         return adecorate_method(
           name=name,
           tlp_service_type=tlp_service_type,
           span_kind=span_kind,
           SpanCapture=TaskSpanCapture,
+          flush_on_exit=flush_on_exit,
           **kwargs
           )
     else:
         return adecorate_class_method(
           name=name,
           method_name=method_name,
           tlp_service_type=tlp_service_type,
           span_kind=span_kind,
           SpanCapture=TaskSpanCapture,
+          flush_on_exit=flush_on_exit,
           **kwargs
         )
 
 
 def agent(
     name: Optional[str] = None,
     method_name: Optional[str] = None,
     span_kind=SpanKind.INTERNAL,
+    flush_on_exit=False,
     **kwargs: Unpack[SharedKwargsWithHooks]
 ):
     return task(
       name=name,
       method_name=method_name,
       tlp_service_type=AgiflowServiceTypes.AGENT,
       span_kind=span_kind,
+      flush_on_exit=flush_on_exit,
       **kwargs
     )
 
 
 def tool(
     name: Optional[str] = None,
     method_name: Optional[str] = None,
     span_kind=SpanKind.INTERNAL,
+    flush_on_exit=False,
     **kwargs: Unpack[SharedKwargsWithHooks]
 ):
     return task(
       name=name,
       method_name=method_name,
       tlp_service_type=AgiflowServiceTypes.TOOL,
       span_kind=span_kind,
+      flush_on_exit=flush_on_exit,
       **kwargs
     )
 
 
 def aagent(
     name: Optional[str] = None,
     method_name: Optional[str] = None,
     span_kind=SpanKind.INTERNAL,
+    flush_on_exit=False,
     **kwargs: Unpack[SharedKwargsWithHooks]
 ):
     return atask(
       name=name,
       method_name=method_name,
       tlp_service_type=AgiflowServiceTypes.AGENT,
       span_kind=span_kind,
+      flush_on_exit=flush_on_exit,
       **kwargs
     )
 
 
 def atool(
     name: Optional[str] = None,
     method_name: Optional[str] = None,
     span_kind=SpanKind.INTERNAL,
+    flush_on_exit=False,
     **kwargs: Unpack[SharedKwargsWithHooks]
 ):
     return atask(
       name=name,
       method_name=method_name,
       tlp_service_type=AgiflowServiceTypes.TOOL,
       span_kind=span_kind,
+      flush_on_exit=flush_on_exit,
       **kwargs
     )
```

### Comparing `agiflow_sdk-0.0.4/agiflow/opentelemetry/trace_decorators/workflow.py` & `agiflow_sdk-0.0.5/agiflow/opentelemetry/trace_decorators/workflow.py`

 * *Files 11% similar despite different names*

```diff
@@ -24,39 +24,37 @@
 
     def capture_input(self):
         super().capture_input()
         self.set_span_attribute(
             SpanAttributes.AGIFLOW_SERVICE_TYPE, self.service_type
         )
 
-    @staticmethod
-    def is_flush_on_exit():
-        return True
-
 
 def workflow(
     name: Optional[str] = None,
     method_name: Optional[str] = None,
     span_kind=SpanKind.INTERNAL,
     **kwargs: Unpack[SharedKwargsWithHooks]
 ):
     if method_name is None:
         return decorate_method(
           name=name,
           tlp_service_type=AgiflowServiceTypes.WORKFLOW,
           span_kind=span_kind,
           SpanCapture=WorkflowSpanCapture,
+          flush_on_exit=True,
           **kwargs
           )
     else:
         return decorate_class_method(
           name=name,
           tlp_service_type=AgiflowServiceTypes.WORKFLOW,
           span_kind=span_kind,
           SpanCapture=WorkflowSpanCapture,
+          flush_on_exit=True,
           **kwargs
           )
 
 
 def aworkflow(
     name: Optional[str] = None,
     method_name: Optional[str] = None,
@@ -65,17 +63,19 @@
 ):
     if method_name is None:
         return adecorate_method(
           name=name,
           tlp_service_type=AgiflowServiceTypes.WORKFLOW,
           span_kind=span_kind,
           SpanCapture=WorkflowSpanCapture,
+          flush_on_exit=True,
           **kwargs
           )
     else:
         return adecorate_class_method(
           name=name,
           tlp_service_type=AgiflowServiceTypes.WORKFLOW,
           span_kind=span_kind,
           SpanCapture=WorkflowSpanCapture,
+          flush_on_exit=True,
           **kwargs
         )
```

### Comparing `agiflow_sdk-0.0.4/agiflow/opentelemetry/trace_decorators/wrapper.py` & `agiflow_sdk-0.0.5/agiflow/opentelemetry/trace_decorators/wrapper.py`

 * *Files 2% similar despite different names*

```diff
@@ -114,18 +114,14 @@
         self.set_span_attribute(SpanAttributes.AGIFLOW_SDK_NAME, 'agiflow-python-sdk')
         self.set_span_attribute(SpanAttributes.AGIFLOW_SDK_VERSION, __version__)
         self.set_span_attribute(SpanAttributes.AGIFLOW_SERVICE_NAME, name)
         extra_attributes: Any = baggage.get_baggage(AGIFLOW_ADDITIONAL_SPAN_ATTRIBUTES_KEY)
         self.pydantic_attributes = extra_attributes if extra_attributes is not None else {}
 
     @staticmethod
-    def is_flush_on_exit():
-        return False
-
-    @staticmethod
     def get_span_name(
         name: Optional[str] = None,
         tlp_service_type: Optional[AgiflowServiceTypes] = AgiflowServiceTypes.TASK,
         instance: Any = None,
     ):
         service_type = tlp_service_type or BaseSpanCapture.get_service_type()
 
@@ -249,14 +245,15 @@
 
 
 def decorate_method(
     name: Optional[str] = None,
     tlp_service_type: Optional[AgiflowServiceTypes] = AgiflowServiceTypes.TASK,
     span_kind=SpanKind.INTERNAL,
     SpanCapture=BaseSpanCapture,
+    flush_on_exit=False,
     **config: Unpack[SharedKwargsWithHooks]
 ):
     def decorate(fn):
         @wraps(fn)
         def wrap(*args, **kwargs):
             if not TracerWrapper.verify_initialized():
                 return fn(*args, **kwargs)
@@ -269,15 +266,15 @@
 
             context_parser = config.get('context_parser')
             context = None
             if context_parser is not None and callable(context_parser):
                 carrier = context_parser(*args, **kwargs)
                 context = get_trace_context_from_carrier(carrier)
 
-            with get_tracer(flush_on_exit=SpanCapture.is_flush_on_exit()) as tracer:
+            with get_tracer(flush_on_exit=flush_on_exit) as tracer:
                 with tracer.start_as_current_span(span_name, kind=span_kind, context=context) as span:
                     span_capture = SpanCapture(
                       *args,
                       name=name,
                       service_type=service_type,
                       span=span,
                       instance=fn,
@@ -317,14 +314,15 @@
 
 
 def adecorate_method(
     name: Optional[str] = None,
     tlp_service_type: Optional[AgiflowServiceTypes] = AgiflowServiceTypes.TASK,
     span_kind=SpanKind.INTERNAL,
     SpanCapture=BaseSpanCapture,
+    flush_on_exit=False,
     **config: Unpack[SharedKwargsWithHooks]
 ):
     def decorate(fn):
         @wraps(fn)
         async def wrap(*args, **kwargs):
             if not TracerWrapper.verify_initialized():
                 return fn(*args, **kwargs)
@@ -337,15 +335,15 @@
 
             context_parser = config.get('context_parser')
             context = None
             if context_parser is not None and callable(context_parser):
                 carrier = context_parser(*args, **kwargs)
                 context = get_trace_context_from_carrier(carrier)
 
-            with get_tracer(flush_on_exit=SpanCapture.is_flush_on_exit()) as tracer:
+            with get_tracer(flush_on_exit=flush_on_exit) as tracer:
                 with tracer.start_as_current_span(span_name, kind=span_kind, context=context) as span:
                     span_capture = SpanCapture(
                       *args,
                       name=name,
                       service_type=service_type,
                       span=span,
                       instance=fn,
@@ -386,53 +384,57 @@
 
 def decorate_class_method(
     name: Optional[str],
     method_name: str,
     tlp_service_type: Optional[AgiflowServiceTypes] = AgiflowServiceTypes.TASK,
     span_kind=SpanKind.INTERNAL,
     SpanCapture=BaseSpanCapture,
+    flush_on_exit=False,
     **kwargs: Unpack[SharedKwargsWithHooks]
 ):
     def decorator(cls):
         task_name = name if name else camel_to_snake(cls.__name__)
         method = getattr(cls, method_name)
         setattr(
             cls,
             method_name,
             decorate_method(
               name=task_name,
               tlp_service_type=tlp_service_type,
               span_kind=span_kind,
               SpanCapture=SpanCapture,
+              flush_on_exit=flush_on_exit,
               **kwargs
               )(method),
         )
         return cls
 
     return decorator
 
 
 def adecorate_class_method(
     name: Optional[str],
     method_name: str,
     tlp_service_type: Optional[AgiflowServiceTypes] = AgiflowServiceTypes.TASK,
     span_kind=SpanKind.INTERNAL,
     SpanCapture=BaseSpanCapture,
+    flush_on_exit=False,
     **kwargs: Unpack[SharedKwargsWithHooks]
 ):
     def decorator(cls):
         task_name = name if name else camel_to_snake(cls.__name__)
         method = getattr(cls, method_name)
         setattr(
             cls,
             method_name,
             adecorate_method(
               name=task_name,
               tlp_service_type=tlp_service_type,
               span_kind=span_kind,
               SpanCapture=SpanCapture,
+              flush_on_exit=flush_on_exit,
               **kwargs
               )(method),
         )
         return cls
 
     return decorator
```

### Comparing `agiflow_sdk-0.0.4/agiflow/opentelemetry/trace_exporter/__pycache__/config.cpython-311.pyc` & `agiflow_sdk-0.0.5/agiflow/opentelemetry/trace_exporter/__pycache__/config.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `agiflow_sdk-0.0.4/agiflow/opentelemetry/trace_exporter/__pycache__/json.cpython-311.pyc` & `agiflow_sdk-0.0.5/agiflow/opentelemetry/trace_exporter/__pycache__/json.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `agiflow_sdk-0.0.4/agiflow/opentelemetry/trace_exporter/config.py` & `agiflow_sdk-0.0.5/agiflow/opentelemetry/trace_exporter/config.py`

 * *Files identical despite different names*

### Comparing `agiflow_sdk-0.0.4/agiflow/opentelemetry/trace_exporter/json.py` & `agiflow_sdk-0.0.5/agiflow/opentelemetry/trace_exporter/json.py`

 * *Files identical despite different names*

### Comparing `agiflow_sdk-0.0.4/agiflow/opentelemetry/trace_sampler/__pycache__/no_sampler.cpython-311.pyc` & `agiflow_sdk-0.0.5/agiflow/opentelemetry/trace_sampler/__pycache__/no_sampler.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `agiflow_sdk-0.0.4/agiflow/opentelemetry/trace_sampler/no_sampler.py` & `agiflow_sdk-0.0.5/agiflow/opentelemetry/trace_sampler/no_sampler.py`

 * *Files identical despite different names*

### Comparing `agiflow_sdk-0.0.4/agiflow/opentelemetry/trace_store.py` & `agiflow_sdk-0.0.5/agiflow/opentelemetry/trace_store.py`

 * *Files identical despite different names*

### Comparing `agiflow_sdk-0.0.4/agiflow/opentelemetry/tracing/.DS_Store` & `agiflow_sdk-0.0.5/agiflow/opentelemetry/tracing/.DS_Store`

 * *Files identical despite different names*

### Comparing `agiflow_sdk-0.0.4/agiflow/opentelemetry/tracing/__pycache__/content_allow_list.cpython-311.pyc` & `agiflow_sdk-0.0.5/agiflow/opentelemetry/tracing/__pycache__/content_allow_list.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `agiflow_sdk-0.0.4/agiflow/opentelemetry/tracing/__pycache__/content_alow_list.cpython-311.pyc` & `agiflow_sdk-0.0.5/agiflow/opentelemetry/tracing/__pycache__/content_alow_list.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `agiflow_sdk-0.0.4/agiflow/opentelemetry/tracing/__pycache__/context.cpython-311.pyc` & `agiflow_sdk-0.0.5/agiflow/opentelemetry/tracing/__pycache__/context.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `agiflow_sdk-0.0.4/agiflow/opentelemetry/tracing/__pycache__/context_manager.cpython-311.pyc` & `agiflow_sdk-0.0.5/agiflow/opentelemetry/tracing/__pycache__/context_manager.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `agiflow_sdk-0.0.4/agiflow/opentelemetry/tracing/__pycache__/context_propagation.cpython-311.pyc` & `agiflow_sdk-0.0.5/agiflow/opentelemetry/tracing/__pycache__/context_propagation.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `agiflow_sdk-0.0.4/agiflow/opentelemetry/tracing/__pycache__/span_from_context.cpython-311.pyc` & `agiflow_sdk-0.0.5/agiflow/opentelemetry/tracing/__pycache__/span_from_context.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `agiflow_sdk-0.0.4/agiflow/opentelemetry/tracing/__pycache__/tracing.cpython-311.pyc` & `agiflow_sdk-0.0.5/agiflow/opentelemetry/tracing/__pycache__/tracing.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `agiflow_sdk-0.0.4/agiflow/opentelemetry/tracing/content_allow_list.py` & `agiflow_sdk-0.0.5/agiflow/opentelemetry/tracing/content_allow_list.py`

 * *Files identical despite different names*

### Comparing `agiflow_sdk-0.0.4/agiflow/opentelemetry/tracing/tracing.py` & `agiflow_sdk-0.0.5/agiflow/opentelemetry/tracing/tracing.py`

 * *Files identical despite different names*

### Comparing `agiflow_sdk-0.0.4/agiflow/opentelemetry/types/__init__.py` & `agiflow_sdk-0.0.5/agiflow/opentelemetry/types/__init__.py`

 * *Files identical despite different names*

### Comparing `agiflow_sdk-0.0.4/agiflow/opentelemetry/types/__pycache__/__init__.cpython-311.pyc` & `agiflow_sdk-0.0.5/agiflow/opentelemetry/types/__pycache__/__init__.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `agiflow_sdk-0.0.4/agiflow/opentelemetry/utils/.DS_Store` & `agiflow_sdk-0.0.5/agiflow/opentelemetry/utils/.DS_Store`

 * *Files identical despite different names*

### Comparing `agiflow_sdk-0.0.4/agiflow/opentelemetry/utils/__pycache__/__init__.cpython-311.pyc` & `agiflow_sdk-0.0.5/agiflow/opentelemetry/utils/__pycache__/__init__.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `agiflow_sdk-0.0.4/agiflow/opentelemetry/utils/__pycache__/llm.cpython-311.pyc` & `agiflow_sdk-0.0.5/agiflow/opentelemetry/utils/__pycache__/llm.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `agiflow_sdk-0.0.4/agiflow/opentelemetry/utils/llm.py` & `agiflow_sdk-0.0.5/agiflow/opentelemetry/utils/llm.py`

 * *Files identical despite different names*

### Comparing `agiflow_sdk-0.0.4/agiflow/services/__pycache__/fetch.cpython-311.pyc` & `agiflow_sdk-0.0.5/agiflow/services/__pycache__/fetch.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `agiflow_sdk-0.0.4/agiflow/services/fetch.py` & `agiflow_sdk-0.0.5/agiflow/services/fetch.py`

 * *Files identical despite different names*

### Comparing `agiflow_sdk-0.0.4/agiflow/telemetry/__init__.py` & `agiflow_sdk-0.0.5/agiflow/telemetry/__init__.py`

 * *Files identical despite different names*

### Comparing `agiflow_sdk-0.0.4/agiflow/telemetry/__pycache__/__init__.cpython-311.pyc` & `agiflow_sdk-0.0.5/agiflow/telemetry/__pycache__/__init__.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `agiflow_sdk-0.0.4/agiflow/utils/.DS_Store` & `agiflow_sdk-0.0.5/agiflow/utils/.DS_Store`

 * *Files identical despite different names*

### Comparing `agiflow_sdk-0.0.4/agiflow/utils/__pycache__/__init__.cpython-311.pyc` & `agiflow_sdk-0.0.5/agiflow/utils/__pycache__/__init__.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `agiflow_sdk-0.0.4/agiflow/utils/__pycache__/assertion.cpython-311.pyc` & `agiflow_sdk-0.0.5/agiflow/utils/__pycache__/assertion.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `agiflow_sdk-0.0.4/agiflow/utils/__pycache__/debugging.cpython-311.pyc` & `agiflow_sdk-0.0.5/agiflow/utils/__pycache__/debugging.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `agiflow_sdk-0.0.4/agiflow/utils/__pycache__/error.cpython-311.pyc` & `agiflow_sdk-0.0.5/agiflow/utils/__pycache__/error.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `agiflow_sdk-0.0.4/agiflow/utils/__pycache__/llm.cpython-311.pyc` & `agiflow_sdk-0.0.5/agiflow/utils/__pycache__/llm.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `agiflow_sdk-0.0.4/agiflow/utils/__pycache__/string.cpython-311.pyc` & `agiflow_sdk-0.0.5/agiflow/utils/__pycache__/string.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `agiflow_sdk-0.0.4/agiflow/utils/__pycache__/time.cpython-311.pyc` & `agiflow_sdk-0.0.5/agiflow/utils/__pycache__/time.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `agiflow_sdk-0.0.4/agiflow/utils/debugging.py` & `agiflow_sdk-0.0.5/agiflow/utils/debugging.py`

 * *Files identical despite different names*

### Comparing `agiflow_sdk-0.0.4/agiflow/utils/error.py` & `agiflow_sdk-0.0.5/agiflow/utils/error.py`

 * *Files identical despite different names*

### Comparing `agiflow_sdk-0.0.4/agiflow/utils/string.py` & `agiflow_sdk-0.0.5/agiflow/utils/string.py`

 * *Files identical despite different names*

### Comparing `agiflow_sdk-0.0.4/pyproject.toml` & `agiflow_sdk-0.0.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 [tool.coverage.report]
 exclude_lines = [ "if TYPE_CHECKING:" ]
 show_missing = true
 
 [tool.poetry]
 name = "agiflow-sdk"
-version = "0.0.4"
+version = "0.0.5"
 description = "Agiflow Software Development Kit (SDK) for Python"
 authors = [ "Vuong Ngo <vuongngo.pd@gmail.com>" ]
 repository = "https://github.com/agiflowAI/agiflow"
 documentation = "https://docs.agiflow.io/category/python"
 license = "Apache-2.0"
 readme = "README.md"
```

### Comparing `agiflow_sdk-0.0.4/PKG-INFO` & `agiflow_sdk-0.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: agiflow-sdk
-Version: 0.0.4
+Version: 0.0.5
 Summary: Agiflow Software Development Kit (SDK) for Python
 Home-page: https://github.com/agiflowAI/agiflow
 License: Apache-2.0
 Author: Vuong Ngo
 Author-email: vuongngo.pd@gmail.com
 Requires-Python: >=3.9,<4
 Classifier: License :: OSI Approved :: Apache Software License
```

