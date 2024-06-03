# Comparing `tmp/ollama_haystack-0.0.6.tar.gz` & `tmp/ollama_haystack-0.0.7.tar.gz`

## Comparing `ollama_haystack-0.0.6.tar` & `ollama_haystack-0.0.7.tar`

### file list

```diff
@@ -1,21 +1,21 @@
--rw-r--r--   0        0        0     2337 2020-02-02 00:00:00.000000 ollama_haystack-0.0.6/examples/chat_generator_example.py
--rw-r--r--   0        0        0     1568 2020-02-02 00:00:00.000000 ollama_haystack-0.0.6/examples/embedders_example.py
--rw-r--r--   0        0        0     2224 2020-02-02 00:00:00.000000 ollama_haystack-0.0.6/examples/generator_example.py
--rw-r--r--   0        0        0     1042 2020-02-02 00:00:00.000000 ollama_haystack-0.0.6/pydoc/config.yml
--rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 ollama_haystack-0.0.6/src/haystack_integrations/components/embedders/ollama/__init__.py
--rw-r--r--   0        0        0     6117 2020-02-02 00:00:00.000000 ollama_haystack-0.0.6/src/haystack_integrations/components/embedders/ollama/document_embedder.py
--rw-r--r--   0        0        0     3111 2020-02-02 00:00:00.000000 ollama_haystack-0.0.6/src/haystack_integrations/components/embedders/ollama/text_embedder.py
--rw-r--r--   0        0        0      146 2020-02-02 00:00:00.000000 ollama_haystack-0.0.6/src/haystack_integrations/components/generators/ollama/__init__.py
--rw-r--r--   0        0        0     7927 2020-02-02 00:00:00.000000 ollama_haystack-0.0.6/src/haystack_integrations/components/generators/ollama/generator.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ollama_haystack-0.0.6/src/haystack_integrations/components/generators/ollama/chat/__init__.py
--rw-r--r--   0        0        0     4584 2020-02-02 00:00:00.000000 ollama_haystack-0.0.6/src/haystack_integrations/components/generators/ollama/chat/chat_generator.py
--rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 ollama_haystack-0.0.6/tests/__init__.py
--rw-r--r--   0        0        0     4852 2020-02-02 00:00:00.000000 ollama_haystack-0.0.6/tests/test_chat_generator.py
--rw-r--r--   0        0        0     1890 2020-02-02 00:00:00.000000 ollama_haystack-0.0.6/tests/test_document_embedder.py
--rw-r--r--   0        0        0     7040 2020-02-02 00:00:00.000000 ollama_haystack-0.0.6/tests/test_generator.py
--rw-r--r--   0        0        0     1451 2020-02-02 00:00:00.000000 ollama_haystack-0.0.6/tests/test_text_embedder.py
--rw-r--r--   0        0        0     1872 2020-02-02 00:00:00.000000 ollama_haystack-0.0.6/.gitignore
--rw-r--r--   0        0        0    11350 2020-02-02 00:00:00.000000 ollama_haystack-0.0.6/LICENSE.txt
--rw-r--r--   0        0        0     1013 2020-02-02 00:00:00.000000 ollama_haystack-0.0.6/README.md
--rw-r--r--   0        0        0     4127 2020-02-02 00:00:00.000000 ollama_haystack-0.0.6/pyproject.toml
--rw-r--r--   0        0        0     2249 2020-02-02 00:00:00.000000 ollama_haystack-0.0.6/PKG-INFO
+-rw-r--r--   0        0        0     2337 2020-02-02 00:00:00.000000 ollama_haystack-0.0.7/examples/chat_generator_example.py
+-rw-r--r--   0        0        0     1568 2020-02-02 00:00:00.000000 ollama_haystack-0.0.7/examples/embedders_example.py
+-rw-r--r--   0        0        0     2224 2020-02-02 00:00:00.000000 ollama_haystack-0.0.7/examples/generator_example.py
+-rw-r--r--   0        0        0     1046 2020-02-02 00:00:00.000000 ollama_haystack-0.0.7/pydoc/config.yml
+-rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 ollama_haystack-0.0.7/src/haystack_integrations/components/embedders/ollama/__init__.py
+-rw-r--r--   0        0        0     6117 2020-02-02 00:00:00.000000 ollama_haystack-0.0.7/src/haystack_integrations/components/embedders/ollama/document_embedder.py
+-rw-r--r--   0        0        0     3111 2020-02-02 00:00:00.000000 ollama_haystack-0.0.7/src/haystack_integrations/components/embedders/ollama/text_embedder.py
+-rw-r--r--   0        0        0      146 2020-02-02 00:00:00.000000 ollama_haystack-0.0.7/src/haystack_integrations/components/generators/ollama/__init__.py
+-rw-r--r--   0        0        0     7927 2020-02-02 00:00:00.000000 ollama_haystack-0.0.7/src/haystack_integrations/components/generators/ollama/generator.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ollama_haystack-0.0.7/src/haystack_integrations/components/generators/ollama/chat/__init__.py
+-rw-r--r--   0        0        0     6742 2020-02-02 00:00:00.000000 ollama_haystack-0.0.7/src/haystack_integrations/components/generators/ollama/chat/chat_generator.py
+-rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 ollama_haystack-0.0.7/tests/__init__.py
+-rw-r--r--   0        0        0     5877 2020-02-02 00:00:00.000000 ollama_haystack-0.0.7/tests/test_chat_generator.py
+-rw-r--r--   0        0        0     1890 2020-02-02 00:00:00.000000 ollama_haystack-0.0.7/tests/test_document_embedder.py
+-rw-r--r--   0        0        0     7040 2020-02-02 00:00:00.000000 ollama_haystack-0.0.7/tests/test_generator.py
+-rw-r--r--   0        0        0     1451 2020-02-02 00:00:00.000000 ollama_haystack-0.0.7/tests/test_text_embedder.py
+-rw-r--r--   0        0        0     1872 2020-02-02 00:00:00.000000 ollama_haystack-0.0.7/.gitignore
+-rw-r--r--   0        0        0    11350 2020-02-02 00:00:00.000000 ollama_haystack-0.0.7/LICENSE.txt
+-rw-r--r--   0        0        0     1013 2020-02-02 00:00:00.000000 ollama_haystack-0.0.7/README.md
+-rw-r--r--   0        0        0     4183 2020-02-02 00:00:00.000000 ollama_haystack-0.0.7/pyproject.toml
+-rw-r--r--   0        0        0     2312 2020-02-02 00:00:00.000000 ollama_haystack-0.0.7/PKG-INFO
```

