# Comparing `tmp/literalai-0.0.604.tar.gz` & `tmp/literalai-0.0.605.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "literalai-0.0.604.tar", last modified: Wed May 29 10:57:43 2024, max compression
+gzip compressed data, was "literalai-0.0.605.tar", last modified: Mon Jun  3 13:31:35 2024, max compression
```

## Comparing `literalai-0.0.604.tar` & `literalai-0.0.605.tar`

### file list

```diff
@@ -1,51 +1,51 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 10:57:43.860548 literalai-0.0.604/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-29 10:57:34.000000 literalai-0.0.604/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      239 2024-05-29 10:57:43.860548 literalai-0.0.604/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      882 2024-05-29 10:57:34.000000 literalai-0.0.604/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 10:57:43.856548 literalai-0.0.604/literalai/
--rw-r--r--   0 runner    (1001) docker     (127)      421 2024-05-29 10:57:34.000000 literalai-0.0.604/literalai/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 10:57:43.860548 literalai-0.0.604/literalai/api/
--rw-r--r--   0 runner    (1001) docker     (127)    86700 2024-05-29 10:57:34.000000 literalai-0.0.604/literalai/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2849 2024-05-29 10:57:34.000000 literalai-0.0.604/literalai/api/attachment_helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)     5717 2024-05-29 10:57:34.000000 literalai-0.0.604/literalai/api/dataset_helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)     1613 2024-05-29 10:57:34.000000 literalai-0.0.604/literalai/api/generation_helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)    21202 2024-05-29 10:57:34.000000 literalai-0.0.604/literalai/api/gql.py
--rw-r--r--   0 runner    (1001) docker     (127)     2162 2024-05-29 10:57:34.000000 literalai-0.0.604/literalai/api/prompt_helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)     4210 2024-05-29 10:57:34.000000 literalai-0.0.604/literalai/api/score_helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)     3724 2024-05-29 10:57:34.000000 literalai-0.0.604/literalai/api/step_helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)     5028 2024-05-29 10:57:34.000000 literalai-0.0.604/literalai/api/thread_helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)     2689 2024-05-29 10:57:34.000000 literalai-0.0.604/literalai/api/user_helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 10:57:43.860548 literalai-0.0.604/literalai/callback/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 10:57:34.000000 literalai-0.0.604/literalai/callback/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    17193 2024-05-29 10:57:34.000000 literalai-0.0.604/literalai/callback/langchain_callback.py
--rw-r--r--   0 runner    (1001) docker     (127)     8446 2024-05-29 10:57:34.000000 literalai-0.0.604/literalai/callback/llama_index_callback.py
--rw-r--r--   0 runner    (1001) docker     (127)     7122 2024-05-29 10:57:34.000000 literalai-0.0.604/literalai/client.py
--rw-r--r--   0 runner    (1001) docker     (127)      334 2024-05-29 10:57:34.000000 literalai-0.0.604/literalai/context.py
--rw-r--r--   0 runner    (1001) docker     (127)     5618 2024-05-29 10:57:34.000000 literalai-0.0.604/literalai/dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)     3593 2024-05-29 10:57:34.000000 literalai-0.0.604/literalai/dataset_experiment.py
--rw-r--r--   0 runner    (1001) docker     (127)     1430 2024-05-29 10:57:34.000000 literalai-0.0.604/literalai/dataset_item.py
--rw-r--r--   0 runner    (1001) docker     (127)     3119 2024-05-29 10:57:34.000000 literalai-0.0.604/literalai/event_processor.py
--rw-r--r--   0 runner    (1001) docker     (127)     2724 2024-05-29 10:57:34.000000 literalai-0.0.604/literalai/filter.py
--rw-r--r--   0 runner    (1001) docker     (127)     1228 2024-05-29 10:57:34.000000 literalai-0.0.604/literalai/helper.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 10:57:43.860548 literalai-0.0.604/literalai/instrumentation/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 10:57:34.000000 literalai-0.0.604/literalai/instrumentation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    18454 2024-05-29 10:57:34.000000 literalai-0.0.604/literalai/instrumentation/openai.py
--rw-r--r--   0 runner    (1001) docker     (127)     4494 2024-05-29 10:57:34.000000 literalai-0.0.604/literalai/message.py
--rw-r--r--   0 runner    (1001) docker     (127)    12560 2024-05-29 10:57:34.000000 literalai-0.0.604/literalai/my_types.py
--rw-r--r--   0 runner    (1001) docker     (127)     8852 2024-05-29 10:57:34.000000 literalai-0.0.604/literalai/prompt.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 10:57:34.000000 literalai-0.0.604/literalai/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)      847 2024-05-29 10:57:34.000000 literalai-0.0.604/literalai/requirements.py
--rw-r--r--   0 runner    (1001) docker     (127)    10028 2024-05-29 10:57:34.000000 literalai-0.0.604/literalai/step.py
--rw-r--r--   0 runner    (1001) docker     (127)     6020 2024-05-29 10:57:34.000000 literalai-0.0.604/literalai/thread.py
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-29 10:57:34.000000 literalai-0.0.604/literalai/version.py
--rw-r--r--   0 runner    (1001) docker     (127)     4708 2024-05-29 10:57:34.000000 literalai-0.0.604/literalai/wrappers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 10:57:43.856548 literalai-0.0.604/literalai.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      239 2024-05-29 10:57:43.000000 literalai-0.0.604/literalai.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1104 2024-05-29 10:57:43.000000 literalai-0.0.604/literalai.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-29 10:57:43.000000 literalai-0.0.604/literalai.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       61 2024-05-29 10:57:43.000000 literalai-0.0.604/literalai.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-29 10:57:43.000000 literalai-0.0.604/literalai.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-29 10:57:43.860548 literalai-0.0.604/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      478 2024-05-29 10:57:34.000000 literalai-0.0.604/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 10:57:43.860548 literalai-0.0.604/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 10:57:34.000000 literalai-0.0.604/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 13:31:35.654740 literalai-0.0.605/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-06-03 13:31:22.000000 literalai-0.0.605/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      239 2024-06-03 13:31:35.654740 literalai-0.0.605/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      882 2024-06-03 13:31:22.000000 literalai-0.0.605/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 13:31:35.650740 literalai-0.0.605/literalai/
+-rw-r--r--   0 runner    (1001) docker     (127)      421 2024-06-03 13:31:22.000000 literalai-0.0.605/literalai/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 13:31:35.654740 literalai-0.0.605/literalai/api/
+-rw-r--r--   0 runner    (1001) docker     (127)    86868 2024-06-03 13:31:22.000000 literalai-0.0.605/literalai/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2849 2024-06-03 13:31:22.000000 literalai-0.0.605/literalai/api/attachment_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5717 2024-06-03 13:31:22.000000 literalai-0.0.605/literalai/api/dataset_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1613 2024-06-03 13:31:22.000000 literalai-0.0.605/literalai/api/generation_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21202 2024-06-03 13:31:22.000000 literalai-0.0.605/literalai/api/gql.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2162 2024-06-03 13:31:22.000000 literalai-0.0.605/literalai/api/prompt_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4210 2024-06-03 13:31:22.000000 literalai-0.0.605/literalai/api/score_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3724 2024-06-03 13:31:22.000000 literalai-0.0.605/literalai/api/step_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5028 2024-06-03 13:31:22.000000 literalai-0.0.605/literalai/api/thread_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2689 2024-06-03 13:31:22.000000 literalai-0.0.605/literalai/api/user_helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 13:31:35.654740 literalai-0.0.605/literalai/callback/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 13:31:22.000000 literalai-0.0.605/literalai/callback/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17193 2024-06-03 13:31:22.000000 literalai-0.0.605/literalai/callback/langchain_callback.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8446 2024-06-03 13:31:22.000000 literalai-0.0.605/literalai/callback/llama_index_callback.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7122 2024-06-03 13:31:22.000000 literalai-0.0.605/literalai/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)      334 2024-06-03 13:31:22.000000 literalai-0.0.605/literalai/context.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5618 2024-06-03 13:31:22.000000 literalai-0.0.605/literalai/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3593 2024-06-03 13:31:22.000000 literalai-0.0.605/literalai/dataset_experiment.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1430 2024-06-03 13:31:22.000000 literalai-0.0.605/literalai/dataset_item.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3119 2024-06-03 13:31:22.000000 literalai-0.0.605/literalai/event_processor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2724 2024-06-03 13:31:22.000000 literalai-0.0.605/literalai/filter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1228 2024-06-03 13:31:22.000000 literalai-0.0.605/literalai/helper.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 13:31:35.654740 literalai-0.0.605/literalai/instrumentation/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 13:31:22.000000 literalai-0.0.605/literalai/instrumentation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18454 2024-06-03 13:31:22.000000 literalai-0.0.605/literalai/instrumentation/openai.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4494 2024-06-03 13:31:22.000000 literalai-0.0.605/literalai/message.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12560 2024-06-03 13:31:22.000000 literalai-0.0.605/literalai/my_types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8852 2024-06-03 13:31:22.000000 literalai-0.0.605/literalai/prompt.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 13:31:22.000000 literalai-0.0.605/literalai/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)      847 2024-06-03 13:31:22.000000 literalai-0.0.605/literalai/requirements.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10028 2024-06-03 13:31:22.000000 literalai-0.0.605/literalai/step.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6020 2024-06-03 13:31:22.000000 literalai-0.0.605/literalai/thread.py
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-06-03 13:31:22.000000 literalai-0.0.605/literalai/version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4708 2024-06-03 13:31:22.000000 literalai-0.0.605/literalai/wrappers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 13:31:35.654740 literalai-0.0.605/literalai.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      239 2024-06-03 13:31:34.000000 literalai-0.0.605/literalai.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1104 2024-06-03 13:31:35.000000 literalai-0.0.605/literalai.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-03 13:31:34.000000 literalai-0.0.605/literalai.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       61 2024-06-03 13:31:34.000000 literalai-0.0.605/literalai.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-06-03 13:31:34.000000 literalai-0.0.605/literalai.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-06-03 13:31:35.654740 literalai-0.0.605/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      478 2024-06-03 13:31:22.000000 literalai-0.0.605/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 13:31:35.654740 literalai-0.0.605/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 13:31:22.000000 literalai-0.0.605/tests/__init__.py
```

### Comparing `literalai-0.0.604/LICENSE` & `literalai-0.0.605/LICENSE`

 * *Files identical despite different names*

### Comparing `literalai-0.0.604/README.md` & `literalai-0.0.605/README.md`

 * *Files identical despite different names*

### Comparing `literalai-0.0.604/literalai/api/__init__.py` & `literalai-0.0.605/literalai/api/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -178,15 +178,15 @@
         """
 
         def raise_error(error):
             logger.error(f"Failed to {description}: {error}")
             raise Exception(error)
 
         variables = self._prepare_variables(variables)
-        with httpx.Client() as client:
+        with httpx.Client(follow_redirects=True) as client:
             response = client.post(
                 self.graphql_endpoint,
                 json={"query": query, "variables": variables},
                 headers=self.headers,
                 timeout=10,
             )
 
@@ -221,15 +221,15 @@
         Args:
             subpath (str): The subpath of the REST API endpoint.
             body (Dict[str, Any]): The JSON body to send with the POST request.
 
         Returns:
             Dict: The JSON response from the REST API endpoint.
         """
