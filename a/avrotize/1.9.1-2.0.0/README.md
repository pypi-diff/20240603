# Comparing `tmp/avrotize-1.9.1.tar.gz` & `tmp/avrotize-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "avrotize-1.9.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "avrotize-2.0.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `avrotize-1.9.1.tar` & `avrotize-2.0.0.tar`

### file list

```diff
@@ -1,71 +1,72 @@
--rw-r--r--   0        0        0    32506 2024-06-03 09:44:41.019177 avrotize-1.9.1/README.md
--rw-r--r--   0        0        0     2382 2024-06-03 09:44:41.023177 avrotize-1.9.1/avrotize/__init__.py
--rw-r--r--   0        0        0       88 2024-06-03 09:44:41.023177 avrotize-1.9.1/avrotize/__main__.py
--rw-r--r--   0        0        0      411 2024-06-03 09:44:47.179170 avrotize-1.9.1/avrotize/_version.py
--rw-r--r--   0        0        0     8386 2024-06-03 09:44:41.023177 avrotize-1.9.1/avrotize/asn1toavro.py
--rw-r--r--   0        0        0     4935 2024-06-03 09:44:41.023177 avrotize-1.9.1/avrotize/avrotize.py
--rw-r--r--   0        0        0    25693 2024-06-03 09:44:41.023177 avrotize-1.9.1/avrotize/avrotocpp.py
--rw-r--r--   0        0        0     3015 2024-06-03 09:44:41.023177 avrotize-1.9.1/avrotize/avrotocpp/CMakeLists.txt.jinja
--rw-r--r--   0        0        0       96 2024-06-03 09:44:41.023177 avrotize-1.9.1/avrotize/avrotocpp/build.bat.jinja
--rw-r--r--   0        0        0       73 2024-06-03 09:44:41.023177 avrotize-1.9.1/avrotize/avrotocpp/build.sh.jinja
--rw-r--r--   0        0        0     4621 2024-06-03 09:44:41.023177 avrotize-1.9.1/avrotize/avrotocpp/dataclass_body.jinja
--rw-r--r--   0        0        0      464 2024-06-03 09:44:41.023177 avrotize-1.9.1/avrotize/avrotocpp/vcpkg.json.jinja
--rw-r--r--   0        0        0    45098 2024-06-03 09:44:41.023177 avrotize-1.9.1/avrotize/avrotocsharp.py
--rw-r--r--   0        0        0     1980 2024-06-03 09:44:41.023177 avrotize-1.9.1/avrotize/avrotocsharp/class_test.cs.jinja
--rw-r--r--   0        0        0     8124 2024-06-03 09:44:41.023177 avrotize-1.9.1/avrotize/avrotocsharp/dataclass_core.jinja
--rw-r--r--   0        0        0      579 2024-06-03 09:44:41.023177 avrotize-1.9.1/avrotize/avrotocsharp/enum_test.cs.jinja
--rw-r--r--   0        0        0      807 2024-06-03 09:44:41.023177 avrotize-1.9.1/avrotize/avrotocsharp/project.csproj.jinja
--rw-r--r--   0        0        0     1440 2024-06-03 09:44:41.023177 avrotize-1.9.1/avrotize/avrotocsharp/project.sln.jinja
--rw-r--r--   0        0        0      663 2024-06-03 09:44:41.023177 avrotize-1.9.1/avrotize/avrotocsharp/testproject.csproj.jinja
--rw-r--r--   0        0        0     3689 2024-06-03 09:44:41.023177 avrotize-1.9.1/avrotize/avrotocsv.py
--rw-r--r--   0        0        0     7259 2024-06-03 09:44:41.023177 avrotize-1.9.1/avrotize/avrotodatapackage.py
--rw-r--r--   0        0        0    45933 2024-06-03 09:44:41.023177 avrotize-1.9.1/avrotize/avrotodb.py
--rw-r--r--   0        0        0    21879 2024-06-03 09:44:41.023177 avrotize-1.9.1/avrotize/avrotogo.py
--rw-r--r--   0        0        0      226 2024-06-03 09:44:41.023177 avrotize-1.9.1/avrotize/avrotogo/go_enum.jinja
--rw-r--r--   0        0        0      506 2024-06-03 09:44:41.023177 avrotize-1.9.1/avrotize/avrotogo/go_helpers.jinja
--rw-r--r--   0        0        0     4272 2024-06-03 09:44:41.023177 avrotize-1.9.1/avrotize/avrotogo/go_struct.jinja
--rw-r--r--   0        0        0     1206 2024-06-03 09:44:41.023177 avrotize-1.9.1/avrotize/avrotogo/go_test.jinja
--rw-r--r--   0        0        0      890 2024-06-03 09:44:41.023177 avrotize-1.9.1/avrotize/avrotogo/go_union.jinja
--rw-r--r--   0        0        0     7394 2024-06-03 09:44:41.023177 avrotize-1.9.1/avrotize/avrotographql.py
--rw-r--r--   0        0        0     9057 2024-06-03 09:44:41.023177 avrotize-1.9.1/avrotize/avrotoiceberg.py
--rw-r--r--   0        0        0    58799 2024-06-03 09:44:41.023177 avrotize-1.9.1/avrotize/avrotojava.py
--rw-r--r--   0        0        0    12249 2024-06-03 09:44:41.023177 avrotize-1.9.1/avrotize/avrotojs.py
--rw-r--r--   0        0        0    18104 2024-06-03 09:44:41.023177 avrotize-1.9.1/avrotize/avrotojsons.py
--rw-r--r--   0        0        0    16181 2024-06-03 09:44:41.023177 avrotize-1.9.1/avrotize/avrotokusto.py
--rw-r--r--   0        0        0     5348 2024-06-03 09:44:41.023177 avrotize-1.9.1/avrotize/avrotomd.py
--rw-r--r--   0        0        0      999 2024-06-03 09:44:41.023177 avrotize-1.9.1/avrotize/avrotomd/README.md.jinja
--rw-r--r--   0        0        0     6052 2024-06-03 09:44:41.023177 avrotize-1.9.1/avrotize/avrotools.py
--rw-r--r--   0        0        0     9088 2024-06-03 09:44:41.023177 avrotize-1.9.1/avrotize/avrotoparquet.py
--rw-r--r--   0        0        0    22433 2024-06-03 09:44:41.023177 avrotize-1.9.1/avrotize/avrotoproto.py
--rw-r--r--   0        0        0    19239 2024-06-03 09:44:41.023177 avrotize-1.9.1/avrotize/avrotopython.py
--rw-r--r--   0        0        0    22173 2024-06-03 09:44:41.023177 avrotize-1.9.1/avrotize/avrotorust.py
--rw-r--r--   0        0        0     2232 2024-06-03 09:44:41.023177 avrotize-1.9.1/avrotize/avrotorust/dataclass_enum.rs.jinja
--rw-r--r--   0        0        0     7853 2024-06-03 09:44:41.023177 avrotize-1.9.1/avrotize/avrotorust/dataclass_struct.rs.jinja
--rw-r--r--   0        0        0     3801 2024-06-03 09:44:41.023177 avrotize-1.9.1/avrotize/avrotorust/dataclass_union.rs.jinja
--rw-r--r--   0        0        0    27698 2024-06-03 09:44:41.023177 avrotize-1.9.1/avrotize/avrotots.py
--rw-r--r--   0        0        0    16420 2024-06-03 09:44:41.023177 avrotize-1.9.1/avrotize/avrotoxsd.py
--rw-r--r--   0        0        0    55158 2024-06-03 09:44:41.023177 avrotize-1.9.1/avrotize/commands.json
--rw-r--r--   0        0        0    18352 2024-06-03 09:44:41.023177 avrotize-1.9.1/avrotize/common.py
--rw-r--r--   0        0        0      112 2024-06-03 09:44:41.023177 avrotize-1.9.1/avrotize/constants.py
--rw-r--r--   0        0        0     4293 2024-06-03 09:44:41.023177 avrotize-1.9.1/avrotize/csvtoavro.py
--rw-r--r--   0        0        0     2607 2024-06-03 09:44:41.023177 avrotize-1.9.1/avrotize/datapackagetoavro.py
--rw-r--r--   0        0        0    19374 2024-06-03 09:44:41.023177 avrotize-1.9.1/avrotize/dependency_resolver.py
--rw-r--r--   0        0        0     1272 2024-06-03 09:44:41.023177 avrotize-1.9.1/avrotize/generic/generic.avsc
--rw-r--r--   0        0        0    95497 2024-06-03 09:44:41.027177 avrotize-1.9.1/avrotize/jsonstoavro.py
--rw-r--r--   0        0        0     2856 2024-06-03 09:44:41.027177 avrotize-1.9.1/avrotize/kstructtoavro.py
--rw-r--r--   0        0        0    21399 2024-06-03 09:44:41.027177 avrotize-1.9.1/avrotize/kustotoavro.py
--rw-r--r--   0        0        0     5531 2024-06-03 09:44:41.027177 avrotize-1.9.1/avrotize/parquettoavro.py
--rw-r--r--   0        0        0    19742 2024-06-03 09:44:41.027177 avrotize-1.9.1/avrotize/proto2parser.py
--rw-r--r--   0        0        0    15536 2024-06-03 09:44:41.027177 avrotize-1.9.1/avrotize/proto3parser.py
--rw-r--r--   0        0        0    10535 2024-06-03 09:44:41.027177 avrotize-1.9.1/avrotize/prototoavro.py
--rw-r--r--   0        0        0     3390 2024-06-03 09:44:41.027177 avrotize-1.9.1/avrotize/prototypes/any.avsc
--rw-r--r--   0        0        0     6521 2024-06-03 09:44:41.027177 avrotize-1.9.1/avrotize/prototypes/api.avsc
--rw-r--r--   0        0        0     1629 2024-06-03 09:44:41.027177 avrotize-1.9.1/avrotize/prototypes/duration.avsc
--rw-r--r--   0        0        0     3558 2024-06-03 09:44:41.027177 avrotize-1.9.1/avrotize/prototypes/field_mask.avsc
--rw-r--r--   0        0        0     2394 2024-06-03 09:44:41.027177 avrotize-1.9.1/avrotize/prototypes/struct.avsc
--rw-r--r--   0        0        0      792 2024-06-03 09:44:41.027177 avrotize-1.9.1/avrotize/prototypes/timestamp.avsc
--rw-r--r--   0        0        0     6296 2024-06-03 09:44:41.027177 avrotize-1.9.1/avrotize/prototypes/type.avsc
--rw-r--r--   0        0        0     2571 2024-06-03 09:44:41.027177 avrotize-1.9.1/avrotize/prototypes/wrappers.avsc
--rw-r--r--   0        0        0    17638 2024-06-03 09:44:41.027177 avrotize-1.9.1/avrotize/xsdtoavro.py
--rw-r--r--   0        0        0     1507 2024-06-03 09:44:41.027177 avrotize-1.9.1/pyproject.toml
--rw-r--r--   0        0        0    34229 1970-01-01 00:00:00.000000 avrotize-1.9.1/PKG-INFO
+-rw-r--r--   0        0        0    32506 2024-06-02 22:25:26.819308 avrotize-2.0.0/README.md
+-rw-r--r--   0        0        0     2382 2024-06-02 22:25:26.819308 avrotize-2.0.0/avrotize/__init__.py
+-rw-r--r--   0        0        0       88 2024-06-02 22:25:26.819308 avrotize-2.0.0/avrotize/__main__.py
+-rw-r--r--   0        0        0      411 2024-06-02 22:25:31.119332 avrotize-2.0.0/avrotize/_version.py
+-rw-r--r--   0        0        0     8386 2024-06-02 22:25:26.819308 avrotize-2.0.0/avrotize/asn1toavro.py
+-rw-r--r--   0        0        0     4961 2024-06-02 22:25:26.819308 avrotize-2.0.0/avrotize/avrotize.py
+-rw-r--r--   0        0        0    25567 2024-06-02 22:25:26.819308 avrotize-2.0.0/avrotize/avrotocpp.py
+-rw-r--r--   0        0        0     3015 2024-06-02 22:25:26.819308 avrotize-2.0.0/avrotize/avrotocpp/CMakeLists.txt.jinja
+-rw-r--r--   0        0        0       96 2024-06-02 22:25:26.819308 avrotize-2.0.0/avrotize/avrotocpp/build.bat.jinja
+-rw-r--r--   0        0        0       73 2024-06-02 22:25:26.819308 avrotize-2.0.0/avrotize/avrotocpp/build.sh.jinja
+-rw-r--r--   0        0        0     4621 2024-06-02 22:25:26.819308 avrotize-2.0.0/avrotize/avrotocpp/dataclass_body.jinja
+-rw-r--r--   0        0        0      464 2024-06-02 22:25:26.819308 avrotize-2.0.0/avrotize/avrotocpp/vcpkg.json.jinja
+-rw-r--r--   0        0        0    45098 2024-06-02 22:25:26.819308 avrotize-2.0.0/avrotize/avrotocsharp.py
+-rw-r--r--   0        0        0     1980 2024-06-02 22:25:26.819308 avrotize-2.0.0/avrotize/avrotocsharp/class_test.cs.jinja
+-rw-r--r--   0        0        0     8124 2024-06-02 22:25:26.819308 avrotize-2.0.0/avrotize/avrotocsharp/dataclass_core.jinja
+-rw-r--r--   0        0        0      579 2024-06-02 22:25:26.819308 avrotize-2.0.0/avrotize/avrotocsharp/enum_test.cs.jinja
+-rw-r--r--   0        0        0      807 2024-06-02 22:25:26.819308 avrotize-2.0.0/avrotize/avrotocsharp/project.csproj.jinja
+-rw-r--r--   0        0        0     1440 2024-06-02 22:25:26.819308 avrotize-2.0.0/avrotize/avrotocsharp/project.sln.jinja
+-rw-r--r--   0        0        0      663 2024-06-02 22:25:26.819308 avrotize-2.0.0/avrotize/avrotocsharp/testproject.csproj.jinja
+-rw-r--r--   0        0        0     3551 2024-06-02 22:25:26.819308 avrotize-2.0.0/avrotize/avrotocsv.py
+-rw-r--r--   0        0        0     7259 2024-06-02 22:25:26.819308 avrotize-2.0.0/avrotize/avrotodatapackage.py
+-rw-r--r--   0        0        0    45933 2024-06-02 22:25:26.819308 avrotize-2.0.0/avrotize/avrotodb.py
+-rw-r--r--   0        0        0    21879 2024-06-02 22:25:26.819308 avrotize-2.0.0/avrotize/avrotogo.py
+-rw-r--r--   0        0        0      226 2024-06-02 22:25:26.819308 avrotize-2.0.0/avrotize/avrotogo/go_enum.jinja
+-rw-r--r--   0        0        0      506 2024-06-02 22:25:26.819308 avrotize-2.0.0/avrotize/avrotogo/go_helpers.jinja
+-rw-r--r--   0        0        0     4272 2024-06-02 22:25:26.819308 avrotize-2.0.0/avrotize/avrotogo/go_struct.jinja
+-rw-r--r--   0        0        0     1206 2024-06-02 22:25:26.819308 avrotize-2.0.0/avrotize/avrotogo/go_test.jinja
+-rw-r--r--   0        0        0      890 2024-06-02 22:25:26.819308 avrotize-2.0.0/avrotize/avrotogo/go_union.jinja
+-rw-r--r--   0        0        0     7394 2024-06-02 22:25:26.819308 avrotize-2.0.0/avrotize/avrotographql.py
+-rw-r--r--   0        0        0     9057 2024-06-02 22:25:26.819308 avrotize-2.0.0/avrotize/avrotoiceberg.py
+-rw-r--r--   0        0        0    58799 2024-06-02 22:25:26.819308 avrotize-2.0.0/avrotize/avrotojava.py
+-rw-r--r--   0        0        0    12117 2024-06-02 22:25:26.819308 avrotize-2.0.0/avrotize/avrotojs.py
+-rw-r--r--   0        0        0    18104 2024-06-02 22:25:26.819308 avrotize-2.0.0/avrotize/avrotojsons.py
+-rw-r--r--   0        0        0    16181 2024-06-02 22:25:26.819308 avrotize-2.0.0/avrotize/avrotokusto.py
+-rw-r--r--   0        0        0     5348 2024-06-02 22:25:26.819308 avrotize-2.0.0/avrotize/avrotomd.py
+-rw-r--r--   0        0        0      999 2024-06-02 22:25:26.819308 avrotize-2.0.0/avrotize/avrotomd/README.md.jinja
+-rw-r--r--   0        0        0     6052 2024-06-02 22:25:26.819308 avrotize-2.0.0/avrotize/avrotools.py
+-rw-r--r--   0        0        0     9088 2024-06-02 22:25:26.819308 avrotize-2.0.0/avrotize/avrotoparquet.py
+-rw-r--r--   0        0        0    22416 2024-06-02 22:25:26.819308 avrotize-2.0.0/avrotize/avrotoproto.py
+-rw-r--r--   0        0        0    19100 2024-06-02 22:25:26.819308 avrotize-2.0.0/avrotize/avrotopython.py
+-rw-r--r--   0        0        0    22029 2024-06-02 22:25:26.819308 avrotize-2.0.0/avrotize/avrotorust.py
+-rw-r--r--   0        0        0     2232 2024-06-02 22:25:26.819308 avrotize-2.0.0/avrotize/avrotorust/dataclass_enum.rs.jinja
+-rw-r--r--   0        0        0     7853 2024-06-02 22:25:26.819308 avrotize-2.0.0/avrotize/avrotorust/dataclass_struct.rs.jinja
+-rw-r--r--   0        0        0     3801 2024-06-02 22:25:26.819308 avrotize-2.0.0/avrotize/avrotorust/dataclass_union.rs.jinja
+-rw-r--r--   0        0        0    27554 2024-06-02 22:25:26.819308 avrotize-2.0.0/avrotize/avrotots.py
+-rw-r--r--   0        0        0    16420 2024-06-02 22:25:26.819308 avrotize-2.0.0/avrotize/avrotoxsd.py
+-rw-r--r--   0        0        0    50817 2024-06-02 22:25:26.819308 avrotize-2.0.0/avrotize/commands.json
+-rw-r--r--   0        0        0    18352 2024-06-02 22:25:26.819308 avrotize-2.0.0/avrotize/common.py
+-rw-r--r--   0        0        0      112 2024-06-02 22:25:26.819308 avrotize-2.0.0/avrotize/constants.py
+-rw-r--r--   0        0        0     6571 2024-06-02 22:25:26.819308 avrotize-2.0.0/avrotize/csvtoavro.py
+-rw-r--r--   0        0        0     2607 2024-06-02 22:25:26.819308 avrotize-2.0.0/avrotize/datapackagetoavro.py
+-rw-r--r--   0        0        0    19374 2024-06-02 22:25:26.819308 avrotize-2.0.0/avrotize/dependency_resolver.py
+-rw-r--r--   0        0        0     1272 2024-06-02 22:25:26.819308 avrotize-2.0.0/avrotize/generic/generic.avsc
+-rw-r--r--   0        0        0    95346 2024-06-02 22:25:26.823308 avrotize-2.0.0/avrotize/jsonstoavro.py
+-rw-r--r--   0        0        0     2112 2024-06-02 22:25:26.823308 avrotize-2.0.0/avrotize/kconnect.json
+-rw-r--r--   0        0        0     2537 2024-06-02 22:25:26.823308 avrotize-2.0.0/avrotize/kstructtoavro.py
+-rw-r--r--   0        0        0    21168 2024-06-02 22:25:26.823308 avrotize-2.0.0/avrotize/kustotoavro.py
+-rw-r--r--   0        0        0     5395 2024-06-02 22:25:26.823308 avrotize-2.0.0/avrotize/parquettoavro.py
+-rw-r--r--   0        0        0    19742 2024-06-02 22:25:26.823308 avrotize-2.0.0/avrotize/proto2parser.py
+-rw-r--r--   0        0        0    15536 2024-06-02 22:25:26.823308 avrotize-2.0.0/avrotize/proto3parser.py
+-rw-r--r--   0        0        0     8722 2024-06-02 22:25:26.823308 avrotize-2.0.0/avrotize/prototoavro.py
+-rw-r--r--   0        0        0     3390 2024-06-02 22:25:26.823308 avrotize-2.0.0/avrotize/prototypes/any.avsc
+-rw-r--r--   0        0        0     6521 2024-06-02 22:25:26.823308 avrotize-2.0.0/avrotize/prototypes/api.avsc
+-rw-r--r--   0        0        0     1629 2024-06-02 22:25:26.823308 avrotize-2.0.0/avrotize/prototypes/duration.avsc
+-rw-r--r--   0        0        0     3558 2024-06-02 22:25:26.823308 avrotize-2.0.0/avrotize/prototypes/field_mask.avsc
+-rw-r--r--   0        0        0     2394 2024-06-02 22:25:26.823308 avrotize-2.0.0/avrotize/prototypes/struct.avsc
+-rw-r--r--   0        0        0      792 2024-06-02 22:25:26.823308 avrotize-2.0.0/avrotize/prototypes/timestamp.avsc
+-rw-r--r--   0        0        0     6296 2024-06-02 22:25:26.823308 avrotize-2.0.0/avrotize/prototypes/type.avsc
+-rw-r--r--   0        0        0     2571 2024-06-02 22:25:26.823308 avrotize-2.0.0/avrotize/prototypes/wrappers.avsc
+-rw-r--r--   0        0        0    17371 2024-06-02 22:25:26.823308 avrotize-2.0.0/avrotize/xsdtoavro.py
+-rw-r--r--   0        0        0     1486 2024-06-02 22:25:26.823308 avrotize-2.0.0/pyproject.toml
+-rw-r--r--   0        0        0    34200 1970-01-01 00:00:00.000000 avrotize-2.0.0/PKG-INFO
```

