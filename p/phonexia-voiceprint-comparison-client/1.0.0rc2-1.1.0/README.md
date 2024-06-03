# Comparing `tmp/phonexia_voiceprint_comparison_client-1.0.0rc2.tar.gz` & `tmp/phonexia_voiceprint_comparison_client-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "phonexia_voiceprint_comparison_client-1.0.0rc2.tar", max compression
+gzip compressed data, was "phonexia_voiceprint_comparison_client-1.1.0.tar", max compression
```

## Comparing `phonexia_voiceprint_comparison_client-1.0.0rc2.tar` & `phonexia_voiceprint_comparison_client-1.1.0.tar`

### file list

```diff
@@ -1,4 +1,4 @@
--rw-r--r--   0        0        0     4680 2023-11-27 14:30:57.838687 phonexia_voiceprint_comparison_client-1.0.0rc2/phonexia_voiceprint_comparison_client.py
--rw-r--r--   0        0        0      971 2023-11-27 14:30:57.838687 phonexia_voiceprint_comparison_client-1.0.0rc2/pypi-README.md
--rw-r--r--   0        0        0     1867 2023-11-27 14:31:19.725949 phonexia_voiceprint_comparison_client-1.0.0rc2/pyproject.toml
--rw-r--r--   0        0        0     1893 1970-01-01 00:00:00.000000 phonexia_voiceprint_comparison_client-1.0.0rc2/PKG-INFO
+-rw-r--r--   0        0        0     5809 2024-06-03 06:49:03.469912 phonexia_voiceprint_comparison_client-1.1.0/phonexia_voiceprint_comparison_client.py
+-rw-r--r--   0        0        0      996 2024-06-03 06:49:03.469912 phonexia_voiceprint_comparison_client-1.1.0/pypi-README.md
+-rw-r--r--   0        0        0     1882 2024-06-03 06:49:21.939138 phonexia_voiceprint_comparison_client-1.1.0/pyproject.toml
+-rw-r--r--   0        0        0     1979 1970-01-01 00:00:00.000000 phonexia_voiceprint_comparison_client-1.1.0/PKG-INFO
```

### Comparing `phonexia_voiceprint_comparison_client-1.0.0rc2/phonexia_voiceprint_comparison_client.py` & `phonexia_voiceprint_comparison_client-1.1.0/phonexia_voiceprint_comparison_client.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 #!/usr/bin/env python3
 
 import argparse
+import json
+import logging
 import os
 from itertools import zip_longest
-import logging
-from typing import Iterator
+from typing import Iterator, Optional
 
 import grpc
 import numpy as np
 import phonexia.grpc.common.core_pb2 as phx_common
 import phonexia.grpc.technologies.speaker_identification.v1.speaker_identification_pb2 as sid
 import phonexia.grpc.technologies.speaker_identification.v1.speaker_identification_pb2_grpc as sid_grpc
 
@@ -50,43 +51,55 @@
             batch_size += 1
 
     # Yield the last request if it contains any voiceprints
     if len(request.voiceprints_a) or len(request.voiceprints_b):
         yield request
 
 
-def print_scores(row: int, cols: int, result: list) -> None:
-    print("Score:")
-    mat = np.array(result).reshape(row, cols)
-    for row in mat:
-        for val in row:
-            print(f"{val:7.1f}", end=" ")
-        print("")
-
-
-def compare_one_to_one(file1: str, file2: str, channel: grpc.Channel) -> None:
+def print_scores(rows: int, cols: int, result: list, to_json: bool = False) -> None:
+    mat = np.array(result).reshape(rows, cols)
+    if to_json:
+        score = {"score": mat.tolist()}
+        print(json.dumps(score, indent=2))
+    else:
+        print("Score:")
+        for row in mat:
+            for val in row:
+                print(f"{val:7.1f}", end=" ")
+            print("")
+
+
+def compare_one_to_one(
+    file1: str, file2: str, channel: grpc.Channel, metadata: Optional[list], to_json: bool = False
+) -> None:
     stub = stub = sid_grpc.VoiceprintComparisonStub(channel)
-    result = stub.Compare(make_request(iter([file1]), iter([file2])))
+    result = stub.Compare(make_request(iter([file1]), iter([file2])), metadata=metadata)
     for res in result:
-        print_scores(1, 1, [res.scores.values])
+        print_scores(1, 1, [res.scores.values], to_json)
 
 
-def compare_m_to_n(list1: Iterator[str], list2: Iterator[str], channel: grpc.Channel) -> None:
+def compare_m_to_n(
+    list1: Iterator[str],
+    list2: Iterator[str],
+    channel: grpc.Channel,
+    metadata: Optional[list],
+    to_json: bool = False,
+) -> None:
     stub = sid_grpc.VoiceprintComparisonStub(channel)
     n_rows = 0
     n_cols = 0
     scores = []
     requests = make_request(list1, list2)
-    for result in stub.Compare(requests):
+    for result in stub.Compare(requests, metadata=metadata):
         if result.scores.rows_count:
             n_rows = result.scores.rows_count
             n_cols = result.scores.columns_count
         scores.extend(result.scores.values)
 
-    print_scores(n_rows, n_cols, scores)
+    print_scores(n_rows, n_cols, scores, to_json)
 
 
 def main():
     parser = argparse.ArgumentParser(
         description="Voiceprint Comparison gRPC client. Compares voiceprints and returns scores.",
     )
     input_group = parser.add_mutually_exclusive_group(required=True)
@@ -103,14 +116,22 @@
     parser.add_argument(
         "-l",
         "--log_level",
         type=str,
         default="error",
         choices=["critical", "error", "warning", "info", "debug"],
     )
