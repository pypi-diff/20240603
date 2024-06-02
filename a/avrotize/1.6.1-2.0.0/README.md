# Comparing `tmp/avrotize-1.6.1.tar.gz` & `tmp/avrotize-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "avrotize-1.6.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "avrotize-2.0.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `avrotize-1.6.1.tar` & `avrotize-2.0.0.tar`

### file list

```diff
@@ -1,39 +1,72 @@
--rw-r--r--   0        0        0    30558 2024-05-16 10:46:05.762026 avrotize-1.6.1/README.md
--rw-r--r--   0        0        0     1817 2024-05-16 10:46:05.762026 avrotize-1.6.1/avrotize/__init__.py
--rw-r--r--   0        0        0       88 2024-05-16 10:46:05.762026 avrotize-1.6.1/avrotize/__main__.py
--rw-r--r--   0        0        0      411 2024-05-16 10:46:10.426071 avrotize-1.6.1/avrotize/_version.py
--rw-r--r--   0        0        0     8386 2024-05-16 10:46:05.762026 avrotize-1.6.1/avrotize/asn1toavro.py
--rw-r--r--   0        0        0    18286 2024-05-16 10:46:05.762026 avrotize-1.6.1/avrotize/avrotize.py
--rw-r--r--   0        0        0    48409 2024-05-16 10:46:05.762026 avrotize-1.6.1/avrotize/avrotocsharp.py
--rw-r--r--   0        0        0    58275 2024-05-16 10:46:05.762026 avrotize-1.6.1/avrotize/avrotojava.py
--rw-r--r--   0        0        0    12117 2024-05-16 10:46:05.762026 avrotize-1.6.1/avrotize/avrotojs.py
--rw-r--r--   0        0        0    18104 2024-05-16 10:46:05.762026 avrotize-1.6.1/avrotize/avrotojsons.py
--rw-r--r--   0        0        0    15169 2024-05-16 10:46:05.762026 avrotize-1.6.1/avrotize/avrotokusto.py
--rw-r--r--   0        0        0     5481 2024-05-16 10:46:05.762026 avrotize-1.6.1/avrotize/avrotoparquet.py
--rw-r--r--   0        0        0    22200 2024-05-16 10:46:05.762026 avrotize-1.6.1/avrotize/avrotoproto.py
--rw-r--r--   0        0        0    13360 2024-05-16 10:46:05.762026 avrotize-1.6.1/avrotize/avrotopython.py
--rw-r--r--   0        0        0    10166 2024-05-16 10:46:05.762026 avrotize-1.6.1/avrotize/avrotots.py
--rw-r--r--   0        0        0     9514 2024-05-16 10:46:05.762026 avrotize-1.6.1/avrotize/avrototsql.py
--rw-r--r--   0        0        0    16313 2024-05-16 10:46:05.762026 avrotize-1.6.1/avrotize/avrotoxsd.py
--rw-r--r--   0        0        0    13758 2024-05-16 10:46:05.762026 avrotize-1.6.1/avrotize/common.py
--rw-r--r--   0        0        0      112 2024-05-16 10:46:05.762026 avrotize-1.6.1/avrotize/constants.py
--rw-r--r--   0        0        0    19374 2024-05-16 10:46:05.762026 avrotize-1.6.1/avrotize/dependency_resolver.py
--rw-r--r--   0        0        0     1272 2024-05-16 10:46:05.762026 avrotize-1.6.1/avrotize/generic/generic.avsc
--rw-r--r--   0        0        0    95346 2024-05-16 10:46:05.762026 avrotize-1.6.1/avrotize/jsonstoavro.py
--rw-r--r--   0        0        0     2112 2024-05-16 10:46:05.762026 avrotize-1.6.1/avrotize/kconnect.json
--rw-r--r--   0        0        0     2537 2024-05-16 10:46:05.762026 avrotize-1.6.1/avrotize/kstructtoavro.py
--rw-r--r--   0        0        0    20901 2024-05-16 10:46:05.762026 avrotize-1.6.1/avrotize/kustotoavro.py
--rw-r--r--   0        0        0    19742 2024-05-16 10:46:05.762026 avrotize-1.6.1/avrotize/proto2parser.py
--rw-r--r--   0        0        0    15536 2024-05-16 10:46:05.762026 avrotize-1.6.1/avrotize/proto3parser.py
--rw-r--r--   0        0        0     8722 2024-05-16 10:46:05.762026 avrotize-1.6.1/avrotize/prototoavro.py
--rw-r--r--   0        0        0     3390 2024-05-16 10:46:05.762026 avrotize-1.6.1/avrotize/prototypes/any.avsc
--rw-r--r--   0        0        0     6521 2024-05-16 10:46:05.762026 avrotize-1.6.1/avrotize/prototypes/api.avsc
--rw-r--r--   0        0        0     1629 2024-05-16 10:46:05.762026 avrotize-1.6.1/avrotize/prototypes/duration.avsc
--rw-r--r--   0        0        0     3558 2024-05-16 10:46:05.762026 avrotize-1.6.1/avrotize/prototypes/field_mask.avsc
--rw-r--r--   0        0        0     2394 2024-05-16 10:46:05.762026 avrotize-1.6.1/avrotize/prototypes/struct.avsc
--rw-r--r--   0        0        0      792 2024-05-16 10:46:05.762026 avrotize-1.6.1/avrotize/prototypes/timestamp.avsc
--rw-r--r--   0        0        0     6296 2024-05-16 10:46:05.762026 avrotize-1.6.1/avrotize/prototypes/type.avsc
--rw-r--r--   0        0        0     2571 2024-05-16 10:46:05.762026 avrotize-1.6.1/avrotize/prototypes/wrappers.avsc
--rw-r--r--   0        0        0    17371 2024-05-16 10:46:05.762026 avrotize-1.6.1/avrotize/xsdtoavro.py
--rw-r--r--   0        0        0     1198 2024-05-16 10:46:05.766026 avrotize-1.6.1/pyproject.toml
--rw-r--r--   0        0        0    31264 1970-01-01 00:00:00.000000 avrotize-1.6.1/PKG-INFO
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

### Comparing `avrotize-1.6.1/README.md` & `avrotize-2.0.0/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,22 +1,47 @@
 # Avrotize
 