### Comparing `avrotize-1.9.1/README.md` & `avrotize-2.0.0/README.md`

 * *Files identical despite different names*

### Comparing `avrotize-1.9.1/avrotize/__init__.py` & `avrotize-2.0.0/avrotize/__init__.py`

 * *Files identical despite different names*

### Comparing `avrotize-1.9.1/avrotize/asn1toavro.py` & `avrotize-2.0.0/avrotize/asn1toavro.py`

 * *Files identical despite different names*

### Comparing `avrotize-1.9.1/avrotize/avrotize.py` & `avrotize-2.0.0/avrotize/avrotize.py`

 * *Files 2% similar despite different names*

```diff
@@ -35,15 +35,16 @@
                 kwargs['default'] = arg['default']
             if arg['type'] == 'bool':
                 kwargs['action'] = 'store_true'
                 del kwargs['type']
                 carg = cmd_parser.add_argument(arg['name'], **kwargs)
             else:
                 carg = cmd_parser.add_argument(arg['name'], **kwargs)
-            carg.required = arg.get('required', True)
+            if arg.get('required', False):
+                carg.required = True
 
 def dynamic_import(module, func):
     """Dynamically import a module and function."""
     mod = __import__(module, fromlist=[func])
     return getattr(mod, func)
 
 def main():
```

### Comparing `avrotize-1.9.1/avrotize/avrotocpp.py` & `avrotize-2.0.0/avrotize/avrotocpp.py`

 * *Files 1% similar despite different names*