-        with httpx.Client() as client:
+        with httpx.Client(follow_redirects=True) as client:
             response = client.post(
                 self.rest_endpoint + subpath,
                 json=body,
                 headers=self.headers,
                 timeout=20,
             )
 
@@ -639,15 +639,15 @@
         id = str(uuid.uuid4())
         body = {"fileName": id, "contentType": mime}
         if thread_id:
             body["threadId"] = thread_id
 
         path = "/api/upload/file"
 
-        with httpx.Client() as client:
+        with httpx.Client(follow_redirects=True) as client:
             response = client.post(
                 f"{self.url}{path}",
                 json=body,
                 headers=self.headers,
             )
             if response.status_code >= 400:
                 reason = response.text
@@ -675,15 +675,15 @@
         for field_name, field_value in fields.items():
             form_data[field_name] = (None, field_value)
 
         # Add file to the form_data
         # Note: The content_type parameter is not needed here, as the correct MIME type should be set in the 'Content-Type' field from upload_details
         form_data["file"] = (id, content, mime)
 
-        with httpx.Client() as client:
+        with httpx.Client(follow_redirects=True) as client:
             if upload_type == "raw":
                 upload_response = client.request(
                     url=url,
                     headers=headers,
                     method=method,
                     data=content,  # type: ignore
                 )
