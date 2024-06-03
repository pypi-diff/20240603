# Comparing `tmp/orchestrate_api-2.1.0.tar.gz` & `tmp/orchestrate_api-2.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "orchestrate_api-2.1.0.tar", max compression
+gzip compressed data, was "orchestrate_api-2.2.0.tar", max compression
```

## Comparing `orchestrate_api-2.1.0.tar` & `orchestrate_api-2.2.0.tar`

### file list

```diff
@@ -1,18 +1,25 @@
--rw-r--r--   0        0        0      840 2024-03-13 13:38:30.313195 orchestrate_api-2.1.0/README.md
--rw-r--r--   0        0        0      350 2024-03-13 13:38:15.741206 orchestrate_api-2.1.0/orchestrate/__init__.py
--rw-r--r--   0        0        0        0 2024-03-13 13:38:15.741206 orchestrate_api-2.1.0/orchestrate/_internal/__init__.py
--rw-r--r--   0        0        0      733 2024-03-13 13:38:15.741206 orchestrate_api-2.1.0/orchestrate/_internal/api.py
--rw-r--r--   0        0        0     1345 2024-03-13 13:38:15.741206 orchestrate_api-2.1.0/orchestrate/_internal/batch.py
--rw-r--r--   0        0        0     9863 2024-03-13 13:38:15.741206 orchestrate_api-2.1.0/orchestrate/_internal/convert.py
--rw-r--r--   0        0        0      677 2024-03-13 13:38:15.741206 orchestrate_api-2.1.0/orchestrate/_internal/exceptions.py
--rw-r--r--   0        0        0     1356 2024-03-13 13:38:15.741206 orchestrate_api-2.1.0/orchestrate/_internal/fhir.py
--rw-r--r--   0        0        0     5549 2024-03-13 13:38:15.741206 orchestrate_api-2.1.0/orchestrate/_internal/http_handler.py
--rw-r--r--   0        0        0     2133 2024-03-13 13:38:15.741206 orchestrate_api-2.1.0/orchestrate/_internal/insight.py
--rw-r--r--   0        0        0    37803 2024-03-13 13:38:15.741206 orchestrate_api-2.1.0/orchestrate/_internal/terminology.py
--rw-r--r--   0        0        0       82 2024-03-13 13:38:15.741206 orchestrate_api-2.1.0/orchestrate/_internal/version.py
--rw-r--r--   0        0        0      669 2024-03-13 13:38:15.741206 orchestrate_api-2.1.0/orchestrate/convert.py
--rw-r--r--   0        0        0      222 2024-03-13 13:38:15.741206 orchestrate_api-2.1.0/orchestrate/exceptions.py
--rw-r--r--   0        0        0      217 2024-03-13 13:38:15.741206 orchestrate_api-2.1.0/orchestrate/insight.py
--rw-r--r--   0        0        0     2035 2024-03-13 13:38:15.741206 orchestrate_api-2.1.0/orchestrate/terminology.py
--rw-r--r--   0        0        0      915 2024-03-13 13:38:32.713193 orchestrate_api-2.1.0/pyproject.toml
--rw-r--r--   0        0        0     1720 1970-01-01 00:00:00.000000 orchestrate_api-2.1.0/PKG-INFO
+-rw-r--r--   0        0        0      840 2024-06-03 15:35:45.073696 orchestrate_api-2.2.0/README.md
+-rw-r--r--   0        0        0      422 2024-06-03 15:35:29.745678 orchestrate_api-2.2.0/orchestrate/__init__.py
+-rw-r--r--   0        0        0        0 2024-06-03 15:35:29.745678 orchestrate_api-2.2.0/orchestrate/_internal/__init__.py
+-rw-r--r--   0        0        0      733 2024-06-03 15:35:29.745678 orchestrate_api-2.2.0/orchestrate/_internal/api.py
+-rw-r--r--   0        0        0     1345 2024-06-03 15:35:29.745678 orchestrate_api-2.2.0/orchestrate/_internal/batch.py
+-rw-r--r--   0        0        0    12884 2024-06-03 15:35:29.745678 orchestrate_api-2.2.0/orchestrate/_internal/convert.py
+-rw-r--r--   0        0        0      677 2024-06-03 15:35:29.745678 orchestrate_api-2.2.0/orchestrate/_internal/exceptions.py
+-rw-r--r--   0        0        0     1356 2024-06-03 15:35:29.745678 orchestrate_api-2.2.0/orchestrate/_internal/fhir.py
+-rw-r--r--   0        0        0     8262 2024-06-03 15:35:29.745678 orchestrate_api-2.2.0/orchestrate/_internal/http_handler.py
+-rw-r--r--   0        0        0      168 2024-06-03 15:35:29.745678 orchestrate_api-2.2.0/orchestrate/_internal/identity/advisories.py
+-rw-r--r--   0        0        0    18701 2024-06-03 15:35:29.745678 orchestrate_api-2.2.0/orchestrate/_internal/identity/api.py
+-rw-r--r--   0        0        0     3137 2024-06-03 15:35:29.745678 orchestrate_api-2.2.0/orchestrate/_internal/identity/demographic.py
+-rw-r--r--   0        0        0     3672 2024-06-03 15:35:29.745678 orchestrate_api-2.2.0/orchestrate/_internal/identity/local_hashing.py
+-rw-r--r--   0        0        0     2635 2024-06-03 15:35:29.745678 orchestrate_api-2.2.0/orchestrate/_internal/identity/monitoring.py
+-rw-r--r--   0        0        0     2202 2024-06-03 15:35:29.745678 orchestrate_api-2.2.0/orchestrate/_internal/insight.py
+-rw-r--r--   0        0        0    38271 2024-06-03 15:35:29.745678 orchestrate_api-2.2.0/orchestrate/_internal/terminology.py
+-rw-r--r--   0        0        0       82 2024-06-03 15:35:29.745678 orchestrate_api-2.2.0/orchestrate/_internal/version.py
+-rw-r--r--   0        0        0     1197 2024-06-03 15:35:29.745678 orchestrate_api-2.2.0/orchestrate/convert.py
+-rw-r--r--   0        0        0      222 2024-06-03 15:35:29.745678 orchestrate_api-2.2.0/orchestrate/exceptions.py
+-rw-r--r--   0        0        0     1361 2024-06-03 15:35:29.745678 orchestrate_api-2.2.0/orchestrate/identity/__init__.py
+-rw-r--r--   0        0        0      547 2024-06-03 15:35:29.745678 orchestrate_api-2.2.0/orchestrate/identity/monitoring.py
+-rw-r--r--   0        0        0      217 2024-06-03 15:35:29.745678 orchestrate_api-2.2.0/orchestrate/insight.py
+-rw-r--r--   0        0        0     2035 2024-06-03 15:35:29.745678 orchestrate_api-2.2.0/orchestrate/terminology.py
+-rw-r--r--   0        0        0     1030 2024-06-03 15:35:47.485698 orchestrate_api-2.2.0/pyproject.toml
+-rw-r--r--   0        0        0     1720 1970-01-01 00:00:00.000000 orchestrate_api-2.2.0/PKG-INFO
```

### Comparing `orchestrate_api-2.1.0/README.md` & `orchestrate_api-2.2.0/README.md`

 * *Files identical despite different names*

### Comparing `orchestrate_api-2.1.0/orchestrate/_internal/api.py` & `orchestrate_api-2.2.0/orchestrate/_internal/api.py`

 * *Files identical despite different names*

### Comparing `orchestrate_api-2.1.0/orchestrate/_internal/batch.py` & `orchestrate_api-2.2.0/orchestrate/_internal/batch.py`

 * *Files identical despite different names*

### Comparing `orchestrate_api-2.1.0/orchestrate/_internal/convert.py` & `orchestrate_api-2.2.0/orchestrate/_internal/convert.py`

 * *Files 13% similar despite different names*

```diff
@@ -25,14 +25,20 @@
 
 ConvertFhirStu3ToFhirR4Response = Bundle
 
 ConvertFhirR4ToHealthLakeResponse = Bundle
 
 ConvertCdaToHtmlResponse = str
 
