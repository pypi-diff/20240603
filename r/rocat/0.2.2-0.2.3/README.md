# Comparing `tmp/rocat-0.2.2.tar.gz` & `tmp/rocat-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rocat-0.2.2.tar", last modified: Sun Jun  2 07:43:37 2024, max compression
+gzip compressed data, was "rocat-0.2.3.tar", last modified: Mon Jun  3 08:09:53 2024, max compression
```

## Comparing `rocat-0.2.2.tar` & `rocat-0.2.3.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxrwxrwx   0        0        0        0 2024-06-02 07:43:37.865668 rocat-0.2.2/
--rw-rw-rw-   0        0        0     1081 2024-05-28 06:15:40.000000 rocat-0.2.2/LICENSE
--rw-rw-rw-   0        0        0     4632 2024-06-02 07:43:37.865668 rocat-0.2.2/PKG-INFO
--rw-rw-rw-   0        0        0     3539 2024-06-02 06:45:57.000000 rocat-0.2.2/README.md
-drwxrwxrwx   0        0        0        0 2024-06-02 07:43:37.845735 rocat-0.2.2/rocat/
--rw-rw-rw-   0        0        0      753 2024-06-02 04:55:56.000000 rocat-0.2.2/rocat/__init__.py
--rw-rw-rw-   0        0        0     1162 2024-05-28 08:32:13.000000 rocat-0.2.2/rocat/__main__.py
--rw-rw-rw-   0        0        0     2449 2024-06-02 05:16:39.000000 rocat-0.2.2/rocat/ai_functions.py
--rw-rw-rw-   0        0        0      651 2024-06-02 06:01:19.000000 rocat-0.2.2/rocat/audio_utils.py
--rw-rw-rw-   0        0        0     2426 2024-06-02 04:57:35.000000 rocat-0.2.2/rocat/config.py
--rw-rw-rw-   0        0        0    11584 2024-06-02 07:35:00.000000 rocat-0.2.2/rocat/file_utils.py
--rw-rw-rw-   0        0        0     1482 2024-06-02 05:30:21.000000 rocat-0.2.2/rocat/image_utils.py
--rw-rw-rw-   0        0        0     5804 2024-06-02 05:14:37.000000 rocat-0.2.2/rocat/language_model.py
--rw-rw-rw-   0        0        0      838 2024-05-28 08:56:06.000000 rocat-0.2.2/rocat/language_utils.py
--rw-rw-rw-   0        0        0      480 2024-05-28 08:56:10.000000 rocat-0.2.2/rocat/main.py
--rw-rw-rw-   0        0        0      807 2024-05-28 08:56:11.000000 rocat-0.2.2/rocat/template_utils.py
--rw-rw-rw-   0        0        0     2215 2024-06-02 01:42:25.000000 rocat-0.2.2/rocat/web_utils.py
-drwxrwxrwx   0        0        0        0 2024-06-02 07:43:37.864672 rocat-0.2.2/rocat.egg-info/
--rw-rw-rw-   0        0        0     4632 2024-06-02 07:43:37.000000 rocat-0.2.2/rocat.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      629 2024-06-02 07:43:37.000000 rocat-0.2.2/rocat.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-06-02 07:43:37.000000 rocat-0.2.2/rocat.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       46 2024-06-02 07:43:37.000000 rocat-0.2.2/rocat.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      336 2024-06-02 07:43:37.000000 rocat-0.2.2/rocat.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2024-06-02 07:43:37.000000 rocat-0.2.2/rocat.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-06-02 07:43:37.866665 rocat-0.2.2/setup.cfg
--rw-rw-rw-   0        0        0     1518 2024-06-02 07:43:35.000000 rocat-0.2.2/setup.py
-drwxrwxrwx   0        0        0        0 2024-06-02 07:43:37.863675 rocat-0.2.2/tests/
--rw-rw-rw-   0        0        0     1988 2024-06-02 05:36:39.000000 rocat-0.2.2/tests/test_ai_functions.py
--rw-rw-rw-   0        0        0      934 2024-06-02 06:11:22.000000 rocat-0.2.2/tests/test_audio_utils.py
--rw-rw-rw-   0        0        0     4864 2024-06-02 06:45:29.000000 rocat-0.2.2/tests/test_file_utils.py
--rw-rw-rw-   0        0        0     1613 2024-06-02 05:38:40.000000 rocat-0.2.2/tests/test_image_utils.py
--rw-rw-rw-   0        0        0     1392 2024-06-02 05:39:16.000000 rocat-0.2.2/tests/test_language_model.py
--rw-rw-rw-   0        0        0      640 2024-06-02 05:39:27.000000 rocat-0.2.2/tests/test_template_utils.py
--rw-rw-rw-   0        0        0     1543 2024-06-02 06:10:32.000000 rocat-0.2.2/tests/test_web_utils.py
+drwxrwxrwx   0        0        0        0 2024-06-03 08:09:53.635848 rocat-0.2.3/
+-rw-rw-rw-   0        0        0     1081 2024-06-03 07:14:31.000000 rocat-0.2.3/LICENSE
+-rw-rw-rw-   0        0        0     4632 2024-06-03 08:09:53.629794 rocat-0.2.3/PKG-INFO
+-rw-rw-rw-   0        0        0     3539 2024-06-03 07:17:12.000000 rocat-0.2.3/README.md
+drwxrwxrwx   0        0        0        0 2024-06-03 08:09:53.603882 rocat-0.2.3/rocat/
+-rw-rw-rw-   0        0        0      753 2024-06-03 07:17:12.000000 rocat-0.2.3/rocat/__init__.py
+-rw-rw-rw-   0        0        0     1162 2024-06-03 07:17:12.000000 rocat-0.2.3/rocat/__main__.py
+-rw-rw-rw-   0        0        0     2449 2024-06-03 07:17:12.000000 rocat-0.2.3/rocat/ai_functions.py
+-rw-rw-rw-   0        0        0      651 2024-06-03 07:17:12.000000 rocat-0.2.3/rocat/audio_utils.py
+-rw-rw-rw-   0        0        0     2426 2024-06-03 07:17:12.000000 rocat-0.2.3/rocat/config.py
+-rw-rw-rw-   0        0        0    11584 2024-06-03 07:17:12.000000 rocat-0.2.3/rocat/file_utils.py
+-rw-rw-rw-   0        0        0     1482 2024-06-03 07:17:12.000000 rocat-0.2.3/rocat/image_utils.py
+-rw-rw-rw-   0        0        0     6846 2024-06-03 08:03:14.000000 rocat-0.2.3/rocat/language_model.py
+-rw-rw-rw-   0        0        0      838 2024-06-03 07:17:12.000000 rocat-0.2.3/rocat/language_utils.py
+-rw-rw-rw-   0        0        0      480 2024-06-03 07:17:12.000000 rocat-0.2.3/rocat/main.py
+-rw-rw-rw-   0        0        0      807 2024-06-03 07:17:12.000000 rocat-0.2.3/rocat/template_utils.py
+-rw-rw-rw-   0        0        0     2215 2024-06-03 07:17:12.000000 rocat-0.2.3/rocat/web_utils.py
+drwxrwxrwx   0        0        0        0 2024-06-03 08:09:53.629794 rocat-0.2.3/rocat.egg-info/
+-rw-rw-rw-   0        0        0     4632 2024-06-03 08:09:53.000000 rocat-0.2.3/rocat.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      629 2024-06-03 08:09:53.000000 rocat-0.2.3/rocat.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-06-03 08:09:53.000000 rocat-0.2.3/rocat.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       46 2024-06-03 08:09:53.000000 rocat-0.2.3/rocat.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      336 2024-06-03 08:09:53.000000 rocat-0.2.3/rocat.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2024-06-03 08:09:53.000000 rocat-0.2.3/rocat.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-06-03 08:09:53.635848 rocat-0.2.3/setup.cfg
+-rw-rw-rw-   0        0        0     1518 2024-06-03 08:06:14.000000 rocat-0.2.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-06-03 08:09:53.629794 rocat-0.2.3/tests/
+-rw-rw-rw-   0        0        0     1988 2024-06-03 07:17:12.000000 rocat-0.2.3/tests/test_ai_functions.py
+-rw-rw-rw-   0        0        0      934 2024-06-03 07:17:12.000000 rocat-0.2.3/tests/test_audio_utils.py
+-rw-rw-rw-   0        0        0     4864 2024-06-03 07:17:12.000000 rocat-0.2.3/tests/test_file_utils.py
+-rw-rw-rw-   0        0        0     1613 2024-06-03 07:17:12.000000 rocat-0.2.3/tests/test_image_utils.py
+-rw-rw-rw-   0        0        0     1990 2024-06-03 07:37:38.000000 rocat-0.2.3/tests/test_language_model.py
+-rw-rw-rw-   0        0        0      640 2024-06-03 07:17:12.000000 rocat-0.2.3/tests/test_template_utils.py
+-rw-rw-rw-   0        0        0     1543 2024-06-03 07:17:12.000000 rocat-0.2.3/tests/test_web_utils.py
```

### Comparing `rocat-0.2.2/LICENSE` & `rocat-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `rocat-0.2.2/PKG-INFO` & `rocat-0.2.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rocat
-Version: 0.2.2
+Version: 0.2.3
 Summary: A simple and user-friendly library for AI services
 Home-page: https://github.com/Yumeta-Lab/rocat-dev
 Author: YumetaLab
 Author-email: root@yumeta.kr
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `rocat-0.2.2/README.md` & `rocat-0.2.3/README.md`

 * *Files identical despite different names*

### Comparing `rocat-0.2.2/rocat/__init__.py` & `rocat-0.2.3/rocat/__init__.py`

 * *Files identical despite different names*

### Comparing `rocat-0.2.2/rocat/__main__.py` & `rocat-0.2.3/rocat/__main__.py`

 * *Files identical despite different names*

### Comparing `rocat-0.2.2/rocat/ai_functions.py` & `rocat-0.2.3/rocat/ai_functions.py`

 * *Files identical despite different names*

### Comparing `rocat-0.2.2/rocat/audio_utils.py` & `rocat-0.2.3/rocat/audio_utils.py`

 * *Files identical despite different names*

### Comparing `rocat-0.2.2/rocat/config.py` & `rocat-0.2.3/rocat/config.py`

 * *Files identical despite different names*

### Comparing `rocat-0.2.2/rocat/file_utils.py` & `rocat-0.2.3/rocat/file_utils.py`

 * *Files identical despite different names*

### Comparing `rocat-0.2.2/rocat/image_utils.py` & `rocat-0.2.3/rocat/image_utils.py`

 * *Files identical despite different names*

### Comparing `rocat-0.2.2/rocat/language_model.py` & `rocat-0.2.3/rocat/language_model.py`

 * *Files 12% similar despite different names*

```diff
@@ -13,66 +13,81 @@
     "gpt4o": "gpt-4o",
     "opus": "claude-3-opus-20240229",
     "haiku": "claude-3-haiku-20240307",
     "sonnet": "claude-3-sonnet-20240229",
     "clova": "HCX-003"
 }
 
