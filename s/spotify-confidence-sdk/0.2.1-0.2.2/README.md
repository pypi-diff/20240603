# Comparing `tmp/spotify_confidence_sdk-0.2.1.tar.gz` & `tmp/spotify_confidence_sdk-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spotify_confidence_sdk-0.2.1.tar", last modified: Wed May 29 12:16:25 2024, max compression
+gzip compressed data, was "spotify_confidence_sdk-0.2.2.tar", last modified: Mon Jun  3 09:00:30 2024, max compression
```

## Comparing `spotify_confidence_sdk-0.2.1.tar` & `spotify_confidence_sdk-0.2.2.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 12:16:25.363485 spotify_confidence_sdk-0.2.1/
--rw-r--r--   0 root         (0) root         (0)    11357 2024-05-29 12:16:11.000000 spotify_confidence_sdk-0.2.1/LICENSE
--rw-r--r--   0 root         (0) root         (0)    15785 2024-05-29 12:16:25.363485 spotify_confidence_sdk-0.2.1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2113 2024-05-29 12:16:11.000000 spotify_confidence_sdk-0.2.1/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 12:16:25.363485 spotify_confidence_sdk-0.2.1/confidence/
--rw-r--r--   0 root         (0) root         (0)      199 2024-05-29 12:16:11.000000 spotify_confidence_sdk-0.2.1/confidence/__init__.py
--rw-r--r--   0 root         (0) root         (0)      411 2024-05-29 12:16:25.000000 spotify_confidence_sdk-0.2.1/confidence/_version.py
--rw-r--r--   0 root         (0) root         (0)     9407 2024-05-29 12:16:11.000000 spotify_confidence_sdk-0.2.1/confidence/confidence.py
--rw-r--r--   0 root         (0) root         (0)     4358 2024-05-29 12:16:11.000000 spotify_confidence_sdk-0.2.1/confidence/errors.py
--rw-r--r--   0 root         (0) root         (0)     1625 2024-05-29 12:16:11.000000 spotify_confidence_sdk-0.2.1/confidence/flag_types.py
--rw-r--r--   0 root         (0) root         (0)      748 2024-05-29 12:16:11.000000 spotify_confidence_sdk-0.2.1/confidence/names.py
--rw-r--r--   0 root         (0) root         (0)     7139 2024-05-29 12:16:11.000000 spotify_confidence_sdk-0.2.1/confidence/openfeature_provider.py
--rw-r--r--   0 root         (0) root         (0)      939 2024-05-29 12:16:11.000000 spotify_confidence_sdk-0.2.1/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2024-05-29 12:16:25.367485 spotify_confidence_sdk-0.2.1/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 12:16:25.363485 spotify_confidence_sdk-0.2.1/spotify_confidence_sdk.egg-info/
--rw-r--r--   0 root         (0) root         (0)    15785 2024-05-29 12:16:25.000000 spotify_confidence_sdk-0.2.1/spotify_confidence_sdk.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      530 2024-05-29 12:16:25.000000 spotify_confidence_sdk-0.2.1/spotify_confidence_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-05-29 12:16:25.000000 spotify_confidence_sdk-0.2.1/spotify_confidence_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      106 2024-05-29 12:16:25.000000 spotify_confidence_sdk-0.2.1/spotify_confidence_sdk.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       22 2024-05-29 12:16:25.000000 spotify_confidence_sdk-0.2.1/spotify_confidence_sdk.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 12:16:25.363485 spotify_confidence_sdk-0.2.1/tests/
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-29 12:16:11.000000 spotify_confidence_sdk-0.2.1/tests/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1054 2024-05-29 12:16:11.000000 spotify_confidence_sdk-0.2.1/tests/test_names.py
--rw-r--r--   0 root         (0) root         (0)    10509 2024-05-29 12:16:11.000000 spotify_confidence_sdk-0.2.1/tests/test_provider.py
--rw-r--r--   0 root         (0) root         (0)     1040 2024-05-29 12:16:11.000000 spotify_confidence_sdk-0.2.1/tests/test_provider_parametrized.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-06-03 09:00:30.742320 spotify_confidence_sdk-0.2.2/
+-rw-r--r--   0 root         (0) root         (0)    11357 2024-06-03 09:00:18.000000 spotify_confidence_sdk-0.2.2/LICENSE
+-rw-r--r--   0 root         (0) root         (0)    15246 2024-06-03 09:00:30.742320 spotify_confidence_sdk-0.2.2/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1574 2024-06-03 09:00:18.000000 spotify_confidence_sdk-0.2.2/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-06-03 09:00:30.738320 spotify_confidence_sdk-0.2.2/confidence/
+-rw-r--r--   0 root         (0) root         (0)      199 2024-06-03 09:00:18.000000 spotify_confidence_sdk-0.2.2/confidence/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      411 2024-06-03 09:00:30.000000 spotify_confidence_sdk-0.2.2/confidence/_version.py
+-rw-r--r--   0 root         (0) root         (0)     9399 2024-06-03 09:00:18.000000 spotify_confidence_sdk-0.2.2/confidence/confidence.py
+-rw-r--r--   0 root         (0) root         (0)     4358 2024-06-03 09:00:18.000000 spotify_confidence_sdk-0.2.2/confidence/errors.py
+-rw-r--r--   0 root         (0) root         (0)     1625 2024-06-03 09:00:18.000000 spotify_confidence_sdk-0.2.2/confidence/flag_types.py
+-rw-r--r--   0 root         (0) root         (0)      748 2024-06-03 09:00:18.000000 spotify_confidence_sdk-0.2.2/confidence/names.py
+-rw-r--r--   0 root         (0) root         (0)     7139 2024-06-03 09:00:18.000000 spotify_confidence_sdk-0.2.2/confidence/openfeature_provider.py
+-rw-r--r--   0 root         (0) root         (0)      939 2024-06-03 09:00:18.000000 spotify_confidence_sdk-0.2.2/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2024-06-03 09:00:30.742320 spotify_confidence_sdk-0.2.2/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-06-03 09:00:30.742320 spotify_confidence_sdk-0.2.2/spotify_confidence_sdk.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    15246 2024-06-03 09:00:30.000000 spotify_confidence_sdk-0.2.2/spotify_confidence_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      530 2024-06-03 09:00:30.000000 spotify_confidence_sdk-0.2.2/spotify_confidence_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-06-03 09:00:30.000000 spotify_confidence_sdk-0.2.2/spotify_confidence_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      106 2024-06-03 09:00:30.000000 spotify_confidence_sdk-0.2.2/spotify_confidence_sdk.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       22 2024-06-03 09:00:30.000000 spotify_confidence_sdk-0.2.2/spotify_confidence_sdk.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-06-03 09:00:30.742320 spotify_confidence_sdk-0.2.2/tests/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-06-03 09:00:18.000000 spotify_confidence_sdk-0.2.2/tests/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1054 2024-06-03 09:00:18.000000 spotify_confidence_sdk-0.2.2/tests/test_names.py
+-rw-r--r--   0 root         (0) root         (0)    10509 2024-06-03 09:00:18.000000 spotify_confidence_sdk-0.2.2/tests/test_provider.py
+-rw-r--r--   0 root         (0) root         (0)     1040 2024-06-03 09:00:18.000000 spotify_confidence_sdk-0.2.2/tests/test_provider_parametrized.py
```

### Comparing `spotify_confidence_sdk-0.2.1/LICENSE` & `spotify_confidence_sdk-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `spotify_confidence_sdk-0.2.1/PKG-INFO` & `spotify_confidence_sdk-0.2.2/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spotify_confidence_sdk
-Version: 0.2.1
+Version: 0.2.2
 Summary: Confidence provider for the OpenFeature SDK
 Author: Confidence team
 License: 
                                          Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
@@ -216,70 +216,54 @@
 Requires-Dist: typing_extensions==4.9.0
 Provides-Extra: dev
 Requires-Dist: pytest; extra == "dev"
 Requires-Dist: black; extra == "dev"
 Requires-Dist: flake8; extra == "dev"
 Requires-Dist: requests_mock; extra == "dev"
 
-# Confidence OpenFeature Python Provider
+# Confidence SDK
 
-This repo contains the OpenFeature Python flag provider for [Confidence](https://confidence.spotify.com/).
-
-## OpenFeature
-
-Before starting to use the provider, it can be helpful to read through the general [OpenFeature docs](https://docs.openfeature.dev/)
-and get familiar with the concepts. 
+This repo contains the [Confidence](https://confidence.spotify.com/) SDK for python and the Confidence OpenFeature flag provider.
 
 ## Adding the dependency
 
 #### pip install
 <!---x-release-please-start-version-->
 ```python