### Comparing `ollama_haystack-0.0.6/examples/chat_generator_example.py` & `ollama_haystack-0.0.7/examples/chat_generator_example.py`

 * *Files identical despite different names*

### Comparing `ollama_haystack-0.0.6/examples/embedders_example.py` & `ollama_haystack-0.0.7/examples/embedders_example.py`

 * *Files identical despite different names*

### Comparing `ollama_haystack-0.0.6/examples/generator_example.py` & `ollama_haystack-0.0.7/examples/generator_example.py`

 * *Files identical despite different names*

### Comparing `ollama_haystack-0.0.6/pydoc/config.yml` & `ollama_haystack-0.0.7/pydoc/config.yml`

 * *Files 9% similar despite different names*

```diff
@@ -13,15 +13,15 @@
     expression:
     documented_only: true
     do_not_filter_modules: false
     skip_empty_modules: true
   - type: smart
   - type: crossref
 renderer:
-  type: haystack_pydoc_tools.renderers.ReadmePreviewRenderer
+  type: haystack_pydoc_tools.renderers.ReadmeIntegrationRenderer
   excerpt: Ollama integration for Haystack
   category_slug: integrations-api
   title: Ollama
   slug: integrations-ollama
   order: 170
   markdown:
     descriptive_class_title: false
```

### Comparing `ollama_haystack-0.0.6/src/haystack_integrations/components/embedders/ollama/document_embedder.py` & `ollama_haystack-0.0.7/src/haystack_integrations/components/embedders/ollama/document_embedder.py`

 * *Files identical despite different names*

### Comparing `ollama_haystack-0.0.6/src/haystack_integrations/components/embedders/ollama/text_embedder.py` & `ollama_haystack-0.0.7/src/haystack_integrations/components/embedders/ollama/text_embedder.py`

 * *Files identical despite different names*

### Comparing `ollama_haystack-0.0.6/src/haystack_integrations/components/generators/ollama/generator.py` & `ollama_haystack-0.0.7/src/haystack_integrations/components/generators/ollama/generator.py`

 * *Files identical despite different names*

### Comparing `ollama_haystack-0.0.6/tests/test_chat_generator.py` & `ollama_haystack-0.0.7/tests/test_chat_generator.py`

 * *Files 15% similar despite different names*

