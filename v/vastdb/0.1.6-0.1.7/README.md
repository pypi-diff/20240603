# Comparing `tmp/vastdb-0.1.6.tar.gz` & `tmp/vastdb-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vastdb-0.1.6.tar", last modified: Thu May 23 11:15:59 2024, max compression
+gzip compressed data, was "vastdb-0.1.7.tar", last modified: Mon Jun  3 12:25:31 2024, max compression
```

## Comparing `vastdb-0.1.6.tar` & `vastdb-0.1.7.tar`

### file list

```diff
@@ -1,198 +1,198 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 11:15:59.140398 vastdb-0.1.6/
--rw-rw-rw-   0 root         (0) root         (0)     5182 2024-05-23 11:00:32.000000 vastdb-0.1.6/CHANGELOG.md
--rw-rw-rw-   0 root         (0) root         (0)    11333 2024-05-20 13:26:33.000000 vastdb-0.1.6/LICENSE
--rw-rw-rw-   0 root         (0) root         (0)       38 2024-05-20 13:26:33.000000 vastdb-0.1.6/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     1348 2024-05-23 11:15:59.139398 vastdb-0.1.6/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     6037 2024-05-20 13:26:33.000000 vastdb-0.1.6/README.md
--rw-rw-rw-   0 root         (0) root         (0)      101 2024-05-20 13:26:33.000000 vastdb-0.1.6/requirements.txt
--rw-r--r--   0 root         (0) root         (0)       38 2024-05-23 11:15:59.140398 vastdb-0.1.6/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1728 2024-05-23 11:00:32.000000 vastdb-0.1.6/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 11:15:59.103397 vastdb-0.1.6/vast_flatbuf/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-23 11:00:32.000000 vastdb-0.1.6/vast_flatbuf/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 11:15:59.103397 vastdb-0.1.6/vast_flatbuf/org/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-23 11:00:32.000000 vastdb-0.1.6/vast_flatbuf/org/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 11:15:59.104397 vastdb-0.1.6/vast_flatbuf/org/apache/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-23 11:00:32.000000 vastdb-0.1.6/vast_flatbuf/org/apache/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 11:15:59.104397 vastdb-0.1.6/vast_flatbuf/org/apache/arrow/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-23 11:00:32.000000 vastdb-0.1.6/vast_flatbuf/org/apache/arrow/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 11:15:59.104397 vastdb-0.1.6/vast_flatbuf/org/apache/arrow/computeir/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-23 11:00:32.000000 vastdb-0.1.6/vast_flatbuf/org/apache/arrow/computeir/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 11:15:59.119397 vastdb-0.1.6/vast_flatbuf/org/apache/arrow/computeir/flatbuf/
--rw-rw-rw-   0 root         (0) root         (0)     5630 2024-05-20 13:26:33.000000 vastdb-0.1.6/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Aggregate.py
--rw-rw-rw-   0 root         (0) root         (0)     2212 2024-05-20 13:26:33.000000 vastdb-0.1.6/vast_flatbuf/org/apache/arrow/computeir/flatbuf/ArraySlice.py
--rw-rw-rw-   0 root         (0) root         (0)     1567 2024-05-20 13:26:33.000000 vastdb-0.1.6/vast_flatbuf/org/apache/arrow/computeir/flatbuf/ArraySubscript.py
--rw-rw-rw-   0 root         (0) root         (0)     2494 2024-05-20 13:26:33.000000 vastdb-0.1.6/vast_flatbuf/org/apache/arrow/computeir/flatbuf/BinaryLiteral.py
--rw-rw-rw-   0 root         (0) root         (0)     1521 2024-05-20 13:26:33.000000 vastdb-0.1.6/vast_flatbuf/org/apache/arrow/computeir/flatbuf/BooleanLiteral.py
--rw-rw-rw-   0 root         (0) root         (0)      182 2024-05-20 13:26:33.000000 vastdb-0.1.6/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Bound.py
--rw-rw-rw-   0 root         (0) root         (0)     4434 2024-05-20 13:26:33.000000 vastdb-0.1.6/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Call.py
--rw-rw-rw-   0 root         (0) root         (0)     2429 2024-05-20 13:26:33.000000 vastdb-0.1.6/vast_flatbuf/org/apache/arrow/computeir/flatbuf/CaseFragment.py
--rw-rw-rw-   0 root         (0) root         (0)     2520 2024-05-20 13:26:33.000000 vastdb-0.1.6/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Cast.py
--rw-rw-rw-   0 root         (0) root         (0)      236 2024-05-20 13:26:33.000000 vastdb-0.1.6/vast_flatbuf/org/apache/arrow/computeir/flatbuf/ConcreteBoundImpl.py
--rw-rw-rw-   0 root         (0) root         (0)     3490 2024-05-20 13:26:33.000000 vastdb-0.1.6/vast_flatbuf/org/apache/arrow/computeir/flatbuf/ConditionalCase.py
--rw-rw-rw-   0 root         (0) root         (0)     1059 2024-05-20 13:26:33.000000 vastdb-0.1.6/vast_flatbuf/org/apache/arrow/computeir/flatbuf/CurrentRow.py
--rw-rw-rw-   0 root         (0) root         (0)     1489 2024-05-20 13:26:33.000000 vastdb-0.1.6/vast_flatbuf/org/apache/arrow/computeir/flatbuf/DateLiteral.py
--rw-rw-rw-   0 root         (0) root         (0)     2576 2024-05-20 13:26:33.000000 vastdb-0.1.6/vast_flatbuf/org/apache/arrow/computeir/flatbuf/DecimalLiteral.py
--rw-rw-rw-   0 root         (0) root         (0)      484 2024-05-20 13:26:33.000000 vastdb-0.1.6/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Deref.py
--rw-rw-rw-   0 root         (0) root         (0)     1521 2024-05-20 13:26:33.000000 vastdb-0.1.6/vast_flatbuf/org/apache/arrow/computeir/flatbuf/DurationLiteral.py
--rw-rw-rw-   0 root         (0) root         (0)     2258 2024-05-20 13:26:33.000000 vastdb-0.1.6/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Expression.py
--rw-rw-rw-   0 root         (0) root         (0)      498 2024-05-20 13:26:33.000000 vastdb-0.1.6/vast_flatbuf/org/apache/arrow/computeir/flatbuf/ExpressionImpl.py
--rw-rw-rw-   0 root         (0) root         (0)     1584 2024-05-20 13:26:33.000000 vastdb-0.1.6/vast_flatbuf/org/apache/arrow/computeir/flatbuf/FieldIndex.py
--rw-rw-rw-   0 root         (0) root         (0)     2850 2024-05-20 13:26:33.000000 vastdb-0.1.6/vast_flatbuf/org/apache/arrow/computeir/flatbuf/FieldRef.py
--rw-rw-rw-   0 root         (0) root         (0)     3260 2024-05-20 13:26:33.000000 vastdb-0.1.6/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Filter.py
--rw-rw-rw-   0 root         (0) root         (0)     2602 2024-05-20 13:26:33.000000 vastdb-0.1.6/vast_flatbuf/org/apache/arrow/computeir/flatbuf/FixedSizeBinaryLiteral.py
--rw-rw-rw-   0 root         (0) root         (0)     1515 2024-05-20 13:26:33.000000 vastdb-0.1.6/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Float16Literal.py
--rw-rw-rw-   0 root         (0) root         (0)     1521 2024-05-20 13:26:33.000000 vastdb-0.1.6/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Float32Literal.py
--rw-rw-rw-   0 root         (0) root         (0)     1521 2024-05-20 13:26:33.000000 vastdb-0.1.6/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Float64Literal.py
--rw-rw-rw-   0 root         (0) root         (0)     2130 2024-05-20 13:26:33.000000 vastdb-0.1.6/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Following.py
--rw-rw-rw-   0 root         (0) root         (0)      186 2024-05-20 13:26:33.000000 vastdb-0.1.6/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Frame.py
--rw-rw-rw-   0 root         (0) root         (0)     2403 2024-05-20 13:26:33.000000 vastdb-0.1.6/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Grouping.py
--rw-rw-rw-   0 root         (0) root         (0)     1497 2024-05-20 13:26:33.000000 vastdb-0.1.6/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Int16Literal.py
--rw-rw-rw-   0 root         (0) root         (0)     1497 2024-05-20 13:26:33.000000 vastdb-0.1.6/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Int32Literal.py
--rw-rw-rw-   0 root         (0) root         (0)     1497 2024-05-20 13:26:33.000000 vastdb-0.1.6/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Int64Literal.py
--rw-rw-rw-   0 root         (0) root         (0)     1487 2024-05-20 13:26:33.000000 vastdb-0.1.6/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Int8Literal.py
--rw-rw-rw-   0 root         (0) root         (0)     2139 2024-05-20 13:26:33.000000 vastdb-0.1.6/vast_flatbuf/org/apache/arrow/computeir/flatbuf/IntervalLiteral.py
--rw-rw-rw-   0 root         (0) root         (0)     2197 2024-05-20 13:26:33.000000 vastdb-0.1.6/vast_flatbuf/org/apache/arrow/computeir/flatbuf/IntervalLiteralDaysMilliseconds.py
--rw-rw-rw-   0 root         (0) root         (0)      211 2024-05-20 13:26:33.000000 vastdb-0.1.6/vast_flatbuf/org/apache/arrow/computeir/flatbuf/IntervalLiteralImpl.py
--rw-rw-rw-   0 root         (0) root         (0)     1578 2024-05-20 13:26:33.000000 vastdb-0.1.6/vast_flatbuf/org/apache/arrow/computeir/flatbuf/IntervalLiteralMonths.py
--rw-rw-rw-   0 root         (0) root         (0)     4455 2024-05-20 13:26:33.000000 vastdb-0.1.6/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Join.py
--rw-rw-rw-   0 root         (0) root         (0)      230 2024-05-20 13:26:33.000000 vastdb-0.1.6/vast_flatbuf/org/apache/arrow/computeir/flatbuf/JoinKind.py
--rw-rw-rw-   0 root         (0) root         (0)     2309 2024-05-20 13:26:33.000000 vastdb-0.1.6/vast_flatbuf/org/apache/arrow/computeir/flatbuf/KeyValue.py
--rw-rw-rw-   0 root         (0) root         (0)     3368 2024-05-20 13:26:33.000000 vastdb-0.1.6/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Limit.py
--rw-rw-rw-   0 root         (0) root         (0)     2400 2024-05-20 13:26:33.000000 vastdb-0.1.6/vast_flatbuf/org/apache/arrow/computeir/flatbuf/ListLiteral.py
--rw-rw-rw-   0 root         (0) root         (0)     2797 2024-05-20 13:26:33.000000 vastdb-0.1.6/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Literal.py
--rw-rw-rw-   0 root         (0) root         (0)     2526 2024-05-20 13:26:33.000000 vastdb-0.1.6/vast_flatbuf/org/apache/arrow/computeir/flatbuf/LiteralColumn.py
--rw-rw-rw-   0 root         (0) root         (0)      682 2024-05-20 13:26:33.000000 vastdb-0.1.6/vast_flatbuf/org/apache/arrow/computeir/flatbuf/LiteralImpl.py
--rw-rw-rw-   0 root         (0) root         (0)     3284 2024-05-20 13:26:33.000000 vastdb-0.1.6/vast_flatbuf/org/apache/arrow/computeir/flatbuf/LiteralRelation.py
--rw-rw-rw-   0 root         (0) root         (0)     1723 2024-05-20 13:26:33.000000 vastdb-0.1.6/vast_flatbuf/org/apache/arrow/computeir/flatbuf/MapKey.py
--rw-rw-rw-   0 root         (0) root         (0)     2392 2024-05-20 13:26:33.000000 vastdb-0.1.6/vast_flatbuf/org/apache/arrow/computeir/flatbuf/MapLiteral.py
--rw-rw-rw-   0 root         (0) root         (0)     3847 2024-05-20 13:26:33.000000 vastdb-0.1.6/vast_flatbuf/org/apache/arrow/computeir/flatbuf/OrderBy.py
--rw-rw-rw-   0 root         (0) root         (0)      349 2024-05-20 13:26:33.000000 vastdb-0.1.6/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Ordering.py
--rw-rw-rw-   0 root         (0) root         (0)     2378 2024-05-20 13:26:33.000000 vastdb-0.1.6/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Plan.py
--rw-rw-rw-   0 root         (0) root         (0)     2130 2024-05-20 13:26:33.000000 vastdb-0.1.6/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Preceding.py
--rw-rw-rw-   0 root         (0) root         (0)     3941 2024-05-20 13:26:33.000000 vastdb-0.1.6/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Project.py
--rw-rw-rw-   0 root         (0) root         (0)     1526 2024-05-20 13:26:33.000000 vastdb-0.1.6/vast_flatbuf/org/apache/arrow/computeir/flatbuf/RelId.py
--rw-rw-rw-   0 root         (0) root         (0)     2113 2024-05-20 13:26:33.000000 vastdb-0.1.6/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Relation.py
--rw-rw-rw-   0 root         (0) root         (0)      315 2024-05-20 13:26:33.000000 vastdb-0.1.6/vast_flatbuf/org/apache/arrow/computeir/flatbuf/RelationImpl.py
--rw-rw-rw-   0 root         (0) root         (0)      217 2024-05-20 13:26:33.000000 vastdb-0.1.6/vast_flatbuf/org/apache/arrow/computeir/flatbuf/SetOpKind.py
--rw-rw-rw-   0 root         (0) root         (0)     3678 2024-05-20 13:26:33.000000 vastdb-0.1.6/vast_flatbuf/org/apache/arrow/computeir/flatbuf/SetOperation.py
--rw-rw-rw-   0 root         (0) root         (0)     3952 2024-05-20 13:26:33.000000 vastdb-0.1.6/vast_flatbuf/org/apache/arrow/computeir/flatbuf/SimpleCase.py
--rw-rw-rw-   0 root         (0) root         (0)     2221 2024-05-20 13:26:33.000000 vastdb-0.1.6/vast_flatbuf/org/apache/arrow/computeir/flatbuf/SortKey.py
--rw-rw-rw-   0 root         (0) root         (0)     5650 2024-05-20 13:26:33.000000 vastdb-0.1.6/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Source.py
--rw-rw-rw-   0 root         (0) root         (0)     1533 2024-05-20 13:26:33.000000 vastdb-0.1.6/vast_flatbuf/org/apache/arrow/computeir/flatbuf/StringLiteral.py
--rw-rw-rw-   0 root         (0) root         (0)     1593 2024-05-20 13:26:33.000000 vastdb-0.1.6/vast_flatbuf/org/apache/arrow/computeir/flatbuf/StructField.py
--rw-rw-rw-   0 root         (0) root         (0)     2539 2024-05-20 13:26:33.000000 vastdb-0.1.6/vast_flatbuf/org/apache/arrow/computeir/flatbuf/StructLiteral.py
--rw-rw-rw-   0 root         (0) root         (0)     1489 2024-05-20 13:26:33.000000 vastdb-0.1.6/vast_flatbuf/org/apache/arrow/computeir/flatbuf/TimeLiteral.py
--rw-rw-rw-   0 root         (0) root         (0)     1529 2024-05-20 13:26:33.000000 vastdb-0.1.6/vast_flatbuf/org/apache/arrow/computeir/flatbuf/TimestampLiteral.py
--rw-rw-rw-   0 root         (0) root         (0)     1507 2024-05-20 13:26:33.000000 vastdb-0.1.6/vast_flatbuf/org/apache/arrow/computeir/flatbuf/UInt16Literal.py
--rw-rw-rw-   0 root         (0) root         (0)     1507 2024-05-20 13:26:33.000000 vastdb-0.1.6/vast_flatbuf/org/apache/arrow/computeir/flatbuf/UInt32Literal.py
--rw-rw-rw-   0 root         (0) root         (0)     1507 2024-05-20 13:26:33.000000 vastdb-0.1.6/vast_flatbuf/org/apache/arrow/computeir/flatbuf/UInt64Literal.py
--rw-rw-rw-   0 root         (0) root         (0)     1497 2024-05-20 13:26:33.000000 vastdb-0.1.6/vast_flatbuf/org/apache/arrow/computeir/flatbuf/UInt8Literal.py
--rw-rw-rw-   0 root         (0) root         (0)     1051 2024-05-20 13:26:33.000000 vastdb-0.1.6/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Unbounded.py
--rw-rw-rw-   0 root         (0) root         (0)     7527 2024-05-20 13:26:33.000000 vastdb-0.1.6/vast_flatbuf/org/apache/arrow/computeir/flatbuf/WindowCall.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-23 11:00:32.000000 vastdb-0.1.6/vast_flatbuf/org/apache/arrow/computeir/flatbuf/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 11:15:59.130398 vastdb-0.1.6/vast_flatbuf/org/apache/arrow/flatbuf/
--rw-rw-rw-   0 root         (0) root         (0)     1026 2024-05-20 13:26:33.000000 vastdb-0.1.6/vast_flatbuf/org/apache/arrow/flatbuf/Binary.py
--rw-rw-rw-   0 root         (0) root         (0)     1326 2024-05-20 13:26:33.000000 vastdb-0.1.6/vast_flatbuf/org/apache/arrow/flatbuf/Block.py
--rw-rw-rw-   0 root         (0) root         (0)     2310 2024-05-20 13:26:33.000000 vastdb-0.1.6/vast_flatbuf/org/apache/arrow/flatbuf/BodyCompression.py
--rw-rw-rw-   0 root         (0) root         (0)      836 2024-05-20 13:26:33.000000 vastdb-0.1.6/vast_flatbuf/org/apache/arrow/flatbuf/BodyCompressionMethod.py
--rw-rw-rw-   0 root         (0) root         (0)      993 2024-05-20 13:26:33.000000 vastdb-0.1.6/vast_flatbuf/org/apache/arrow/flatbuf/Bool.py
--rw-rw-rw-   0 root         (0) root         (0)     1430 2024-05-20 13:26:33.000000 vastdb-0.1.6/vast_flatbuf/org/apache/arrow/flatbuf/Buffer.py
--rw-rw-rw-   0 root         (0) root         (0)      155 2024-05-20 13:26:33.000000 vastdb-0.1.6/vast_flatbuf/org/apache/arrow/flatbuf/CompressionType.py
--rw-rw-rw-   0 root         (0) root         (0)     1760 2024-05-20 13:26:33.000000 vastdb-0.1.6/vast_flatbuf/org/apache/arrow/flatbuf/Date.py
--rw-rw-rw-   0 root         (0) root         (0)      149 2024-05-20 13:26:33.000000 vastdb-0.1.6/vast_flatbuf/org/apache/arrow/flatbuf/DateUnit.py
--rw-rw-rw-   0 root         (0) root         (0)     2855 2024-05-20 13:26:33.000000 vastdb-0.1.6/vast_flatbuf/org/apache/arrow/flatbuf/Decimal.py
--rw-rw-rw-   0 root         (0) root         (0)     3148 2024-05-20 13:26:33.000000 vastdb-0.1.6/vast_flatbuf/org/apache/arrow/flatbuf/DictionaryBatch.py
--rw-rw-rw-   0 root         (0) root         (0)     4091 2024-05-20 13:26:33.000000 vastdb-0.1.6/vast_flatbuf/org/apache/arrow/flatbuf/DictionaryEncoding.py
--rw-rw-rw-   0 root         (0) root         (0)      410 2024-05-20 13:26:33.000000 vastdb-0.1.6/vast_flatbuf/org/apache/arrow/flatbuf/DictionaryKind.py
--rw-rw-rw-   0 root         (0) root         (0)     1456 2024-05-20 13:26:33.000000 vastdb-0.1.6/vast_flatbuf/org/apache/arrow/flatbuf/Duration.py
--rw-rw-rw-   0 root         (0) root         (0)      267 2024-05-20 13:26:33.000000 vastdb-0.1.6/vast_flatbuf/org/apache/arrow/flatbuf/Endianness.py
--rw-rw-rw-   0 root         (0) root         (0)     1289 2024-05-20 13:26:33.000000 vastdb-0.1.6/vast_flatbuf/org/apache/arrow/flatbuf/Feature.py
--rw-rw-rw-   0 root         (0) root         (0)     7048 2024-05-20 13:26:33.000000 vastdb-0.1.6/vast_flatbuf/org/apache/arrow/flatbuf/Field.py
--rw-rw-rw-   0 root         (0) root         (0)     1669 2024-05-20 13:26:33.000000 vastdb-0.1.6/vast_flatbuf/org/apache/arrow/flatbuf/FieldNode.py
--rw-rw-rw-   0 root         (0) root         (0)     1589 2024-05-20 13:26:33.000000 vastdb-0.1.6/vast_flatbuf/org/apache/arrow/flatbuf/FixedSizeBinary.py
--rw-rw-rw-   0 root         (0) root         (0)     1569 2024-05-20 13:26:33.000000 vastdb-0.1.6/vast_flatbuf/org/apache/arrow/flatbuf/FixedSizeList.py
--rw-rw-rw-   0 root         (0) root         (0)     1541 2024-05-20 13:26:33.000000 vastdb-0.1.6/vast_flatbuf/org/apache/arrow/flatbuf/FloatingPoint.py
--rw-rw-rw-   0 root         (0) root         (0)     6448 2024-05-20 13:26:33.000000 vastdb-0.1.6/vast_flatbuf/org/apache/arrow/flatbuf/Footer.py
--rw-rw-rw-   0 root         (0) root         (0)     1925 2024-05-20 13:26:33.000000 vastdb-0.1.6/vast_flatbuf/org/apache/arrow/flatbuf/Int.py
--rw-rw-rw-   0 root         (0) root         (0)     1456 2024-05-20 13:26:33.000000 vastdb-0.1.6/vast_flatbuf/org/apache/arrow/flatbuf/Interval.py
--rw-rw-rw-   0 root         (0) root         (0)      180 2024-05-20 13:26:33.000000 vastdb-0.1.6/vast_flatbuf/org/apache/arrow/flatbuf/IntervalUnit.py
--rw-rw-rw-   0 root         (0) root         (0)     2139 2024-05-20 13:26:33.000000 vastdb-0.1.6/vast_flatbuf/org/apache/arrow/flatbuf/KeyValue.py
--rw-rw-rw-   0 root         (0) root         (0)     1131 2024-05-20 13:26:33.000000 vastdb-0.1.6/vast_flatbuf/org/apache/arrow/flatbuf/LargeBinary.py
--rw-rw-rw-   0 root         (0) root         (0)     1117 2024-05-20 13:26:33.000000 vastdb-0.1.6/vast_flatbuf/org/apache/arrow/flatbuf/LargeList.py
--rw-rw-rw-   0 root         (0) root         (0)     1117 2024-05-20 13:26:33.000000 vastdb-0.1.6/vast_flatbuf/org/apache/arrow/flatbuf/LargeUtf8.py
--rw-rw-rw-   0 root         (0) root         (0)      993 2024-05-20 13:26:33.000000 vastdb-0.1.6/vast_flatbuf/org/apache/arrow/flatbuf/List.py
--rw-rw-rw-   0 root         (0) root         (0)     2541 2024-05-20 13:26:33.000000 vastdb-0.1.6/vast_flatbuf/org/apache/arrow/flatbuf/Map.py
--rw-rw-rw-   0 root         (0) root         (0)     4486 2024-05-20 13:26:33.000000 vastdb-0.1.6/vast_flatbuf/org/apache/arrow/flatbuf/Message.py
--rw-rw-rw-   0 root         (0) root         (0)      671 2024-05-20 13:26:33.000000 vastdb-0.1.6/vast_flatbuf/org/apache/arrow/flatbuf/MessageHeader.py
--rw-rw-rw-   0 root         (0) root         (0)      786 2024-05-20 13:26:33.000000 vastdb-0.1.6/vast_flatbuf/org/apache/arrow/flatbuf/MetadataVersion.py
--rw-rw-rw-   0 root         (0) root         (0)     1054 2024-05-20 13:26:33.000000 vastdb-0.1.6/vast_flatbuf/org/apache/arrow/flatbuf/Null.py
--rw-rw-rw-   0 root         (0) root         (0)      161 2024-05-20 13:26:33.000000 vastdb-0.1.6/vast_flatbuf/org/apache/arrow/flatbuf/Precision.py
--rw-rw-rw-   0 root         (0) root         (0)     5589 2024-05-20 13:26:33.000000 vastdb-0.1.6/vast_flatbuf/org/apache/arrow/flatbuf/RecordBatch.py
--rw-rw-rw-   0 root         (0) root         (0)     6042 2024-05-20 13:26:33.000000 vastdb-0.1.6/vast_flatbuf/org/apache/arrow/flatbuf/Schema.py
--rw-rw-rw-   0 root         (0) root         (0)      162 2024-05-20 13:26:33.000000 vastdb-0.1.6/vast_flatbuf/org/apache/arrow/flatbuf/SparseMatrixCompressedAxis.py
--rw-rw-rw-   0 root         (0) root         (0)     5785 2024-05-20 13:26:33.000000 vastdb-0.1.6/vast_flatbuf/org/apache/arrow/flatbuf/SparseMatrixIndexCSX.py
--rw-rw-rw-   0 root         (0) root         (0)     6091 2024-05-20 13:26:33.000000 vastdb-0.1.6/vast_flatbuf/org/apache/arrow/flatbuf/SparseTensor.py
--rw-rw-rw-   0 root         (0) root         (0)      226 2024-05-20 13:26:33.000000 vastdb-0.1.6/vast_flatbuf/org/apache/arrow/flatbuf/SparseTensorIndex.py
--rw-rw-rw-   0 root         (0) root         (0)     6389 2024-05-20 13:26:33.000000 vastdb-0.1.6/vast_flatbuf/org/apache/arrow/flatbuf/SparseTensorIndexCOO.py
--rw-rw-rw-   0 root         (0) root         (0)     9409 2024-05-20 13:26:33.000000 vastdb-0.1.6/vast_flatbuf/org/apache/arrow/flatbuf/SparseTensorIndexCSF.py
--rw-rw-rw-   0 root         (0) root         (0)     1193 2024-05-20 13:26:33.000000 vastdb-0.1.6/vast_flatbuf/org/apache/arrow/flatbuf/Struct_.py
--rw-rw-rw-   0 root         (0) root         (0)     5767 2024-05-20 13:26:33.000000 vastdb-0.1.6/vast_flatbuf/org/apache/arrow/flatbuf/Tensor.py
--rw-rw-rw-   0 root         (0) root         (0)     2149 2024-05-20 13:26:33.000000 vastdb-0.1.6/vast_flatbuf/org/apache/arrow/flatbuf/TensorDim.py
--rw-rw-rw-   0 root         (0) root         (0)     2639 2024-05-20 13:26:33.000000 vastdb-0.1.6/vast_flatbuf/org/apache/arrow/flatbuf/Time.py
--rw-rw-rw-   0 root         (0) root         (0)      191 2024-05-20 13:26:33.000000 vastdb-0.1.6/vast_flatbuf/org/apache/arrow/flatbuf/TimeUnit.py
--rw-rw-rw-   0 root         (0) root         (0)     7925 2024-05-20 13:26:33.000000 vastdb-0.1.6/vast_flatbuf/org/apache/arrow/flatbuf/Timestamp.py
--rw-rw-rw-   0 root         (0) root         (0)      698 2024-05-20 13:26:33.000000 vastdb-0.1.6/vast_flatbuf/org/apache/arrow/flatbuf/Type.py
--rw-rw-rw-   0 root         (0) root         (0)     3142 2024-05-20 13:26:33.000000 vastdb-0.1.6/vast_flatbuf/org/apache/arrow/flatbuf/Union.py
--rw-rw-rw-   0 root         (0) root         (0)      147 2024-05-20 13:26:33.000000 vastdb-0.1.6/vast_flatbuf/org/apache/arrow/flatbuf/UnionMode.py
--rw-rw-rw-   0 root         (0) root         (0)     1023 2024-05-20 13:26:33.000000 vastdb-0.1.6/vast_flatbuf/org/apache/arrow/flatbuf/Utf8.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-23 11:00:32.000000 vastdb-0.1.6/vast_flatbuf/org/apache/arrow/flatbuf/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 11:15:59.133398 vastdb-0.1.6/vast_flatbuf/tabular/
--rw-rw-rw-   0 root         (0) root         (0)     2114 2024-05-20 13:26:33.000000 vastdb-0.1.6/vast_flatbuf/tabular/AlterColumnRequest.py
--rw-rw-rw-   0 root         (0) root         (0)     2222 2024-05-20 13:26:33.000000 vastdb-0.1.6/vast_flatbuf/tabular/AlterProjectionTableRequest.py
--rw-rw-rw-   0 root         (0) root         (0)     1618 2024-05-20 13:26:33.000000 vastdb-0.1.6/vast_flatbuf/tabular/AlterSchemaRequest.py
--rw-rw-rw-   0 root         (0) root         (0)     1610 2024-05-20 13:26:33.000000 vastdb-0.1.6/vast_flatbuf/tabular/AlterTableRequest.py
--rw-rw-rw-   0 root         (0) root         (0)     1901 2024-05-20 13:26:33.000000 vastdb-0.1.6/vast_flatbuf/tabular/Column.py
--rw-rw-rw-   0 root         (0) root         (0)      151 2024-05-20 13:26:33.000000 vastdb-0.1.6/vast_flatbuf/tabular/ColumnType.py
--rw-rw-rw-   0 root         (0) root         (0)     2516 2024-05-20 13:26:33.000000 vastdb-0.1.6/vast_flatbuf/tabular/CreateProjectionRequest.py
--rw-rw-rw-   0 root         (0) root         (0)     1626 2024-05-20 13:26:33.000000 vastdb-0.1.6/vast_flatbuf/tabular/CreateSchemaRequest.py
--rw-rw-rw-   0 root         (0) root         (0)     3474 2024-05-20 13:26:33.000000 vastdb-0.1.6/vast_flatbuf/tabular/GetProjectionTableStatsResponse.py
--rw-rw-rw-   0 root         (0) root         (0)     4655 2024-05-20 13:26:33.000000 vastdb-0.1.6/vast_flatbuf/tabular/GetTableStatsResponse.py
--rw-rw-rw-   0 root         (0) root         (0)     2450 2024-05-20 13:26:33.000000 vastdb-0.1.6/vast_flatbuf/tabular/ImportDataRequest.py
--rw-rw-rw-   0 root         (0) root         (0)     4240 2024-05-20 13:26:33.000000 vastdb-0.1.6/vast_flatbuf/tabular/ListProjectionsResponse.py
--rw-rw-rw-   0 root         (0) root         (0)     3036 2024-05-20 13:26:33.000000 vastdb-0.1.6/vast_flatbuf/tabular/ListSchemasResponse.py
--rw-rw-rw-   0 root         (0) root         (0)     3550 2024-05-20 13:26:33.000000 vastdb-0.1.6/vast_flatbuf/tabular/ListTablesResponse.py
--rw-rw-rw-   0 root         (0) root         (0)     3589 2024-05-20 13:26:33.000000 vastdb-0.1.6/vast_flatbuf/tabular/ObjectDetails.py
--rw-rw-rw-   0 root         (0) root         (0)     4450 2024-05-20 13:26:33.000000 vastdb-0.1.6/vast_flatbuf/tabular/S3File.py
--rw-rw-rw-   0 root         (0) root         (0)     2069 2024-05-20 13:26:33.000000 vastdb-0.1.6/vast_flatbuf/tabular/VipRange.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-23 11:00:32.000000 vastdb-0.1.6/vast_flatbuf/tabular/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 11:15:59.135398 vastdb-0.1.6/vastdb/
--rw-rw-rw-   0 root         (0) root         (0)      292 2024-05-20 13:26:33.000000 vastdb-0.1.6/vastdb/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 11:15:59.137398 vastdb-0.1.6/vastdb/bench/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-23 11:00:32.000000 vastdb-0.1.6/vastdb/bench/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1084 2024-05-21 19:41:14.000000 vastdb-0.1.6/vastdb/bench/test_perf.py
--rw-rw-rw-   0 root         (0) root         (0)     2536 2024-05-21 19:41:14.000000 vastdb-0.1.6/vastdb/bucket.py
--rw-rw-rw-   0 root         (0) root         (0)     2359 2024-05-21 19:41:14.000000 vastdb-0.1.6/vastdb/conftest.py
--rw-rw-rw-   0 root         (0) root         (0)     4098 2024-05-21 19:41:14.000000 vastdb-0.1.6/vastdb/errors.py
--rw-rw-rw-   0 root         (0) root         (0)    97586 2024-05-23 11:00:32.000000 vastdb-0.1.6/vastdb/internal_commands.py
--rw-rw-rw-   0 root         (0) root         (0)     5642 2024-05-21 19:41:14.000000 vastdb-0.1.6/vastdb/schema.py
--rw-rw-rw-   0 root         (0) root         (0)     2984 2024-05-21 19:41:14.000000 vastdb-0.1.6/vastdb/session.py
--rw-rw-rw-   0 root         (0) root         (0)    30646 2024-05-21 19:41:14.000000 vastdb-0.1.6/vastdb/table.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 11:15:59.139398 vastdb-0.1.6/vastdb/tests/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-23 11:00:32.000000 vastdb-0.1.6/vastdb/tests/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1913 2024-05-20 13:26:33.000000 vastdb-0.1.6/vastdb/tests/test_duckdb.py
--rw-rw-rw-   0 root         (0) root         (0)     5669 2024-05-20 13:26:33.000000 vastdb-0.1.6/vastdb/tests/test_imports.py
--rw-rw-rw-   0 root         (0) root         (0)     3448 2024-05-20 13:26:33.000000 vastdb-0.1.6/vastdb/tests/test_nested.py
--rw-rw-rw-   0 root         (0) root         (0)     4223 2024-05-21 19:41:14.000000 vastdb-0.1.6/vastdb/tests/test_projections.py
--rw-rw-rw-   0 root         (0) root         (0)     2960 2024-05-20 13:26:33.000000 vastdb-0.1.6/vastdb/tests/test_sanity.py
--rw-rw-rw-   0 root         (0) root         (0)     3312 2024-05-21 19:41:14.000000 vastdb-0.1.6/vastdb/tests/test_schemas.py
--rw-rw-rw-   0 root         (0) root         (0)    28342 2024-05-21 19:41:14.000000 vastdb-0.1.6/vastdb/tests/test_tables.py
--rw-rw-rw-   0 root         (0) root         (0)     1046 2024-05-20 13:26:33.000000 vastdb-0.1.6/vastdb/tests/test_util.py
--rw-rw-rw-   0 root         (0) root         (0)      555 2024-05-20 13:26:33.000000 vastdb-0.1.6/vastdb/tests/util.py
--rw-rw-rw-   0 root         (0) root         (0)     3178 2024-05-20 13:26:33.000000 vastdb-0.1.6/vastdb/transaction.py
--rw-rw-rw-   0 root         (0) root         (0)     4342 2024-05-21 19:41:14.000000 vastdb-0.1.6/vastdb/util.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 11:15:59.139398 vastdb-0.1.6/vastdb.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1348 2024-05-23 11:15:59.000000 vastdb-0.1.6/vastdb.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     9048 2024-05-23 11:15:59.000000 vastdb-0.1.6/vastdb.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-05-23 11:15:59.000000 vastdb-0.1.6/vastdb.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      100 2024-05-23 11:15:59.000000 vastdb-0.1.6/vastdb.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       20 2024-05-23 11:15:59.000000 vastdb-0.1.6/vastdb.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-06-03 12:25:31.754987 vastdb-0.1.7/
+-rw-rw-rw-   0 root         (0) root         (0)     5988 2024-06-03 11:57:14.000000 vastdb-0.1.7/CHANGELOG.md
+-rw-rw-rw-   0 root         (0) root         (0)    11333 2024-06-03 11:57:14.000000 vastdb-0.1.7/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)       38 2024-06-03 11:57:14.000000 vastdb-0.1.7/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     1348 2024-06-03 12:25:31.754987 vastdb-0.1.7/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     6835 2024-06-03 11:57:14.000000 vastdb-0.1.7/README.md
+-rw-rw-rw-   0 root         (0) root         (0)      101 2024-06-03 11:57:14.000000 vastdb-0.1.7/requirements.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2024-06-03 12:25:31.754987 vastdb-0.1.7/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1728 2024-06-03 11:57:14.000000 vastdb-0.1.7/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-06-03 12:25:31.720987 vastdb-0.1.7/vast_flatbuf/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-06-03 11:57:14.000000 vastdb-0.1.7/vast_flatbuf/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-06-03 12:25:31.720987 vastdb-0.1.7/vast_flatbuf/org/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-06-03 11:57:14.000000 vastdb-0.1.7/vast_flatbuf/org/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-06-03 12:25:31.720987 vastdb-0.1.7/vast_flatbuf/org/apache/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-06-03 11:57:14.000000 vastdb-0.1.7/vast_flatbuf/org/apache/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-06-03 12:25:31.720987 vastdb-0.1.7/vast_flatbuf/org/apache/arrow/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-06-03 11:57:14.000000 vastdb-0.1.7/vast_flatbuf/org/apache/arrow/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-06-03 12:25:31.721987 vastdb-0.1.7/vast_flatbuf/org/apache/arrow/computeir/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-06-03 11:57:14.000000 vastdb-0.1.7/vast_flatbuf/org/apache/arrow/computeir/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-06-03 12:25:31.734987 vastdb-0.1.7/vast_flatbuf/org/apache/arrow/computeir/flatbuf/
+-rw-rw-rw-   0 root         (0) root         (0)     5630 2024-06-03 11:57:14.000000 vastdb-0.1.7/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Aggregate.py
+-rw-rw-rw-   0 root         (0) root         (0)     2212 2024-06-03 11:57:14.000000 vastdb-0.1.7/vast_flatbuf/org/apache/arrow/computeir/flatbuf/ArraySlice.py
+-rw-rw-rw-   0 root         (0) root         (0)     1567 2024-06-03 11:57:14.000000 vastdb-0.1.7/vast_flatbuf/org/apache/arrow/computeir/flatbuf/ArraySubscript.py
+-rw-rw-rw-   0 root         (0) root         (0)     2494 2024-06-03 11:57:14.000000 vastdb-0.1.7/vast_flatbuf/org/apache/arrow/computeir/flatbuf/BinaryLiteral.py
+-rw-rw-rw-   0 root         (0) root         (0)     1521 2024-06-03 11:57:14.000000 vastdb-0.1.7/vast_flatbuf/org/apache/arrow/computeir/flatbuf/BooleanLiteral.py
+-rw-rw-rw-   0 root         (0) root         (0)      182 2024-06-03 11:57:14.000000 vastdb-0.1.7/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Bound.py
+-rw-rw-rw-   0 root         (0) root         (0)     4434 2024-06-03 11:57:14.000000 vastdb-0.1.7/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Call.py
+-rw-rw-rw-   0 root         (0) root         (0)     2429 2024-06-03 11:57:14.000000 vastdb-0.1.7/vast_flatbuf/org/apache/arrow/computeir/flatbuf/CaseFragment.py
+-rw-rw-rw-   0 root         (0) root         (0)     2520 2024-06-03 11:57:14.000000 vastdb-0.1.7/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Cast.py
+-rw-rw-rw-   0 root         (0) root         (0)      236 2024-06-03 11:57:14.000000 vastdb-0.1.7/vast_flatbuf/org/apache/arrow/computeir/flatbuf/ConcreteBoundImpl.py
+-rw-rw-rw-   0 root         (0) root         (0)     3490 2024-06-03 11:57:14.000000 vastdb-0.1.7/vast_flatbuf/org/apache/arrow/computeir/flatbuf/ConditionalCase.py
+-rw-rw-rw-   0 root         (0) root         (0)     1059 2024-06-03 11:57:14.000000 vastdb-0.1.7/vast_flatbuf/org/apache/arrow/computeir/flatbuf/CurrentRow.py
+-rw-rw-rw-   0 root         (0) root         (0)     1489 2024-06-03 11:57:14.000000 vastdb-0.1.7/vast_flatbuf/org/apache/arrow/computeir/flatbuf/DateLiteral.py
+-rw-rw-rw-   0 root         (0) root         (0)     2576 2024-06-03 11:57:14.000000 vastdb-0.1.7/vast_flatbuf/org/apache/arrow/computeir/flatbuf/DecimalLiteral.py
+-rw-rw-rw-   0 root         (0) root         (0)      484 2024-06-03 11:57:14.000000 vastdb-0.1.7/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Deref.py
+-rw-rw-rw-   0 root         (0) root         (0)     1521 2024-06-03 11:57:14.000000 vastdb-0.1.7/vast_flatbuf/org/apache/arrow/computeir/flatbuf/DurationLiteral.py
+-rw-rw-rw-   0 root         (0) root         (0)     2258 2024-06-03 11:57:14.000000 vastdb-0.1.7/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Expression.py
+-rw-rw-rw-   0 root         (0) root         (0)      498 2024-06-03 11:57:14.000000 vastdb-0.1.7/vast_flatbuf/org/apache/arrow/computeir/flatbuf/ExpressionImpl.py
+-rw-rw-rw-   0 root         (0) root         (0)     1584 2024-06-03 11:57:14.000000 vastdb-0.1.7/vast_flatbuf/org/apache/arrow/computeir/flatbuf/FieldIndex.py
+-rw-rw-rw-   0 root         (0) root         (0)     2850 2024-06-03 11:57:14.000000 vastdb-0.1.7/vast_flatbuf/org/apache/arrow/computeir/flatbuf/FieldRef.py
+-rw-rw-rw-   0 root         (0) root         (0)     3260 2024-06-03 11:57:14.000000 vastdb-0.1.7/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Filter.py
+-rw-rw-rw-   0 root         (0) root         (0)     2602 2024-06-03 11:57:14.000000 vastdb-0.1.7/vast_flatbuf/org/apache/arrow/computeir/flatbuf/FixedSizeBinaryLiteral.py
+-rw-rw-rw-   0 root         (0) root         (0)     1515 2024-06-03 11:57:14.000000 vastdb-0.1.7/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Float16Literal.py
+-rw-rw-rw-   0 root         (0) root         (0)     1521 2024-06-03 11:57:14.000000 vastdb-0.1.7/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Float32Literal.py
+-rw-rw-rw-   0 root         (0) root         (0)     1521 2024-06-03 11:57:14.000000 vastdb-0.1.7/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Float64Literal.py
+-rw-rw-rw-   0 root         (0) root         (0)     2130 2024-06-03 11:57:14.000000 vastdb-0.1.7/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Following.py
+-rw-rw-rw-   0 root         (0) root         (0)      186 2024-06-03 11:57:14.000000 vastdb-0.1.7/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Frame.py
+-rw-rw-rw-   0 root         (0) root         (0)     2403 2024-06-03 11:57:14.000000 vastdb-0.1.7/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Grouping.py
+-rw-rw-rw-   0 root         (0) root         (0)     1497 2024-06-03 11:57:14.000000 vastdb-0.1.7/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Int16Literal.py
+-rw-rw-rw-   0 root         (0) root         (0)     1497 2024-06-03 11:57:14.000000 vastdb-0.1.7/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Int32Literal.py
+-rw-rw-rw-   0 root         (0) root         (0)     1497 2024-06-03 11:57:14.000000 vastdb-0.1.7/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Int64Literal.py
+-rw-rw-rw-   0 root         (0) root         (0)     1487 2024-06-03 11:57:14.000000 vastdb-0.1.7/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Int8Literal.py
+-rw-rw-rw-   0 root         (0) root         (0)     2139 2024-06-03 11:57:14.000000 vastdb-0.1.7/vast_flatbuf/org/apache/arrow/computeir/flatbuf/IntervalLiteral.py
+-rw-rw-rw-   0 root         (0) root         (0)     2197 2024-06-03 11:57:14.000000 vastdb-0.1.7/vast_flatbuf/org/apache/arrow/computeir/flatbuf/IntervalLiteralDaysMilliseconds.py
+-rw-rw-rw-   0 root         (0) root         (0)      211 2024-06-03 11:57:14.000000 vastdb-0.1.7/vast_flatbuf/org/apache/arrow/computeir/flatbuf/IntervalLiteralImpl.py
+-rw-rw-rw-   0 root         (0) root         (0)     1578 2024-06-03 11:57:14.000000 vastdb-0.1.7/vast_flatbuf/org/apache/arrow/computeir/flatbuf/IntervalLiteralMonths.py
+-rw-rw-rw-   0 root         (0) root         (0)     4455 2024-06-03 11:57:14.000000 vastdb-0.1.7/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Join.py
+-rw-rw-rw-   0 root         (0) root         (0)      230 2024-06-03 11:57:14.000000 vastdb-0.1.7/vast_flatbuf/org/apache/arrow/computeir/flatbuf/JoinKind.py
+-rw-rw-rw-   0 root         (0) root         (0)     2309 2024-06-03 11:57:14.000000 vastdb-0.1.7/vast_flatbuf/org/apache/arrow/computeir/flatbuf/KeyValue.py
+-rw-rw-rw-   0 root         (0) root         (0)     3368 2024-06-03 11:57:14.000000 vastdb-0.1.7/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Limit.py
+-rw-rw-rw-   0 root         (0) root         (0)     2400 2024-06-03 11:57:14.000000 vastdb-0.1.7/vast_flatbuf/org/apache/arrow/computeir/flatbuf/ListLiteral.py
+-rw-rw-rw-   0 root         (0) root         (0)     2797 2024-06-03 11:57:14.000000 vastdb-0.1.7/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Literal.py
+-rw-rw-rw-   0 root         (0) root         (0)     2526 2024-06-03 11:57:14.000000 vastdb-0.1.7/vast_flatbuf/org/apache/arrow/computeir/flatbuf/LiteralColumn.py
+-rw-rw-rw-   0 root         (0) root         (0)      682 2024-06-03 11:57:14.000000 vastdb-0.1.7/vast_flatbuf/org/apache/arrow/computeir/flatbuf/LiteralImpl.py
+-rw-rw-rw-   0 root         (0) root         (0)     3284 2024-06-03 11:57:14.000000 vastdb-0.1.7/vast_flatbuf/org/apache/arrow/computeir/flatbuf/LiteralRelation.py
+-rw-rw-rw-   0 root         (0) root         (0)     1723 2024-06-03 11:57:14.000000 vastdb-0.1.7/vast_flatbuf/org/apache/arrow/computeir/flatbuf/MapKey.py
+-rw-rw-rw-   0 root         (0) root         (0)     2392 2024-06-03 11:57:14.000000 vastdb-0.1.7/vast_flatbuf/org/apache/arrow/computeir/flatbuf/MapLiteral.py
+-rw-rw-rw-   0 root         (0) root         (0)     3847 2024-06-03 11:57:14.000000 vastdb-0.1.7/vast_flatbuf/org/apache/arrow/computeir/flatbuf/OrderBy.py
+-rw-rw-rw-   0 root         (0) root         (0)      349 2024-06-03 11:57:14.000000 vastdb-0.1.7/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Ordering.py
+-rw-rw-rw-   0 root         (0) root         (0)     2378 2024-06-03 11:57:14.000000 vastdb-0.1.7/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Plan.py
+-rw-rw-rw-   0 root         (0) root         (0)     2130 2024-06-03 11:57:14.000000 vastdb-0.1.7/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Preceding.py
+-rw-rw-rw-   0 root         (0) root         (0)     3941 2024-06-03 11:57:14.000000 vastdb-0.1.7/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Project.py
+-rw-rw-rw-   0 root         (0) root         (0)     1526 2024-06-03 11:57:14.000000 vastdb-0.1.7/vast_flatbuf/org/apache/arrow/computeir/flatbuf/RelId.py
+-rw-rw-rw-   0 root         (0) root         (0)     2113 2024-06-03 11:57:14.000000 vastdb-0.1.7/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Relation.py
+-rw-rw-rw-   0 root         (0) root         (0)      315 2024-06-03 11:57:14.000000 vastdb-0.1.7/vast_flatbuf/org/apache/arrow/computeir/flatbuf/RelationImpl.py
+-rw-rw-rw-   0 root         (0) root         (0)      217 2024-06-03 11:57:14.000000 vastdb-0.1.7/vast_flatbuf/org/apache/arrow/computeir/flatbuf/SetOpKind.py
+-rw-rw-rw-   0 root         (0) root         (0)     3678 2024-06-03 11:57:14.000000 vastdb-0.1.7/vast_flatbuf/org/apache/arrow/computeir/flatbuf/SetOperation.py
+-rw-rw-rw-   0 root         (0) root         (0)     3952 2024-06-03 11:57:14.000000 vastdb-0.1.7/vast_flatbuf/org/apache/arrow/computeir/flatbuf/SimpleCase.py
+-rw-rw-rw-   0 root         (0) root         (0)     2221 2024-06-03 11:57:14.000000 vastdb-0.1.7/vast_flatbuf/org/apache/arrow/computeir/flatbuf/SortKey.py
+-rw-rw-rw-   0 root         (0) root         (0)     5650 2024-06-03 11:57:14.000000 vastdb-0.1.7/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Source.py
+-rw-rw-rw-   0 root         (0) root         (0)     1533 2024-06-03 11:57:14.000000 vastdb-0.1.7/vast_flatbuf/org/apache/arrow/computeir/flatbuf/StringLiteral.py
+-rw-rw-rw-   0 root         (0) root         (0)     1593 2024-06-03 11:57:14.000000 vastdb-0.1.7/vast_flatbuf/org/apache/arrow/computeir/flatbuf/StructField.py
+-rw-rw-rw-   0 root         (0) root         (0)     2539 2024-06-03 11:57:14.000000 vastdb-0.1.7/vast_flatbuf/org/apache/arrow/computeir/flatbuf/StructLiteral.py
+-rw-rw-rw-   0 root         (0) root         (0)     1489 2024-06-03 11:57:14.000000 vastdb-0.1.7/vast_flatbuf/org/apache/arrow/computeir/flatbuf/TimeLiteral.py
+-rw-rw-rw-   0 root         (0) root         (0)     1529 2024-06-03 11:57:14.000000 vastdb-0.1.7/vast_flatbuf/org/apache/arrow/computeir/flatbuf/TimestampLiteral.py
+-rw-rw-rw-   0 root         (0) root         (0)     1507 2024-06-03 11:57:14.000000 vastdb-0.1.7/vast_flatbuf/org/apache/arrow/computeir/flatbuf/UInt16Literal.py
+-rw-rw-rw-   0 root         (0) root         (0)     1507 2024-06-03 11:57:14.000000 vastdb-0.1.7/vast_flatbuf/org/apache/arrow/computeir/flatbuf/UInt32Literal.py
+-rw-rw-rw-   0 root         (0) root         (0)     1507 2024-06-03 11:57:14.000000 vastdb-0.1.7/vast_flatbuf/org/apache/arrow/computeir/flatbuf/UInt64Literal.py
+-rw-rw-rw-   0 root         (0) root         (0)     1497 2024-06-03 11:57:14.000000 vastdb-0.1.7/vast_flatbuf/org/apache/arrow/computeir/flatbuf/UInt8Literal.py
+-rw-rw-rw-   0 root         (0) root         (0)     1051 2024-06-03 11:57:14.000000 vastdb-0.1.7/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Unbounded.py
+-rw-rw-rw-   0 root         (0) root         (0)     7527 2024-06-03 11:57:14.000000 vastdb-0.1.7/vast_flatbuf/org/apache/arrow/computeir/flatbuf/WindowCall.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-06-03 11:57:14.000000 vastdb-0.1.7/vast_flatbuf/org/apache/arrow/computeir/flatbuf/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-06-03 12:25:31.745987 vastdb-0.1.7/vast_flatbuf/org/apache/arrow/flatbuf/
+-rw-rw-rw-   0 root         (0) root         (0)     1026 2024-06-03 11:57:14.000000 vastdb-0.1.7/vast_flatbuf/org/apache/arrow/flatbuf/Binary.py
+-rw-rw-rw-   0 root         (0) root         (0)     1326 2024-06-03 11:57:14.000000 vastdb-0.1.7/vast_flatbuf/org/apache/arrow/flatbuf/Block.py
+-rw-rw-rw-   0 root         (0) root         (0)     2310 2024-06-03 11:57:14.000000 vastdb-0.1.7/vast_flatbuf/org/apache/arrow/flatbuf/BodyCompression.py
+-rw-rw-rw-   0 root         (0) root         (0)      836 2024-06-03 11:57:14.000000 vastdb-0.1.7/vast_flatbuf/org/apache/arrow/flatbuf/BodyCompressionMethod.py
+-rw-rw-rw-   0 root         (0) root         (0)      993 2024-06-03 11:57:14.000000 vastdb-0.1.7/vast_flatbuf/org/apache/arrow/flatbuf/Bool.py
+-rw-rw-rw-   0 root         (0) root         (0)     1430 2024-06-03 11:57:14.000000 vastdb-0.1.7/vast_flatbuf/org/apache/arrow/flatbuf/Buffer.py
+-rw-rw-rw-   0 root         (0) root         (0)      155 2024-06-03 11:57:14.000000 vastdb-0.1.7/vast_flatbuf/org/apache/arrow/flatbuf/CompressionType.py
+-rw-rw-rw-   0 root         (0) root         (0)     1760 2024-06-03 11:57:14.000000 vastdb-0.1.7/vast_flatbuf/org/apache/arrow/flatbuf/Date.py
+-rw-rw-rw-   0 root         (0) root         (0)      149 2024-06-03 11:57:14.000000 vastdb-0.1.7/vast_flatbuf/org/apache/arrow/flatbuf/DateUnit.py
+-rw-rw-rw-   0 root         (0) root         (0)     2855 2024-06-03 11:57:14.000000 vastdb-0.1.7/vast_flatbuf/org/apache/arrow/flatbuf/Decimal.py
+-rw-rw-rw-   0 root         (0) root         (0)     3148 2024-06-03 11:57:14.000000 vastdb-0.1.7/vast_flatbuf/org/apache/arrow/flatbuf/DictionaryBatch.py
+-rw-rw-rw-   0 root         (0) root         (0)     4091 2024-06-03 11:57:14.000000 vastdb-0.1.7/vast_flatbuf/org/apache/arrow/flatbuf/DictionaryEncoding.py
+-rw-rw-rw-   0 root         (0) root         (0)      410 2024-06-03 11:57:14.000000 vastdb-0.1.7/vast_flatbuf/org/apache/arrow/flatbuf/DictionaryKind.py
+-rw-rw-rw-   0 root         (0) root         (0)     1456 2024-06-03 11:57:14.000000 vastdb-0.1.7/vast_flatbuf/org/apache/arrow/flatbuf/Duration.py
+-rw-rw-rw-   0 root         (0) root         (0)      267 2024-06-03 11:57:14.000000 vastdb-0.1.7/vast_flatbuf/org/apache/arrow/flatbuf/Endianness.py
+-rw-rw-rw-   0 root         (0) root         (0)     1289 2024-06-03 11:57:14.000000 vastdb-0.1.7/vast_flatbuf/org/apache/arrow/flatbuf/Feature.py
+-rw-rw-rw-   0 root         (0) root         (0)     7048 2024-06-03 11:57:14.000000 vastdb-0.1.7/vast_flatbuf/org/apache/arrow/flatbuf/Field.py
+-rw-rw-rw-   0 root         (0) root         (0)     1669 2024-06-03 11:57:14.000000 vastdb-0.1.7/vast_flatbuf/org/apache/arrow/flatbuf/FieldNode.py
+-rw-rw-rw-   0 root         (0) root         (0)     1589 2024-06-03 11:57:14.000000 vastdb-0.1.7/vast_flatbuf/org/apache/arrow/flatbuf/FixedSizeBinary.py
+-rw-rw-rw-   0 root         (0) root         (0)     1569 2024-06-03 11:57:14.000000 vastdb-0.1.7/vast_flatbuf/org/apache/arrow/flatbuf/FixedSizeList.py
+-rw-rw-rw-   0 root         (0) root         (0)     1541 2024-06-03 11:57:14.000000 vastdb-0.1.7/vast_flatbuf/org/apache/arrow/flatbuf/FloatingPoint.py
+-rw-rw-rw-   0 root         (0) root         (0)     6448 2024-06-03 11:57:14.000000 vastdb-0.1.7/vast_flatbuf/org/apache/arrow/flatbuf/Footer.py
+-rw-rw-rw-   0 root         (0) root         (0)     1925 2024-06-03 11:57:14.000000 vastdb-0.1.7/vast_flatbuf/org/apache/arrow/flatbuf/Int.py
+-rw-rw-rw-   0 root         (0) root         (0)     1456 2024-06-03 11:57:14.000000 vastdb-0.1.7/vast_flatbuf/org/apache/arrow/flatbuf/Interval.py
+-rw-rw-rw-   0 root         (0) root         (0)      180 2024-06-03 11:57:14.000000 vastdb-0.1.7/vast_flatbuf/org/apache/arrow/flatbuf/IntervalUnit.py
+-rw-rw-rw-   0 root         (0) root         (0)     2139 2024-06-03 11:57:14.000000 vastdb-0.1.7/vast_flatbuf/org/apache/arrow/flatbuf/KeyValue.py
+-rw-rw-rw-   0 root         (0) root         (0)     1131 2024-06-03 11:57:14.000000 vastdb-0.1.7/vast_flatbuf/org/apache/arrow/flatbuf/LargeBinary.py
+-rw-rw-rw-   0 root         (0) root         (0)     1117 2024-06-03 11:57:14.000000 vastdb-0.1.7/vast_flatbuf/org/apache/arrow/flatbuf/LargeList.py
+-rw-rw-rw-   0 root         (0) root         (0)     1117 2024-06-03 11:57:14.000000 vastdb-0.1.7/vast_flatbuf/org/apache/arrow/flatbuf/LargeUtf8.py
+-rw-rw-rw-   0 root         (0) root         (0)      993 2024-06-03 11:57:14.000000 vastdb-0.1.7/vast_flatbuf/org/apache/arrow/flatbuf/List.py
+-rw-rw-rw-   0 root         (0) root         (0)     2541 2024-06-03 11:57:14.000000 vastdb-0.1.7/vast_flatbuf/org/apache/arrow/flatbuf/Map.py
+-rw-rw-rw-   0 root         (0) root         (0)     4486 2024-06-03 11:57:14.000000 vastdb-0.1.7/vast_flatbuf/org/apache/arrow/flatbuf/Message.py
+-rw-rw-rw-   0 root         (0) root         (0)      671 2024-06-03 11:57:14.000000 vastdb-0.1.7/vast_flatbuf/org/apache/arrow/flatbuf/MessageHeader.py
+-rw-rw-rw-   0 root         (0) root         (0)      786 2024-06-03 11:57:14.000000 vastdb-0.1.7/vast_flatbuf/org/apache/arrow/flatbuf/MetadataVersion.py
+-rw-rw-rw-   0 root         (0) root         (0)     1054 2024-06-03 11:57:14.000000 vastdb-0.1.7/vast_flatbuf/org/apache/arrow/flatbuf/Null.py
+-rw-rw-rw-   0 root         (0) root         (0)      161 2024-06-03 11:57:14.000000 vastdb-0.1.7/vast_flatbuf/org/apache/arrow/flatbuf/Precision.py
+-rw-rw-rw-   0 root         (0) root         (0)     5589 2024-06-03 11:57:14.000000 vastdb-0.1.7/vast_flatbuf/org/apache/arrow/flatbuf/RecordBatch.py
+-rw-rw-rw-   0 root         (0) root         (0)     6042 2024-06-03 11:57:14.000000 vastdb-0.1.7/vast_flatbuf/org/apache/arrow/flatbuf/Schema.py
+-rw-rw-rw-   0 root         (0) root         (0)      162 2024-06-03 11:57:14.000000 vastdb-0.1.7/vast_flatbuf/org/apache/arrow/flatbuf/SparseMatrixCompressedAxis.py
+-rw-rw-rw-   0 root         (0) root         (0)     5785 2024-06-03 11:57:14.000000 vastdb-0.1.7/vast_flatbuf/org/apache/arrow/flatbuf/SparseMatrixIndexCSX.py
+-rw-rw-rw-   0 root         (0) root         (0)     6091 2024-06-03 11:57:14.000000 vastdb-0.1.7/vast_flatbuf/org/apache/arrow/flatbuf/SparseTensor.py
+-rw-rw-rw-   0 root         (0) root         (0)      226 2024-06-03 11:57:14.000000 vastdb-0.1.7/vast_flatbuf/org/apache/arrow/flatbuf/SparseTensorIndex.py
+-rw-rw-rw-   0 root         (0) root         (0)     6389 2024-06-03 11:57:14.000000 vastdb-0.1.7/vast_flatbuf/org/apache/arrow/flatbuf/SparseTensorIndexCOO.py
+-rw-rw-rw-   0 root         (0) root         (0)     9409 2024-06-03 11:57:14.000000 vastdb-0.1.7/vast_flatbuf/org/apache/arrow/flatbuf/SparseTensorIndexCSF.py
+-rw-rw-rw-   0 root         (0) root         (0)     1193 2024-06-03 11:57:14.000000 vastdb-0.1.7/vast_flatbuf/org/apache/arrow/flatbuf/Struct_.py
+-rw-rw-rw-   0 root         (0) root         (0)     5767 2024-06-03 11:57:14.000000 vastdb-0.1.7/vast_flatbuf/org/apache/arrow/flatbuf/Tensor.py
+-rw-rw-rw-   0 root         (0) root         (0)     2149 2024-06-03 11:57:14.000000 vastdb-0.1.7/vast_flatbuf/org/apache/arrow/flatbuf/TensorDim.py
+-rw-rw-rw-   0 root         (0) root         (0)     2639 2024-06-03 11:57:14.000000 vastdb-0.1.7/vast_flatbuf/org/apache/arrow/flatbuf/Time.py
+-rw-rw-rw-   0 root         (0) root         (0)      191 2024-06-03 11:57:14.000000 vastdb-0.1.7/vast_flatbuf/org/apache/arrow/flatbuf/TimeUnit.py
+-rw-rw-rw-   0 root         (0) root         (0)     7925 2024-06-03 11:57:14.000000 vastdb-0.1.7/vast_flatbuf/org/apache/arrow/flatbuf/Timestamp.py
+-rw-rw-rw-   0 root         (0) root         (0)      698 2024-06-03 11:57:14.000000 vastdb-0.1.7/vast_flatbuf/org/apache/arrow/flatbuf/Type.py
+-rw-rw-rw-   0 root         (0) root         (0)     3142 2024-06-03 11:57:14.000000 vastdb-0.1.7/vast_flatbuf/org/apache/arrow/flatbuf/Union.py
+-rw-rw-rw-   0 root         (0) root         (0)      147 2024-06-03 11:57:14.000000 vastdb-0.1.7/vast_flatbuf/org/apache/arrow/flatbuf/UnionMode.py
+-rw-rw-rw-   0 root         (0) root         (0)     1023 2024-06-03 11:57:14.000000 vastdb-0.1.7/vast_flatbuf/org/apache/arrow/flatbuf/Utf8.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-06-03 11:57:14.000000 vastdb-0.1.7/vast_flatbuf/org/apache/arrow/flatbuf/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-06-03 12:25:31.748987 vastdb-0.1.7/vast_flatbuf/tabular/
+-rw-rw-rw-   0 root         (0) root         (0)     2114 2024-06-03 11:57:14.000000 vastdb-0.1.7/vast_flatbuf/tabular/AlterColumnRequest.py
+-rw-rw-rw-   0 root         (0) root         (0)     2222 2024-06-03 11:57:14.000000 vastdb-0.1.7/vast_flatbuf/tabular/AlterProjectionTableRequest.py
+-rw-rw-rw-   0 root         (0) root         (0)     1618 2024-06-03 11:57:14.000000 vastdb-0.1.7/vast_flatbuf/tabular/AlterSchemaRequest.py
+-rw-rw-rw-   0 root         (0) root         (0)     1610 2024-06-03 11:57:14.000000 vastdb-0.1.7/vast_flatbuf/tabular/AlterTableRequest.py
+-rw-rw-rw-   0 root         (0) root         (0)     1901 2024-06-03 11:57:14.000000 vastdb-0.1.7/vast_flatbuf/tabular/Column.py
+-rw-rw-rw-   0 root         (0) root         (0)      151 2024-06-03 11:57:14.000000 vastdb-0.1.7/vast_flatbuf/tabular/ColumnType.py
+-rw-rw-rw-   0 root         (0) root         (0)     2516 2024-06-03 11:57:14.000000 vastdb-0.1.7/vast_flatbuf/tabular/CreateProjectionRequest.py
+-rw-rw-rw-   0 root         (0) root         (0)     1626 2024-06-03 11:57:14.000000 vastdb-0.1.7/vast_flatbuf/tabular/CreateSchemaRequest.py
+-rw-rw-rw-   0 root         (0) root         (0)     3474 2024-06-03 11:57:14.000000 vastdb-0.1.7/vast_flatbuf/tabular/GetProjectionTableStatsResponse.py
+-rw-rw-rw-   0 root         (0) root         (0)     4655 2024-06-03 11:57:14.000000 vastdb-0.1.7/vast_flatbuf/tabular/GetTableStatsResponse.py
+-rw-rw-rw-   0 root         (0) root         (0)     2450 2024-06-03 11:57:14.000000 vastdb-0.1.7/vast_flatbuf/tabular/ImportDataRequest.py
+-rw-rw-rw-   0 root         (0) root         (0)     4240 2024-06-03 11:57:14.000000 vastdb-0.1.7/vast_flatbuf/tabular/ListProjectionsResponse.py
+-rw-rw-rw-   0 root         (0) root         (0)     3036 2024-06-03 11:57:14.000000 vastdb-0.1.7/vast_flatbuf/tabular/ListSchemasResponse.py
+-rw-rw-rw-   0 root         (0) root         (0)     3550 2024-06-03 11:57:14.000000 vastdb-0.1.7/vast_flatbuf/tabular/ListTablesResponse.py
+-rw-rw-rw-   0 root         (0) root         (0)     3589 2024-06-03 11:57:14.000000 vastdb-0.1.7/vast_flatbuf/tabular/ObjectDetails.py
+-rw-rw-rw-   0 root         (0) root         (0)     4450 2024-06-03 11:57:14.000000 vastdb-0.1.7/vast_flatbuf/tabular/S3File.py
+-rw-rw-rw-   0 root         (0) root         (0)     2069 2024-06-03 11:57:14.000000 vastdb-0.1.7/vast_flatbuf/tabular/VipRange.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-06-03 11:57:14.000000 vastdb-0.1.7/vast_flatbuf/tabular/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-06-03 12:25:31.750987 vastdb-0.1.7/vastdb/
+-rw-rw-rw-   0 root         (0) root         (0)      386 2024-06-03 11:57:14.000000 vastdb-0.1.7/vastdb/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    89095 2024-06-03 11:57:14.000000 vastdb-0.1.7/vastdb/_internal.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-06-03 12:25:31.751987 vastdb-0.1.7/vastdb/bench/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-06-03 11:57:14.000000 vastdb-0.1.7/vastdb/bench/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1084 2024-06-03 11:57:14.000000 vastdb-0.1.7/vastdb/bench/test_perf.py
+-rw-rw-rw-   0 root         (0) root         (0)     2544 2024-06-03 11:57:14.000000 vastdb-0.1.7/vastdb/bucket.py
+-rw-rw-rw-   0 root         (0) root         (0)     2359 2024-06-03 11:57:14.000000 vastdb-0.1.7/vastdb/conftest.py
+-rw-rw-rw-   0 root         (0) root         (0)     4098 2024-06-03 11:57:14.000000 vastdb-0.1.7/vastdb/errors.py
+-rw-rw-rw-   0 root         (0) root         (0)     5913 2024-06-03 11:57:14.000000 vastdb-0.1.7/vastdb/schema.py
+-rw-rw-rw-   0 root         (0) root         (0)     3349 2024-06-03 11:57:14.000000 vastdb-0.1.7/vastdb/session.py
+-rw-rw-rw-   0 root         (0) root         (0)    31047 2024-06-03 11:57:14.000000 vastdb-0.1.7/vastdb/table.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-06-03 12:25:31.753987 vastdb-0.1.7/vastdb/tests/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-06-03 11:57:14.000000 vastdb-0.1.7/vastdb/tests/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1880 2024-06-03 11:57:14.000000 vastdb-0.1.7/vastdb/tests/test_duckdb.py
+-rw-rw-rw-   0 root         (0) root         (0)     5669 2024-06-03 11:57:14.000000 vastdb-0.1.7/vastdb/tests/test_imports.py
+-rw-rw-rw-   0 root         (0) root         (0)     3448 2024-06-03 11:57:14.000000 vastdb-0.1.7/vastdb/tests/test_nested.py
+-rw-rw-rw-   0 root         (0) root         (0)     4223 2024-06-03 11:57:14.000000 vastdb-0.1.7/vastdb/tests/test_projections.py
+-rw-rw-rw-   0 root         (0) root         (0)     3054 2024-06-03 11:57:14.000000 vastdb-0.1.7/vastdb/tests/test_sanity.py
+-rw-rw-rw-   0 root         (0) root         (0)     3312 2024-06-03 11:57:14.000000 vastdb-0.1.7/vastdb/tests/test_schemas.py
+-rw-rw-rw-   0 root         (0) root         (0)    30124 2024-06-03 11:57:14.000000 vastdb-0.1.7/vastdb/tests/test_tables.py
+-rw-rw-rw-   0 root         (0) root         (0)     1260 2024-06-03 11:57:14.000000 vastdb-0.1.7/vastdb/tests/test_util.py
+-rw-rw-rw-   0 root         (0) root         (0)      555 2024-06-03 11:57:14.000000 vastdb-0.1.7/vastdb/tests/util.py
+-rw-rw-rw-   0 root         (0) root         (0)     3186 2024-06-03 11:57:14.000000 vastdb-0.1.7/vastdb/transaction.py
+-rw-rw-rw-   0 root         (0) root         (0)     5684 2024-06-03 11:57:14.000000 vastdb-0.1.7/vastdb/util.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-06-03 12:25:31.753987 vastdb-0.1.7/vastdb.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1348 2024-06-03 12:25:31.000000 vastdb-0.1.7/vastdb.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     9040 2024-06-03 12:25:31.000000 vastdb-0.1.7/vastdb.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-06-03 12:25:31.000000 vastdb-0.1.7/vastdb.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      100 2024-06-03 12:25:31.000000 vastdb-0.1.7/vastdb.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       20 2024-06-03 12:25:31.000000 vastdb-0.1.7/vastdb.egg-info/top_level.txt
```

### Comparing `vastdb-0.1.6/CHANGELOG.md` & `vastdb-0.1.7/CHANGELOG.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,39 @@
 # Changelog
 
 All notable changes to this project will be documented in this file.
 
 The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/).
 