-pip install spotify-confidence-sdk==0.2.1
+pip install spotify-confidence-sdk==0.2.2
 
 #### requirements.txt
 ```python
-spotify-confidence-sdk==0.2.1
+spotify-confidence-sdk==0.2.2
 
 pip install -r requirements.txt
 ```
 <!---x-release-please-end-->
 
 ### Creating and using the flag provider
 
-Below is an example for how to create a OpenFeature client using the Confidence flag provider, and then resolve
-a flag with a boolean attribute. The provider is configured with an api key and a region, which will determine
-where it will send the resolving requests. 
+Below is an example for how to initialize the Confidence SDK, and then resolve
+a flag with a boolean attribute. The SDK is configured with an api key, which will authorize the resolving requests. 
 
 The flag will be applied immediately, meaning that Confidence will count the targeted user as having received the treatment. 
 
 You can retrieve attributes on the flag variant using property dot notation, meaning `test-flag.boolean-key` will retrieve
 the attribute `boolean-key` on the flag `test-flag`. 
 
 You can also use only the flag name `test-flag` and retrieve all values as a map with `resolve_object_details()`. 
 
 The flag's schema is validated against the requested data type, and if it doesn't match it will fall back to the default value.
 
 ```python
 
+from confidence.confidence import Confidence
 from confidence.confidence import Region
-from confidence.openfeature_provider import ConfidenceOpenFeatureProvider
-from openfeature.api import EvaluationContext
-from openfeature import api
-
-provider = ConfidenceOpenFeatureProvider("client_secret", Region.EU)
-
-api.set_provider(provider)
-open_feature_client = api.get_client()
-
-ctx = EvaluationContext(targeting_key="random", attributes={
-    "user": {
-        "country": "SE"
-    }
-})
-
-flag_value = open_feature_client.get_boolean_value(flag_key="test-flag.boolean-key", default_value=False,
-                                                   evaluation_context=ctx)
 
+confidence = Confidence("API_KEY")
+# to send an event
+confidence.with_context({"app": "python"}).track("event_name", {})
+#to resolve a flag
+default_value = False
+flag_value = confidence.resolve_boolean_details("test-flag.boolean-key", default_value)
 print(flag_value)
 
 ```
