# Comparing `tmp/aily_code_sdk-0.1.0b5.tar.gz` & `tmp/aily_code_sdk-0.1.0b6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aily_code_sdk-0.1.0b5.tar", max compression
+gzip compressed data, was "aily_code_sdk-0.1.0b6.tar", max compression
```

## Comparing `aily_code_sdk-0.1.0b5.tar` & `aily_code_sdk-0.1.0b6.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0    10947 2024-05-29 05:58:44.305920 aily_code_sdk-0.1.0b5/LICENSE
--rw-r--r--   0        0        0     1134 2024-05-30 09:07:10.878909 aily_code_sdk-0.1.0b5/README.md
--rw-r--r--   0        0        0      547 2024-06-03 04:00:25.716316 aily_code_sdk-0.1.0b5/pyproject.toml
--rw-r--r--   0        0        0        0 2024-05-29 07:12:18.585377 aily_code_sdk-0.1.0b5/src/aily_code_sdk/__init__.py
--rw-r--r--   0        0        0        0 2024-05-16 05:24:43.434521 aily_code_sdk-0.1.0b5/src/aily_code_sdk/app.py
--rw-r--r--   0        0        0     1379 2024-05-30 06:32:18.557919 aily_code_sdk-0.1.0b5/src/aily_code_sdk/conversation.py
--rw-r--r--   0        0        0     1593 2024-05-31 06:55:16.269599 aily_code_sdk-0.1.0b5/src/aily_code_sdk/data.py
--rw-r--r--   0        0        0        0 2024-05-24 06:39:18.516015 aily_code_sdk-0.1.0b5/src/aily_code_sdk/integration/__init__.py
--rw-r--r--   0        0        0      440 2024-05-20 06:57:18.552870 aily_code_sdk-0.1.0b5/src/aily_code_sdk/integration/feishu.py
--rw-r--r--   0        0        0     2266 2024-06-03 04:02:21.287407 aily_code_sdk-0.1.0b5/src/aily_code_sdk/knowledge.py
--rw-r--r--   0        0        0     5158 2024-06-03 03:39:14.785567 aily_code_sdk-0.1.0b5/src/aily_code_sdk/llm.py
--rw-r--r--   0        0        0      607 2024-05-20 07:16:43.931725 aily_code_sdk-0.1.0b5/src/aily_code_sdk/skill.py
--rw-r--r--   0        0        0     1706 1970-01-01 00:00:00.000000 aily_code_sdk-0.1.0b5/PKG-INFO
+-rw-r--r--   0        0        0    10947 2024-05-29 05:58:44.305920 aily_code_sdk-0.1.0b6/LICENSE
+-rw-r--r--   0        0        0     1134 2024-05-30 09:07:10.878909 aily_code_sdk-0.1.0b6/README.md
+-rw-r--r--   0        0        0      571 2024-06-03 09:51:12.258438 aily_code_sdk-0.1.0b6/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-05-29 07:12:18.585377 aily_code_sdk-0.1.0b6/src/aily_code_sdk/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-16 05:24:43.434521 aily_code_sdk-0.1.0b6/src/aily_code_sdk/app.py
+-rw-r--r--   0        0        0     1379 2024-05-30 06:32:18.557919 aily_code_sdk-0.1.0b6/src/aily_code_sdk/conversation.py
+-rw-r--r--   0        0        0     1593 2024-05-31 06:55:16.269599 aily_code_sdk-0.1.0b6/src/aily_code_sdk/data.py
+-rw-r--r--   0        0        0        0 2024-05-24 06:39:18.516015 aily_code_sdk-0.1.0b6/src/aily_code_sdk/integration/__init__.py
+-rw-r--r--   0        0        0      440 2024-05-20 06:57:18.552870 aily_code_sdk-0.1.0b6/src/aily_code_sdk/integration/feishu.py
+-rw-r--r--   0        0        0     2266 2024-06-03 04:02:21.287407 aily_code_sdk-0.1.0b6/src/aily_code_sdk/knowledge.py
+-rw-r--r--   0        0        0     4444 2024-06-03 09:50:44.680838 aily_code_sdk-0.1.0b6/src/aily_code_sdk/llm.py
+-rw-r--r--   0        0        0      607 2024-05-20 07:16:43.931725 aily_code_sdk-0.1.0b6/src/aily_code_sdk/skill.py
+-rw-r--r--   0        0        0     1751 1970-01-01 00:00:00.000000 aily_code_sdk-0.1.0b6/PKG-INFO
```

### Comparing `aily_code_sdk-0.1.0b5/LICENSE` & `aily_code_sdk-0.1.0b6/LICENSE`

 * *Files identical despite different names*

### Comparing `aily_code_sdk-0.1.0b5/README.md` & `aily_code_sdk-0.1.0b6/README.md`

 * *Files identical despite different names*

### Comparing `aily_code_sdk-0.1.0b5/pyproject.toml` & `aily_code_sdk-0.1.0b6/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 [tool.poetry]
 name = "aily-code-sdk"
 description = "Aily Code SDK"