+## [0.1.7] (2024-06-03)
+[0.1.7]: https://github.com/vast-data/vastdb_sdk/compare/v0.1.6...v0.1.7
+
+## Added
+ - Retry idempotent requests in case of retriable errors
+ - Allow setting `Table.select()` RPC queue priority
+ - Send SDK version via Tabular RPC
+ - Support external row IDs allocation
+ - Document required VAST release
+ - Add a helper function for defining a range of VIPs
+
+## Changed
+ - Update `ibis-framework` dependency to 9.0.0
+ - Refactor internal RPC client to support retries
+ - Refactor request invocation and result handling
+
+## Fixed
+ - Sort record batch according to internal row ID column for updates/deletes
+ - Don't use `ListBuckets` RPC to probe for server's version
+ - Don't fail on an empty batch
+ - Don't use 'us-east-1' region name
+
+## Removed
+ - Remove unused internal methods
+
+
 ## [0.1.6] (2024-05-23)
 [0.1.6]: https://github.com/vast-data/vastdb_sdk/compare/v0.1.5...v0.1.6
 
 ### Added
  - Allow listing and querying Catalog snapshots
  - Support nested schemas
  - Use automatic split estimation
```

### Comparing `vastdb-0.1.6/LICENSE` & `vastdb-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.6/PKG-INFO` & `vastdb-0.1.7/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vastdb
-Version: 0.1.6
+Version: 0.1.7
 Summary: VAST Data SDK
 Home-page: https://github.com/vast-data/vastdb_sdk
 Author: VAST DATA
 Author-email: hello@vastdata.com
 License: Copyright (C) VAST Data Ltd.
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: Apache Software License
@@ -17,15 +17,15 @@
 Classifier: Topic :: Database :: Front-Ends
 Requires-Python: >=3.9.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: aws-requests-auth
 Requires-Dist: boto3
 Requires-Dist: flatbuffers
