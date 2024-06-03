# Comparing `tmp/aily_code_sdk-0.1.0b4.tar.gz` & `tmp/aily_code_sdk-0.1.0b5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aily_code_sdk-0.1.0b4.tar", max compression
+gzip compressed data, was "aily_code_sdk-0.1.0b5.tar", max compression
```

## Comparing `aily_code_sdk-0.1.0b4.tar` & `aily_code_sdk-0.1.0b5.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0    10947 2024-05-29 05:58:44.305920 aily_code_sdk-0.1.0b4/LICENSE
--rw-r--r--   0        0        0     1134 2024-05-30 09:07:10.878909 aily_code_sdk-0.1.0b4/README.md
--rw-r--r--   0        0        0      547 2024-06-03 03:42:19.946927 aily_code_sdk-0.1.0b4/pyproject.toml
--rw-r--r--   0        0        0        0 2024-05-29 07:12:18.585377 aily_code_sdk-0.1.0b4/src/aily_code_sdk/__init__.py
--rw-r--r--   0        0        0        0 2024-05-16 05:24:43.434521 aily_code_sdk-0.1.0b4/src/aily_code_sdk/app.py
--rw-r--r--   0        0        0     1379 2024-05-30 06:32:18.557919 aily_code_sdk-0.1.0b4/src/aily_code_sdk/conversation.py
--rw-r--r--   0        0        0     1593 2024-05-31 06:55:16.269599 aily_code_sdk-0.1.0b4/src/aily_code_sdk/data.py
--rw-r--r--   0        0        0        0 2024-05-24 06:39:18.516015 aily_code_sdk-0.1.0b4/src/aily_code_sdk/integration/__init__.py
--rw-r--r--   0        0        0      440 2024-05-20 06:57:18.552870 aily_code_sdk-0.1.0b4/src/aily_code_sdk/integration/feishu.py
--rw-r--r--   0        0        0     1662 2024-05-30 03:54:23.488815 aily_code_sdk-0.1.0b4/src/aily_code_sdk/knowledge.py
--rw-r--r--   0        0        0     5158 2024-06-03 03:39:14.785567 aily_code_sdk-0.1.0b4/src/aily_code_sdk/llm.py
--rw-r--r--   0        0        0      607 2024-05-20 07:16:43.931725 aily_code_sdk-0.1.0b4/src/aily_code_sdk/skill.py
--rw-r--r--   0        0        0     1706 1970-01-01 00:00:00.000000 aily_code_sdk-0.1.0b4/PKG-INFO
+-rw-r--r--   0        0        0    10947 2024-05-29 05:58:44.305920 aily_code_sdk-0.1.0b5/LICENSE
+-rw-r--r--   0        0        0     1134 2024-05-30 09:07:10.878909 aily_code_sdk-0.1.0b5/README.md
+-rw-r--r--   0        0        0      547 2024-06-03 04:00:25.716316 aily_code_sdk-0.1.0b5/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-05-29 07:12:18.585377 aily_code_sdk-0.1.0b5/src/aily_code_sdk/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-16 05:24:43.434521 aily_code_sdk-0.1.0b5/src/aily_code_sdk/app.py
+-rw-r--r--   0        0        0     1379 2024-05-30 06:32:18.557919 aily_code_sdk-0.1.0b5/src/aily_code_sdk/conversation.py
+-rw-r--r--   0        0        0     1593 2024-05-31 06:55:16.269599 aily_code_sdk-0.1.0b5/src/aily_code_sdk/data.py
+-rw-r--r--   0        0        0        0 2024-05-24 06:39:18.516015 aily_code_sdk-0.1.0b5/src/aily_code_sdk/integration/__init__.py
+-rw-r--r--   0        0        0      440 2024-05-20 06:57:18.552870 aily_code_sdk-0.1.0b5/src/aily_code_sdk/integration/feishu.py
+-rw-r--r--   0        0        0     2266 2024-06-03 04:02:21.287407 aily_code_sdk-0.1.0b5/src/aily_code_sdk/knowledge.py
+-rw-r--r--   0        0        0     5158 2024-06-03 03:39:14.785567 aily_code_sdk-0.1.0b5/src/aily_code_sdk/llm.py
+-rw-r--r--   0        0        0      607 2024-05-20 07:16:43.931725 aily_code_sdk-0.1.0b5/src/aily_code_sdk/skill.py
+-rw-r--r--   0        0        0     1706 1970-01-01 00:00:00.000000 aily_code_sdk-0.1.0b5/PKG-INFO
```

### Comparing `aily_code_sdk-0.1.0b4/LICENSE` & `aily_code_sdk-0.1.0b5/LICENSE`

 * *Files identical despite different names*

### Comparing `aily_code_sdk-0.1.0b4/README.md` & `aily_code_sdk-0.1.0b5/README.md`

 * *Files identical despite different names*

### Comparing `aily_code_sdk-0.1.0b4/pyproject.toml` & `aily_code_sdk-0.1.0b5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool.poetry]
 name = "aily-code-sdk"
 description = "Aily Code SDK"
-version = "0.1.0-beta.4"
+version = "0.1.0-beta.5"
 authors = [
     "lijiuyang.5137 <lijiuyang.5137@bytedance.com>",
     "zhaolizi.milo <zhaolizi.milo@bytedance.com>"
 ]
 readme = "README.md"
 packages = [{ include = "aily_code_sdk", from = "src" }]
 classifiers = [
```

### Comparing `aily_code_sdk-0.1.0b4/src/aily_code_sdk/conversation.py` & `aily_code_sdk-0.1.0b5/src/aily_code_sdk/conversation.py`

 * *Files identical despite different names*

### Comparing `aily_code_sdk-0.1.0b4/src/aily_code_sdk/data.py` & `aily_code_sdk-0.1.0b5/src/aily_code_sdk/data.py`

 * *Files identical despite different names*

### Comparing `aily_code_sdk-0.1.0b4/src/aily_code_sdk/llm.py` & `aily_code_sdk-0.1.0b5/src/aily_code_sdk/llm.py`

 * *Files identical despite different names*

### Comparing `aily_code_sdk-0.1.0b4/src/aily_code_sdk/skill.py` & `aily_code_sdk-0.1.0b5/src/aily_code_sdk/skill.py`

 * *Files identical despite different names*

### Comparing `aily_code_sdk-0.1.0b4/PKG-INFO` & `aily_code_sdk-0.1.0b5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aily-code-sdk
-Version: 0.1.0b4
+Version: 0.1.0b5
 Summary: Aily Code SDK
 Author: lijiuyang.5137
 Author-email: lijiuyang.5137@bytedance.com
 Requires-Python: >=3.8.1,<4.0.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
```