-version = "0.1.0-beta.5"
+version = "0.1.0-beta.6"
 authors = [
     "lijiuyang.5137 <lijiuyang.5137@bytedance.com>",
     "zhaolizi.milo <zhaolizi.milo@bytedance.com>"
 ]
 readme = "README.md"
 packages = [{ include = "aily_code_sdk", from = "src" }]
 classifiers = [
     "License :: OSI Approved :: Apache Software License",
 ]
 
 
 [tool.poetry.dependencies]
 python = "^3.8.1"
-aily-code-sdk-core = "0.1.0b5"
+aily-code-sdk-core = "0.1.0-beta.6"
 pydantic = "^2.7.2"
+openai = "^1.30.5"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `aily_code_sdk-0.1.0b5/src/aily_code_sdk/conversation.py` & `aily_code_sdk-0.1.0b6/src/aily_code_sdk/conversation.py`

 * *Files identical despite different names*

### Comparing `aily_code_sdk-0.1.0b5/src/aily_code_sdk/data.py` & `aily_code_sdk-0.1.0b6/src/aily_code_sdk/data.py`

 * *Files identical despite different names*

### Comparing `aily_code_sdk-0.1.0b5/src/aily_code_sdk/knowledge.py` & `aily_code_sdk-0.1.0b6/src/aily_code_sdk/knowledge.py`

 * *Files identical despite different names*

### Comparing `aily_code_sdk-0.1.0b5/src/aily_code_sdk/llm.py` & `aily_code_sdk-0.1.0b6/src/aily_code_sdk/llm.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,59 +1,62 @@
-from enum import Enum
-from typing import List, Union, Literal, Optional, Dict
+import json
+from typing import List, Union, Literal, Optional, Dict, Iterable
 
+from openai.types.chat import ChatCompletionMessageParam, ChatCompletionToolParam, ChatCompletionToolChoiceOptionParam
 from pydantic import BaseModel
 
 from aily_code_sdk_core import action
 
 ACTION_API_NAME = 'action:brn:cn:spring:all:all:connector_action_runtime:/spring_sdk_llm'
 
 
-class LLMModel(Enum):
-    BYOM_PRO = "BYOM-pro"
-    BYOM_ULTRA = "BYOM-ultra"
-    FOUR_TURBO = "4-turbo"
-
-
 class Function(BaseModel):
-    name: str
-    description: str
-    parameters: Optional[str]
+    arguments: Optional[str] = None
+
+    name: Optional[str] = None
 
 
 class MessageToolCall(BaseModel):
     id: str
-    """The ID of the tool call."""
+
     function: Function
-    """The function that the model called."""
+
     type: Literal["function"]
-    """The type of the tool. Currently, only `function` is supported."""
 
 
 class Usage(BaseModel):
     input_tokens: int
-    """The number of input tokens which were used."""
 
     output_tokens: int
-    """The number of output tokens which were used."""
 
 
 class Message(BaseModel):
     content: Optional[str] = None
     role: Literal["assistant", "user", "system"]
-    """The role of the author of this message."""
-    # tool_calls: Optional[List[MessageToolCall]] = None
-    # """The tool calls generated by the model, such as function calls."""
-    # function_call: Optional[dict] = None
-    # """The function call generated by the model."""
+
+    tool_calls: Optional[List[MessageToolCall]] = None
+
     usage: Optional[Usage] = None
 
 