-def run_model(model, prompt, system_prompt="", temperature=0.7, top_p=1, max_tokens=1024, output="default", lang="", tools=[]):
+def run_model(model, prompt, system_prompt="", temperature=0.7, top_p=1, max_tokens=1024, output="default", lang="", tools=[], stream=False):
     """
     주어진 모델을 사용하여 프롬프트에 대한 응답을 생성합니다.
     
     Parameters:
         model (str): 사용할 모델의 이름.
         prompt (str): 모델에 입력할 프롬프트.
         system_prompt (str): 시스템 프롬프트, 대화의 맥락을 설정하는 데 사용됩니다 (옵션).
         temperature (float): 생성의 무작위성을 결정하는 값.
         top_p (float): 토큰 확률의 누적 분포 임곗값.
         max_tokens (int): 생성할 최대 토큰 수.
         output (str): 응답의 출력 형식 (default, word, sentence, bullet, json).
         lang (str): 응답 언어 코드 (ISO 639-1).
         tools (list): 사용할 도구 목록.
+        stream (bool): 스트림 모드 사용 여부 (기본값: False).
     
     Returns:
-        str: 생성된 텍스트 응답.
+        str: 생성된 텍스트 응답 (stream=False인 경우).
+        generator: 텍스트를 스트리밍하는 제너레이터 (stream=True인 경우).
     """
     full_model_name = MODEL_MAP.get(model.lower())
     if not full_model_name:
         raise ValueError(f"Unknown model: {model}")
     
     if "gpt" in model.lower():