+ConvertFhirR4ToNemsisV34Response = str
+
+ConvertFhirR4ToNemsisV35Response = str
+
+ConvertFhirR4ToManifestResponse = bytes
+
 
 def generate_convert_combine_fhir_bundles_request_from_bundles(
     fhir_bundles: list[Bundle],
 ) -> str:
     """
     Converts a list of FHIR bundles into a request body for the combine FHIR bundles endpoint.
 
@@ -63,33 +69,36 @@
     def __repr__(self) -> str:
         return f"{self.__class__.__name__}(base_url={self.__http_handler.base_url!r})"
 
     def hl7_to_fhir_r4(
         self,
         content: str,
         patient_id: Optional[str] = None,
+        tz: Optional[str] = None,
     ) -> ConvertHl7ToFhirR4Response:
         """
         Converts one or more HL7v2 messages into a FHIR R4 bundle
 
         ### Parameters
 
         - `hl7_message`: The HL7 message(s) to convert
         - `patient_id`: The patient ID to use for the FHIR bundle
+        - `tz`: Default timezone for date-times in the HL7 when no timezone offset is present. Must be IANA or Windows timezone name. Defaults to UTC.
 
         ### Returns
 
         A FHIR R4 Bundle containing the clinical data parsed out of the HL7 messages
 
         ### Documentation
 
         <https://rosetta-api.docs.careevolution.com/convert/hl7_to_fhir.html>
         """
         headers = {"Content-Type": "text/plain"}
         parameters = _get_id_dependent_parameters("patientId", patient_id)
+        parameters = {**parameters, **_get_id_dependent_parameters("tz", tz)}
         return self.__http_handler.post(
             path="/convert/v1/hl7tofhirr4",
             body=content,
             headers=headers,
             parameters=parameters,
         )
 
@@ -342,7 +351,86 @@
         """
         headers = {"Content-Type": "application/xml", "Accept": "text/html"}
         return self.__http_handler.post(
             path="/convert/v1/cdatohtml",
             body=content,
             headers=headers,
         )