-def generate(
-        messages: Union[List[Message], List[Dict[str, str]]],
+def capitalize_keys_and_stringify_properties(tools):
+    new_tools = []
+    for tool in tools:
+        new_tool = {k.capitalize(): v for k, v in tool.items()}
+        if 'Function' in new_tool:
+            function = new_tool['Function']
+            function = {k.capitalize(): v for k, v in function.items()}
+            function['Parameters'] = json.dumps(function['Parameters'])
+            new_tool['Function'] = function
+        new_tools.append(new_tool)
+    return new_tools
+
+
+def chat_completion(
+        messages: Iterable[ChatCompletionMessageParam],
         model: Union[
             str,
             Literal[
                 "BYOM-lite",
                 "BYOM-plus",
                 "BYOM-pro",
                 "BYOM-max",
@@ -67,95 +70,77 @@
                 "4-Turbo",
                 "4o",
             ],
         ],
         max_tokens: Optional[int] = None,
         temperature: Optional[float] = None,
         # stream: bool = False,  # 当前并不支持
-        # tools: Optional[List[Function]] = None,
-        # tool_choice: Literal["none", "auto", "required"] = "none",
+        tools: Iterable[ChatCompletionToolParam] = None,
+        tool_choice: ChatCompletionToolChoiceOptionParam = "none",
         timeout: Optional[float] = None,
 ) -> Message:
     """
     Generates a response message based on the input messages and parameters.
 
     Args:
         messages: The list of input messages.
         model: The LLM model to use for generation.
         max_tokens: The maximum number of tokens to generate.
         temperature: The temperature value for generation.
         # stream: Whether to stream the response. Currently not supported.
-        # tools: The tools available for the model to use.
-        # tool_choice: The choice of tool usage. Can be "none", "auto", or "required".
+        tools: The tools available for the model to use.
+        tool_choice: The choice of tool usage. Can be "none", "auto", or "required".
         timeout: The timeout value for the API request.
 
     Returns:
         The generated response message.
     """
-    model_value = model.value if isinstance(model, LLMModel) else model
-    if isinstance(messages[0], dict):
-        messages = [Message(role=message["role"], content=message["content"]) for message in messages]
-
     action_data = {
-        "llmID": model_value,
+        "llmID": model,
         "chatCompletionParameters": {
             "ChatCompletionMessages": [
                 {
-                    "Role": message.role,
-                    "Content": message.content,
+                    "Role": message['role'],
+                    "Content": message['content'],
                 }
                 for message in messages
             ],
             "MaxTokens": max_tokens,
             "Temperature": temperature,
-            # "Stream": stream,
+            "Tools": capitalize_keys_and_stringify_properties(tools),
+            "ToolChoice": tool_choice,
         },
     }
 
-    # if tools:
-    #     action_data["chatCompletionParameters"]["FunctionDefinitions"] = [
-    #         {
-    #             "Name": tool.name,
-    #             "Description": tool.description,
-    #             "Parameters": tool.parameters,
-    #         }
-    #         for tool in tools
-    #     ]
-
-    # if tool_choice == "required":
-    #     action_data["chatCompletionParameters"]["FunctionCall"] = '{"name": "extract_entity_tool"}'
-    #     action_data["chatCompletionParameters"]["ToolChoice"] = tool_choice
-
     res = action.call_action(
         action_api_name=ACTION_API_NAME,
         action_data=action_data,
     )
-
     if res["Choices"]:
         choice = res["Choices"][0]
-        content = choice["Message"].get("Content")
-        role = choice["Message"]["Role"]
-        # function_call = choice["Message"].get("FunctionCall")
-        # tool_calls = [
-        #     MessageToolCall(
-        #         id=tool_call["ID"],
-        #         function=Function(
-        #             name=tool_call["Function"]["Name"],
-        #             parameters=tool_call["Function"]["Arguments"],
-        #             description=""
-        #         ),
-        #         type="function",
-        #     )
-        #     for tool_call in choice["Message"].get("ToolCalls", [])
-        # ]
+        message = choice["Message"]
+        content = message.get("Content")
+        role = message["Role"]
+        function_call = message.get("FunctionCall")
+        tool_calls = [
+            MessageToolCall(
+                id=tool_call["ID"],
+                function=Function(
+                    name=tool_call["Function"]["Name"],
+                    arguments=tool_call["Function"]["Arguments"],
+                ),
+                type="function",
+            )
+            for tool_call in message.get("ToolCalls", [])
+        ]
         return Message(
             content=content,
             role=role,
-            # function_call=function_call,
-            # tool_calls=tool_calls if tool_calls else None,
+            function_call=function_call,
+            tool_calls=tool_calls if tool_calls else None,
             usage=Usage(
                 input_tokens=res.get('Usage', {}).get('PromptTokens'),
                 output_tokens=res.get('Usage', {}).get('CompletionTokens'),
             )
         )
     else:
         return Message()
```

### Comparing `aily_code_sdk-0.1.0b5/src/aily_code_sdk/skill.py` & `aily_code_sdk-0.1.0b6/src/aily_code_sdk/skill.py`

 * *Files identical despite different names*

### Comparing `aily_code_sdk-0.1.0b5/PKG-INFO` & `aily_code_sdk-0.1.0b6/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 Metadata-Version: 2.1
 Name: aily-code-sdk
-Version: 0.1.0b5
+Version: 0.1.0b6
 Summary: Aily Code SDK
 Author: lijiuyang.5137
 Author-email: lijiuyang.5137@bytedance.com
 Requires-Python: >=3.8.1,<4.0.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: aily-code-sdk-core (==0.1.0b5)
+Requires-Dist: aily-code-sdk-core (==0.1.0-beta.6)
+Requires-Dist: openai (>=1.30.5,<2.0.0)
 Requires-Dist: pydantic (>=2.7.2,<3.0.0)
 Description-Content-Type: text/markdown
 
 # Aily Code SDK
 
 ## 调用LLM
 ```python
```

