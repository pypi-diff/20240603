# Comparing `tmp/opentelemetry_instrumentation_ollama-0.21.2.tar.gz` & `tmp/opentelemetry_instrumentation_ollama-0.21.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "opentelemetry_instrumentation_ollama-0.21.2.tar", max compression
+gzip compressed data, was "opentelemetry_instrumentation_ollama-0.21.3.tar", max compression
```

## Comparing `opentelemetry_instrumentation_ollama-0.21.2.tar` & `opentelemetry_instrumentation_ollama-0.21.3.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1146 2024-05-31 18:54:20.351480 opentelemetry_instrumentation_ollama-0.21.2/README.md
--rw-r--r--   0        0        0     9986 2024-05-31 18:54:20.351480 opentelemetry_instrumentation_ollama-0.21.2/opentelemetry/instrumentation/ollama/__init__.py
--rw-r--r--   0        0        0       42 2024-05-31 18:54:20.351480 opentelemetry_instrumentation_ollama-0.21.2/opentelemetry/instrumentation/ollama/config.py
--rw-r--r--   0        0        0      740 2024-05-31 18:54:20.351480 opentelemetry_instrumentation_ollama-0.21.2/opentelemetry/instrumentation/ollama/utils.py
--rw-r--r--   0        0        0       23 2024-05-31 18:54:20.351480 opentelemetry_instrumentation_ollama-0.21.2/opentelemetry/instrumentation/ollama/version.py
--rw-r--r--   0        0        0     1399 2024-05-31 18:54:50.135362 opentelemetry_instrumentation_ollama-0.21.2/pyproject.toml
--rw-r--r--   0        0        0     2293 1970-01-01 00:00:00.000000 opentelemetry_instrumentation_ollama-0.21.2/PKG-INFO
+-rw-r--r--   0        0        0     1146 2024-06-03 09:43:21.522364 opentelemetry_instrumentation_ollama-0.21.3/README.md
+-rw-r--r--   0        0        0     9986 2024-06-03 09:43:21.522364 opentelemetry_instrumentation_ollama-0.21.3/opentelemetry/instrumentation/ollama/__init__.py
+-rw-r--r--   0        0        0       42 2024-06-03 09:43:21.522364 opentelemetry_instrumentation_ollama-0.21.3/opentelemetry/instrumentation/ollama/config.py
+-rw-r--r--   0        0        0      740 2024-06-03 09:43:21.522364 opentelemetry_instrumentation_ollama-0.21.3/opentelemetry/instrumentation/ollama/utils.py
+-rw-r--r--   0        0        0       23 2024-06-03 09:43:21.522364 opentelemetry_instrumentation_ollama-0.21.3/opentelemetry/instrumentation/ollama/version.py
+-rw-r--r--   0        0        0     1399 2024-06-03 09:43:46.486222 opentelemetry_instrumentation_ollama-0.21.3/pyproject.toml
+-rw-r--r--   0        0        0     2293 1970-01-01 00:00:00.000000 opentelemetry_instrumentation_ollama-0.21.3/PKG-INFO
```

### Comparing `opentelemetry_instrumentation_ollama-0.21.2/README.md` & `opentelemetry_instrumentation_ollama-0.21.3/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # OpenTelemetry Ollama Instrumentation
 
 <a href="https://pypi.org/project/opentelemetry-instrumentation-ollama/">
     <img src="https://badge.fury.io/py/opentelemetry-instrumentation-ollama.svg">
 </a>
 
-This library allows tracing calls to any of Cohere's endpoints sent with the official [Ollama Python Library](https://github.com/ollama/ollama-python).
+This library allows tracing calls to any of Ollama's endpoints sent with the official [Ollama Python Library](https://github.com/ollama/ollama-python).
 
 ## Installation
 
 ```bash
 pip install opentelemetry-instrumentation-ollama
 ```
```

#### html2text {}

```diff
@@ -1,9 +1,9 @@
 # OpenTelemetry Ollama Instrumentation _[_h_t_t_p_s_:_/_/_b_a_d_g_e_._f_u_r_y_._i_o_/_p_y_/_o_p_e_n_t_e_l_e_m_e_t_r_y_-
-_i_n_s_t_r_u_m_e_n_t_a_t_i_o_n_-_o_l_l_a_m_a_._s_v_g_]This library allows tracing calls to any of Cohere's
+_i_n_s_t_r_u_m_e_n_t_a_t_i_o_n_-_o_l_l_a_m_a_._s_v_g_]This library allows tracing calls to any of Ollama's
 endpoints sent with the official [Ollama Python Library](https://github.com/
 ollama/ollama-python). ## Installation ```bash pip install opentelemetry-
 instrumentation-ollama ``` ## Example usage ```python from
 opentelemetry.instrumentation.ollama import OllamaInstrumentor
 OllamaInstrumentor().instrument() ``` ## Privacy **By default, this
 instrumentation logs prompts, completions, and embeddings to span attributes**.
 This gives you a clear visibility into how your LLM application is working, and
```