+
+    def fhir_r4_to_nemsis_v34(
+        self, content: Bundle
+    ) -> ConvertFhirR4ToNemsisV34Response:
+        """
+        Converts a FHIR R4 bundle (including one from CDA-to-FHIR, HL7-to-FHIR, or Combine Bundles) into the National Emergency Medical Services Information System (NEMSIS) XML format.
+
+        ### Parameters
+
+        - `fhir_bundle`: A FHIR R4 bundle for a single patient. The bundle must contain at least one Encounter resource with a valid admission date.
+
+        ### Returns
+
+        A NEMSIS v3.4 document in XML format.
+
+        ### Documentation
+
+        <https://orchestrate.docs.careevolution.com/convert/fhir_to_nemsis.html>
+        """
+        headers = {"Accept": "application/xml"}
+        return self.__http_handler.post(
+            path="/convert/v1/fhirr4tonemsisv34",
+            body=content,
+            headers=headers,
+        )
+
+    def fhir_r4_to_nemsis_v35(
+        self, content: Bundle
+    ) -> ConvertFhirR4ToNemsisV35Response:
+        """
+        Converts a FHIR R4 bundle (including one from CDA-to-FHIR, HL7-to-FHIR, or Combine Bundles) into the National Emergency Medical Services Information System (NEMSIS) XML format.
+
+        ### Parameters
+
+        - `fhir_bundle`: A FHIR R4 bundle for a single patient. The bundle must contain at least one Encounter resource with a valid admission date.
+
+        ### Returns
+
+        A NEMSIS v3.5 document in XML format.
+
+        ### Documentation
+
+        <https://orchestrate.docs.careevolution.com/convert/fhir_to_nemsis.html>
+        """
+        headers = {"Accept": "application/xml"}
+        return self.__http_handler.post(
+            path="/convert/v1/fhirr4tonemsisv35",
+            body=content,
+            headers=headers,
+        )
+
+    def fhir_r4_to_manifest(self, content: Bundle) -> ConvertFhirR4ToManifestResponse:
+        """
+        Generates a tabular report of clinical concepts from a FHIR R4
+        bundle. With this tabular data, you can easily scan results, run
+        queries, and understand the value of your clinical data.
+
+        ### Parameters
+
+        - `content`: A FHIR R4 bundle
+
+        ### Returns
+
+        A ZIP file containing a number of Comma-Separated Value (CSV)
+        files corresponding to clinical concepts (conditions,
+        encounters, etc.).
+
+        ### Documentation
+
+        <https://orchestrate.docs.careevolution.com/convert/fhir_manifest.html>
+        """
+        headers = {
+            "Accept": "application/zip",
+        }
+        return self.__http_handler.post(
+            path="/convert/v1/fhirr4tomanifest",
+            body=content,
+            headers=headers,
+        )
```

### Comparing `orchestrate_api-2.1.0/orchestrate/_internal/exceptions.py` & `orchestrate_api-2.2.0/orchestrate/_internal/exceptions.py`

 * *Files identical despite different names*

### Comparing `orchestrate_api-2.1.0/orchestrate/_internal/fhir.py` & `orchestrate_api-2.2.0/orchestrate/_internal/fhir.py`

 * *Files identical despite different names*

### Comparing `orchestrate_api-2.1.0/orchestrate/_internal/insight.py` & `orchestrate_api-2.2.0/orchestrate/_internal/insight.py`

 * *Files 4% similar despite different names*

```diff
@@ -64,15 +64,15 @@
 
         ### Returns
 
         A new FHIR R4 Bundle containing measure and assessment resources
 
         ### Documentation
 