```

### Comparing `spotify_confidence_sdk-0.2.1/confidence/confidence.py` & `spotify_confidence_sdk-0.2.2/confidence/confidence.py`

 * *Files 1% similar despite different names*

```diff
@@ -166,15 +166,15 @@
             variant=variant_name.variant,
             reason=Reason.TARGETING_MATCH,
             flag_metadata={"flag_key": flag_key},
         )
 
     # type-arg: ignore
     def track(self, event_name: str, data: Dict[str, FieldType]) -> None:
-        asyncio.create_task(self._send_event(event_name, data))
+        asyncio.run(self._send_event(event_name, data))
 
     async def track_async(self, event_name: str, data: Dict[str, FieldType]) -> None:
         await self._send_event(event_name, data)
 
     async def _send_event(self, event_name: str, data: Dict[str, FieldType]) -> None:
         current_time = datetime.utcnow().isoformat() + "Z"
         request_body = {
```

### Comparing `spotify_confidence_sdk-0.2.1/confidence/errors.py` & `spotify_confidence_sdk-0.2.2/confidence/errors.py`

 * *Files identical despite different names*

### Comparing `spotify_confidence_sdk-0.2.1/confidence/flag_types.py` & `spotify_confidence_sdk-0.2.2/confidence/flag_types.py`

 * *Files identical despite different names*

### Comparing `spotify_confidence_sdk-0.2.1/confidence/names.py` & `spotify_confidence_sdk-0.2.2/confidence/names.py`

 * *Files identical despite different names*

### Comparing `spotify_confidence_sdk-0.2.1/confidence/openfeature_provider.py` & `spotify_confidence_sdk-0.2.2/confidence/openfeature_provider.py`

 * *Files identical despite different names*

### Comparing `spotify_confidence_sdk-0.2.1/pyproject.toml` & `spotify_confidence_sdk-0.2.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `spotify_confidence_sdk-0.2.1/spotify_confidence_sdk.egg-info/PKG-INFO` & `spotify_confidence_sdk-0.2.2/spotify_confidence_sdk.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spotify_confidence_sdk
-Version: 0.2.1
+Version: 0.2.2
 Summary: Confidence provider for the OpenFeature SDK
 Author: Confidence team
 License: 
                                          Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
@@ -216,70 +216,54 @@
 Requires-Dist: typing_extensions==4.9.0
 Provides-Extra: dev
 Requires-Dist: pytest; extra == "dev"
 Requires-Dist: black; extra == "dev"
 Requires-Dist: flake8; extra == "dev"
 Requires-Dist: requests_mock; extra == "dev"
 
-# Confidence OpenFeature Python Provider
+# Confidence SDK
 
-This repo contains the OpenFeature Python flag provider for [Confidence](https://confidence.spotify.com/).
-
-## OpenFeature
-
-Before starting to use the provider, it can be helpful to read through the general [OpenFeature docs](https://docs.openfeature.dev/)
-and get familiar with the concepts. 
+This repo contains the [Confidence](https://confidence.spotify.com/) SDK for python and the Confidence OpenFeature flag provider.
 
 ## Adding the dependency
 
 #### pip install
 <!---x-release-please-start-version-->
 ```python
-pip install spotify-confidence-sdk==0.2.1
+pip install spotify-confidence-sdk==0.2.2
 
 #### requirements.txt
 ```python
-spotify-confidence-sdk==0.2.1
+spotify-confidence-sdk==0.2.2
 
 pip install -r requirements.txt
 ```
 <!---x-release-please-end-->
 
 ### Creating and using the flag provider
 
-Below is an example for how to create a OpenFeature client using the Confidence flag provider, and then resolve
-a flag with a boolean attribute. The provider is configured with an api key and a region, which will determine
-where it will send the resolving requests. 
+Below is an example for how to initialize the Confidence SDK, and then resolve
+a flag with a boolean attribute. The SDK is configured with an api key, which will authorize the resolving requests. 
 
 The flag will be applied immediately, meaning that Confidence will count the targeted user as having received the treatment. 
 
 You can retrieve attributes on the flag variant using property dot notation, meaning `test-flag.boolean-key` will retrieve
 the attribute `boolean-key` on the flag `test-flag`. 
 
 You can also use only the flag name `test-flag` and retrieve all values as a map with `resolve_object_details()`. 
 
 The flag's schema is validated against the requested data type, and if it doesn't match it will fall back to the default value.
 
 ```python
 
+from confidence.confidence import Confidence
 from confidence.confidence import Region
-from confidence.openfeature_provider import ConfidenceOpenFeatureProvider
-from openfeature.api import EvaluationContext
-from openfeature import api
-
-provider = ConfidenceOpenFeatureProvider("client_secret", Region.EU)
-
-api.set_provider(provider)
-open_feature_client = api.get_client()
-
-ctx = EvaluationContext(targeting_key="random", attributes={
-    "user": {
-        "country": "SE"
-    }
-})
-
-flag_value = open_feature_client.get_boolean_value(flag_key="test-flag.boolean-key", default_value=False,
-                                                   evaluation_context=ctx)
 
+confidence = Confidence("API_KEY")
+# to send an event
+confidence.with_context({"app": "python"}).track("event_name", {})
+#to resolve a flag
+default_value = False
+flag_value = confidence.resolve_boolean_details("test-flag.boolean-key", default_value)
 print(flag_value)
 
 ```
```

### Comparing `spotify_confidence_sdk-0.2.1/spotify_confidence_sdk.egg-info/SOURCES.txt` & `spotify_confidence_sdk-0.2.2/spotify_confidence_sdk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `spotify_confidence_sdk-0.2.1/tests/test_names.py` & `spotify_confidence_sdk-0.2.2/tests/test_names.py`

 * *Files identical despite different names*

### Comparing `spotify_confidence_sdk-0.2.1/tests/test_provider.py` & `spotify_confidence_sdk-0.2.2/tests/test_provider.py`

 * *Files identical despite different names*

### Comparing `spotify_confidence_sdk-0.2.1/tests/test_provider_parametrized.py` & `spotify_confidence_sdk-0.2.2/tests/test_provider_parametrized.py`

 * *Files identical despite different names*

