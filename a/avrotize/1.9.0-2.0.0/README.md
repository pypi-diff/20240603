# Comparing `tmp/avrotize-1.9.0.tar.gz` & `tmp/avrotize-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "avrotize-1.9.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "avrotize-2.0.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `avrotize-1.9.0.tar` & `avrotize-2.0.0.tar`

### file list

```diff
@@ -1,72 +1,72 @@
--rw-r--r--   0        0        0    32506 2024-06-03 07:34:56.504679 avrotize-1.9.0/README.md
--rw-r--r--   0        0        0     2382 2024-06-03 07:34:56.504679 avrotize-1.9.0/avrotize/__init__.py
--rw-r--r--   0        0        0       88 2024-06-03 07:34:56.504679 avrotize-1.9.0/avrotize/__main__.py
--rw-r--r--   0        0        0      411 2024-06-03 07:35:01.016775 avrotize-1.9.0/avrotize/_version.py
--rw-r--r--   0        0        0     8386 2024-06-03 07:34:56.504679 avrotize-1.9.0/avrotize/asn1toavro.py
--rw-r--r--   0        0        0     4961 2024-06-03 07:34:56.504679 avrotize-1.9.0/avrotize/avrotize.py
--rw-r--r--   0        0        0    25567 2024-06-03 07:34:56.504679 avrotize-1.9.0/avrotize/avrotocpp.py
--rw-r--r--   0        0        0     3015 2024-06-03 07:34:56.504679 avrotize-1.9.0/avrotize/avrotocpp/CMakeLists.txt.jinja
--rw-r--r--   0        0        0       96 2024-06-03 07:34:56.504679 avrotize-1.9.0/avrotize/avrotocpp/build.bat.jinja
--rw-r--r--   0        0        0       73 2024-06-03 07:34:56.504679 avrotize-1.9.0/avrotize/avrotocpp/build.sh.jinja
--rw-r--r--   0        0        0     4621 2024-06-03 07:34:56.504679 avrotize-1.9.0/avrotize/avrotocpp/dataclass_body.jinja
--rw-r--r--   0        0        0      464 2024-06-03 07:34:56.504679 avrotize-1.9.0/avrotize/avrotocpp/vcpkg.json.jinja
--rw-r--r--   0        0        0    45098 2024-06-03 07:34:56.504679 avrotize-1.9.0/avrotize/avrotocsharp.py
--rw-r--r--   0        0        0     1980 2024-06-03 07:34:56.504679 avrotize-1.9.0/avrotize/avrotocsharp/class_test.cs.jinja
--rw-r--r--   0        0        0     8124 2024-06-03 07:34:56.504679 avrotize-1.9.0/avrotize/avrotocsharp/dataclass_core.jinja
--rw-r--r--   0        0        0      579 2024-06-03 07:34:56.504679 avrotize-1.9.0/avrotize/avrotocsharp/enum_test.cs.jinja
--rw-r--r--   0        0        0      807 2024-06-03 07:34:56.504679 avrotize-1.9.0/avrotize/avrotocsharp/project.csproj.jinja
--rw-r--r--   0        0        0     1440 2024-06-03 07:34:56.504679 avrotize-1.9.0/avrotize/avrotocsharp/project.sln.jinja
--rw-r--r--   0        0        0      663 2024-06-03 07:34:56.508679 avrotize-1.9.0/avrotize/avrotocsharp/testproject.csproj.jinja
--rw-r--r--   0        0        0     3551 2024-06-03 07:34:56.508679 avrotize-1.9.0/avrotize/avrotocsv.py
--rw-r--r--   0        0        0     7259 2024-06-03 07:34:56.508679 avrotize-1.9.0/avrotize/avrotodatapackage.py
--rw-r--r--   0        0        0    45933 2024-06-03 07:34:56.508679 avrotize-1.9.0/avrotize/avrotodb.py
--rw-r--r--   0        0        0    21879 2024-06-03 07:34:56.508679 avrotize-1.9.0/avrotize/avrotogo.py
--rw-r--r--   0        0        0      226 2024-06-03 07:34:56.508679 avrotize-1.9.0/avrotize/avrotogo/go_enum.jinja
--rw-r--r--   0        0        0      506 2024-06-03 07:34:56.508679 avrotize-1.9.0/avrotize/avrotogo/go_helpers.jinja
--rw-r--r--   0        0        0     4272 2024-06-03 07:34:56.508679 avrotize-1.9.0/avrotize/avrotogo/go_struct.jinja
--rw-r--r--   0        0        0     1206 2024-06-03 07:34:56.508679 avrotize-1.9.0/avrotize/avrotogo/go_test.jinja
--rw-r--r--   0        0        0      890 2024-06-03 07:34:56.508679 avrotize-1.9.0/avrotize/avrotogo/go_union.jinja
--rw-r--r--   0        0        0     7394 2024-06-03 07:34:56.508679 avrotize-1.9.0/avrotize/avrotographql.py
--rw-r--r--   0        0        0     9057 2024-06-03 07:34:56.508679 avrotize-1.9.0/avrotize/avrotoiceberg.py
--rw-r--r--   0        0        0    58799 2024-06-03 07:34:56.508679 avrotize-1.9.0/avrotize/avrotojava.py
--rw-r--r--   0        0        0    12117 2024-06-03 07:34:56.508679 avrotize-1.9.0/avrotize/avrotojs.py
--rw-r--r--   0        0        0    18104 2024-06-03 07:34:56.508679 avrotize-1.9.0/avrotize/avrotojsons.py
--rw-r--r--   0        0        0    16181 2024-06-03 07:34:56.508679 avrotize-1.9.0/avrotize/avrotokusto.py
--rw-r--r--   0        0        0     5348 2024-06-03 07:34:56.508679 avrotize-1.9.0/avrotize/avrotomd.py
--rw-r--r--   0        0        0      999 2024-06-03 07:34:56.508679 avrotize-1.9.0/avrotize/avrotomd/README.md.jinja
--rw-r--r--   0        0        0     6052 2024-06-03 07:34:56.508679 avrotize-1.9.0/avrotize/avrotools.py
--rw-r--r--   0        0        0     9088 2024-06-03 07:34:56.508679 avrotize-1.9.0/avrotize/avrotoparquet.py
--rw-r--r--   0        0        0    22416 2024-06-03 07:34:56.508679 avrotize-1.9.0/avrotize/avrotoproto.py
--rw-r--r--   0        0        0    19100 2024-06-03 07:34:56.508679 avrotize-1.9.0/avrotize/avrotopython.py
--rw-r--r--   0        0        0    22029 2024-06-03 07:34:56.508679 avrotize-1.9.0/avrotize/avrotorust.py
--rw-r--r--   0        0        0     2232 2024-06-03 07:34:56.508679 avrotize-1.9.0/avrotize/avrotorust/dataclass_enum.rs.jinja
--rw-r--r--   0        0        0     7853 2024-06-03 07:34:56.508679 avrotize-1.9.0/avrotize/avrotorust/dataclass_struct.rs.jinja
--rw-r--r--   0        0        0     3801 2024-06-03 07:34:56.508679 avrotize-1.9.0/avrotize/avrotorust/dataclass_union.rs.jinja
--rw-r--r--   0        0        0    27554 2024-06-03 07:34:56.508679 avrotize-1.9.0/avrotize/avrotots.py
--rw-r--r--   0        0        0    16420 2024-06-03 07:34:56.508679 avrotize-1.9.0/avrotize/avrotoxsd.py
--rw-r--r--   0        0        0    50817 2024-06-03 07:34:56.508679 avrotize-1.9.0/avrotize/commands.json
--rw-r--r--   0        0        0    18352 2024-06-03 07:34:56.508679 avrotize-1.9.0/avrotize/common.py
--rw-r--r--   0        0        0      112 2024-06-03 07:34:56.508679 avrotize-1.9.0/avrotize/constants.py
--rw-r--r--   0        0        0     6571 2024-06-03 07:34:56.508679 avrotize-1.9.0/avrotize/csvtoavro.py
--rw-r--r--   0        0        0     2607 2024-06-03 07:34:56.508679 avrotize-1.9.0/avrotize/datapackagetoavro.py
--rw-r--r--   0        0        0    19374 2024-06-03 07:34:56.508679 avrotize-1.9.0/avrotize/dependency_resolver.py
--rw-r--r--   0        0        0     1272 2024-06-03 07:34:56.508679 avrotize-1.9.0/avrotize/generic/generic.avsc
--rw-r--r--   0        0        0    95346 2024-06-03 07:34:56.508679 avrotize-1.9.0/avrotize/jsonstoavro.py
--rw-r--r--   0        0        0     2112 2024-06-03 07:34:56.508679 avrotize-1.9.0/avrotize/kconnect.json
--rw-r--r--   0        0        0     2537 2024-06-03 07:34:56.508679 avrotize-1.9.0/avrotize/kstructtoavro.py
--rw-r--r--   0        0        0    21168 2024-06-03 07:34:56.508679 avrotize-1.9.0/avrotize/kustotoavro.py
--rw-r--r--   0        0        0     5395 2024-06-03 07:34:56.508679 avrotize-1.9.0/avrotize/parquettoavro.py
--rw-r--r--   0        0        0    19742 2024-06-03 07:34:56.508679 avrotize-1.9.0/avrotize/proto2parser.py
--rw-r--r--   0        0        0    15536 2024-06-03 07:34:56.508679 avrotize-1.9.0/avrotize/proto3parser.py
--rw-r--r--   0        0        0     8722 2024-06-03 07:34:56.508679 avrotize-1.9.0/avrotize/prototoavro.py
--rw-r--r--   0        0        0     3390 2024-06-03 07:34:56.508679 avrotize-1.9.0/avrotize/prototypes/any.avsc
--rw-r--r--   0        0        0     6521 2024-06-03 07:34:56.508679 avrotize-1.9.0/avrotize/prototypes/api.avsc
--rw-r--r--   0        0        0     1629 2024-06-03 07:34:56.508679 avrotize-1.9.0/avrotize/prototypes/duration.avsc
--rw-r--r--   0        0        0     3558 2024-06-03 07:34:56.508679 avrotize-1.9.0/avrotize/prototypes/field_mask.avsc
--rw-r--r--   0        0        0     2394 2024-06-03 07:34:56.508679 avrotize-1.9.0/avrotize/prototypes/struct.avsc
--rw-r--r--   0        0        0      792 2024-06-03 07:34:56.508679 avrotize-1.9.0/avrotize/prototypes/timestamp.avsc
--rw-r--r--   0        0        0     6296 2024-06-03 07:34:56.508679 avrotize-1.9.0/avrotize/prototypes/type.avsc
--rw-r--r--   0        0        0     2571 2024-06-03 07:34:56.512679 avrotize-1.9.0/avrotize/prototypes/wrappers.avsc
--rw-r--r--   0        0        0    17371 2024-06-03 07:34:56.512679 avrotize-1.9.0/avrotize/xsdtoavro.py
--rw-r--r--   0        0        0     1486 2024-06-03 07:34:56.512679 avrotize-1.9.0/pyproject.toml
--rw-r--r--   0        0        0    34200 1970-01-01 00:00:00.000000 avrotize-1.9.0/PKG-INFO
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

### Comparing `avrotize-1.9.0/README.md` & `avrotize-2.0.0/README.md`

 * *Files identical despite different names*

### Comparing `avrotize-1.9.0/avrotize/__init__.py` & `avrotize-2.0.0/avrotize/__init__.py`

 * *Files identical despite different names*

### Comparing `avrotize-1.9.0/avrotize/asn1toavro.py` & `avrotize-2.0.0/avrotize/asn1toavro.py`

 * *Files identical despite different names*

### Comparing `avrotize-1.9.0/avrotize/avrotize.py` & `avrotize-2.0.0/avrotize/avrotize.py`

 * *Files identical despite different names*

### Comparing `avrotize-1.9.0/avrotize/avrotocpp.py` & `avrotize-2.0.0/avrotize/avrotocpp.py`

 * *Files identical despite different names*

### Comparing `avrotize-1.9.0/avrotize/avrotocpp/CMakeLists.txt.jinja` & `avrotize-2.0.0/avrotize/avrotocpp/CMakeLists.txt.jinja`

 * *Files identical despite different names*

### Comparing `avrotize-1.9.0/avrotize/avrotocpp/dataclass_body.jinja` & `avrotize-2.0.0/avrotize/avrotocpp/dataclass_body.jinja`

 * *Files identical despite different names*

### Comparing `avrotize-1.9.0/avrotize/avrotocsharp.py` & `avrotize-2.0.0/avrotize/avrotocsharp.py`

 * *Files identical despite different names*

### Comparing `avrotize-1.9.0/avrotize/avrotocsharp/class_test.cs.jinja` & `avrotize-2.0.0/avrotize/avrotocsharp/class_test.cs.jinja`

 * *Files identical despite different names*

### Comparing `avrotize-1.9.0/avrotize/avrotocsharp/dataclass_core.jinja` & `avrotize-2.0.0/avrotize/avrotocsharp/dataclass_core.jinja`

 * *Files identical despite different names*

### Comparing `avrotize-1.9.0/avrotize/avrotocsharp/enum_test.cs.jinja` & `avrotize-2.0.0/avrotize/avrotocsharp/enum_test.cs.jinja`

 * *Files identical despite different names*

### Comparing `avrotize-1.9.0/avrotize/avrotocsharp/project.csproj.jinja` & `avrotize-2.0.0/avrotize/avrotocsharp/project.csproj.jinja`

 * *Files identical despite different names*

### Comparing `avrotize-1.9.0/avrotize/avrotocsharp/project.sln.jinja` & `avrotize-2.0.0/avrotize/avrotocsharp/project.sln.jinja`

 * *Files identical despite different names*

### Comparing `avrotize-1.9.0/avrotize/avrotocsharp/testproject.csproj.jinja` & `avrotize-2.0.0/avrotize/avrotocsharp/testproject.csproj.jinja`

 * *Files identical despite different names*

### Comparing `avrotize-1.9.0/avrotize/avrotocsv.py` & `avrotize-2.0.0/avrotize/avrotocsv.py`

 * *Files identical despite different names*

### Comparing `avrotize-1.9.0/avrotize/avrotodatapackage.py` & `avrotize-2.0.0/avrotize/avrotodatapackage.py`

 * *Files identical despite different names*

### Comparing `avrotize-1.9.0/avrotize/avrotodb.py` & `avrotize-2.0.0/avrotize/avrotodb.py`

 * *Files identical despite different names*

### Comparing `avrotize-1.9.0/avrotize/avrotogo.py` & `avrotize-2.0.0/avrotize/avrotogo.py`

 * *Files identical despite different names*

### Comparing `avrotize-1.9.0/avrotize/avrotogo/go_struct.jinja` & `avrotize-2.0.0/avrotize/avrotogo/go_struct.jinja`

 * *Files identical despite different names*

### Comparing `avrotize-1.9.0/avrotize/avrotogo/go_test.jinja` & `avrotize-2.0.0/avrotize/avrotogo/go_test.jinja`

 * *Files identical despite different names*

### Comparing `avrotize-1.9.0/avrotize/avrotogo/go_union.jinja` & `avrotize-2.0.0/avrotize/avrotogo/go_union.jinja`

 * *Files identical despite different names*

### Comparing `avrotize-1.9.0/avrotize/avrotographql.py` & `avrotize-2.0.0/avrotize/avrotographql.py`

 * *Files identical despite different names*

### Comparing `avrotize-1.9.0/avrotize/avrotoiceberg.py` & `avrotize-2.0.0/avrotize/avrotoiceberg.py`

 * *Files identical despite different names*

### Comparing `avrotize-1.9.0/avrotize/avrotojava.py` & `avrotize-2.0.0/avrotize/avrotojava.py`

 * *Files identical despite different names*

### Comparing `avrotize-1.9.0/avrotize/avrotojs.py` & `avrotize-2.0.0/avrotize/avrotojs.py`

 * *Files identical despite different names*

### Comparing `avrotize-1.9.0/avrotize/avrotojsons.py` & `avrotize-2.0.0/avrotize/avrotojsons.py`

 * *Files identical despite different names*

### Comparing `avrotize-1.9.0/avrotize/avrotokusto.py` & `avrotize-2.0.0/avrotize/avrotokusto.py`

 * *Files identical despite different names*

### Comparing `avrotize-1.9.0/avrotize/avrotomd.py` & `avrotize-2.0.0/avrotize/avrotomd.py`

 * *Files identical despite different names*

### Comparing `avrotize-1.9.0/avrotize/avrotomd/README.md.jinja` & `avrotize-2.0.0/avrotize/avrotomd/README.md.jinja`

 * *Files identical despite different names*

### Comparing `avrotize-1.9.0/avrotize/avrotools.py` & `avrotize-2.0.0/avrotize/avrotools.py`

 * *Files identical despite different names*

### Comparing `avrotize-1.9.0/avrotize/avrotoparquet.py` & `avrotize-2.0.0/avrotize/avrotoparquet.py`

 * *Files identical despite different names*

### Comparing `avrotize-1.9.0/avrotize/avrotoproto.py` & `avrotize-2.0.0/avrotize/avrotoproto.py`

 * *Files identical despite different names*

### Comparing `avrotize-1.9.0/avrotize/avrotopython.py` & `avrotize-2.0.0/avrotize/avrotopython.py`

 * *Files identical despite different names*

### Comparing `avrotize-1.9.0/avrotize/avrotorust.py` & `avrotize-2.0.0/avrotize/avrotorust.py`

 * *Files identical despite different names*

### Comparing `avrotize-1.9.0/avrotize/avrotorust/dataclass_enum.rs.jinja` & `avrotize-2.0.0/avrotize/avrotorust/dataclass_enum.rs.jinja`

 * *Files identical despite different names*

### Comparing `avrotize-1.9.0/avrotize/avrotorust/dataclass_struct.rs.jinja` & `avrotize-2.0.0/avrotize/avrotorust/dataclass_struct.rs.jinja`

 * *Files identical despite different names*

### Comparing `avrotize-1.9.0/avrotize/avrotorust/dataclass_union.rs.jinja` & `avrotize-2.0.0/avrotize/avrotorust/dataclass_union.rs.jinja`

 * *Files identical despite different names*

### Comparing `avrotize-1.9.0/avrotize/avrotots.py` & `avrotize-2.0.0/avrotize/avrotots.py`

 * *Files identical despite different names*

### Comparing `avrotize-1.9.0/avrotize/avrotoxsd.py` & `avrotize-2.0.0/avrotize/avrotoxsd.py`

 * *Files identical despite different names*

### Comparing `avrotize-1.9.0/avrotize/commands.json` & `avrotize-2.0.0/avrotize/commands.json`

 * *Files identical despite different names*

### Comparing `avrotize-1.9.0/avrotize/common.py` & `avrotize-2.0.0/avrotize/common.py`

 * *Files identical despite different names*

### Comparing `avrotize-1.9.0/avrotize/csvtoavro.py` & `avrotize-2.0.0/avrotize/csvtoavro.py`

 * *Files identical despite different names*

### Comparing `avrotize-1.9.0/avrotize/datapackagetoavro.py` & `avrotize-2.0.0/avrotize/datapackagetoavro.py`

 * *Files identical despite different names*

### Comparing `avrotize-1.9.0/avrotize/dependency_resolver.py` & `avrotize-2.0.0/avrotize/dependency_resolver.py`

 * *Files identical despite different names*

### Comparing `avrotize-1.9.0/avrotize/generic/generic.avsc` & `avrotize-2.0.0/avrotize/generic/generic.avsc`

 * *Files identical despite different names*

### Comparing `avrotize-1.9.0/avrotize/jsonstoavro.py` & `avrotize-2.0.0/avrotize/jsonstoavro.py`

 * *Files identical despite different names*

### Comparing `avrotize-1.9.0/avrotize/kconnect.json` & `avrotize-2.0.0/avrotize/kconnect.json`

 * *Files identical despite different names*

### Comparing `avrotize-1.9.0/avrotize/kstructtoavro.py` & `avrotize-2.0.0/avrotize/kstructtoavro.py`

 * *Files identical despite different names*

### Comparing `avrotize-1.9.0/avrotize/kustotoavro.py` & `avrotize-2.0.0/avrotize/kustotoavro.py`

 * *Files identical despite different names*

### Comparing `avrotize-1.9.0/avrotize/parquettoavro.py` & `avrotize-2.0.0/avrotize/parquettoavro.py`

 * *Files identical despite different names*

### Comparing `avrotize-1.9.0/avrotize/proto2parser.py` & `avrotize-2.0.0/avrotize/proto2parser.py`

 * *Files identical despite different names*

### Comparing `avrotize-1.9.0/avrotize/proto3parser.py` & `avrotize-2.0.0/avrotize/proto3parser.py`

 * *Files identical despite different names*

### Comparing `avrotize-1.9.0/avrotize/prototoavro.py` & `avrotize-2.0.0/avrotize/prototoavro.py`

 * *Files identical despite different names*

### Comparing `avrotize-1.9.0/avrotize/prototypes/any.avsc` & `avrotize-2.0.0/avrotize/prototypes/any.avsc`

 * *Files identical despite different names*

### Comparing `avrotize-1.9.0/avrotize/prototypes/api.avsc` & `avrotize-2.0.0/avrotize/prototypes/api.avsc`

 * *Files identical despite different names*

### Comparing `avrotize-1.9.0/avrotize/prototypes/duration.avsc` & `avrotize-2.0.0/avrotize/prototypes/duration.avsc`

 * *Files identical despite different names*

### Comparing `avrotize-1.9.0/avrotize/prototypes/field_mask.avsc` & `avrotize-2.0.0/avrotize/prototypes/field_mask.avsc`

 * *Files identical despite different names*

### Comparing `avrotize-1.9.0/avrotize/prototypes/struct.avsc` & `avrotize-2.0.0/avrotize/prototypes/struct.avsc`

 * *Files identical despite different names*

### Comparing `avrotize-1.9.0/avrotize/prototypes/timestamp.avsc` & `avrotize-2.0.0/avrotize/prototypes/timestamp.avsc`

 * *Files identical despite different names*

### Comparing `avrotize-1.9.0/avrotize/prototypes/type.avsc` & `avrotize-2.0.0/avrotize/prototypes/type.avsc`

 * *Files identical despite different names*

### Comparing `avrotize-1.9.0/avrotize/prototypes/wrappers.avsc` & `avrotize-2.0.0/avrotize/prototypes/wrappers.avsc`

 * *Files identical despite different names*

### Comparing `avrotize-1.9.0/avrotize/xsdtoavro.py` & `avrotize-2.0.0/avrotize/xsdtoavro.py`

 * *Files identical despite different names*

### Comparing `avrotize-1.9.0/pyproject.toml` & `avrotize-2.0.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `avrotize-1.9.0/PKG-INFO` & `avrotize-2.0.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: avrotize
-Version: 1.9.0
+Version: 2.0.0
 Summary: Tools to convert from and to Avro Schema from various other schema languages.
 Author-email: Clemens Vasters <clemensv@microsoft.com>
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