-Avrotize is a command-line tool for converting data structure definitions between
-different schema formats, using [Apache Avro](https://avro.apache.org/) Schema
-as the integration schema model.
-
-You can use the tool to convert between Avro Schema and other schema formats
-like JSON Schema, XML Schema (XSD), Protocol Buffers (Protobuf), ASN.1, and
-database schema formats like Kusto Data Table Definition (KQL) and T-SQL Table
-Definition (SQL). That means you can also convert from JSON Schema to Protobuf
-going via Avro Schema. 
-
-You can also generate C#, Java, TypeScript, JavaScript, and Python code from the
-Avro Schema documents with Avrotize. The difference to the native Avro tools is
-that Avrotize can emit data classes without Avro library dependencies and,
+Avrotize is a ["Rosetta Stone"](https://en.wikipedia.org/wiki/Rosetta_Stone) for
+data structure definitions, allowing you to convert between numerous data and
+database schema formats and to generate code for different programming
+languages.
+
+It is, for instance, a well-documented and predictable converter and code
+generator for data structures originally defined in JSON Schema (of arbitrary
+complexity).
+
+The tool leans on the Apache Avro-derived [Avrotize
+Schema](specs/avrotize-schema.md) as its schema model.
+
+- Programming languages: Python, C#, Java, TypeScript, JavaScript, Rust, Go, C++
+- SQL Databases: MySQL, MariaDB, PostgreSQL, SQL Server, Oracle, SQLite, BigQuery, Snowflake, Redshift, DB2
+- Other databases: KQL/Kusto, MongoDB, Cassandra, Redis, Elasticsearch, DynamoDB, CosmosDB
+- Data schema formats: Avro, JSON Schema, XML Schema (XSD), Protocol Buffers 2
+  and 3, ASN.1, Apache Parquet
+
+## Installation
+
+You can install Avrotize from PyPI, [having installed Python 3.11 or
+later](https://www.python.org/downloads/):
+
+```bash
+pip install avrotize
+```
+
+## Overview
+
+You can use Avrotize to convert between Avro/Avrotize Schema and other schema
+formats like JSON Schema, XML Schema (XSD), Protocol Buffers (Protobuf), ASN.1,
+and database schema formats like Kusto Data Table Definition (KQL) and T-SQL
+Table Definition (SQL). That means you can also convert from JSON Schema to
+Protobuf going via Avrotize Schema.
+
+You can also generate C#, Java, TypeScript, JavaScript, and Python code from
+Avrotize Schema documents. The difference to the native Avro tools is that
+Avrotize can emit data classes without Avro library dependencies and,
 optionally, with annotations for JSON serialization libraries like Jackson or
 System.Text.Json.
 
 The tool does not convert data (instances of schemas), only the data structure
 definitions.
 
 Mind that the primary objective of the tool is the conversion of schemas that
@@ -47,18 +72,24 @@
 and to common programming language types.
 
 Therefore, Avrotize intentionally ignores common techniques to model
 object-oriented inheritance. For instance, when converting from JSON Schema, all
 content from `allOf` expressions is merged into a single record type rather than
 trying to model the inheritance tree in Avro.
 
-## Why Avro Schema?
+## Avrotize Schema
+
+Avrotize Schema is a schema model that is a full superset of the popular Apache
+Avrotize Schema model. Avrotize Schema is the "pivot point" for this tool. All
+schemas are converted from and to Avrotize Schema.
+
+Since Avrotize Schema is a superset of Avrotize Schema and uses its extensibility
+features, every Avrotize Schema is also a valid Avrotize Schema and vice versa.
 
-Apache Avro Schema is the "pivot point" for this tool. All schemas are converted
-from and to Avro Schema.
+Why did we pick Avro Schema as the foundational schema model?
 
 Avro Schema ...
 
 - provides a simple, clean, and concise way to define data structures. It is
   quite easy to understand and use.
 - is self-contained by design without having or requiring external references.
   Avro Schema can express complex data structure hierarchies spanning multiple
@@ -77,18 +108,16 @@
 - is itself expressed as JSON. That makes it easy to parse and generate, which
   is not the case for Protobuf or ASN.1, which require bespoke parsers.
 
 > It needs to be noted here that while Avro Schema is great for defining data
 > structures, and data classes generated from Avro Schema using this tool or
 > other tools can be used to with the most popular JSON serialization libraries,
 > the Apache Avro project's own JSON encoding has fairly grave interoperability
-> issues with common usage of JSON. A alternate Avro JSON encoding that is more
-> interoperable is proposed in [`avrojson.md`](avrojson.md) for submission to
-> the Apache Avro project; the document also enumerates the specific
-> interoperability issues.
+> issues with common usage of JSON. Avrotize defines an alternate JSON encoding
+> in [`avrojson.md`](avrojson.md).
 
 Avro Schema does not support all the bells and whistles of XML Schema or JSON
 Schema, but that is a feature, not a bug, as it ensures the portability of the
 schemas across different systems and infrastructures. Specifically, Avro Schema
 does not support many of the data validation features found in JSON Schema or
 XML Schema. There are no `pattern`, `format`, `minimum`, `maximum`, or `required`
 keywords in Avro Schema, and Avro does not support conditional validation.
@@ -96,167 +125,161 @@
 In a system where data originates as XML or JSON described by a validating XML
 Schema or JSON Schema, the assumption we make here is that data will be
 validated using its native schema language first, and then the Avro Schema will
 be used for transformation or transfer or storage.
 
 ## Adding CloudEvents columns for database tables
 
-When converting Avro Schema to Kusto Data Table Definition (KQL), T-SQL Table
+When converting Avrotize Schema to Kusto Data Table Definition (KQL), T-SQL Table
 Definition (SQL), or Parquet Schema, the tool can add special columns for
 [CloudEvents](https://cloudevents.io) attributes. CNCF CloudEvents is a
 specification for describing event data in a common way.
 
 The rationale for adding such columns to database tables is that messages and
 events commonly separate event metadata from the payload data, while that
 information is merged when events are projected into a database. The metadata
 often carries important context information about the event that is not
 contained in the payload itself. Therefore, the tool can add those columns to
 the database tables for easy alignment of the message context with the payload
 when building event stores.
 
-## Installation
-
-You can install Avrotize from PyPI, [having installed Python 3.11 or later](https://www.python.org/downloads/):
-
-```bash
-pip install avrotize
-```
 
 ## Usage
 
-Avrotize provides several commands for converting schema formats via Avro Schema.
+Avrotize provides several commands for converting schema formats via Avrotize Schema.
 
-Converting to Avro Schema:
+Converting to Avrotize Schema:
 
-- [`avrotize p2a`´](#convert-proto-schema-to-avro-schema) - Convert Protobuf (2 or 3) schema to Avro schema.
-- [`avrotize j2a`](#convert-json-schema-to-avro-schema) - Convert JSON schema to Avro schema.
-- [`avrotize x2a`](#convert-xml-schema-xsd-to-avro-schema) - Convert XML schema to Avro schema.
-- [`avrotize asn2a`](#convert-asn1-schema-to-avro-schema) - Convert ASN.1 to Avro schema.
-- [`avrotize k2a`](#convert-kusto-table-definition-to-avro-schema) - Convert Kusto table definitions to Avro schema.
-
-Converting from Avro Schema:
-
-- [`avrotize a2p`](#convert-avro-schema-to-proto-schema) - Convert Avro schema to Protobuf 3 schema.
-- [`avrotize a2j`](#convert-avro-schema-to-json-schema) - Convert Avro schema to JSON schema.
-- [`avrotize a2x`](#convert-avro-schema-to-xml-schema) - Convert Avro schema to XML schema.
-- [`avrotize a2k`](#convert-avro-schema-to-kusto-table-declaration) - Convert Avro schema to Kusto table definition.
-- [`avrotize a2tsql`](#convert-avro-schema-to-t-sql-table-definition) - Convert Avro schema to T-SQL table definition.
-- [`avrotize a2pq`](#convert-avro-schema-to-empty-parquet-file) - Convert Avro schema to empty Parquet file.
-
-Generate code from Avro Schema:
-
-- [`avrotize a2csharp`](#generate-c-code-from-avro-schema) - Generate C# code from Avro schema.
-- [`avrotize a2java`](#generate-java-code-from-avro-schema) - Generate Java code from Avro schema.
-- [`avrotize a2py`](#generate-python-code-from-avro-schema) - Generate Python code from Avro schema.
-- [`avrotize a2ts`](#generate-typescript-code-from-avro-schema) - Generate TypeScript code from Avro schema.
-- [`avrotize a2js`](#generate-javascript-code-from-avro-schema) - Generate JavaScript code from Avro schema.
+- [`avrotize p2a`´](#convert-proto-schema-to-avrotize-schema) - Convert Protobuf (2 or 3) schema to Avrotize Schema.
+- [`avrotize j2a`](#convert-json-schema-to-avrotize-schema) - Convert JSON schema to Avrotize Schema.
+- [`avrotize x2a`](#convert-xml-schema-xsd-to-avrotize-schema) - Convert XML schema to Avrotize Schema.
+- [`avrotize asn2a`](#convert-asn1-schema-to-avrotize-schema) - Convert ASN.1 to Avrotize Schema.
+- [`avrotize k2a`](#convert-kusto-table-definition-to-avrotize-schema) - Convert Kusto table definitions to Avrotize Schema.
+- [`avrotize pq2a`](#convert-parquet-schema-to-avrotize-schema) - Convert Parquet schema to Avrotize Schema.
+
+Converting from Avrotize Schema:
+
+- [`avrotize a2p`](#convert-avro-schema-to-proto-schema) - Convert Avrotize Schema to Protobuf 3 schema.
+- [`avrotize a2j`](#convert-avro-schema-to-json-schema) - Convert Avrotize Schema to JSON schema.
+- [`avrotize a2x`](#convert-avro-schema-to-xml-schema) - Convert Avrotize Schema to XML schema.
+- [`avrotize a2k`](#convert-avro-schema-to-kusto-table-declaration) - Convert Avrotize Schema to Kusto table definition.
+- [`avrotize a2tsql`](#convert-avro-schema-to-t-sql-table-definition) - Convert Avrotize Schema to T-SQL table definition.
+- [`avrotize a2pq`](#convert-avro-schema-to-empty-parquet-file) - Convert Avrotize Schema to empty Parquet file.
+
+Generate code from Avrotize Schema:
+
+- [`avrotize a2csharp`](#generate-c-code-from-avro-schema) - Generate C# code from Avrotize Schema.
+- [`avrotize a2java`](#generate-java-code-from-avro-schema) - Generate Java code from Avrotize Schema.
+- [`avrotize a2py`](#generate-python-code-from-avro-schema) - Generate Python code from Avrotize Schema.
+- [`avrotize a2ts`](#generate-typescript-code-from-avro-schema) - Generate TypeScript code from Avrotize Schema.
+- [`avrotize a2js`](#generate-javascript-code-from-avro-schema) - Generate JavaScript code from Avrotize Schema.
 
-### Convert Proto schema to Avro schema
+### Convert Proto schema to Avrotize Schema
 
 ```bash
 avrotize p2a --proto <path_to_proto_file> --avsc <path_to_avro_schema_file>
 ```
 
 Parameters:
 
 - `--proto`: The path to the Protobuf schema file to be converted.
-- `--avsc`: The path to the Avro schema file to write the conversion result to.
+- `--avsc`: The path to the Avrotize Schema file to write the conversion result to.
 
 Conversion notes:
 
 - Proto 2 and Proto 3 syntax are supported.
 - Proto package names are mapped to Avro namespaces. The tool does resolve imports
-  and consolidates all imported types into a single Avro schema file.
+  and consolidates all imported types into a single Avrotize Schema file.
 - The tool embeds all 'well-known' Protobuf 3.0 types in Avro format and injects
   them as needed when the respective types are imported. Only the `Timestamp` type is
   mapped to the Avro logical type 'timestamp-millis'. The rest of the well-known
   Protobuf types are kept as Avro record types with the same field names and types.
 - Protobuf allows any scalar type as key in a `map`, Avro does not. When converting
   from Proto to Avro, the type information for the map keys is ignored.
 - The field numbers in message types are not mapped to the positions of the
   fields in Avro records. The fields in Avro are ordered as they appear in the
-  Proto schema. Consequently, the Avro schema also ignores the `extensions` and
+  Proto schema. Consequently, the Avrotize Schema also ignores the `extensions` and
   `reserved` keywords in the Proto schema.
 - The `optional` keyword results in an Avro field being nullable (union with the
   `null` type), while the `required` keyword results in a non-nullable field.
   The `repeated` keyword results in an Avro field being an array of the field
   type.
 - The `oneof` keyword in Proto is mapped to an Avro union type. 
 - All `options` in the Proto schema are ignored.
 
 
-### Convert Avro schema to Proto schema
+### Convert Avrotize Schema to Proto schema
 
 ```bash
 avrotize a2p --avsc <path_to_avro_schema_file> --proto <path_to_proto_directory>
 ```
 
 Parameters:
 
-- `--avsc`: The path to the Avro schema file to be converted.
+- `--avsc`: The path to the Avrotize Schema file to be converted.
 - `--proto`: The path to the Protobuf schema directory to write the conversion result to.
 
 Conversion notes:
 
 - Avro namespaces are resolved into distinct proto package definitions. The tool will
   create a new `.proto` file with the package definition and an `import` statement for
-  each namespace found in the Avro schema.
+  each namespace found in the Avrotize Schema.
 - Avro type unions `[]` are converted to `oneof` expressions in Proto. Avro allows for
   maps and arrays in the type union, whereas Proto only supports scalar types and
   message type references. The tool will therefore emit message types containing
   a single array or map field for any such case and add it to the containing type,
   and will also recursively resolve further unions in the array and map values.
 - The sequence of fields in a message follows the sequence of fields in the Avro
   record. When type unions need to be resolved into `oneof` expressions, the alternative
   fields need to be assigned field numbers, which will shift the field numbers for any
   subsequent fields.
 
-### Convert JSON schema to Avro schema
+### Convert JSON schema to Avrotize Schema
 
 ```bash
 avrotize j2a --jsons <path_to_json_schema_file> --avsc <path_to_avro_schema_file> [--namespace <avro_schema_namespace>]
 ```
 
 Parameters:
 
 - `--jsons`: The path to the JSON schema file to be converted.
-- `--avsc`: The path to the Avro schema file to write the conversion result to.
-- `--namespace`: (optional) The namespace to use in the Avro schema if the JSON
+- `--avsc`: The path to the Avrotize Schema file to write the conversion result to.
+- `--namespace`: (optional) The namespace to use in the Avrotize Schema if the JSON
   schema does not define a namespace.
 
 Conversion notes:
 
 - [JSON Schema Handling in Avrotize](jsonschema.md)
 
-### Convert Avro schema to JSON schema
+### Convert Avrotize Schema to JSON schema
 
 ```bash
 avrotize a2j --avsc <path_to_avro_schema_file> --json <path_to_json_schema_file>
 ```
 
 Parameters:
 
-- `--avsc`: The path to the Avro schema file to be converted.
+- `--avsc`: The path to the Avrotize Schema file to be converted.
 - `--json`: The path to the JSON schema file to write the conversion result to.
 
 Conversion notes:
 
 - [JSON Schema Handling in Avrotize](jsonschema.md)
 
-### Convert XML Schema (XSD) to Avro schema
+### Convert XML Schema (XSD) to Avrotize Schema
 
 ```bash
 avrotize x2a --xsd <path_to_xsd_file> --avsc <path_to_avro_schema_file> [--namespace <avro_schema_namespace>]
 ```
 
 Parameters:
 
 - `--xsd`: The path to the XML schema file to be converted.
-- `--avsc`: The path to the Avro schema file to write the conversion result to.
-- `--namespace`: (optional) The namespace to use in the Avro schema if the XML
+- `--avsc`: The path to the Avrotize Schema file to write the conversion result to.
+- `--namespace`: (optional) The namespace to use in the Avrotize Schema if the XML
   schema does not define a namespace.
 
 Conversion notes:
 
 - All XML Schema constructs are mapped to Avro record types with fields, whereby
   **both**, elements and attributes, become fields in the record. XML is therefore
   flattened into fields and this aspect of the structure is not preserved.
@@ -269,51 +292,51 @@
   Avro type.
 - `complexType` declarations that have simple content where a base type is augmented
   with attributes is mapped to a record type in Avro. Any other facets defined on
   the complex type are ignored.
 - If the schema defines a single root element, the tool will emit a single Avro
   record type. If the schema defines multiple root elements, the tool will emit a
   union of record types, each corresponding to a root element.
-- All fields in the resulting Avro Schema are annotated with an `xmlkind`
+- All fields in the resulting Avrotize Schema are annotated with an `xmlkind`
   extension attribute that indicates whether the field was an `element` or an
   `attribute` in the XML schema.
 
-## Convert Avro schema to XML schema
+## Convert Avrotize Schema to XML schema
 
 ```bash
 avrotize a2x --avsc <path_to_avro_schema_file> --xsd <path_to_xsd_schema_file>
 ```
 
 Parameters:
 
-- `--avsc`: The path to the Avro schema file to be converted.
+- `--avsc`: The path to the Avrotize Schema file to be converted.
 - `--xsd`: The path to the XML schema file to write the conversion result to.
 
 Conversion notes:
 
 - Avro record types are mapped to XML Schema complex types with elements.
 - Avro enum types are mapped to XML Schema simple types with restrictions.
 - Avro logical types are mapped to XML Schema simple types with restrictions
   where required.
 - Avro unions are mapped to standalone XSD simple type definitions with a
   union restriction if all union types are primitives.
 - Avro unions with complex types are resolved into distinct types for
   each option that are then joined with a choice.
 
-## Convert ASN.1 schema to Avro schema
+## Convert ASN.1 schema to Avrotize Schema
 
 ```bash
 avrotize asn2a --asn <path_to_asn1_schema_file>[,<path_to_asn1_schema_file>,...]  --avsc <path_to_avro_schema_file>
 ```
 
 Parameters:
 
 - `--asn`: The path to the ASN.1 schema file to be converted. The tool supports
   multiple files in a comma-separated list.
-- `--avsc`: The path to the Avro schema file to write the conversion result to.
+- `--avsc`: The path to the Avrotize Schema file to write the conversion result to.
 
 Conversion notes:
 
 - All ASN.1 types are mapped to Avro record types, enums, and unions. Avro does
   not support the same level of nesting of types as ASN.1, the tool will map
   the types to the best fit.
 - The tool will map the following ASN.1 types to Avro types:
@@ -334,25 +357,25 @@
     `VideotexString`, `GraphicString`, `VisibleString`, `GeneralString`, `UniversalString`,
     `CharacterString`, `T61String` are all mapped to Avro string type.
   - All other ASN.1 types are mapped to Avro string type.
 - The ability to parse ASN.1 schema files is limited and the tool may not be able
   to parse all ASN.1 files. The tool is based on the Python asn1tools package and
   is limited to that package's capabilities.
 
-### Convert Kusto table definition to Avro schema
+### Convert Kusto table definition to Avrotize Schema
 
 ```bash
 avrotize k2a --kusto-uri <kusto_cluster_uri> --kusto-database <kusto_database> --avsc <path_to_avro_schema_file> --emit-cloudevents-xregistry
 ```
 
 Parameters:
 
 - `--kusto-uri`: The URI of the Kusto cluster to connect to.
 - `--kusto-database`: The name of the Kusto database to read the table definitions from.
-- `--avsc`: The path to the Avro schema file to write the conversion result to.
+- `--avsc`: The path to the Avrotize Schema file to write the conversion result to.
 - `--emit-cloudevents-xregistry`: (optional) See discussion below.
 
 Conversion notes:
 - The tool directly connects to the Kusto cluster and reads the table
   definitions from the specified database. The tool will convert all tables in
   the database to Avro record types, returned in a top-level type union.
 - Connecting to the Kusto cluster leans on the same authentication mechanisms as
@@ -383,218 +406,235 @@
   Schema for each table in the embedded schema registry. If one or more tables
   are found to contain CloudEvent data (as indicated by the presence of the
   CloudEvents attribute columns), the tool will inspect the content of the
   `type` (or `__type` or `__type`) columns to determine which CloudEvent types
   have been stored in the table and will emit a CloudEvent definition and schema
   for each unique type.
 
-### Convert Avro schema to Kusto table declaration
+### Convert Avrotize Schema to Kusto table declaration
 
 ```bash
 avrotize a2k --avsc <path_to_avro_schema_file> --kusto <path_to_kusto_kql_file> [--record-type <record_type>] [--emit-cloudevents-columns] [--emit-cloudevents-dispatch]
 ```
 
 Parameters:
 
-- `--avsc`: The path to the Avro schema file to be converted.
+- `--avsc`: The path to the Avrotize Schema file to be converted.
 - `--kusto`: The path to the Kusto KQL file to write the conversion result to.
 - `--record-type`: (optional) The name of the Avro record type to convert to a Kusto table.
 - `--emit-cloudevents-columns`: (optional) If set, the tool will add
   [CloudEvents](https://cloudevents.io) attribute columns to the table: `___id`,
   `___source`, `___subject`, `___type`, and `___time`.
 - `--emit-cloudevents-dispatch`: (optional) If set, the tool will add a table named
   `_cloudevents_dispatch` to the script or database, which serves as an ingestion and
   dispatch table for CloudEvents. The table has columns for the core CloudEvents attributes
-  and a `data` column that holds the CloudEvents data. For each table in the Avro schema,
+  and a `data` column that holds the CloudEvents data. For each table in the Avrotize Schema,
   the tool will create an update policy that maps events whose `type` attribute matches
   the Avro type name to the respective table.
   
 
 Conversion notes:
 
-- Only the Avro `record` type can be mapped to a Kusto table. If the Avro schema
+- Only the Avro `record` type can be mapped to a Kusto table. If the Avrotize Schema
   contains other types (like `enum` or `array`), the tool will ignore them.
-- Only the first `record` type in the Avro schema is converted to a Kusto table.
-  If the Avro schema contains other `record` types, they will be ignored. The
+- Only the first `record` type in the Avrotize Schema is converted to a Kusto table.
+  If the Avrotize Schema contains other `record` types, they will be ignored. The
   `--record-type` option can be used to specify which `record` type to convert.
 - The fields of the record are mapped to columns in the Kusto table. Fields that
   are records or arrays or maps are mapped to columns of type `dynamic` in the
   Kusto table.
 
-### Convert Avro schema to T-SQL table definition
+### Convert Avrotize Schema to T-SQL table definition
 
 ```bash
 avrotize a2tsql --avsc <path_to_avro_schema_file> --tsql <path_to_sql_file> [--record-type <record_type>] [--emit-cloudevents-columns]
 ```
 
 Parameters:
 
-- `--avsc`: The path to the Avro schema file to be converted.
+- `--avsc`: The path to the Avrotize Schema file to be converted.
 - `--tsql`: The path to the T-SQL file to write the conversion result to.
 - `--record-type`: (optional) The name of the Avro record type to convert to a T-SQL table.
 - `--emit-cloudevents-columns`: (optional) If set, the tool will add
   [CloudEvents](https://cloudevents.io) attribute columns to the table: `__id`,
   `__source`, `__subject`, `__type`, and `__time`.
 
 Conversion notes:
 
-- Only the Avro `record` type can be mapped to a T-SQL table. If the Avro schema
+- Only the Avro `record` type can be mapped to a T-SQL table. If the Avrotize Schema
   contains other types (like `enum` or `array`), the tool will ignore them.
-- Only the first `record` type in the Avro schema is converted to a T-SQL table.
-  If the Avro schema contains other `record` types, they will be ignored. The
+- Only the first `record` type in the Avrotize Schema is converted to a T-SQL table.
+  If the Avrotize Schema contains other `record` types, they will be ignored. The
   `--record-type` option can be used to specify which `record` type to convert.
 - The fields of the record are mapped to columns in the T-SQL table. Fields of
   type `record` or `array` or `map` are mapped to columns of type `varchar(max)` in
   the T-SQL table and it's assumed for them to hold JSON data.
-- The emitted script sets extended properties to the columns with the Avro schema
+- The emitted script sets extended properties to the columns with the Avrotize Schema
   definition of the field in a JSON format. This allows for easy introspection of
-  the serialized Avro schema in the field definition.
+  the serialized Avrotize Schema in the field definition.
 
-## Convert Avro schema to empty Parquet file
+## Convert Avrotize Schema to empty Parquet file
 
 ```bash
 avrotize a2pq --avsc <path_to_avro_schema_file> --parquet <path_to_parquet_schema_file> [--record-type <record-type-from-avro>] [--emit-cloudevents-columns]
 ```
 
 Parameters:
 
-- `--avsc`: The path to the Avro schema file to be converted.
+- `--avsc`: The path to the Avrotize Schema file to be converted.
 - `--parquet`: The path to the Parquet schema file to write the conversion result to.
 - `--record-type`: (optional) The name of the Avro record type to convert to a Parquet schema.
 - `--emit-cloudevents-columns`: (optional) If set, the tool will add
   [CloudEvents](https://cloudevents.io) attribute columns to the Parquet schema:
   `__id`, `__source`, `__subject`, `__type`, and `__time`.
 
 Conversion notes:
 
 - The emitted Parquet file contains only the schema, no data rows.
-- The tool only supports writing Parquet files for Avro schema that describe a
-  single `record` type. If the Avro schema contains a top-level union, the
+- The tool only supports writing Parquet files for Avrotize Schema that describe a
+  single `record` type. If the Avrotize Schema contains a top-level union, the
   `--record-type` option must be used to specify which record type to emit.
 - The fields of the record are mapped to columns in the Parquet file. Array and
   record fields are mapped to Parquet nested types. Avro type unions are mapped
   to structures, not to Parquet unions since those are not supported by the
   PyArrow library used here.
 
-### Generate C# code from Avro schema
+## Convert Parquet schema to Avrotize Schema
+
+```bash
+avrotize pq2a --parquet <path_to_parquet_schema_file> --avsc <path_to_avro_schema_file> --namespace <avro_schema_namespace>
+```
+
+Parameters:
+
+- `--parquet`: The path to the Parquet file whose schema is to be converted.
+- `--avsc`: The path to the Avrotize Schema file to write the conversion result to.
+- `--namespace`: The namespace to use in the Avrotize Schema.
+
+Conversion notes:
+
+- The tool reads the schema from the Parquet file and converts it to an Avro
+  schema. The Avrotize Schema is written to the specified file.
+
+### Generate C# code from Avrotize Schema
 
 ```bash
 avrotize a2csharp --avsc <path_to_avro_schema_file> --csharp <path_to_csharp_directory> [--avro-annotation] [--system-text-json-annotation] [--newtonsoft-json-annotation] [--pascal-properties]
 ```
 
 Parameters:
-- `--avsc`: The path to the Avro schema file to be converted.
+- `--avsc`: The path to the Avrotize Schema file to be converted.
 - `--csharp`: The path to the C# directory to write the conversion result to.
 - `--avro-annotation`: (optional) If set, the tool will add Avro annotations to the C# classes.
 - `--system-text-json-annotation`: (optional) If set, the tool will add System.Text.Json annotations to the C# classes.
 - `--newtonsoft-json-annotation`: (optional) If set, the tool will add Newtonsoft.Json annotations to the C# classes.
 - `--pascal-properties`: (optional) If set, the tool will use PascalCase properties in the C# classes.
 - `--namespace`: (optional) The namespace to use in the generated C# classes.
 
 Conversion notes:
-- The tool generates C# classes that represent the Avro schema as data classes.
+- The tool generates C# classes that represent the Avrotize Schema as data classes.
 - Using the `--system-text-json-annotation` or `--newtonsoft-json-annotation` option
   will add annotations for the respective JSON serialization library to the generated
-  C# classes. Because the [`JSON Schema to Avro`](#convert-json-schema-to-avro-schema) conversion generally
-  preserves the JSON Schema structure in the Avro schema, the generated C# classes
+  C# classes. Because the [`JSON Schema to Avro`](#convert-json-schema-to-avrotize-schema) conversion generally
+  preserves the JSON Schema structure in the Avrotize Schema, the generated C# classes
   can be used to serialize and deserialize data that is valid per the input JSON schema.
 - Only the `--system-text-json-annotation` option generates classes that support type unions.
 - The classes are generated into a directory structure that reflects the Avro namespace
   structure. The tool drops a minimal, default `.csproj` project file into the given
   directory if none exists.
 
 Read more about the C# code generation in the [C# code generation documentation](csharpcodegen.md).
 
 
-### Generate Java code from Avro schema
+### Generate Java code from Avrotize Schema
 
 ```bash
 avrotize a2java --avsc <path_to_avro_schema_file> --java <path_to_java_directory> [--package <java_package_name>] [--avro-annotation] [--jackson-annotation] [--pascal-properties]
 ```
 
 Parameters:
-- `--avsc`: The path to the Avro schema file to be converted.
+- `--avsc`: The path to the Avrotize Schema file to be converted.
 - `--java`: The path to the Java directory to write the conversion result to.
 - `--package`: (optional) The Java package name to use in the generated Java classes.
 - `--avro-annotation`: (optional) If set, the tool will add Avro annotations to the Java classes.
 - `--jackson-annotation`: (optional) If set, the tool will add Jackson annotations to the Java classes.
 - `--pascal-properties`: (optional) If set, the tool will use PascalCase properties in the Java classes.
 
 Conversion notes:
 
-- The tool generates Java classes that represent the Avro schema as data classes. 
+- The tool generates Java classes that represent the Avrotize Schema as data classes. 
 - Using the `--jackson-annotation` option will add annotations for the Jackson 
   JSON serialization library to the generated Java classes. Because the 
-  [`JSON Schema to Avro`](#convert-json-schema-to-avro-schema) conversion generally
-  preserves the JSON Schema structure in the Avro schema, the generated Java classes
+  [`JSON Schema to Avro`](#convert-json-schema-to-avrotize-schema) conversion generally
+  preserves the JSON Schema structure in the Avrotize Schema, the generated Java classes
   can be used to serialize and deserialize data that is valid per the input JSON schema.
 - The directory `/src/main/java` is created in the specified directory and the
   generated Java classes are written to this directory. The tool drops a
   minimal, default `pom.xml` Maven project file into the given directory if none
   exists.
 
 Read more about the Java code generation in the [Java code generation documentation](javacodegen.md).
 
-### Generate Python code from Avro schema
+### Generate Python code from Avrotize Schema
 
-This command generates Python dataclasses from an Avro schema.
+This command generates Python dataclasses from an Avrotize Schema.
 
 ```bash
 avrotize a2py --avsc <path_to_avro_schema_file> --python <path_to_python_directory> [--package <python_package_name>]
 ```
 
 Parameters:
-- `--avsc`: The path to the Avro schema file to be converted.
+- `--avsc`: The path to the Avrotize Schema file to be converted.
 - `--python`: The path to the Python directory to write the conversion result to.
 - `--package`: (optional) The Python package name to use in the generated Python classes.
 - `--avro-annotation`: (optional) If set, the tool will add Avro annotations to the Python classes.
 - `--dataclasses-json-annotation`: (optional) If set, the tool will add dataclasses-json annotations to the Python classes
 
 Conversion notes:
 - The tool generates Python dataclasses (Python 3.7 or later)
 - The classes are generated into a directory structure that reflects the Avro namespace
   structure. The tool drops a minimal, default `__init__.py` file into any created
   package directories if none exists.
 
-### Generate TypeScript code from Avro schema
+### Generate TypeScript code from Avrotize Schema
 
 ```bash
 avrotize a2ts --avsc <path_to_avro_schema_file> --ts <path_to_typescript_directory> [--package <typescript_namespace>] [--avro-annotation] [--typedjson-annotation]
 ``` 
 
 Parameters:
-- `--avsc`: The path to the Avro schema file to be converted.
+- `--avsc`: The path to the Avrotize Schema file to be converted.
 - `--ts`: The path to the TypeScript directory to write the conversion result to.
 - `--package`: (optional) The TypeScript namespace to use in the generated TypeScript classes.
 - `--avro-annotation`: (optional) If set, the tool will add Avro annotations to the TypeScript classes.
 - `--typedjson-annotation`: (optional) If set, the tool will add TypedJSON annotations to the TypeScript classes.
 
 Conversion notes:
-- The tool generates TypeScript interfaces that represent the Avro schema as data classes.
+- The tool generates TypeScript interfaces that represent the Avrotize Schema as data classes.
 - Using the `--typedjson-annotation` option will add annotations for the TypedJSON
   JSON serialization library to the generated TypeScript classes. Because the
-  [`JSON Schema to Avro`](#convert-json-schema-to-avro-schema) conversion generally
-  preserves the JSON Schema structure in the Avro schema, the generated TypeScript
+  [`JSON Schema to Avro`](#convert-json-schema-to-avrotize-schema) conversion generally
+  preserves the JSON Schema structure in the Avrotize Schema, the generated TypeScript
   classes can be used to serialize and deserialize data that is valid per the input JSON schema.
 - The classes are generated into a directory structure that reflects the Avro namespace
 
-### Generate JavaScript code from Avro schema
+### Generate JavaScript code from Avrotize Schema
 
 ```bash
 avrotize a2js --avsc <path_to_avro_schema_file> --js <path_to_javascript_directory> [--package <javascript_namespace>] [--avro-annotation]
 ```
 
 Parameters:
-- `--avsc`: The path to the Avro schema file to be converted.
+- `--avsc`: The path to the Avrotize Schema file to be converted.
 - `--js`: The path to the JavaScript directory to write the conversion result to.
 - `--package`: (optional) The JavaScript namespace to use in the generated JavaScript classes.
 - `--avro-annotation`: (optional) If set, the tool will add Avro annotations to the JavaScript classes.
 
 Conversion notes:
-- The tool generates JavaScript classes that represent the Avro schema as data classes.
+- The tool generates JavaScript classes that represent the Avrotize Schema as data classes.
 - The classes are generated into a directory structure that reflects the Avro namespace
 
 
 ## Contributing
 
 Contributions are welcome! Please feel free to submit a Pull Request.
```

### Comparing `avrotize-1.6.1/avrotize/__init__.py` & `avrotize-2.0.0/avrotize/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -6,41 +6,54 @@
 from .asn1toavro import convert_asn1_to_avro
 from .xsdtoavro import convert_xsd_to_avro
 from .prototoavro import  convert_proto_to_avro
 from .avrotojsons import convert_avro_to_json_schema
 from .avrotokusto import convert_avro_to_kusto_file, convert_avro_to_kusto_db
 from .avrotoparquet import convert_avro_to_parquet
 from .avrotoproto import convert_avro_to_proto
-from .avrototsql import convert_avro_to_tsql
+from .avrotodb import convert_avro_to_sql
 from .avrotoxsd import convert_avro_to_xsd
 from .avrotojava import convert_avro_to_java, convert_avro_schema_to_java
 from .avrotocsharp import convert_avro_to_csharp, convert_avro_schema_to_csharp
 from .avrotopython import convert_avro_to_python, convert_avro_schema_to_python
 from .avrotots import convert_avro_to_typescript, convert_avro_schema_to_typescript
 from .avrotojs import convert_avro_to_javascript, convert_avro_schema_to_javascript
+from .avrotomd import convert_avro_to_markdown
+from .avrotocpp import convert_avro_to_cpp, convert_avro_schema_to_cpp
+from .avrotogo import convert_avro_to_go, convert_avro_schema_to_go
+from .avrotorust import convert_avro_to_rust, convert_avro_schema_to_rust
+from .avrotodatapackage import convert_avro_to_datapackage
 
 __all__ = [
     "convert_proto_to_avro",
     "convert_jsons_to_avro",
     "convert_kafka_struct_to_avro_schema",
     "convert_kusto_to_avro",
     "convert_asn1_to_avro",
     "convert_xsd_to_avro",
     "convert_proto_to_avro",
     "convert_avro_to_json_schema",
     "convert_avro_to_kusto_file",
     "convert_avro_to_kusto_db",
     "convert_avro_to_parquet",
     "convert_avro_to_proto",
-    "convert_avro_to_tsql",
+    "convert_avro_to_sql",
     "convert_avro_to_xsd",
     "convert_avro_to_java",
     "convert_avro_schema_to_java",
     "convert_avro_to_csharp",
     "convert_avro_schema_to_csharp",
     "convert_avro_to_python",
     "convert_avro_schema_to_python",
     "convert_avro_to_typescript",
     "convert_avro_schema_to_typescript",
     "convert_avro_to_javascript",
-    "convert_avro_schema_to_javascript"
+    "convert_avro_schema_to_javascript",
+    "convert_avro_to_markdown",
+    "convert_avro_to_cpp",
+    "convert_avro_schema_to_cpp",
+    "convert_avro_to_go",
+    "convert_avro_schema_to_go",
+    "convert_avro_to_rust",
+    "convert_avro_schema_to_rust",
+    "convert_avro_to_datapackage"
 ]
```

### Comparing `avrotize-1.6.1/avrotize/asn1toavro.py` & `avrotize-2.0.0/avrotize/asn1toavro.py`

 * *Files identical despite different names*

### Comparing `avrotize-1.6.1/avrotize/avrotocsharp.py` & `avrotize-2.0.0/avrotize/avrotocsharp.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,195 +1,24 @@
 # pylint: disable=line-too-long
 
 """ AvroToCSharp class for converting Avro schema to C# classes """
 
 import json
 import os
 import re
-from typing import Dict, List, Tuple, Union
+from typing import Any, Dict, List, Tuple, Union, cast
+import uuid
 
-from avrotize.common import is_generic_avro_type, pascal
+from avrotize.common import is_generic_avro_type, pascal, process_template
 import glob
 
 JsonNode = Dict[str, 'JsonNode'] | List['JsonNode'] | str | None
 
 
 INDENT = '    '
-CSPROJ_CONTENT = """
-<Project Sdk="Microsoft.NET.Sdk">
-    <PropertyGroup>
-        <TargetFramework>net8.0</TargetFramework>
-        <Nullable>enable</Nullable>
-        <GenerateDocumentationFile>true</GenerateDocumentationFile>
-    </PropertyGroup>
-    <ItemGroup>
-        <PackageReference Include="Apache.Avro" Version="1.11.3" />
-        <PackageReference Include="Newtonsoft.Json" Version="13.0.3" />
-        <PackageReference Include="System.Text.Json" Version="8.0.3" />
-        <PackageReference Include="System.Memory.Data" Version="8.0.0" />
-    </ItemGroup>
-</Project>     
-"""
-
-PREAMBLE_TOBYTEARRAY = \
-"""
-var contentType = new System.Net.Mime.ContentType(contentTypeString);
-byte[]? result = null;
-"""
-
-
-EPILOGUE_TOBYTEARRAY_COMPRESSION = \
-"""
-if (result != null && contentType.MediaType.EndsWith("+gzip"))
-{
-    var stream = new System.IO.MemoryStream();
-    using (var gzip = new System.IO.Compression.GZipStream(stream, System.IO.Compression.CompressionMode.Compress))
-    {
-        gzip.Write(result, 0, result.Length);
-    }
-    result = stream.ToArray();
-}
-"""
-
-EPILOGUE_TOBYTEARRAY = \
-"""
-return ( result != null ) ? result : throw new System.NotSupportedException($"Unsupported media type {contentType.MediaType}");
-"""
-
-AVRO_TOBYTEARRAY = \
-"""
-if (contentType.MediaType.StartsWith("avro/binary") || contentType.MediaType.StartsWith("application/vnd.apache.avro+avro"))
-{
-    var stream = new System.IO.MemoryStream();
-    var writer = new global::Avro.Specific.SpecificDatumWriter<{type_name}>({type_name}.AvroSchema);
-    var encoder = new global::Avro.IO.BinaryEncoder(stream);
-    writer.Write(this, encoder);
-    encoder.Flush();
-    result = stream.ToArray();
-}
-else if (contentType.MediaType.StartsWith("avro/json") || contentType.MediaType.StartsWith("application/vnd.apache.avro+json"))
-{
-    var stream = new System.IO.MemoryStream();
-    var writer = new global::Avro.Specific.SpecificDatumWriter<{type_name}>({type_name}.AvroSchema);
-    var encoder = new global::Avro.IO.JsonEncoder({type_name}.AvroSchema, stream);
-    writer.Write(this, encoder);
-    encoder.Flush();
-    result = stream.ToArray();
-}
-"""
-
-SYSTEM_TEXT_JSON_TOBYTEARRAY = \
-"""
-if (contentType.MediaType.StartsWith(System.Net.Mime.MediaTypeNames.Application.Json))
-{
-    result = System.Text.Json.JsonSerializer.SerializeToUtf8Bytes(this);
-}"""
-
-NEWTONSOFT_JSON_TOBYTEARRAY = \
-"""
-if (contentType.MediaType.StartsWith(System.Net.Mime.MediaTypeNames.Application.Json))
-{
-    result = System.Text.Encoding.GetEncoding(contentType.CharSet??"utf-8").GetBytes(Newtonsoft.Json.JsonConvert.SerializeObject(this));
-}
-"""
-
-PREAMBLE_FROMDATA = \
-"""
-var contentType = new System.Net.Mime.ContentType(contentTypeString);
-"""
-
-PREAMBLE_FROMDATA_COMPRESSION = \
-"""
-if ( contentType.MediaType.EndsWith("+gzip"))
-{
-    var stream = data switch
-    {
-        System.IO.Stream s => s, System.BinaryData bd => bd.ToStream(), byte[] bytes => new System.IO.MemoryStream(bytes),
-        _ => throw new NotSupportedException("Data is not of a supported type for gzip decompression")
-    };
-    using (var gzip = new System.IO.Compression.GZipStream(stream, System.IO.Compression.CompressionMode.Decompress))
-    {
-        System.IO.MemoryStream memoryStream = new System.IO.MemoryStream();
-        gzip.CopyTo(memoryStream);
-        memoryStream.Position = 0;
-        data = memoryStream.ToArray();
-    }
-}
-"""
-
-EPILOGUE_FROMDATA = \
-"""
-throw new System.NotSupportedException($"Unsupported media type {contentType.MediaType}");
-"""
-
-SYSTEM_TEXT_JSON_FROMDATA = \
-"""
-if ( contentType.MediaType.StartsWith(System.Net.Mime.MediaTypeNames.Application.Json))
-{
-    if (data is System.Text.Json.JsonElement) 
-    {
-        return System.Text.Json.JsonSerializer.Deserialize<{type_name}>((System.Text.Json.JsonElement)data);
-    }
-    else if ( data is string)
-    {
-        return System.Text.Json.JsonSerializer.Deserialize<{type_name}>((string)data);
-    }
-    else if (data is System.BinaryData)
-    {
-        return ((System.BinaryData)data).ToObjectFromJson<{type_name}>();
-    }
-    else if (data is byte[])
-    {
-        return System.Text.Json.JsonSerializer.Deserialize<{type_name}>(new ReadOnlySpan<byte>((byte[])data));
-    }
-    else if (data is System.IO.Stream)
-    {
-        return System.Text.Json.JsonSerializer.DeserializeAsync<{type_name}>((System.IO.Stream)data).Result;
-    }
-}
-"""
-
-NEWTONSOFT_JSON_FROMDATA = \
-"""
-if ( contentType.MediaType.StartsWith(System.Net.Mime.MediaTypeNames.Application.Json))
-{
-    if (data is string)
-    {
-        return Newtonsoft.Json.JsonConvert.DeserializeObject<{type_name}>((string)data);
-    }
-    else if (data is System.BinaryData)
-    {
-        return ((System.BinaryData)data).ToObjectFromJson<{type_name}>();
-    }
-}
-"""
-
-AVRO_FROMDATA = \
-"""
-if ( contentType.MediaType.StartsWith("avro/") || contentType.MediaType.StartsWith("application/vnd.apache.avro") )
-{
-    var stream = data switch
-    {
-        System.IO.Stream s => s, System.BinaryData bd => bd.ToStream(), byte[] bytes => new System.IO.MemoryStream(bytes),
-        _ => throw new NotSupportedException("Data is not of a supported type for conversion to Stream")
-    };
-    #pragma warning disable CS8625 // Cannot convert null literal to non-nullable reference type.
-    if (contentType.MediaType.StartsWith("avro/binary") || contentType.MediaType.StartsWith("application/vnd.apache.avro+avro"))
-    {
-        var reader = new global::Avro.Generic.GenericDatumReader<global::Avro.Generic.GenericRecord>({type_name}.AvroSchema, {type_name}.AvroSchema);
-        return new {type_name}(reader.Read(null, new global::Avro.IO.BinaryDecoder(stream)));
-    }
-    if ( contentType.MediaType.StartsWith("avro/json") || contentType.MediaType.StartsWith("application/vnd.apache.avro+json"))
-    {
-        var reader = new global::Avro.Generic.GenericDatumReader<global::Avro.Generic.GenericRecord>({type_name}.AvroSchema, {type_name}.AvroSchema);
-        return new {type_name}(reader.Read(null, new global::Avro.IO.JsonDecoder({type_name}.AvroSchema, stream)));
-    }
-    #pragma warning restore CS8625
-}    
-"""
 
 AVRO_CLASS_PREAMBLE = \
 """
 public {type_name}(global::Avro.Generic.GenericRecord obj)
 {
     global::Avro.Specific.ISpecificRecord self = this;
     for (int i = 0; obj.Schema.Fields.Count > i; ++i)
@@ -207,18 +36,28 @@
         self.schema_doc: JsonNode = None
         self.output_dir = os.getcwd()
         self.pascal_properties = False
         self.system_text_json_annotation = False
         self.newtonsoft_json_annotation = False
         self.avro_annotation = False
         self.generated_types: Dict[str,str] = {}
+        self.generated_avro_types: Dict[str, Dict[str, Union[str, Dict, List]]] = {}
 
-    def concat_namespace(self, namespace: str, name: str) -> str:
+    def get_qualified_name(self, namespace: str, name: str) -> str:
         """ Concatenates namespace and name with a dot separator """
         return f"{namespace}.{name}" if namespace != '' else name
+    
+    def concat_namespace(self, namespace: str, name: str) -> str:
+        """ Concatenates namespace and name with a dot separator """
+        if namespace and name:
+            return f"{namespace}.{name}"
+        elif namespace:
+            return namespace
+        else:
+            return name
 
     def map_primitive_to_csharp(self, avro_type: str) -> str:
         """ Maps Avro primitive types to C# types """
         mapping = {
             'null': 'void',  # Placeholder, actual handling for nullable types is in the union logic
             'boolean': 'bool',
             'int': 'int',
@@ -239,17 +78,19 @@
             'internal', 'is', 'lock', 'long', 'namespace', 'new', 'null', 'object', 'operator', 'out', 'override',
             'params', 'private', 'protected', 'public', 'readonly', 'ref', 'return', 'sbyte', 'sealed', 'short', 'sizeof',
             'stackalloc', 'static', 'string', 'struct', 'switch', 'this', 'throw', 'true', 'try', 'typeof', 'uint', 'ulong',
             'unchecked', 'unsafe', 'ushort', 'using', 'virtual', 'void', 'volatile', 'while'
         ]
         return word in reserved_words
 
-    def is_csharp_primitive_type(self, avro_type: str) -> bool:
+    def is_csharp_primitive_type(self, csharp_type: str) -> bool:
         """ Checks if an Avro type is a C# primitive type """
-        return avro_type in ['null', 'bool', 'int', 'long', 'float', 'double', 'bytes', 'string', 'DateTime', 'decimal', 'short', 'sbyte', 'ushort', 'uint', 'ulong', 'byte[]', 'object']
+        if csharp_type.endswith('?'):
+            csharp_type = csharp_type[:-1]
+        return csharp_type in ['null', 'bool', 'int', 'long', 'float', 'double', 'bytes', 'string', 'DateTime', 'decimal', 'short', 'sbyte', 'ushort', 'uint', 'ulong', 'byte[]', 'object']
     
     def map_csharp_primitive_to_clr_type(self, cs_type: str) -> str:
         """ Maps C# primitive types to CLR types"""
         map = {
             "int": "Int32",
             "long": "Int64",
             "float": "Single",
@@ -259,15 +100,15 @@
             "sbyte": "SByte",
             "ushort": "UInt16",
             "uint": "UInt32",
             "ulong": "UInt64"
         }
         return map.get(cs_type, cs_type)
 
-    def convert_avro_type_to_csharp(self, class_name: str, field_name: str, avro_type: Union[str, Dict, List], parent_namespace: str) -> str:
+    def convert_avro_type_to_csharp(self, class_name: str, field_name: str, avro_type: JsonNode, parent_namespace: str) -> str:
         """ Converts Avro type to C# type """
         if isinstance(avro_type, str):
             return self.map_primitive_to_csharp(avro_type)
         elif isinstance(avro_type, list):
             # Handle nullable types and unions
             if is_generic_avro_type(avro_type):
                 return 'Dictionary<string, object>'
@@ -301,14 +142,17 @@
         """ Generates a Class """
         class_definition = ''
         avro_namespace = avro_schema.get('namespace', parent_namespace)
         if not 'namespace' in avro_schema:
             avro_schema['namespace'] = parent_namespace
         namespace = pascal(self.concat_namespace(self.base_namespace, avro_namespace))
         class_name = pascal(avro_schema['name'])
+        ref = 'global::'+self.get_qualified_name(namespace, class_name)
+        if ref in self.generated_types:
+            return ref
         
         class_definition += f"/// <summary>\n/// { avro_schema.get('doc', class_name ) }\n/// </summary>\n"
         fields_str = [self.generate_property(field, class_name, avro_namespace) for field in avro_schema.get('fields', [])]
         class_body = "\n".join(fields_str)
         class_definition += f"public partial class {class_name}"
         if self.avro_annotation:
             class_definition += " : global::Avro.Specific.ISpecificRecord"
@@ -340,104 +184,60 @@
                 if self.is_csharp_reserved_word(field_name):
                     field_name = f"@{field_name}"
                 field_type = self.convert_avro_type_to_csharp(class_name, field_name, field['type'], avro_namespace)
                 if self.pascal_properties:
                     field_name = pascal(field_name)
                 if field_name == class_name:
                     field_name += "_"
-                if class_name + '.' + field_type in self.generated_types and self.generated_types[class_name + '.' + field_type] == "union":
+                if field_type in self.generated_types and self.generated_types[field_type] == "union":
                     get_method += f"\n{INDENT*3}case {pos}: return this.{field_name}?.ToObject();"
                     put_method += f"\n{INDENT*3}case {pos}: this.{field_name} = {field_type}.FromObject(fieldValue); break;"
                 else:    
                     get_method += f"\n{INDENT*3}case {pos}: return this.{field_name};"
                     put_method += f"\n{INDENT*3}case {pos}: this.{field_name} = ({field_type})fieldValue; break;"
             get_method += f"\n{INDENT*3}default: throw new global::Avro.AvroRuntimeException($\"Bad index {{fieldPos}} in Get()\");"
             put_method += f"\n{INDENT*3}default: throw new global::Avro.AvroRuntimeException($\"Bad index {{fieldPos}} in Put()\");"
             get_method += "\n"+INDENT+INDENT+"}\n"+INDENT+"}"
             put_method += "\n"+INDENT+INDENT+"}\n"+INDENT+"}"
             class_definition += f"\n{get_method}\n{put_method}\n"
 
-        # emit ToByteArray method
-        if self.avro_annotation or self.system_text_json_annotation or self.newtonsoft_json_annotation:
-            class_definition += f"\n{INDENT}/// <summary>\n{INDENT}/// Converts the object to a byte array\n{INDENT}/// </summary>"
-            class_definition += f"\n{INDENT}/// <param name=\"contentTypeString\">The content type string of the desired encoding</param>"
-            class_definition += f"\n{INDENT}/// <returns>The encoded data</returns>"
-            class_definition += f"\n{INDENT}public byte[] ToByteArray(string contentTypeString)\n{INDENT}{{"
-            class_definition += f'\n{INDENT*2}'.join((PREAMBLE_TOBYTEARRAY).split("\n"))
-            if self.avro_annotation:
-                class_definition += f'\n{INDENT*2}'+f'\n{INDENT*2}'.join(
-                    AVRO_TOBYTEARRAY.strip().replace("{type_name}", class_name).split("\n"))
-            if self.system_text_json_annotation:
-                class_definition += f'\n{INDENT*2}'+f'\n{INDENT*2}'.join(
-                    SYSTEM_TEXT_JSON_TOBYTEARRAY.strip().replace("{type_name}", class_name).split("\n"))
-            if self.newtonsoft_json_annotation:
-                class_definition += f'\n{INDENT*2}'+f'\n{INDENT*2}'.join(
-                    NEWTONSOFT_JSON_TOBYTEARRAY.strip().replace("{type_name}", class_name).split("\n"))
-            if self.avro_annotation or self.system_text_json_annotation or self.newtonsoft_json_annotation:
-                class_definition += f"\n{INDENT*2}".join((EPILOGUE_TOBYTEARRAY_COMPRESSION).split("\n"))
-            class_definition += f"\n{INDENT*2}".join((EPILOGUE_TOBYTEARRAY).split("\n"))+f"\n{INDENT}}}"
-
-            # emit FromData factory method
-            class_definition += f"\n\n{INDENT}/// <summary>\n{INDENT}/// Creates an object from the data\n{INDENT}/// </summary>"
-            class_definition += f"\n{INDENT}/// <param name=\"data\">The input data to convert</param>"
-            class_definition += f"\n{INDENT}/// <param name=\"contentTypeString\">The content type string of the derired encoding</param>"
-            class_definition += f"\n{INDENT}/// <returns>The converted object</returns>"
-            class_definition += f"\n{INDENT}public static {class_name}? FromData(object? data, string? contentTypeString )\n{INDENT}{{"
-            class_definition += f'\n{INDENT*2}if ( data == null ) return null;'
-            class_definition += f'\n{INDENT*2}if ( data is {class_name}) return ({class_name})data;'
-            class_definition += f'\n{INDENT*2}if ( contentTypeString == null ) contentTypeString = System.Net.Mime.MediaTypeNames.Application.Octet;'
-            class_definition += f'\n{INDENT*2}'.join(((PREAMBLE_FROMDATA)).split("\n"))
-            if self.avro_annotation or self.system_text_json_annotation or self.newtonsoft_json_annotation:
-                class_definition += f'\n{INDENT*2}'.join(((PREAMBLE_FROMDATA_COMPRESSION)).split("\n"))
-            if self.avro_annotation:
-                class_definition += f'\n{INDENT*2}'+f'\n{INDENT*2}'.join(
-                    AVRO_FROMDATA.strip().replace("{type_name}", class_name).split("\n"))
-            if self.system_text_json_annotation:
-                class_definition += f'\n{INDENT*2}'+f'\n{INDENT*2}'.join(
-                    SYSTEM_TEXT_JSON_FROMDATA.strip().replace("{type_name}", class_name).split("\n"))
-            if self.newtonsoft_json_annotation:
-                class_definition += f'\n{INDENT*2}'+f'\n{INDENT*2}'.join(
-                    NEWTONSOFT_JSON_FROMDATA.strip().replace("{type_name}", class_name).split("\n"))
-            class_definition += f"\n{INDENT*2}".join((EPILOGUE_FROMDATA).split('\n'))+f"\n{INDENT}}}"
+        # emit helper methods
+        class_definition += process_template(
+            "avrotocsharp/dataclass_core.jinja", 
+            class_name=class_name, 
+            avro_annotation=self.avro_annotation, 
+            system_text_json_annotation=self.system_text_json_annotation, 
+            newtonsoft_json_annotation=self.newtonsoft_json_annotation,
+            json_match_clauses=self.create_is_json_match_clauses(avro_schema, avro_namespace, class_name))
 
-            # emit IsJsonMatch method for System.Text.Json
-            if self.system_text_json_annotation:
-                class_definition += self.create_is_json_match_method(avro_schema, avro_namespace, class_name)
         class_definition += "\n"+"}"
 
         if write_file:
             self.write_to_file(namespace, class_name, class_definition)
-        ref = 'global::'+self.concat_namespace(namespace, class_name)
+        
         self.generated_types[ref] = "class"
+        self.generated_avro_types[ref] = avro_schema
         return ref
 
-    def create_is_json_match_method(self, avro_schema, parent_namespace, class_name) -> str:
+    def create_is_json_match_clauses(self, avro_schema, parent_namespace, class_name) -> List[str]:
         """ Generates the IsJsonMatch method for System.Text.Json """
-        class_definition = ''
-        class_definition += f"\n\n{INDENT}/// <summary>\n{INDENT}/// Checks if the JSON element matches the schema\n{INDENT}/// </summary>"
-        class_definition += f"\n{INDENT}/// <param name=\"element\">The JSON element to check</param>"
-        class_definition += f"\n{INDENT}public static bool IsJsonMatch(System.Text.Json.JsonElement element)\n{INDENT}{{"
-        class_definition += f"\n{INDENT*2}return "
+        clauses: List[str] = []
         field_count = 0
         for field in avro_schema.get('fields', []):
-            if field_count > 0:
-                class_definition += f" && \n{INDENT*3}"
-            field_count += 1
             field_name = field['name']
             if self.is_csharp_reserved_word(field_name):
                 field_name = f"@{field_name}"
             if field_name == class_name:
                 field_name += "_"
             field_type = self.convert_avro_type_to_csharp(
                     class_name, field_name, field['type'], parent_namespace)
-            class_definition += self.get_is_json_match_clause(class_name, field_name, field_type)
+            clauses.append(self.get_is_json_match_clause(class_name, field_name, field_type))
         if field_count == 0:
-            class_definition += "true"
-        class_definition += f";\n{INDENT}}}"
-        return class_definition
+            clauses.append("true")
+        return clauses
 
     def get_is_json_match_clause(self, class_name, field_name, field_type) -> str:
         """ Generates the IsJsonMatch clause for a field """
         class_definition = ''
         field_name_js = field_name[1:] if field_name[0] == '@' else field_name
         is_optional = field_type[-1] == '?'
         field_type = field_type[:-1] if is_optional else field_type
@@ -502,36 +302,44 @@
 
     def generate_enum(self, avro_schema: Dict, parent_namespace: str, write_file: bool) -> str:
         """ Generates an Enum """
         enum_definition = ''
         namespace = pascal(self.concat_namespace(
             self.base_namespace, avro_schema.get('namespace', parent_namespace)))
         enum_name = pascal(avro_schema['name'])
+        ref = 'global::'+self.get_qualified_name(namespace, enum_name)
+        if ref in self.generated_types:
+            return ref
+
         enum_definition += "#pragma warning disable 1591\n\n"
         enum_definition += f"/// <summary>\n/// {avro_schema.get('doc', enum_name )}\n/// </summary>\n"        
         symbols_str = [
             f"{INDENT}{symbol}" for symbol in avro_schema['symbols']]
         enum_body = ",\n".join(symbols_str)
         enum_definition += f"public enum {enum_name}\n{{\n{enum_body}\n}}"
         
         
         if write_file:
             self.write_to_file(namespace, enum_name, enum_definition)
-        ref = 'global::'+self.concat_namespace(namespace, enum_name)
+        ref = 'global::'+self.get_qualified_name(namespace, enum_name)
         self.generated_types[ref] = "enum"
+        self.generated_avro_types[ref] = avro_schema
         return ref
 
     def generate_embedded_union(self, class_name: str, field_name: str, avro_type: List, parent_namespace: str, write_file: bool) -> str:
         """ Generates an embedded Union Class """
+        
         class_definition_ctors = class_definition_decls = class_definition_read = ''
         class_definition_write = class_definition = class_definition_toobject = ''
         class_definition_objctr = class_definition_genericrecordctor = ''
         namespace = pascal(self.concat_namespace(self.base_namespace, parent_namespace))
         list_is_json_match: List [str] = []
         union_class_name = pascal(field_name)+'Union'
+        ref = class_name+'.'+union_class_name
+        
         union_types = [self.convert_avro_type_to_csharp(class_name, field_name+"Option"+str(i), t, parent_namespace) for i,t in enumerate(avro_type)]
         for i, union_type in enumerate(union_types):
             is_dict = is_list = False
             if union_type.startswith("Dictionary<"):
                 # get the type information from the dictionary
                 is_dict = True
                 match = re.findall(r"Dictionary<(.+)\s*,\s*(.+)>", union_type)
@@ -643,16 +451,17 @@
                 f"\n{INDENT*2}/// <summary>\n{INDENT*2}/// Checks if the JSON element matches the schema\n{INDENT*2}/// </summary>\n" + \
                 f"{INDENT*2}public static bool IsJsonMatch(System.Text.Json.JsonElement element)\n{INDENT*2}{{" + \
                 f"\n{INDENT*3}return "+f"\n{INDENT*3} || ".join(list_is_json_match)+f";\n{INDENT*2}}}\n"
         class_definition += f"{INDENT}}}\n}}"
 
         if write_file:
             self.write_to_file(namespace, class_name +"."+union_class_name, class_definition)
-        self.generated_types[class_name+'.'+union_class_name] = "union" # it doesn't matter if the names clash, we just need to know whether it's a union
-        return union_class_name
+        
+        self.generated_types[ref] = "union" # it doesn't matter if the names clash, we just need to know whether it's a union
+        return ref
 
     def find_type(self, kind: str, avro_schema: JsonNode, type_name: str, type_namespace: str, parent_namespace = '') -> JsonNode:
         """ recursively find the type (kind 'record' or 'enum') in the schema """
         if isinstance(avro_schema, list):
             for s in avro_schema:
                 found = self.find_type(kind, s, type_name, type_namespace, parent_namespace)
                 if found:
@@ -704,50 +513,169 @@
             prop += f"{INDENT}[Newtonsoft.Json.JsonProperty(\"{annotation_name}\")]\n"
         prop += f"{INDENT}public {field_type} {field_name} {{ get; {'private ' if 'const' in field else ''}set; }}" + ((" = "+(f"\"{field_default}\"" if isinstance(field_default,str) else field_default) + ";") if field_default else "")
         return prop
 
     def write_to_file(self, namespace: str, name: str, definition: str):
         """ Writes the class or enum to a file """
         directory_path = os.path.join(
-            self.output_dir, os.path.join(namespace.replace('.', os.sep)))
+            self.output_dir, os.path.join('src', namespace.replace('.', os.sep)))
         if not os.path.exists(directory_path):
             os.makedirs(directory_path, exist_ok=True)
         file_path = os.path.join(directory_path, f"{name}.cs")
 
         with open(file_path, 'w', encoding='utf-8') as file:
             # Common using statements (add more as needed)
             file_content = "#pragma warning disable CS8618\n#pragma warning disable CS8603\n\nusing System;\nusing System.Collections.Generic;\n"
             if self.system_text_json_annotation:
                 file_content += "using System.Text.Json;\n"
                 file_content += "using System.Text.Json.Serialization;\n"
             if self.newtonsoft_json_annotation:
                 file_content += "using Newtonsoft.Json;\n"
             
-            # Namespace declaration with correct indentation for the definition
-            file_content += f"\nnamespace {namespace}\n{{\n"
-            indented_definition = '\n'.join(
-                [f"{INDENT}{line}" for line in definition.split('\n')])
-            file_content += f"{indented_definition}\n}}"
+            if namespace:
+                # Namespace declaration with correct indentation for the definition
+                file_content += f"\nnamespace {namespace}\n{{\n"
+                indented_definition = '\n'.join(
+                    [f"{INDENT}{line}" for line in definition.split('\n')])
+                file_content += f"{indented_definition}\n}}"
+            else:
+                file_content += definition
             file.write(file_content)
 
+    def generate_tests(self, output_dir: str) -> None:
+        """ Generates unit tests for all the generated C# classes and enums """
+        test_directory_path = os.path.join(output_dir, "test")
+        if not os.path.exists(test_directory_path):
+            os.makedirs(test_directory_path, exist_ok=True)
+
+        for class_name, type_kind in self.generated_types.items():
+            if type_kind in ["class", "enum"]:
+                self.generate_test_class(class_name, type_kind, test_directory_path)
+
+    def generate_test_class(self, class_name: str, type_kind: str, test_directory_path: str) -> None:
+        """ Generates a unit test class for a given C# class or enum """
+        avro_schema:Dict[str,JsonNode] = cast(Dict[str,JsonNode], self.generated_avro_types.get(class_name, {}))
+        if class_name.startswith("global::"):
+            class_name = class_name[8:]
+        test_class_name = f"{class_name.split('.')[-1]}Tests"
+        namespace = ".".join(class_name.split('.')[:-1])
+        class_base_name = class_name.split('.')[-1]
+
+        if type_kind == "class":
+            fields = self.get_class_test_fields(avro_schema, class_base_name)
+            test_class_definition = process_template(
+                "avrotocsharp/class_test.cs.jinja",
+                namespace=namespace,
+                test_class_name=test_class_name,
+                class_base_name=class_base_name,
+                fields=fields,
+                avro_annotation=self.avro_annotation
+            )
+        elif type_kind == "enum":
+            test_class_definition = process_template(
+                "avrotocsharp/enum_test.cs.jinja",
+                namespace=namespace,
+                test_class_name=test_class_name,
+                enum_base_name=class_base_name
+            )
+
+        test_file_path = os.path.join(test_directory_path, f"{test_class_name}.cs")
+        with open(test_file_path, 'w', encoding='utf-8') as test_file:
+            test_file.write(test_class_definition)
+
+    def get_class_test_fields(self, avro_schema: Dict[str,JsonNode], class_name: str) -> List[Any]:
+        """ Retrieves fields for a given class name """
+        
+        class Field:
+            def __init__(self, fn: str, ft:str, tv:Any, ct: bool, pm: bool):
+                self.field_name = fn
+                self.field_type = ft
+                self.test_value = tv
+                self.is_const = ct
+                self.is_primitive = pm
+
+        fields: List[Field] = []
+        if avro_schema and 'fields' in avro_schema:
+            for field in cast(List[Dict[str,JsonNode]],avro_schema['fields']):
+                field_name = str(field['name'])
+                if self.pascal_properties:
+                    field_name = pascal(field_name)
+                if field_name == class_name:
+                    field_name += "_"
+                if self.is_csharp_reserved_word(field_name):
+                    field_name = f"@{field_name}"
+                field_type = self.convert_avro_type_to_csharp(class_name, field_name, field['type'], str(avro_schema.get('namespace', '')))
+                is_class = field_type in self.generated_types and self.generated_types[field_type] == "class"
+                f = Field(field_name, 
+                          field_type, 
+                          (self.get_test_value(field_type) if not "const" in field else '\"'+str(field["const"])+'\"'), 
+                          "const" in field and field["const"] is not None,
+                          not is_class)
+                fields.append(f)
+        return cast(List[Any], fields)
+    
+    def get_test_value(self, csharp_type: str) -> str:
+        """Returns a default test value based on the Avro type"""
+        test_values = {
+            'string': '"test_string"',
+            'bool': 'true',
+            'int': '42',
+            'long': '42L',
+            'float': '3.14f',
+            'double': '3.14',
+            'decimal': '3.14d',
+            'byte[]': '{0x01, 0x02, 0x03}',
+            'null': 'null',
+            'Date': 'new Date()',
+            'DateTime': 'DateTime.UtcNow()',
+            'Guid': 'Guid.NewGuid()'
+        }
+        if csharp_type.endswith('?'):
+            csharp_type = csharp_type[:-1]
+        return test_values.get(csharp_type, f'new {csharp_type}()')
+
     def convert_schema(self, schema: JsonNode, output_dir: str):
         """ Converts Avro schema to C# """
         if not isinstance(schema, list):
             schema = [schema]
-            
+        
+        project_name = os.path.basename(output_dir)
         self.schema_doc = schema
-        if not glob.glob(os.path.join(output_dir, '*.csproj')):
+        if not os.path.exists(output_dir):
+            os.makedirs(output_dir, exist_ok=True)
+        if not glob.glob(os.path.join(output_dir, "src", "*.sln")):
+            sln_file = os.path.join(
+                output_dir, f"{project_name}.sln")
+            if not os.path.exists(sln_file):
+                if not os.path.exists(os.path.dirname(sln_file)):
+                    os.makedirs(os.path.dirname(sln_file))
+                with open(sln_file, 'w', encoding='utf-8') as file:
+                    file.write(process_template("avrotocsharp/project.sln.jinja", project_name=project_name, uuid=lambda:str(uuid.uuid4())))
+        if not glob.glob(os.path.join(output_dir, "src", "*.csproj")):
             csproj_file = os.path.join(
-                output_dir, f"{os.path.basename(output_dir)}.csproj")
+                output_dir, "src", f"{project_name}.csproj")
             if not os.path.exists(csproj_file):
+                if not os.path.exists(os.path.dirname(csproj_file)):
+                    os.makedirs(os.path.dirname(csproj_file))
                 with open(csproj_file, 'w', encoding='utf-8') as file:
-                    file.write(CSPROJ_CONTENT)
+                    file.write(process_template("avrotocsharp/project.csproj.jinja"))
+        if not glob.glob(os.path.join(output_dir, "test", "*.csproj")):
+            csproj_test_file = os.path.join(
+                output_dir, "test", f"{project_name}-test.csproj")
+            if not os.path.exists(csproj_test_file):
+                if not os.path.exists(os.path.dirname(csproj_test_file)):
+                    os.makedirs(os.path.dirname(csproj_test_file))
+                with open(csproj_test_file, 'w', encoding='utf-8') as file:
+                    file.write(process_template("avrotocsharp/testproject.csproj.jinja", project_name=project_name))
+        
+            
         self.output_dir = output_dir
         for avro_schema in (avs for avs in schema if isinstance(avs, dict)):
             self.generate_class_or_enum(avro_schema, '')
+        self.generate_tests(output_dir)
 
     def convert(self, avro_schema_path: str, output_dir: str):
         """ Converts Avro schema to C# """
         with open(avro_schema_path, 'r', encoding='utf-8') as file:
             schema = json.load(file)
         self.convert_schema(schema, output_dir)
 
@@ -757,14 +685,17 @@
 
     Converts Avro schema to C# classes
 
     Args:
         avro_schema_path (_type_): Avro input schema path  
         cs_file_path (_type_): Output C# file path 
     """
+    
+    if not base_namespace:
+        base_namespace = os.path.splitext(os.path.basename(cs_file_path))[0].replace('-', '_')
     avrotocs = AvroToCSharp(base_namespace)
     avrotocs.pascal_properties = pascal_properties
     avrotocs.system_text_json_annotation = system_text_json_annotation
     avrotocs.newtonsoft_json_annotation = newtonsoft_json_annotation
     avrotocs.avro_annotation = avro_annotation
     avrotocs.convert(avro_schema_path, cs_file_path)
```

### Comparing `avrotize-1.6.1/avrotize/avrotojava.py` & `avrotize-2.0.0/avrotize/avrotojava.py`

 * *Files 1% similar despite different names*

```diff
@@ -195,17 +195,25 @@
         self.output_dir = os.getcwd()
         self.avro_annotation = False
         self.jackson_annotations = False
         self.pascal_properties = False
         self.generated_types_avro_namespace: Dict[str,str] = {}
         self.generated_types_java_package: Dict[str,str] = {}
 
-    def concat_package(self, package: str, name: str) -> str:
+    def qualified_name(self, package: str, name: str) -> str:
         """Concatenates package and name using a dot separator"""
         return f"{package.lower()}.{name}" if package else name
+    
+    def join_packages(self, parent_package: str, package: str) -> str:
+        """Joins package and name using a dot separator"""
+        if parent_package and package:
+            return f"{parent_package}.{package}".lower()
+        elif parent_package:
+            return parent_package.lower()
+        return package.lower()
 
     class JavaType:
         """Java type definition"""
 
         def __init__(self, type_name: str, union_types: List['AvroToJava.JavaType'] | None = None, is_class: bool = False, is_enum: bool = False) -> None:
             self.type_name = type_name
             self.union_types = union_types
@@ -241,18 +249,18 @@
             'double': 'double',
             'bytes': 'byte[]',
             'string': 'String',
         }
         if '.' in avro_type:
             type_name = avro_type.split('.')[-1]
             package_name = '.'.join(avro_type.split('.')[:-1]).lower()
-            avro_type = self.concat_package(package_name, type_name)
+            avro_type = self.qualified_name(package_name, type_name)
         if avro_type in self.generated_types_avro_namespace:
             kind = self.generated_types_avro_namespace[avro_type]
-            qualified_class_name = self.concat_package(self.base_package, avro_type)
+            qualified_class_name = self.qualified_name(self.base_package, avro_type)
             return AvroToJava.JavaType(qualified_class_name, is_class=kind=="class", is_enum=kind=="enum")
         else:
             return AvroToJava.JavaType(required_mapping.get(avro_type, avro_type) if not is_optional else optional_mapping.get(avro_type, avro_type))
     
     def is_java_primitive(self, java_type: JavaType) -> bool:
         """Checks if a Java type is a primitive type"""
         return java_type.type_name in [
@@ -331,18 +339,19 @@
         """ Generates a Java class from an Avro record schema """
         class_definition = ''
         if 'doc' in avro_schema:
             class_definition += f"/** {avro_schema['doc']} */\n"
         namespace = avro_schema.get('namespace', parent_package)
         if not 'namespace' in avro_schema:
             avro_schema['namespace'] = namespace
-        package = self.concat_package(self.base_package, namespace).replace('.', '/').lower()
+        package = self.join_packages(self.base_package, namespace).replace('.', '/').lower()
+        package = package.replace('.', '/').lower()
         class_name = self.safe_identifier(avro_schema['name'])
-        namespace_qualified_name = self.concat_package(namespace,avro_schema['name'])
-        qualified_class_name = self.concat_package(package.replace('/', '.'), class_name)
+        namespace_qualified_name = self.qualified_name(namespace,avro_schema['name'])
+        qualified_class_name = self.qualified_name(package.replace('/', '.'), class_name)
         if namespace_qualified_name in self.generated_types_avro_namespace:
             return AvroToJava.JavaType(qualified_class_name, is_class=True)
         self.generated_types_avro_namespace[namespace_qualified_name] = "class"
         self.generated_types_java_package[qualified_class_name] = "class"
         fields_str = [self.generate_property(class_name, field, namespace) for field in avro_schema.get('fields', [])]
         class_body = "\n".join(fields_str)
         class_definition += f"public class {class_name}"
@@ -417,15 +426,15 @@
         class_definition += "\n}"
 
         if write_file:
             self.write_to_file(package, class_name, class_definition)
         return AvroToJava.JavaType(qualified_class_name, is_class=True)
     
     def create_is_json_match_method(self, avro_schema, parent_namespace, class_name) -> str:
-        """ Generates the isJsonMatch method for Jackson """
+        """ Generates the isJsonMatch method for a class using Jackson """
         predicates = ''
         class_definition = ''
         class_definition += f"\n\n{INDENT}/**\n{INDENT} * Checks if the JSON node matches the schema\n{INDENT}"
         class_definition += f"\n{INDENT}@param node The JSON node to check */"
         class_definition += f"\n{INDENT}public static boolean isJsonMatch(com.fasterxml.jackson.databind.JsonNode node)\n{INDENT}{{"
         field_defs = ''
         
@@ -655,18 +664,18 @@
 
     def generate_enum(self, avro_schema: Dict, parent_package: str, write_file: bool) -> JavaType:
         """ Generates a Java enum from an Avro enum schema """
         enum_definition = ''
         if 'doc' in avro_schema:
             enum_definition += f"/** {avro_schema['doc']} */\n"
             
-        package = self.concat_package(self.base_package, avro_schema.get('namespace', parent_package)).replace('.', '/').lower()       
+        package = self.join_packages(self.base_package, avro_schema.get('namespace', parent_package)).replace('.', '/').lower()       
         enum_name = self.safe_identifier(avro_schema['name'])
-        type_name = self.concat_package(package.replace('/', '.'), enum_name)
-        self.generated_types_avro_namespace[self.concat_package(avro_schema.get('namespace', parent_package),avro_schema['name'])] = "enum"
+        type_name = self.qualified_name(package.replace('/', '.'), enum_name)
+        self.generated_types_avro_namespace[self.qualified_name(avro_schema.get('namespace', parent_package),avro_schema['name'])] = "enum"
         self.generated_types_java_package[type_name] = "enum"       
         symbols = avro_schema.get('symbols', [])
         symbols_str = ', '.join(symbols)
         enum_definition += f"public enum {enum_name} {{\n"
         enum_definition += f"{INDENT}{symbols_str};\n"
         enum_definition += "}\n"
         if write_file:
@@ -676,15 +685,15 @@
     def generate_embedded_union_class_jackson(self, class_name: str, field_name: str, avro_type: List, parent_package: str, write_file: bool) -> str:
         """ Generates an embedded Union Class for Java using Jackson """
         class_definition_ctors = class_definition_decls = class_definition_read = class_definition_write = class_definition = ''
         class_definition_toobject = class_definition_fromobjectctor = class_definition_genericrecordctor = ''
         
         list_is_json_match: List[str] = []
         union_class_name = class_name + pascal(field_name) + 'Union'
-        package = self.concat_package(self.base_package, parent_package).replace('.', '/').lower()
+        package = self.join_packages(self.base_package, parent_package).replace('.', '/').lower()
         union_types: List[AvroToJava.JavaType] = [self.convert_avro_type_to_java(class_name, field_name + "Option" + str(i), t, parent_package) for i, t in enumerate(avro_type)]
         for i, union_type in enumerate(union_types):
             # we need the nullable version (wrapper) of all primitive types
             if self.is_java_primitive(union_type):
                 union_type = self.map_primitive_to_java(union_type.type_name, True)
             union_variable_name = union_type.type_name
             is_dict = is_list = False
@@ -964,14 +973,16 @@
 
     Converts Avro schema to C# classes
 
     Args:
         avro_schema_path (_type_): Avro input schema path  
         cs_file_path (_type_): Output C# file path 
     """
+    if not package_name:
+        package_name = os.path.splitext(os.path.basename(java_file_path))[0].replace('-', '_').lower()
     avrotojava = AvroToJava()
     avrotojava.base_package = package_name
     avrotojava.pascal_properties = pascal_properties
     avrotojava.avro_annotation = avro_annotation
     avrotojava.jackson_annotations = jackson_annotation
     avrotojava.convert(avro_schema_path, java_file_path)
```

### Comparing `avrotize-1.6.1/avrotize/avrotojs.py` & `avrotize-2.0.0/avrotize/avrotojs.py`

 * *Files identical despite different names*

### Comparing `avrotize-1.6.1/avrotize/avrotojsons.py` & `avrotize-2.0.0/avrotize/avrotojsons.py`

 * *Files identical despite different names*

### Comparing `avrotize-1.6.1/avrotize/avrotokusto.py` & `avrotize-2.0.0/avrotize/avrotokusto.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 class AvroToKusto:
     """Converts an Avro schema to a Kusto table schema."""
 
     def ___init___(self):
         """Initializes a new instance of the AvroToKusto class."""
         pass
 
-    def convert_record_to_kusto(self, schema: dict, emit_cloud_events_columns: bool, emit_cloudevents_dispatch_table: bool) -> List[str]:
+    def convert_record_to_kusto(self, schema: dict, emit_cloudevents_columns: bool, emit_cloudevents_dispatch_table: bool) -> List[str]:
         """Converts an Avro record schema to a Kusto table schema."""
         # Get the name and fields of the top-level record
         table_name = schema["name"]
         fields = schema["fields"]
 
         # Create a StringBuilder to store the kusto statements
         kusto = []
@@ -25,15 +25,15 @@
         # Append the create table statement with the column names and types
         kusto.append(f".create-merge table [{table_name}] (")
         columns = []
         for field in fields:
             column_name = field["name"]
             column_type = self.convert_avro_type_to_kusto_type(field["type"])
             columns.append(f"   [{column_name}]: {column_type}")
-        if emit_cloud_events_columns:
+        if emit_cloudevents_columns:
             columns.append("   [___type]: string")
             columns.append("   [___source]: string")
             columns.append("   [___id]: string")
             columns.append("   [___time]: datetime")
             columns.append("   [___subject]: string")
         kusto.append(",\n".join(columns))
         kusto.append(");")
@@ -55,15 +55,15 @@
                 doc_content = {
                     "description": field["doc"]
                 }
                 if isinstance(field["type"], list) or isinstance(field["type"], dict):
                     doc_content["type"] = field["type"]
                 doc = json.dumps(json.dumps(doc_content))
                 doc_string_statement.append(f"   [{column_name}]: {doc}")
-        if doc_string_statement and emit_cloud_events_columns:
+        if doc_string_statement and emit_cloudevents_columns:
             doc_string_statement.extend([
                 "   [___type] : 'Event type'",
                 "   [___source]: 'Context origin/source of the event'",
                 "   [___id]: 'Event identifier'",
                 "   [___time]: 'Event generation time'",
                 "   [___subject]: 'Context subject of the event'"
             ])
@@ -74,15 +74,15 @@
             kusto.append("")
 
         # add the JSON mapping for the table
         # .create-or-alter table dfl_data_events ingestion json mapping
         kusto.append(
             f".create-or-alter table [{table_name}] ingestion json mapping \"{table_name}_json_flat\"")
         kusto.append("```\n[")
-        if emit_cloud_events_columns:
+        if emit_cloudevents_columns:
             kusto.append("  {\"column\": \"___type\", \"path\": \"$.type\"},")
             kusto.append(
                 "  {\"column\": \"___source\", \"path\": \"$.source\"},")
             kusto.append("  {\"column\": \"___id\", \"path\": \"$.id\"},")
             kusto.append("  {\"column\": \"___time\", \"path\": \"$.time\"},")
             kusto.append(
                 "  {\"column\": \"___subject\", \"path\": \"$.subject\"},")
@@ -93,15 +93,15 @@
                     column_name = field['altnames']['kql']
                 if 'json' in field['altnames']:
                     json_name = field['altnames']['json']
             kusto.append(
                 f"  {{\"column\": \"{column_name}\", \"path\": \"$.{json_name}\"}},")
         kusto.append("]\n```\n\n")
 
-        if emit_cloud_events_columns:
+        if emit_cloudevents_columns:
             kusto.append(
                 f".create-or-alter table [{table_name}] ingestion json mapping \"{table_name}_json_ce_structured\"")
             kusto.append("```\n[")
             kusto.append("  {\"column\": \"___type\", \"path\": \"$.type\"},")
             kusto.append(
                 "  {\"column\": \"___source\", \"path\": \"$.source\"},")
             kusto.append("  {\"column\": \"___id\", \"path\": \"$.id\"},")
@@ -115,14 +115,22 @@
                         column_name = field['altnames']['kql']
                     if 'json' in field['altnames']:
                         json_name = field['altnames']['json']
                 kusto.append(
                     f"  {{\"column\": \"{column_name}\", \"path\": \"$.data.{json_name}\"}},")
             kusto.append("]\n```\n\n")
 
+        if emit_cloudevents_columns:
+            kusto.append(
+                f".create materialized-view with (backfill=true) {table_name}Latest on table {table_name} {{")
+            kusto.append(
+                f"    {table_name} | summarize arg_max(___time, *) by ___type, ___source, ___subject")
+            kusto.append("}")
+            kusto.append("")
+
         if emit_cloudevents_dispatch_table:
             event_type = schema["namespace"] + "." + \
                 schema["name"] if "namespace" in schema else schema["name"]
 
             query = f"_cloudevents_dispatch | where (specversion == '1.0' and type == '{event_type}') | " + \
                     "project"                        
             for field in fields:
@@ -141,22 +149,22 @@
             kusto.append("  \"IsEnabled\": true,")
             kusto.append("  \"Source\": \"_cloudevents_dispatch\",")
             kusto.append(
                 f"  \"Query\": \"{query}\",")
             kusto.append("  \"IsTransactional\": false,")
             kusto.append("  \"PropagateIngestionProperties\": true,")
             kusto.append("}]")
-            kusto.append("```")
+            kusto.append("```\n")
 
         return kusto
 
-    def convert_avro_to_kusto_script(self, avro_schema_path, avro_record_type, emit_cloud_events_columns=False, emit_cloudevents_dispatch_table=False) -> str:
+    def convert_avro_to_kusto_script(self, avro_schema_path, avro_record_type, emit_cloudevents_columns=False, emit_cloudevents_dispatch_table=False) -> str:
         """Converts an Avro schema to a Kusto table schema."""
         if emit_cloudevents_dispatch_table:
-            emit_cloud_events_columns = True
+            emit_cloudevents_columns = True
         schema_file = avro_schema_path
         if not schema_file:
             print("Please specify the avro schema file")
             sys.exit(1)
         with open(schema_file, "r", encoding="utf-8") as f:
             schema_json = f.read()
 
@@ -214,21 +222,21 @@
                 "  {\"column\": \"dataschema\", \"path\": \"$.dataschema\"},")
             kusto_script.append(
                 "  {\"column\": \"data\", \"path\": \"$.data\"}")
             kusto_script.append("]\n```\n\n")
 
         for record in schema:
             kusto_script.extend(self.convert_record_to_kusto(
-                record, emit_cloud_events_columns, emit_cloudevents_dispatch_table))
+                record, emit_cloudevents_columns, emit_cloudevents_dispatch_table))
         return "\n".join(kusto_script)
 
-    def convert_avro_to_kusto_file(self, avro_schema_path, avro_record_type, kusto_file_path, emit_cloud_events_columns=False, emit_cloudevents_dispatch_table=False):
+    def convert_avro_to_kusto_file(self, avro_schema_path, avro_record_type, kusto_file_path, emit_cloudevents_columns=False, emit_cloudevents_dispatch_table=False):
         """Converts an Avro schema to a Kusto table schema."""
         script = self.convert_avro_to_kusto_script(
-            avro_schema_path, avro_record_type, emit_cloud_events_columns, emit_cloudevents_dispatch_table)
+            avro_schema_path, avro_record_type, emit_cloudevents_columns, emit_cloudevents_dispatch_table)
         with open(kusto_file_path, "w", encoding="utf-8") as kusto_file:
             kusto_file.write(script)
 
     def convert_avro_type_to_kusto_type(self, avro_type: str | dict | list):
         """Converts an Avro type to a Kusto type."""
         if isinstance(avro_type, list):
             # If the type is an array, then it is a union type. Look whether it's a pair of a scalar type and null:
@@ -319,7 +327,16 @@
     for statement in script.split("\n\n"):
         if statement.strip():
             try:
                 client.execute_mgmt(kusto_database, statement)
             except Exception as e:
                 print(e)
                 sys.exit(1)
+
+def convert_avro_to_kusto(avro_schema_path, avro_record_type, kusto_file_path, kusto_uri, kusto_database, emit_cloudevents_columns=False, emit_cloudevents_dispatch_table=False, token_provider=None):
+    """Converts an Avro schema to a Kusto table schema."""
+    if not kusto_uri and not kusto_database:
+        convert_avro_to_kusto_file(
+            avro_schema_path, avro_record_type, kusto_file_path, emit_cloudevents_columns, emit_cloudevents_dispatch_table)
+    else:
+        convert_avro_to_kusto_db(
+            avro_schema_path, avro_record_type, kusto_uri, kusto_database, emit_cloudevents_columns, emit_cloudevents_dispatch_table, token_provider)
```

### Comparing `avrotize-1.6.1/avrotize/avrotoproto.py` & `avrotize-2.0.0/avrotize/avrotoproto.py`

 * *Files 0% similar despite different names*

```diff
@@ -21,14 +21,15 @@
 ProtoFiles = NamedTuple('ProtoFiles', [('files', List['ProtoFile'])])
 
 class AvroToProto:
     
     def __init__(self) -> None:
         self.naming_mode: Literal['snake', 'pascal', 'camel'] = 'pascal'
         self.allow_optional: bool = False
+        self.default_namespace: str = ''
 
     def avro_primitive_to_proto_type(self, avro_type: str, dependencies: List[str]) -> str:
         """Map Avro primitive types to Protobuf types."""
         mapping = {
             'null': 'google.protobuf.Empty',  # Special handling may be required
             'boolean': 'bool',
             'int': 'int32',
@@ -229,31 +230,33 @@
         elif isinstance(field_type, str):
             deps2: List[str] = []
             proto_type = self.avro_primitive_to_proto_type(field_type, deps2)
             return Field(comment, label, proto_type, '', '', field_name, index, deps2)
         raise ValueError(f"Unknown field type {field_type}")
 
     def avro_schema_to_proto_message(self, avro_schema: dict, proto_files: ProtoFiles) -> str:
+        """Convert an Avro schema to a Protobuf message definition."""
         comment = Comment('',{})
         if 'doc' in avro_schema:
             comment = Comment(avro_schema["doc"], {})
+        namespace = avro_schema.get("namespace", self.default_namespace)
         if avro_schema['type'] == 'record':
             message = self.convert_record_type(avro_schema, comment, proto_files)
-            file = next((f for f in proto_files.files if f.package == avro_schema["namespace"]), None)
+            file = next((f for f in proto_files.files if f.package == namespace), None)
             if not file:
-                file = ProtoFile({}, {}, {}, [], {}, avro_schema["namespace"])
+                file = ProtoFile({}, {}, {}, [], {}, namespace)
                 proto_files.files.append(file)
             file.messages[message.name] = message
         elif avro_schema['type'] == 'enum':
             enum_name = avro_schema['name']
             enum_symbols = {symbol: Field(comment, '', symbol, '', '', symbol, s, []) for s, symbol in enumerate(avro_schema['symbols'])}
             enum = Enum(comment, enum_name, enum_symbols)
-            file = next((f for f in proto_files.files if f.package == avro_schema["namespace"]), None)
+            file = next((f for f in proto_files.files if f.package == namespace), None)
             if not file:
-                file = ProtoFile({}, {}, {}, [], {}, avro_schema["namespace"])
+                file = ProtoFile({}, {}, {}, [], {}, namespace)
                 proto_files.files.append(file)
             file.enums[enum_name] = enum
         return avro_schema["name"]
         
     def avro_schema_to_proto_messages(self, avro_schema_input, proto_files: ProtoFiles):
         """Convert an Avro schema to Protobuf message definitions."""
         if not isinstance(avro_schema_input, list):
@@ -346,8 +349,9 @@
         self.avro_schema_to_proto_messages(avro_schema, proto_files)
         self.save_proto_to_file(proto_files, proto_file_path)
 
 def convert_avro_to_proto(avro_schema_path, proto_file_path, naming_mode: Literal['snake', 'pascal', 'camel'] = 'pascal', allow_optional: bool = False):
     avrotoproto = AvroToProto()
     avrotoproto.naming_mode = naming_mode
     avrotoproto.allow_optional = allow_optional
+    avrotoproto.default_namespace = os.path.splitext(os.path.basename(proto_file_path))[0]
     avrotoproto.convert_avro_to_proto(avro_schema_path, proto_file_path)
```

### Comparing `avrotize-1.6.1/avrotize/avrotoxsd.py` & `avrotize-2.0.0/avrotize/avrotoxsd.py`

 * *Files 1% similar despite different names*

```diff
@@ -306,15 +306,17 @@
         tree_str = tostring(schema, 'utf-8')
         pretty_tree = minidom.parseString(tree_str).toprettyxml(indent="  ")
         with open(xml_path, 'w') as xml_file:
             xml_file.write(pretty_tree)
 
     def convert_avro_to_xsd(self, avro_schema_path: str, xml_file_path: str) -> None:
         """Convert Avro schema file to XML schema file."""
-        with open(avro_schema_path, 'r') as avro_file:
+        with open(avro_schema_path, 'r', encoding='utf-8') as avro_file:
+           with open(avro_schema_path, 'r', encoding='utf-8') as avro_file:
             avro_schema = json.load(avro_file)
+            
         xml_schema = self.avro_schema_to_xsd(avro_schema)
         self.save_xsd_to_file(xml_schema, xml_file_path)
 
 def convert_avro_to_xsd(avro_schema_path: str, xml_file_path: str) -> None:
     avrotoxml = AvroToXSD()
     avrotoxml.convert_avro_to_xsd(avro_schema_path, xml_file_path)
```

### Comparing `avrotize-1.6.1/avrotize/common.py` & `avrotize-2.0.0/avrotize/common.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,13 +1,18 @@
 from collections import defaultdict
+import os
 import re
 from typing import Dict, Tuple, Union, Any, List
+import uuid
 from jsoncomparison import NO_DIFF, Compare
 import hashlib
 import json    
+import jinja2
+from jinja2.ext import Extension
+from jinja2 import Template, nodes
 
 def avro_name(name):
     """Convert a name into an Avro name."""
     if isinstance(name, int):
         name = '_'+str(name)
     val = re.sub(r'[^a-zA-Z0-9_]', '_', name)
     if re.match(r'^[0-9]', val):
@@ -343,8 +348,123 @@
     elif string[0].isupper():
         # PascalCase
         words = re.findall(r'[A-Z][a-z0-9_]*\.?', string)
     else:
         # camelCase
         words = re.findall(r'[a-z0-9]+\.?|[A-Z][a-z0-9_]*\.?', string)
     result = words[0].lower() + ''.join(word.capitalize() for word in words[1:])
-    return result
+    return result
+
+def snake(string):
+    """ Convert a string to snake_case """
+    if '::' in string:
+        strings = string.split('::')
+        return strings[0] + '::' + '::'.join(snake(s) for s in strings[1:])
+    if '.' in string:
+        strings = string.split('.')
+        return '.'.join(snake(s) for s in strings)
+    if not string or len(string) == 0:
+        return string
+    words = []
+    if '_' in string:
+        # snake_case
+        words = re.split(r'_', string)
+    elif string[0].isupper():
+        # PascalCase
+        words = re.findall(r'[A-Z][a-z0-9_]*\.?', string)
+    else:
+        # camelCase
+        words = re.findall(r'[a-z0-9]+\.?|[A-Z][a-z0-9_]*\.?', string)
+    result = '_'.join(word.lower() for word in words)
+    return result
+
+def fullname(avro_schema: dict):
+    name = avro_schema.get("name", "")
+    namespace = avro_schema.get("namespace", "")
+    return namespace + "." + name if namespace else name
+
+def altname(schema_obj: dict, purpose: str):
+    """
+    Retrieves the alternative name for a given purpose from the schema object.
+
+    Args:
+        schema_obj (dict): The schema object (record or field).
+        default_name (str): The default name.
+        purpose (str): The purpose for the alternative name (e.g., 'sql').
+
+    Returns:
+        str: The alternative name if present, otherwise the default name.
+    """
+    if "altnames" in schema_obj and purpose in schema_obj["altnames"]:
+        return schema_obj["altnames"][purpose]
+    return schema_obj["name"]
+
+def process_template(file_path: str, **kvargs) -> str:
+    """
+    Process a file as a Jinja2 template with the given object as input.
+
+    Args:
+        file_path (str): The path to the file.
+        obj (Any): The object to use as input for the template.
+
+    Returns:
+        str: The processed template as a string.
+    """
+    # Load the template environment
+    file_dir = os.path.dirname(__file__)
+    template_loader = jinja2.FileSystemLoader(searchpath=file_dir)
+    template_env = jinja2.Environment(loader=template_loader)
+    template_env.filters['pascal'] = pascal
+    template_env.filters['camel'] = camel
+
+    # Load the template from the file
+    template = template_env.get_template(file_path)
+
+    # Render the template with the object as input
+    output = template.render(**kvargs)
+
+    return output
+
+def render_template(template: str, output: str, **kvargs):
+    """ Render a template and write it to a file """
+    out = process_template(template, **kvargs)
+    # make sure the directory exists
+    os.makedirs(os.path.dirname(output), exist_ok=True)
+    with open(output, 'w', encoding='utf-8') as f:
+        f.write(out)
+        
+        
+def get_longest_namespace_prefix(schema):
+    """ Get the longest common prefix for the namespace of all types in the schema. """
+    namespaces = set(collect_namespaces(schema))
+    longest_common_prefix = ''
+    # find longest common prefix of the namespaces (not with os.path!!!)
+    for ns in namespaces:
+        if not longest_common_prefix:
+            longest_common_prefix = ns
+        else:
+            for i in range(min(len(longest_common_prefix), len(ns))):
+                if longest_common_prefix[i] != ns[i]:
+                    longest_common_prefix = longest_common_prefix[:i]
+                    break
+    return longest_common_prefix.strip('.')
+
+def collect_namespaces(schema: Any, parent_namespace: str = '') -> List[str]:
+    """ Performs a deep search of the schema to collect all namespaces """
+    namespaces = []
+    if isinstance(schema, dict):
+        namespace = str(schema.get('namespace', parent_namespace))
+        if namespace:
+            namespaces.append(namespace)
+        if 'fields' in schema and isinstance(schema['fields'], list):
+            for field in schema['fields']:
+                if isinstance(field, dict) and 'type' in field and isinstance(field['type'], dict):
+                    namespaces.extend(collect_namespaces(field['type'], namespace))
+                namespaces.extend(collect_namespaces(field, namespace))
+        if 'items' in schema and isinstance(schema['items'], dict):
+            namespaces.extend(collect_namespaces(schema['items'], namespace))
+        if 'values' in schema and isinstance(schema['values'], dict):
+            namespaces.extend(collect_namespaces(schema['values'], namespace))
+    elif isinstance(schema, list):
+        for item in schema:
+            namespaces.extend(collect_namespaces(item, parent_namespace))
+    return namespaces
```

### Comparing `avrotize-1.6.1/avrotize/dependency_resolver.py` & `avrotize-2.0.0/avrotize/dependency_resolver.py`

 * *Files identical despite different names*

### Comparing `avrotize-1.6.1/avrotize/generic/generic.avsc` & `avrotize-2.0.0/avrotize/generic/generic.avsc`

 * *Files identical despite different names*

### Comparing `avrotize-1.6.1/avrotize/jsonstoavro.py` & `avrotize-2.0.0/avrotize/jsonstoavro.py`

 * *Files identical despite different names*

### Comparing `avrotize-1.6.1/avrotize/kconnect.json` & `avrotize-2.0.0/avrotize/kconnect.json`

 * *Files identical despite different names*

### Comparing `avrotize-1.6.1/avrotize/kstructtoavro.py` & `avrotize-2.0.0/avrotize/kstructtoavro.py`

 * *Files identical despite different names*

### Comparing `avrotize-1.6.1/avrotize/kustotoavro.py` & `avrotize-2.0.0/avrotize/kustotoavro.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,23 +10,24 @@
 
 JsonNode = Dict[str, 'JsonNode'] | List['JsonNode'] | str | bool | int | None
 
 
 class KustoToAvro:
     """ Converts Kusto table schemas to Avro schema format."""
 
-    def __init__(self, kusto_uri, kusto_database, avro_namespace: str, avro_schema_path, emit_cloudevents_xregistry: bool, token_provider=None):
+    def __init__(self, kusto_uri, kusto_database, avro_namespace: str, avro_schema_path, emit_cloudevents: bool, emit_cloudevents_xregistry: bool, token_provider=None):
         """ Initializes the KustoToAvro class with the Kusto URI and database name. """
         kcsb = KustoConnectionStringBuilder.with_az_cli_authentication(kusto_uri) if not token_provider else KustoConnectionStringBuilder.with_token_provider(kusto_uri, token_provider)
         self.client = KustoClient(kcsb)
         self.kusto_database = kusto_database
         self.avro_namespace = avro_namespace
         self.avro_schema_path = avro_schema_path
-        self.emit_cloudevents_xregistry = emit_cloudevents_xregistry
-        if self.emit_cloudevents_xregistry:
+        self.emit_xregistry = emit_cloudevents_xregistry
+        self.emit_cloudevents = emit_cloudevents or emit_cloudevents_xregistry
+        if self.emit_xregistry:
             if not self.avro_namespace:
                 raise ValueError(
                     "The avro_namespace must be specified when emit_cloudevents_xregistry is True")
         self.generated_types: List[str] = []
 
     def fetch_table_schema_and_docs(self, table_name: str):
         """ Fetches the schema and docstrings for a given table."""
@@ -203,15 +204,15 @@
     def kusto_to_avro_schema(self, kusto_schema: dict, table_name: str) -> JsonNode:
         """ Converts a Kusto schema to Avro schema."""
         column_names = set([column['Name'].lstrip('_')
                            for column in kusto_schema['OrderedColumns']])
         type_values: List[str|None] = []
         type_column: Dict[str, JsonNode] = {}
         is_cloudevent = False
-        if self.emit_cloudevents_xregistry:
+        if self.emit_cloudevents:
             is_cloudevent = 'type' in column_names and 'source' in column_names and 'data' in column_names and 'id' in column_names
             if is_cloudevent:
                 type_column = next(
                     (column for column in kusto_schema['OrderedColumns'] if column['Name'].lstrip('_') == 'type'), {})
                 type_sampling_query = f"{table_name} | distinct {type_column['Name']}"
                 type_sampling_rows = self.client.execute(
                     self.kusto_database, type_sampling_query)
@@ -240,19 +241,20 @@
                         column['CslType'], table_name, column['Name'], type_column, type_value)           
                 if isinstance(data_schemas, dict):
                     data_schemas = [data_schemas]
                 if isinstance(data_schemas, list):
                     for schema in data_schemas:
                         if not isinstance(schema, dict) or "type" not in schema or schema["type"] != "record":
                             schema = self.wrap_schema_in_root_record(schema, type_name_name, type_namespace)
-                        ce_attribs: Dict[str, JsonNode] ={}
-                        for col in [col for col in kusto_schema['OrderedColumns'] if col['Name'].lstrip('_') != 'data']:
-                            ce_attribs[col['Name'].lstrip('_')] = "string"
-                        if isinstance(schema, dict):
-                            schema["ce_attribs"] = ce_attribs
+                        if self.emit_xregistry:
+                            ce_attribs: Dict[str, JsonNode] ={}
+                            for col in [col for col in kusto_schema['OrderedColumns'] if col['Name'].lstrip('_') != 'data']:
+                                ce_attribs[col['Name'].lstrip('_')] = "string"
+                            if isinstance(schema, dict):
+                                schema["ce_attribs"] = ce_attribs
                         self.apply_schema_attributes(schema, kusto_schema, table_name, type_value, type_namespace)
                         schemas.append(schema)
             else:
                 for column in kusto_schema['OrderedColumns']:
                     avro_type = self.map_kusto_type_to_avro_type(
                         column['CslType'], table_name, column['Name'], type_column, type_value)
                     field: Dict[str, JsonNode] = {"name": column['Name'], "type": avro_type}
@@ -290,15 +292,15 @@
     
     def apply_schema_attributes(self, schema, kusto_schema, table_name, type_value, type_namespace):
         """ Applies schema attributes to the schema."""
         if isinstance(schema, dict):
             schema["altnames"] = {
                     "kql": table_name
                 }
-            if self.emit_cloudevents_xregistry and type_value:
+            if self.emit_cloudevents and type_value:
                 schema["ce_type"] = type_value
             if type_namespace:
                 schema["namespace"] = type_namespace
             doc = kusto_schema.get('DocString', '')
             if doc:
                 schema["doc"] = doc
 
@@ -352,15 +354,15 @@
                     kusto_schema, table_name)
                 if isinstance(avro_schema, list):
                     union_schema.extend(avro_schema)
                 else:
                     union_schema.append(avro_schema)
 
         output = None
-        if self.emit_cloudevents_xregistry:
+        if self.emit_xregistry:
             xregistry_messages = {}
             xregistry_schemas = {}
             groupname = self.avro_namespace
             for schema in union_schema:
                 self.generated_types = []
                 self.make_type_names_unique([schema])
                 ce_attribs: Dict[str, JsonNode] = {}
@@ -385,15 +387,18 @@
                 xregistry_messages[schemaid] = {
                     "id": schemaid,
                     "name": schema_name,
                     "format": "CloudEvents/1.0",
                     "metadata": {
                         "type": {
                             "value": schemaid
-                        }
+                        },
+                        "source": {
+                            "value": "{source}"
+                        },
                     },
                     "schemaformat": f"Avro/{AVRO_VERSION}",
                     "schemaurl": f"#/schemagroups/{groupname}/schemas/{schemaid}"
                 }
                 for key, value in ce_attribs.items():
                     # skip the required attributes
                     if key == "type" or key == "source" or key == "id" or key == "specversion":
@@ -425,12 +430,12 @@
         base_dir = os.path.dirname(self.avro_schema_path)
         if base_dir and not os.path.exists(base_dir):
             os.makedirs(base_dir)
         with open(self.avro_schema_path, 'w', encoding='utf-8') as avro_file:
             json.dump(output, avro_file, indent=4)
 
 
-def convert_kusto_to_avro(kusto_uri: str, kusto_database: str, avro_namespace: str, avro_schema_file: str, emit_cloudevents_xregistry: bool, token_provider=None):
+def convert_kusto_to_avro(kusto_uri: str, kusto_database: str, avro_namespace: str, avro_schema_file: str, emit_cloudevents:bool, emit_cloudevents_xregistry: bool, token_provider=None):
     """ Converts Kusto table schemas to Avro schema format."""
     kusto_to_avro = KustoToAvro(
-        kusto_uri, kusto_database, avro_namespace, avro_schema_file, emit_cloudevents_xregistry, token_provider=token_provider)
+        kusto_uri, kusto_database, avro_namespace, avro_schema_file,emit_cloudevents, emit_cloudevents_xregistry, token_provider=token_provider)
     return kusto_to_avro.process_all_tables()
```

### Comparing `avrotize-1.6.1/avrotize/proto2parser.py` & `avrotize-2.0.0/avrotize/proto2parser.py`

 * *Files identical despite different names*

### Comparing `avrotize-1.6.1/avrotize/proto3parser.py` & `avrotize-2.0.0/avrotize/proto3parser.py`

 * *Files identical despite different names*

### Comparing `avrotize-1.6.1/avrotize/prototoavro.py` & `avrotize-2.0.0/avrotize/prototoavro.py`

 * *Files identical despite different names*

### Comparing `avrotize-1.6.1/avrotize/prototypes/any.avsc` & `avrotize-2.0.0/avrotize/prototypes/any.avsc`

 * *Files identical despite different names*

### Comparing `avrotize-1.6.1/avrotize/prototypes/api.avsc` & `avrotize-2.0.0/avrotize/prototypes/api.avsc`

 * *Files identical despite different names*

### Comparing `avrotize-1.6.1/avrotize/prototypes/duration.avsc` & `avrotize-2.0.0/avrotize/prototypes/duration.avsc`

 * *Files identical despite different names*

### Comparing `avrotize-1.6.1/avrotize/prototypes/field_mask.avsc` & `avrotize-2.0.0/avrotize/prototypes/field_mask.avsc`

 * *Files identical despite different names*

### Comparing `avrotize-1.6.1/avrotize/prototypes/struct.avsc` & `avrotize-2.0.0/avrotize/prototypes/struct.avsc`

 * *Files identical despite different names*

### Comparing `avrotize-1.6.1/avrotize/prototypes/timestamp.avsc` & `avrotize-2.0.0/avrotize/prototypes/timestamp.avsc`

 * *Files identical despite different names*

### Comparing `avrotize-1.6.1/avrotize/prototypes/type.avsc` & `avrotize-2.0.0/avrotize/prototypes/type.avsc`

 * *Files identical despite different names*

### Comparing `avrotize-1.6.1/avrotize/prototypes/wrappers.avsc` & `avrotize-2.0.0/avrotize/prototypes/wrappers.avsc`

 * *Files identical despite different names*

### Comparing `avrotize-1.6.1/avrotize/xsdtoavro.py` & `avrotize-2.0.0/avrotize/xsdtoavro.py`

 * *Files identical despite different names*

### Comparing `avrotize-1.6.1/pyproject.toml` & `avrotize-2.0.0/pyproject.toml`

 * *Files 21% similar despite different names*

```diff
@@ -22,26 +22,38 @@
     "pyarrow>=15.0.0",
     "asn1tools>=0.166.0",
     "jsonpointer>=2.4",
     "jsonpath-ng>=1.6.1",
     "jsoncomparison>=1.1.0",
     "requests>=2.31.0",
     "azure-kusto-data>=4.4.1",
+    "azure-identity>=1.6.0",
+    "datapackage>=1.15.4",
+    "jinja2>=3.1.4",
+    "pyiceberg>=0.6.1",
 ]
-dev-dependencies = [
+[project.optional-dependencies]
+dev = [
     "pytest>=7.2.1",
     "fastavro>=1.9.4",
     "xmlschema>=3.0.2",
     "xmlunittest>=0.5.0",
     "pylint>=3.1.0",
     "dataclasses_json>0.6.4",
     "dataclasses>=0.6",
     "pydantic>=2.7.1",
     "avro>=1.11.3",
     "testcontainers>=4.4.1",
+    "pymysql>=1.1.0",
+    "psycopg2>=2.9.9",
+    "pyodbc>=5.1.0",
+    "pymongo>=4.7.2",
+    "oracledb>=2.2.1",
+    "cassandra-driver>=3.29.1",
+    "sqlalchemy>=2.0.15"
 ]
 
 [project.scripts]
 avrotize = "avrotize.avrotize:main"
 
 [tool.setuptools_scm]
 write_to = "avrotize/_version.py"
```

### Comparing `avrotize-1.6.1/PKG-INFO` & `avrotize-2.0.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: avrotize
-Version: 1.6.1
+Version: 2.0.0
 Summary: Tools to convert from and to Avro Schema from various other schema languages.
 Author-email: Clemens Vasters <clemensv@microsoft.com>
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -13,30 +13,77 @@
 Requires-Dist: pyarrow>=15.0.0
 Requires-Dist: asn1tools>=0.166.0
 Requires-Dist: jsonpointer>=2.4
 Requires-Dist: jsonpath-ng>=1.6.1
 Requires-Dist: jsoncomparison>=1.1.0
 Requires-Dist: requests>=2.31.0
 Requires-Dist: azure-kusto-data>=4.4.1
+Requires-Dist: azure-identity>=1.6.0
+Requires-Dist: datapackage>=1.15.4
+Requires-Dist: jinja2>=3.1.4
+Requires-Dist: pyiceberg>=0.6.1
+Requires-Dist: pytest>=7.2.1 ; extra == "dev"
+Requires-Dist: fastavro>=1.9.4 ; extra == "dev"
+Requires-Dist: xmlschema>=3.0.2 ; extra == "dev"
+Requires-Dist: xmlunittest>=0.5.0 ; extra == "dev"
+Requires-Dist: pylint>=3.1.0 ; extra == "dev"
+Requires-Dist: dataclasses_json>0.6.4 ; extra == "dev"
+Requires-Dist: dataclasses>=0.6 ; extra == "dev"
+Requires-Dist: pydantic>=2.7.1 ; extra == "dev"
+Requires-Dist: avro>=1.11.3 ; extra == "dev"
+Requires-Dist: testcontainers>=4.4.1 ; extra == "dev"
+Requires-Dist: pymysql>=1.1.0 ; extra == "dev"
+Requires-Dist: psycopg2>=2.9.9 ; extra == "dev"
+Requires-Dist: pyodbc>=5.1.0 ; extra == "dev"
+Requires-Dist: pymongo>=4.7.2 ; extra == "dev"
+Requires-Dist: oracledb>=2.2.1 ; extra == "dev"
+Requires-Dist: cassandra-driver>=3.29.1 ; extra == "dev"
+Requires-Dist: sqlalchemy>=2.0.15 ; extra == "dev"
+Provides-Extra: dev
 
 # Avrotize
 
-Avrotize is a command-line tool for converting data structure definitions between
-different schema formats, using [Apache Avro](https://avro.apache.org/) Schema
-as the integration schema model.
-
-You can use the tool to convert between Avro Schema and other schema formats
-like JSON Schema, XML Schema (XSD), Protocol Buffers (Protobuf), ASN.1, and
-database schema formats like Kusto Data Table Definition (KQL) and T-SQL Table
-Definition (SQL). That means you can also convert from JSON Schema to Protobuf
-going via Avro Schema. 
-
-You can also generate C#, Java, TypeScript, JavaScript, and Python code from the
-Avro Schema documents with Avrotize. The difference to the native Avro tools is
-that Avrotize can emit data classes without Avro library dependencies and,
+Avrotize is a ["Rosetta Stone"](https://en.wikipedia.org/wiki/Rosetta_Stone) for
+data structure definitions, allowing you to convert between numerous data and
+database schema formats and to generate code for different programming
+languages.
+
+It is, for instance, a well-documented and predictable converter and code
+generator for data structures originally defined in JSON Schema (of arbitrary
+complexity).
+
+The tool leans on the Apache Avro-derived [Avrotize
+Schema](specs/avrotize-schema.md) as its schema model.
+
+- Programming languages: Python, C#, Java, TypeScript, JavaScript, Rust, Go, C++
+- SQL Databases: MySQL, MariaDB, PostgreSQL, SQL Server, Oracle, SQLite, BigQuery, Snowflake, Redshift, DB2
+- Other databases: KQL/Kusto, MongoDB, Cassandra, Redis, Elasticsearch, DynamoDB, CosmosDB
+- Data schema formats: Avro, JSON Schema, XML Schema (XSD), Protocol Buffers 2
+  and 3, ASN.1, Apache Parquet
+
+## Installation
+
+You can install Avrotize from PyPI, [having installed Python 3.11 or
+later](https://www.python.org/downloads/):
+
+```bash
+pip install avrotize
+```
+
+## Overview
+
+You can use Avrotize to convert between Avro/Avrotize Schema and other schema
+formats like JSON Schema, XML Schema (XSD), Protocol Buffers (Protobuf), ASN.1,
+and database schema formats like Kusto Data Table Definition (KQL) and T-SQL
+Table Definition (SQL). That means you can also convert from JSON Schema to
+Protobuf going via Avrotize Schema.
+
+You can also generate C#, Java, TypeScript, JavaScript, and Python code from
+Avrotize Schema documents. The difference to the native Avro tools is that
+Avrotize can emit data classes without Avro library dependencies and,
 optionally, with annotations for JSON serialization libraries like Jackson or
 System.Text.Json.
 
 The tool does not convert data (instances of schemas), only the data structure
 definitions.
 
 Mind that the primary objective of the tool is the conversion of schemas that
@@ -67,18 +114,24 @@
 and to common programming language types.
 
 Therefore, Avrotize intentionally ignores common techniques to model
 object-oriented inheritance. For instance, when converting from JSON Schema, all
 content from `allOf` expressions is merged into a single record type rather than
 trying to model the inheritance tree in Avro.
 
-## Why Avro Schema?
+## Avrotize Schema
+
+Avrotize Schema is a schema model that is a full superset of the popular Apache
+Avrotize Schema model. Avrotize Schema is the "pivot point" for this tool. All
+schemas are converted from and to Avrotize Schema.
+
+Since Avrotize Schema is a superset of Avrotize Schema and uses its extensibility
+features, every Avrotize Schema is also a valid Avrotize Schema and vice versa.
 
-Apache Avro Schema is the "pivot point" for this tool. All schemas are converted
-from and to Avro Schema.
+Why did we pick Avro Schema as the foundational schema model?
 
 Avro Schema ...
 
 - provides a simple, clean, and concise way to define data structures. It is
   quite easy to understand and use.
 - is self-contained by design without having or requiring external references.
   Avro Schema can express complex data structure hierarchies spanning multiple
@@ -97,18 +150,16 @@
 - is itself expressed as JSON. That makes it easy to parse and generate, which
   is not the case for Protobuf or ASN.1, which require bespoke parsers.
 
 > It needs to be noted here that while Avro Schema is great for defining data
 > structures, and data classes generated from Avro Schema using this tool or
 > other tools can be used to with the most popular JSON serialization libraries,
 > the Apache Avro project's own JSON encoding has fairly grave interoperability
-> issues with common usage of JSON. A alternate Avro JSON encoding that is more
-> interoperable is proposed in [`avrojson.md`](avrojson.md) for submission to
-> the Apache Avro project; the document also enumerates the specific
-> interoperability issues.
+> issues with common usage of JSON. Avrotize defines an alternate JSON encoding
+> in [`avrojson.md`](avrojson.md).
 
 Avro Schema does not support all the bells and whistles of XML Schema or JSON
 Schema, but that is a feature, not a bug, as it ensures the portability of the
 schemas across different systems and infrastructures. Specifically, Avro Schema
 does not support many of the data validation features found in JSON Schema or
 XML Schema. There are no `pattern`, `format`, `minimum`, `maximum`, or `required`
 keywords in Avro Schema, and Avro does not support conditional validation.
@@ -116,167 +167,161 @@
 In a system where data originates as XML or JSON described by a validating XML
 Schema or JSON Schema, the assumption we make here is that data will be
 validated using its native schema language first, and then the Avro Schema will
 be used for transformation or transfer or storage.
 
 ## Adding CloudEvents columns for database tables
 
-When converting Avro Schema to Kusto Data Table Definition (KQL), T-SQL Table
+When converting Avrotize Schema to Kusto Data Table Definition (KQL), T-SQL Table
 Definition (SQL), or Parquet Schema, the tool can add special columns for
 [CloudEvents](https://cloudevents.io) attributes. CNCF CloudEvents is a
 specification for describing event data in a common way.
 
 The rationale for adding such columns to database tables is that messages and
 events commonly separate event metadata from the payload data, while that
 information is merged when events are projected into a database. The metadata
 often carries important context information about the event that is not
 contained in the payload itself. Therefore, the tool can add those columns to
 the database tables for easy alignment of the message context with the payload
 when building event stores.
 
-## Installation
-
-You can install Avrotize from PyPI, [having installed Python 3.11 or later](https://www.python.org/downloads/):
-
-```bash
-pip install avrotize
-```
 
 ## Usage
 
-Avrotize provides several commands for converting schema formats via Avro Schema.
+Avrotize provides several commands for converting schema formats via Avrotize Schema.
 
-Converting to Avro Schema:
+Converting to Avrotize Schema:
 
-- [`avrotize p2a`´](#convert-proto-schema-to-avro-schema) - Convert Protobuf (2 or 3) schema to Avro schema.
-- [`avrotize j2a`](#convert-json-schema-to-avro-schema) - Convert JSON schema to Avro schema.
-- [`avrotize x2a`](#convert-xml-schema-xsd-to-avro-schema) - Convert XML schema to Avro schema.
-- [`avrotize asn2a`](#convert-asn1-schema-to-avro-schema) - Convert ASN.1 to Avro schema.
-- [`avrotize k2a`](#convert-kusto-table-definition-to-avro-schema) - Convert Kusto table definitions to Avro schema.
-
-Converting from Avro Schema:
-
-- [`avrotize a2p`](#convert-avro-schema-to-proto-schema) - Convert Avro schema to Protobuf 3 schema.
-- [`avrotize a2j`](#convert-avro-schema-to-json-schema) - Convert Avro schema to JSON schema.
-- [`avrotize a2x`](#convert-avro-schema-to-xml-schema) - Convert Avro schema to XML schema.
-- [`avrotize a2k`](#convert-avro-schema-to-kusto-table-declaration) - Convert Avro schema to Kusto table definition.
-- [`avrotize a2tsql`](#convert-avro-schema-to-t-sql-table-definition) - Convert Avro schema to T-SQL table definition.
-- [`avrotize a2pq`](#convert-avro-schema-to-empty-parquet-file) - Convert Avro schema to empty Parquet file.
-
-Generate code from Avro Schema:
-
-- [`avrotize a2csharp`](#generate-c-code-from-avro-schema) - Generate C# code from Avro schema.
-- [`avrotize a2java`](#generate-java-code-from-avro-schema) - Generate Java code from Avro schema.
-- [`avrotize a2py`](#generate-python-code-from-avro-schema) - Generate Python code from Avro schema.
-- [`avrotize a2ts`](#generate-typescript-code-from-avro-schema) - Generate TypeScript code from Avro schema.
-- [`avrotize a2js`](#generate-javascript-code-from-avro-schema) - Generate JavaScript code from Avro schema.
+- [`avrotize p2a`´](#convert-proto-schema-to-avrotize-schema) - Convert Protobuf (2 or 3) schema to Avrotize Schema.
+- [`avrotize j2a`](#convert-json-schema-to-avrotize-schema) - Convert JSON schema to Avrotize Schema.
+- [`avrotize x2a`](#convert-xml-schema-xsd-to-avrotize-schema) - Convert XML schema to Avrotize Schema.
+- [`avrotize asn2a`](#convert-asn1-schema-to-avrotize-schema) - Convert ASN.1 to Avrotize Schema.
+- [`avrotize k2a`](#convert-kusto-table-definition-to-avrotize-schema) - Convert Kusto table definitions to Avrotize Schema.
+- [`avrotize pq2a`](#convert-parquet-schema-to-avrotize-schema) - Convert Parquet schema to Avrotize Schema.
+
+Converting from Avrotize Schema:
+
+- [`avrotize a2p`](#convert-avro-schema-to-proto-schema) - Convert Avrotize Schema to Protobuf 3 schema.
+- [`avrotize a2j`](#convert-avro-schema-to-json-schema) - Convert Avrotize Schema to JSON schema.
+- [`avrotize a2x`](#convert-avro-schema-to-xml-schema) - Convert Avrotize Schema to XML schema.
+- [`avrotize a2k`](#convert-avro-schema-to-kusto-table-declaration) - Convert Avrotize Schema to Kusto table definition.
+- [`avrotize a2tsql`](#convert-avro-schema-to-t-sql-table-definition) - Convert Avrotize Schema to T-SQL table definition.
+- [`avrotize a2pq`](#convert-avro-schema-to-empty-parquet-file) - Convert Avrotize Schema to empty Parquet file.
+
+Generate code from Avrotize Schema:
+
+- [`avrotize a2csharp`](#generate-c-code-from-avro-schema) - Generate C# code from Avrotize Schema.
+- [`avrotize a2java`](#generate-java-code-from-avro-schema) - Generate Java code from Avrotize Schema.
+- [`avrotize a2py`](#generate-python-code-from-avro-schema) - Generate Python code from Avrotize Schema.
+- [`avrotize a2ts`](#generate-typescript-code-from-avro-schema) - Generate TypeScript code from Avrotize Schema.
+- [`avrotize a2js`](#generate-javascript-code-from-avro-schema) - Generate JavaScript code from Avrotize Schema.
 
-### Convert Proto schema to Avro schema
+### Convert Proto schema to Avrotize Schema
 
 ```bash
 avrotize p2a --proto <path_to_proto_file> --avsc <path_to_avro_schema_file>
 ```
 
 Parameters:
 
 - `--proto`: The path to the Protobuf schema file to be converted.
-- `--avsc`: The path to the Avro schema file to write the conversion result to.
+- `--avsc`: The path to the Avrotize Schema file to write the conversion result to.
 
 Conversion notes:
 
 - Proto 2 and Proto 3 syntax are supported.
 - Proto package names are mapped to Avro namespaces. The tool does resolve imports
-  and consolidates all imported types into a single Avro schema file.
+  and consolidates all imported types into a single Avrotize Schema file.
 - The tool embeds all 'well-known' Protobuf 3.0 types in Avro format and injects
   them as needed when the respective types are imported. Only the `Timestamp` type is
   mapped to the Avro logical type 'timestamp-millis'. The rest of the well-known
   Protobuf types are kept as Avro record types with the same field names and types.
 - Protobuf allows any scalar type as key in a `map`, Avro does not. When converting
   from Proto to Avro, the type information for the map keys is ignored.
 - The field numbers in message types are not mapped to the positions of the
   fields in Avro records. The fields in Avro are ordered as they appear in the
-  Proto schema. Consequently, the Avro schema also ignores the `extensions` and
+  Proto schema. Consequently, the Avrotize Schema also ignores the `extensions` and
   `reserved` keywords in the Proto schema.
 - The `optional` keyword results in an Avro field being nullable (union with the
   `null` type), while the `required` keyword results in a non-nullable field.
   The `repeated` keyword results in an Avro field being an array of the field
   type.
 - The `oneof` keyword in Proto is mapped to an Avro union type. 
 - All `options` in the Proto schema are ignored.
 
 
-### Convert Avro schema to Proto schema
+### Convert Avrotize Schema to Proto schema
 
 ```bash
 avrotize a2p --avsc <path_to_avro_schema_file> --proto <path_to_proto_directory>
 ```
 
 Parameters:
 
-- `--avsc`: The path to the Avro schema file to be converted.
+- `--avsc`: The path to the Avrotize Schema file to be converted.
 - `--proto`: The path to the Protobuf schema directory to write the conversion result to.
 
 Conversion notes:
 
 - Avro namespaces are resolved into distinct proto package definitions. The tool will
   create a new `.proto` file with the package definition and an `import` statement for
-  each namespace found in the Avro schema.
+  each namespace found in the Avrotize Schema.
 - Avro type unions `[]` are converted to `oneof` expressions in Proto. Avro allows for
   maps and arrays in the type union, whereas Proto only supports scalar types and
   message type references. The tool will therefore emit message types containing
   a single array or map field for any such case and add it to the containing type,
   and will also recursively resolve further unions in the array and map values.
 - The sequence of fields in a message follows the sequence of fields in the Avro
   record. When type unions need to be resolved into `oneof` expressions, the alternative
   fields need to be assigned field numbers, which will shift the field numbers for any
   subsequent fields.
 
-### Convert JSON schema to Avro schema
+### Convert JSON schema to Avrotize Schema
 
 ```bash
 avrotize j2a --jsons <path_to_json_schema_file> --avsc <path_to_avro_schema_file> [--namespace <avro_schema_namespace>]
 ```
 
 Parameters:
 
 - `--jsons`: The path to the JSON schema file to be converted.
-- `--avsc`: The path to the Avro schema file to write the conversion result to.
-- `--namespace`: (optional) The namespace to use in the Avro schema if the JSON
+- `--avsc`: The path to the Avrotize Schema file to write the conversion result to.
+- `--namespace`: (optional) The namespace to use in the Avrotize Schema if the JSON
   schema does not define a namespace.
 
 Conversion notes:
 
 - [JSON Schema Handling in Avrotize](jsonschema.md)
 
-### Convert Avro schema to JSON schema
+### Convert Avrotize Schema to JSON schema
 
 ```bash
 avrotize a2j --avsc <path_to_avro_schema_file> --json <path_to_json_schema_file>
 ```
 
 Parameters:
 
-- `--avsc`: The path to the Avro schema file to be converted.
+- `--avsc`: The path to the Avrotize Schema file to be converted.
 - `--json`: The path to the JSON schema file to write the conversion result to.
 
 Conversion notes:
 
 - [JSON Schema Handling in Avrotize](jsonschema.md)
 
-### Convert XML Schema (XSD) to Avro schema
+### Convert XML Schema (XSD) to Avrotize Schema
 
 ```bash
 avrotize x2a --xsd <path_to_xsd_file> --avsc <path_to_avro_schema_file> [--namespace <avro_schema_namespace>]
 ```
 
 Parameters:
 
 - `--xsd`: The path to the XML schema file to be converted.
-- `--avsc`: The path to the Avro schema file to write the conversion result to.
-- `--namespace`: (optional) The namespace to use in the Avro schema if the XML
+- `--avsc`: The path to the Avrotize Schema file to write the conversion result to.
+- `--namespace`: (optional) The namespace to use in the Avrotize Schema if the XML
   schema does not define a namespace.
 
 Conversion notes:
 
 - All XML Schema constructs are mapped to Avro record types with fields, whereby
   **both**, elements and attributes, become fields in the record. XML is therefore
   flattened into fields and this aspect of the structure is not preserved.
@@ -289,51 +334,51 @@
   Avro type.
 - `complexType` declarations that have simple content where a base type is augmented
   with attributes is mapped to a record type in Avro. Any other facets defined on
   the complex type are ignored.
 - If the schema defines a single root element, the tool will emit a single Avro
   record type. If the schema defines multiple root elements, the tool will emit a
   union of record types, each corresponding to a root element.
-- All fields in the resulting Avro Schema are annotated with an `xmlkind`
+- All fields in the resulting Avrotize Schema are annotated with an `xmlkind`
   extension attribute that indicates whether the field was an `element` or an
   `attribute` in the XML schema.
 
-## Convert Avro schema to XML schema
+## Convert Avrotize Schema to XML schema
 
 ```bash
 avrotize a2x --avsc <path_to_avro_schema_file> --xsd <path_to_xsd_schema_file>
 ```
 
 Parameters:
 
-- `--avsc`: The path to the Avro schema file to be converted.
+- `--avsc`: The path to the Avrotize Schema file to be converted.
 - `--xsd`: The path to the XML schema file to write the conversion result to.
 
 Conversion notes:
 
 - Avro record types are mapped to XML Schema complex types with elements.
 - Avro enum types are mapped to XML Schema simple types with restrictions.
 - Avro logical types are mapped to XML Schema simple types with restrictions
   where required.
 - Avro unions are mapped to standalone XSD simple type definitions with a
   union restriction if all union types are primitives.
 - Avro unions with complex types are resolved into distinct types for
   each option that are then joined with a choice.
 
-## Convert ASN.1 schema to Avro schema
+## Convert ASN.1 schema to Avrotize Schema
 
 ```bash
 avrotize asn2a --asn <path_to_asn1_schema_file>[,<path_to_asn1_schema_file>,...]  --avsc <path_to_avro_schema_file>
 ```
 
 Parameters:
 
 - `--asn`: The path to the ASN.1 schema file to be converted. The tool supports
   multiple files in a comma-separated list.
-- `--avsc`: The path to the Avro schema file to write the conversion result to.
+- `--avsc`: The path to the Avrotize Schema file to write the conversion result to.
 
 Conversion notes:
 
 - All ASN.1 types are mapped to Avro record types, enums, and unions. Avro does
   not support the same level of nesting of types as ASN.1, the tool will map
   the types to the best fit.
 - The tool will map the following ASN.1 types to Avro types:
@@ -354,25 +399,25 @@
     `VideotexString`, `GraphicString`, `VisibleString`, `GeneralString`, `UniversalString`,
     `CharacterString`, `T61String` are all mapped to Avro string type.
   - All other ASN.1 types are mapped to Avro string type.
 - The ability to parse ASN.1 schema files is limited and the tool may not be able
   to parse all ASN.1 files. The tool is based on the Python asn1tools package and
   is limited to that package's capabilities.
 
-### Convert Kusto table definition to Avro schema
+### Convert Kusto table definition to Avrotize Schema
 
 ```bash
 avrotize k2a --kusto-uri <kusto_cluster_uri> --kusto-database <kusto_database> --avsc <path_to_avro_schema_file> --emit-cloudevents-xregistry
 ```
 
 Parameters:
 
 - `--kusto-uri`: The URI of the Kusto cluster to connect to.
 - `--kusto-database`: The name of the Kusto database to read the table definitions from.
-- `--avsc`: The path to the Avro schema file to write the conversion result to.
+- `--avsc`: The path to the Avrotize Schema file to write the conversion result to.
 - `--emit-cloudevents-xregistry`: (optional) See discussion below.
 
 Conversion notes:
 - The tool directly connects to the Kusto cluster and reads the table
   definitions from the specified database. The tool will convert all tables in
   the database to Avro record types, returned in a top-level type union.
 - Connecting to the Kusto cluster leans on the same authentication mechanisms as
@@ -403,218 +448,235 @@
   Schema for each table in the embedded schema registry. If one or more tables
   are found to contain CloudEvent data (as indicated by the presence of the
   CloudEvents attribute columns), the tool will inspect the content of the
   `type` (or `__type` or `__type`) columns to determine which CloudEvent types
   have been stored in the table and will emit a CloudEvent definition and schema
   for each unique type.
 
-### Convert Avro schema to Kusto table declaration
+### Convert Avrotize Schema to Kusto table declaration
 
 ```bash
 avrotize a2k --avsc <path_to_avro_schema_file> --kusto <path_to_kusto_kql_file> [--record-type <record_type>] [--emit-cloudevents-columns] [--emit-cloudevents-dispatch]
 ```
 
 Parameters:
 
-- `--avsc`: The path to the Avro schema file to be converted.
+- `--avsc`: The path to the Avrotize Schema file to be converted.
 - `--kusto`: The path to the Kusto KQL file to write the conversion result to.
 - `--record-type`: (optional) The name of the Avro record type to convert to a Kusto table.
 - `--emit-cloudevents-columns`: (optional) If set, the tool will add
   [CloudEvents](https://cloudevents.io) attribute columns to the table: `___id`,
   `___source`, `___subject`, `___type`, and `___time`.
 - `--emit-cloudevents-dispatch`: (optional) If set, the tool will add a table named
   `_cloudevents_dispatch` to the script or database, which serves as an ingestion and
   dispatch table for CloudEvents. The table has columns for the core CloudEvents attributes
-  and a `data` column that holds the CloudEvents data. For each table in the Avro schema,
+  and a `data` column that holds the CloudEvents data. For each table in the Avrotize Schema,
   the tool will create an update policy that maps events whose `type` attribute matches
   the Avro type name to the respective table.
   
 
 Conversion notes:
 
-- Only the Avro `record` type can be mapped to a Kusto table. If the Avro schema
+- Only the Avro `record` type can be mapped to a Kusto table. If the Avrotize Schema
   contains other types (like `enum` or `array`), the tool will ignore them.
-- Only the first `record` type in the Avro schema is converted to a Kusto table.
-  If the Avro schema contains other `record` types, they will be ignored. The
+- Only the first `record` type in the Avrotize Schema is converted to a Kusto table.
+  If the Avrotize Schema contains other `record` types, they will be ignored. The
   `--record-type` option can be used to specify which `record` type to convert.
 - The fields of the record are mapped to columns in the Kusto table. Fields that
   are records or arrays or maps are mapped to columns of type `dynamic` in the
   Kusto table.
 
-### Convert Avro schema to T-SQL table definition
+### Convert Avrotize Schema to T-SQL table definition
 
 ```bash
 avrotize a2tsql --avsc <path_to_avro_schema_file> --tsql <path_to_sql_file> [--record-type <record_type>] [--emit-cloudevents-columns]
 ```
 
 Parameters:
 
-- `--avsc`: The path to the Avro schema file to be converted.
+- `--avsc`: The path to the Avrotize Schema file to be converted.
 - `--tsql`: The path to the T-SQL file to write the conversion result to.
 - `--record-type`: (optional) The name of the Avro record type to convert to a T-SQL table.
 - `--emit-cloudevents-columns`: (optional) If set, the tool will add
   [CloudEvents](https://cloudevents.io) attribute columns to the table: `__id`,
   `__source`, `__subject`, `__type`, and `__time`.
 
 Conversion notes:
 
-- Only the Avro `record` type can be mapped to a T-SQL table. If the Avro schema
+- Only the Avro `record` type can be mapped to a T-SQL table. If the Avrotize Schema
   contains other types (like `enum` or `array`), the tool will ignore them.
-- Only the first `record` type in the Avro schema is converted to a T-SQL table.
-  If the Avro schema contains other `record` types, they will be ignored. The
+- Only the first `record` type in the Avrotize Schema is converted to a T-SQL table.
+  If the Avrotize Schema contains other `record` types, they will be ignored. The
   `--record-type` option can be used to specify which `record` type to convert.
 - The fields of the record are mapped to columns in the T-SQL table. Fields of
   type `record` or `array` or `map` are mapped to columns of type `varchar(max)` in
   the T-SQL table and it's assumed for them to hold JSON data.
-- The emitted script sets extended properties to the columns with the Avro schema
+- The emitted script sets extended properties to the columns with the Avrotize Schema
   definition of the field in a JSON format. This allows for easy introspection of
-  the serialized Avro schema in the field definition.
+  the serialized Avrotize Schema in the field definition.
 
-## Convert Avro schema to empty Parquet file
+## Convert Avrotize Schema to empty Parquet file
 
 ```bash
 avrotize a2pq --avsc <path_to_avro_schema_file> --parquet <path_to_parquet_schema_file> [--record-type <record-type-from-avro>] [--emit-cloudevents-columns]
 ```
 
 Parameters:
 
-- `--avsc`: The path to the Avro schema file to be converted.
+- `--avsc`: The path to the Avrotize Schema file to be converted.
 - `--parquet`: The path to the Parquet schema file to write the conversion result to.
 - `--record-type`: (optional) The name of the Avro record type to convert to a Parquet schema.
 - `--emit-cloudevents-columns`: (optional) If set, the tool will add
   [CloudEvents](https://cloudevents.io) attribute columns to the Parquet schema:
   `__id`, `__source`, `__subject`, `__type`, and `__time`.
 
 Conversion notes:
 
 - The emitted Parquet file contains only the schema, no data rows.
-- The tool only supports writing Parquet files for Avro schema that describe a
-  single `record` type. If the Avro schema contains a top-level union, the
+- The tool only supports writing Parquet files for Avrotize Schema that describe a
+  single `record` type. If the Avrotize Schema contains a top-level union, the
   `--record-type` option must be used to specify which record type to emit.
 - The fields of the record are mapped to columns in the Parquet file. Array and
   record fields are mapped to Parquet nested types. Avro type unions are mapped
   to structures, not to Parquet unions since those are not supported by the
   PyArrow library used here.
 
-### Generate C# code from Avro schema
+## Convert Parquet schema to Avrotize Schema
+
+```bash
+avrotize pq2a --parquet <path_to_parquet_schema_file> --avsc <path_to_avro_schema_file> --namespace <avro_schema_namespace>
+```
+
+Parameters:
+
+- `--parquet`: The path to the Parquet file whose schema is to be converted.
+- `--avsc`: The path to the Avrotize Schema file to write the conversion result to.
+- `--namespace`: The namespace to use in the Avrotize Schema.
+
+Conversion notes:
+
+- The tool reads the schema from the Parquet file and converts it to an Avro
+  schema. The Avrotize Schema is written to the specified file.
+
+### Generate C# code from Avrotize Schema
 
 ```bash
 avrotize a2csharp --avsc <path_to_avro_schema_file> --csharp <path_to_csharp_directory> [--avro-annotation] [--system-text-json-annotation] [--newtonsoft-json-annotation] [--pascal-properties]
 ```
 
 Parameters:
-- `--avsc`: The path to the Avro schema file to be converted.
+- `--avsc`: The path to the Avrotize Schema file to be converted.
 - `--csharp`: The path to the C# directory to write the conversion result to.
 - `--avro-annotation`: (optional) If set, the tool will add Avro annotations to the C# classes.
 - `--system-text-json-annotation`: (optional) If set, the tool will add System.Text.Json annotations to the C# classes.
 - `--newtonsoft-json-annotation`: (optional) If set, the tool will add Newtonsoft.Json annotations to the C# classes.
 - `--pascal-properties`: (optional) If set, the tool will use PascalCase properties in the C# classes.
 - `--namespace`: (optional) The namespace to use in the generated C# classes.
 
 Conversion notes:
-- The tool generates C# classes that represent the Avro schema as data classes.
+- The tool generates C# classes that represent the Avrotize Schema as data classes.
 - Using the `--system-text-json-annotation` or `--newtonsoft-json-annotation` option
   will add annotations for the respective JSON serialization library to the generated
-  C# classes. Because the [`JSON Schema to Avro`](#convert-json-schema-to-avro-schema) conversion generally
-  preserves the JSON Schema structure in the Avro schema, the generated C# classes
+  C# classes. Because the [`JSON Schema to Avro`](#convert-json-schema-to-avrotize-schema) conversion generally
+  preserves the JSON Schema structure in the Avrotize Schema, the generated C# classes
   can be used to serialize and deserialize data that is valid per the input JSON schema.
 - Only the `--system-text-json-annotation` option generates classes that support type unions.
 - The classes are generated into a directory structure that reflects the Avro namespace
   structure. The tool drops a minimal, default `.csproj` project file into the given
   directory if none exists.
 
 Read more about the C# code generation in the [C# code generation documentation](csharpcodegen.md).
 
 
-### Generate Java code from Avro schema
+### Generate Java code from Avrotize Schema
 
 ```bash
 avrotize a2java --avsc <path_to_avro_schema_file> --java <path_to_java_directory> [--package <java_package_name>] [--avro-annotation] [--jackson-annotation] [--pascal-properties]
 ```
 
 Parameters:
-- `--avsc`: The path to the Avro schema file to be converted.
+- `--avsc`: The path to the Avrotize Schema file to be converted.
 - `--java`: The path to the Java directory to write the conversion result to.
 - `--package`: (optional) The Java package name to use in the generated Java classes.
 - `--avro-annotation`: (optional) If set, the tool will add Avro annotations to the Java classes.
 - `--jackson-annotation`: (optional) If set, the tool will add Jackson annotations to the Java classes.
 - `--pascal-properties`: (optional) If set, the tool will use PascalCase properties in the Java classes.
 
 Conversion notes:
 
-- The tool generates Java classes that represent the Avro schema as data classes. 
+- The tool generates Java classes that represent the Avrotize Schema as data classes. 
 - Using the `--jackson-annotation` option will add annotations for the Jackson 
   JSON serialization library to the generated Java classes. Because the 
-  [`JSON Schema to Avro`](#convert-json-schema-to-avro-schema) conversion generally
-  preserves the JSON Schema structure in the Avro schema, the generated Java classes
+  [`JSON Schema to Avro`](#convert-json-schema-to-avrotize-schema) conversion generally
+  preserves the JSON Schema structure in the Avrotize Schema, the generated Java classes
   can be used to serialize and deserialize data that is valid per the input JSON schema.
 - The directory `/src/main/java` is created in the specified directory and the
   generated Java classes are written to this directory. The tool drops a
   minimal, default `pom.xml` Maven project file into the given directory if none
   exists.
 
 Read more about the Java code generation in the [Java code generation documentation](javacodegen.md).
 
-### Generate Python code from Avro schema
+### Generate Python code from Avrotize Schema
 
-This command generates Python dataclasses from an Avro schema.
+This command generates Python dataclasses from an Avrotize Schema.
 
 ```bash
 avrotize a2py --avsc <path_to_avro_schema_file> --python <path_to_python_directory> [--package <python_package_name>]
 ```
 
 Parameters:
-- `--avsc`: The path to the Avro schema file to be converted.
+- `--avsc`: The path to the Avrotize Schema file to be converted.
 - `--python`: The path to the Python directory to write the conversion result to.
 - `--package`: (optional) The Python package name to use in the generated Python classes.
 - `--avro-annotation`: (optional) If set, the tool will add Avro annotations to the Python classes.
 - `--dataclasses-json-annotation`: (optional) If set, the tool will add dataclasses-json annotations to the Python classes
 
 Conversion notes:
 - The tool generates Python dataclasses (Python 3.7 or later)
 - The classes are generated into a directory structure that reflects the Avro namespace
   structure. The tool drops a minimal, default `__init__.py` file into any created
   package directories if none exists.
 
-### Generate TypeScript code from Avro schema
+### Generate TypeScript code from Avrotize Schema
 
 ```bash
 avrotize a2ts --avsc <path_to_avro_schema_file> --ts <path_to_typescript_directory> [--package <typescript_namespace>] [--avro-annotation] [--typedjson-annotation]
 ``` 
 
 Parameters:
-- `--avsc`: The path to the Avro schema file to be converted.
+- `--avsc`: The path to the Avrotize Schema file to be converted.
 - `--ts`: The path to the TypeScript directory to write the conversion result to.
 - `--package`: (optional) The TypeScript namespace to use in the generated TypeScript classes.
 - `--avro-annotation`: (optional) If set, the tool will add Avro annotations to the TypeScript classes.
 - `--typedjson-annotation`: (optional) If set, the tool will add TypedJSON annotations to the TypeScript classes.
 
 Conversion notes:
-- The tool generates TypeScript interfaces that represent the Avro schema as data classes.
+- The tool generates TypeScript interfaces that represent the Avrotize Schema as data classes.
 - Using the `--typedjson-annotation` option will add annotations for the TypedJSON
   JSON serialization library to the generated TypeScript classes. Because the
-  [`JSON Schema to Avro`](#convert-json-schema-to-avro-schema) conversion generally
-  preserves the JSON Schema structure in the Avro schema, the generated TypeScript
+  [`JSON Schema to Avro`](#convert-json-schema-to-avrotize-schema) conversion generally
+  preserves the JSON Schema structure in the Avrotize Schema, the generated TypeScript
   classes can be used to serialize and deserialize data that is valid per the input JSON schema.
 - The classes are generated into a directory structure that reflects the Avro namespace
 
-### Generate JavaScript code from Avro schema
+### Generate JavaScript code from Avrotize Schema
 
 ```bash
 avrotize a2js --avsc <path_to_avro_schema_file> --js <path_to_javascript_directory> [--package <javascript_namespace>] [--avro-annotation]
 ```
 
 Parameters:
-- `--avsc`: The path to the Avro schema file to be converted.
+- `--avsc`: The path to the Avrotize Schema file to be converted.
 - `--js`: The path to the JavaScript directory to write the conversion result to.
 - `--package`: (optional) The JavaScript namespace to use in the generated JavaScript classes.
 - `--avro-annotation`: (optional) If set, the tool will add Avro annotations to the JavaScript classes.
 
 Conversion notes:
-- The tool generates JavaScript classes that represent the Avro schema as data classes.
+- The tool generates JavaScript classes that represent the Avrotize Schema as data classes.
 - The classes are generated into a directory structure that reflects the Avro namespace
 
 
 ## Contributing
 
 Contributions are welcome! Please feel free to submit a Pull Request.
```