```diff
@@ -462,18 +462,14 @@
         with open(avro_schema_path, 'r', encoding='utf-8') as file:
             schema = json.load(file)
         self.convert_schema(schema, output_dir)
 
 
 def convert_avro_to_cpp(avro_schema_path, output_dir, namespace='', avro_annotation=False, json_annotation=False):
     """Converts Avro schema to C++ classes"""
-    
-    if not namespace:
-        namespace = os.path.splitext(os.path.basename(avro_schema_path))[0].replace('-', '_')
-    
     avroToCpp = AvroToCpp(namespace)
     avroToCpp.avro_annotation = avro_annotation
     avroToCpp.json_annotation = json_annotation
     avroToCpp.convert(avro_schema_path, output_dir)
 
 def convert_avro_schema_to_cpp(avro_schema: Dict, output_dir: str, namespace: str = '', avro_annotation: bool = False, json_annotation: bool = False):
     """Converts Avro schema to C++ classes"""
```

### Comparing `avrotize-1.9.1/avrotize/avrotocpp/CMakeLists.txt.jinja` & `avrotize-2.0.0/avrotize/avrotocpp/CMakeLists.txt.jinja`

 * *Files identical despite different names*

### Comparing `avrotize-1.9.1/avrotize/avrotocpp/dataclass_body.jinja` & `avrotize-2.0.0/avrotize/avrotocpp/dataclass_body.jinja`

 * *Files identical despite different names*

### Comparing `avrotize-1.9.1/avrotize/avrotocsharp.py` & `avrotize-2.0.0/avrotize/avrotocsharp.py`

 * *Files identical despite different names*

### Comparing `avrotize-1.9.1/avrotize/avrotocsharp/class_test.cs.jinja` & `avrotize-2.0.0/avrotize/avrotocsharp/class_test.cs.jinja`

 * *Files identical despite different names*

### Comparing `avrotize-1.9.1/avrotize/avrotocsharp/dataclass_core.jinja` & `avrotize-2.0.0/avrotize/avrotocsharp/dataclass_core.jinja`

 * *Files identical despite different names*

### Comparing `avrotize-1.9.1/avrotize/avrotocsharp/enum_test.cs.jinja` & `avrotize-2.0.0/avrotize/avrotocsharp/enum_test.cs.jinja`

 * *Files identical despite different names*

### Comparing `avrotize-1.9.1/avrotize/avrotocsharp/project.csproj.jinja` & `avrotize-2.0.0/avrotize/avrotocsharp/project.csproj.jinja`

 * *Files identical despite different names*

### Comparing `avrotize-1.9.1/avrotize/avrotocsharp/project.sln.jinja` & `avrotize-2.0.0/avrotize/avrotocsharp/project.sln.jinja`

 * *Files identical despite different names*

### Comparing `avrotize-1.9.1/avrotize/avrotocsharp/testproject.csproj.jinja` & `avrotize-2.0.0/avrotize/avrotocsharp/testproject.csproj.jinja`

 * *Files identical despite different names*

### Comparing `avrotize-1.9.1/avrotize/avrotocsv.py` & `avrotize-2.0.0/avrotize/avrotocsv.py`

 * *Files 5% similar despite different names*

```diff
@@ -109,13 +109,9 @@
 def convert_avro_to_csv_schema(avro_schema_path, csv_schema_path):
     """
     Convert an Avro schema file to a CSV schema file.
 
     :param avro_schema_path: Path to the Avro schema file.
     :param csv_schema_path: Path to save the CSV schema file.
     """
-    
-    if not os.path.exists(avro_schema_path):
-        raise FileNotFoundError(f"Avro schema file not found: {avro_schema_path}")
-    
     converter = AvroToCSVSchemaConverter(avro_schema_path, csv_schema_path)
     converter.convert()
```

### Comparing `avrotize-1.9.1/avrotize/avrotodatapackage.py` & `avrotize-2.0.0/avrotize/avrotodatapackage.py`

 * *Files identical despite different names*

### Comparing `avrotize-1.9.1/avrotize/avrotodb.py` & `avrotize-2.0.0/avrotize/avrotodb.py`

 * *Files identical despite different names*

### Comparing `avrotize-1.9.1/avrotize/avrotogo.py` & `avrotize-2.0.0/avrotize/avrotogo.py`

 * *Files identical despite different names*

### Comparing `avrotize-1.9.1/avrotize/avrotogo/go_struct.jinja` & `avrotize-2.0.0/avrotize/avrotogo/go_struct.jinja`

 * *Files identical despite different names*

### Comparing `avrotize-1.9.1/avrotize/avrotogo/go_test.jinja` & `avrotize-2.0.0/avrotize/avrotogo/go_test.jinja`

 * *Files identical despite different names*

### Comparing `avrotize-1.9.1/avrotize/avrotogo/go_union.jinja` & `avrotize-2.0.0/avrotize/avrotogo/go_union.jinja`

 * *Files identical despite different names*

### Comparing `avrotize-1.9.1/avrotize/avrotographql.py` & `avrotize-2.0.0/avrotize/avrotographql.py`

 * *Files identical despite different names*

### Comparing `avrotize-1.9.1/avrotize/avrotoiceberg.py` & `avrotize-2.0.0/avrotize/avrotoiceberg.py`

 * *Files identical despite different names*

### Comparing `avrotize-1.9.1/avrotize/avrotojava.py` & `avrotize-2.0.0/avrotize/avrotojava.py`

 * *Files identical despite different names*

### Comparing `avrotize-1.9.1/avrotize/avrotojs.py` & `avrotize-2.0.0/avrotize/avrotojs.py`

 * *Files 2% similar despite different names*

```diff
@@ -233,18 +233,14 @@
         """ Convert Avro schema to TypeScript classes """
         with open(avro_schema_path, 'r', encoding='utf-8') as file:
             schema = json.load(file)
         self.convert_schema(schema, output_dir)
 
 def convert_avro_to_javascript(avro_schema_path, js_dir_path, package_name='', avro_annotation=False):
     """ Convert Avro schema to TypeScript classes """
-    
-    if not package_name:
-        package_name = os.path.splitext(os.path.basename(avro_schema_path))[0].replace('-', '_')
-    
     converter = AvroToJavaScript(package_name, avro_annotation=avro_annotation)
     converter.convert(avro_schema_path, js_dir_path)
     
 def convert_avro_schema_to_javascript(avro_schema, js_dir_path, package_name='', avro_annotation=False):
     """ Convert Avro schema to TypeScript classes """
     converter = AvroToJavaScript(package_name, avro_annotation=avro_annotation)
     converter.convert_schema(avro_schema, js_dir_path)
```

### Comparing `avrotize-1.9.1/avrotize/avrotojsons.py` & `avrotize-2.0.0/avrotize/avrotojsons.py`

 * *Files identical despite different names*

### Comparing `avrotize-1.9.1/avrotize/avrotokusto.py` & `avrotize-2.0.0/avrotize/avrotokusto.py`

 * *Files identical despite different names*

### Comparing `avrotize-1.9.1/avrotize/avrotomd.py` & `avrotize-2.0.0/avrotize/avrotomd.py`

 * *Files identical despite different names*

### Comparing `avrotize-1.9.1/avrotize/avrotomd/README.md.jinja` & `avrotize-2.0.0/avrotize/avrotomd/README.md.jinja`

 * *Files identical despite different names*

### Comparing `avrotize-1.9.1/avrotize/avrotools.py` & `avrotize-2.0.0/avrotize/avrotools.py`

 * *Files identical despite different names*

### Comparing `avrotize-1.9.1/avrotize/avrotoparquet.py` & `avrotize-2.0.0/avrotize/avrotoparquet.py`

 * *Files identical despite different names*

### Comparing `avrotize-1.9.1/avrotize/avrotoproto.py` & `avrotize-2.0.0/avrotize/avrotoproto.py`

 * *Files 0% similar despite different names*

```diff
@@ -349,9 +349,9 @@
         self.avro_schema_to_proto_messages(avro_schema, proto_files)
         self.save_proto_to_file(proto_files, proto_file_path)
 
 def convert_avro_to_proto(avro_schema_path, proto_file_path, naming_mode: Literal['snake', 'pascal', 'camel'] = 'pascal', allow_optional: bool = False):
     avrotoproto = AvroToProto()
     avrotoproto.naming_mode = naming_mode
     avrotoproto.allow_optional = allow_optional
-    avrotoproto.default_namespace = os.path.splitext(os.path.basename(proto_file_path))[0].replace('-','_')
+    avrotoproto.default_namespace = os.path.splitext(os.path.basename(proto_file_path))[0]
     avrotoproto.convert_avro_to_proto(avro_schema_path, proto_file_path)
```

### Comparing `avrotize-1.9.1/avrotize/avrotopython.py` & `avrotize-2.0.0/avrotize/avrotopython.py`

 * *Files 0% similar despite different names*

```diff
@@ -325,17 +325,14 @@
             schema = json.load(file)
         if isinstance(schema, dict):
             schema = [schema]
         return self.convert_schemas(schema, output_dir)
 
 def convert_avro_to_python(avro_schema_path, py_file_path, package_name = '', dataclasses_json_annotation = False, avro_annotation = False):
     """Converts Avro schema to Python data classes"""
-    if not package_name:
-        package_name = os.path.splitext(os.path.basename(avro_schema_path))[0].lower().replace('-', '_')
-        
     avro_to_python = AvroToPython(package_name, dataclasses_json_annotation=dataclasses_json_annotation, avro_annotation=avro_annotation)
     avro_to_python.convert(avro_schema_path, py_file_path)
 
 def convert_avro_schema_to_python(avro_schema, py_file_path, package_name = '', dataclasses_json_annotation = False, avro_annotation = False):
     """Converts Avro schema to Python data classes"""
     avro_to_python = AvroToPython(package_name, dataclasses_json_annotation=dataclasses_json_annotation, avro_annotation=avro_annotation)
     if isinstance(avro_schema, dict):
```

### Comparing `avrotize-1.9.1/avrotize/avrotorust.py` & `avrotize-2.0.0/avrotize/avrotorust.py`

 * *Files 1% similar despite different names*

```diff
@@ -403,18 +403,14 @@
     Args:
         avro_schema_path (str): Avro input schema path  
         rust_file_path (str): Output Rust file path 
         package_name (str): Base package name
         avro_annotation (bool): Include Avro annotations
         serde_annotation (bool): Include Serde annotations
     """
-    
-    if not package_name:
-        package_name = os.path.splitext(os.path.basename(avro_schema_path))[0].lower().replace('-', '_')
-        
     avrotorust = AvroToRust()
     avrotorust.base_package = package_name
     avrotorust.avro_annotation = avro_annotation
     avrotorust.serde_annotation = serde_annotation
     avrotorust.convert(avro_schema_path, rust_file_path)
```

### Comparing `avrotize-1.9.1/avrotize/avrotorust/dataclass_enum.rs.jinja` & `avrotize-2.0.0/avrotize/avrotorust/dataclass_enum.rs.jinja`

 * *Files identical despite different names*

### Comparing `avrotize-1.9.1/avrotize/avrotorust/dataclass_struct.rs.jinja` & `avrotize-2.0.0/avrotize/avrotorust/dataclass_struct.rs.jinja`

 * *Files identical despite different names*

### Comparing `avrotize-1.9.1/avrotize/avrotorust/dataclass_union.rs.jinja` & `avrotize-2.0.0/avrotize/avrotorust/dataclass_union.rs.jinja`

 * *Files identical despite different names*

### Comparing `avrotize-1.9.1/avrotize/avrotots.py` & `avrotize-2.0.0/avrotize/avrotots.py`

 * *Files 1% similar despite different names*