-        <
+        <https://orchestrate.docs.careevolution.com/insight/risk_profile.html>
         """
         parameters = {
             "hccVersion": hcc_version,
             "periodEndDate": period_end_date,
             "raSegment": ra_segment,
         }
         return self.__http_handler.post(
```

### Comparing `orchestrate_api-2.1.0/orchestrate/_internal/terminology.py` & `orchestrate_api-2.2.0/orchestrate/_internal/terminology.py`

 * *Files 1% similar despite different names*

```diff
@@ -324,14 +324,38 @@
     id: str
     resourceType: Literal["Bundle"]
     entry: list[_CodeSystemBundleEntry]
 
 
 SummarizeFhirR4CodeSystemsResponse = _CodeSystemBundle
 
+
+class ConceptMap(TypedDict):
+    resourceType: Literal["ConceptMap"]
+    id: str
+    name: str
+    status: Literal["active", "draft", "retired"]
+    url: str
+    source: str
+    target: str
+    group: list[dict[str, Any]]
+
+
+class _ConceptMapBundleEntry(TypedDict):
+    resource: ConceptMap
+
+
+class ConceptMapBundle(TypedDict):
+    id: str
+    resourceType: Literal["Bundle"]
+    entry: list[_ConceptMapBundleEntry]
+
+
+GetFhirR4ConceptMapsResponse = ConceptMapBundle
+
 TranslateFhirR4ConceptMapResponse = Parameters
 
 TranslateDomains = Literal[
     "Condition",
     "AllergyIntolerance",
     "MedicationDispense",
     "MedicationAdministration",
@@ -1174,15 +1198,15 @@
             path="/terminology/v1/fhir/r4/codesystem", parameters={"_summary": "true"}
         )
 
     def get_fhir_r4_concept_maps(
         self,
         page_number: Optional[int] = None,
         page_size: Optional[int] = None,
-    ) -> GetFhirR4CodeSystemResponse:
+    ) -> GetFhirR4ConceptMapsResponse:
         """
         Describes available concept maps
 
         ### Returns
 
         A bundle of known ConceptMaps
```

### Comparing `orchestrate_api-2.1.0/orchestrate/terminology.py` & `orchestrate_api-2.2.0/orchestrate/terminology.py`

 * *Files identical despite different names*

### Comparing `orchestrate_api-2.1.0/pyproject.toml` & `orchestrate_api-2.2.0/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -8,28 +8,36 @@
 keywords = ["careevolution", "rosetta", "orchestrate"]
 license = "Apache-2.0"
 name = "orchestrate-api"
 packages = [
   {include = "orchestrate"},
 ]
 readme = "README.md"
-version = "2.1.0"
+version = "2.2.0"
 
 [tool.poetry.dependencies]
 python = "^3.9"
 requests = "^2.31.0"
 typing-extensions = {version = "^4.0.1", python = "<3.11"}
 
 [tool.poetry.group.dev.dependencies]
 black = ">=23.7,<25.0"
 mypy = "^1.4.1"
 notebook = "^7.0.0"
+pytest-xdist = "^3.6.1"
 python-dotenv = "^1.0.0"
 types-requests = "^2.31.0.2"
 
 [tool.poetry.group.test.dependencies]
 pytest = ">=7.4,<9.0"
 python-dotenv = "^1.0.0"
 
 [build-system]
 build-backend = "poetry.core.masonry.api"
 requires = ["poetry-core"]
+
+[tool.pytest.ini_options]
+addopts = "-n 4 -m default"
+markers = [
+  "e2e",
+  "default",
+]
```

### Comparing `orchestrate_api-2.1.0/PKG-INFO` & `orchestrate_api-2.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: orchestrate-api
-Version: 2.1.0
+Version: 2.2.0
 Summary: SDK for the Orchestrate API at api.careevolutionapi.com
 Home-page: https://rosetta-api.docs.careevolution.com/
 License: Apache-2.0
 Keywords: careevolution,rosetta,orchestrate
 Author: Jeremy Fortune
 Author-email: jeremy@careevolution.com
 Requires-Python: >=3.9,<4.0
```