+    parser.add_argument(
+        "--metadata",
+        metavar="key=value",
+        nargs="+",
+        type=lambda x: tuple(x.split("=")),
+        help="Custom client metadata",
+    )
+    parser.add_argument("--to_json", action="store_true", help="Output comparison to json")
     parser.add_argument("--use_ssl", action="store_true", help="Use SSL connection")
     args = parser.parse_args()
 
     logging.basicConfig(
         level=args.log_level.upper(),
         format="[%(asctime)s.%(msecs)03d] [%(levelname)s] %(message)s",
         datefmt="%Y-%m-%d %H:%M:%S",
@@ -119,23 +140,39 @@
     try:
         logging.info(f"Connecting to {args.host}")
         if args.use_ssl:
             with grpc.secure_channel(
                 target=args.host, credentials=grpc.ssl_channel_credentials()
             ) as channel:
                 if args.files:
-                    compare_one_to_one(args.files[0], args.files[1], channel)
+                    compare_one_to_one(
+                        args.files[0], args.files[1], channel, args.metadata, args.to_json
+                    )
                 elif args.lists:
-                    compare_m_to_n(list_reader(args.lists[0]), list_reader(args.lists[1]), channel)
+                    compare_m_to_n(
+                        list_reader(args.lists[0]),
+                        list_reader(args.lists[1]),
+                        channel,
+                        args.metadata,
+                        args.to_json,
+                    )
         else:
             with grpc.insecure_channel(target=args.host) as channel:
                 if args.files:
-                    compare_one_to_one(args.files[0], args.files[1], channel)
+                    compare_one_to_one(
+                        args.files[0], args.files[1], channel, args.metadata, args.to_json
+                    )
                 elif args.lists:
-                    compare_m_to_n(list_reader(args.lists[0]), list_reader(args.lists[1]), channel)
+                    compare_m_to_n(
+                        list_reader(args.lists[0]),
+                        list_reader(args.lists[1]),
+                        channel,
+                        args.metadata,
+                        args.to_json,
+                    )
 
     except grpc.RpcError:
         logging.exception("RPC failed")
         exit(1)
     except Exception:
         logging.exception("Unknown error")
         exit(1)
```

### Comparing `phonexia_voiceprint_comparison_client-1.0.0rc2/pypi-README.md` & `phonexia_voiceprint_comparison_client-1.1.0/pypi-README.md`

 * *Files 16% similar despite different names*

```diff
@@ -3,10 +3,10 @@
 
 # Phonexia voiceprint comparison client
 
 This module contains client for communication with [voiceprint comparison microservice](https://hub.docker.com/repository/docker/phonexia/voiceprint-comparison/general) developed by [Phonexia](https://phonexia.com).
 
 To use this client you will first need a running instance of any *Phonexia voiceprint comparison microservice*. If you don't yet have any running instance, don't hesitate to [contact our sales department](mailto:info@phonexia.com).
 
-You can learn more about the speaker identification technology [here](https://docs.cloud.phonexia.com/docs/common/technologies/speaker-identification).
+You can learn more about the speaker identification technology [here](https://docs.cloud.phonexia.com/docs/technologies/speaker-identification/).
 
-On [this page](https://docs.cloud.phonexia.com/docs/grpc/phonexia/grpc/technologies/speaker_identification/v1/speaker_identification.proto#voiceprintcomparison), you will find a *gRPC API* reference for *voiceprint comparison microservice*.
+On [this page](https://docs.cloud.phonexia.com/docs/products/speech-platform-4/grpc/api/phonexia/grpc/technologies/speaker_identification/v1/speaker_identification.proto#voiceprintcomparison), you will find a *gRPC API* reference for *voiceprint comparison microservice*.
```

### Comparing `phonexia_voiceprint_comparison_client-1.0.0rc2/pyproject.toml` & `phonexia_voiceprint_comparison_client-1.1.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 [tool.poetry]
 name = "phonexia-voiceprint-comparison-client"
-version = "1.0.0rc2"
+version = "1.1.0"
 description = "Client for communication with Phonexia voiceprint comparison microservice."
 readme = "pypi-README.md"
 keywords = ["grpc", "voice", "voice-biometry", "speech", "language", "identification"]
 authors = ["Phonexia <info@phonexia.com>"]
 
 [tool.poetry.urls]
 Homepage = "https://phonexia.com"
 Issues = "https://phonexia.atlassian.net/servicedesk/customer/portal/15/group/20/create/40"
-# protofiles = "link to protofiles"
+protofiles = "https://github.com/phonexia/protofiles"
 
 [tool.poetry.scripts]
 voiceprint_comparison_client = 'phonexia_voiceprint_comparison_client:main'
 
 [tool.poetry.dependencies]
 python = ">=3.8,<4.0"
 grpcio = "^1.54.0"
-phonexia-grpc = {version="^1.0.0", source="pypi"}
+phonexia-grpc = {version="^2.0.0", source="pypi"}
 numpy = "^1.26"
 
 [tool.poetry.group.dev.dependencies]
-pytest = "^7.2.0"
-pytest-cov = "^4.0.0"
+pytest = "^8.0.0"
+pytest-cov = "^5.0.0"
 pytest-env = "^1.0.0"
 pytest-random-order = "^1.1.0"
-black = "^23.3.0"
-ruff = "^0.1.0"
+black = "^24.0.0"
+ruff = "^0.3.0"
 
 [[tool.poetry.source]]
 name = "gitlab"
 url = "https://gitlab.cloud.phonexia.com/api/v4/groups/39/-/packages/pypi/simple"
 priority = "primary"
```

### Comparing `phonexia_voiceprint_comparison_client-1.0.0rc2/PKG-INFO` & `phonexia_voiceprint_comparison_client-1.1.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,33 +1,34 @@
 Metadata-Version: 2.1
 Name: phonexia-voiceprint-comparison-client
-Version: 1.0.0rc2
+Version: 1.1.0
 Summary: Client for communication with Phonexia voiceprint comparison microservice.
 Keywords: grpc,voice,voice-biometry,speech,language,identification
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
 Requires-Dist: numpy (>=1.26,<2.0)
-Requires-Dist: phonexia-grpc (>=1.0.0,<2.0.0)
+Requires-Dist: phonexia-grpc (>=2.0.0,<3.0.0)
 Project-URL: Homepage, https://phonexia.com
 Project-URL: Issues, https://phonexia.atlassian.net/servicedesk/customer/portal/15/group/20/create/40
+Project-URL: protofiles, https://github.com/phonexia/protofiles
 Description-Content-Type: text/markdown
 
 
 ![](https://www.phonexia.com/wp-content/uploads/phonexia-logo-transparent-500px.png)
 
 # Phonexia voiceprint comparison client
 
 This module contains client for communication with [voiceprint comparison microservice](https://hub.docker.com/repository/docker/phonexia/voiceprint-comparison/general) developed by [Phonexia](https://phonexia.com).
 
 To use this client you will first need a running instance of any *Phonexia voiceprint comparison microservice*. If you don't yet have any running instance, don't hesitate to [contact our sales department](mailto:info@phonexia.com).
 
-You can learn more about the speaker identification technology [here](https://docs.cloud.phonexia.com/docs/common/technologies/speaker-identification).
+You can learn more about the speaker identification technology [here](https://docs.cloud.phonexia.com/docs/technologies/speaker-identification/).
 
-On [this page](https://docs.cloud.phonexia.com/docs/grpc/phonexia/grpc/technologies/speaker_identification/v1/speaker_identification.proto#voiceprintcomparison), you will find a *gRPC API* reference for *voiceprint comparison microservice*.
+On [this page](https://docs.cloud.phonexia.com/docs/products/speech-platform-4/grpc/api/phonexia/grpc/technologies/speaker_identification/v1/speaker_identification.proto#voiceprintcomparison), you will find a *gRPC API* reference for *voiceprint comparison microservice*.
```

