# Comparing `tmp/dynatrace_opentelemetry_core-1.289.2-py3-none-any.whl.zip` & `tmp/dynatrace_opentelemetry_core-1.291.2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
-Zip file size: 281986 bytes, number of entries: 109
+Zip file size: 281982 bytes, number of entries: 109
 -rw-r--r--  2.0 unx     1706 b- defN 20-Feb-02 00:00 dynatrace/_vendor/google/protobuf/__init__.py
 -rw-r--r--  2.0 unx       24 b- defN 20-Feb-02 00:00 dynatrace/_vendor/google/protobuf/_version.py
 -rw-r--r--  2.0 unx     1449 b- defN 20-Feb-02 00:00 dynatrace/_vendor/google/protobuf/any_pb2.py
 -rw-r--r--  2.0 unx     2857 b- defN 20-Feb-02 00:00 dynatrace/_vendor/google/protobuf/api_pb2.py
 -rw-r--r--  2.0 unx    46761 b- defN 20-Feb-02 00:00 dynatrace/_vendor/google/protobuf/descriptor.py
 -rw-r--r--  2.0 unx     6819 b- defN 20-Feb-02 00:00 dynatrace/_vendor/google/protobuf/descriptor_database.py
 -rw-r--r--  2.0 unx   116074 b- defN 20-Feb-02 00:00 dynatrace/_vendor/google/protobuf/descriptor_pb2.py
@@ -100,12 +100,12 @@
 -rw-r--r--  2.0 unx     3559 b- defN 20-Feb-02 00:00 dynatrace/opentelemetry/tracing/_util/byteops.py
 -rw-r--r--  2.0 unx     3661 b- defN 20-Feb-02 00:00 dynatrace/opentelemetry/tracing/_util/context.py
 -rw-r--r--  2.0 unx     6002 b- defN 20-Feb-02 00:00 dynatrace/opentelemetry/tracing/_util/exceptions.py
 -rw-r--r--  2.0 unx     3287 b- defN 20-Feb-02 00:00 dynatrace/opentelemetry/tracing/_util/hashes.py
 -rw-r--r--  2.0 unx     2577 b- defN 20-Feb-02 00:00 dynatrace/opentelemetry/tracing/_util/http.py
 -rw-r--r--  2.0 unx     3307 b- defN 20-Feb-02 00:00 dynatrace/opentelemetry/tracing/_util/meta.py
 -rw-r--r--  2.0 unx     1626 b- defN 20-Feb-02 00:00 dynatrace/opentelemetry/tracing/_util/tenant.py
-?rw-r--r--  2.0 unx     1204 b- defN 20-Feb-02 00:00 dynatrace_opentelemetry_core-1.289.2.dist-info/METADATA
-?rw-r--r--  2.0 unx       87 b- defN 20-Feb-02 00:00 dynatrace_opentelemetry_core-1.289.2.dist-info/WHEEL
-?rw-r--r--  2.0 unx    11342 b- defN 20-Feb-02 00:00 dynatrace_opentelemetry_core-1.289.2.dist-info/licenses/LICENSE
-?rw-r--r--  2.0 unx    11712 b- defN 20-Feb-02 00:00 dynatrace_opentelemetry_core-1.289.2.dist-info/RECORD
-109 files, 1028548 bytes uncompressed, 262530 bytes compressed:  74.5%
+?rw-r--r--  2.0 unx     1204 b- defN 20-Feb-02 00:00 dynatrace_opentelemetry_core-1.291.2.dist-info/METADATA
+?rw-r--r--  2.0 unx       87 b- defN 20-Feb-02 00:00 dynatrace_opentelemetry_core-1.291.2.dist-info/WHEEL
+?rw-r--r--  2.0 unx    11342 b- defN 20-Feb-02 00:00 dynatrace_opentelemetry_core-1.291.2.dist-info/licenses/LICENSE
+?rw-r--r--  2.0 unx    11712 b- defN 20-Feb-02 00:00 dynatrace_opentelemetry_core-1.291.2.dist-info/RECORD
+109 files, 1028548 bytes uncompressed, 262526 bytes compressed:  74.5%
```

## zipnote {}

```diff
@@ -309,20 +309,20 @@
 
 Filename: dynatrace/opentelemetry/tracing/_util/meta.py
 Comment: 
 
 Filename: dynatrace/opentelemetry/tracing/_util/tenant.py
 Comment: 
 