-Requires-Dist: ibis-framework==8.0.0
+Requires-Dist: ibis-framework==9.0.0
 Requires-Dist: pyarrow
 Requires-Dist: requests
 Requires-Dist: xmltodict
 Requires-Dist: backoff==2.2.1
 
 
 `vastdb` is a Python-based SDK designed for interacting
```

### Comparing `vastdb-0.1.6/README.md` & `vastdb-0.1.7/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -128,251 +128,301 @@
 000007f0: 5b31 3131 2c20 3232 322c 2033 3333 5d2c  [111, 222, 333],
 00000800: 0a20 2020 2020 2020 205b 302e 352c 2031  .        [0.5, 1
 00000810: 2e35 2c20 322e 355d 2c0a 2020 2020 2020  .5, 2.5],.      
 00000820: 2020 5b27 6127 2c20 2762 6227 2c20 2763    ['a', 'bb', 'c
 00000830: 6363 275d 2c0a 2020 2020 5d29 0a20 2020  cc'],.    ]).   
 00000840: 2074 6162 6c65 2e69 6e73 6572 7428 6172   table.insert(ar
 00000850: 726f 775f 7461 626c 6529 0a0a 2020 2020  row_table)..    
-00000860: 7265 7375 6c74 203d 2070 612e 5461 626c  result = pa.Tabl
-00000870: 652e 6672 6f6d 5f62 6174 6368 6573 2874  e.from_batches(t
-00000880: 6162 6c65 2e73 656c 6563 7428 2929 2020  able.select())  
-00000890: 2320 5345 4c45 4354 202a 2046 524f 4d20  # SELECT * FROM 
-000008a0: 740a 2020 2020 6173 7365 7274 2072 6573  t.    assert res
-000008b0: 756c 7420 3d3d 2061 7272 6f77 5f74 6162  ult == arrow_tab
-000008c0: 6c65 0a0a 2020 2020 2320 7468 6520 7472  le..    # the tr
-000008d0: 616e 7361 6374 696f 6e20 6973 2061 7574  ansaction is aut
-000008e0: 6f6d 6174 6963 616c 6c79 2063 6f6d 6d69  omatically commi
-000008f0: 7474 6564 2077 6865 6e20 6578 6974 696e  tted when exitin
-00000900: 6720 7468 6520 636f 6e74 6578 740a 6060  g the context.``
-00000910: 600a 0a23 2320 4669 6c74 6572 7320 616e  `..## Filters an
-00000920: 6420 7072 6f6a 6563 7469 6f6e 730a 0a4f  d projections..O
-00000930: 7572 2053 444b 2073 7570 706f 7274 7320  ur SDK supports 
-00000940: 7072 6564 6963 6174 6520 616e 6420 7072  predicate and pr
-00000950: 6f6a 6563 7469 6f6e 2070 7573 6864 6f77  ojection pushdow
-00000960: 6e3a 0a0a 6060 6070 7974 686f 6e0a 2020  n:..```python.  
-00000970: 2020 6672 6f6d 2069 6269 7320 696d 706f    from ibis impo
-00000980: 7274 205f 0a0a 2020 2020 2320 5345 4c45  rt _..    # SELE
-00000990: 4354 2063 3120 4652 4f4d 2074 2057 4845  CT c1 FROM t WHE
-000009a0: 5245 2028 6332 203e 2032 2920 414e 4420  RE (c2 > 2) AND 
-000009b0: 2863 3320 4953 204e 554c 4c29 0a20 2020  (c3 IS NULL).   
-000009c0: 2074 6162 6c65 2e73 656c 6563 7428 636f   table.select(co
-000009d0: 6c75 6d6e 733d 5b27 6331 275d 2c0a 2020  lumns=['c1'],.  
-000009e0: 2020 2020 2020 2020 2020 2020 2020 2070                 p
-000009f0: 7265 6469 6361 7465 3d28 5f2e 6332 203e  redicate=(_.c2 >
-00000a00: 2032 2920 2620 5f2e 6333 2e69 736e 756c   2) & _.c3.isnul
-00000a10: 6c28 2929 0a0a 2020 2020 2320 5345 4c45  l())..    # SELE
-00000a20: 4354 2063 322c 2063 3320 4652 4f4d 2074  CT c2, c3 FROM t
-00000a30: 2057 4845 5245 2028 6332 2042 4554 5745   WHERE (c2 BETWE
-00000a40: 454e 2030 2041 4e44 2031 2920 4f52 2028  EN 0 AND 1) OR (
-00000a50: 6332 203e 2031 3029 0a20 2020 2074 6162  c2 > 10).    tab
-00000a60: 6c65 2e73 656c 6563 7428 636f 6c75 6d6e  le.select(column
-00000a70: 733d 5b27 6332 272c 2027 6333 275d 2c0a  s=['c2', 'c3'],.
-00000a80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000a90: 2070 7265 6469 6361 7465 3d28 5f2e 6332   predicate=(_.c2
-00000aa0: 2e62 6574 7765 656e 2830 2c20 3129 207c  .between(0, 1) |
-00000ab0: 2028 7461 626c 655b 2763 3227 5d20 3e20   (table['c2'] > 
-00000ac0: 3130 2929 0a0a 2020 2020 2320 5345 4c45  10))..    # SELE
-00000ad0: 4354 202a 2046 524f 4d20 7420 5748 4552  CT * FROM t WHER
-00000ae0: 4520 6333 204c 494b 4520 2725 7375 6273  E c3 LIKE '%subs
-00000af0: 7472 696e 6725 270a 2020 2020 7461 626c  tring%'.    tabl
-00000b00: 652e 7365 6c65 6374 2870 7265 6469 6361  e.select(predica
-00000b10: 7465 3d5f 2e63 332e 636f 6e74 6169 6e73  te=_.c3.contains
-00000b20: 2827 7375 6273 7472 696e 6727 2929 0a60  ('substring')).`
-00000b30: 6060 0a0a 5365 6520 5b68 6572 6520 666f  ``..See [here fo
-00000b40: 7220 6d6f 7265 2064 6574 6169 6c73 5d28  r more details](
-00000b50: 646f 6373 2f70 7265 6469 6361 7465 2e6d  docs/predicate.m
-00000b60: 6429 2e0a 0a23 2320 496d 706f 7274 2061  d)...## Import a
-00000b70: 2073 696e 676c 6520 5061 7271 7565 7420   single Parquet 
-00000b80: 6669 6c65 2076 6961 2053 3320 7072 6f74  file via S3 prot
-00000b90: 6f63 6f6c 0a0a 4974 2069 7320 706f 7373  ocol..It is poss
-00000ba0: 6962 6c65 2074 6f20 6566 6669 6369 656e  ible to efficien
-00000bb0: 746c 7920 6372 6561 7465 2061 2074 6162  tly create a tab
-00000bc0: 6c65 2066 726f 6d20 6120 5061 7271 7565  le from a Parque
-00000bd0: 7420 6669 6c65 2028 7769 7468 6f75 7420  t file (without 
-00000be0: 636f 7079 696e 6720 6974 2076 6961 2074  copying it via t
-00000bf0: 6865 2063 6c69 656e 7429 3a0a 0a60 6060  he client):..```
-00000c00: 7079 7468 6f6e 0a20 2020 2077 6974 6820  python.    with 
-00000c10: 7465 6d70 6669 6c65 2e4e 616d 6564 5465  tempfile.NamedTe
-00000c20: 6d70 6f72 6172 7946 696c 6528 2920 6173  mporaryFile() as
-00000c30: 2066 3a0a 2020 2020 2020 2020 7061 2e70   f:.        pa.p
-00000c40: 6172 7175 6574 2e77 7269 7465 5f74 6162  arquet.write_tab
-00000c50: 6c65 2861 7272 6f77 5f74 6162 6c65 2c20  le(arrow_table, 
-00000c60: 662e 6e61 6d65 290a 2020 2020 2020 2020  f.name).        
-00000c70: 7333 2e70 7574 5f6f 626a 6563 7428 4275  s3.put_object(Bu
-00000c80: 636b 6574 3d27 6275 636b 6574 2d6e 616d  cket='bucket-nam
-00000c90: 6527 2c20 4b65 793d 2773 7461 6769 6e67  e', Key='staging
-00000ca0: 2f66 696c 652e 7061 7271 7565 7427 2c20  /file.parquet', 
-00000cb0: 426f 6479 3d66 290a 0a20 2020 2073 6368  Body=f)..    sch
-00000cc0: 656d 6120 3d20 7478 2e62 7563 6b65 7428  ema = tx.bucket(
-00000cd0: 2762 7563 6b65 742d 6e61 6d65 2729 2e73  'bucket-name').s
-00000ce0: 6368 656d 6128 2773 6368 656d 612d 6e61  chema('schema-na
-00000cf0: 6d65 2729 0a20 2020 2074 6162 6c65 203d  me').    table =
-00000d00: 2075 7469 6c2e 6372 6561 7465 5f74 6162   util.create_tab
-00000d10: 6c65 5f66 726f 6d5f 6669 6c65 7328 0a20  le_from_files(. 
-00000d20: 2020 2020 2020 2073 6368 656d 613d 7363         schema=sc
-00000d30: 6865 6d61 2c20 7461 626c 655f 6e61 6d65  hema, table_name
-00000d40: 3d27 696d 706f 7274 6564 2d74 6162 6c65  ='imported-table
-00000d50: 272c 0a20 2020 2020 2020 2070 6172 7175  ',.        parqu
-00000d60: 6574 5f66 696c 6573 3d5b 272f 6275 636b  et_files=['/buck
-00000d70: 6574 2d6e 616d 652f 7374 6167 696e 672f  et-name/staging/
-00000d80: 6669 6c65 2e70 6172 7175 6574 275d 290a  file.parquet']).
-00000d90: 6060 600a 0a23 2320 496d 706f 7274 206d  ```..## Import m
-00000da0: 756c 7469 706c 6520 5061 7271 7565 7420  ultiple Parquet 
-00000db0: 6669 6c65 7320 636f 6e63 7572 7265 6e74  files concurrent
-00000dc0: 6c79 2076 6961 2053 3320 7072 6f74 6f63  ly via S3 protoc
-00000dd0: 6f6c 0a0a 5765 2063 616e 2069 6d70 6f72  ol..We can impor
-00000de0: 7420 6d75 6c74 6970 6c65 2066 696c 6573  t multiple files
-00000df0: 2063 6f6e 6375 7272 656e 746c 7920 696e   concurrently in
-00000e00: 746f 2061 2074 6162 6c65 2028 6279 2075  to a table (by u
-00000e10: 7469 6c69 7a69 6e67 206d 756c 7469 706c  tilizing multipl
-00000e20: 6520 434e 6f64 6573 2720 636f 7265 7329  e CNodes' cores)
-00000e30: 3a0a 0a60 6060 7079 7468 6f6e 0a20 2020  :..```python.   
-00000e40: 2073 6368 656d 6120 3d20 7478 2e62 7563   schema = tx.buc
-00000e50: 6b65 7428 2762 7563 6b65 742d 6e61 6d65  ket('bucket-name
-00000e60: 2729 2e73 6368 656d 6128 2773 6368 656d  ').schema('schem
-00000e70: 612d 6e61 6d65 2729 0a20 2020 2074 6162  a-name').    tab
-00000e80: 6c65 203d 2075 7469 6c2e 6372 6561 7465  le = util.create
-00000e90: 5f74 6162 6c65 5f66 726f 6d5f 6669 6c65  _table_from_file
-00000ea0: 7328 0a20 2020 2020 2020 2073 6368 656d  s(.        schem
-00000eb0: 613d 7363 6865 6d61 2c20 7461 626c 655f  a=schema, table_
-00000ec0: 6e61 6d65 3d27 6c61 7267 652d 696d 706f  name='large-impo
-00000ed0: 7274 6564 2d74 6162 6c65 272c 0a20 2020  rted-table',.   
-00000ee0: 2020 2020 2070 6172 7175 6574 5f66 696c       parquet_fil
-00000ef0: 6573 3d5b 6627 2f62 7563 6b65 742d 6e61  es=[f'/bucket-na
-00000f00: 6d65 2f73 7461 6769 6e67 2f66 696c 657b  me/staging/file{
-00000f10: 697d 2e70 6172 7175 6574 2720 666f 7220  i}.parquet' for 
-00000f20: 6920 696e 2072 616e 6765 2831 3029 5d29  i in range(10)])
-00000f30: 0a60 6060 0a0a 2323 2050 6f73 742d 7072  .```..## Post-pr
-00000f40: 6f63 6573 7369 6e67 0a0a 2323 2320 4578  ocessing..### Ex
-00000f50: 706f 7274 0a0a 6054 6162 6c65 2e73 656c  port..`Table.sel
-00000f60: 6563 7428 2960 2072 6574 7572 6e73 2061  ect()` returns a
-00000f70: 2073 7472 6561 6d20 6f66 205b 5079 4172   stream of [PyAr
-00000f80: 726f 7720 7265 636f 7264 2062 6174 6368  row record batch
-00000f90: 6573 5d28 6874 7470 733a 2f2f 6172 726f  es](https://arro
-00000fa0: 772e 6170 6163 6865 2e6f 7267 2f64 6f63  w.apache.org/doc
-00000fb0: 732f 7079 7468 6f6e 2f64 6174 612e 6874  s/python/data.ht
-00000fc0: 6d6c 2372 6563 6f72 642d 6261 7463 6865  ml#record-batche
-00000fd0: 7329 2c20 7768 6963 6820 6361 6e20 6265  s), which can be
-00000fe0: 2064 6972 6563 746c 7920 6578 706f 7274   directly export
-00000ff0: 6564 2069 6e74 6f20 6120 5061 7271 7565  ed into a Parque
-00001000: 7420 6669 6c65 3a0a 0a60 6060 7079 7468  t file:..```pyth
-00001010: 6f6e 0a62 6174 6368 6573 203d 2074 6162  on.batches = tab
-00001020: 6c65 2e73 656c 6563 7428 290a 7769 7468  le.select().with
-00001030: 2063 6f6e 7465 7874 6c69 622e 636c 6f73   contextlib.clos
-00001040: 696e 6728 7061 2e70 6172 7175 6574 2e50  ing(pa.parquet.P
-00001050: 6172 7175 6574 5772 6974 6572 2827 2f70  arquetWriter('/p
-00001060: 6174 682f 746f 2f66 696c 652e 7061 7271  ath/to/file.parq
-00001070: 7565 7427 2c20 6261 7463 6865 732e 7363  uet', batches.sc
-00001080: 6865 6d61 2929 2061 7320 7772 6974 6572  hema)) as writer
-00001090: 3a0a 2020 2020 666f 7220 6261 7463 6820  :.    for batch 
-000010a0: 696e 2074 6162 6c65 5f62 6174 6368 6573  in table_batches
-000010b0: 3a0a 2020 2020 2020 2020 7772 6974 6572  :.        writer
-000010c0: 2e77 7269 7465 5f62 6174 6368 2862 6174  .write_batch(bat
-000010d0: 6368 290a 6060 600a 0a23 2323 2044 7563  ch).```..### Duc
-000010e0: 6b44 420a 0a57 6520 6361 6e20 7573 6520  kDB..We can use 
-000010f0: 5b44 7563 6b44 425d 2868 7474 7073 3a2f  [DuckDB](https:/
-00001100: 2f64 7563 6b64 622e 6f72 672f 646f 6373  /duckdb.org/docs
-00001110: 2f67 7569 6465 732f 7079 7468 6f6e 2f73  /guides/python/s
-00001120: 716c 5f6f 6e5f 6172 726f 772e 6874 6d6c  ql_on_arrow.html
-00001130: 2920 746f 2070 6f73 742d 7072 6f63 6573  ) to post-proces
-00001140: 7320 7468 6520 7265 7375 6c74 696e 6720  s the resulting 
-00001150: 7374 7265 616d 206f 6620 5b50 7941 7272  stream of [PyArr
-00001160: 6f77 2072 6563 6f72 6420 6261 7463 6865  ow record batche
-00001170: 735d 2868 7474 7073 3a2f 2f61 7272 6f77  s](https://arrow
-00001180: 2e61 7061 6368 652e 6f72 672f 646f 6373  .apache.org/docs
-00001190: 2f70 7974 686f 6e2f 6461 7461 2e68 746d  /python/data.htm
-000011a0: 6c23 7265 636f 7264 2d62 6174 6368 6573  l#record-batches
-000011b0: 293a 0a0a 6060 6070 7974 686f 6e0a 6672  ):..```python.fr
-000011c0: 6f6d 2069 6269 7320 696d 706f 7274 205f  om ibis import _
-000011d0: 0a0a 696d 706f 7274 2064 7563 6b64 620a  ..import duckdb.
-000011e0: 636f 6e6e 203d 2064 7563 6b64 622e 636f  conn = duckdb.co
-000011f0: 6e6e 6563 7428 290a 0a62 6174 6368 6573  nnect()..batches
-00001200: 203d 2074 6162 6c65 2e73 656c 6563 7428   = table.select(
-00001210: 636f 6c75 6d6e 733d 5b27 6331 275d 2c20  columns=['c1'], 
-00001220: 7072 6564 6963 6174 653d 285f 2e63 3220  predicate=(_.c2 
-00001230: 3e20 3229 290a 7072 696e 7428 636f 6e6e  > 2)).print(conn
-00001240: 2e65 7865 6375 7465 2822 5345 4c45 4354  .execute("SELECT
-00001250: 2073 756d 2863 3129 2046 524f 4d20 6261   sum(c1) FROM ba
-00001260: 7463 6865 7322 292e 6172 726f 7728 2929  tches").arrow())
-00001270: 0a60 6060 0a0a 2323 2053 656d 692d 736f  .```..## Semi-so
-00001280: 7274 6564 2070 726f 6a65 6374 696f 6e73  rted projections
-00001290: 0a0a 5765 2063 616e 2063 7265 6174 652c  ..We can create,
-000012a0: 206c 6973 7420 616e 6420 6465 6c65 7465   list and delete
-000012b0: 205b 6176 6169 6c61 626c 6520 7365 6d69   [available semi
-000012c0: 2d73 6f72 7465 6420 7072 6f6a 6563 7469  -sorted projecti
-000012d0: 6f6e 735d 2868 7474 7073 3a2f 2f73 7570  ons](https://sup
-000012e0: 706f 7274 2e76 6173 7464 6174 612e 636f  port.vastdata.co
-000012f0: 6d2f 732f 6172 7469 636c 652f 5555 4944  m/s/article/UUID
-00001300: 2d65 3463 6134 3261 622d 6431 3562 2d36  -e4ca42ab-d15b-6
-00001310: 6237 322d 6264 3662 2d66 3363 3737 6234  b72-bd6b-f3c77b4
-00001320: 3535 6465 3429 3a0a 0a60 6060 7079 7468  55de4):..```pyth
-00001330: 6f6e 0a70 203d 2074 6162 6c65 2e63 7265  on.p = table.cre
-00001340: 6174 655f 7072 6f6a 6563 7469 6f6e 2827  ate_projection('
-00001350: 7072 6f6a 272c 2073 6f72 7465 643d 5b27  proj', sorted=['
-00001360: 6333 275d 2c20 756e 736f 7274 6564 3d5b  c3'], unsorted=[
-00001370: 2763 3127 5d29 0a70 7269 6e74 2874 6162  'c1']).print(tab
-00001380: 6c65 2e70 726f 6a65 6374 696f 6e73 2829  le.projections()
-00001390: 290a 7072 696e 7428 702e 6765 745f 7374  ).print(p.get_st
-000013a0: 6174 7328 2929 0a70 2e64 726f 7028 290a  ats()).p.drop().
-000013b0: 6060 600a 0a23 2320 536e 6170 7368 6f74  ```..## Snapshot
-000013c0: 730a 0a49 7420 6973 2070 6f73 7369 626c  s..It is possibl
-000013d0: 6520 746f 2075 7365 205b 736e 6170 7368  e to use [snapsh
-000013e0: 6f74 735d 2868 7474 7073 3a2f 2f76 6173  ots](https://vas
-000013f0: 7464 6174 612e 636f 6d2f 626c 6f67 2f62  tdata.com/blog/b
-00001400: 7269 6e67 696e 672d 736e 6170 7368 6f74  ringing-snapshot
-00001410: 732d 746f 2d76 6173 7473 2d65 6c65 6d65  s-to-vasts-eleme
-00001420: 6e74 2d73 746f 7265 2920 666f 7220 6163  nt-store) for ac
-00001430: 6365 7373 696e 6720 7468 6520 4461 7461  cessing the Data
-00001440: 6261 7365 3a0a 0a60 6060 7079 7468 6f6e  base:..```python
-00001450: 0a73 6e61 7073 203d 2062 7563 6b65 742e  .snaps = bucket.
-00001460: 6c69 7374 5f73 6e61 7073 686f 7473 2829  list_snapshots()
-00001470: 0a62 6174 6368 6573 203d 2073 6e61 7073  .batches = snaps
-00001480: 5b30 5d2e 7363 6865 6d61 2827 7363 6865  [0].schema('sche
-00001490: 6d61 2d6e 616d 6527 292e 7461 626c 6528  ma-name').table(
-000014a0: 2774 6162 6c65 2d6e 616d 6527 292e 7365  'table-name').se
-000014b0: 6c65 6374 2829 0a60 6060 0a0a 2323 2056  lect().```..## V
-000014c0: 4153 5420 4361 7461 6c6f 670a 0a5b 5641  AST Catalog..[VA
-000014d0: 5354 2043 6174 616c 6f67 5d28 6874 7470  ST Catalog](http
-000014e0: 733a 2f2f 7661 7374 6461 7461 2e63 6f6d  s://vastdata.com
-000014f0: 2f62 6c6f 672f 7661 7374 2d63 6174 616c  /blog/vast-catal
-00001500: 6f67 2d74 7265 6174 2d79 6f75 722d 6669  og-treat-your-fi
-00001510: 6c65 2d73 7973 7465 6d2d 6c69 6b65 2d61  le-system-like-a
-00001520: 2d64 6174 6162 6173 6529 2063 616e 2062  -database) can b
-00001530: 6520 7175 6572 6965 6420 6173 2061 2072  e queried as a r
-00001540: 6567 756c 6172 2074 6162 6c65 3a0a 0a60  egular table:..`
-00001550: 6060 7079 7468 6f6e 0a74 6162 6c65 203d  ``python.table =
-00001560: 2070 612e 5461 626c 652e 6672 6f6d 5f62   pa.Table.from_b
-00001570: 6174 6368 6573 2874 782e 6361 7461 6c6f  atches(tx.catalo
-00001580: 672e 7365 6c65 6374 285b 2765 6c65 6d65  g.select(['eleme
-00001590: 6e74 5f74 7970 6527 5d29 290a 6466 203d  nt_type'])).df =
-000015a0: 2074 6162 6c65 2e74 6f5f 7061 6e64 6173   table.to_pandas
-000015b0: 2829 0a0a 746f 7461 6c5f 656c 656d 656e  ()..total_elemen
-000015c0: 7473 203d 206c 656e 2864 6629 0a70 7269  ts = len(df).pri
-000015d0: 6e74 2866 2254 6f74 616c 2065 6c65 6d65  nt(f"Total eleme
-000015e0: 6e74 7320 696e 2074 6865 2063 6174 616c  nts in the catal
-000015f0: 6f67 3a20 7b74 6f74 616c 5f65 6c65 6d65  og: {total_eleme
-00001600: 6e74 737d 2229 0a0a 6669 6c65 5f63 6f75  nts}")..file_cou
-00001610: 6e74 203d 2028 6466 5b27 656c 656d 656e  nt = (df['elemen
-00001620: 745f 7479 7065 275d 203d 3d20 2746 494c  t_type'] == 'FIL
-00001630: 4527 292e 7375 6d28 290a 7072 696e 7428  E').sum().print(
-00001640: 6622 4e75 6d62 6572 206f 6620 6669 6c65  f"Number of file
-00001650: 732f 6f62 6a65 6374 733a 207b 6669 6c65  s/objects: {file
-00001660: 5f63 6f75 6e74 7d22 290a 0a64 6973 7469  _count}")..disti
-00001670: 6e63 745f 656c 656d 656e 7473 203d 2064  nct_elements = d
-00001680: 665b 2765 6c65 6d65 6e74 5f74 7970 6527  f['element_type'
-00001690: 5d2e 756e 6971 7565 2829 0a70 7269 6e74  ].unique().print
-000016a0: 2822 4469 7374 696e 6374 2065 6c65 6d65  ("Distinct eleme
-000016b0: 6e74 2074 7970 6573 206f 6e20 7468 6520  nt types on the 
-000016c0: 7379 7374 656d 3a22 290a 7072 696e 7428  system:").print(
-000016d0: 6469 7374 696e 6374 5f65 6c65 6d65 6e74  distinct_element
-000016e0: 7329 0a60 6060 0a0a 5365 6520 7468 6520  s).```..See the 
-000016f0: 666f 6c6c 6f77 696e 6720 626c 6f67 2070  following blog p
-00001700: 6f73 7473 2066 6f72 206d 6f72 6520 6578  osts for more ex
-00001710: 616d 706c 6573 3a0a 0a2d 2068 7474 7073  amples:..- https
-00001720: 3a2f 2f76 6173 7464 6174 612e 636f 6d2f  ://vastdata.com/
-00001730: 626c 6f67 2f74 6865 2d76 6173 742d 6361  blog/the-vast-ca
-00001740: 7461 6c6f 672d 696e 2d61 6374 696f 6e2d  talog-in-action-
-00001750: 7061 7274 2d31 0a2d 2068 7474 7073 3a2f  part-1.- https:/
-00001760: 2f76 6173 7464 6174 612e 636f 6d2f 626c  /vastdata.com/bl
-00001770: 6f67 2f74 6865 2d76 6173 742d 6361 7461  og/the-vast-cata
-00001780: 6c6f 672d 696e 2d61 6374 696f 6e2d 7061  log-in-action-pa
-00001790: 7274 2d32 0a                             rt-2.
+00000860: 2320 7275 6e20 6053 454c 4543 5420 2a20  # run `SELECT * 
+00000870: 4652 4f4d 2074 600a 2020 2020 7265 6164  FROM t`.    read
+00000880: 6572 203d 2074 6162 6c65 2e73 656c 6563  er = table.selec
+00000890: 7428 2920 2023 2072 6574 7572 6e20 6120  t()  # return a 
+000008a0: 6070 7961 7272 6f77 2e52 6563 6f72 6442  `pyarrow.RecordB
+000008b0: 6174 6368 5265 6164 6572 600a 2020 2020  atchReader`.    
+000008c0: 7265 7375 6c74 203d 2070 612e 5461 626c  result = pa.Tabl
+000008d0: 652e 6672 6f6d 5f62 6174 6368 6573 2872  e.from_batches(r
+000008e0: 6561 6465 7229 2020 2320 6275 696c 6420  eader)  # build 
+000008f0: 616e 2050 7941 7272 6f77 2054 6162 6c65  an PyArrow Table
+00000900: 2066 726f 6d20 7468 6520 6070 7961 7272   from the `pyarr
+00000910: 6f77 2e52 6563 6f72 6442 6174 6368 6020  ow.RecordBatch` 
+00000920: 6f62 6a65 6374 7320 7265 6164 2066 726f  objects read fro
+00000930: 6d20 5641 5354 0a20 2020 2061 7373 6572  m VAST.    asser
+00000940: 7420 7265 7375 6c74 203d 3d20 6172 726f  t result == arro
+00000950: 775f 7461 626c 650a 0a20 2020 2023 2074  w_table..    # t
+00000960: 6865 2074 7261 6e73 6163 7469 6f6e 2069  he transaction i
+00000970: 7320 6175 746f 6d61 7469 6361 6c6c 7920  s automatically 
+00000980: 636f 6d6d 6974 7465 6420 7768 656e 2065  committed when e
+00000990: 7869 7469 6e67 2074 6865 2063 6f6e 7465  xiting the conte
+000009a0: 7874 0a60 6060 0a0a 4e6f 7465 3a20 7468  xt.```..Note: th
+000009b0: 6520 7472 616e 7361 6374 696f 6e20 6d75  e transaction mu
+000009c0: 7374 2062 6520 7265 6d61 696e 206f 7065  st be remain ope
+000009d0: 6e20 7768 696c 6520 7468 6520 7265 7475  n while the retu
+000009e0: 726e 6564 205b 7079 6172 726f 772e 5265  rned [pyarrow.Re
+000009f0: 636f 7264 4261 7463 6852 6561 6465 725d  cordBatchReader]
+00000a00: 2868 7474 7073 3a2f 2f61 7272 6f77 2e61  (https://arrow.a
+00000a10: 7061 6368 652e 6f72 672f 646f 6373 2f70  pache.org/docs/p
+00000a20: 7974 686f 6e2f 6765 6e65 7261 7465 642f  ython/generated/
+00000a30: 7079 6172 726f 772e 5265 636f 7264 4261  pyarrow.RecordBa
+00000a40: 7463 6852 6561 6465 722e 6874 6d6c 2920  tchReader.html) 
+00000a50: 6765 6e65 7261 746f 7220 6973 2062 6569  generator is bei
+00000a60: 6e67 2075 7365 642e 0a0a 2323 2046 696c  ng used...## Fil
+00000a70: 7465 7273 2061 6e64 2070 726f 6a65 6374  ters and project
+00000a80: 696f 6e73 0a0a 4f75 7220 5344 4b20 7375  ions..Our SDK su
+00000a90: 7070 6f72 7473 2070 7265 6469 6361 7465  pports predicate
+00000aa0: 2061 6e64 2070 726f 6a65 6374 696f 6e20   and projection 
+00000ab0: 7075 7368 646f 776e 3a0a 0a60 6060 7079  pushdown:..```py
+00000ac0: 7468 6f6e 0a20 2020 2066 726f 6d20 6962  thon.    from ib
+00000ad0: 6973 2069 6d70 6f72 7420 5f0a 0a20 2020  is import _..   
+00000ae0: 2023 2053 454c 4543 5420 6331 2046 524f   # SELECT c1 FRO
+00000af0: 4d20 7420 5748 4552 4520 2863 3220 3e20  M t WHERE (c2 > 
+00000b00: 3229 2041 4e44 2028 6333 2049 5320 4e55  2) AND (c3 IS NU
+00000b10: 4c4c 290a 2020 2020 7461 626c 652e 7365  LL).    table.se
+00000b20: 6c65 6374 2863 6f6c 756d 6e73 3d5b 2763  lect(columns=['c
+00000b30: 3127 5d2c 0a20 2020 2020 2020 2020 2020  1'],.           
+00000b40: 2020 2020 2020 7072 6564 6963 6174 653d        predicate=
+00000b50: 285f 2e63 3220 3e20 3229 2026 205f 2e63  (_.c2 > 2) & _.c
+00000b60: 332e 6973 6e75 6c6c 2829 290a 0a20 2020  3.isnull())..   
+00000b70: 2023 2053 454c 4543 5420 6332 2c20 6333   # SELECT c2, c3
+00000b80: 2046 524f 4d20 7420 5748 4552 4520 2863   FROM t WHERE (c
+00000b90: 3220 4245 5457 4545 4e20 3020 414e 4420  2 BETWEEN 0 AND 
+00000ba0: 3129 204f 5220 2863 3220 3e20 3130 290a  1) OR (c2 > 10).
+00000bb0: 2020 2020 7461 626c 652e 7365 6c65 6374      table.select
+00000bc0: 2863 6f6c 756d 6e73 3d5b 2763 3227 2c20  (columns=['c2', 
+00000bd0: 2763 3327 5d2c 0a20 2020 2020 2020 2020  'c3'],.         
+00000be0: 2020 2020 2020 2020 7072 6564 6963 6174          predicat
+00000bf0: 653d 285f 2e63 322e 6265 7477 6565 6e28  e=(_.c2.between(
+00000c00: 302c 2031 2920 7c20 285f 2e63 3220 3e20  0, 1) | (_.c2 > 
+00000c10: 3130 2929 0a0a 2020 2020 2320 5345 4c45  10))..    # SELE
+00000c20: 4354 202a 2046 524f 4d20 7420 5748 4552  CT * FROM t WHER
+00000c30: 4520 6333 204c 494b 4520 2725 7375 6273  E c3 LIKE '%subs
+00000c40: 7472 696e 6725 270a 2020 2020 7461 626c  tring%'.    tabl
+00000c50: 652e 7365 6c65 6374 2870 7265 6469 6361  e.select(predica
+00000c60: 7465 3d5f 2e63 332e 636f 6e74 6169 6e73  te=_.c3.contains
+00000c70: 2827 7375 6273 7472 696e 6727 2929 0a60  ('substring')).`
+00000c80: 6060 0a0a 5365 6520 5b68 6572 6520 666f  ``..See [here fo
+00000c90: 7220 6d6f 7265 2064 6574 6169 6c73 5d28  r more details](
+00000ca0: 646f 6373 2f70 7265 6469 6361 7465 2e6d  docs/predicate.m
+00000cb0: 6429 2e0a 0a23 2320 496d 706f 7274 2061  d)...## Import a
+00000cc0: 2073 696e 676c 6520 5061 7271 7565 7420   single Parquet 
+00000cd0: 6669 6c65 2076 6961 2053 3320 7072 6f74  file via S3 prot
+00000ce0: 6f63 6f6c 0a0a 4974 2069 7320 706f 7373  ocol..It is poss
+00000cf0: 6962 6c65 2074 6f20 6566 6669 6369 656e  ible to efficien
+00000d00: 746c 7920 6372 6561 7465 2061 2074 6162  tly create a tab
+00000d10: 6c65 2066 726f 6d20 6120 5061 7271 7565  le from a Parque
+00000d20: 7420 6669 6c65 2028 7769 7468 6f75 7420  t file (without 
+00000d30: 636f 7079 696e 6720 6974 2076 6961 2074  copying it via t
+00000d40: 6865 2063 6c69 656e 7429 3a0a 0a60 6060  he client):..```
+00000d50: 7079 7468 6f6e 0a20 2020 2077 6974 6820  python.    with 
+00000d60: 7465 6d70 6669 6c65 2e4e 616d 6564 5465  tempfile.NamedTe
+00000d70: 6d70 6f72 6172 7946 696c 6528 2920 6173  mporaryFile() as
+00000d80: 2066 3a0a 2020 2020 2020 2020 7061 2e70   f:.        pa.p
+00000d90: 6172 7175 6574 2e77 7269 7465 5f74 6162  arquet.write_tab
+00000da0: 6c65 2861 7272 6f77 5f74 6162 6c65 2c20  le(arrow_table, 
+00000db0: 662e 6e61 6d65 290a 2020 2020 2020 2020  f.name).        
+00000dc0: 7333 2e70 7574 5f6f 626a 6563 7428 4275  s3.put_object(Bu
+00000dd0: 636b 6574 3d27 6275 636b 6574 2d6e 616d  cket='bucket-nam
+00000de0: 6527 2c20 4b65 793d 2773 7461 6769 6e67  e', Key='staging
+00000df0: 2f66 696c 652e 7061 7271 7565 7427 2c20  /file.parquet', 
+00000e00: 426f 6479 3d66 290a 0a20 2020 2073 6368  Body=f)..    sch
+00000e10: 656d 6120 3d20 7478 2e62 7563 6b65 7428  ema = tx.bucket(
+00000e20: 2762 7563 6b65 742d 6e61 6d65 2729 2e73  'bucket-name').s
+00000e30: 6368 656d 6128 2773 6368 656d 612d 6e61  chema('schema-na
+00000e40: 6d65 2729 0a20 2020 2074 6162 6c65 203d  me').    table =
+00000e50: 2075 7469 6c2e 6372 6561 7465 5f74 6162   util.create_tab
+00000e60: 6c65 5f66 726f 6d5f 6669 6c65 7328 0a20  le_from_files(. 
+00000e70: 2020 2020 2020 2073 6368 656d 613d 7363         schema=sc
+00000e80: 6865 6d61 2c20 7461 626c 655f 6e61 6d65  hema, table_name
+00000e90: 3d27 696d 706f 7274 6564 2d74 6162 6c65  ='imported-table
+00000ea0: 272c 0a20 2020 2020 2020 2070 6172 7175  ',.        parqu
+00000eb0: 6574 5f66 696c 6573 3d5b 272f 6275 636b  et_files=['/buck
+00000ec0: 6574 2d6e 616d 652f 7374 6167 696e 672f  et-name/staging/
+00000ed0: 6669 6c65 2e70 6172 7175 6574 275d 290a  file.parquet']).
+00000ee0: 6060 600a 0a23 2320 496d 706f 7274 206d  ```..## Import m
+00000ef0: 756c 7469 706c 6520 5061 7271 7565 7420  ultiple Parquet 
+00000f00: 6669 6c65 7320 636f 6e63 7572 7265 6e74  files concurrent
+00000f10: 6c79 2076 6961 2053 3320 7072 6f74 6f63  ly via S3 protoc
+00000f20: 6f6c 0a0a 5765 2063 616e 2069 6d70 6f72  ol..We can impor
+00000f30: 7420 6d75 6c74 6970 6c65 2066 696c 6573  t multiple files
+00000f40: 2063 6f6e 6375 7272 656e 746c 7920 696e   concurrently in
+00000f50: 746f 2061 2074 6162 6c65 2028 6279 2075  to a table (by u
+00000f60: 7469 6c69 7a69 6e67 206d 756c 7469 706c  tilizing multipl
+00000f70: 6520 434e 6f64 6573 2720 636f 7265 7329  e CNodes' cores)
+00000f80: 3a0a 0a60 6060 7079 7468 6f6e 0a20 2020  :..```python.   
+00000f90: 2073 6368 656d 6120 3d20 7478 2e62 7563   schema = tx.buc
+00000fa0: 6b65 7428 2762 7563 6b65 742d 6e61 6d65  ket('bucket-name
+00000fb0: 2729 2e73 6368 656d 6128 2773 6368 656d  ').schema('schem
+00000fc0: 612d 6e61 6d65 2729 0a20 2020 2074 6162  a-name').    tab
+00000fd0: 6c65 203d 2075 7469 6c2e 6372 6561 7465  le = util.create
+00000fe0: 5f74 6162 6c65 5f66 726f 6d5f 6669 6c65  _table_from_file
+00000ff0: 7328 0a20 2020 2020 2020 2073 6368 656d  s(.        schem
+00001000: 613d 7363 6865 6d61 2c20 7461 626c 655f  a=schema, table_
+00001010: 6e61 6d65 3d27 6c61 7267 652d 696d 706f  name='large-impo
+00001020: 7274 6564 2d74 6162 6c65 272c 0a20 2020  rted-table',.   
+00001030: 2020 2020 2070 6172 7175 6574 5f66 696c       parquet_fil
+00001040: 6573 3d5b 6627 2f62 7563 6b65 742d 6e61  es=[f'/bucket-na
+00001050: 6d65 2f73 7461 6769 6e67 2f66 696c 657b  me/staging/file{
+00001060: 697d 2e70 6172 7175 6574 2720 666f 7220  i}.parquet' for 
+00001070: 6920 696e 2072 616e 6765 2831 3029 5d29  i in range(10)])
+00001080: 0a60 6060 0a0a 2323 2050 6f73 742d 7072  .```..## Post-pr
+00001090: 6f63 6573 7369 6e67 0a0a 2323 2320 4578  ocessing..### Ex
+000010a0: 706f 7274 0a0a 6054 6162 6c65 2e73 656c  port..`Table.sel
+000010b0: 6563 7428 2960 2072 6574 7572 6e73 2061  ect()` returns a
+000010c0: 2073 7472 6561 6d20 6f66 205b 5079 4172   stream of [PyAr
+000010d0: 726f 7720 7265 636f 7264 2062 6174 6368  row record batch
+000010e0: 6573 5d28 6874 7470 733a 2f2f 6172 726f  es](https://arro
+000010f0: 772e 6170 6163 6865 2e6f 7267 2f64 6f63  w.apache.org/doc
+00001100: 732f 7079 7468 6f6e 2f64 6174 612e 6874  s/python/data.ht
+00001110: 6d6c 2372 6563 6f72 642d 6261 7463 6865  ml#record-batche
+00001120: 7329 2c20 7768 6963 6820 6361 6e20 6265  s), which can be
+00001130: 2064 6972 6563 746c 7920 6578 706f 7274   directly export
+00001140: 6564 2069 6e74 6f20 6120 5061 7271 7565  ed into a Parque
+00001150: 7420 6669 6c65 3a0a 0a60 6060 7079 7468  t file:..```pyth
+00001160: 6f6e 0a62 6174 6368 6573 203d 2074 6162  on.batches = tab
+00001170: 6c65 2e73 656c 6563 7428 290a 7769 7468  le.select().with
+00001180: 2063 6f6e 7465 7874 6c69 622e 636c 6f73   contextlib.clos
+00001190: 696e 6728 7061 2e70 6172 7175 6574 2e50  ing(pa.parquet.P
+000011a0: 6172 7175 6574 5772 6974 6572 2827 2f70  arquetWriter('/p
+000011b0: 6174 682f 746f 2f66 696c 652e 7061 7271  ath/to/file.parq
+000011c0: 7565 7427 2c20 6261 7463 6865 732e 7363  uet', batches.sc
+000011d0: 6865 6d61 2929 2061 7320 7772 6974 6572  hema)) as writer
+000011e0: 3a0a 2020 2020 666f 7220 6261 7463 6820  :.    for batch 
+000011f0: 696e 2074 6162 6c65 5f62 6174 6368 6573  in table_batches
+00001200: 3a0a 2020 2020 2020 2020 7772 6974 6572  :.        writer
+00001210: 2e77 7269 7465 5f62 6174 6368 2862 6174  .write_batch(bat
+00001220: 6368 290a 6060 600a 0a23 2323 2044 7563  ch).```..### Duc
+00001230: 6b44 4220 696e 7465 6772 6174 696f 6e0a  kDB integration.
+00001240: 0a57 6520 6361 6e20 7573 6520 5b44 7563  .We can use [Duc
+00001250: 6b44 425d 2868 7474 7073 3a2f 2f64 7563  kDB](https://duc
+00001260: 6b64 622e 6f72 672f 646f 6373 2f67 7569  kdb.org/docs/gui
+00001270: 6465 732f 7079 7468 6f6e 2f73 716c 5f6f  des/python/sql_o
+00001280: 6e5f 6172 726f 772e 6874 6d6c 2920 746f  n_arrow.html) to
+00001290: 2070 6f73 742d 7072 6f63 6573 7320 7468   post-process th
+000012a0: 6520 7265 7375 6c74 696e 6720 7374 7265  e resulting stre
+000012b0: 616d 206f 6620 5b50 7941 7272 6f77 2072  am of [PyArrow r
+000012c0: 6563 6f72 6420 6261 7463 6865 735d 2868  ecord batches](h
+000012d0: 7474 7073 3a2f 2f61 7272 6f77 2e61 7061  ttps://arrow.apa
+000012e0: 6368 652e 6f72 672f 646f 6373 2f70 7974  che.org/docs/pyt
+000012f0: 686f 6e2f 6461 7461 2e68 746d 6c23 7265  hon/data.html#re
+00001300: 636f 7264 2d62 6174 6368 6573 293a 0a0a  cord-batches):..
+00001310: 6060 6070 7974 686f 6e0a 6672 6f6d 2069  ```python.from i
+00001320: 6269 7320 696d 706f 7274 205f 0a0a 696d  bis import _..im
+00001330: 706f 7274 2064 7563 6b64 620a 636f 6e6e  port duckdb.conn
+00001340: 203d 2064 7563 6b64 622e 636f 6e6e 6563   = duckdb.connec
+00001350: 7428 290a 0a77 6974 6820 7365 7373 696f  t()..with sessio
+00001360: 6e2e 7472 616e 7361 6374 696f 6e28 2920  n.transaction() 
+00001370: 6173 2074 783a 0a20 2020 2074 6162 6c65  as tx:.    table
+00001380: 203d 2074 782e 6275 636b 6574 2822 6275   = tx.bucket("bu
+00001390: 636b 6574 2d6e 616d 6522 292e 7363 6865  cket-name").sche
+000013a0: 6d61 2822 7363 6865 6d61 2d6e 616d 6522  ma("schema-name"
+000013b0: 292e 7461 626c 6528 2274 6162 6c65 2d6e  ).table("table-n
+000013c0: 616d 6522 290a 2020 2020 6261 7463 6865  ame").    batche
+000013d0: 7320 3d20 7461 626c 652e 7365 6c65 6374  s = table.select
+000013e0: 2863 6f6c 756d 6e73 3d5b 2763 3127 5d2c  (columns=['c1'],
+000013f0: 2070 7265 6469 6361 7465 3d28 5f2e 6332   predicate=(_.c2
+00001400: 203e 2032 2929 0a20 2020 2070 7269 6e74   > 2)).    print
+00001410: 2863 6f6e 6e2e 6578 6563 7574 6528 2253  (conn.execute("S
+00001420: 454c 4543 5420 7375 6d28 6331 2920 4652  ELECT sum(c1) FR
+00001430: 4f4d 2062 6174 6368 6573 2229 2e61 7272  OM batches").arr
+00001440: 6f77 2829 290a 6060 600a 0a4e 6f74 653a  ow()).```..Note:
+00001450: 2074 6865 2074 7261 6e73 6163 7469 6f6e   the transaction
+00001460: 206d 7573 7420 6265 2061 6374 6976 6520   must be active 
+00001470: 7768 696c 6520 4475 636b 4442 2071 7565  while DuckDB que
+00001480: 7279 2069 7320 6578 6563 7574 696e 6720  ry is executing 
+00001490: 616e 6420 6665 7463 6869 6e67 2072 6573  and fetching res
+000014a0: 756c 7473 2075 7369 6e67 2074 6865 2050  ults using the P
+000014b0: 7974 686f 6e20 5344 4b2e 0a0a 2323 2053  ython SDK...## S
+000014c0: 656d 692d 736f 7274 6564 2070 726f 6a65  emi-sorted proje
+000014d0: 6374 696f 6e73 0a0a 5765 2063 616e 2063  ctions..We can c
+000014e0: 7265 6174 652c 206c 6973 7420 616e 6420  reate, list and 
+000014f0: 6465 6c65 7465 205b 6176 6169 6c61 626c  delete [availabl
+00001500: 6520 7365 6d69 2d73 6f72 7465 6420 7072  e semi-sorted pr
+00001510: 6f6a 6563 7469 6f6e 735d 2868 7474 7073  ojections](https
+00001520: 3a2f 2f73 7570 706f 7274 2e76 6173 7464  ://support.vastd
+00001530: 6174 612e 636f 6d2f 732f 6172 7469 636c  ata.com/s/articl
+00001540: 652f 5555 4944 2d65 3463 6134 3261 622d  e/UUID-e4ca42ab-
+00001550: 6431 3562 2d36 6237 322d 6264 3662 2d66  d15b-6b72-bd6b-f
+00001560: 3363 3737 6234 3535 6465 3429 3a0a 0a60  3c77b455de4):..`
+00001570: 6060 7079 7468 6f6e 0a70 203d 2074 6162  ``python.p = tab
+00001580: 6c65 2e63 7265 6174 655f 7072 6f6a 6563  le.create_projec
+00001590: 7469 6f6e 2827 7072 6f6a 272c 2073 6f72  tion('proj', sor
+000015a0: 7465 643d 5b27 6333 275d 2c20 756e 736f  ted=['c3'], unso
+000015b0: 7274 6564 3d5b 2763 3127 5d29 0a70 7269  rted=['c1']).pri
+000015c0: 6e74 2874 6162 6c65 2e70 726f 6a65 6374  nt(table.project
+000015d0: 696f 6e73 2829 290a 7072 696e 7428 702e  ions()).print(p.
+000015e0: 6765 745f 7374 6174 7328 2929 0a70 2e64  get_stats()).p.d
+000015f0: 726f 7028 290a 6060 600a 0a23 2320 536e  rop().```..## Sn
+00001600: 6170 7368 6f74 730a 0a49 7420 6973 2070  apshots..It is p
+00001610: 6f73 7369 626c 6520 746f 2075 7365 205b  ossible to use [
+00001620: 736e 6170 7368 6f74 735d 2868 7474 7073  snapshots](https
+00001630: 3a2f 2f76 6173 7464 6174 612e 636f 6d2f  ://vastdata.com/
+00001640: 626c 6f67 2f62 7269 6e67 696e 672d 736e  blog/bringing-sn
+00001650: 6170 7368 6f74 732d 746f 2d76 6173 7473  apshots-to-vasts
+00001660: 2d65 6c65 6d65 6e74 2d73 746f 7265 2920  -element-store) 
+00001670: 666f 7220 6163 6365 7373 696e 6720 7468  for accessing th
+00001680: 6520 4461 7461 6261 7365 3a0a 0a60 6060  e Database:..```
+00001690: 7079 7468 6f6e 0a73 6e61 7073 203d 2062  python.snaps = b
+000016a0: 7563 6b65 742e 6c69 7374 5f73 6e61 7073  ucket.list_snaps
+000016b0: 686f 7473 2829 0a62 6174 6368 6573 203d  hots().batches =
+000016c0: 2073 6e61 7073 5b30 5d2e 7363 6865 6d61   snaps[0].schema
+000016d0: 2827 7363 6865 6d61 2d6e 616d 6527 292e  ('schema-name').
+000016e0: 7461 626c 6528 2774 6162 6c65 2d6e 616d  table('table-nam
+000016f0: 6527 292e 7365 6c65 6374 2829 0a60 6060  e').select().```
+00001700: 0a0a 2323 2056 4153 5420 4361 7461 6c6f  ..## VAST Catalo
+00001710: 670a 0a5b 5641 5354 2043 6174 616c 6f67  g..[VAST Catalog
+00001720: 5d28 6874 7470 733a 2f2f 7661 7374 6461  ](https://vastda
+00001730: 7461 2e63 6f6d 2f62 6c6f 672f 7661 7374  ta.com/blog/vast
+00001740: 2d63 6174 616c 6f67 2d74 7265 6174 2d79  -catalog-treat-y
+00001750: 6f75 722d 6669 6c65 2d73 7973 7465 6d2d  our-file-system-
+00001760: 6c69 6b65 2d61 2d64 6174 6162 6173 6529  like-a-database)
+00001770: 2063 616e 2062 6520 7175 6572 6965 6420   can be queried 
+00001780: 6173 2061 2072 6567 756c 6172 2074 6162  as a regular tab
+00001790: 6c65 3a0a 0a60 6060 7079 7468 6f6e 0a74  le:..```python.t
+000017a0: 6162 6c65 203d 2070 612e 5461 626c 652e  able = pa.Table.
+000017b0: 6672 6f6d 5f62 6174 6368 6573 2874 782e  from_batches(tx.
+000017c0: 6361 7461 6c6f 672e 7365 6c65 6374 285b  catalog.select([
+000017d0: 2765 6c65 6d65 6e74 5f74 7970 6527 5d29  'element_type'])
+000017e0: 290a 6466 203d 2074 6162 6c65 2e74 6f5f  ).df = table.to_
+000017f0: 7061 6e64 6173 2829 0a0a 746f 7461 6c5f  pandas()..total_
+00001800: 656c 656d 656e 7473 203d 206c 656e 2864  elements = len(d
+00001810: 6629 0a70 7269 6e74 2866 2254 6f74 616c  f).print(f"Total
+00001820: 2065 6c65 6d65 6e74 7320 696e 2074 6865   elements in the
+00001830: 2063 6174 616c 6f67 3a20 7b74 6f74 616c   catalog: {total
+00001840: 5f65 6c65 6d65 6e74 737d 2229 0a0a 6669  _elements}")..fi
+00001850: 6c65 5f63 6f75 6e74 203d 2028 6466 5b27  le_count = (df['
+00001860: 656c 656d 656e 745f 7479 7065 275d 203d  element_type'] =
+00001870: 3d20 2746 494c 4527 292e 7375 6d28 290a  = 'FILE').sum().
+00001880: 7072 696e 7428 6622 4e75 6d62 6572 206f  print(f"Number o
+00001890: 6620 6669 6c65 732f 6f62 6a65 6374 733a  f files/objects:
+000018a0: 207b 6669 6c65 5f63 6f75 6e74 7d22 290a   {file_count}").
+000018b0: 0a64 6973 7469 6e63 745f 656c 656d 656e  .distinct_elemen
+000018c0: 7473 203d 2064 665b 2765 6c65 6d65 6e74  ts = df['element
+000018d0: 5f74 7970 6527 5d2e 756e 6971 7565 2829  _type'].unique()
+000018e0: 0a70 7269 6e74 2822 4469 7374 696e 6374  .print("Distinct
+000018f0: 2065 6c65 6d65 6e74 2074 7970 6573 206f   element types o
+00001900: 6e20 7468 6520 7379 7374 656d 3a22 290a  n the system:").
+00001910: 7072 696e 7428 6469 7374 696e 6374 5f65  print(distinct_e
+00001920: 6c65 6d65 6e74 7329 0a60 6060 0a0a 5365  lements).```..Se
+00001930: 6520 7468 6520 666f 6c6c 6f77 696e 6720  e the following 
+00001940: 626c 6f67 2070 6f73 7473 2066 6f72 206d  blog posts for m
+00001950: 6f72 6520 6578 616d 706c 6573 3a0a 0a2d  ore examples:..-
+00001960: 2068 7474 7073 3a2f 2f76 6173 7464 6174   https://vastdat
+00001970: 612e 636f 6d2f 626c 6f67 2f74 6865 2d76  a.com/blog/the-v
+00001980: 6173 742d 6361 7461 6c6f 672d 696e 2d61  ast-catalog-in-a
+00001990: 6374 696f 6e2d 7061 7274 2d31 0a2d 2068  ction-part-1.- h
+000019a0: 7474 7073 3a2f 2f76 6173 7464 6174 612e  ttps://vastdata.
+000019b0: 636f 6d2f 626c 6f67 2f74 6865 2d76 6173  com/blog/the-vas
+000019c0: 742d 6361 7461 6c6f 672d 696e 2d61 6374  t-catalog-in-act
+000019d0: 696f 6e2d 7061 7274 2d32 0a0a 0a23 2320  ion-part-2...## 
+000019e0: 5265 7175 6972 6564 2056 4153 5420 7265  Required VAST re
+000019f0: 6c65 6173 650a 0a43 7572 7265 6e74 6c79  lease..Currently
+00001a00: 2c20 5641 5354 2044 4220 5079 7468 6f6e  , VAST DB Python
+00001a10: 2053 444b 2072 6571 7569 7265 7320 6035   SDK requires `5
+00001a20: 2e30 2e30 2d73 7031 3060 206f 7220 6c61  .0.0-sp10` or la
+00001a30: 7465 7220 5641 5354 2072 656c 6561 7365  ter VAST release
+00001a40: 2e0a 0a49 6620 7468 6520 636c 7573 7465  ...If the cluste
+00001a50: 7220 6973 2072 756e 6e69 6e67 2061 6e20  r is running an 
+00001a60: 6f6c 6465 7220 5641 5354 2072 656c 6561  older VAST relea
+00001a70: 7365 2c20 706c 6561 7365 2063 6f6e 7461  se, please conta
+00001a80: 6374 2063 7573 746f 6d65 722e 7375 7070  ct customer.supp
+00001a90: 6f72 7440 7661 7374 6461 7461 2e63 6f6d  ort@vastdata.com
+00001aa0: 2066 6f72 206d 6f72 6520 6465 7461 696c   for more detail
+00001ab0: 732e 0a                                  s..
```

### Comparing `vastdb-0.1.6/setup.py` & `vastdb-0.1.7/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 if os.environ.get('VASTDB_APPEND_VERSION_SUFFIX'):
     suffix = _get_version_suffix()
 
 setup(
     name='vastdb',
     python_requires='>=3.9.0',
     description='VAST Data SDK',
-    version='0.1.6' + suffix,
+    version='0.1.7' + suffix,
     url='https://github.com/vast-data/vastdb_sdk',
     author='VAST DATA',
     author_email='hello@vastdata.com',
     license='Copyright (C) VAST Data Ltd.',
     packages=find_packages(),
     install_requires=Path('requirements.txt').read_text().strip().split(),
     long_description=long_description,
```

### Comparing `vastdb-0.1.6/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Aggregate.py` & `vastdb-0.1.7/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Aggregate.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.6/vast_flatbuf/org/apache/arrow/computeir/flatbuf/ArraySlice.py` & `vastdb-0.1.7/vast_flatbuf/org/apache/arrow/computeir/flatbuf/ArraySlice.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.6/vast_flatbuf/org/apache/arrow/computeir/flatbuf/ArraySubscript.py` & `vastdb-0.1.7/vast_flatbuf/org/apache/arrow/computeir/flatbuf/ArraySubscript.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.6/vast_flatbuf/org/apache/arrow/computeir/flatbuf/BinaryLiteral.py` & `vastdb-0.1.7/vast_flatbuf/org/apache/arrow/computeir/flatbuf/BinaryLiteral.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.6/vast_flatbuf/org/apache/arrow/computeir/flatbuf/BooleanLiteral.py` & `vastdb-0.1.7/vast_flatbuf/org/apache/arrow/computeir/flatbuf/BooleanLiteral.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.6/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Call.py` & `vastdb-0.1.7/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Call.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.6/vast_flatbuf/org/apache/arrow/computeir/flatbuf/CaseFragment.py` & `vastdb-0.1.7/vast_flatbuf/org/apache/arrow/computeir/flatbuf/CaseFragment.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.6/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Cast.py` & `vastdb-0.1.7/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Cast.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.6/vast_flatbuf/org/apache/arrow/computeir/flatbuf/ConditionalCase.py` & `vastdb-0.1.7/vast_flatbuf/org/apache/arrow/computeir/flatbuf/ConditionalCase.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.6/vast_flatbuf/org/apache/arrow/computeir/flatbuf/CurrentRow.py` & `vastdb-0.1.7/vast_flatbuf/org/apache/arrow/computeir/flatbuf/CurrentRow.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.6/vast_flatbuf/org/apache/arrow/computeir/flatbuf/DateLiteral.py` & `vastdb-0.1.7/vast_flatbuf/org/apache/arrow/computeir/flatbuf/DateLiteral.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.6/vast_flatbuf/org/apache/arrow/computeir/flatbuf/DecimalLiteral.py` & `vastdb-0.1.7/vast_flatbuf/org/apache/arrow/computeir/flatbuf/DecimalLiteral.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.6/vast_flatbuf/org/apache/arrow/computeir/flatbuf/DurationLiteral.py` & `vastdb-0.1.7/vast_flatbuf/org/apache/arrow/computeir/flatbuf/DurationLiteral.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.6/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Expression.py` & `vastdb-0.1.7/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Expression.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.6/vast_flatbuf/org/apache/arrow/computeir/flatbuf/FieldIndex.py` & `vastdb-0.1.7/vast_flatbuf/org/apache/arrow/computeir/flatbuf/FieldIndex.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.6/vast_flatbuf/org/apache/arrow/computeir/flatbuf/FieldRef.py` & `vastdb-0.1.7/vast_flatbuf/org/apache/arrow/computeir/flatbuf/FieldRef.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.6/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Filter.py` & `vastdb-0.1.7/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Filter.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.6/vast_flatbuf/org/apache/arrow/computeir/flatbuf/FixedSizeBinaryLiteral.py` & `vastdb-0.1.7/vast_flatbuf/org/apache/arrow/computeir/flatbuf/FixedSizeBinaryLiteral.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.6/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Float16Literal.py` & `vastdb-0.1.7/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Float16Literal.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.6/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Float32Literal.py` & `vastdb-0.1.7/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Float32Literal.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.6/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Float64Literal.py` & `vastdb-0.1.7/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Float64Literal.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.6/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Following.py` & `vastdb-0.1.7/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Following.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.6/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Grouping.py` & `vastdb-0.1.7/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Grouping.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.6/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Int16Literal.py` & `vastdb-0.1.7/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Int16Literal.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.6/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Int32Literal.py` & `vastdb-0.1.7/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Int32Literal.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.6/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Int64Literal.py` & `vastdb-0.1.7/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Int64Literal.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.6/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Int8Literal.py` & `vastdb-0.1.7/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Int8Literal.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.6/vast_flatbuf/org/apache/arrow/computeir/flatbuf/IntervalLiteral.py` & `vastdb-0.1.7/vast_flatbuf/org/apache/arrow/computeir/flatbuf/IntervalLiteral.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.6/vast_flatbuf/org/apache/arrow/computeir/flatbuf/IntervalLiteralDaysMilliseconds.py` & `vastdb-0.1.7/vast_flatbuf/org/apache/arrow/computeir/flatbuf/IntervalLiteralDaysMilliseconds.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.6/vast_flatbuf/org/apache/arrow/computeir/flatbuf/IntervalLiteralMonths.py` & `vastdb-0.1.7/vast_flatbuf/org/apache/arrow/computeir/flatbuf/IntervalLiteralMonths.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.6/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Join.py` & `vastdb-0.1.7/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Join.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.6/vast_flatbuf/org/apache/arrow/computeir/flatbuf/KeyValue.py` & `vastdb-0.1.7/vast_flatbuf/org/apache/arrow/computeir/flatbuf/KeyValue.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.6/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Limit.py` & `vastdb-0.1.7/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Limit.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.6/vast_flatbuf/org/apache/arrow/computeir/flatbuf/ListLiteral.py` & `vastdb-0.1.7/vast_flatbuf/org/apache/arrow/computeir/flatbuf/ListLiteral.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.6/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Literal.py` & `vastdb-0.1.7/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Literal.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.6/vast_flatbuf/org/apache/arrow/computeir/flatbuf/LiteralColumn.py` & `vastdb-0.1.7/vast_flatbuf/org/apache/arrow/computeir/flatbuf/LiteralColumn.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.6/vast_flatbuf/org/apache/arrow/computeir/flatbuf/LiteralImpl.py` & `vastdb-0.1.7/vast_flatbuf/org/apache/arrow/computeir/flatbuf/LiteralImpl.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.6/vast_flatbuf/org/apache/arrow/computeir/flatbuf/LiteralRelation.py` & `vastdb-0.1.7/vast_flatbuf/org/apache/arrow/computeir/flatbuf/LiteralRelation.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.6/vast_flatbuf/org/apache/arrow/computeir/flatbuf/MapKey.py` & `vastdb-0.1.7/vast_flatbuf/org/apache/arrow/computeir/flatbuf/MapKey.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.6/vast_flatbuf/org/apache/arrow/computeir/flatbuf/MapLiteral.py` & `vastdb-0.1.7/vast_flatbuf/org/apache/arrow/computeir/flatbuf/MapLiteral.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.6/vast_flatbuf/org/apache/arrow/computeir/flatbuf/OrderBy.py` & `vastdb-0.1.7/vast_flatbuf/org/apache/arrow/computeir/flatbuf/OrderBy.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.6/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Plan.py` & `vastdb-0.1.7/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Plan.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.6/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Preceding.py` & `vastdb-0.1.7/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Preceding.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.6/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Project.py` & `vastdb-0.1.7/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Project.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.6/vast_flatbuf/org/apache/arrow/computeir/flatbuf/RelId.py` & `vastdb-0.1.7/vast_flatbuf/org/apache/arrow/computeir/flatbuf/RelId.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.6/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Relation.py` & `vastdb-0.1.7/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Relation.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.6/vast_flatbuf/org/apache/arrow/computeir/flatbuf/SetOperation.py` & `vastdb-0.1.7/vast_flatbuf/org/apache/arrow/computeir/flatbuf/SetOperation.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.6/vast_flatbuf/org/apache/arrow/computeir/flatbuf/SimpleCase.py` & `vastdb-0.1.7/vast_flatbuf/org/apache/arrow/computeir/flatbuf/SimpleCase.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.6/vast_flatbuf/org/apache/arrow/computeir/flatbuf/SortKey.py` & `vastdb-0.1.7/vast_flatbuf/org/apache/arrow/computeir/flatbuf/SortKey.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.6/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Source.py` & `vastdb-0.1.7/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Source.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.6/vast_flatbuf/org/apache/arrow/computeir/flatbuf/StringLiteral.py` & `vastdb-0.1.7/vast_flatbuf/org/apache/arrow/computeir/flatbuf/StringLiteral.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.6/vast_flatbuf/org/apache/arrow/computeir/flatbuf/StructField.py` & `vastdb-0.1.7/vast_flatbuf/org/apache/arrow/computeir/flatbuf/StructField.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.6/vast_flatbuf/org/apache/arrow/computeir/flatbuf/StructLiteral.py` & `vastdb-0.1.7/vast_flatbuf/org/apache/arrow/computeir/flatbuf/StructLiteral.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.6/vast_flatbuf/org/apache/arrow/computeir/flatbuf/TimeLiteral.py` & `vastdb-0.1.7/vast_flatbuf/org/apache/arrow/computeir/flatbuf/TimeLiteral.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.6/vast_flatbuf/org/apache/arrow/computeir/flatbuf/TimestampLiteral.py` & `vastdb-0.1.7/vast_flatbuf/org/apache/arrow/computeir/flatbuf/TimestampLiteral.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.6/vast_flatbuf/org/apache/arrow/computeir/flatbuf/UInt16Literal.py` & `vastdb-0.1.7/vast_flatbuf/org/apache/arrow/computeir/flatbuf/UInt16Literal.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.6/vast_flatbuf/org/apache/arrow/computeir/flatbuf/UInt32Literal.py` & `vastdb-0.1.7/vast_flatbuf/org/apache/arrow/computeir/flatbuf/UInt32Literal.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.6/vast_flatbuf/org/apache/arrow/computeir/flatbuf/UInt64Literal.py` & `vastdb-0.1.7/vast_flatbuf/org/apache/arrow/computeir/flatbuf/UInt64Literal.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.6/vast_flatbuf/org/apache/arrow/computeir/flatbuf/UInt8Literal.py` & `vastdb-0.1.7/vast_flatbuf/org/apache/arrow/computeir/flatbuf/UInt8Literal.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.6/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Unbounded.py` & `vastdb-0.1.7/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Unbounded.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.6/vast_flatbuf/org/apache/arrow/computeir/flatbuf/WindowCall.py` & `vastdb-0.1.7/vast_flatbuf/org/apache/arrow/computeir/flatbuf/WindowCall.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.6/vast_flatbuf/org/apache/arrow/flatbuf/Binary.py` & `vastdb-0.1.7/vast_flatbuf/org/apache/arrow/flatbuf/Binary.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.6/vast_flatbuf/org/apache/arrow/flatbuf/Block.py` & `vastdb-0.1.7/vast_flatbuf/org/apache/arrow/flatbuf/Block.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.6/vast_flatbuf/org/apache/arrow/flatbuf/BodyCompression.py` & `vastdb-0.1.7/vast_flatbuf/org/apache/arrow/flatbuf/BodyCompression.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.6/vast_flatbuf/org/apache/arrow/flatbuf/BodyCompressionMethod.py` & `vastdb-0.1.7/vast_flatbuf/org/apache/arrow/flatbuf/BodyCompressionMethod.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.6/vast_flatbuf/org/apache/arrow/flatbuf/Bool.py` & `vastdb-0.1.7/vast_flatbuf/org/apache/arrow/flatbuf/Bool.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.6/vast_flatbuf/org/apache/arrow/flatbuf/Buffer.py` & `vastdb-0.1.7/vast_flatbuf/org/apache/arrow/flatbuf/Buffer.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.6/vast_flatbuf/org/apache/arrow/flatbuf/Date.py` & `vastdb-0.1.7/vast_flatbuf/org/apache/arrow/flatbuf/Date.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.6/vast_flatbuf/org/apache/arrow/flatbuf/Decimal.py` & `vastdb-0.1.7/vast_flatbuf/org/apache/arrow/flatbuf/Decimal.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.6/vast_flatbuf/org/apache/arrow/flatbuf/DictionaryBatch.py` & `vastdb-0.1.7/vast_flatbuf/org/apache/arrow/flatbuf/DictionaryBatch.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.6/vast_flatbuf/org/apache/arrow/flatbuf/DictionaryEncoding.py` & `vastdb-0.1.7/vast_flatbuf/org/apache/arrow/flatbuf/DictionaryEncoding.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.6/vast_flatbuf/org/apache/arrow/flatbuf/Duration.py` & `vastdb-0.1.7/vast_flatbuf/org/apache/arrow/flatbuf/Duration.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.6/vast_flatbuf/org/apache/arrow/flatbuf/Feature.py` & `vastdb-0.1.7/vast_flatbuf/org/apache/arrow/flatbuf/Feature.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.6/vast_flatbuf/org/apache/arrow/flatbuf/Field.py` & `vastdb-0.1.7/vast_flatbuf/org/apache/arrow/flatbuf/Field.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.6/vast_flatbuf/org/apache/arrow/flatbuf/FieldNode.py` & `vastdb-0.1.7/vast_flatbuf/org/apache/arrow/flatbuf/FieldNode.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.6/vast_flatbuf/org/apache/arrow/flatbuf/FixedSizeBinary.py` & `vastdb-0.1.7/vast_flatbuf/org/apache/arrow/flatbuf/FixedSizeBinary.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.6/vast_flatbuf/org/apache/arrow/flatbuf/FixedSizeList.py` & `vastdb-0.1.7/vast_flatbuf/org/apache/arrow/flatbuf/FixedSizeList.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.6/vast_flatbuf/org/apache/arrow/flatbuf/FloatingPoint.py` & `vastdb-0.1.7/vast_flatbuf/org/apache/arrow/flatbuf/FloatingPoint.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.6/vast_flatbuf/org/apache/arrow/flatbuf/Footer.py` & `vastdb-0.1.7/vast_flatbuf/org/apache/arrow/flatbuf/Footer.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.6/vast_flatbuf/org/apache/arrow/flatbuf/Int.py` & `vastdb-0.1.7/vast_flatbuf/org/apache/arrow/flatbuf/Int.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.6/vast_flatbuf/org/apache/arrow/flatbuf/Interval.py` & `vastdb-0.1.7/vast_flatbuf/org/apache/arrow/flatbuf/Interval.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.6/vast_flatbuf/org/apache/arrow/flatbuf/KeyValue.py` & `vastdb-0.1.7/vast_flatbuf/org/apache/arrow/flatbuf/KeyValue.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.6/vast_flatbuf/org/apache/arrow/flatbuf/LargeBinary.py` & `vastdb-0.1.7/vast_flatbuf/org/apache/arrow/flatbuf/LargeBinary.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.6/vast_flatbuf/org/apache/arrow/flatbuf/LargeList.py` & `vastdb-0.1.7/vast_flatbuf/org/apache/arrow/flatbuf/LargeList.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.6/vast_flatbuf/org/apache/arrow/flatbuf/LargeUtf8.py` & `vastdb-0.1.7/vast_flatbuf/org/apache/arrow/flatbuf/LargeUtf8.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.6/vast_flatbuf/org/apache/arrow/flatbuf/List.py` & `vastdb-0.1.7/vast_flatbuf/org/apache/arrow/flatbuf/List.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.6/vast_flatbuf/org/apache/arrow/flatbuf/Map.py` & `vastdb-0.1.7/vast_flatbuf/org/apache/arrow/flatbuf/Map.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.6/vast_flatbuf/org/apache/arrow/flatbuf/Message.py` & `vastdb-0.1.7/vast_flatbuf/org/apache/arrow/flatbuf/Message.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.6/vast_flatbuf/org/apache/arrow/flatbuf/MessageHeader.py` & `vastdb-0.1.7/vast_flatbuf/org/apache/arrow/flatbuf/MessageHeader.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.6/vast_flatbuf/org/apache/arrow/flatbuf/MetadataVersion.py` & `vastdb-0.1.7/vast_flatbuf/org/apache/arrow/flatbuf/MetadataVersion.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.6/vast_flatbuf/org/apache/arrow/flatbuf/Null.py` & `vastdb-0.1.7/vast_flatbuf/org/apache/arrow/flatbuf/Null.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.6/vast_flatbuf/org/apache/arrow/flatbuf/RecordBatch.py` & `vastdb-0.1.7/vast_flatbuf/org/apache/arrow/flatbuf/RecordBatch.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.6/vast_flatbuf/org/apache/arrow/flatbuf/Schema.py` & `vastdb-0.1.7/vast_flatbuf/org/apache/arrow/flatbuf/Schema.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.6/vast_flatbuf/org/apache/arrow/flatbuf/SparseMatrixIndexCSX.py` & `vastdb-0.1.7/vast_flatbuf/org/apache/arrow/flatbuf/SparseMatrixIndexCSX.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.6/vast_flatbuf/org/apache/arrow/flatbuf/SparseTensor.py` & `vastdb-0.1.7/vast_flatbuf/org/apache/arrow/flatbuf/SparseTensor.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.6/vast_flatbuf/org/apache/arrow/flatbuf/SparseTensorIndexCOO.py` & `vastdb-0.1.7/vast_flatbuf/org/apache/arrow/flatbuf/SparseTensorIndexCOO.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.6/vast_flatbuf/org/apache/arrow/flatbuf/SparseTensorIndexCSF.py` & `vastdb-0.1.7/vast_flatbuf/org/apache/arrow/flatbuf/SparseTensorIndexCSF.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.6/vast_flatbuf/org/apache/arrow/flatbuf/Struct_.py` & `vastdb-0.1.7/vast_flatbuf/org/apache/arrow/flatbuf/Struct_.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.6/vast_flatbuf/org/apache/arrow/flatbuf/Tensor.py` & `vastdb-0.1.7/vast_flatbuf/org/apache/arrow/flatbuf/Tensor.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.6/vast_flatbuf/org/apache/arrow/flatbuf/TensorDim.py` & `vastdb-0.1.7/vast_flatbuf/org/apache/arrow/flatbuf/TensorDim.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.6/vast_flatbuf/org/apache/arrow/flatbuf/Time.py` & `vastdb-0.1.7/vast_flatbuf/org/apache/arrow/flatbuf/Time.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.6/vast_flatbuf/org/apache/arrow/flatbuf/Timestamp.py` & `vastdb-0.1.7/vast_flatbuf/org/apache/arrow/flatbuf/Timestamp.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.6/vast_flatbuf/org/apache/arrow/flatbuf/Type.py` & `vastdb-0.1.7/vast_flatbuf/org/apache/arrow/flatbuf/Type.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.6/vast_flatbuf/org/apache/arrow/flatbuf/Union.py` & `vastdb-0.1.7/vast_flatbuf/org/apache/arrow/flatbuf/Union.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.6/vast_flatbuf/org/apache/arrow/flatbuf/Utf8.py` & `vastdb-0.1.7/vast_flatbuf/org/apache/arrow/flatbuf/Utf8.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.6/vast_flatbuf/tabular/AlterColumnRequest.py` & `vastdb-0.1.7/vast_flatbuf/tabular/AlterColumnRequest.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.6/vast_flatbuf/tabular/AlterProjectionTableRequest.py` & `vastdb-0.1.7/vast_flatbuf/tabular/AlterProjectionTableRequest.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.6/vast_flatbuf/tabular/AlterSchemaRequest.py` & `vastdb-0.1.7/vast_flatbuf/tabular/AlterSchemaRequest.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.6/vast_flatbuf/tabular/AlterTableRequest.py` & `vastdb-0.1.7/vast_flatbuf/tabular/AlterTableRequest.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.6/vast_flatbuf/tabular/Column.py` & `vastdb-0.1.7/vast_flatbuf/tabular/Column.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.6/vast_flatbuf/tabular/CreateProjectionRequest.py` & `vastdb-0.1.7/vast_flatbuf/tabular/CreateProjectionRequest.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.6/vast_flatbuf/tabular/CreateSchemaRequest.py` & `vastdb-0.1.7/vast_flatbuf/tabular/CreateSchemaRequest.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.6/vast_flatbuf/tabular/GetProjectionTableStatsResponse.py` & `vastdb-0.1.7/vast_flatbuf/tabular/GetProjectionTableStatsResponse.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.6/vast_flatbuf/tabular/GetTableStatsResponse.py` & `vastdb-0.1.7/vast_flatbuf/tabular/GetTableStatsResponse.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.6/vast_flatbuf/tabular/ImportDataRequest.py` & `vastdb-0.1.7/vast_flatbuf/tabular/ImportDataRequest.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.6/vast_flatbuf/tabular/ListProjectionsResponse.py` & `vastdb-0.1.7/vast_flatbuf/tabular/ListProjectionsResponse.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.6/vast_flatbuf/tabular/ListSchemasResponse.py` & `vastdb-0.1.7/vast_flatbuf/tabular/ListSchemasResponse.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.6/vast_flatbuf/tabular/ListTablesResponse.py` & `vastdb-0.1.7/vast_flatbuf/tabular/ListTablesResponse.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.6/vast_flatbuf/tabular/ObjectDetails.py` & `vastdb-0.1.7/vast_flatbuf/tabular/ObjectDetails.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.6/vast_flatbuf/tabular/S3File.py` & `vastdb-0.1.7/vast_flatbuf/tabular/S3File.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.6/vast_flatbuf/tabular/VipRange.py` & `vastdb-0.1.7/vast_flatbuf/tabular/VipRange.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.6/vastdb/bench/test_perf.py` & `vastdb-0.1.7/vastdb/bench/test_perf.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.6/vastdb/bucket.py` & `vastdb-0.1.7/vastdb/bucket.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 VAST S3 buckets can be used to create Database schemas and tables.
 It is possible to list and access VAST snapshots generated over a bucket.
 """
 
 import logging
 from dataclasses import dataclass, field
-from typing import TYPE_CHECKING, List, Optional
+from typing import TYPE_CHECKING, Iterable, Optional
 
 from . import errors, schema, transaction
 
 if TYPE_CHECKING:
     from .schema import Schema
 
 log = logging.getLogger(__name__)
@@ -51,15 +51,15 @@
             if fail_if_missing:
                 raise errors.MissingSnapshot(self.name, expected_name)
             else:
                 return None
 
         return Bucket(name=f'{self.name}/{expected_name}', tx=self.tx)
 
-    def snapshots(self) -> List["Bucket"]:
+    def snapshots(self) -> Iterable["Bucket"]:
         """List bucket's snapshots."""
         snapshots = []
         next_key = 0
         while True:
             curr_snapshots, is_truncated, next_key = \
                 self.tx._rpc.api.list_snapshots(bucket=self.name, next_token=next_key)
             if not curr_snapshots:
```

### Comparing `vastdb-0.1.6/vastdb/conftest.py` & `vastdb-0.1.7/vastdb/conftest.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.6/vastdb/errors.py` & `vastdb-0.1.7/vastdb/errors.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.6/vastdb/internal_commands.py` & `vastdb-0.1.7/vastdb/_internal.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,25 +1,45 @@
 import itertools
 import json
 import logging
 import re
 import struct
 import urllib.parse
 from collections import defaultdict, namedtuple
+from dataclasses import dataclass, field
 from enum import Enum
-from typing import Any, Dict, Iterator, List, Optional, Union
+from typing import Any, Callable, Dict, Iterator, List, Optional, Tuple, Union
 
+import backoff
 import flatbuffers
 import ibis
 import pyarrow as pa
-import pyarrow.parquet as pq
 import requests
 import urllib3
 import xmltodict
 from aws_requests_auth.aws_auth import AWSRequestsAuth
+from ibis.expr.operations.generic import (
+    IsNull,
+    Literal,
+)
+from ibis.expr.operations.logical import (
+    And,
+    Between,
+    Equals,
+    Greater,
+    GreaterEqual,
+    InValues,
+    Less,
+    LessEqual,
+    Not,
+    NotEquals,
+    Or,
+)
+from ibis.expr.operations.relations import Field
+from ibis.expr.operations.strings import StringContains
 
 import vast_flatbuf.org.apache.arrow.computeir.flatbuf.BinaryLiteral as fb_binary_lit
 import vast_flatbuf.org.apache.arrow.computeir.flatbuf.BooleanLiteral as fb_bool_lit
 import vast_flatbuf.org.apache.arrow.computeir.flatbuf.Call as fb_call
 import vast_flatbuf.org.apache.arrow.computeir.flatbuf.DateLiteral as fb_date32_lit
 import vast_flatbuf.org.apache.arrow.computeir.flatbuf.DecimalLiteral as fb_decimal_lit
 import vast_flatbuf.org.apache.arrow.computeir.flatbuf.Expression as fb_expression
@@ -133,34 +153,14 @@
         # Arrow schema contains the top-level columns, where each column may include multiple subfields
         # We use DFS is used to enumerate all the sub-columns, using `index` as an ID allocator
         nodes = [FieldNode(field, index) for field in schema]
         self.nodes_map = {node.field.name: node for node in nodes}
         self.expr = expr
 
     def serialize(self, builder: 'flatbuffers.builder.Builder'):
-        from ibis.expr.operations.generic import (
-            IsNull,
-            Literal,
-            TableColumn,
-        )
-        from ibis.expr.operations.logical import (
-            And,
-            Between,
-            Equals,
-            Greater,
-            GreaterEqual,
-            InValues,
-            Less,
-            LessEqual,
-            Not,
-            NotEquals,
-            Or,
-        )
-        from ibis.expr.operations.strings import StringContains
-
         builder_map = {
             Greater: self.build_greater,
             GreaterEqual: self.build_greater_equal,
             Less: self.build_less,
             LessEqual: self.build_less_equal,
             Equals: self.build_equal,
             NotEquals: self.build_not_equal,
@@ -212,15 +212,15 @@
                             literals = arg
                         else:
                             literals = (arg,)
                         for literal in literals:
                             if not isinstance(literal, Literal):
                                 raise NotImplementedError(self.expr)
 
-                    if not isinstance(column, TableColumn):
+                    if not isinstance(column, Field):
                         raise NotImplementedError(self.expr)
 
                     field_name = column.name
                     if prev_field_name is None:
                         prev_field_name = field_name
                     elif prev_field_name != field_name:
                         raise NotImplementedError(self.expr)
@@ -718,73 +718,111 @@
 
 # Results that returns from tablestats
 
 
 TableStatsResult = namedtuple("TableStatsResult", ["num_rows", "size_in_bytes", "is_external_rowid_alloc", "endpoints"])
 
 
+def _backoff_giveup(exc: Exception) -> bool:
+
+    if isinstance(exc, errors.Slowdown):
+        # the server is overloaded, retry later
+        return False
+
+    if isinstance(exc, requests.exceptions.ConnectionError):
+        if exc.request.method == "GET":
+            # low-level connection issue, it is safe to retry only read-only requests
+            return False
+
+    return True  # giveup in case of other exceptions
+
+
+@dataclass
+class BackoffConfig:
+    wait_gen: Callable = field(default=backoff.expo)
+    max_tries: int = 10
+    max_time: float = 60.0  # in seconds
+    backoff_log_level: int = logging.DEBUG
+
+
 class VastdbApi:
     # we expect the vast version to be <major>.<minor>.<patch>.<protocol>
     VAST_VERSION_REGEX = re.compile(r'^vast (\d+\.\d+\.\d+\.\d+)$')
 
-    def __init__(self, endpoint, access_key, secret_key, auth_type=AuthType.SIGV4, ssl_verify=True):
+    def __init__(self, endpoint, access_key, secret_key,
+            *,
+            auth_type=AuthType.SIGV4,
+            ssl_verify=True,
+            backoff_config: Optional[BackoffConfig] = None):
+
+        from . import __version__  # import lazily here (to avoid circular dependencies)
+        self.client_sdk_version = f"VAST Database Python SDK {__version__} - 2024 (c)"
+
         url = urllib3.util.parse_url(endpoint)
         self.access_key = access_key
         self.secret_key = secret_key
 
         self.default_max_list_columns_page_size = 1000
-        self.session = requests.Session()
-        self.session.verify = ssl_verify
-        self.session.headers['user-agent'] = "VastData Tabular API 1.0 - 2022 (c)"
+        self._session = requests.Session()
+        self._session.verify = ssl_verify
+        self._session.headers['user-agent'] = self.client_sdk_version
+
+        backoff_config = backoff_config or BackoffConfig()
+        backoff_decorator = backoff.on_exception(
+            wait_gen=backoff_config.wait_gen,
+            exception=(requests.exceptions.ConnectionError, errors.Slowdown),
+            giveup=_backoff_giveup,
+            max_tries=backoff_config.max_tries,
+            max_time=backoff_config.max_time,
+            backoff_log_level=backoff_config.backoff_log_level)
+        self._request = backoff_decorator(self._single_request)
 
         if url.port in {80, 443, None}:
             self.aws_host = f'{url.host}'
         else:
             self.aws_host = f'{url.host}:{url.port}'
 
         self.url = str(url)
         _logger.debug('url=%s aws_host=%s', self.url, self.aws_host)
 
-        self.session.auth = AWSRequestsAuth(aws_access_key=access_key,
+        self._session.auth = AWSRequestsAuth(aws_access_key=access_key,
                                             aws_secret_access_key=secret_key,
                                             aws_host=self.aws_host,
-                                            aws_region='us-east-1',
+                                            aws_region='',
                                             aws_service='s3')
 
         # probe the cluster for its version
-        self.vast_version = None
-        res = self.session.get(self.url)
+        res = self._request(method="GET", url=self._url(command="transaction"), skip_status_check=True)  # used only for the response headers
+        _logger.debug("headers=%s code=%s content=%s", res.headers, res.status_code, res.content)
         server_header = res.headers.get("Server")
         if server_header is None:
             _logger.error("Response doesn't contain 'Server' header")
         else:
-            _logger.debug("Server header is '%s'", server_header)
             if m := self.VAST_VERSION_REGEX.match(server_header):
-                self.vast_version, = m.groups()
+                self.vast_version: Tuple[int, ...] = tuple(int(v) for v in m.group(1).split("."))
                 return
             else:
                 _logger.error("'Server' header '%s' doesn't match the expected pattern", server_header)
 
         msg = (
             f'Please use `vastdb` <= 0.0.5.x with current VAST cluster version ("{server_header or "N/A"}"). '
             'To use the latest SDK, please upgrade your cluster to the latest service pack. '
             'Please contact customer.support@vastdata.com for more details.'
         )
         _logger.critical(msg)
         raise NotImplementedError(msg)
 
-    def update_mgmt_session(self, access_key: str, secret_key: str, auth_type=AuthType.SIGV4):
-        if auth_type != AuthType.BASIC:
-            self.session.auth = AWSRequestsAuth(aws_access_key=access_key,
-                                                aws_secret_access_key=secret_key,
-                                                aws_host=self.aws_host,
-                                                aws_region='us-east-1',
-                                                aws_service='s3')
+    def _single_request(self, *, method, url, skip_status_check=False, **kwargs):
+        res = self._session.request(method=method, url=url, **kwargs)
+        if not skip_status_check:
+            if exc := errors.from_response(res):
+                raise exc  # application-level error
+        return res  # successful response
 
-    def _api_prefix(self, bucket="", schema="", table="", command="", url_params={}):
+    def _url(self, bucket="", schema="", table="", command="", url_params={}):
         prefix_list = [self.url]
         if len(bucket):
             prefix_list.append(bucket)
 
         if len(schema):
             prefix_list.append(schema)
 
@@ -811,19 +849,14 @@
             'tabular-txid': str(txid),
             'tabular-api-version-id': str(version_id),
             'tabular-client-name': 'tabular-api'
         }
 
         return common_headers | {f'tabular-client-tags-{index}': tag for index, tag in enumerate(client_tags)}
 
-    def _check_res(self, res, cmd="", expected_retvals=[]):
-        if exc := errors.from_response(res):
-            raise exc
-        return res
-
     def create_schema(self, bucket, name, txid=0, client_tags=[], schema_properties="", expected_retvals=[]):
         """
         Create a collection of tables, use the following request
         POST /bucket/schema?schema HTTP/1.1
 
         The body of the POST request contains schema properties as flatbuffer
         Request Headers
@@ -837,18 +870,18 @@
         tabular_create_schema.AddProperties(builder, properties_offset)
         params = tabular_create_schema.End(builder)
         builder.Finish(params)
         create_schema_req = builder.Output()
 
         headers = self._fill_common_headers(txid=txid, client_tags=client_tags)
         headers['Content-Length'] = str(len(create_schema_req))
-        res = self.session.post(self._api_prefix(bucket=bucket, schema=name, command="schema"),
-                                data=create_schema_req, headers=headers, stream=True)
-
-        return self._check_res(res, "create_schema", expected_retvals)
+        self._request(
+            method="POST",
+            url=self._url(bucket=bucket, schema=name, command="schema"),
+            data=create_schema_req, headers=headers)
 
     def alter_schema(self, bucket, name, txid=0, client_tags=[], schema_properties="", new_name="", expected_retvals=[]):
         """
         ALTER an existing schema name and/or properties
         PUT /bucket/schema?schema&tabular-new-schema-name=NewSchemaName HTTP/1.1
 
         Request Headers
@@ -866,31 +899,32 @@
         builder.Finish(params)
         alter_schema_req = builder.Output()
 
         headers = self._fill_common_headers(txid=txid, client_tags=client_tags)
         headers['Content-Length'] = str(len(alter_schema_req))
         url_params = {'tabular-new-schema-name': new_name} if len(new_name) else {}
 
-        res = self.session.put(self._api_prefix(bucket=bucket, schema=name, command="schema", url_params=url_params),
-                               data=alter_schema_req, headers=headers)
-
-        return self._check_res(res, "alter_schema", expected_retvals)
+        self._request(
+            method="PUT",
+            url=self._url(bucket=bucket, schema=name, command="schema", url_params=url_params),
+            data=alter_schema_req, headers=headers)
 
     def drop_schema(self, bucket, name, txid=0, client_tags=[], expected_retvals=[]):
         """
         Drop (delete) a schema
         DELETE /bucket/schema?schema HTTP/1.1
 
         Request Headers
         """
         headers = self._fill_common_headers(txid=txid, client_tags=client_tags)
 
-        res = self.session.delete(self._api_prefix(bucket=bucket, schema=name, command="schema"), headers=headers)
-
-        return self._check_res(res, "drop_schema", expected_retvals)
+        self._request(
+            method="DELETE",
+            url=self._url(bucket=bucket, schema=name, command="schema"),
+            headers=headers)
 
     def list_schemas(self, bucket, schema="", txid=0, client_tags=[], max_keys=1000, next_key=0, name_prefix="",
                      exact_match=False, expected_retvals=[], count_only=False):
         """
         List all schemas
         GET /bucket/schema_path?schema HTTP/1.1
 
@@ -911,42 +945,45 @@
         else:
             headers['tabular-name-prefix'] = name_prefix
 
         headers['tabular-list-count-only'] = str(count_only)
 
         schemas = []
         schema = schema or ""
-        res = self.session.get(self._api_prefix(bucket=bucket, schema=schema, command="schema"), headers=headers, stream=True)
-        self._check_res(res, "list_schemas", expected_retvals)
-        if res.status_code == 200:
-            res_headers = res.headers
-            next_key = int(res_headers['tabular-next-key'])
-            is_truncated = res_headers['tabular-is-truncated'] == 'true'
-            lists = list_schemas.GetRootAs(res.content)
-            bucket_name = lists.BucketName().decode()
-            if not bucket.startswith(bucket_name):
-                raise ValueError(f'bucket: {bucket} did not start from {bucket_name}')
-            schemas_length = lists.SchemasLength()
-            count = int(res_headers['tabular-list-count']) if 'tabular-list-count' in res_headers else schemas_length
-            for i in range(schemas_length):
-                schema_obj = lists.Schemas(i)
-                name = schema_obj.Name().decode()
-                properties = schema_obj.Properties().decode()
-                schemas.append([name, properties])
+        res = self._request(
+            method="GET",
+            url=self._url(bucket=bucket, schema=schema, command="schema"),
+            headers=headers)
+
+        res_headers = res.headers
+        next_key = int(res_headers['tabular-next-key'])
+        is_truncated = res_headers['tabular-is-truncated'] == 'true'
+        lists = list_schemas.GetRootAs(res.content)
+        bucket_name = lists.BucketName().decode()
+        if not bucket.startswith(bucket_name):
+            raise ValueError(f'bucket: {bucket} did not start from {bucket_name}')
+        schemas_length = lists.SchemasLength()
+        count = int(res_headers['tabular-list-count']) if 'tabular-list-count' in res_headers else schemas_length
+        for i in range(schemas_length):
+            schema_obj = lists.Schemas(i)
+            name = schema_obj.Name().decode()
+            properties = schema_obj.Properties().decode()
+            schemas.append([name, properties])
 
-            return bucket_name, schemas, next_key, is_truncated, count
+        return bucket_name, schemas, next_key, is_truncated, count
 
     def list_snapshots(self, bucket, max_keys=1000, next_token=None, name_prefix=''):
         next_token = next_token or ''
         url_params = {'list_type': '2', 'prefix': '.snapshot/' + name_prefix, 'delimiter': '/', 'max_keys': str(max_keys)}
         if next_token:
             url_params['continuation-token'] = next_token
 
-        res = self.session.get(self._api_prefix(bucket=bucket, command="list", url_params=url_params), headers={}, stream=True)
-        self._check_res(res, "list_snapshots")
+        res = self._request(
+            method="GET",
+            url=self._url(bucket=bucket, command="list", url_params=url_params))
 
         xml_str = res.content.decode()
         xml_dict = xmltodict.parse(xml_str)
         list_res = xml_dict['ListBucketResult']
         is_truncated = list_res['IsTruncated'] == 'true'
         marker = list_res['Marker']
         common_prefixes = list_res.get('CommonPrefixes', [])
@@ -981,54 +1018,33 @@
         if use_external_row_ids_allocation:
             headers['use-external-row-ids-alloc'] = str(use_external_row_ids_allocation)
 
         url_params = {'topic_partitions': str(topic_partitions)} if topic_partitions else {}
         if create_imports_table:
             url_params['sub-table'] = IMPORTED_OBJECTS_TABLE_NAME
 
-        res = self.session.post(self._api_prefix(bucket=bucket, schema=schema, table=name, command="table", url_params=url_params),
-                                data=serialized_schema, headers=headers)
-        return self._check_res(res, "create_table", expected_retvals)
-
-    def create_table_from_parquet_schema(self, bucket, schema, name, parquet_path=None,
-                                         parquet_bucket_name=None, parquet_object_name=None,
-                                         txid=0, client_tags=[], expected_retvals=[]):
-
-        # Use pyarrow.parquet.ParquetDataset to open the Parquet file
-        if parquet_path:
-            parquet_ds = pq.ParquetDataset(parquet_path)
-        elif parquet_bucket_name and parquet_object_name:
-            s3fs = pa.fs.S3FileSystem(access_key=self.access_key, secret_key=self.secret_key, endpoint_override=self.url)
-            parquet_ds = pq.ParquetDataset('/'.join([parquet_bucket_name, parquet_object_name]), filesystem=s3fs)
-        else:
-            raise RuntimeError(f'invalid params parquet_path={parquet_path} parquet_bucket_name={parquet_bucket_name} parquet_object_name={parquet_object_name}')
-
-        # Get the schema of the Parquet file
-        if isinstance(parquet_ds.schema, pq.ParquetSchema):
-            arrow_schema = parquet_ds.schema.to_arrow_schema()
-        elif isinstance(parquet_ds.schema, pa.Schema):
-            arrow_schema = parquet_ds.schema
-        else:
-            raise RuntimeError(f'invalid type(parquet_ds.schema) = {type(parquet_ds.schema)}')
-
-        # create the table
-        return self.create_table(bucket, schema, name, arrow_schema, txid, client_tags, expected_retvals)
+        self._request(
+            method="POST",
+            url=self._url(bucket=bucket, schema=schema, table=name, command="table", url_params=url_params),
+            data=serialized_schema, headers=headers)
 
     def get_table_stats(self, bucket, schema, name, txid=0, client_tags=[], expected_retvals=[], imports_table_stats=False):
         """
         GET /mybucket/myschema/mytable?stats HTTP/1.1
         tabular-txid: TransactionId
         tabular-client-tag: ClientTag
 
         The Command will return the statistics in flatbuf format
         """
         headers = self._fill_common_headers(txid=txid, client_tags=client_tags)
         url_params = {'sub-table': IMPORTED_OBJECTS_TABLE_NAME} if imports_table_stats else {}
-        res = self.session.get(self._api_prefix(bucket=bucket, schema=schema, table=name, command="stats", url_params=url_params), headers=headers)
-        self._check_res(res, "get_table_stats", expected_retvals)
+        res = self._request(
+            method="GET",
+            url=self._url(bucket=bucket, schema=schema, table=name, command="stats", url_params=url_params),
+            headers=headers)
 
         stats = get_table_stats.GetRootAs(res.content)
         num_rows = stats.NumRows()
         size_in_bytes = stats.SizeInBytes()
         is_external_rowid_alloc = stats.IsExternalRowidAlloc()
         endpoints = [self.url]  # we cannot replace the host by a VIP address in HTTPS-based URLs
         return TableStatsResult(num_rows, size_in_bytes, is_external_rowid_alloc, tuple(endpoints))
@@ -1055,33 +1071,34 @@
         builder.Finish(params)
         alter_table_req = builder.Output()
 
         headers = self._fill_common_headers(txid=txid, client_tags=client_tags)
         headers['Content-Length'] = str(len(alter_table_req))
         url_params = {'tabular-new-table-name': schema + "/" + new_name} if len(new_name) else {}
 
-        res = self.session.put(self._api_prefix(bucket=bucket, schema=schema, table=name, command="table", url_params=url_params),
-                               data=alter_table_req, headers=headers)
-
-        return self._check_res(res, "alter_table", expected_retvals)
+        self._request(
+            method="PUT",
+            url=self._url(bucket=bucket, schema=schema, table=name, command="table", url_params=url_params),
+            data=alter_table_req, headers=headers)
 
     def drop_table(self, bucket, schema, name, txid=0, client_tags=[], expected_retvals=[], remove_imports_table=False):
         """
         DELETE /mybucket/schema_path/mytable?table HTTP/1.1
         tabular-txid: TransactionId
         tabular-client-tag: ClientTag
 
         To remove the internal vastdb-imported-objects table just set remove_imports_table=True
         """
         headers = self._fill_common_headers(txid=txid, client_tags=client_tags)
         url_params = {'sub-table': IMPORTED_OBJECTS_TABLE_NAME} if remove_imports_table else {}
 
-        res = self.session.delete(self._api_prefix(bucket=bucket, schema=schema, table=name, command="table", url_params=url_params),
-                                  headers=headers)
-        return self._check_res(res, "drop_table", expected_retvals)
+        self._request(
+            method="DELETE",
+            url=self._url(bucket=bucket, schema=schema, table=name, command="table", url_params=url_params),
+            headers=headers)
 
     def list_tables(self, bucket, schema, txid=0, client_tags=[], max_keys=1000, next_key=0, name_prefix="",
                     exact_match=False, expected_retvals=[], include_list_stats=False, count_only=False):
         """
         GET /mybucket/schema_path?table HTTP/1.1
         tabular-txid: TransactionId
         tabular-client-tag: ClientTag
@@ -1097,31 +1114,33 @@
         else:
             headers['tabular-name-prefix'] = name_prefix
 
         headers['tabular-list-count-only'] = str(count_only)
         headers['tabular-include-list-stats'] = str(include_list_stats)
 
         tables = []
-        res = self.session.get(self._api_prefix(bucket=bucket, schema=schema, command="table"), headers=headers)
-        self._check_res(res, "list_table", expected_retvals)
-        if res.status_code == 200:
-            res_headers = res.headers
-            next_key = int(res_headers['tabular-next-key'])
-            is_truncated = res_headers['tabular-is-truncated'] == 'true'
-            lists = list_tables.GetRootAs(res.content)
-            bucket_name = lists.BucketName().decode()
-            schema_name = lists.SchemaName().decode()
-            if not bucket.startswith(bucket_name):  # ignore snapshot name
-                raise ValueError(f'bucket: {bucket} did not start from {bucket_name}')
-            tables_length = lists.TablesLength()
-            count = int(res_headers['tabular-list-count']) if 'tabular-list-count' in res_headers else tables_length
-            for i in range(tables_length):
-                tables.append(_parse_table_info(lists.Tables(i)))
+        res = self._request(
+            method="GET",
+            url=self._url(bucket=bucket, schema=schema, command="table"),
+            headers=headers)
+
+        res_headers = res.headers
+        next_key = int(res_headers['tabular-next-key'])
+        is_truncated = res_headers['tabular-is-truncated'] == 'true'
+        lists = list_tables.GetRootAs(res.content)
+        bucket_name = lists.BucketName().decode()
+        schema_name = lists.SchemaName().decode()
+        if not bucket.startswith(bucket_name):  # ignore snapshot name
+            raise ValueError(f'bucket: {bucket} did not start from {bucket_name}')
+        tables_length = lists.TablesLength()
+        count = int(res_headers['tabular-list-count']) if 'tabular-list-count' in res_headers else tables_length
+        for i in range(tables_length):
+            tables.append(_parse_table_info(lists.Tables(i)))
 
-            return bucket_name, schema_name, tables, next_key, is_truncated, count
+        return bucket_name, schema_name, tables, next_key, is_truncated, count
 
     def add_columns(self, bucket, schema, name, arrow_schema, txid=0, client_tags=[], expected_retvals=[]):
         """
         Add a column to table, use the following request
         POST /bucket/schema/table?column HTTP/1.1
 
         Request Headers
@@ -1135,17 +1154,18 @@
             "table_properties": {"key1":"val1", "key2":"val2", ...}
         }
         """
         headers = self._fill_common_headers(txid=txid, client_tags=client_tags)
         serialized_schema = arrow_schema.serialize()
         headers['Content-Length'] = str(len(serialized_schema))
 
-        res = self.session.post(self._api_prefix(bucket=bucket, schema=schema, table=name, command="column"),
-                                data=serialized_schema, headers=headers)
-        return self._check_res(res, "add_columns", expected_retvals)
+        self._request(
+            method="POST",
+            url=self._url(bucket=bucket, schema=schema, table=name, command="column"),
+            data=serialized_schema, headers=headers)
 
     def alter_column(self, bucket, schema, table, name, txid=0, client_tags=[], column_properties="",
                      new_name="", column_sep=".", column_stats="", expected_retvals=[]):
         """
         PUT /bucket/schema/table?column&tabular-column-name=ColumnName&tabular-new-column-name=NewColumnName HTTP/1.1
         Content-Length: ContentLength
         tabular-txid: TransactionId
@@ -1173,32 +1193,34 @@
         headers['tabular-column-sep'] = column_sep
         headers['Content-Length'] = str(len(alter_column_req))
 
         url_params = {'tabular-column-name': name}
         if len(new_name):
             url_params['tabular-new-column-name'] = new_name
 
-        res = self.session.put(self._api_prefix(bucket=bucket, schema=schema, table=table, command="column", url_params=url_params),
-                               data=alter_column_req, headers=headers)
-        return self._check_res(res, "alter_column", expected_retvals)
+        self._request(
+            method="PUT",
+            url=self._url(bucket=bucket, schema=schema, table=table, command="column", url_params=url_params),
+            data=alter_column_req, headers=headers)
 
     def drop_columns(self, bucket, schema, table, arrow_schema, txid=0, client_tags=[], expected_retvals=[]):
         """
         DELETE /mybucket/myschema/mytable?column HTTP/1.1
         tabular-txid: TransactionId
         tabular-client-tag: ClientTag
         tabular-column-name: OldColumnName
         """
         headers = self._fill_common_headers(txid=txid, client_tags=client_tags)
         serialized_schema = arrow_schema.serialize()
         headers['Content-Length'] = str(len(serialized_schema))
 
-        res = self.session.delete(self._api_prefix(bucket=bucket, schema=schema, table=table, command="column"),
-                                data=serialized_schema, headers=headers)
-        return self._check_res(res, "drop_columns", expected_retvals)
+        self._request(
+            method="DELETE",
+            url=self._url(bucket=bucket, schema=schema, table=table, command="column"),
+            data=serialized_schema, headers=headers)
 
     def list_columns(self, bucket, schema, table, *, txid=0, client_tags=None, max_keys=None, next_key=0,
                      count_only=False, name_prefix="", exact_match=False,
                      expected_retvals=None, bc_list_internals=False, list_imports_table=False):
         """
         GET /mybucket/myschema/mytable?columns HTTP/1.1
         tabular-txid: TransactionId
@@ -1222,116 +1244,76 @@
 
         if exact_match:
             headers['tabular-name-exact-match'] = name_prefix
         else:
             headers['tabular-name-prefix'] = name_prefix
 
         url_params = {'sub-table': IMPORTED_OBJECTS_TABLE_NAME} if list_imports_table else {}
-        res = self.session.get(self._api_prefix(bucket=bucket, schema=schema, table=table, command="column",
-                                                url_params=url_params),
-                               headers=headers, stream=True)
-        self._check_res(res, "list_columns", expected_retvals)
-        if res.status_code == 200:
-            res_headers = res.headers
-            next_key = int(res_headers['tabular-next-key'])
-            is_truncated = res_headers['tabular-is-truncated'] == 'true'
-            count = int(res_headers['tabular-list-count'])
-            columns = [] if count_only else pa.ipc.open_stream(res.content).schema
+        res = self._request(
+            method="GET",
+            url=self._url(bucket=bucket, schema=schema, table=table, command="column", url_params=url_params),
+            headers=headers)
+
+        res_headers = res.headers
+        next_key = int(res_headers['tabular-next-key'])
+        is_truncated = res_headers['tabular-is-truncated'] == 'true'
+        count = int(res_headers['tabular-list-count'])
+        columns = [] if count_only else pa.ipc.open_stream(res.content).schema
 
-            return columns, next_key, is_truncated, count
+        return columns, next_key, is_truncated, count
 
     def begin_transaction(self, client_tags=[], expected_retvals=[]):
         """
         POST /?transaction HTTP/1.1
         tabular-client-tag: ClientTag
 
         Response
         tabular-txid: TransactionId
         """
         headers = self._fill_common_headers(client_tags=client_tags)
-        res = self.session.post(self._api_prefix(command="transaction"), headers=headers)
-        return self._check_res(res, "begin_transaction", expected_retvals)
+        return self._request(
+            method="POST",
+            url=self._url(command="transaction"),
+            headers=headers)
 
     def commit_transaction(self, txid, client_tags=[], expected_retvals=[]):
         """
         PUT /?transaction HTTP/1.1
         tabular-txid: TransactionId
         tabular-client-tag: ClientTag
         """
         headers = self._fill_common_headers(txid=txid, client_tags=client_tags)
-        res = self.session.put(self._api_prefix(command="transaction"), headers=headers)
-        return self._check_res(res, "commit_transaction", expected_retvals)
+        self._request(
+            method="PUT",
+            url=self._url(command="transaction"),
+            headers=headers)
 
     def rollback_transaction(self, txid, client_tags=[], expected_retvals=[]):
         """
         DELETE /?transaction HTTP/1.1
         tabular-txid: TransactionId
         tabular-client-tag: ClientTag
         """
         headers = self._fill_common_headers(txid=txid, client_tags=client_tags)
-        res = self.session.delete(self._api_prefix(command="transaction"), headers=headers)
-        return self._check_res(res, "rollback_transaction", expected_retvals)
+        self._request(
+            method="DELETE",
+            url=self._url(command="transaction"),
+            headers=headers)
 
     def get_transaction(self, txid, client_tags=[], expected_retvals=[]):
         """
         GET /?transaction HTTP/1.1
         tabular-txid: TransactionId
         tabular-client-tag: ClientTag
         """
         headers = self._fill_common_headers(txid=txid, client_tags=client_tags)
-        res = self.session.get(self._api_prefix(command="transaction"), headers=headers)
-        return self._check_res(res, "get_transaction", expected_retvals)
-
-    def select_row_ids(self, bucket, schema, table, params, txid=0, client_tags=[], expected_retvals=[],
-                       retry_count=0, enable_sorted_projections=True):
-        """
-        POST /mybucket/myschema/mytable?query-data=SelectRowIds HTTP/1.1
-        """
-
-        # add query option select-only and read-only
-        headers = self._fill_common_headers(txid=txid, client_tags=client_tags)
-        headers['Content-Length'] = str(len(params))
-        headers['tabular-enable-sorted-projections'] = str(enable_sorted_projections)
-        if retry_count > 0:
-            headers['tabular-retry-count'] = str(retry_count)
-
-        res = self.session.post(self._api_prefix(bucket=bucket, schema=schema, table=table, command="query-data=SelectRowIds",),
-                                data=params, headers=headers, stream=True)
-        return self._check_res(res, "query_data", expected_retvals)
-
-    def read_columns_data(self, bucket, schema, table, params, txid=0, client_tags=[], expected_retvals=[], tenant_guid=None,
-                          retry_count=0, enable_sorted_projections=True):
-        """
-        POST /mybucket/myschema/mytable?query-data=ReadColumns HTTP/1.1
-        """
-
-        headers = self._fill_common_headers(txid=txid, client_tags=client_tags)
-        headers['Content-Length'] = str(len(params))
-        headers['tabular-enable-sorted-projections'] = str(enable_sorted_projections)
-        if retry_count > 0:
-            headers['tabular-retry-count'] = str(retry_count)
-
-        res = self.session.post(self._api_prefix(bucket=bucket, schema=schema, table=table, command="query-data=ReadColumns",),
-                               data=params, headers=headers, stream=True)
-        return self._check_res(res, "query_data", expected_retvals)
-
-    def count_rows(self, bucket, schema, table, params, txid=0, client_tags=[], expected_retvals=[], tenant_guid=None,
-                   retry_count=0, enable_sorted_projections=True):
-        """
-        POST /mybucket/myschema/mytable?query-data=CountRows HTTP/1.1
-        """
-        headers = self._fill_common_headers(txid=txid, client_tags=client_tags)
-        headers['Content-Length'] = str(len(params))
-        headers['tabular-enable-sorted-projections'] = str(enable_sorted_projections)
-        if retry_count > 0:
-            headers['tabular-retry-count'] = str(retry_count)
-
-        res = self.session.post(self._api_prefix(bucket=bucket, schema=schema, table=table, command="query-data=CountRows",),
-                               data=params, headers=headers, stream=True)
-        return self._check_res(res, "query_data", expected_retvals)
+        self._request(
+            method="GET",
+            url=self._url(command="transaction"),
+            headers=headers)
 
     def _build_query_data_headers(self, txid, client_tags, params, split, num_sub_splits, request_format, response_format,
                                   enable_sorted_projections, limit_rows, schedule_id, retry_count, search_path, tenant_guid,
                                   sub_split_start_row_ids):
         headers = self._fill_common_headers(txid=txid, client_tags=client_tags)
         headers['Content-Length'] = str(len(params))
         headers['tabular-split'] = ','.join(map(str, split))
@@ -1365,43 +1347,14 @@
         url_params = {}
         if query_imports_table:
             url_params['sub-table'] = IMPORTED_OBJECTS_TABLE_NAME
         elif projection:
             url_params['name'] = projection
         return url_params
 
-    def legacy_query_data(self, bucket, schema, table, params, split=(0, 1, 8), num_sub_splits=1, response_row_id=False,
-                      txid=0, client_tags=[], expected_retvals=[], limit_rows=0, schedule_id=None, retry_count=0,
-                      search_path=None, sub_split_start_row_ids=[], tenant_guid=None, projection='', enable_sorted_projections=True,
-                      request_format='string', response_format='string', query_imports_table=False):
-        """
-        POST /mybucket/myschema/mytable?query-data=LegacyQueryData HTTP/1.1
-        Content-Length: ContentLength
-        tabular-txid: TransactionId
-        tabular-client-tag: ClientTag
-        tabular-split: "split_id,total_splits,num_row_groups_per_split"
-        tabular-num-of-subsplits: "total"
-        tabular-request-format: "string"
-        tabular-response-format: "string" #arrow/trino
-        tabular-schedule-id: "schedule-id"
-
-        Request Body (flatbuf)
-        projections_chunk [expressions]
-        predicate_chunk "formatted_data", (required)
-
-        """
-        headers = self._build_query_data_headers(txid, client_tags, params, split, num_sub_splits, request_format, response_format,
-                                                  enable_sorted_projections, limit_rows, schedule_id, retry_count, search_path, tenant_guid,
-                                                  sub_split_start_row_ids)
-        url_params = self._build_query_data_url_params(projection, query_imports_table)
-
-        res = self.session.post(self._api_prefix(bucket=bucket, schema=schema, table=table, command="query-data=LegacyQueryData",
-                                                  url_params=url_params), data=params, headers=headers, stream=True)
-        return self._check_res(res, "legacy_query_data", expected_retvals)
-
     def query_data(self, bucket, schema, table, params, split=(0, 1, 8), num_sub_splits=1, response_row_id=False,
                    txid=0, client_tags=[], expected_retvals=[], limit_rows=0, schedule_id=None, retry_count=0,
                    search_path=None, sub_split_start_row_ids=[], tenant_guid=None, projection='', enable_sorted_projections=True,
                    request_format='string', response_format='string', query_imports_table=False):
         """
         GET /mybucket/myschema/mytable?data HTTP/1.1
         Content-Length: ContentLength
@@ -1423,17 +1376,18 @@
 
         headers = self._build_query_data_headers(txid, client_tags, params, split, num_sub_splits, request_format, response_format,
                                                  enable_sorted_projections, limit_rows, schedule_id, retry_count, search_path, tenant_guid,
                                                  sub_split_start_row_ids)
 
         url_params = self._build_query_data_url_params(projection, query_imports_table)
 
-        res = self.session.get(self._api_prefix(bucket=bucket, schema=schema, table=table, command="data", url_params=url_params),
-                               data=params, headers=headers, stream=True)
-        return self._check_res(res, "query_data", expected_retvals)
+        return self._request(
+            method="GET",
+            url=self._url(bucket=bucket, schema=schema, table=table, command="data", url_params=url_params),
+            data=params, headers=headers, stream=True)
 
     """
     source_files: list of (bucket_name, file_name)
     """
     def import_data(self, bucket, schema, table, source_files, txid=0, client_tags=[], expected_retvals=[], case_sensitive=True,
                     schedule_id=None, retry_count=0, blocking=True):
         """
@@ -1511,52 +1465,56 @@
         headers = self._fill_common_headers(txid=txid, client_tags=client_tags)
         headers['Content-Length'] = str(len(import_req))
         headers['tabular-case-sensitive'] = str(case_sensitive)
         if schedule_id is not None:
             headers['tabular-schedule-id'] = str(schedule_id)
         if retry_count > 0:
             headers['tabular-retry-count'] = str(retry_count)
-        res = self.session.post(self._api_prefix(bucket=bucket, schema=schema, table=table, command="data"),
-                                data=import_req, headers=headers, stream=True)
+        res = self._request(
+            method="POST",
+            url=self._url(bucket=bucket, schema=schema, table=table, command="data"),
+            data=import_req, headers=headers, stream=True)
         if blocking:
             res = iterate_over_import_data_response(res)
 
-        return self._check_res(res, "import_data", expected_retvals)
+        return res
 
     def insert_rows(self, bucket, schema, table, record_batch, txid=0, client_tags=[], expected_retvals=[]):
         """
         POST /mybucket/myschema/mytable?rows HTTP/1.1
         Content-Length: ContentLength
         tabular-txid: TransactionId
         tabular-client-tag: ClientTag
 
         Request Body
             RecordBatch
         """
         headers = self._fill_common_headers(txid=txid, client_tags=client_tags)
         headers['Content-Length'] = str(len(record_batch))
-        res = self.session.post(self._api_prefix(bucket=bucket, schema=schema, table=table, command="rows"),
-                                data=record_batch, headers=headers, stream=True)
-        return self._check_res(res, "insert_rows", expected_retvals)
+        return self._request(
+            method="POST",
+            url=self._url(bucket=bucket, schema=schema, table=table, command="rows"),
+            data=record_batch, headers=headers)
 
     def update_rows(self, bucket, schema, table, record_batch, txid=0, client_tags=[], expected_retvals=[]):
         """
         PUT /mybucket/myschema/mytable?rows HTTP/1.1
         Content-Length: ContentLength
         tabular-txid: TransactionId
         tabular-client-tag: ClientTag
 
         Request Body
             RecordBatch where first column must be row_id
         """
         headers = self._fill_common_headers(txid=txid, client_tags=client_tags)
         headers['Content-Length'] = str(len(record_batch))
-        res = self.session.put(self._api_prefix(bucket=bucket, schema=schema, table=table, command="rows"),
-                                data=record_batch, headers=headers)
-        self._check_res(res, "update_rows", expected_retvals)
+        self._request(
+            method="PUT",
+            url=self._url(bucket=bucket, schema=schema, table=table, command="rows"),
+            data=record_batch, headers=headers)
 
     def delete_rows(self, bucket, schema, table, record_batch, txid=0, client_tags=[], expected_retvals=[],
                     delete_from_imports_table=False):
         """
         DELETE /mybucket/myschema/mytable?rows HTTP/1.1
         Content-Length: ContentLength
         tabular-txid: TransactionId
@@ -1565,17 +1523,18 @@
         Request Body
             RecordBatch with single column '$row_id'
         """
         headers = self._fill_common_headers(txid=txid, client_tags=client_tags)
         headers['Content-Length'] = str(len(record_batch))
         url_params = {'sub-table': IMPORTED_OBJECTS_TABLE_NAME} if delete_from_imports_table else {}
 
-        res = self.session.delete(self._api_prefix(bucket=bucket, schema=schema, table=table, command="rows", url_params=url_params),
-                                  data=record_batch, headers=headers)
-        self._check_res(res, "delete_rows", expected_retvals)
+        self._request(
+            method="DELETE",
+            url=self._url(bucket=bucket, schema=schema, table=table, command="rows", url_params=url_params),
+            data=record_batch, headers=headers)
 
     def create_projection(self, bucket, schema, table, name, columns, txid=0, client_tags=[], expected_retvals=[]):
         """
         Create a table, use the following request
         POST /bucket/schema/table?projection&name=my_projection HTTP/1.1
 
         The user may define several Sorted and/Or Unsorted columns from the original table
@@ -1614,39 +1573,40 @@
         create_projection_req = builder.Output()
 
         headers = self._fill_common_headers(txid=txid, client_tags=client_tags)
 
         headers['Content-Length'] = str(len(create_projection_req))
         url_params = {'name': name}
 
-        res = self.session.post(self._api_prefix(bucket=bucket, schema=schema, table=table, command="projection", url_params=url_params),
-                                data=create_projection_req, headers=headers)
-        return self._check_res(res, "create_projection", expected_retvals)
+        self._request(
+            method="POST",
+            url=self._url(bucket=bucket, schema=schema, table=table, command="projection", url_params=url_params),
+            data=create_projection_req, headers=headers)
 
     def get_projection_stats(self, bucket, schema, table, name, txid=0, client_tags=[], expected_retvals=[]):
         """
         GET /mybucket/myschema/mytable?projection-stats&name=my_projection HTTP/1.1
         tabular-txid: TransactionId
         tabular-client-tag: ClientTag
 
         The Command will return the statistics in flatbuf format
         """
         headers = self._fill_common_headers(txid=txid, client_tags=client_tags)
         url_params = {'name': name}
-        res = self.session.get(self._api_prefix(bucket=bucket, schema=schema, table=table, command="projection-stats", url_params=url_params),
-                               headers=headers)
-        if res.status_code == 200:
-            stats = get_projection_table_stats.GetRootAs(res.content)
-            num_rows = stats.NumRows()
-            size_in_bytes = stats.SizeInBytes()
-            dirty_blocks_percentage = stats.DirtyBlocksPercentage()
-            initial_sync_progress = stats.InitialSyncProgress()
-            return num_rows, size_in_bytes, dirty_blocks_percentage, initial_sync_progress
+        res = self._request(
+            method="GET",
+            url=self._url(bucket=bucket, schema=schema, table=table, command="projection-stats", url_params=url_params),
+            headers=headers)
 
-        return self._check_res(res, "get_projection_stats", expected_retvals)
+        stats = get_projection_table_stats.GetRootAs(res.content)
+        num_rows = stats.NumRows()
+        size_in_bytes = stats.SizeInBytes()
+        dirty_blocks_percentage = stats.DirtyBlocksPercentage()
+        initial_sync_progress = stats.InitialSyncProgress()
+        return num_rows, size_in_bytes, dirty_blocks_percentage, initial_sync_progress
 
     def alter_projection(self, bucket, schema, table, name, txid=0, client_tags=[], table_properties="",
                          new_name="", expected_retvals=[]):
         """
         PUT /mybucket/myschema/mytable?projection&name=my_projection HTTP/1.1
         Content-Length: ContentLength
         tabular-txid: TransactionId
@@ -1670,31 +1630,32 @@
         builder.Finish(params)
         alter_projection_req = builder.Output()
 
         headers = self._fill_common_headers(txid=txid, client_tags=client_tags)
         headers['Content-Length'] = str(len(alter_projection_req))
         url_params = {'name': name}
 
-        res = self.session.put(self._api_prefix(bucket=bucket, schema=schema, table=table, command="projection", url_params=url_params),
-                               data=alter_projection_req, headers=headers)
-
-        return self._check_res(res, "alter_projection", expected_retvals)
+        self._request(
+            method="PUT",
+            url=self._url(bucket=bucket, schema=schema, table=table, command="projection", url_params=url_params),
+            data=alter_projection_req, headers=headers)
 
     def drop_projection(self, bucket, schema, table, name, txid=0, client_tags=[], expected_retvals=[]):
         """
         DELETE /mybucket/schema_path/mytable?projection&name=my_projection HTTP/1.1
         tabular-txid: TransactionId
         tabular-client-tag: ClientTag
         """
         headers = self._fill_common_headers(txid=txid, client_tags=client_tags)
         url_params = {'name': name}
 
-        res = self.session.delete(self._api_prefix(bucket=bucket, schema=schema, table=table, command="projection", url_params=url_params),
-                                  headers=headers)
-        return self._check_res(res, "drop_projection", expected_retvals)
+        self._request(
+            method="DELETE",
+            url=self._url(bucket=bucket, schema=schema, table=table, command="projection", url_params=url_params),
+            headers=headers)
 
     def list_projections(self, bucket, schema, table, txid=0, client_tags=[], max_keys=1000, next_key=0, name_prefix="",
                          exact_match=False, expected_retvals=[], include_list_stats=False, count_only=False):
         """
         GET /mybucket/schema_path/my_table?projection HTTP/1.1
         tabular-txid: TransactionId
         tabular-client-tag: ClientTag
@@ -1710,32 +1671,34 @@
         else:
             headers['tabular-name-prefix'] = name_prefix
 
         headers['tabular-list-count-only'] = str(count_only)
         headers['tabular-include-list-stats'] = str(include_list_stats)
 
         projections = []
-        res = self.session.get(self._api_prefix(bucket=bucket, schema=schema, table=table, command="projection"), headers=headers)
-        self._check_res(res, "list_projections", expected_retvals)
-        if res.status_code == 200:
-            res_headers = res.headers
-            next_key = int(res_headers['tabular-next-key'])
-            is_truncated = res_headers['tabular-is-truncated'] == 'true'
-            count = int(res_headers['tabular-list-count'])
-            lists = list_projections.GetRootAs(res.content)
-            bucket_name = lists.BucketName().decode()
-            schema_name = lists.SchemaName().decode()
-            table_name = lists.TableName().decode()
-            if not bucket.startswith(bucket_name):  # ignore snapshot name
-                raise ValueError(f'bucket: {bucket} did not start from {bucket_name}')
-            projections_length = lists.ProjectionsLength()
-            for i in range(projections_length):
-                projections.append(_parse_table_info(lists.Projections(i)))
+        res = self._request(
+            method="GET",
+            url=self._url(bucket=bucket, schema=schema, table=table, command="projection"),
+            headers=headers)
+
+        res_headers = res.headers
+        next_key = int(res_headers['tabular-next-key'])
+        is_truncated = res_headers['tabular-is-truncated'] == 'true'
+        count = int(res_headers['tabular-list-count'])
+        lists = list_projections.GetRootAs(res.content)
+        bucket_name = lists.BucketName().decode()
+        schema_name = lists.SchemaName().decode()
+        table_name = lists.TableName().decode()
+        if not bucket.startswith(bucket_name):  # ignore snapshot name
+            raise ValueError(f'bucket: {bucket} did not start from {bucket_name}')
+        projections_length = lists.ProjectionsLength()
+        for i in range(projections_length):
+            projections.append(_parse_table_info(lists.Projections(i)))
 
-            return bucket_name, schema_name, table_name, projections, next_key, is_truncated, count
+        return bucket_name, schema_name, table_name, projections, next_key, is_truncated, count
 
     def list_projection_columns(self, bucket, schema, table, projection, txid=0, client_tags=[], max_keys=1000,
                                 next_key=0, count_only=False, name_prefix="", exact_match=False,
                                 expected_retvals=None):
         """
         GET /mybucket/myschema/mytable?projection-columns HTTP/1.1
         tabular-txid: TransactionId
@@ -1755,27 +1718,28 @@
         if exact_match:
             headers['tabular-name-exact-match'] = name_prefix
         else:
             headers['tabular-name-prefix'] = name_prefix
 
         url_params = {'name': projection}
 
-        res = self.session.get(self._api_prefix(bucket=bucket, schema=schema, table=table, command="projection-columns", url_params=url_params),
-                               headers=headers, stream=True)
-        self._check_res(res, "list_projection_columns", expected_retvals)
+        res = self._request(
+            method="GET",
+            url=self._url(bucket=bucket, schema=schema, table=table, command="projection-columns", url_params=url_params),
+            headers=headers)
+
         # list projection columns response will also show column type Sorted/UnSorted
-        if res.status_code == 200:
-            res_headers = res.headers
-            next_key = int(res_headers['tabular-next-key'])
-            is_truncated = res_headers['tabular-is-truncated'] == 'true'
-            count = int(res_headers['tabular-list-count'])
-            columns = [] if count_only else [[f.name, f.type, f.metadata] for f in
-                                             pa.ipc.open_stream(res.content).schema]
+        res_headers = res.headers
+        next_key = int(res_headers['tabular-next-key'])
+        is_truncated = res_headers['tabular-is-truncated'] == 'true'
+        count = int(res_headers['tabular-list-count'])
+        columns = [] if count_only else [[f.name, f.type, f.metadata] for f in
+                                         pa.ipc.open_stream(res.content).schema]
 
-            return columns, next_key, is_truncated, count
+        return columns, next_key, is_truncated, count
 
 
 class QueryDataInternalError(Exception):
     pass
 
 
 def _iter_query_data_response_columns(fileobj, stream_ids=None):
@@ -2114,44 +2078,7 @@
     fb_relation.AddImplType(builder, rel_impl.RelationImpl.Source)
     fb_relation.AddImpl(builder, source)
     relation = fb_relation.End(builder)
 
     builder.Finish(relation)
 
     return QueryDataRequest(serialized=builder.Output(), response_schema=response_schema, response_parser=QueryDataParser(response_schema))
-
-
-def convert_column_types(table: 'pa.Table') -> 'pa.Table':
-    """
-    Adjusting table values
-
-    1. Because the timestamp resolution is too high it is necessary to trim it. ORION-96961
-    2. Since the values of nfs_mode_bits are returned in decimal, need to convert them to octal,
-    as in all representations, so that the mode of 448 turn into 700
-    3. for owner_name and group_owner_name 0 -> root, and 65534 -> nobody
-    """
-    ts_indexes = []
-    indexes_of_fields_to_change = {}
-    sid_to_name = {
-        '0': 'root',
-        '65534': 'nobody'  # NFSNOBODY_UID_16_BIT
-    }
-    column_matcher = {  # column_name: custom converting rule
-        'nfs_mode_bits': lambda val: int(oct(val).replace('0o', '')) if val is not None else val,
-        'owner_name': lambda val: sid_to_name.get(val, val),
-        'group_owner_name': lambda val: sid_to_name.get(val, val),
-    }
-    for index, field in enumerate(table.schema):
-        if isinstance(field.type, pa.TimestampType) and field.type.unit == 'ns':
-            ts_indexes.append(index)
-        if field.name in column_matcher:
-            indexes_of_fields_to_change[field.name] = index
-    for changing_index in ts_indexes:
-        field_name = table.schema[changing_index].name
-        new_column = table[field_name].cast(pa.timestamp('us'), safe=False)
-        table = table.set_column(changing_index, field_name, new_column)
-    for field_name, changing_index in indexes_of_fields_to_change.items():
-        new_column = table[field_name].to_pylist()
-        new_column = list(map(column_matcher[field_name], new_column))
-        new_column = pa.array(new_column, table[field_name].type)
-        table = table.set_column(changing_index, field_name, new_column)
-    return table
```

### Comparing `vastdb-0.1.6/vastdb/schema.py` & `vastdb-0.1.7/vastdb/schema.py`

 * *Files 7% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 VAST S3 buckets can be used to create Database schemas and tables.
 It is possible to list and access VAST snapshots generated over a bucket.
 """
 
 import logging
 from dataclasses import dataclass
-from typing import TYPE_CHECKING, List, Optional
+from typing import TYPE_CHECKING, Iterable, List, Optional
 
 import pyarrow as pa
 
 from . import bucket, errors, schema, table
 
 if TYPE_CHECKING:
     from .table import Table
@@ -58,36 +58,40 @@
                 raise errors.MissingSchema(self.bucket.name, self._subschema_full_name(name))
             else:
                 return None
 
         assert len(names) == 1, f"Expected to receive only a single schema, but got {len(schemas)}: ({schemas})"
         return schema.Schema(name=self._subschema_full_name(names[0]), bucket=self.bucket)
 
-    def schemas(self, batch_size=None) -> List["Schema"]:
+    def schemas(self, batch_size=None) -> Iterable["Schema"]:
         """List child schemas."""
         next_key = 0
         if not batch_size:
             batch_size = 1000
         result: List["Schema"] = []
         while True:
             _bucket_name, curr_schemas, next_key, is_truncated, _ = \
                 self.tx._rpc.api.list_schemas(bucket=self.bucket.name, schema=self.name, next_key=next_key, max_keys=batch_size, txid=self.tx.txid)
             result.extend(schema.Schema(name=self._subschema_full_name(name), bucket=self.bucket) for name, *_ in curr_schemas)
             if not is_truncated:
                 break
         return result
 
-    def create_table(self, table_name: str, columns: pa.Schema, fail_if_exists=True) -> "Table":
+    def create_table(self, table_name: str, columns: pa.Schema, fail_if_exists=True, use_external_row_ids_allocation=False) -> "Table":
         """Create a new table under this schema."""
         if current := self.table(table_name, fail_if_missing=False):
             if fail_if_exists:
                 raise errors.TableExists(self.bucket.name, self.name, table_name)
             else:
                 return current
-        self.tx._rpc.api.create_table(self.bucket.name, self.name, table_name, columns, txid=self.tx.txid)
+        if use_external_row_ids_allocation:
+            self.tx._rpc.features.check_external_row_ids_allocation()
+
+        self.tx._rpc.api.create_table(self.bucket.name, self.name, table_name, columns, txid=self.tx.txid,
+                                      use_external_row_ids_allocation=use_external_row_ids_allocation)
         log.info("Created table: %s", table_name)
         return self.table(table_name)  # type: ignore[return-value]
 
     def table(self, name: str, fail_if_missing=True) -> Optional["table.Table"]:
         """Get a specific table under this schema."""
         t = self.tables(table_name=name)
         if not t:
```

### Comparing `vastdb-0.1.6/vastdb/session.py` & `vastdb-0.1.7/vastdb/session.py`

 * *Files 9% similar despite different names*

```diff
@@ -5,18 +5,20 @@
 - [Virtual IP pool configured with DNS service](https://support.vastdata.com/s/topic/0TOV40000000FThOAM/configuring-network-access-v50)
 - [S3 access & secret keys on VAST cluster](https://support.vastdata.com/s/article/UUID-4d2e7e23-b2fb-7900-d98f-96c31a499626)
 - [Tabular identity policy with the proper permissions](https://support.vastdata.com/s/article/UUID-14322b60-d6a2-89ac-3df0-3dfbb6974182)
 """
 
 import logging
 import os
+from typing import Optional
 
 import boto3
 
-from . import errors, internal_commands, transaction
+from . import _internal, errors, transaction
+from ._internal import BackoffConfig
 
 log = logging.getLogger()
 
 
 class Features:
     """VAST database features - check if server is already support a feature."""
 
@@ -32,14 +34,18 @@
             "Returning row IDs requires 5.1+ VAST release",
             vast_version >= (5, 1))
 
         self.check_enforce_semisorted_projection = self._check(
             "Semi-sorted projection enforcement requires 5.1+ VAST release",
             vast_version >= (5, 1))
 
+        self.check_external_row_ids_allocation = self._check(
+            "External row IDs allocation requires 5.1+ VAST release",
+            vast_version >= (5, 1))
+
     def _check(self, msg, supported):
         log.debug("%s (current version is %s): supported=%s", msg, self.vast_version, supported)
         if not supported:
             def fail():
                 raise errors.NotSupportedVersion(msg, self.vast_version)
             return fail
 
@@ -47,26 +53,33 @@
             pass
         return noop
 
 
 class Session:
     """VAST database session."""
 
-    def __init__(self, access=None, secret=None, endpoint=None, ssl_verify=True):
+    def __init__(self, access=None, secret=None, endpoint=None,
+                 *,
+                 ssl_verify=True,
+                 backoff_config: Optional[BackoffConfig] = None):
         """Connect to a VAST Database endpoint, using specified credentials."""
         if access is None:
             access = os.environ['AWS_ACCESS_KEY_ID']
         if secret is None:
             secret = os.environ['AWS_SECRET_ACCESS_KEY']
         if endpoint is None:
             endpoint = os.environ['AWS_S3_ENDPOINT_URL']
 
-        self.api = internal_commands.VastdbApi(endpoint, access, secret, ssl_verify=ssl_verify)
-        version_tuple = tuple(int(part) for part in self.api.vast_version.split('.'))
-        self.features = Features(version_tuple)
+        self.api = _internal.VastdbApi(
+            endpoint=endpoint,
+            access_key=access,
+            secret_key=secret,
+            ssl_verify=ssl_verify,
+            backoff_config=backoff_config)
+        self.features = Features(self.api.vast_version)
         self.s3 = boto3.client('s3',
             aws_access_key_id=access,
             aws_secret_access_key=secret,
             endpoint_url=endpoint)
 
     def __repr__(self):
         """Don't show the secret key."""
```

### Comparing `vastdb-0.1.6/vastdb/table.py` & `vastdb-0.1.7/vastdb/table.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,22 +3,22 @@
 import concurrent.futures
 import logging
 import os
 import queue
 from dataclasses import dataclass, field
 from math import ceil
 from threading import Event
-from typing import Any, Dict, List, Optional, Tuple, Union
+from typing import Any, Dict, Iterable, List, Optional, Tuple, Union
 
 import backoff
 import ibis
 import pyarrow as pa
 import requests
 
-from . import errors, internal_commands, schema, util
+from . import _internal, errors, schema, util
 
 log = logging.getLogger(__name__)
 
 
 INTERNAL_ROW_ID = "$row_id"
 INTERNAL_ROW_ID_FIELD = pa.field(INTERNAL_ROW_ID, pa.uint64())
 
@@ -76,15 +76,20 @@
 
     # used to estimate the number of splits, given the table rows' count
     rows_per_split: int = 4000000
 
     # used for worker threads' naming
     query_id: str = ""
 
-    # allows retrying QueryData when the server is overloaded
+    # non-negative integer, used for server-side prioritization of queued requests:
+    # - requests with lower values will be served before requests with higher values.
+    # - if unset, the request will be added to the queue's end.
+    queue_priority: Optional[int] = None
+
+    # DEPRECATED: will be removed in a future release
     backoff_func: Any = field(default=backoff.on_exception(backoff.expo, RETRIABLE_ERRORS, max_tries=10))
 
 
 @dataclass
 class ImportConfig:
     """Import execution configiration."""
 
@@ -98,50 +103,50 @@
         """Initialize query split state."""
         self.split_id = split_id
         self.subsplits_state = {i: 0 for i in range(config.num_sub_splits)}
         self.config = config
         self.query_data_request = query_data_request
         self.table = table
 
-    def batches(self, api: internal_commands.VastdbApi):
+    def batches(self, api: _internal.VastdbApi):
         """Execute QueryData request, and yield parsed RecordBatch objects.
 
         Can be called repeatedly, to allow pagination.
         """
         while not self.done:
-            query_with_backoff = self.config.backoff_func(api.query_data)
-            response = query_with_backoff(
+            response = api.query_data(
                             bucket=self.table.bucket.name,
                             schema=self.table.schema.name,
                             table=self.table.name,
                             params=self.query_data_request.serialized,
                             split=(self.split_id, self.config.num_splits, self.config.num_row_groups_per_sub_split),
                             num_sub_splits=self.config.num_sub_splits,
                             response_row_id=False,
                             txid=self.table.tx.txid,
                             limit_rows=self.config.limit_rows_per_sub_split,
                             sub_split_start_row_ids=self.subsplits_state.items(),
+                            schedule_id=self.config.queue_priority,
                             enable_sorted_projections=self.config.use_semi_sorted_projections,
                             query_imports_table=self.table._imports_table,
                             projection=self.config.semi_sorted_projection_name)
-            pages_iter = internal_commands.parse_query_data_response(
+            pages_iter = _internal.parse_query_data_response(
                 conn=response.raw,
                 schema=self.query_data_request.response_schema,
                 start_row_ids=self.subsplits_state,
                 parser=self.query_data_request.response_parser)
 
             for page in pages_iter:
                 for batch in page.to_batches():
                     if len(batch) > 0:
                         yield batch
 
     @property
     def done(self):
         """Returns true iff the pagination over."""
-        return all(row_id == internal_commands.TABULAR_INVALID_ROW_ID for row_id in self.subsplits_state.values())
+        return all(row_id == _internal.TABULAR_INVALID_ROW_ID for row_id in self.subsplits_state.values())
 
 
 @dataclass
 class Table:
     """VAST Table."""
 
     name: str
@@ -183,22 +188,22 @@
         self.arrow_schema = pa.schema(fields)
         return self.arrow_schema
 
     def projection(self, name: str) -> "Projection":
         """Get a specific semi-sorted projection of this table."""
         if self._imports_table:
             raise errors.NotSupportedCommand(self.bucket.name, self.schema.name, self.name)
-        projs = self.projections(projection_name=name)
+        projs = tuple(self.projections(projection_name=name))
         if not projs:
             raise errors.MissingProjection(self.bucket.name, self.schema.name, self.name, name)
         assert len(projs) == 1, f"Expected to receive only a single projection, but got: {len(projs)}. projections: {projs}"
         log.debug("Found projection: %s", projs[0])
         return projs[0]
 
-    def projections(self, projection_name=None) -> List["Projection"]:
+    def projections(self, projection_name=None) -> Iterable["Projection"]:
         """List all semi-sorted projections of this table."""
         if self._imports_table:
             raise errors.NotSupportedCommand(self.bucket.name, self.schema.name, self.name)
         projections = []
         next_key = 0
         name_prefix = projection_name if projection_name else ""
         exact_match = bool(projection_name)
@@ -210,15 +215,15 @@
             if not curr_projections:
                 break
             projections.extend(curr_projections)
             if not is_truncated:
                 break
         return [_parse_projection_info(projection, self) for projection in projections]
 
-    def import_files(self, files_to_import: List[str], config: Optional[ImportConfig] = None) -> None:
+    def import_files(self, files_to_import: Iterable[str], config: Optional[ImportConfig] = None) -> None:
         """Import a list of Parquet files into this table.
 
         The files must be on VAST S3 server and be accessible using current credentials.
         """
         if self._imports_table:
             raise errors.NotSupportedCommand(self.bucket.name, self.schema.name, self.name)
         source_files = {}
@@ -279,15 +284,15 @@
                 raise
 
         futures = []
         with concurrent.futures.ThreadPoolExecutor(
                 max_workers=config.import_concurrency, thread_name_prefix='import_thread') as pool:
             try:
                 for endpoint in endpoints:
-                    session = internal_commands.VastdbApi(endpoint, self.tx._rpc.api.access_key, self.tx._rpc.api.secret_key)
+                    session = _internal.VastdbApi(endpoint, self.tx._rpc.api.access_key, self.tx._rpc.api.secret_key)
                     futures.append(pool.submit(import_worker, files_queue, session))
 
                 log.debug("Waiting for import workers to finish")
                 for future in concurrent.futures.as_completed(futures):
                     future.result()
             finally:
                 stop_event.set()
@@ -338,21 +343,21 @@
             queried_fields.extend(column for column in self.arrow_schema)
             query_schema = pa.schema(queried_fields)
             columns.append(INTERNAL_ROW_ID)
 
         if predicate is True:
             predicate = None
         if predicate is False:
-            response_schema = internal_commands.get_response_schema(schema=query_schema, field_names=columns)
+            response_schema = _internal.get_response_schema(schema=query_schema, field_names=columns)
             return pa.RecordBatchReader.from_batches(response_schema, [])
 
         if isinstance(predicate, ibis.common.deferred.Deferred):
             predicate = predicate.resolve(self._ibis_table)  # may raise if the predicate is invalid (e.g. wrong types / missing column)
 
-        query_data_request = internal_commands.build_query_data_request(
+        query_data_request = _internal.build_query_data_request(
             schema=query_schema,
             predicate=predicate,
             field_names=columns)
         if len(query_data_request.serialized) > util.MAX_QUERY_DATA_REQUEST_SIZE:
             raise errors.TooLargeRequest(f"{len(query_data_request.serialized)} bytes")
 
         splits_queue: queue.Queue[int] = queue.Queue()
@@ -372,15 +377,15 @@
 
         def check_stop():
             if stop_event.is_set():
                 raise StoppedException
 
         def single_endpoint_worker(endpoint: str):
             try:
-                host_api = internal_commands.VastdbApi(endpoint=endpoint, access_key=self.tx._rpc.api.access_key, secret_key=self.tx._rpc.api.secret_key)
+                host_api = _internal.VastdbApi(endpoint=endpoint, access_key=self.tx._rpc.api.access_key, secret_key=self.tx._rpc.api.secret_key)
                 while True:
                     check_stop()
                     try:
                         split = splits_queue.get_nowait()
                     except queue.Empty:
                         log.debug("splits queue is empty")
                         break
@@ -469,15 +474,15 @@
             raise errors.NotSupportedCommand(self.bucket.name, self.schema.name, self.name)
         try:
             row_ids = []
             serialized_slices = util.iter_serialized_slices(rows, MAX_INSERT_ROWS_PER_PATCH)
             for slice in serialized_slices:
                 res = self.tx._rpc.api.insert_rows(self.bucket.name, self.schema.name, self.name, record_batch=slice,
                                                    txid=self.tx.txid)
-                (batch,) = pa.RecordBatchStreamReader(res.raw)
+                (batch,) = pa.RecordBatchStreamReader(res.content)
                 row_ids.append(batch[INTERNAL_ROW_ID])
             try:
                 self.tx._rpc.features.check_return_row_ids()
             except errors.NotSupportedVersion:
                 return  # type: ignore
             return pa.chunked_array(row_ids)
         except errors.TooWideRow:
@@ -505,14 +510,16 @@
                 update_fields.append(rows.field(col))
                 update_values.append(_combine_chunks(rows[col]))
 
             update_rows_rb = pa.record_batch(schema=pa.schema(update_fields), data=update_values)
         else:
             update_rows_rb = rows
 
+        update_rows_rb = util.sort_record_batch_if_needed(update_rows_rb, INTERNAL_ROW_ID)
+
         serialized_slices = util.iter_serialized_slices(update_rows_rb, MAX_ROWS_PER_BATCH)
         for slice in serialized_slices:
             self.tx._rpc.api.update_rows(self.bucket.name, self.schema.name, self.name, record_batch=slice,
                                          txid=self.tx.txid)
 
     def delete(self, rows: Union[pa.RecordBatch, pa.Table]) -> None:
         """Delete a subset of rows in this table.
@@ -524,14 +531,16 @@
         try:
             rows_chunk = rows[INTERNAL_ROW_ID]
         except KeyError:
             raise errors.MissingRowIdColumn
         delete_rows_rb = pa.record_batch(schema=pa.schema([(INTERNAL_ROW_ID, pa.uint64())]),
                                          data=[_combine_chunks(rows_chunk)])
 
+        delete_rows_rb = util.sort_record_batch_if_needed(delete_rows_rb, INTERNAL_ROW_ID)
+
         serialized_slices = util.iter_serialized_slices(delete_rows_rb, MAX_ROWS_PER_BATCH)
         for slice in serialized_slices:
             self.tx._rpc.api.delete_rows(self.bucket.name, self.schema.name, self.name, record_batch=slice,
                                          txid=self.tx.txid, delete_from_imports_table=self._imports_table)
 
     def drop(self) -> None:
         """Drop this table."""
@@ -589,15 +598,15 @@
         empty_schema = pa.schema([])
         self.tx._rpc.api.create_table(self.bucket.name, self.schema.name, self.name, empty_schema, txid=self.tx.txid,
                                         create_imports_table=True)
         log.info("Created imports table for table: %s", self.name)
         return self.imports_table()  # type: ignore[return-value]
 
     def imports_table(self) -> Optional["Table"]:
-        """Get the imports table under of this table."""
+        """Get the imports table of this table."""
         self.tx._rpc.features.check_imports_table()
         return Table(name=self.name, schema=self.schema, handle=int(self.handle), stats=self.stats, _imports_table=True)
 
     def __getitem__(self, col_name):
         """Allow constructing ibis-like column expressions from this table.
 
         It is useful for constructing expressions for predicate pushdown in `Table.select()` method.
```

### Comparing `vastdb-0.1.6/vastdb/tests/test_duckdb.py` & `vastdb-0.1.7/vastdb/tests/test_duckdb.py`

 * *Files 13% similar despite different names*

```diff
@@ -52,10 +52,10 @@
         first = next(batches)  # make sure that HTTP response processing has started
         assert first['a'].to_pylist() == list(range(100))
 
         conn = duckdb.connect()
         res = conn.execute('SELECT a FROM batches')
         log.debug("closing tx=%s after first batch=%s", t.tx, first)
 
-    # transaction is closed, collecting the result should fail
-    with pytest.raises(duckdb.InvalidInputException, match="Detail: Python exception: MissingTransaction"):
+    # transaction is closed, collecting the result should fail internally in DuckDB
+    with pytest.raises(duckdb.InvalidInputException):
         res.arrow()
```

### Comparing `vastdb-0.1.6/vastdb/tests/test_imports.py` & `vastdb-0.1.7/vastdb/tests/test_imports.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.6/vastdb/tests/test_nested.py` & `vastdb-0.1.7/vastdb/tests/test_nested.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.6/vastdb/tests/test_projections.py` & `vastdb-0.1.7/vastdb/tests/test_projections.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.6/vastdb/tests/test_sanity.py` & `vastdb-0.1.7/vastdb/tests/test_sanity.py`

 * *Files 9% similar despite different names*

```diff
@@ -21,26 +21,27 @@
     bad_session = vastdb.connect(access='BAD', secret='BAD', endpoint=session.api.url)
     with pytest.raises(vastdb.errors.Forbidden):
         with bad_session.transaction():
             pass
 
 
 def test_bad_endpoint(session):
+    backoff_config = vastdb.session.BackoffConfig(max_tries=3)
     with pytest.raises(requests.exceptions.ConnectionError):
-        vastdb.connect(access='BAD', secret='BAD', endpoint='http://invalid-host-name-for-tests:12345')
+        vastdb.connect(access='BAD', secret='BAD', endpoint='http://invalid-host-name-for-tests:12345', backoff_config=backoff_config)
 
 
 def test_version_extraction():
     # A list of version and expected version parsed by API
     TEST_CASES = [
             (None, None),                                   # vast server without version in header
             ("5", None),                                    # major
             ("5.2", None),                                  # major.minor
             ("5.2.0", None),                                # major.minor.patch
-            ("5.2.0.10", "5.2.0.10"),                       # major.minor.patch.protocol
+            ("5.2.0.10", (5, 2, 0, 10)),                    # major.minor.patch.protocol
             ("5.2.0.10 some other things", None),           # suffix
             ("5.2.0.10.20", None),                          # extra version
     ]
 
     # Mock OPTIONS handle that cycles through the test cases response
     class MockOptionsHandler(BaseHTTPRequestHandler):
         versions_iterator = cycle(TEST_CASES)
```

### Comparing `vastdb-0.1.6/vastdb/tests/test_schemas.py` & `vastdb-0.1.7/vastdb/tests/test_schemas.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.6/vastdb/tests/test_tables.py` & `vastdb-0.1.7/vastdb/tests/test_tables.py`

 * *Files 1% similar despite different names*

```diff
@@ -54,15 +54,15 @@
         log.debug("actual=%s", actual)
         assert actual.to_pydict() == {
             's': ['a', 'bb', 'ccc'],
             INTERNAL_ROW_ID: [0, 1, 2]
         }
 
         columns_to_delete = pa.schema([(INTERNAL_ROW_ID, pa.uint64())])
-        rb = pa.record_batch(schema=columns_to_delete, data=[[0]])  # delete rows 0,1
+        rb = pa.record_batch(schema=columns_to_delete, data=[[0]])  # delete row 0
         t.delete(rb)
 
         selected_rows = t.select(columns=['b'], predicate=(t['a'] == 222), internal_row_id=True).read_all()
         t.delete(selected_rows)
         actual = t.select(columns=['a', 'b', 's']).read_all()
         assert actual.to_pydict() == {
             'a': [333],
@@ -77,14 +77,27 @@
     expected = pa.table(schema=columns, data=data)
 
     with prepare_data(session, clean_bucket_name, 's', 't', expected) as t:
         actual = t.select().read_all()
         assert actual == expected
 
 
+def test_insert_empty(session, clean_bucket_name):
+    columns = pa.schema([('a', pa.int8()), ('b', pa.float32())])
+    data = [[None] * 5, [None] * 5]
+    all_nulls = pa.table(schema=columns, data=data)
+    no_columns = all_nulls.select([])
+
+    with session.transaction() as tx:
+        t = tx.bucket(clean_bucket_name).create_schema('s').create_table('t', columns)
+        t.insert(all_nulls)
+        with pytest.raises(errors.NotImplemented):
+            t.insert(no_columns)
+
+
 def test_exists(session, clean_bucket_name):
     with session.transaction() as tx:
         s = tx.bucket(clean_bucket_name).create_schema('s1')
         assert s.tables() == []
 
         t = s.create_table('t', pa.schema([('x', pa.int64())]))
 
@@ -152,14 +165,35 @@
         t.update(update_table.to_batches()[0], columns=['a'])
         actual = t.select(columns=['a', 'b']).read_all()
         assert actual.to_pydict() == {
             'a': [111, 2222, 333],
             'b': [0.5, 1.5, 2.5]
         }
 
+        # test update for not sorted rows:
+        rb = pa.record_batch(schema=columns_to_update, data=[
+            [2, 0],  # update rows 0,2
+            [231, 235]
+        ])
+        t.update(rb)
+        actual = t.select(columns=['a', 'b']).read_all()
+        assert actual.to_pydict() == {
+            'a': [235, 2222, 231],
+            'b': [0.5, 1.5, 2.5]
+        }
+
+        # test delete for not sorted rows:
+        rb = pa.record_batch(schema=pa.schema([(INTERNAL_ROW_ID, pa.uint64())]), data=[[2, 0]])
+        t.delete(rb)
+        actual = t.select(columns=['a', 'b']).read_all()
+        assert actual.to_pydict() == {
+            'a': [2222],
+            'b': [1.5]
+        }
+
 
 def test_select_with_multisplits(session, clean_bucket_name):
     columns = pa.schema([
         ('a', pa.int32())
     ])
 
     data = [1, 2, 3, 4, 5, 6, 7, 8, 9, 10]
@@ -170,14 +204,33 @@
     config.rows_per_split = 1000
 
     with prepare_data(session, clean_bucket_name, 's', 't', expected) as t:
         actual = t.select(columns=['a'], config=config).read_all()
         assert actual == expected
 
 
+def test_select_with_priority(session, clean_bucket_name):
+    columns = pa.schema([
+        ('a', pa.int32())
+    ])
+    expected = pa.table(schema=columns, data=[range(100)])
+    with prepare_data(session, clean_bucket_name, 's', 't', expected) as t:
+        config = QueryConfig()
+
+        config.queue_priority = 0
+        assert t.select(config=config).read_all() == expected
+
+        config.queue_priority = 12345
+        assert t.select(config=config).read_all() == expected
+
+        config.queue_priority = -1
+        with pytest.raises(errors.BadRequest):
+            t.select(config=config).read_all()
+
+
 def test_types(session, clean_bucket_name):
     columns = pa.schema([
         ('tb', pa.bool_()),
         ('a1', pa.int8()),
         ('a2', pa.int16()),
         ('a4', pa.int64()),
         ('b', pa.float32()),
```

### Comparing `vastdb-0.1.6/vastdb/tests/test_util.py` & `vastdb-0.1.7/vastdb/tests/test_util.py`

 * *Files 18% similar despite different names*

```diff
@@ -29,11 +29,17 @@
     t = pa.table(values, schema=pa.schema(cols))
     assert len(t) == 1
 
     with pytest.raises(errors.TooWideRow):
         list(util.iter_serialized_slices(t))
 
 
+def test_expand_ip_ranges():
+    endpoints = ["http://172.19.101.1-3"]
+    expected = ["http://172.19.101.1", "http://172.19.101.2", "http://172.19.101.3"]
+    assert util.expand_ip_ranges(endpoints) == expected
+
+
 def _parse(bufs):
     for buf in bufs:
         with pa.ipc.open_stream(buf) as reader:
             yield from reader
```

### Comparing `vastdb-0.1.6/vastdb/tests/util.py` & `vastdb-0.1.7/vastdb/tests/util.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.6/vastdb/transaction.py` & `vastdb-0.1.7/vastdb/transaction.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
     with session.transaction() as tx:
         tx.bucket("bucket").create_schema("schema")
 """
 
 import logging
 from dataclasses import dataclass
-from typing import TYPE_CHECKING, List, Optional
+from typing import TYPE_CHECKING, Iterable, Optional
 
 import botocore
 
 from . import bucket, errors, schema, session
 
 if TYPE_CHECKING:
     from bucket import Bucket
@@ -68,15 +68,15 @@
         except botocore.exceptions.ClientError as e:
             log.warning("res: %s", e.response)
             if e.response['Error']['Code'] == '404':
                 raise errors.MissingBucket(name) from e
             raise
         return bucket.Bucket(name, self)
 
-    def catalog_snapshots(self) -> List["Bucket"]:
+    def catalog_snapshots(self) -> Iterable["Bucket"]:
         """Return VAST Catalog bucket snapshots."""
         return bucket.Bucket(VAST_CATALOG_BUCKET_NAME, self).snapshots()
 
     def catalog(self, snapshot: Optional["Bucket"] = None, fail_if_missing=True) -> Optional["Table"]:
         """Return VAST Catalog table."""
         b = snapshot or bucket.Bucket(VAST_CATALOG_BUCKET_NAME, self)
         s = schema.Schema(VAST_CATALOG_SCHEMA_NAME, b)
```

### Comparing `vastdb-0.1.6/vastdb.egg-info/PKG-INFO` & `vastdb-0.1.7/vastdb.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vastdb
-Version: 0.1.6
+Version: 0.1.7
 Summary: VAST Data SDK
 Home-page: https://github.com/vast-data/vastdb_sdk
 Author: VAST DATA
 Author-email: hello@vastdata.com
 License: Copyright (C) VAST Data Ltd.
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: Apache Software License
@@ -17,15 +17,15 @@
 Classifier: Topic :: Database :: Front-Ends
 Requires-Python: >=3.9.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: aws-requests-auth
 Requires-Dist: boto3
 Requires-Dist: flatbuffers
-Requires-Dist: ibis-framework==8.0.0
+Requires-Dist: ibis-framework==9.0.0
 Requires-Dist: pyarrow
 Requires-Dist: requests
 Requires-Dist: xmltodict
 Requires-Dist: backoff==2.2.1
 
 
 `vastdb` is a Python-based SDK designed for interacting
```

### Comparing `vastdb-0.1.6/vastdb.egg-info/SOURCES.txt` & `vastdb-0.1.7/vastdb.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -151,18 +151,18 @@
 vast_flatbuf/tabular/ListSchemasResponse.py
 vast_flatbuf/tabular/ListTablesResponse.py
 vast_flatbuf/tabular/ObjectDetails.py
 vast_flatbuf/tabular/S3File.py
 vast_flatbuf/tabular/VipRange.py
 vast_flatbuf/tabular/__init__.py
 vastdb/__init__.py
+vastdb/_internal.py
 vastdb/bucket.py
 vastdb/conftest.py
 vastdb/errors.py
-vastdb/internal_commands.py
 vastdb/schema.py
 vastdb/session.py
 vastdb/table.py
 vastdb/transaction.py
 vastdb/util.py
 vastdb.egg-info/PKG-INFO
 vastdb.egg-info/SOURCES.txt
```

