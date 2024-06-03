# Comparing `tmp/openbb_agents-0.0.3.tar.gz` & `tmp/openbb_agents-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openbb_agents-0.0.3.tar", max compression
+gzip compressed data, was "openbb_agents-0.0.4.tar", max compression
```

## Comparing `openbb_agents-0.0.3.tar` & `openbb_agents-0.0.4.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     4153 2024-05-20 11:03:56.175819 openbb_agents-0.0.3/README.md
--rw-r--r--   0        0        0     1210 2024-05-20 11:03:56.175819 openbb_agents-0.0.3/openbb_agents/__init__.py
--rw-r--r--   0        0        0    10409 2024-05-20 11:03:56.175819 openbb_agents-0.0.3/openbb_agents/agent.py
--rw-r--r--   0        0        0     8626 2024-05-20 11:03:56.175819 openbb_agents-0.0.3/openbb_agents/chains.py
--rw-r--r--   0        0        0      753 2024-05-20 11:03:56.175819 openbb_agents-0.0.3/openbb_agents/models.py
--rw-r--r--   0        0        0     6496 2024-05-20 11:03:56.175819 openbb_agents-0.0.3/openbb_agents/prompts.py
--rw-r--r--   0        0        0     1595 2024-05-20 11:03:56.175819 openbb_agents-0.0.3/openbb_agents/testing.py
--rw-r--r--   0        0        0     4160 2024-05-20 11:03:56.175819 openbb_agents-0.0.3/openbb_agents/tools.py
--rw-r--r--   0        0        0      506 2024-05-20 11:03:56.175819 openbb_agents-0.0.3/openbb_agents/utils.py
--rw-r--r--   0        0        0      999 2024-05-20 11:03:56.175819 openbb_agents-0.0.3/pyproject.toml
--rw-r--r--   0        0        0     5035 1970-01-01 00:00:00.000000 openbb_agents-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0     4400 2024-06-03 09:11:20.308784 openbb_agents-0.0.4/README.md
+-rw-r--r--   0        0        0     1210 2024-06-03 09:11:20.308784 openbb_agents-0.0.4/openbb_agents/__init__.py
+-rw-r--r--   0        0        0    11587 2024-06-03 09:11:20.308784 openbb_agents-0.0.4/openbb_agents/agent.py
+-rw-r--r--   0        0        0     8626 2024-06-03 09:11:20.308784 openbb_agents-0.0.4/openbb_agents/chains.py
+-rw-r--r--   0        0        0      753 2024-06-03 09:11:20.308784 openbb_agents-0.0.4/openbb_agents/models.py
+-rw-r--r--   0        0        0     6496 2024-06-03 09:11:20.308784 openbb_agents-0.0.4/openbb_agents/prompts.py
+-rw-r--r--   0        0        0     1595 2024-06-03 09:11:20.308784 openbb_agents-0.0.4/openbb_agents/testing.py
+-rw-r--r--   0        0        0     5963 2024-06-03 09:11:20.312784 openbb_agents-0.0.4/openbb_agents/tools.py
+-rw-r--r--   0        0        0     2025 2024-06-03 09:11:20.312784 openbb_agents-0.0.4/openbb_agents/utils.py
+-rw-r--r--   0        0        0      999 2024-06-03 09:11:20.312784 openbb_agents-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0     5282 1970-01-01 00:00:00.000000 openbb_agents-0.0.4/PKG-INFO
```

### Comparing `openbb_agents-0.0.3/README.md` & `openbb_agents-0.0.4/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -29,14 +29,16 @@
 
 ### OpenBB Platform data provider credentials
 To use the OpenBB Platform functions, you need to configure the necessary [data provider API credentials](https://docs.openbb.co/platform/usage/api_keys). This can be done in one of two ways:
 
 1. **Local Configuration**: Specify your credentials in a `~/.openbb_platform/user_settings.json` file. Follow the [local environment setup guide](https://docs.openbb.co/platform/usage/api_keys#local-environment) for detailed instructions.
 2. **OpenBB Hub**: Create a personal access token (PAT) via your [OpenBB Hub](https://my.openbb.co/) account. This PAT can then be passed to the agent as an argument.
 
+## Getting started
+It is highly recommended to take a look at the [Getting Started Notebook](https://github.com/OpenBB-finance/openbb-agents/blob/main/getting_started.ipynb), which runs you through the features of `openbb-agents` at a high level.
 
 ## Usage
 
 ``` python
 >>> from openbb_agents.agent import openbb_agent
 >>> result = openbb_agent("What is the current market cap of TSLA?")  # Will print some logs to show you progress
 >>> print(result)
```

### Comparing `openbb_agents-0.0.3/openbb_agents/__init__.py` & `openbb_agents-0.0.4/openbb_agents/__init__.py`

 * *Files identical despite different names*

### Comparing `openbb_agents-0.0.3/openbb_agents/agent.py` & `openbb_agents-0.0.4/openbb_agents/agent.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,71 +1,85 @@
 import asyncio
 import logging
+from typing import Callable
 
 from langchain.vectorstores import VectorStore
 
 from .chains import (
     agenerate_subquestion_answer,
     agenerate_subquestions_from_query,
     asearch_tools,
     generate_final_answer,
     generate_subquestion_answer,
     generate_subquestions_from_query,
     search_tools,
 )
 from .models import AnsweredSubQuestion, SubQuestion
 from .tools import (
+    append_tools_to_vector_index,
     build_openbb_tool_vector_index,
     build_vector_index_from_openbb_function_descriptions,
     get_valid_list_of_providers,
     map_name_to_openbb_function_description,
 )
-from .utils import get_dependencies
+from .utils import configure_logging, get_dependencies
 
 logger = logging.getLogger(__name__)
 
 
 def openbb_agent(
-    query: str, openbb_tools: list[str] | None = None, openbb_pat: str | None = None
+    query: str,
+    openbb_tools: list[str] | None = None,
+    openbb_pat: str | None = None,
+    extra_tools: list[Callable] | None = None,
+    verbose: bool = True,
 ) -> str:
     """Answer a query using the OpenBB Agent equipped with tools.
 
-    By default all available openbb tools are used. You can have a query
-    answered using a smaller subset of OpenBB tools by using the `openbb_tools`
-    argument.
-
     Parameters
     ----------
     query : str
         The query to be answered.
     openbb_tools : list[str] | None, optional
         A list of specific OpenBB functions to use. If not provided, all
         available OpenBB tools that you have valid credentials for will be
         utilized. See `openbb_pat`.
     openbb_pat : str | None, optional
         The OpenBB PAT for retrieving credentials from the OpenBB Hub. If not
         provided, local OpenBB credentials will be used.
+    extra_tools : list[Callable] | None, optional
+        A list of extra tools to add to the tool index, which makes it available
+        to the LLM to use.
+    verbose : bool, optional
+        Whether to print out additional information about the agent's behavior.
+        Defaults to True.
 
     Examples
     --------
     >>> # Use all OpenBB tools to answer the query
     >>> openbb_agent("What is the stock price of TSLA?")
     >>> # Use only the specified tools to answer the query
     >>> openbb_agent("What is the stock price of TSLA?",
     ...              openbb_tools=['.equity.price.quote'])
-
     """
+    configure_logging(verbose)
     if openbb_pat:
         from openbb import obb
 
         obb.account.login(pat=openbb_pat)
 
     tool_vector_index = _handle_tool_vector_index(openbb_tools)
-    subquestions = generate_subquestions_from_query(user_query=query)
+    if extra_tools:
+        tool_vector_index = append_tools_to_vector_index(
+            vector_store=tool_vector_index,
+            tools=extra_tools,
+        )
 
+    logger.info("Generating subquestions for user query: %s", query)
+    subquestions = generate_subquestions_from_query(user_query=query)
     logger.info("Generated subquestions: %s", subquestions)
 
     answered_subquestions = []
     for subquestion in subquestions:
         if _is_subquestion_answerable(
             subquestion=subquestion, answered_subquestions=answered_subquestions
         ):
@@ -81,42 +95,58 @@
             logger.info("Skipping unanswerable subquestion: %s", subquestion)
     return generate_final_answer(
         user_query=query,
         answered_subquestions=answered_subquestions,
     )
 
 
-async def aopenbb_agent(query: str, openbb_tools: list[str] | None = None) -> str:
+async def aopenbb_agent(
+    query: str,
+    openbb_tools: list[str] | None = None,
+    extra_tools: list[Callable] | None = None,
+    verbose: bool = True,
+) -> str:
     """Answer a query using the OpenBB Agent equipped with tools.
 
     Async variant of `openbb_agent`.
 
-    By default all available openbb tools are used. You can have a query
-    answered using a smaller subset of OpenBB tools by using the `openbb_tools`
-    argument.
-
     Parameters
     ----------
     query : str
-        The query you want to have answered.
-    openbb_tools : list[Callable]
-        Optional. Specify the OpenBB functions you want to use. If not
-        specified, every available OpenBB tool will be used.
+        The query to be answered.
+    openbb_tools : list[str] | None, optional
+        A list of specific OpenBB functions to use. If not provided, all
+        available OpenBB tools that you have valid credentials for will be
+        utilized. See `openbb_pat`.
+    openbb_pat : str | None, optional
+        The OpenBB PAT for retrieving credentials from the OpenBB Hub. If not
+        provided, local OpenBB credentials will be used.
+    extra_tools : list[Callable] | None, optional
+        A list of extra tools to add to the tool index, which makes it available
+        to the LLM to use.
+    verbose : bool, optional
+        Whether to print out additional information about the agent's behavior.
+        Defaults to True.
 
     Examples
     --------
     >>> # Use all OpenBB tools to answer the query
     >>> openbb_agent("What is the stock price of TSLA?")
     >>> # Use only the specified tools to answer the query
     >>> openbb_agent("What is the stock price of TSLA?",
     ...              openbb_tools=['.equity.price.quote'])
 
     """
+    configure_logging(verbose)
     tool_vector_index = _handle_tool_vector_index(openbb_tools)
-
+    if extra_tools:
+        tool_vector_index = append_tools_to_vector_index(
+            vector_store=tool_vector_index,
+            tools=extra_tools,
+        )
     subquestions = await agenerate_subquestions_from_query(user_query=query)
     answered_subquestions = await _aprocess_subquestions(
         user_query=query,
         subquestions=subquestions,
         tool_vector_index=tool_vector_index,
     )
```

### Comparing `openbb_agents-0.0.3/openbb_agents/chains.py` & `openbb_agents-0.0.4/openbb_agents/chains.py`

 * *Files identical despite different names*

### Comparing `openbb_agents-0.0.3/openbb_agents/models.py` & `openbb_agents-0.0.4/openbb_agents/models.py`

 * *Files identical despite different names*

### Comparing `openbb_agents-0.0.3/openbb_agents/prompts.py` & `openbb_agents-0.0.4/openbb_agents/prompts.py`

 * *Files identical despite different names*

### Comparing `openbb_agents-0.0.3/openbb_agents/testing.py` & `openbb_agents-0.0.4/openbb_agents/testing.py`

 * *Files identical despite different names*

### Comparing `openbb_agents-0.0.3/pyproject.toml` & `openbb_agents-0.0.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "openbb-agents"
-version = "0.0.3"
+version = "0.0.4"
 description = "LLMs X OpenBB Platform"
 authors = ["Michael Struwig <michael.struwig@openbb.finance>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = ">=3.10,<3.12"
 jupyterlab = "^4.0.9"
```

### Comparing `openbb_agents-0.0.3/PKG-INFO` & `openbb_agents-0.0.4/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openbb-agents
-Version: 0.0.3
+Version: 0.0.4
 Summary: LLMs X OpenBB Platform
 Author: Michael Struwig
 Author-email: michael.struwig@openbb.finance
 Requires-Python: >=3.10,<3.12
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
@@ -52,14 +52,16 @@
 
 ### OpenBB Platform data provider credentials
 To use the OpenBB Platform functions, you need to configure the necessary [data provider API credentials](https://docs.openbb.co/platform/usage/api_keys). This can be done in one of two ways:
 
 1. **Local Configuration**: Specify your credentials in a `~/.openbb_platform/user_settings.json` file. Follow the [local environment setup guide](https://docs.openbb.co/platform/usage/api_keys#local-environment) for detailed instructions.
 2. **OpenBB Hub**: Create a personal access token (PAT) via your [OpenBB Hub](https://my.openbb.co/) account. This PAT can then be passed to the agent as an argument.
 
+## Getting started
+It is highly recommended to take a look at the [Getting Started Notebook](https://github.com/OpenBB-finance/openbb-agents/blob/main/getting_started.ipynb), which runs you through the features of `openbb-agents` at a high level.
 
 ## Usage
 
 ``` python
 >>> from openbb_agents.agent import openbb_agent
 >>> result = openbb_agent("What is the current market cap of TSLA?")  # Will print some logs to show you progress
 >>> print(result)
```