-        return _run_openai(full_model_name, prompt, system_prompt, temperature, top_p, max_tokens)
+        return _run_openai(full_model_name, prompt, system_prompt, temperature, top_p, max_tokens, stream)
     elif "claude" in full_model_name or "opus" in full_model_name or "haiku" in full_model_name or "sonnet" in full_model_name:
-        return _run_anthropic(full_model_name, prompt, system_prompt, temperature, top_p, max_tokens, output, lang, tools)
+        return _run_anthropic(full_model_name, prompt, system_prompt, temperature, top_p, max_tokens, output, lang, tools, stream)
     elif "clova" in model.lower():
         return _run_clova(full_model_name, prompt, temperature, top_p, max_tokens)
     else:
         raise ValueError(f"Unknown model: {model}")
 
-def _run_openai(model, prompt, system_prompt="", temperature=0.7, top_p=1, max_tokens=1024):
+def _run_openai(model, prompt, system_prompt="", temperature=0.7, top_p=1, max_tokens=1024, stream=False):
     key = get_api_key("openai")
     client = OpenAI(api_key=key)
     
     messages = [{"role": "system", "content": system_prompt}] if system_prompt else []
     
     if isinstance(prompt, str):
         prompt = [prompt]
     
     for p in prompt:
         messages.append({"role": "user", "content": p})
     
