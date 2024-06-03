# Comparing `tmp/jbtsdk-0.0.29.tar.gz` & `tmp/jbtsdk-0.0.30.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jbtsdk-0.0.29.tar", last modified: Wed May 29 19:52:46 2024, max compression
+gzip compressed data, was "jbtsdk-0.0.30.tar", last modified: Mon Jun  3 13:20:53 2024, max compression
```

## Comparing `jbtsdk-0.0.29.tar` & `jbtsdk-0.0.30.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2024-05-29 19:52:46.057169 jbtsdk-0.0.29/
--rw-rw-rw-   0        0        0     1069 2024-05-29 19:51:16.000000 jbtsdk-0.0.29/LICENSE
--rw-rw-rw-   0        0        0      270 2024-05-29 19:52:46.055168 jbtsdk-0.0.29/PKG-INFO
--rw-rw-rw-   0        0        0      173 2024-03-26 18:30:45.000000 jbtsdk-0.0.29/README.md
-drwxrwxrwx   0        0        0        0 2024-05-29 19:52:46.045155 jbtsdk-0.0.29/jbtsdk/
--rw-rw-rw-   0        0        0     5160 2024-05-29 17:49:20.000000 jbtsdk-0.0.29/jbtsdk/JabutiSDK.py
--rw-rw-rw-   0        0        0      159 2024-03-28 14:11:07.000000 jbtsdk-0.0.29/jbtsdk/__init__.py
--rw-rw-rw-   0        0        0     1192 2024-03-28 14:09:50.000000 jbtsdk-0.0.29/jbtsdk/utils.py
-drwxrwxrwx   0        0        0        0 2024-05-29 19:52:46.054172 jbtsdk-0.0.29/jbtsdk.egg-info/
--rw-rw-rw-   0        0        0      270 2024-05-29 19:52:45.000000 jbtsdk-0.0.29/jbtsdk.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      230 2024-05-29 19:52:45.000000 jbtsdk-0.0.29/jbtsdk.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-29 19:52:45.000000 jbtsdk-0.0.29/jbtsdk.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       49 2024-05-29 19:52:45.000000 jbtsdk-0.0.29/jbtsdk.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2024-05-29 19:52:45.000000 jbtsdk-0.0.29/jbtsdk.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-29 19:52:46.057169 jbtsdk-0.0.29/setup.cfg
--rw-rw-rw-   0        0        0      309 2024-05-29 19:52:28.000000 jbtsdk-0.0.29/setup.py
+drwxrwxrwx   0        0        0        0 2024-06-03 13:20:53.738857 jbtsdk-0.0.30/
+-rw-rw-rw-   0        0        0     1069 2024-05-29 19:51:16.000000 jbtsdk-0.0.30/LICENSE
+-rw-rw-rw-   0        0        0      270 2024-06-03 13:20:53.735563 jbtsdk-0.0.30/PKG-INFO
+-rw-rw-rw-   0        0        0      173 2024-03-26 18:30:45.000000 jbtsdk-0.0.30/README.md
+drwxrwxrwx   0        0        0        0 2024-06-03 13:20:53.717486 jbtsdk-0.0.30/jbtsdk/
+-rw-rw-rw-   0        0        0     5196 2024-06-03 13:19:48.000000 jbtsdk-0.0.30/jbtsdk/JabutiSDK.py
+-rw-rw-rw-   0        0        0      159 2024-03-28 14:11:07.000000 jbtsdk-0.0.30/jbtsdk/__init__.py
+-rw-rw-rw-   0        0        0     1192 2024-03-28 14:09:50.000000 jbtsdk-0.0.30/jbtsdk/utils.py
+drwxrwxrwx   0        0        0        0 2024-06-03 13:20:53.734276 jbtsdk-0.0.30/jbtsdk.egg-info/
+-rw-rw-rw-   0        0        0      270 2024-06-03 13:20:53.000000 jbtsdk-0.0.30/jbtsdk.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      230 2024-06-03 13:20:53.000000 jbtsdk-0.0.30/jbtsdk.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-06-03 13:20:53.000000 jbtsdk-0.0.30/jbtsdk.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       49 2024-06-03 13:20:53.000000 jbtsdk-0.0.30/jbtsdk.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2024-06-03 13:20:53.000000 jbtsdk-0.0.30/jbtsdk.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-06-03 13:20:53.738857 jbtsdk-0.0.30/setup.cfg
+-rw-rw-rw-   0        0        0      309 2024-06-03 13:19:52.000000 jbtsdk-0.0.30/setup.py
```

### Comparing `jbtsdk-0.0.29/LICENSE` & `jbtsdk-0.0.30/LICENSE`

 * *Files identical despite different names*

### Comparing `jbtsdk-0.0.29/jbtsdk/JabutiSDK.py` & `jbtsdk-0.0.30/jbtsdk/JabutiSDK.py`

 * *Files 1% similar despite different names*

```diff
@@ -52,15 +52,16 @@
             _payload["username"] = username
         try:
             headers = {'x-api-key': self.api_key}
             response = requests.post(self.api_url, data=json.dumps(_payload), headers=headers, timeout=60)
             # if callbacks:
             #     for cb in callbacks:
             #         cb.on_llm_new_token(token=response.text)
-            return response.content.decode('UTF-8')
+            # return response.content.decode('UTF-8')
+            return response.text
             
         except Exception as e:
             print(f"Error: {e}")
             raise Exception("Falha na execução.")
         
     async def async_fast_chat(self, input, username=None ,callbacks=[]):
         _payload = dict()
```

### Comparing `jbtsdk-0.0.29/jbtsdk/utils.py` & `jbtsdk-0.0.30/jbtsdk/utils.py`

 * *Files identical despite different names*