```diff
@@ -544,18 +544,14 @@
             schema = json.load(file)
         self.convert_schema(schema, output_dir)
         self.generate_project_files(output_dir)
 
 
 def convert_avro_to_typescript(avro_schema_path, js_dir_path, package_name='', typedjson_annotation=False, avro_annotation=False):
     """ Convert Avro schema to TypeScript classes """
-    
-    if not package_name:
-        package_name = os.path.splitext(os.path.basename(avro_schema_path))[0].lower().replace('-', '_')
-        
     converter = AvroToTypeScript(package_name, typed_json_annotation=typedjson_annotation, avro_annotation=avro_annotation)
     converter.convert(avro_schema_path, js_dir_path)
 
 
 def convert_avro_schema_to_typescript(avro_schema, js_dir_path, package_name='', typedjson_annotation=False, avro_annotation=False):
     """ Convert Avro schema to TypeScript classes """
     converter = AvroToTypeScript(package_name, typed_json_annotation=typedjson_annotation, avro_annotation=avro_annotation)
```

### Comparing `avrotize-1.9.1/avrotize/avrotoxsd.py` & `avrotize-2.0.0/avrotize/avrotoxsd.py`

 * *Files identical despite different names*

### Comparing `avrotize-1.9.1/avrotize/commands.json` & `avrotize-2.0.0/avrotize/commands.json`

 * *Files 6% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9513062169312171%*

 * *Differences: {'0': "{'args': {0: {delete: ['required']}, 2: {delete: ['required']}}}",*

 * * '1': "{'args': {0: {delete: ['required']}, 1: {'required': True}, 2: {delete: ['required']}, 4: "*

 * *      "{delete: ['required']}}, 'prompts': {0: {delete: ['required']}, 1: {delete: ['required']}}}",*

 * * '10': "{'args': {0: {delete: ['required']}, 2: {delete: ['required']}, 4: {delete: "*

 * *       "['required']}}}",*

 * * '11': "{'args': {0: {delete: ['required']}, 3: {delete: ['required']}}}",*

 * * '12': "{'args': {0: {delete: ['required']}, 2: {de […]*

```diff
@@ -1,27 +1,25 @@
 [
     {
         "args": [
             {
                 "help": "Path of the proto file (or read from stdin if omitted)",
                 "name": "input",
                 "nargs": "?",
-                "required": false,
                 "type": "str"
             },
             {
                 "help": "Path to the Avrotize schema file",
                 "name": "--out",
                 "required": false,
                 "type": "str"
             },
             {
                 "help": "Deprecated: Path of the proto file (for backcompat)",
                 "name": "--proto",
-                "required": false,
                 "type": "str"
             }
         ],
         "command": "p2a",
         "description": "Convert Proto schema to Avrotize schema",
         "extensions": [
             ".proto"
@@ -38,27 +36,25 @@
     },
     {
         "args": [
             {
                 "help": "Path to the Proto file (or read from stdin if omitted)",
                 "name": "input",
                 "nargs": "?",
-                "required": false,
                 "type": "str"
             },
             {
                 "help": "Path to the Avrotize schema file",
                 "name": "--out",
-                "required": false,
+                "required": true,
                 "type": "str"
             },
             {
                 "help": "Deprecated: Path to the Proto file (for backcompat)",
                 "name": "--avsc",
-                "required": false,
                 "type": "str"
             },
             {
                 "choices": [
                     "snake",
                     "camel",
                     "pascal"
@@ -69,15 +65,14 @@
                 "required": false,
                 "type": "str"
             },
             {
                 "default": false,
                 "help": "Enable support for 'optional' fields",
                 "name": "--allow-optional",
-                "required": false,
                 "type": "bool"
             }
         ],
         "command": "a2p",
         "description": "Convert Avrotize schema to Proto schema",
         "extensions": [
             ".avsc"
@@ -96,59 +91,54 @@
                 "choices": [
                     "snake",
                     "camel",
                     "pascal"
                 ],
                 "default": "pascal",
                 "message": "Select type naming convention",
-                "name": "--naming",
-                "required": false
+                "name": "--naming"
             },
             {
                 "default": false,
                 "message": "Enable support for 'optional' fields?",
                 "name": "--allow-optional",
-                "required": false,
                 "type": "bool"
             }
         ],
         "suggested_output_file_path": "{input_file_name}-proto"
     },
     {
         "args": [
             {
                 "help": "Path to the JSON schema file (or read from stdin if omitted)",
                 "name": "input",
                 "nargs": "?",
-                "required": false,
                 "type": "str"
             },
             {
                 "help": "Path to the Avrotize schema file",
                 "name": "--out",
                 "required": false,
                 "type": "str"
             },
             {
                 "help": "Deprecated: Path to the JSON schema file (for backcompat)",
                 "name": "--jsons",
-                "required": false,
                 "type": "str"
             },
             {
                 "help": "Namespace for the Avrotize schema",
                 "name": "--namespace",
                 "required": false,
                 "type": "str"
             },
             {
                 "default": false,
                 "help": "Split top-level records into separate files",
                 "name": "--split-top-level-records",
-                "required": false,
                 "type": "bool"
             }
         ],
         "command": "j2a",
         "description": "Convert JSON schema to Avrotize schema",
         "extensions": [
             ".json",
@@ -170,39 +160,36 @@
                 "required": false,
                 "type": "str"
             },
             {
                 "default": false,
                 "message": "Split top-level records into separate files?",
                 "name": "--split-top-level-records",
-                "required": false,
                 "type": "bool"
             }
         ],
         "suggested_output_file_path": "{input_file_name}.avsc"
     },
     {
         "args": [
             {
                 "help": "Path to the Avrotize schema file (or read from stdin if omitted)",
                 "name": "input",
                 "nargs": "?",
-                "required": false,
                 "type": "str"
             },
             {
                 "help": "Path to the JSON schema file",
                 "name": "--out",
                 "required": false,
                 "type": "str"
             },
             {
                 "help": "Deprecated: Path to the Avrotize schema file (for backcompat)",
                 "name": "--avsc",
-                "required": false,
                 "type": "str"
             },
             {
                 "choices": [
                     "snake",
                     "camel",
                     "pascal",
@@ -233,27 +220,25 @@
     },
     {
         "args": [
             {
                 "help": "Path to the XSD schema file (or read from stdin if omitted)",
                 "name": "input",
                 "nargs": "?",
-                "required": false,
                 "type": "str"
             },
             {
                 "help": "Path to the Avrotize schema file",
                 "name": "--out",
                 "required": false,
                 "type": "str"
             },
             {
                 "help": "Deprecated: Path to the XSD schema file (for backcompat)",
                 "name": "--xsd",
-                "required": false,
                 "type": "str"
             },
             {
                 "help": "Namespace for the Avrotize schema",
                 "name": "--namespace",
                 "required": false,
                 "type": "str"
@@ -284,27 +269,25 @@
     },
     {
         "args": [
             {
                 "help": "Path to the Avrotize schema file (or read from stdin if omitted)",
                 "name": "input",
                 "nargs": "?",
-                "required": false,
                 "type": "str"
             },
             {
                 "help": "Path to the XSD schema file",
                 "name": "--out",
                 "required": false,
                 "type": "str"
             },
             {
                 "help": "Deprecated: Path to the Avrotize schema file (for backcompat)",
                 "name": "--avsc",
-                "required": false,
                 "type": "str"
             }
         ],
         "command": "a2x",
         "description": "Convert Avrotize schema to XSD schema",
         "extensions": [
             ".avsc"
@@ -321,27 +304,25 @@
     },
     {
         "args": [
             {
                 "help": "Path to the Avrotize schema file (or read from stdin if omitted)",
                 "name": "input",
                 "nargs": "?",
-                "required": false,
                 "type": "str"
             },
             {
                 "help": "Path to the Kusto table",
                 "name": "--out",
                 "required": false,
                 "type": "str"
             },
             {
                 "help": "Deprecated: Path to the Avrotize schema file (for backcompat)",
                 "name": "--avsc",
-                "required": false,
                 "type": "str"
             },
             {
                 "help": "Kusto Cluster URI to apply the generated schema to.",
                 "name": "--kusto-uri",
                 "required": false,
                 "type": "str"
@@ -358,15 +339,14 @@
                 "required": false,
                 "type": "str"
             },
             {
                 "default": false,
                 "help": "Add CloudEvents columns to the Kusto table",
                 "name": "--emit-cloudevents-columns",
-                "required": false,
                 "type": "bool"
             },
             {
                 "help": "Emit a _cloudevents_dispatch ingestion table and update policies for each generated table",
                 "name": "--emit-cloudevents-dispatch",
                 "required": false,
                 "type": "bool"
@@ -402,34 +382,31 @@
                 "required": false,
                 "type": "str"
             },
             {
                 "default": false,
                 "message": "Add CloudEvents columns to the Kusto table?",
                 "name": "--emit-cloudevents-columns",
-                "required": false,
                 "type": "bool"
             },
             {
                 "default": false,
                 "message": "Emit a _cloudevents_dispatch ingestion table and update policies?",
                 "name": "--emit-cloudevents-dispatch",
-                "required": false,
                 "type": "bool"
             }
         ],
         "suggested_output_file_path": "{input_file_name}.kql"
     },
     {
         "args": [
             {
-                "help": "Kusto file",
+                "help": "Kusto URI (or read from stdin if omitted)",
                 "name": "input",
                 "nargs": "?",
-                "required": false,
                 "type": "str"
             },
             {
                 "help": "Path to the Avrotize schema file",
                 "name": "--out",
                 "required": false,
                 "type": "str"
@@ -488,47 +465,43 @@
                 "required": false,
                 "type": "str"
             },
             {
                 "default": false,
                 "message": "Emit CloudEvents declarations for each table?",
                 "name": "--emit-cloudevents",
-                "required": false,
                 "type": "bool"
             },
             {
                 "default": false,
                 "message": "Emit an xRegistry manifest with CloudEvents declarations?",
                 "name": "--emit-xregistry",
-                "required": false,
                 "type": "bool"
             }
         ],
         "skip_input_file_handling": true,
         "suggested_output_file_path": "{kusto_database}.avsc"
     },
     {
         "args": [
             {
                 "help": "Path to the Avrotize schema file (or read from stdin if omitted)",
                 "name": "input",
                 "nargs": "?",
-                "required": false,
                 "type": "str"
             },
             {
                 "help": "Path to the SQL table",
                 "name": "--out",
                 "required": false,
                 "type": "str"
             },
             {
                 "help": "Deprecated: Path to the Avrotize schema file (for backcompat)",
                 "name": "--avsc",
-                "required": false,
                 "type": "str"
             },
             {
                 "choices": [
                     "mysql",
                     "mariadb",
                     "postgres",
@@ -545,15 +518,14 @@
                 "required": true,
                 "type": "str"
             },
             {
                 "default": false,
                 "help": "Add CloudEvents columns to the SQL table",
                 "name": "--emit-cloudevents-columns",
-                "required": false,
                 "type": "bool"
             }
         ],
         "command": "a2sql",
         "description": "Convert Avrotize schema to SQL schema",
         "extensions": [
             ".avsc"
@@ -579,47 +551,43 @@
                     "bigquery",
                     "snowflake",
                     "redshift",
                     "db2"
                 ],
                 "default": "mysql",
                 "message": "Select the SQL dialect",
-                "name": "--dialect",
-                "required": true
+                "name": "--dialect"
             },
             {
                 "default": false,
                 "message": "Add CloudEvents columns to the SQL table?",
                 "name": "--emit-cloudevents-columns",
-                "required": false,
                 "type": "bool"
             }
         ],
         "suggested_output_file_path": "{input_file_name}.sql"
     },
     {
         "args": [
             {
                 "help": "Path to the Avrotize schema file (or read from stdin if omitted)",
                 "name": "input",
                 "nargs": "?",
-                "required": false,
                 "type": "str"
             },
             {
-                "help": "Path to the MongoDB schemas",
+                "help": "Path to the MongoDB schema",
                 "name": "--out",
-                "required": true,
+                "required": false,
                 "type": "str"
             },
             {
                 "default": false,
                 "help": "Add CloudEvents columns to the MongoDB schema",
                 "name": "--emit-cloudevents-columns",
-                "required": false,
                 "type": "bool"
             }
         ],
         "command": "a2mongo",
         "description": "Convert Avrotize schema to MongoDB schema",
         "extensions": [
             ".avsc"
@@ -645,40 +613,37 @@
     },
     {
         "args": [
             {
                 "help": "Path to the Avrotize schema file (or read from stdin if omitted)",
                 "name": "input",
                 "nargs": "?",
-                "required": false,
                 "type": "str"
             },
             {
                 "help": "Path to the Parquet file",
                 "name": "--out",
                 "required": false,
                 "type": "str"
             },
             {
                 "help": "Deprecated: Path to the Avrotize schema file (for backcompat)",
                 "name": "--avsc",
-                "required": false,
                 "type": "str"
             },
             {
                 "help": "Record type in the Avrotize schema",
                 "name": "--record-type",
                 "required": false,
                 "type": "str"
             },
             {
                 "default": false,
                 "help": "Add CloudEvents columns to the Parquet file",
                 "name": "--emit-cloudevents-columns",
-                "required": false,
                 "type": "bool"
             }
         ],
         "command": "a2pq",
         "description": "Convert Avrotize schema to Parquet or Iceberg schema",
         "extensions": [
             ".avsc"
@@ -704,15 +669,14 @@
     },
     {
         "args": [
             {
                 "help": "Path to the Avrotize schema file (or read from stdin if omitted)",
                 "name": "input",
                 "nargs": "?",
-                "required": false,
                 "type": "str"
             },
             {
                 "help": "Path to the Iceberg schema",
                 "name": "--out",
                 "required": false,
                 "type": "str"
@@ -723,15 +687,14 @@
                 "required": false,
                 "type": "str"
             },
             {
                 "default": false,
                 "help": "Add CloudEvents columns to the Iceberg schema",
                 "name": "--emit-cloudevents-columns",
-                "required": false,
                 "type": "bool"
             }
         ],
         "command": "a2ib",
         "description": "Convert Avrotize schema to Iceberg schema",
         "extensions": [
             ".avsc"
@@ -757,27 +720,25 @@
     },
     {
         "args": [
             {
                 "help": "Path to the Parquet file (or read from stdin if omitted)",
                 "name": "input",
                 "nargs": "?",
-                "required": false,
                 "type": "str"
             },
             {
                 "help": "Path to the Avrotize schema file",
                 "name": "--out",
                 "required": false,
                 "type": "str"
             },
             {
                 "help": "Deprecated: Path to the Parquet file (for backcompat)",
                 "name": "--parquet",
-                "required": false,
                 "type": "str"
             },
             {
                 "help": "Namespace for the Avrotize schema",
                 "name": "--namespace",
                 "required": false,
                 "type": "str"
@@ -808,28 +769,26 @@
     },
     {
         "args": [
             {
                 "help": "Path(s) to the ASN.1 schema file(s) (or read from stdin if omitted)",
                 "name": "input",
                 "nargs": "?",
-                "required": false,
                 "type": "str"
             },
             {
                 "help": "Path to the Avrotize schema file",
                 "name": "--out",
                 "required": false,
                 "type": "str"
             },
             {
                 "help": "Deprecated: Path(s) to the ASN.1 schema file(s) (for backcompat)",
                 "name": "--asn",
                 "nargs": "+",
-                "required": false,
                 "type": "str"
             }
         ],
         "command": "asn2a",
         "description": "Convert ASN.1 schema to Avrotize schema",
         "extensions": [
             ".asn1"
@@ -846,27 +805,25 @@
     },
     {
         "args": [
             {
                 "help": "Path to the Kafka Struct file (or read from stdin if omitted)",
                 "name": "input",
                 "nargs": "?",
-                "required": false,
                 "type": "str"
             },
             {
                 "help": "Path to the Avrotize schema file",
                 "name": "--out",
                 "required": false,
                 "type": "str"
             },
             {
                 "help": "Deprecated: Path to the Kafka Struct file (for backcompat)",
                 "name": "--kstruct",
-                "required": false,
                 "type": "str"
             }
         ],
         "command": "kstruct2a",
         "description": "Convert Kafka Struct to Avrotize schema",
         "extensions": [
             ".kstruct"
@@ -883,61 +840,55 @@
     },
     {
         "args": [
             {
                 "help": "Path to the Kafka Struct file (or read from stdin if omitted)",
                 "name": "input",
                 "nargs": "?",
-                "required": false,
                 "type": "str"
             },
             {
                 "help": "Path to the Avrotize schema file",
                 "name": "--out",
                 "required": false,
                 "type": "str"
             },
             {
                 "help": "Deprecated: Path to the Avrotize schema file (for backcompat)",
                 "name": "--avsc",
-                "required": false,
                 "type": "str"
             },
             {
                 "help": "C# project name",
                 "name": "--namespace",
                 "required": false,
                 "type": "str"
             },
             {
                 "default": false,
                 "help": "Use Avro annotations",
                 "name": "--avro-annotation",
-                "required": false,
                 "type": "bool"
             },
             {
                 "default": false,
                 "help": "Use System.Text.Json annotations",
                 "name": "--system_text_json_annotation",
-                "required": false,
                 "type": "bool"
             },
             {
                 "default": false,
                 "help": "Use Newtonsoft.Json annotations",
                 "name": "--newtonsoft-json-annotation",
-                "required": false,
                 "type": "bool"
             },
             {
                 "default": false,
                 "help": "Use PascalCase properties",
                 "name": "--pascal-properties",
-                "required": false,
                 "type": "bool"
             }
         ],
         "command": "a2cs",
         "description": "Convert Avrotize schema to C# classes",
         "extensions": [
             ".avsc"
@@ -962,80 +913,72 @@
                 "required": false,
                 "type": "str"
             },
             {
                 "default": false,
                 "message": "Use Avro annotations?",
                 "name": "--avro-annotation",
-                "required": false,
                 "type": "bool"
             },
             {
                 "default": false,
                 "message": "Use System.Text.Json annotations?",
                 "name": "--system_text_json_annotation",
-                "required": false,
                 "type": "bool"
             },
             {
                 "default": false,
                 "message": "Use PascalCase properties?",
                 "name": "--pascal-properties",
-                "required": false,
                 "type": "bool"
             }
         ],
         "suggested_output_file_path": "{input_file_name}-cs"
     },
     {
         "args": [
             {
                 "help": "Path to the Avrotize schema file (or read from stdin if omitted)",
                 "name": "input",
                 "nargs": "?",
-                "required": false,
                 "type": "str"
             },
             {
                 "help": "Output path for the Java classes",
                 "name": "--out",
                 "required": true,
                 "type": "str"
             },
             {
                 "help": "Deprecated: Path to the Avrotize schema file (for backcompat)",
                 "name": "--avsc",
-                "required": false,
                 "type": "str"
             },
             {
                 "help": "Java package name",
                 "name": "--package",
                 "required": false,
                 "type": "str"
             },
             {
                 "default": false,
                 "help": "Use Avro annotations",
                 "name": "--avro-annotation",
-                "required": false,
                 "type": "bool"
             },
             {
                 "default": false,
                 "help": "Use Jackson annotations",
                 "name": "--jackson-annotation",
-                "required": false,
                 "type": "bool"
             },
             {
                 "default": false,
                 "help": "Use PascalCase properties",
                 "name": "--pascal-properties",
-                "required": false,
                 "type": "bool"
             }
         ],
         "command": "a2java",
         "description": "Convert Avrotize schema to Java classes",
         "extensions": [
             ".avsc"
@@ -1075,47 +1018,43 @@
     },
     {
         "args": [
             {
                 "help": "Path to the Avrotize schema file (or read from stdin if omitted)",
                 "name": "input",
                 "nargs": "?",
-                "required": false,
                 "type": "str"
             },
             {
                 "help": "Output path for the Python classes",
                 "name": "--out",
                 "required": true,
                 "type": "str"
             },
             {
                 "help": "Deprecated: Path to the Avrotize schema file (for backcompat)",
                 "name": "--avsc",
-                "required": false,
                 "type": "str"
             },
             {
                 "help": "Python package name",
                 "name": "--package",
                 "required": false,
                 "type": "str"
             },
             {
                 "default": false,
                 "help": "Use dataclasses-json annotations",
                 "name": "--dataclasses-json-annotation",
-                "required": false,
                 "type": "bool"
             },
             {
                 "default": false,
                 "help": "Use Avro annotations",
                 "name": "--avro-annotation",
-                "required": false,
                 "type": "bool"
             }
         ],
         "command": "a2py",
         "description": "Convert Avrotize schema to Python classes",
         "extensions": [
             ".avsc"
@@ -1148,47 +1087,43 @@
     },
     {
         "args": [
             {
                 "help": "Path to the Avrotize schema file (or read from stdin if omitted)",
                 "name": "input",
                 "nargs": "?",
-                "required": false,
                 "type": "str"
             },
             {
                 "help": "Output path for the TypeScript classes",
                 "name": "--out",
                 "required": true,
                 "type": "str"
             },
             {
                 "help": "Deprecated: Path to the Avrotize schema file (for backcompat)",
                 "name": "--avsc",
-                "required": false,
                 "type": "str"
             },
             {
                 "help": "TypeScript package name",
                 "name": "--package",
                 "required": false,
                 "type": "str"
             },
             {
                 "default": false,
                 "help": "Use Avro annotations",
                 "name": "--avro-annotation",
-                "required": false,
                 "type": "bool"
             },
             {
                 "default": false,
                 "help": "Use TypedJSON annotations",
                 "name": "--typedjson-annotation",
-                "required": false,
                 "type": "bool"
             }
         ],
         "command": "a2ts",
         "description": "Convert Avrotize schema to TypeScript classes",
         "extensions": [
             ".avsc"
@@ -1221,40 +1156,37 @@
     },
     {
         "args": [
             {
                 "help": "Path to the Avrotize schema file (or read from stdin if omitted)",
                 "name": "input",
                 "nargs": "?",
-                "required": false,
                 "type": "str"
             },
             {
                 "help": "Output path for the JavaScript classes",
                 "name": "--out",
                 "required": true,
                 "type": "str"
             },
             {
                 "help": "Deprecated: Path to the Avrotize schema file (for backcompat)",
                 "name": "--avsc",
-                "required": false,
                 "type": "str"
             },
             {
                 "help": "JavaScript package name",
                 "name": "--package",
                 "required": false,
                 "type": "str"
             },
             {
                 "default": false,
                 "help": "Use Avro annotations",
                 "name": "--avro-annotation",
-                "required": false,
                 "type": "bool"
             }
         ],
         "command": "a2js",
         "description": "Convert Avrotize schema to JavaScript classes",
         "extensions": [
             ".avsc"
@@ -1280,47 +1212,43 @@
     },
     {
         "args": [
             {
                 "help": "Path to the Avrotize schema file (or read from stdin if omitted)",
                 "name": "input",
                 "nargs": "?",
-                "required": false,
                 "type": "str"
             },
             {
                 "help": "Output path for the C++ classes",
                 "name": "--out",
                 "required": true,
                 "type": "str"
             },
             {
                 "help": "Deprecated: Path to the Avrotize schema file (for backcompat)",
                 "name": "--avsc",
-                "required": false,
                 "type": "str"
             },
             {
                 "help": "C++ namespace",
                 "name": "--namespace",
                 "required": false,
                 "type": "str"
             },
             {
                 "default": false,
                 "help": "Use Avro annotations",
                 "name": "--avro-annotation",
-                "required": false,
                 "type": "bool"
             },
             {
                 "default": false,
                 "help": "Use JSON annotations",
                 "name": "--json-annotation",
-                "required": false,
                 "type": "bool"
             }
         ],
         "command": "a2cpp",
         "description": "Convert Avrotize schema to C++ classes",
         "extensions": [
             ".avsc"
@@ -1333,15 +1261,14 @@
                 "namespace": "args.namespace",
                 "output_dir": "output_file_path"
             },
             "name": "avrotize.avrotocpp.convert_avro_to_cpp"
         },
         "prompts": [
             {
-                "default": "{input_file_name}",
                 "message": "Enter the root namespace for the C++ classes (optional)",
                 "name": "--namespace",
                 "required": false,
                 "type": "str"
             },
             {
                 "default": false,
@@ -1360,27 +1287,25 @@
     },
     {
         "args": [
             {
                 "help": "Path to the Avrotize schema file (or read from stdin if omitted)",
                 "name": "input",
                 "nargs": "?",
-                "required": false,
                 "type": "str"
             },
             {
                 "help": "Output path for the Go classes",
                 "name": "--out",
                 "required": true,
                 "type": "str"
             },
             {
                 "help": "Deprecated: Path to the Avrotize schema file (for backcompat)",
                 "name": "--avsc",
-                "required": false,
                 "type": "str"
             },
             {
                 "help": "Go package name",
                 "name": "--package",
                 "required": false,
                 "type": "str"
@@ -1397,22 +1322,20 @@
                 "required": false,
                 "type": "str"
             },
             {
                 "default": false,
                 "help": "Use Avro annotations",
                 "name": "--avro-annotation",
-                "required": false,
                 "type": "bool"
             },
             {
                 "default": false,
                 "help": "Use JSON annotations",
                 "name": "--json-annotation",
-                "required": false,
                 "type": "bool"
             }
         ],
         "command": "a2go",
         "description": "Convert Avrotize schema to Go classes",
         "extensions": [
             ".avsc"
@@ -1465,47 +1388,43 @@
     },
     {
         "args": [
             {
                 "help": "Path to the Avrotize schema file (or read from stdin if omitted)",
                 "name": "input",
                 "nargs": "?",
-                "required": false,
                 "type": "str"
             },
             {
                 "help": "Output path for the Rust classes",
                 "name": "--out",
                 "required": true,
                 "type": "str"
             },
             {
                 "help": "Deprecated: Path to the Avrotize schema file (for backcompat)",
                 "name": "--avsc",
-                "required": false,
                 "type": "str"
             },
             {
                 "help": "Rust package name",
                 "name": "--package",
                 "required": false,
                 "type": "str"
             },
             {
                 "default": false,
                 "help": "Use Avro annotations",
                 "name": "--avro-annotation",
-                "required": false,
                 "type": "bool"
             },
             {
                 "default": false,
                 "help": "Use JSON annotations",
                 "name": "--json-annotation",
-                "required": false,
                 "type": "bool"
             }
         ],
         "command": "a2rust",
         "description": "Convert Avrotize schema to Rust classes",
         "extensions": [
             ".avsc"
@@ -1544,15 +1463,14 @@
     },
     {
         "args": [
             {
                 "help": "Path to the Avrotize schema file (or read from stdin if omitted)",
                 "name": "input",
                 "nargs": "?",
-                "required": false,
                 "type": "str"
             },
             {
                 "help": "Output path for the Datapackage schema",
                 "name": "--out",
                 "required": true,
                 "type": "str"
@@ -1589,21 +1507,20 @@
     },
     {
         "args": [
             {
                 "help": "Path to the Avrotize schema file (or read from stdin if omitted)",
                 "name": "input",
                 "nargs": "?",
-                "required": false,
                 "type": "str"
             },
             {
                 "help": "Output path for the Markdown documentation",
                 "name": "--out",
-                "required": false,
+                "required": true,
                 "type": "str"
             }
         ],
         "command": "a2md",
         "description": "Convert Avrotize schema to Markdown documentation",
         "extensions": [
             ".avsc"
@@ -1620,15 +1537,14 @@
     },
     {
         "args": [
             {
                 "help": "Path to the Avrotize schema file (or read from stdin if omitted)",
                 "name": "input",
                 "nargs": "?",
-                "required": false,
                 "type": "str"
             }
         ],
         "command": "pcf",
         "description": "Create the Parsing Canonical Form (PCF) of an Avrotize schema",
         "extensions": [
             ".avsc"
@@ -1636,54 +1552,9 @@
         "function": {
             "args": {
                 "schema_file": "input_file_path"
             },
             "name": "avrotize.avrotools.avsc_to_pcf"
         },
         "prompts": []
-    },
-    {
-        "args": [
-            {
-                "help": "Path to the CSV file (or read from stdin if omitted)",
-                "name": "input",
-                "nargs": "?",
-                "required": false,
-                "type": "str"
-            },
-            {
-                "help": "Path to the Avrotize schema file",
-                "name": "--out",
-                "required": false,
-                "type": "str"
-            },
-            {
-                "help": "Namespace for the Avrotize schema",
-                "name": "--namespace",
-                "required": false,
-                "type": "str"
-            }
-        ],
-        "command": "csv2a",
-        "description": "Convert CSV file to Avrotize schema",
-        "extensions": [
-            ".csv"
-        ],
-        "function": {
-            "args": {
-                "avro_file_path": "output_file_path",
-                "csv_file_path": "input_file_path",
-                "namespace": "args.namespace"
-            },
-            "name": "avrotize.csvtoavro.convert_csv_to_avro"
-        },
-        "prompts": [
-            {
-                "message": "Enter the namespace for the Avro schema",
-                "name": "--namespace",
-                "required": false,
-                "type": "str"
-            }
-        ],
-        "suggested_output_file_path": "{input_file_name}.avsc"
     }
 ]
```

### Comparing `avrotize-1.9.1/avrotize/common.py` & `avrotize-2.0.0/avrotize/common.py`

 * *Files identical despite different names*

### Comparing `avrotize-1.9.1/avrotize/datapackagetoavro.py` & `avrotize-2.0.0/avrotize/datapackagetoavro.py`

 * *Files identical despite different names*

### Comparing `avrotize-1.9.1/avrotize/dependency_resolver.py` & `avrotize-2.0.0/avrotize/dependency_resolver.py`

 * *Files identical despite different names*

### Comparing `avrotize-1.9.1/avrotize/generic/generic.avsc` & `avrotize-2.0.0/avrotize/generic/generic.avsc`

 * *Files identical despite different names*

### Comparing `avrotize-1.9.1/avrotize/jsonstoavro.py` & `avrotize-2.0.0/avrotize/jsonstoavro.py`

 * *Files 1% similar despite different names*

```diff
@@ -1669,18 +1669,14 @@
             with open(avro_schema_path, 'w') as avro_file:
                 json.dump(avro_schema, avro_file, indent=4)
         return avro_schema
 
 
 def convert_jsons_to_avro(json_schema_file_path: str, avro_schema_path: str, namespace: str = '', utility_namespace='', root_class_name='', split_top_level_records=False) -> list | dict | str:
     """Convert JSON schema file to Avro schema file."""
-    
-    if not os.path.exists(json_schema_file_path):
-        raise FileNotFoundError(f'JSON schema file {json_schema_file_path} not found')
-        
     try:
         converter = JsonToAvroConverter()
         converter.split_top_level_records = split_top_level_records
         if root_class_name:
             converter.root_class_name = root_class_name
         return converter.convert_jsons_to_avro(json_schema_file_path, avro_schema_path, namespace, utility_namespace)
     except Exception as e:
```

### Comparing `avrotize-1.9.1/avrotize/kstructtoavro.py` & `avrotize-2.0.0/avrotize/kstructtoavro.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,93 +1,78 @@
-"""
-
-Convert a Kafka schema to an Avro schema.
-
-"""
-
 import json
 
-
 def kafka_type_to_avro_type(kafka_field):
-    """Convert a Kafka field type to an Avro field type."""
     kafka_to_avro_types = {
         'int32': 'int',
         'int64': 'long',
         'string': 'string',
         'boolean': 'boolean',
         'bytes': 'bytes',
         'array': 'array',
         'map': 'map',
         'struct': 'record'
     }
-
+    
     if kafka_field['type'] in kafka_to_avro_types:
         return kafka_to_avro_types[kafka_field['type']]
     elif isinstance(kafka_field['type'], dict):  # Nested struct
         return convert_schema(kafka_field['type'])
     else:
         raise ValueError(f"Unsupported Kafka type: {kafka_field['type']}")
 
-
 def convert_field(field):
-    """Convert a Kafka field to an Avro field."""
     avro_field = {
         'name': field['field'],
         'type': []
     }
-
+    
     if field['optional']:
         avro_field['type'].append('null')
-
+    
     kafka_field_type = kafka_type_to_avro_type(field)
-
+    
     if field['type'] == 'array':
         item_type = kafka_type_to_avro_type(field['items'])
         avro_field['type'].append({'type': 'array', 'items': item_type})
     elif field['type'] == 'map':
         value_type = kafka_type_to_avro_type(field['values'])
         avro_field['type'].append({'type': 'map', 'values': value_type})
     elif field['type'] == 'struct':
         avro_field['type'].append(convert_schema(field))
     else:
         avro_field['type'].append(kafka_field_type)
-
-    if len(avro_field['type']) == 1:
+    
+    if len(avro_field['type'])==1:
         avro_field['type'] = avro_field['type'][0]
-
+        
     return avro_field
 
-
 def convert_schema(kafka_schema):
-    """Convert a Kafka schema to an Avro schema."""
     avro_schema = {
         'type': 'record',
         'name': kafka_schema.get('name', 'MyRecord'),
         'fields': []
     }
-
+    
     for field in kafka_schema['fields']:
         avro_schema['fields'].append(convert_field(field))
-
+    
     return avro_schema
 
 
 def convert_kafka_struct_to_avro_schema(kafka_schema_file_path, avro_file_path):
     """Read a Kafka schema from a file, convert it to an Avro schema, and save it to another file."""
-
-    if not kafka_schema_file_path:
-        raise ValueError("Kafka schema file path is required.")
-
     # Open and read the Kafka schema file
-    with open(kafka_schema_file_path, 'r', encoding='utf-8') as kafka_schema_file:
+    with open(kafka_schema_file_path, 'r') as kafka_schema_file:
         kafka_schema_data = json.load(kafka_schema_file)
 
     # Assuming the whole file content is the schema
     if isinstance(kafka_schema_data, dict) and 'schema' in kafka_schema_data:
         kafka_schema = kafka_schema_data['schema']
     else:
-        kafka_schema = kafka_schema_data
+        kafka_schema = kafka_schema_data 
     avro_schema = convert_schema(kafka_schema)
 
     # Write the converted Avro schema to a file
-    with open(avro_file_path, 'w', encoding='utf-8') as avro_file:
+    with open(avro_file_path, 'w') as avro_file:
         json.dump(avro_schema, avro_file, indent=4)
+
```

### Comparing `avrotize-1.9.1/avrotize/kustotoavro.py` & `avrotize-2.0.0/avrotize/kustotoavro.py`

 * *Files 1% similar despite different names*

```diff
@@ -432,18 +432,10 @@
             os.makedirs(base_dir)
         with open(self.avro_schema_path, 'w', encoding='utf-8') as avro_file:
             json.dump(output, avro_file, indent=4)
 
 
 def convert_kusto_to_avro(kusto_uri: str, kusto_database: str, avro_namespace: str, avro_schema_file: str, emit_cloudevents:bool, emit_cloudevents_xregistry: bool, token_provider=None):
     """ Converts Kusto table schemas to Avro schema format."""
-    
-    if not kusto_uri:
-        raise ValueError("kusto_uri is required")
-    if not kusto_database:
-        raise ValueError("kusto_database is required")
-    if not avro_namespace:
-        avro_namespace = kusto_database
-    
     kusto_to_avro = KustoToAvro(
         kusto_uri, kusto_database, avro_namespace, avro_schema_file,emit_cloudevents, emit_cloudevents_xregistry, token_provider=token_provider)
     return kusto_to_avro.process_all_tables()
```

### Comparing `avrotize-1.9.1/avrotize/parquettoavro.py` & `avrotize-2.0.0/avrotize/parquettoavro.py`

 * *Files 5% similar despite different names*

```diff
@@ -144,14 +144,10 @@
     """
     Convert a Parquet file to an Avro schema file.
 
     :param parquet_file_path: Path to the Parquet file.
     :param avro_file_path: Path to save the Avro schema file.
     :param namespace: Namespace for Avro records.
     """
-    
-    if not os.path.exists(parquet_file_path):
-        raise FileNotFoundError(f"Parquet file not found: {parquet_file_path}")
-    
     converter = ParquetToAvroConverter(parquet_file_path, avro_file_path, namespace)
     converter.convert()
```

### Comparing `avrotize-1.9.1/avrotize/proto2parser.py` & `avrotize-2.0.0/avrotize/proto2parser.py`

 * *Files identical despite different names*

### Comparing `avrotize-1.9.1/avrotize/proto3parser.py` & `avrotize-2.0.0/avrotize/proto3parser.py`

 * *Files identical despite different names*

### Comparing `avrotize-1.9.1/avrotize/prototoavro.py` & `avrotize-2.0.0/avrotize/prototoavro.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,304 +1,243 @@
-"""
-Module to convert Protobuf .proto files to Avro schema.
-"""
-
+import argparse
 import json
 import os
-import re
+
 from avrotize.dependency_resolver import sort_messages_by_dependencies
+
 from . import proto2parser
 from . import proto3parser
+import re
+    
+isomorphic_types = ['float', 'double', 'bytes', 'string']
+imported_types = {}
+
+def proto_type_to_avro_primitive(proto_type):
+    """Map Protobuf types to Avro primitive types."""
+    mapping = {
+        'google.protobuf.Empty': 'null',  # Special handling may be required
+        'bool': 'boolean',
+        'int32': 'int',
+        'uint32': 'int',
+        'sint32': 'int',
+        'int64': 'long',
+        'uint64': 'long',
+        'sint64': 'long',
+        'fixed32': 'int',
+        'fixed64': 'long',
+        'sfixed32': 'int',
+        'sfixed64': 'long',
+        #'NullValue': 'null', 
+        'google.protobuf.Timestamp' : {
+            "type": "long",
+            "logicalType": "timestamp-micros"
+        }
+    }
+    if proto_type in isomorphic_types:
+        return proto_type
+    return mapping.get(proto_type, proto_type)  
 
-class ProtoToAvroConverter:
-    """Class to convert Protobuf .proto files to Avro schema."""
 
-    isomorphic_types = ['float', 'double', 'bytes', 'string']
-    imported_types = {}
+def convert_proto_to_avro(proto_file_path: str, avro_schema_path: str):
+    """Convert Protobuf .proto file to Avro schema."""
 
-    def __init__(self):
-        """Initialize ProtoToAvroConverter."""
-        pass
-
-    def proto_type_to_avro_primitive(self, proto_type):
-        """
-        Map Protobuf types to Avro primitive types.
-
-        Args:
-            proto_type (str): Protobuf type to convert.
-
-        Returns:
-            str or dict: Corresponding Avro type.
-        """
-        mapping = {
-            'google.protobuf.Empty': 'null',  # Special handling may be required
-            'bool': 'boolean',
-            'int32': 'int',
-            'uint32': 'int',
-            'sint32': 'int',
-            'int64': 'long',
-            'uint64': 'long',
-            'sint64': 'long',
-            'fixed32': 'int',
-            'fixed64': 'long',
-            'sfixed32': 'int',
-            'sfixed64': 'long',
-            'google.protobuf.Timestamp': {
-                "type": "long",
-                "logicalType": "timestamp-micros"
-            }
-        }
-        if proto_type in self.isomorphic_types:
-            return proto_type
-        return mapping.get(proto_type, proto_type)
-
-    def convert_proto_to_avro_schema(self, proto_file_path: str) -> list:
-        """
-        Convert .proto file to Avro schema.
-
-        Args:
-            proto_file_path (str): Path to the Protobuf .proto file.
-
-        Returns:
-            list: Avro schema as a list of dictionaries.
-        """
-        with open(proto_file_path, 'r', encoding='utf-8') as proto_file:
+    def convert_proto_to_avro_schema(proto_file_path: str) -> list:
+        """Convert .proto file to Avro schema."""
+        with open(proto_file_path, 'r') as proto_file:
             proto_schema = proto_file.read()
 
-        # Determine whether we have proto3 or proto2 and parse the data
+        # determine whether we have proto3 or proto2 and parse the data
         if re.search(r'syntax\s*=\s*"proto3"', proto_schema):
             data = proto3parser.parse(proto_schema)
         else:
             data = proto2parser.parse(proto_schema)
 
-        # Get the namespace
-        namespace = data.package.value if data.package else ''
-
+        # get the namespace
+        if data.package:
+            namespace = data.package.value
+        else:
+            namespace = ''
         # Avro schema header
         avro_schema = []
-
+        
         for import_ in data.imports:
-            # Handle protobuf imports
+            # handle protobuf imports
             if import_.startswith('google/protobuf/'):
                 script_path = os.path.dirname(os.path.abspath(__file__))
-                avsc_dir = os.path.join(script_path, 'prototypes')
+                avsc_dir = os.path.join(script_path, 'prototypes')            
 
-                # Load the corresponding avsc file from ./prototypes at this script's path into avro_schema
+                # load the corresponding avsc file from ./prototypes at this script's path into avro_schema
                 avsc = f'{avsc_dir}/{import_.replace("google/protobuf/", "").replace(".proto", ".avsc")}'
-                with open(avsc, 'r', encoding='utf-8') as avsc_file:
+                with open(avsc, 'r') as avsc_file:
                     types = json.load(avsc_file)
                     for t in types:
-                        self.imported_types[t["namespace"] + "." + t["name"]] = t
+                        imported_types[t["namespace"]+"."+t["name"]] = t                
             else:
-                # Find the path relative to the current directory
-                cwd = os.path.join(os.getcwd(), os.path.dirname(proto_file_path))
+                # find the path relative to the current directory
+                cwd = os.path.join(os.getcwd(),os.path.dirname(proto_file_path))
                 import_path = os.path.join(cwd, import_)
-                # Raise an exception if the imported file does not exist
+                # raise an exception if the imported file does not exist
                 if not os.path.exists(import_path):
                     raise FileNotFoundError(f'Import file {import_path} does not exist.')
-
-                avro_schema.extend(self.convert_proto_to_avro_schema(import_path))
-
-        # Convert message fields
+                                
+                avro_schema.extend(convert_proto_to_avro_schema(import_path))
+                    
+        
+        ## Convert message fields
         for _, m in data.messages.items():
-            self.handle_message(m, avro_schema, namespace)
+            handle_message(m, avro_schema, namespace)        
 
-        # Convert enum fields
+        ## Convert enum fields
         for _, enum_type in data.enums.items():
-            self.handle_enum(enum_type, avro_schema, namespace)
+            handle_enum(enum_type, avro_schema, namespace)
 
         # Sort the messages in avro_schema by dependencies
         return sort_messages_by_dependencies(avro_schema)
+        
+    
+    avro_schema = convert_proto_to_avro_schema(proto_file_path)
+    ## Convert the Avro schema to JSON and write it to the file
+    with open(avro_schema_path, 'w') as avro_file:
+        avro_file.write(json.dumps(avro_schema, indent=2))
 
-    @staticmethod
-    def clean_comment(comment):
-        """
-        Clean comments by stripping slashes, newlines, linefeeds, and extra whitespace.
-
-        Args:
-            comment (str): The comment to clean.
-
-        Returns:
-            str: Cleaned comment.
-        """
-        if comment:
-            return comment.replace('//', '').replace('\n', '').lstrip().rstrip()
-        return None
+    print(f'Converted {proto_file_path} to {avro_schema_path}')
 
-    def handle_enum(self, enum_type, avro_schema, namespace):
-        """
-        Convert enum fields to avro schema.
-
-        Args:
-            enum_type: The enum type from the parsed proto file.
-            avro_schema (list): The list to append the converted enum schema.
-            namespace (str): The namespace for the enum.
-        """
-        comment = self.clean_comment(enum_type.comment.content if enum_type.comment and enum_type.comment.content else None)
 
-        # Create avro schema
-        avro_enum = {
+def handle_enum(enum_type, avro_schema, namespace):
+    """Convert enum fields to avro schema."""
+    comment = enum_type.comment.content if enum_type.comment and enum_type.comment.content else None
+    if comment:
+        # strip slashes, newlines, linefeeds from the comment and then extra whitespace
+        comment = comment.replace('//', '').replace('\n','').lstrip().rstrip()
+
+    # create avro schema
+    avro_enum = {
             'name': enum_type.name,
             'type': 'enum',
-            'namespace': namespace,
+            'namespace' : namespace,
             'symbols': [],
             'dependencies': []
         }
 
-        if comment:
-            avro_enum['doc'] = comment
+    if comment:
+        avro_enum['doc'] = comment
 
-        for value in enum_type.fields:
-            avro_enum['symbols'].append(value.name)
+    for value in enum_type.fields:
+        avro_enum['symbols'].append(value.name)
 
-        avro_schema.append(avro_enum)
+    avro_schema.append(avro_enum)
 
-    def handle_message(self, m, avro_schema, namespace):
-        """
-        Convert protobuf messages to avro records.
 
-        Args:
-            m: The message type from the parsed proto file.
-            avro_schema (list): The list to append the converted message schema.
-            namespace (str): The namespace for the message.
-        """
-        dependencies = []
+def handle_message(m, avro_schema, namespace):
+    """Convert protobuf messages to avro records."""
+    dependencies = []
 
-        comment = self.clean_comment(m.comment.content if m.comment and m.comment.content else None)
-
-        avro_record = {
+    comment = m.comment.content if m.comment and m.comment.content else None
+    if comment:
+           # strip slashes, newlines, linefeeds from the comment and then extra whitespace
+       comment = comment.replace('//', '').replace('\n','').lstrip().rstrip()
+    avro_record = {
             'type': 'record',
             'name': m.name,
-            'namespace': namespace,
+            'namespace' : namespace,
             'fields': []
         }
+    if comment:
+        avro_record['doc'] = comment
 
+        
+    for f in m.fields:
+        avro_type = get_avro_type_for_field(m, namespace, dependencies, f)
+        comment = f.comment.content if f.comment and f.comment.content else None
         if comment:
-            avro_record['doc'] = comment
-
-        for f in m.fields:
-            avro_type = self.get_avro_type_for_field(m, namespace, dependencies, f)
-            comment = self.clean_comment(f.comment.content if f.comment and f.comment.content else None)
+                # strip slashes, newlines, linefeeds from the comment and then extra whitespace
+            comment = comment.replace('//', '').replace('\n','').lstrip().rstrip()
 
-            avro_field = {
+        avro_field = {
                 'name': f.name,
                 'type': avro_type,
-            }
-
-            if comment:
-                avro_field['doc'] = comment
+                }
+        if comment:
+            avro_field['doc'] = comment
 
-            avro_record['fields'].append(avro_field)
+        avro_record['fields'].append(avro_field)
 
-        for f in m.oneofs:
-            avro_oneof = {
+    for f in m.oneofs:
+        avro_oneof = {
                 'name': f.name,
                 'type': []
-            }
-            comment = self.clean_comment(f.comment.content if f.comment and f.comment.content else None)
-
+                }
+        comment = f.comment.content if f.comment and f.comment.content else None
+        if comment:
+                # strip slashes, newlines, linefeeds from the comment and then extra whitespace
+            comment = comment.replace('//', '').replace('\n','').lstrip().rstrip()
+            avro_oneof['doc'] = comment
+
+        for o in f.fields:
+            avro_type = get_avro_type_for_field(m, namespace, dependencies, o)
+            comment = o.comment.content if o.comment and o.comment.content else None
             if comment:
-                avro_oneof['doc'] = comment
-
-            for o in f.fields:
-                avro_type = self.get_avro_type_for_field(m, namespace, dependencies, o)
-                comment = self.clean_comment(o.comment.content if o.comment and o.comment.content else None)
-
-                if comment:
-                    o['doc'] = comment
-
-                avro_oneof['type'].append(avro_type)
-
-            avro_record['fields'].append(avro_oneof)
-
-        if dependencies:
-            avro_record['dependencies'] = dependencies
-        avro_schema.append(avro_record)
-
-        for _, mi in m.messages.items():
-            self.handle_message(mi, avro_schema, namespace)
-
-        # Convert enum fields
-        for _, enum_type in m.enums.items():
-            self.handle_enum(enum_type, avro_schema, namespace)
-
-    def get_avro_type_for_field(self, m, namespace, dependencies, f):
-        """
-        Get Avro type for a Protobuf field.
-
-        Args:
-            m: The message type from the parsed proto file.
-            namespace (str): The namespace for the message.
-            dependencies (list): The list to append the dependencies.
-            f: The field from the parsed proto file.
-
-        Returns:
-            str or dict: Corresponding Avro type.
-        """
-        field_type = None
-        is_custom = False
-        if f.label == 'repeated' or f.type == 'map':
-            field_type = self.proto_type_to_avro_primitive(f.val_type)
-            is_custom = field_type == f.val_type and field_type not in self.isomorphic_types
+                # strip slashes, newlines, linefeeds from the comment and then extra whitespace
+                comment = comment.replace('//', '').replace('\n','').lstrip().rstrip()
+            avro_oneof['type'].append(avro_type)            
+
+        avro_record['fields'].append(avro_oneof)
+
+    if dependencies:
+       avro_record['dependencies'] = dependencies    
+    avro_schema.append(avro_record)
+
+    for _, mi in m.messages.items():
+        handle_message(mi, avro_schema, namespace)        
+
+    ## Convert enum fields
+    for _, enum_type in m.enums.items():
+        handle_enum(enum_type, avro_schema, namespace)
+
+def get_avro_type_for_field(m, namespace, dependencies, f):
+    field_type = None
+    is_custom = False
+    if f.label == 'repeated' or f.type == 'map':
+        field_type = proto_type_to_avro_primitive(f.val_type)
+        is_custom = field_type == f.val_type and field_type not in isomorphic_types
+    else:
+        field_type = proto_type_to_avro_primitive(f.type)
+        is_custom = field_type == f.type and field_type not in isomorphic_types
+
+    if is_custom:
+        if f.type in imported_types:
+            field_type = imported_types[f.type]
+            imported_types[f.type] = f.type
         else:
-            field_type = self.proto_type_to_avro_primitive(f.type)
-            is_custom = field_type == f.type and field_type not in self.isomorphic_types
-
-        if is_custom:
-            if f.type in self.imported_types:
-                field_type = self.imported_types[f.type]
-                self.imported_types[f.type] = f.type
-            else:
-                found = False
-                for k, mi in m.messages.items():
-                    if mi.name == field_type:
-                        schema = []
-                        self.handle_message(mi, schema, namespace)
-                        del m.messages[k]
-                        field_type = schema[0]
-                        if 'dependencies' in field_type:
-                            dependencies.extend(field_type['dependencies'])
-                            del field_type['dependencies']
-                        found = True
-                        break
-                if not found:
-                    dependencies.append(field_type)
-
-        if f.label == 'optional':
-            field_type = ["null", field_type]
-        if f.label == 'repeated':
-            avro_type = {
+            found = False
+            for k, mi in m.messages.items():
+                if mi.name == field_type:
+                    schema = []
+                    handle_message(mi, schema, namespace)
+                    del m.messages[k]
+                    field_type = schema[0]
+                    if 'dependencies' in field_type:
+                        dependencies.extend(field_type['dependencies'])
+                        del field_type['dependencies']
+
+                    found = True
+                    break 
+            if not found:
+                dependencies.append(field_type)
+
+    if f.label == 'optional':
+        field_type = ["null", field_type]
+    if f.label == 'repeated':
+        avro_type = {
                 "type": "array",
-                "items": field_type
-            }
-        elif f.type == 'map':
-            avro_type = {
+                "items" : field_type                    
+                }
+    elif f.type == 'map':
+        avro_type = {
                 "type": "map",
-                "values": field_type,
-            }
-        else:
-            avro_type = field_type
-        return avro_type
-
-def convert_proto_to_avro(proto_file_path: str, avro_schema_path: str):
-    """
-    Convert Protobuf .proto file to Avro schema.
+                "values" : field_type,
+                }
+    else:
+        avro_type = field_type
+    return avro_type
 
-    Args:
-        proto_file_path (str): Path to the Protobuf .proto file.
-        avro_schema_path (str): Path to save the Avro schema .avsc file.
-
-    Raises:
-        FileNotFoundError: If the proto file does not exist.
-        ValueError: If the file extensions are incorrect.
-    """
-    if not os.path.exists(proto_file_path):
-        raise FileNotFoundError(f'Proto file {proto_file_path} does not exist.')
 
-    converter = ProtoToAvroConverter()
-    avro_schema = converter.convert_proto_to_avro_schema(proto_file_path)
-
-    # Convert the Avro schema to JSON and write it to the file
-    with open(avro_schema_path, 'w', encoding='utf-8') as avro_file:
-        avro_file.write(json.dumps(avro_schema, indent=2))
-
-    print(f'Converted {proto_file_path} to {avro_schema_path}')
```

### Comparing `avrotize-1.9.1/avrotize/prototypes/any.avsc` & `avrotize-2.0.0/avrotize/prototypes/any.avsc`

 * *Files identical despite different names*

### Comparing `avrotize-1.9.1/avrotize/prototypes/api.avsc` & `avrotize-2.0.0/avrotize/prototypes/api.avsc`

 * *Files identical despite different names*

### Comparing `avrotize-1.9.1/avrotize/prototypes/duration.avsc` & `avrotize-2.0.0/avrotize/prototypes/duration.avsc`

 * *Files identical despite different names*

### Comparing `avrotize-1.9.1/avrotize/prototypes/field_mask.avsc` & `avrotize-2.0.0/avrotize/prototypes/field_mask.avsc`

 * *Files identical despite different names*

### Comparing `avrotize-1.9.1/avrotize/prototypes/struct.avsc` & `avrotize-2.0.0/avrotize/prototypes/struct.avsc`

 * *Files identical despite different names*

### Comparing `avrotize-1.9.1/avrotize/prototypes/timestamp.avsc` & `avrotize-2.0.0/avrotize/prototypes/timestamp.avsc`

 * *Files identical despite different names*

### Comparing `avrotize-1.9.1/avrotize/prototypes/type.avsc` & `avrotize-2.0.0/avrotize/prototypes/type.avsc`

 * *Files identical despite different names*

### Comparing `avrotize-1.9.1/avrotize/prototypes/wrappers.avsc` & `avrotize-2.0.0/avrotize/prototypes/wrappers.avsc`

 * *Files identical despite different names*

### Comparing `avrotize-1.9.1/avrotize/xsdtoavro.py` & `avrotize-2.0.0/avrotize/xsdtoavro.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 # pylint: disable=line-too-long, consider-iterating-dictionary, too-many-locals, too-many-branches
 
 """Converts XSD to Avro schema."""
 
-import os
 import re
 from typing import Dict, List, Tuple
 import xml.etree.ElementTree as ET
 import json
 from urllib.parse import urlparse
 from avrotize.common import avro_namespace, generic_type
 
@@ -355,30 +354,23 @@
         if len(avro_schema) == 1:
             return avro_schema[0]
         else:
             return avro_schema
 
     def convert_xsd_to_avro(self, xsd_path: str, avro_path: str, namespace: str | None = None):
         """Convert XSD to Avro schema and write to a file."""
-        
-        
         avro_schema = self.xsd_to_avro(xsd_path, code_namespace=namespace)
         with open(avro_path, 'w', encoding='utf-8') as f:
             json.dump(avro_schema, f, indent=4)
 
 
 def convert_xsd_to_avro(xsd_path: str, avro_path: str, namespace: str | None = None):
     """ 
     Convert XSD to Avro schema and write to a file. 
     
     Params:
     xsd_path: str - Path to the XSD file.
     avro_path: str - Path to the Avro file.
     namespace: str | None - Namespace of the Avro schema.    
     """
-    
-    if not os.path.exists(xsd_path):
-        raise FileNotFoundError(f"XSD file not found at {xsd_path}")    
-    if not namespace:
-        namespace = os.path.splitext(os.path.basename(xsd_path))[0].lower().replace('-', '_')        
     xsd_to_avro = XSDToAvro()
     xsd_to_avro.convert_xsd_to_avro(xsd_path, avro_path, namespace)
```

### Comparing `avrotize-1.9.1/pyproject.toml` & `avrotize-2.0.0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -26,15 +26,14 @@
     "jsoncomparison>=1.1.0",
     "requests>=2.31.0",
     "azure-kusto-data>=4.4.1",
     "azure-identity>=1.6.0",
     "datapackage>=1.15.4",
     "jinja2>=3.1.4",
     "pyiceberg>=0.6.1",
-    "pandas>=2.2.2",
 ]
 [project.optional-dependencies]
 dev = [
     "pytest>=7.2.1",
     "fastavro>=1.9.4",
     "xmlschema>=3.0.2",
     "xmlunittest>=0.5.0",
```

### Comparing `avrotize-1.9.1/PKG-INFO` & `avrotize-2.0.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: avrotize
-Version: 1.9.1
+Version: 2.0.0
 Summary: Tools to convert from and to Avro Schema from various other schema languages.
 Author-email: Clemens Vasters <clemensv@microsoft.com>
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -17,15 +17,14 @@
 Requires-Dist: jsoncomparison>=1.1.0
 Requires-Dist: requests>=2.31.0
 Requires-Dist: azure-kusto-data>=4.4.1
 Requires-Dist: azure-identity>=1.6.0
 Requires-Dist: datapackage>=1.15.4
 Requires-Dist: jinja2>=3.1.4
 Requires-Dist: pyiceberg>=0.6.1
-Requires-Dist: pandas>=2.2.2
 Requires-Dist: pytest>=7.2.1 ; extra == "dev"
 Requires-Dist: fastavro>=1.9.4 ; extra == "dev"
 Requires-Dist: xmlschema>=3.0.2 ; extra == "dev"
 Requires-Dist: xmlunittest>=0.5.0 ; extra == "dev"
 Requires-Dist: pylint>=3.1.0 ; extra == "dev"
 Requires-Dist: dataclasses_json>0.6.4 ; extra == "dev"
 Requires-Dist: dataclasses>=0.6 ; extra == "dev"
```