-    response = client.chat.completions.create(
-        model=model,
-        messages=messages,
-        max_tokens=max_tokens
-    )
-    
-    return response.choices[0].message.content
+    if stream:
+        response = client.chat.completions.create(
+            model=model,
+            messages=messages,
+            max_tokens=max_tokens,
+            stream=True
+        )
+        for chunk in response:
+            if chunk.choices[0].delta.content is not None:
+                yield chunk.choices[0].delta.content
+    else:
+        response = client.chat.completions.create(
+            model=model,
+            messages=messages,
+            max_tokens=max_tokens
+        )
+        return response.choices[0].message.content
+
 
-def _run_anthropic(model_name, prompt, system_prompt="", temperature=0.7, top_p=1, max_tokens=1024, output="default", lang="", tools=[]):
+
+
+def _run_anthropic(model_name, prompt, system_prompt="", temperature=0.7, top_p=1, max_tokens=1024, output="default", lang="", tools=[], stream=False):
     key = get_api_key("anthropic")
     anth_client = anthropic.Anthropic(api_key=key)
     output_format = {
         "default": "",
         "word": " Don't explain, keep your output to very short one word.",
         "sentence": " Keep your output to very short one sentence.",
         "bullet": " Don't explain, keep your output in bullet points. Don't say anything else.",
@@ -90,23 +105,36 @@
     
     if isinstance(prompt, str):
         prompt = [prompt]
     for user_message in prompt:
         messages.append({"role": "user", "content": user_message})
 
     if not tools:
-        response = anth_client.messages.create(
-            model=model_name,
-            max_tokens=max_tokens,
-            messages=messages,
-            temperature=temperature,
-            top_p=top_p
-        )
-        content = response.content
-        return "\n".join([block.text for block in content if hasattr(block, 'text')])
+        if stream:
+            with anth_client.messages.stream(
+                model=model_name,
+                max_tokens=max_tokens,
+                messages=messages,
+                temperature=temperature,
+                top_p=top_p,
+            ) as stream:
+                for text in stream.text_stream:
+                    yield text
+        else:
+            response = anth_client.messages.create(
+                model=model_name,
+                max_tokens=max_tokens,
+                messages=messages,
+                temperature=temperature,
+                top_p=top_p
+            )
+            content = response.content
+            return "\n".join([block.text for block in content if hasattr(block, 'text')])
+
+
 
 def _run_clova(model, prompt, temperature=0.7, top_p=0.8, max_tokens=256):
     host = 'https://clovastudio.stream.ntruss.com'
     
     api_key = get_api_key("naver_clovastudio")
     api_key_primary_val = get_api_key("naver_apigw")
```

### Comparing `rocat-0.2.2/rocat/language_utils.py` & `rocat-0.2.3/rocat/language_utils.py`

 * *Files identical despite different names*

### Comparing `rocat-0.2.2/rocat/template_utils.py` & `rocat-0.2.3/rocat/template_utils.py`

 * *Files identical despite different names*

### Comparing `rocat-0.2.2/rocat/web_utils.py` & `rocat-0.2.3/rocat/web_utils.py`

 * *Files identical despite different names*

### Comparing `rocat-0.2.2/rocat.egg-info/PKG-INFO` & `rocat-0.2.3/rocat.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rocat
-Version: 0.2.2
+Version: 0.2.3
 Summary: A simple and user-friendly library for AI services
 Home-page: https://github.com/Yumeta-Lab/rocat-dev
 Author: YumetaLab
 Author-email: root@yumeta.kr
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `rocat-0.2.2/rocat.egg-info/SOURCES.txt` & `rocat-0.2.3/rocat.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `rocat-0.2.2/setup.py` & `rocat-0.2.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name="rocat",
-    version="0.2.2",
+    version="0.2.3",
     description="A simple and user-friendly library for AI services",
     long_description=long_description,
     long_description_content_type="text/markdown",
     author="YumetaLab",
     author_email="root@yumeta.kr",
     url="https://github.com/Yumeta-Lab/rocat-dev",
     packages=find_packages(exclude=["tests"]),
```

### Comparing `rocat-0.2.2/tests/test_ai_functions.py` & `rocat-0.2.3/tests/test_ai_functions.py`

 * *Files identical despite different names*

### Comparing `rocat-0.2.2/tests/test_audio_utils.py` & `rocat-0.2.3/tests/test_audio_utils.py`

 * *Files identical despite different names*

### Comparing `rocat-0.2.2/tests/test_file_utils.py` & `rocat-0.2.3/tests/test_file_utils.py`

 * *Files identical despite different names*

### Comparing `rocat-0.2.2/tests/test_image_utils.py` & `rocat-0.2.3/tests/test_image_utils.py`

 * *Files identical despite different names*

### Comparing `rocat-0.2.2/tests/test_language_model.py` & `rocat-0.2.3/tests/test_language_model.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,30 +1,42 @@
-#tests/test_language_model.py   
-
+# tests/test_language_model.py
 import pytest
 from rocat.language_model import run_model
 from unittest.mock import patch, MagicMock
 
-@pytest.mark.parametrize("model, prompt, expected_response", [
-    ("gpt3", "Tell me a joke", "This is a joke."),
-    ("gpt4o", "What is the capital of France?", "The capital of France is Paris."),
-    ("opus", "Write a short poem about the moon", "This is a short poem about the moon."),
-    ("haiku", "Write a haiku about the ocean", "This is a haiku about the ocean."),
-    ("sonnet", "Write a sonnet about love", "This is a sonnet about love."),
-    ("clova", "Summarize the benefits of exercise in one sentence", "Exercise improves health.")
+@pytest.mark.parametrize("model, prompt, expected_response, stream", [
+    ("gpt3", "Tell me a joke", "This is a joke.", False),
+    ("gpt4o", "What is the capital of France?", "The capital of France is Paris.", False),
+    ("opus", "Write a short poem about the moon", "This is a short poem about the moon.", False),
+    ("haiku", "Write a haiku about the ocean", "This is a haiku about the ocean.", False),
+    ("sonnet", "Write a sonnet about love", "This is a sonnet about love.", False),
+    ("clova", "Summarize the benefits of exercise in one sentence", "Exercise improves health.", False),
+    ("gpt3", "Tell me a story", "Once upon a time...", True),
+    ("opus", "Describe a beautiful landscape", "The sun rises over the mountains...", True)
 ])
 @patch('rocat.language_model._run_openai')
 @patch('rocat.language_model._run_anthropic')
 @patch('rocat.language_model._run_clova')
-def test_run_model(mock_run_clova, mock_run_anthropic, mock_run_openai, model, prompt, expected_response):
+def test_run_model(mock_run_clova, mock_run_anthropic, mock_run_openai, model, prompt, expected_response, stream):
     if "gpt" in model:
-        mock_run_openai.return_value = expected_response
+        if stream:
+            mock_run_openai.return_value = (chunk for chunk in expected_response)
+        else:
+            mock_run_openai.return_value = expected_response
     elif "claude" in model or "opus" in model or "haiku" in model or "sonnet" in model:
-        mock_run_anthropic.return_value = expected_response
+        if stream:
+            mock_run_anthropic.return_value = (chunk for chunk in expected_response)
+        else:
+            mock_run_anthropic.return_value = expected_response
     elif "clova" in model:
         mock_run_clova.return_value = expected_response
 
-    response = run_model(model, prompt)
-    assert response == expected_response
+    response = run_model(model, prompt, stream=stream)
+
+    if stream:
+        response_text = "".join(response)
+        assert response_text == expected_response
+    else:
+        assert response == expected_response
 
 if __name__ == "__main__":
-    pytest.main()
+    pytest.main()
```

### Comparing `rocat-0.2.2/tests/test_template_utils.py` & `rocat-0.2.3/tests/test_template_utils.py`

 * *Files identical despite different names*

### Comparing `rocat-0.2.2/tests/test_web_utils.py` & `rocat-0.2.3/tests/test_web_utils.py`

 * *Files identical despite different names*