```diff
@@ -37,15 +37,17 @@
         assert component.model == "llama2"
         assert component.url == "http://my-custom-endpoint:11434/api/chat"
         assert component.generation_kwargs == {"temperature": 0.5}
         assert component.template is None
         assert component.timeout == 5
 
     def test_create_json_payload(self, chat_messages):
-        observed = OllamaChatGenerator(model="some_model")._create_json_payload(chat_messages, {"temperature": 0.1})
+        observed = OllamaChatGenerator(model="some_model")._create_json_payload(
+            chat_messages, False, {"temperature": 0.1}
+        )
         expected = {
             "messages": [
                 {"role": "user", "content": "Tell me about why Super Mario is the greatest superhero"},
                 {"role": "assistant", "content": "Super Mario has prevented Bowser from destroying the world"},
             ],
             "model": "some_model",
             "stream": False,
@@ -121,7 +123,31 @@
         component = OllamaChatGenerator(model="Alistair_and_Stefano_are_great")
 
         with pytest.raises(HTTPError):
             message = ChatMessage.from_user(
                 "Based on your infinite wisdom, can you tell me why Alistair and Stefano are so great?"
             )
             component.run([message])
+
+    @pytest.mark.integration
+    def test_run_with_streaming(self):
+        streaming_callback = Mock()
+        chat_generator = OllamaChatGenerator(streaming_callback=streaming_callback)
+
+        chat_history = [
+            {"role": "user", "content": "What is the largest city in the United Kingdom by population?"},
+            {"role": "assistant", "content": "London is the largest city in the United Kingdom by population"},
+            {"role": "user", "content": "And what is the second largest?"},
+        ]
+
+        chat_messages = [
+            ChatMessage(role=ChatRole(message["role"]), content=message["content"], name=None)
+            for message in chat_history
+        ]
+
+        response = chat_generator.run(chat_messages)
+
+        streaming_callback.assert_called()
+
+        assert isinstance(response, dict)
+        assert isinstance(response["replies"], list)
+        assert "Manchester" in response["replies"][-1].content or "Glasgow" in response["replies"][-1].content
```

### Comparing `ollama_haystack-0.0.6/tests/test_document_embedder.py` & `ollama_haystack-0.0.7/tests/test_document_embedder.py`

 * *Files identical despite different names*

### Comparing `ollama_haystack-0.0.6/tests/test_generator.py` & `ollama_haystack-0.0.7/tests/test_generator.py`

 * *Files identical despite different names*

### Comparing `ollama_haystack-0.0.6/tests/test_text_embedder.py` & `ollama_haystack-0.0.7/tests/test_text_embedder.py`

 * *Files identical despite different names*

### Comparing `ollama_haystack-0.0.6/.gitignore` & `ollama_haystack-0.0.7/.gitignore`

 * *Files identical despite different names*

### Comparing `ollama_haystack-0.0.6/LICENSE.txt` & `ollama_haystack-0.0.7/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `ollama_haystack-0.0.6/README.md` & `ollama_haystack-0.0.7/README.md`

 * *Files identical despite different names*

### Comparing `ollama_haystack-0.0.6/pyproject.toml` & `ollama_haystack-0.0.7/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 keywords = []
 authors = [
     { name = "Alistair Rogers", email = "alistairlr112@gmail.com" },
     { name = "Sachin Sachdeva", email = "emailforsachinsachdeva@gmail.com" },
     { name = "deepset GmbH", email = "info@deepset.ai" },
 ]
 classifiers = [
+  "License :: OSI Approved :: Apache Software License",
     "Development Status :: 4 - Beta",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "Programming Language :: Python :: 3.12",
```

### Comparing `ollama_haystack-0.0.6/PKG-INFO` & `ollama_haystack-0.0.7/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 Metadata-Version: 2.3
 Name: ollama-haystack
-Version: 0.0.6
+Version: 0.0.7
 Summary: An integration between the Ollama LLM framework and Haystack
 Project-URL: Documentation, https://github.com/deepset-ai/haystack-core-integrations/tree/main/integrations/ollama#readme
 Project-URL: Issues, https://github.com/deepset-ai/haystack-core-integrations/issues
 Project-URL: Source, https://github.com/deepset-ai/haystack-core-integrations/tree/main/integrations/ollama
 Author-email: Alistair Rogers <alistairlr112@gmail.com>, Sachin Sachdeva <emailforsachinsachdeva@gmail.com>, deepset GmbH <info@deepset.ai>
 License-Expression: Apache-2.0
 License-File: LICENSE.txt
 Classifier: Development Status :: 4 - Beta
+Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: CPython
```