@@ -1360,15 +1360,15 @@
 
         def raise_error(error):
             logger.error(f"Failed to {description}: {error}")
             raise Exception(error)
 
         variables = self._prepare_variables(variables)
 
-        async with httpx.AsyncClient() as client:
+        async with httpx.AsyncClient(follow_redirects=True) as client:
             response = await client.post(
                 self.graphql_endpoint,
                 json={"query": query, "variables": variables},
                 headers=self.headers,
                 timeout=10,
             )
 
@@ -1403,15 +1403,15 @@
         Args:
             subpath (str): The endpoint subpath to which the POST request is made.
             body (Dict[str, Any]): The JSON body of the POST request.
 
         Returns:
             Dict: The JSON response from the REST API endpoint.
         """
-        async with httpx.AsyncClient() as client:
+        async with httpx.AsyncClient(follow_redirects=True) as client:
             response = await client.post(
                 self.rest_endpoint + subpath,
                 json=body,
                 headers=self.headers,
                 timeout=20,
             )
 
@@ -1848,15 +1848,15 @@
             A dictionary containing the object key and URL of the uploaded file.
         """
         id = str(uuid.uuid4())
         body = {"fileName": id, "contentType": mime, "threadId": thread_id}
 
         path = "/api/upload/file"
 
-        async with httpx.AsyncClient() as client:
+        async with httpx.AsyncClient(follow_redirects=True) as client:
             response = await client.post(
                 f"{self.url}{path}",
                 json=body,
                 headers=self.headers,
             )
             if response.status_code >= 400:
                 reason = response.text