-Filename: dynatrace_opentelemetry_core-1.289.2.dist-info/METADATA
+Filename: dynatrace_opentelemetry_core-1.291.2.dist-info/METADATA
 Comment: 
 
-Filename: dynatrace_opentelemetry_core-1.289.2.dist-info/WHEEL
+Filename: dynatrace_opentelemetry_core-1.291.2.dist-info/WHEEL
 Comment: 
 
-Filename: dynatrace_opentelemetry_core-1.289.2.dist-info/licenses/LICENSE
+Filename: dynatrace_opentelemetry_core-1.291.2.dist-info/licenses/LICENSE
 Comment: 
 
-Filename: dynatrace_opentelemetry_core-1.289.2.dist-info/RECORD
+Filename: dynatrace_opentelemetry_core-1.291.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## dynatrace/opentelemetry/tracing/version.py

```diff
@@ -1,7 +1,7 @@
-__version__ = "1.289.2"
+__version__ = "1.291.2"
 
-FULL_VERSION = "1.289.2.20240322-043008"
-BUILD_DATE = "2024.03.22 04:30:08"
-SCM_REVISION = "2550eb48efff690c97f0a6a80daa4140c309e609"
+FULL_VERSION = "1.291.2.20240419-043530"
+BUILD_DATE = "2024.04.19 04:35:30"
+SCM_REVISION = "3615a079fc3124875de4e5b2fc26fc1b0998f2a0"
 IS_DEV_VERSION = False
 IS_PACKAGE_MODE = True
```

## Comparing `dynatrace_opentelemetry_core-1.289.2.dist-info/METADATA` & `dynatrace_opentelemetry_core-1.291.2.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: dynatrace-opentelemetry-core
-Version: 1.289.2
+Version: 1.291.2
 Summary: Dynatrace OpenTelemetry core package
 Project-URL: Homepage, https://www.dynatrace.com/technologies/python-monitoring/
 Author: Dynatrace
 License-Expression: Apache-2.0
 License-File: LICENSE
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

## Comparing `dynatrace_opentelemetry_core-1.289.2.dist-info/licenses/LICENSE` & `dynatrace_opentelemetry_core-1.291.2.dist-info/licenses/LICENSE`

 * *Files identical despite different names*

## Comparing `dynatrace_opentelemetry_core-1.289.2.dist-info/RECORD` & `dynatrace_opentelemetry_core-1.291.2.dist-info/RECORD`

 * *Files 2% similar despite different names*

