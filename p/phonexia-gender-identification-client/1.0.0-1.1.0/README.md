# Comparing `tmp/phonexia_gender_identification_client-1.0.0.tar.gz` & `tmp/phonexia_gender_identification_client-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "phonexia_gender_identification_client-1.0.0.tar", max compression
+gzip compressed data, was "phonexia_gender_identification_client-1.1.0.tar", max compression
```

## Comparing `phonexia_gender_identification_client-1.0.0.tar` & `phonexia_gender_identification_client-1.1.0.tar`

### file list

```diff
@@ -1,4 +1,4 @@
--rw-r--r--   0        0        0     2903 2024-03-28 14:11:18.712977 phonexia_gender_identification_client-1.0.0/phonexia_gender_identification_client.py
--rw-r--r--   0        0        0      924 2024-03-28 14:11:18.712977 phonexia_gender_identification_client-1.0.0/pypi-README.md
--rw-r--r--   0        0        0     1896 2024-03-28 14:11:34.178211 phonexia_gender_identification_client-1.0.0/pyproject.toml
--rw-r--r--   0        0        0     1900 1970-01-01 00:00:00.000000 phonexia_gender_identification_client-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0     3065 2024-06-03 07:01:10.280265 phonexia_gender_identification_client-1.1.0/phonexia_gender_identification_client.py
+-rw-r--r--   0        0        0      924 2024-06-03 07:01:10.280265 phonexia_gender_identification_client-1.1.0/pypi-README.md
+-rw-r--r--   0        0        0     1930 2024-06-03 07:01:30.822613 phonexia_gender_identification_client-1.1.0/pyproject.toml
+-rw-r--r--   0        0        0     1900 1970-01-01 00:00:00.000000 phonexia_gender_identification_client-1.1.0/PKG-INFO
```

### Comparing `phonexia_gender_identification_client-1.0.0/phonexia_gender_identification_client.py` & `phonexia_gender_identification_client-1.1.0/phonexia_gender_identification_client.py`

 * *Files 12% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 import logging
 from typing import Iterator, Optional
 
 import grpc
 import phonexia.grpc.common.core_pb2 as phx_common
 import phonexia.grpc.technologies.gender_identification.v1.gender_identification_pb2 as gid
 import phonexia.grpc.technologies.gender_identification.v1.gender_identification_pb2_grpc as gid_grpc
+from google.protobuf.json_format import MessageToJson
 
 MAX_BATCH_SIZE = 1024
 
 
 def parse_vp(path: str) -> phx_common.Voiceprint:
     with open(path, mode="rb") as file:
         return phx_common.Voiceprint(content=file.read())
@@ -31,15 +32,15 @@
         yield request
 
 
 def identify_gender(voiceprint_file: str, channel: grpc.Channel, metadata: Optional[list]):
     stub = gid_grpc.GenderIdentificationStub(channel)
     batch_request = make_batch_request(iter([voiceprint_file]))
     for result in stub.Identify(batch_request, metadata=metadata):
-        print(result)
+        print(MessageToJson(result))
 
 
 def main():
     parser = argparse.ArgumentParser(
         description="Gender Identification gRPC client. Identifies gender from input voiceprint.",
     )
     parser.add_argument("-f", "--file", type=str, help="Voiceprint from which to identify gender")
@@ -63,14 +64,17 @@
         nargs="+",
         type=lambda x: tuple(x.split("=")),
         help="Custom client metadata",
     )
     parser.add_argument("--use_ssl", action="store_true", help="Use SSL connection")
     args = parser.parse_args()
 
+    if not args.file:
+        raise ValueError("Parameter --file must not be empty string")
+
     logging.basicConfig(
         level=args.log_level.upper(),
         format="[%(asctime)s.%(msecs)03d] [%(levelname)s] %(message)s",
         datefmt="%Y-%m-%d %H:%M:%S",
     )
 
     try:
```

### Comparing `phonexia_gender_identification_client-1.0.0/pypi-README.md` & `phonexia_gender_identification_client-1.1.0/pypi-README.md`

 * *Files identical despite different names*

### Comparing `phonexia_gender_identification_client-1.0.0/pyproject.toml` & `phonexia_gender_identification_client-1.1.0/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "phonexia-gender-identification-client"
-version = "1.0.0"
+version = "1.1.0"
 description = "Client script for communicationg with Phonexia gender identification microservice."
 readme = "pypi-README.md"
 keywords = ["grpc", "voice", "voice-biometry", "speech", "gender", "identification", "gender identification"]
 authors = ["Phonexia <info@phonexia.com>"]
 
 [tool.poetry.urls]
 Homepage = "https://phonexia.com"
@@ -13,23 +13,23 @@
 
 [tool.poetry.scripts]
 gender_identification_client = 'phonexia_gender_identification_client:main'
 
 [tool.poetry.dependencies]
 python = ">=3.8,<4.0"
 grpcio = "^1.54.0"
-phonexia-grpc = {version="^1.0.0", source="pypi"}
+phonexia-grpc = {version="^2.0.0", source="pypi"}
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^8.0.0"
 pytest-cov = "^5.0.0"
 pytest-env = "^1.0.0"
 pytest-random-order = "^1.1.0"
 black = "^24.0.0"
-ruff = "^0.3.0"
+ruff = "^0.4.0"
 
 [[tool.poetry.source]]
 name = "gitlab"
 url = "https://gitlab.cloud.phonexia.com/api/v4/groups/39/-/packages/pypi/simple"
 priority = "primary"
 
 [[tool.poetry.source]]
@@ -82,8 +82,10 @@
     "TRY",
 ]
 ignore = [
     # LineTooLong
     "E501",
     # DoNotAssignLambda
     "E731",
+    # long messages
+    "TRY003",
 ]
```

### Comparing `phonexia_gender_identification_client-1.0.0/PKG-INFO` & `phonexia_gender_identification_client-1.1.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: phonexia-gender-identification-client
-Version: 1.0.0
+Version: 1.1.0
 Summary: Client script for communicationg with Phonexia gender identification microservice.
 Keywords: grpc,voice,voice-biometry,speech,gender,identification,gender identification
 Author: Phonexia
 Author-email: info@phonexia.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: grpcio (>=1.54.0,<2.0.0)
-Requires-Dist: phonexia-grpc (>=1.0.0,<2.0.0)
+Requires-Dist: phonexia-grpc (>=2.0.0,<3.0.0)
 Project-URL: Homepage, https://phonexia.com
 Project-URL: Issues, https://phonexia.atlassian.net/servicedesk/customer/portal/15/group/20/create/40
 Project-URL: protofiles, https://github.com/phonexia/protofiles
 Description-Content-Type: text/markdown
 
 
 ![](https://www.phonexia.com/wp-content/uploads/phonexia-logo-transparent-500px.png)
```