### Comparing `opentelemetry_instrumentation_ollama-0.21.2/opentelemetry/instrumentation/ollama/__init__.py` & `opentelemetry_instrumentation_ollama-0.21.3/opentelemetry/instrumentation/ollama/__init__.py`

 * *Files identical despite different names*

### Comparing `opentelemetry_instrumentation_ollama-0.21.2/opentelemetry/instrumentation/ollama/utils.py` & `opentelemetry_instrumentation_ollama-0.21.3/opentelemetry/instrumentation/ollama/utils.py`

 * *Files identical despite different names*

### Comparing `opentelemetry_instrumentation_ollama-0.21.2/pyproject.toml` & `opentelemetry_instrumentation_ollama-0.21.3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 [tool.coverage.report]
 exclude_lines = ['if TYPE_CHECKING:']
 show_missing = true
 
 [tool.poetry]
 name = "opentelemetry-instrumentation-ollama"
-version = "0.21.2"
+version = "0.21.3"
 description = "OpenTelemetry Ollama instrumentation"
 authors = [
   "Gal Kleinman <gal@traceloop.com>",
   "Nir Gazit <nir@traceloop.com>",
 ]
 repository = "https://github.com/traceloop/openllmetry/tree/main/packages/opentelemetry-instrumentation-ollama"
 license = "Apache-2.0"
```

### Comparing `opentelemetry_instrumentation_ollama-0.21.2/PKG-INFO` & `opentelemetry_instrumentation_ollama-0.21.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: opentelemetry-instrumentation-ollama
-Version: 0.21.2
+Version: 0.21.3
 Summary: OpenTelemetry Ollama instrumentation
 Home-page: https://github.com/traceloop/openllmetry/tree/main/packages/opentelemetry-instrumentation-ollama
 License: Apache-2.0
 Author: Gal Kleinman
 Author-email: gal@traceloop.com
 Requires-Python: >=3.9,<4
 Classifier: License :: OSI Approved :: Apache Software License
@@ -24,15 +24,15 @@
 
 # OpenTelemetry Ollama Instrumentation
 
 <a href="https://pypi.org/project/opentelemetry-instrumentation-ollama/">
     <img src="https://badge.fury.io/py/opentelemetry-instrumentation-ollama.svg">
 </a>
 
-This library allows tracing calls to any of Cohere's endpoints sent with the official [Ollama Python Library](https://github.com/ollama/ollama-python).
+This library allows tracing calls to any of Ollama's endpoints sent with the official [Ollama Python Library](https://github.com/ollama/ollama-python).
 
 ## Installation
 
 ```bash
 pip install opentelemetry-instrumentation-ollama
 ```
```

#### html2text {}

```diff
@@ -1,9 +1,9 @@
 Metadata-Version: 2.1 Name: opentelemetry-instrumentation-ollama Version:
-0.21.2 Summary: OpenTelemetry Ollama instrumentation Home-page: https://
+0.21.3 Summary: OpenTelemetry Ollama instrumentation Home-page: https://
 github.com/traceloop/openllmetry/tree/main/packages/opentelemetry-
 instrumentation-ollama License: Apache-2.0 Author: Gal Kleinman Author-email:
 gal@traceloop.com Requires-Python: >=3.9,<4 Classifier: License :: OSI Approved
 :: Apache Software License Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
 Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12 Provides-Extra: instruments
@@ -11,15 +11,15 @@
 opentelemetry-api (>=1.25.0,<2.0.0) Requires-Dist: opentelemetry-
 instrumentation (>=0.46b0,<0.47) Requires-Dist: opentelemetry-semantic-
 conventions (>=0.46b0,<0.47) Requires-Dist: opentelemetry-semantic-conventions-
 ai (==0.2.0) Project-URL: Repository, https://github.com/traceloop/openllmetry/
 tree/main/packages/opentelemetry-instrumentation-ollama Description-Content-
 Type: text/markdown # OpenTelemetry Ollama Instrumentation _[_h_t_t_p_s_:_/_/
 _b_a_d_g_e_._f_u_r_y_._i_o_/_p_y_/_o_p_e_n_t_e_l_e_m_e_t_r_y_-_i_n_s_t_r_u_m_e_n_t_a_t_i_o_n_-_o_l_l_a_m_a_._s_v_g_]This library allows
-tracing calls to any of Cohere's endpoints sent with the official [Ollama
+tracing calls to any of Ollama's endpoints sent with the official [Ollama
 Python Library](https://github.com/ollama/ollama-python). ## Installation
 ```bash pip install opentelemetry-instrumentation-ollama ``` ## Example usage
 ```python from opentelemetry.instrumentation.ollama import OllamaInstrumentor
 OllamaInstrumentor().instrument() ``` ## Privacy **By default, this
 instrumentation logs prompts, completions, and embeddings to span attributes**.
 This gives you a clear visibility into how your LLM application is working, and
 can make it easy to debug and evaluate the quality of the outputs. However, you
```