```diff
@@ -61,15 +61,15 @@
 dynatrace/odin/proto/trace/v1/trace_pb2.py,sha256=xFXu6VknTx4IEE5lDrOyGp-syGo9uPmMmmOLSydUZec,5808
 dynatrace/odin/semconv/_version.py,sha256=65mKDHQqSD9iQ6jJ9l9tzVDIbb2fEIQ2LBKY3KVcUK8,39
 dynatrace/odin/semconv/v1/__init__.py,sha256=l-wGJH3OGhJj4nhz7Px0Fa8lTDD8C1CgzyG_tf-YSHs,62508
 dynatrace/opentelemetry/tracing/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 dynatrace/opentelemetry/tracing/api.py,sha256=c7Rb1TkphWCUqKerxW5E310Smvj-VBqIfJsJlu5VEtk,1012
 dynatrace/opentelemetry/tracing/api.pyi,sha256=QkVFJRNMk2p5loY3VO5rCFHQxz8MacstxiWQzKY2DfY,1678
 dynatrace/opentelemetry/tracing/py.typed,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-dynatrace/opentelemetry/tracing/version.py,sha256=TWomcuyDgSelxzt0XhdxgOuU0vAdUwxZJffhE8LArBM,205
+dynatrace/opentelemetry/tracing/version.py,sha256=KfOfualYfnf0k9jAHAXm_-zQd6v-UZwAwTpSaAJyfag,205
 dynatrace/opentelemetry/tracing/_config/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 dynatrace/opentelemetry/tracing/_config/banner.py,sha256=HKXTTNkvvSy8j1Kwik_9kbjqve9RaivwNNSfbnn4H2U,3752
 dynatrace/opentelemetry/tracing/_config/configure.py,sha256=zC2p9ba7isZh-aOnfwd0Y9Fx5k2Njx0iagSzqt9ncgU,1780
 dynatrace/opentelemetry/tracing/_config/reader.py,sha256=52wMwG_9MbS97y0H4OeG4d7uWgBfyEfB6o4AkraVGKE,10949
 dynatrace/opentelemetry/tracing/_config/settings.py,sha256=ubM2q6okDQiUYIe9ZLtgKyWYWVqeRUvxbEf7JzGZdaU,20103
 dynatrace/opentelemetry/tracing/_export/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 dynatrace/opentelemetry/tracing/_export/exporter.py,sha256=T3aWOs1GFtHUoqcJXm123RN3-ZThjRzEoRMf-Wltpr0,13853
@@ -99,11 +99,11 @@
 dynatrace/opentelemetry/tracing/_util/byteops.py,sha256=d9NPDsMmu338laXMgDjX4EIooSeEvgXkdneQLm9-Qhs,3559
 dynatrace/opentelemetry/tracing/_util/context.py,sha256=RjrJeY_L5v3kyhRSd7fFC6cBgJEsclbIabqwgeMbHlc,3661
 dynatrace/opentelemetry/tracing/_util/exceptions.py,sha256=XLYTvsqoNfhHeHheSFTizqQKaltYDqCuseGITDXz-aA,6002
 dynatrace/opentelemetry/tracing/_util/hashes.py,sha256=Ea7W7XVS1iOdp85qlaqK9ue3YLSJJvErkb4Ja646sqc,3287
 dynatrace/opentelemetry/tracing/_util/http.py,sha256=txTmLF-Z4Px58yFmC-nrmsO-_lYDkDc0FQLkH9tFMII,2577
 dynatrace/opentelemetry/tracing/_util/meta.py,sha256=BkkQp6X6JgkH6beoUJqSfNovZd3LAT8FGKo7s8mAjOA,3307
 dynatrace/opentelemetry/tracing/_util/tenant.py,sha256=tIuLrPLpD3rhcBzv3i7inj4LIP6mgeRWY72DLL_DKvU,1626
-dynatrace_opentelemetry_core-1.289.2.dist-info/METADATA,sha256=NU-H3SQCnmnYS19ptm275ZEkuoMa9Hj0qX7UUDPtGBw,1204
-dynatrace_opentelemetry_core-1.289.2.dist-info/WHEEL,sha256=bq9SyP5NxIRA9EpQgMCd-9RmPHWvbH-4lTDGwxgIR64,87
-dynatrace_opentelemetry_core-1.289.2.dist-info/licenses/LICENSE,sha256=OUyLShRPZFGLXlxbnRr7Of_8mNYYQ_qda632uhGSIaY,11342
-dynatrace_opentelemetry_core-1.289.2.dist-info/RECORD,,
+dynatrace_opentelemetry_core-1.291.2.dist-info/METADATA,sha256=RTO614E93jhLS110-5F2nDFSUyxALA5cSqo5ThPYcCA,1204
+dynatrace_opentelemetry_core-1.291.2.dist-info/WHEEL,sha256=osohxoshIHTFJFVPhsi1UkZuLRGMHRXZzwEBW2ezjrc,87
+dynatrace_opentelemetry_core-1.291.2.dist-info/licenses/LICENSE,sha256=OUyLShRPZFGLXlxbnRr7Of_8mNYYQ_qda632uhGSIaY,11342
+dynatrace_opentelemetry_core-1.291.2.dist-info/RECORD,,
```