@@ -1884,15 +1884,15 @@
         for field_name, field_value in fields.items():
             form_data[field_name] = (None, field_value)
 
         # Add file to the form_data
         # Note: The content_type parameter is not needed here, as the correct MIME type should be set in the 'Content-Type' field from upload_details
         form_data["file"] = (id, content, mime)
 
-        async with httpx.AsyncClient() as client:
+        async with httpx.AsyncClient(follow_redirects=True) as client:
             if upload_type == "raw":
                 upload_response = await client.request(
                     url=url,
                     headers=headers,
                     method=method,
                     data=content,  # type: ignore
                 )
```

### Comparing `literalai-0.0.604/literalai/api/attachment_helpers.py` & `literalai-0.0.605/literalai/api/attachment_helpers.py`

 * *Files identical despite different names*

### Comparing `literalai-0.0.604/literalai/api/dataset_helpers.py` & `literalai-0.0.605/literalai/api/dataset_helpers.py`

 * *Files identical despite different names*

### Comparing `literalai-0.0.604/literalai/api/generation_helpers.py` & `literalai-0.0.605/literalai/api/generation_helpers.py`

 * *Files identical despite different names*

### Comparing `literalai-0.0.604/literalai/api/gql.py` & `literalai-0.0.605/literalai/api/gql.py`

 * *Files identical despite different names*

### Comparing `literalai-0.0.604/literalai/api/prompt_helpers.py` & `literalai-0.0.605/literalai/api/prompt_helpers.py`

 * *Files identical despite different names*

### Comparing `literalai-0.0.604/literalai/api/score_helpers.py` & `literalai-0.0.605/literalai/api/score_helpers.py`

 * *Files identical despite different names*

### Comparing `literalai-0.0.604/literalai/api/step_helpers.py` & `literalai-0.0.605/literalai/api/step_helpers.py`

 * *Files identical despite different names*

### Comparing `literalai-0.0.604/literalai/api/thread_helpers.py` & `literalai-0.0.605/literalai/api/thread_helpers.py`

 * *Files identical despite different names*

### Comparing `literalai-0.0.604/literalai/api/user_helpers.py` & `literalai-0.0.605/literalai/api/user_helpers.py`

 * *Files identical despite different names*

### Comparing `literalai-0.0.604/literalai/callback/langchain_callback.py` & `literalai-0.0.605/literalai/callback/langchain_callback.py`

 * *Files identical despite different names*

### Comparing `literalai-0.0.604/literalai/callback/llama_index_callback.py` & `literalai-0.0.605/literalai/callback/llama_index_callback.py`

 * *Files identical despite different names*

### Comparing `literalai-0.0.604/literalai/client.py` & `literalai-0.0.605/literalai/client.py`

 * *Files identical despite different names*

### Comparing `literalai-0.0.604/literalai/dataset.py` & `literalai-0.0.605/literalai/dataset.py`

 * *Files identical despite different names*

### Comparing `literalai-0.0.604/literalai/dataset_experiment.py` & `literalai-0.0.605/literalai/dataset_experiment.py`

 * *Files identical despite different names*

### Comparing `literalai-0.0.604/literalai/dataset_item.py` & `literalai-0.0.605/literalai/dataset_item.py`

 * *Files identical despite different names*

### Comparing `literalai-0.0.604/literalai/event_processor.py` & `literalai-0.0.605/literalai/event_processor.py`

 * *Files identical despite different names*

### Comparing `literalai-0.0.604/literalai/filter.py` & `literalai-0.0.605/literalai/filter.py`

 * *Files identical despite different names*

### Comparing `literalai-0.0.604/literalai/helper.py` & `literalai-0.0.605/literalai/helper.py`

 * *Files identical despite different names*

### Comparing `literalai-0.0.604/literalai/instrumentation/openai.py` & `literalai-0.0.605/literalai/instrumentation/openai.py`

 * *Files identical despite different names*

### Comparing `literalai-0.0.604/literalai/message.py` & `literalai-0.0.605/literalai/message.py`

 * *Files identical despite different names*

### Comparing `literalai-0.0.604/literalai/my_types.py` & `literalai-0.0.605/literalai/my_types.py`

 * *Files identical despite different names*

### Comparing `literalai-0.0.604/literalai/prompt.py` & `literalai-0.0.605/literalai/prompt.py`

 * *Files identical despite different names*

### Comparing `literalai-0.0.604/literalai/requirements.py` & `literalai-0.0.605/literalai/requirements.py`

 * *Files identical despite different names*

### Comparing `literalai-0.0.604/literalai/step.py` & `literalai-0.0.605/literalai/step.py`

 * *Files identical despite different names*

### Comparing `literalai-0.0.604/literalai/thread.py` & `literalai-0.0.605/literalai/thread.py`

 * *Files identical despite different names*

### Comparing `literalai-0.0.604/literalai/wrappers.py` & `literalai-0.0.605/literalai/wrappers.py`

 * *Files identical despite different names*

### Comparing `literalai-0.0.604/literalai.egg-info/SOURCES.txt` & `literalai-0.0.605/literalai.egg-info/SOURCES.txt`

 * *Files identical despite different names*

