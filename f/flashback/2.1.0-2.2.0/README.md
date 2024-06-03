# Comparing `tmp/flashback-2.1.0.tar.gz` & `tmp/flashback-2.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flashback-2.1.0.tar", last modified: Sun Jun  2 00:54:17 2024, max compression
+gzip compressed data, was "flashback-2.2.0.tar", last modified: Mon Jun  3 09:00:28 2024, max compression
```

## Comparing `flashback-2.1.0.tar` & `flashback-2.2.0.tar`

### file list

```diff
@@ -1,106 +1,107 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 00:54:17.661113 flashback-2.1.0/
--rw-r--r--   0 runner    (1001) docker     (127)     6511 2024-06-02 00:53:57.000000 flashback-2.1.0/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (127)     1077 2024-06-02 00:53:57.000000 flashback-2.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      143 2024-06-02 00:53:57.000000 flashback-2.1.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     6197 2024-06-02 00:54:17.661113 flashback-2.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5142 2024-06-02 00:53:57.000000 flashback-2.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 00:54:17.649113 flashback-2.1.0/flashback/
--rw-r--r--   0 runner    (1001) docker     (127)      538 2024-06-02 00:53:57.000000 flashback-2.1.0/flashback/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 00:54:17.653113 flashback-2.1.0/flashback/accessing/
--rw-r--r--   0 runner    (1001) docker     (127)      133 2024-06-02 00:53:57.000000 flashback-2.1.0/flashback/accessing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1254 2024-06-02 00:53:57.000000 flashback-2.1.0/flashback/accessing/dig.py
--rw-r--r--   0 runner    (1001) docker     (127)      761 2024-06-02 00:53:57.000000 flashback-2.1.0/flashback/accessing/pick.py
--rw-r--r--   0 runner    (1001) docker     (127)      718 2024-06-02 00:53:57.000000 flashback-2.1.0/flashback/accessing/values_at.py
--rw-r--r--   0 runner    (1001) docker     (127)     4777 2024-06-02 00:53:57.000000 flashback-2.1.0/flashback/borg.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 00:54:17.653113 flashback-2.1.0/flashback/caching/
--rw-r--r--   0 runner    (1001) docker     (127)       95 2024-06-02 00:53:57.000000 flashback-2.1.0/flashback/caching/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 00:54:17.653113 flashback-2.1.0/flashback/caching/adapters/
--rw-r--r--   0 runner    (1001) docker     (127)      268 2024-06-02 00:53:57.000000 flashback-2.1.0/flashback/caching/adapters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4325 2024-06-02 00:53:57.000000 flashback-2.1.0/flashback/caching/adapters/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     2995 2024-06-02 00:53:57.000000 flashback-2.1.0/flashback/caching/adapters/disk_adapter.py
--rw-r--r--   0 runner    (1001) docker     (127)     3008 2024-06-02 00:53:57.000000 flashback-2.1.0/flashback/caching/adapters/memcached_adapter.py
--rw-r--r--   0 runner    (1001) docker     (127)     2093 2024-06-02 00:53:57.000000 flashback-2.1.0/flashback/caching/adapters/memory_adapter.py
--rw-r--r--   0 runner    (1001) docker     (127)     2253 2024-06-02 00:53:57.000000 flashback-2.1.0/flashback/caching/adapters/redis_adapter.py
--rw-r--r--   0 runner    (1001) docker     (127)     9412 2024-06-02 00:53:57.000000 flashback-2.1.0/flashback/caching/cache.py
--rw-r--r--   0 runner    (1001) docker     (127)     1977 2024-06-02 00:53:57.000000 flashback-2.1.0/flashback/caching/cached.py
--rw-r--r--   0 runner    (1001) docker     (127)     2756 2024-06-02 00:53:57.000000 flashback-2.1.0/flashback/classproperty.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 00:54:17.653113 flashback-2.1.0/flashback/debugging/
--rw-r--r--   0 runner    (1001) docker     (127)      325 2024-06-02 00:53:57.000000 flashback-2.1.0/flashback/debugging/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3248 2024-06-02 00:53:57.000000 flashback-2.1.0/flashback/debugging/caller.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 00:54:17.657113 flashback-2.1.0/flashback/debugging/filters/
--rw-r--r--   0 runner    (1001) docker     (127)      274 2024-06-02 00:53:57.000000 flashback-2.1.0/flashback/debugging/filters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1966 2024-06-02 00:53:57.000000 flashback-2.1.0/flashback/debugging/filters/call_highlight_filter.py
--rw-r--r--   0 runner    (1001) docker     (127)     1253 2024-06-02 00:53:57.000000 flashback-2.1.0/flashback/debugging/filters/decorator_operator_filter.py
--rw-r--r--   0 runner    (1001) docker     (127)     1141 2024-06-02 00:53:57.000000 flashback-2.1.0/flashback/debugging/filters/type_highlight_filter.py
--rw-r--r--   0 runner    (1001) docker     (127)    12467 2024-06-02 00:53:57.000000 flashback-2.1.0/flashback/debugging/formatter.py
--rw-r--r--   0 runner    (1001) docker     (127)     2983 2024-06-02 00:53:57.000000 flashback-2.1.0/flashback/debugging/get_call_context.py
--rw-r--r--   0 runner    (1001) docker     (127)     2014 2024-06-02 00:53:57.000000 flashback-2.1.0/flashback/debugging/get_callable.py
--rw-r--r--   0 runner    (1001) docker     (127)     1580 2024-06-02 00:53:57.000000 flashback-2.1.0/flashback/debugging/get_frameinfo.py
--rw-r--r--   0 runner    (1001) docker     (127)     7920 2024-06-02 00:53:57.000000 flashback-2.1.0/flashback/debugging/parser.py
--rw-r--r--   0 runner    (1001) docker     (127)     1870 2024-06-02 00:53:57.000000 flashback-2.1.0/flashback/debugging/profiled.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 00:54:17.657113 flashback-2.1.0/flashback/debugging/styles/
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-06-02 00:53:57.000000 flashback-2.1.0/flashback/debugging/styles/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2225 2024-06-02 00:53:57.000000 flashback-2.1.0/flashback/debugging/styles/jellybeans.py
--rw-r--r--   0 runner    (1001) docker     (127)     2314 2024-06-02 00:53:57.000000 flashback-2.1.0/flashback/debugging/xp.py
--rw-r--r--   0 runner    (1001) docker     (127)     1520 2024-06-02 00:53:57.000000 flashback-2.1.0/flashback/deprecated.py
--rw-r--r--   0 runner    (1001) docker     (127)     6574 2024-06-02 00:53:57.000000 flashback-2.1.0/flashback/encrypted_file.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 00:54:17.657113 flashback-2.1.0/flashback/formatting/
--rw-r--r--   0 runner    (1001) docker     (127)      640 2024-06-02 00:53:57.000000 flashback-2.1.0/flashback/formatting/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1145 2024-06-02 00:53:57.000000 flashback-2.1.0/flashback/formatting/_inflect.py
--rw-r--r--   0 runner    (1001) docker     (127)      782 2024-06-02 00:53:57.000000 flashback-2.1.0/flashback/formatting/adverbize.py
--rw-r--r--   0 runner    (1001) docker     (127)     1592 2024-06-02 00:53:57.000000 flashback-2.1.0/flashback/formatting/camelize.py
--rw-r--r--   0 runner    (1001) docker     (127)     1011 2024-06-02 00:53:57.000000 flashback-2.1.0/flashback/formatting/kebabize.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 00:54:17.657113 flashback-2.1.0/flashback/formatting/locales/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-02 00:53:57.000000 flashback-2.1.0/flashback/formatting/locales/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6568 2024-06-02 00:53:57.000000 flashback-2.1.0/flashback/formatting/locales/de.py
--rw-r--r--   0 runner    (1001) docker     (127)    17353 2024-06-02 00:53:57.000000 flashback-2.1.0/flashback/formatting/locales/en.py
--rw-r--r--   0 runner    (1001) docker     (127)     4821 2024-06-02 00:53:57.000000 flashback-2.1.0/flashback/formatting/locales/es.py
--rw-r--r--   0 runner    (1001) docker     (127)    11522 2024-06-02 00:53:57.000000 flashback-2.1.0/flashback/formatting/locales/fr.py
--rw-r--r--   0 runner    (1001) docker     (127)     1117 2024-06-02 00:53:57.000000 flashback-2.1.0/flashback/formatting/ordinalize.py
--rw-r--r--   0 runner    (1001) docker     (127)     1391 2024-06-02 00:53:57.000000 flashback-2.1.0/flashback/formatting/oxford_join.py
--rw-r--r--   0 runner    (1001) docker     (127)     1443 2024-06-02 00:53:57.000000 flashback-2.1.0/flashback/formatting/parameterize.py
--rw-r--r--   0 runner    (1001) docker     (127)     1220 2024-06-02 00:53:57.000000 flashback-2.1.0/flashback/formatting/pascalize.py
--rw-r--r--   0 runner    (1001) docker     (127)     1224 2024-06-02 00:53:57.000000 flashback-2.1.0/flashback/formatting/pluralize.py
--rw-r--r--   0 runner    (1001) docker     (127)     1248 2024-06-02 00:53:57.000000 flashback-2.1.0/flashback/formatting/singularize.py
--rw-r--r--   0 runner    (1001) docker     (127)     1809 2024-06-02 00:53:57.000000 flashback-2.1.0/flashback/formatting/snakeize.py
--rw-r--r--   0 runner    (1001) docker     (127)      808 2024-06-02 00:53:57.000000 flashback-2.1.0/flashback/formatting/transliterate.py
--rw-r--r--   0 runner    (1001) docker     (127)     1749 2024-06-02 00:53:57.000000 flashback-2.1.0/flashback/formatting/truncate.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 00:54:17.657113 flashback-2.1.0/flashback/i16g/
--rw-r--r--   0 runner    (1001) docker     (127)       57 2024-06-02 00:53:57.000000 flashback-2.1.0/flashback/i16g/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5190 2024-06-02 00:53:57.000000 flashback-2.1.0/flashback/i16g/locale.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 00:54:17.657113 flashback-2.1.0/flashback/importing/
--rw-r--r--   0 runner    (1001) docker     (127)      197 2024-06-02 00:53:57.000000 flashback-2.1.0/flashback/importing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1818 2024-06-02 00:53:57.000000 flashback-2.1.0/flashback/importing/import_class_from_path.py
--rw-r--r--   0 runner    (1001) docker     (127)     1431 2024-06-02 00:53:57.000000 flashback-2.1.0/flashback/importing/import_module_from_path.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 00:54:17.661113 flashback-2.1.0/flashback/iterating/
--rw-r--r--   0 runner    (1001) docker     (127)      374 2024-06-02 00:53:57.000000 flashback-2.1.0/flashback/iterating/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1180 2024-06-02 00:53:57.000000 flashback-2.1.0/flashback/iterating/chunks.py
--rw-r--r--   0 runner    (1001) docker     (127)      546 2024-06-02 00:53:57.000000 flashback-2.1.0/flashback/iterating/compact.py
--rw-r--r--   0 runner    (1001) docker     (127)      911 2024-06-02 00:53:57.000000 flashback-2.1.0/flashback/iterating/flat_map.py
--rw-r--r--   0 runner    (1001) docker     (127)      821 2024-06-02 00:53:57.000000 flashback-2.1.0/flashback/iterating/flatten.py
--rw-r--r--   0 runner    (1001) docker     (127)      908 2024-06-02 00:53:57.000000 flashback-2.1.0/flashback/iterating/partition.py
--rw-r--r--   0 runner    (1001) docker     (127)      733 2024-06-02 00:53:57.000000 flashback-2.1.0/flashback/iterating/renumerate.py
--rw-r--r--   0 runner    (1001) docker     (127)      896 2024-06-02 00:53:57.000000 flashback-2.1.0/flashback/iterating/uniq.py
--rw-r--r--   0 runner    (1001) docker     (127)     1311 2024-06-02 00:53:57.000000 flashback-2.1.0/flashback/iterating/uniq_by.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 00:54:17.661113 flashback-2.1.0/flashback/logging/
--rw-r--r--   0 runner    (1001) docker     (127)      606 2024-06-02 00:53:57.000000 flashback-2.1.0/flashback/logging/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3241 2024-06-02 00:53:57.000000 flashback-2.1.0/flashback/logging/affixed_stream_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)     4745 2024-06-02 00:53:57.000000 flashback-2.1.0/flashback/logging/configurations.py
--rw-r--r--   0 runner    (1001) docker     (127)     2338 2024-06-02 00:53:57.000000 flashback-2.1.0/flashback/logging/muted.py
--rw-r--r--   0 runner    (1001) docker     (127)     3542 2024-06-02 00:53:57.000000 flashback-2.1.0/flashback/retryable.py
--rw-r--r--   0 runner    (1001) docker     (127)     4115 2024-06-02 00:53:57.000000 flashback-2.1.0/flashback/sampled.py
--rw-r--r--   0 runner    (1001) docker     (127)      761 2024-06-02 00:53:57.000000 flashback-2.1.0/flashback/sentinel.py
--rw-r--r--   0 runner    (1001) docker     (127)     2305 2024-06-02 00:53:57.000000 flashback-2.1.0/flashback/singleton.py
--rw-r--r--   0 runner    (1001) docker     (127)     1371 2024-06-02 00:53:57.000000 flashback-2.1.0/flashback/timed.py
--rw-r--r--   0 runner    (1001) docker     (127)     1320 2024-06-02 00:53:57.000000 flashback-2.1.0/flashback/timeoutable.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 00:54:17.653113 flashback-2.1.0/flashback.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6197 2024-06-02 00:54:17.000000 flashback-2.1.0/flashback.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2824 2024-06-02 00:54:17.000000 flashback-2.1.0/flashback.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-02 00:54:17.000000 flashback-2.1.0/flashback.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      103 2024-06-02 00:54:17.000000 flashback-2.1.0/flashback.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-06-02 00:54:17.000000 flashback-2.1.0/flashback.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      110 2024-06-02 00:53:57.000000 flashback-2.1.0/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (127)      136 2024-06-02 00:53:57.000000 flashback-2.1.0/requirements-test.txt
--rw-r--r--   0 runner    (1001) docker     (127)      122 2024-06-02 00:53:57.000000 flashback-2.1.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-06-02 00:54:17.661113 flashback-2.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2273 2024-06-02 00:53:57.000000 flashback-2.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 09:00:28.353516 flashback-2.2.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     6554 2024-06-03 09:00:10.000000 flashback-2.2.0/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1077 2024-06-03 09:00:10.000000 flashback-2.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      143 2024-06-03 09:00:10.000000 flashback-2.2.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     6197 2024-06-03 09:00:28.353516 flashback-2.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5142 2024-06-03 09:00:10.000000 flashback-2.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 09:00:28.341516 flashback-2.2.0/flashback/
+-rw-r--r--   0 runner    (1001) docker     (127)      538 2024-06-03 09:00:10.000000 flashback-2.2.0/flashback/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 09:00:28.345516 flashback-2.2.0/flashback/accessing/
+-rw-r--r--   0 runner    (1001) docker     (127)      133 2024-06-03 09:00:10.000000 flashback-2.2.0/flashback/accessing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1296 2024-06-03 09:00:10.000000 flashback-2.2.0/flashback/accessing/dig.py
+-rw-r--r--   0 runner    (1001) docker     (127)      836 2024-06-03 09:00:10.000000 flashback-2.2.0/flashback/accessing/pick.py
+-rw-r--r--   0 runner    (1001) docker     (127)      788 2024-06-03 09:00:10.000000 flashback-2.2.0/flashback/accessing/values_at.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4727 2024-06-03 09:00:10.000000 flashback-2.2.0/flashback/borg.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 09:00:28.345516 flashback-2.2.0/flashback/caching/
+-rw-r--r--   0 runner    (1001) docker     (127)       95 2024-06-03 09:00:10.000000 flashback-2.2.0/flashback/caching/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 09:00:28.345516 flashback-2.2.0/flashback/caching/adapters/
+-rw-r--r--   0 runner    (1001) docker     (127)      268 2024-06-03 09:00:10.000000 flashback-2.2.0/flashback/caching/adapters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4469 2024-06-03 09:00:10.000000 flashback-2.2.0/flashback/caching/adapters/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3444 2024-06-03 09:00:10.000000 flashback-2.2.0/flashback/caching/adapters/disk_adapter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3156 2024-06-03 09:00:10.000000 flashback-2.2.0/flashback/caching/adapters/memcached_adapter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2468 2024-06-03 09:00:10.000000 flashback-2.2.0/flashback/caching/adapters/memory_adapter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2612 2024-06-03 09:00:10.000000 flashback-2.2.0/flashback/caching/adapters/redis_adapter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9489 2024-06-03 09:00:10.000000 flashback-2.2.0/flashback/caching/cache.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1990 2024-06-03 09:00:10.000000 flashback-2.2.0/flashback/caching/cached.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2822 2024-06-03 09:00:10.000000 flashback-2.2.0/flashback/classproperty.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 09:00:28.345516 flashback-2.2.0/flashback/debugging/
+-rw-r--r--   0 runner    (1001) docker     (127)      325 2024-06-03 09:00:10.000000 flashback-2.2.0/flashback/debugging/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3398 2024-06-03 09:00:10.000000 flashback-2.2.0/flashback/debugging/caller.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 09:00:28.345516 flashback-2.2.0/flashback/debugging/filters/
+-rw-r--r--   0 runner    (1001) docker     (127)      274 2024-06-03 09:00:10.000000 flashback-2.2.0/flashback/debugging/filters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2089 2024-06-03 09:00:10.000000 flashback-2.2.0/flashback/debugging/filters/call_highlight_filter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1368 2024-06-03 09:00:10.000000 flashback-2.2.0/flashback/debugging/filters/decorator_operator_filter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1252 2024-06-03 09:00:10.000000 flashback-2.2.0/flashback/debugging/filters/type_highlight_filter.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13429 2024-06-03 09:00:10.000000 flashback-2.2.0/flashback/debugging/formatter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3029 2024-06-03 09:00:10.000000 flashback-2.2.0/flashback/debugging/get_call_context.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2114 2024-06-03 09:00:10.000000 flashback-2.2.0/flashback/debugging/get_callable.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1601 2024-06-03 09:00:10.000000 flashback-2.2.0/flashback/debugging/get_frameinfo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7104 2024-06-03 09:00:10.000000 flashback-2.2.0/flashback/debugging/parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2034 2024-06-03 09:00:10.000000 flashback-2.2.0/flashback/debugging/profiled.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 09:00:28.345516 flashback-2.2.0/flashback/debugging/styles/
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-06-03 09:00:10.000000 flashback-2.2.0/flashback/debugging/styles/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2347 2024-06-03 09:00:10.000000 flashback-2.2.0/flashback/debugging/styles/jellybeans.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2409 2024-06-03 09:00:10.000000 flashback-2.2.0/flashback/debugging/xp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1620 2024-06-03 09:00:10.000000 flashback-2.2.0/flashback/deprecated.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6740 2024-06-03 09:00:10.000000 flashback-2.2.0/flashback/encrypted_file.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 09:00:28.349516 flashback-2.2.0/flashback/formatting/
+-rw-r--r--   0 runner    (1001) docker     (127)      640 2024-06-03 09:00:10.000000 flashback-2.2.0/flashback/formatting/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1292 2024-06-03 09:00:10.000000 flashback-2.2.0/flashback/formatting/_inflect.py
+-rw-r--r--   0 runner    (1001) docker     (127)      783 2024-06-03 09:00:10.000000 flashback-2.2.0/flashback/formatting/adverbize.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1655 2024-06-03 09:00:10.000000 flashback-2.2.0/flashback/formatting/camelize.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1100 2024-06-03 09:00:10.000000 flashback-2.2.0/flashback/formatting/kebabize.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 09:00:28.349516 flashback-2.2.0/flashback/formatting/locales/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 09:00:10.000000 flashback-2.2.0/flashback/formatting/locales/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6890 2024-06-03 09:00:10.000000 flashback-2.2.0/flashback/formatting/locales/de.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20078 2024-06-03 09:00:10.000000 flashback-2.2.0/flashback/formatting/locales/en.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4910 2024-06-03 09:00:10.000000 flashback-2.2.0/flashback/formatting/locales/es.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14310 2024-06-03 09:00:10.000000 flashback-2.2.0/flashback/formatting/locales/fr.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1118 2024-06-03 09:00:10.000000 flashback-2.2.0/flashback/formatting/ordinalize.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1491 2024-06-03 09:00:10.000000 flashback-2.2.0/flashback/formatting/oxford_join.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1438 2024-06-03 09:00:10.000000 flashback-2.2.0/flashback/formatting/parameterize.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1329 2024-06-03 09:00:10.000000 flashback-2.2.0/flashback/formatting/pascalize.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1194 2024-06-03 09:00:10.000000 flashback-2.2.0/flashback/formatting/pluralize.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1235 2024-06-03 09:00:10.000000 flashback-2.2.0/flashback/formatting/singularize.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1880 2024-06-03 09:00:10.000000 flashback-2.2.0/flashback/formatting/snakeize.py
+-rw-r--r--   0 runner    (1001) docker     (127)      810 2024-06-03 09:00:10.000000 flashback-2.2.0/flashback/formatting/transliterate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1753 2024-06-03 09:00:10.000000 flashback-2.2.0/flashback/formatting/truncate.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 09:00:28.349516 flashback-2.2.0/flashback/i16g/
+-rw-r--r--   0 runner    (1001) docker     (127)       57 2024-06-03 09:00:10.000000 flashback-2.2.0/flashback/i16g/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5318 2024-06-03 09:00:10.000000 flashback-2.2.0/flashback/i16g/locale.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 09:00:28.349516 flashback-2.2.0/flashback/importing/
+-rw-r--r--   0 runner    (1001) docker     (127)      197 2024-06-03 09:00:10.000000 flashback-2.2.0/flashback/importing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1813 2024-06-03 09:00:10.000000 flashback-2.2.0/flashback/importing/import_class_from_path.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1439 2024-06-03 09:00:10.000000 flashback-2.2.0/flashback/importing/import_module_from_path.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 09:00:28.349516 flashback-2.2.0/flashback/iterating/
+-rw-r--r--   0 runner    (1001) docker     (127)      374 2024-06-03 09:00:10.000000 flashback-2.2.0/flashback/iterating/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1373 2024-06-03 09:00:10.000000 flashback-2.2.0/flashback/iterating/chunks.py
+-rw-r--r--   0 runner    (1001) docker     (127)      668 2024-06-03 09:00:10.000000 flashback-2.2.0/flashback/iterating/compact.py
+-rw-r--r--   0 runner    (1001) docker     (127)      974 2024-06-03 09:00:10.000000 flashback-2.2.0/flashback/iterating/flat_map.py
+-rw-r--r--   0 runner    (1001) docker     (127)      962 2024-06-03 09:00:10.000000 flashback-2.2.0/flashback/iterating/flatten.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-06-03 09:00:10.000000 flashback-2.2.0/flashback/iterating/partition.py
+-rw-r--r--   0 runner    (1001) docker     (127)      961 2024-06-03 09:00:10.000000 flashback-2.2.0/flashback/iterating/renumerate.py
+-rw-r--r--   0 runner    (1001) docker     (127)      947 2024-06-03 09:00:10.000000 flashback-2.2.0/flashback/iterating/uniq.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1353 2024-06-03 09:00:10.000000 flashback-2.2.0/flashback/iterating/uniq_by.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 09:00:28.353516 flashback-2.2.0/flashback/logging/
+-rw-r--r--   0 runner    (1001) docker     (127)      606 2024-06-03 09:00:10.000000 flashback-2.2.0/flashback/logging/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3316 2024-06-03 09:00:10.000000 flashback-2.2.0/flashback/logging/affixed_stream_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4293 2024-06-03 09:00:10.000000 flashback-2.2.0/flashback/logging/configurations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2399 2024-06-03 09:00:10.000000 flashback-2.2.0/flashback/logging/muted.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3646 2024-06-03 09:00:10.000000 flashback-2.2.0/flashback/retryable.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4256 2024-06-03 09:00:10.000000 flashback-2.2.0/flashback/sampled.py
+-rw-r--r--   0 runner    (1001) docker     (127)      762 2024-06-03 09:00:10.000000 flashback-2.2.0/flashback/sentinel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2316 2024-06-03 09:00:10.000000 flashback-2.2.0/flashback/singleton.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1409 2024-06-03 09:00:10.000000 flashback-2.2.0/flashback/timed.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1362 2024-06-03 09:00:10.000000 flashback-2.2.0/flashback/timeoutable.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 09:00:28.341516 flashback-2.2.0/flashback.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6197 2024-06-03 09:00:28.000000 flashback-2.2.0/flashback.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2839 2024-06-03 09:00:28.000000 flashback-2.2.0/flashback.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-03 09:00:28.000000 flashback-2.2.0/flashback.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      137 2024-06-03 09:00:28.000000 flashback-2.2.0/flashback.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-06-03 09:00:28.000000 flashback-2.2.0/flashback.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      556 2024-06-03 09:00:10.000000 flashback-2.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      124 2024-06-03 09:00:10.000000 flashback-2.2.0/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      176 2024-06-03 09:00:10.000000 flashback-2.2.0/requirements-test.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      156 2024-06-03 09:00:10.000000 flashback-2.2.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-06-03 09:00:28.353516 flashback-2.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2273 2024-06-03 09:00:10.000000 flashback-2.2.0/setup.py
```

### Comparing `flashback-2.1.0/CHANGELOG.md` & `flashback-2.2.0/CHANGELOG.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,13 @@
 # Changelog
 
+## 2.2.0 (06/03/2024)
+
+- Added WIP typing
+
 ## 2.1.0 (06/02/2024)
 
 - Added `iterating/uniq_by` to remove duplicates from an iterable while keeping the items' order with a user-supplied callable
 - Added `accessing/pick` to fetch key/value pairs with given keys from a dictionary
 - Added `accessing/values_at` to retrieves values from each given keys in dictionary
 - Updated `accessing/dig` to support sequences and their indices
 - Fixed `iterating/flat_map` to correctly load flatten method
```

### Comparing `flashback-2.1.0/LICENSE` & `flashback-2.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `flashback-2.1.0/PKG-INFO` & `flashback-2.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flashback
-Version: 2.1.0
+Version: 2.2.0
 Summary: An utility library for python
 Home-page: https://github.com/PaulRenvoise/flashback
 Author: Paul Renvoisé
 Author-email: renvoisepaul@gmail.com
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
@@ -121,15 +121,15 @@
 The Pull Request template has a checklist containing everything you need to submit a new PR.
 
 Run the tests with `pytest`:
 ```bash
 pytest tests
 ```
 
-Run the lint with `pylint`:
+Run the lint with `ruff`:
 ```bash
-pylint flashback/ tests/
+ruff check flashback tests
 ```
 
 ## License
 
 Flashback is released under the [MIT License](https://tldrlegal.com/license/mit-license#summary).
```

### Comparing `flashback-2.1.0/README.md` & `flashback-2.2.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -94,15 +94,15 @@
 The Pull Request template has a checklist containing everything you need to submit a new PR.
 
 Run the tests with `pytest`:
 ```bash
 pytest tests
 ```
 
-Run the lint with `pylint`:
+Run the lint with `ruff`:
 ```bash
-pylint flashback/ tests/
+ruff check flashback tests
 ```
 
 ## License
 
 Flashback is released under the [MIT License](https://tldrlegal.com/license/mit-license#summary).
```

### Comparing `flashback-2.1.0/flashback/__init__.py` & `flashback-2.2.0/flashback/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,8 +20,8 @@
     "deprecated",
     "retryable",
     "sampled",
     "timed",
     "timeoutable",
 )
 
-__version__ = "2.1.0"
+__version__ = "2.2.0"
```

### Comparing `flashback-2.1.0/flashback/accessing/dig.py` & `flashback-2.2.0/flashback/accessing/dig.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 from __future__ import annotations
 
-from collections.abc import Sequence
-from typing import Any
+from collections.abc import Sequence, Hashable
+from typing import TypeVar
 
+T = TypeVar("T")
 
-def dig(container: dict[Any, Any] | Sequence[Any], *keys: tuple[Any]) -> Any |None:
+
+def dig(container: dict[Hashable, T] | Sequence[T], *keys: tuple[Hashable, ...]) -> T | None:
     """
     Retrieves the value corresponding to each `keys` repeatedly from `container`,
     supporting both dict and list indices.
 
     Examples:
         ```python
         from flashback.accessing import dig
```

### Comparing `flashback-2.1.0/flashback/accessing/pick.py` & `flashback-2.2.0/flashback/accessing/pick.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,13 +1,16 @@
 from __future__ import annotations
 
-from typing import Any
+from collections.abc import Hashable
+from typing import TypeVar
 
+T = TypeVar("T")
 
-def pick(dictionary: dict[Any, Any], *keys: tuple[Any]) -> dict[Any, Any]:
+
+def pick(dictionary: dict[Hashable, T], *keys: tuple[Hashable, ...]) -> dict[Hashable, T]:
     """
     Fetches key/value pairs from `dictionary` corresponding to `keys`.
 
     Examples:
         ```python
         from flashback.accessing import pick
```

### Comparing `flashback-2.1.0/flashback/accessing/values_at.py` & `flashback-2.2.0/flashback/accessing/values_at.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,13 +1,16 @@
 from __future__ import annotations
 
-from typing import Any
+from collections.abc import Hashable
+from typing import TypeVar
 
+T = TypeVar("T")
 
-def values_at(dictionary: dict[Any, Any], *keys: tuple[Any]) -> list[Any]:
+
+def values_at(dictionary: dict[Hashable, T], *keys: tuple[Hashable, ...]) -> list[T]:
     """
     Retrieves the values corresponding to each `keys` in `dictionary`.
 
     Examples:
         ```python
         from flashback.accessing import values_at
```

### Comparing `flashback-2.1.0/flashback/borg.py` & `flashback-2.2.0/flashback/borg.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-# pylint: disable=access-member-before-definition
-
 class Borg:
     """
     Implements the Borg design pattern, used to implement singleton behavior across multiple
     instances of a class.
 
     In the Borg design pattern, the focus is on sharing instance state instead of instance
     identity.
@@ -31,14 +29,15 @@
         # And their attributes are not overridable
         borg_1.assign_attribute("attr", "foo")
 
         assert borg_1.attr == 0
         assert borg_2.attr == 0
         ```
     """
+
     def __new__(cls, *_args, **_kwargs):
         if "_shared_state" not in cls.__dict__:
             cls._shared_state = {}
 
         obj = object.__new__(cls)
         obj.__dict__ = cls._shared_state
```

### Comparing `flashback-2.1.0/flashback/caching/adapters/base.py` & `flashback-2.2.0/flashback/caching/adapters/base.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,158 +1,163 @@
+from __future__ import annotations
+
 from abc import ABC, abstractmethod
+from collections.abc import Sequence
+from typing import Any
 
 
 class BaseAdapter(ABC):
     """
     Defines an abstract class that needs to be implemented to register a new adapter.
     """
+
     @abstractmethod
-    def __init__(self, **kwargs):
+    def __init__(self, **kwargs) -> None:
         """
         Instanciates the adapter, without testing the connection (ping is used for that).
 
         Params:
-            kwargs (dict): every given keyword arguments
+            kwargs: every given keyword arguments
         """
 
     @abstractmethod
-    def set(self, key, value, ttl):
+    def set(self, key: str, value: Any, ttl: int) -> bool:
         """
         Caches a `value` under a given `key`.
 
         Params:
-            key (str): the key under which to cache the value
-            value (str): the value to cache
-            ttl (int): the number of seconds before expiring the key
+            key: the key under which to cache the value
+            value: the value to cache
+            ttl: the number of seconds before expiring the key
 
         Returns:
-            bool: whether or not the operation succeeded
+            whether or not the operation succeeded
 
         Raises:
             Base.connection_exceptions: if no connection to the underlying storage is active
         """
 
     @abstractmethod
-    def batch_set(self, keys, values, ttls):
+    def batch_set(self, keys: Sequence[str], values: Sequence[Any], ttls: Sequence[int]) -> bool:
         """
         Caches each value from a list of `values` to its respective key in a list of `keys`.
 
         Params:
-            keys (Iterable<str>): the keys under which to cache the values
-            values (Iterable<str>): the values to cache
-            ttls (Iterable<int>): the number of seconds before expiring the keys
+            keys: the keys under which to cache the values
+            values: the values to cache
+            ttls: the number of seconds before expiring the keys
 
         Returns:
-            bool: whether or not the operation succeeded
+            whether or not the operation succeeded
 
         Raises:
             Base.connection_exceptions: if no connection to the underlying storage is active
         """
 
     @abstractmethod
-    def get(self, key):
+    def get(self, key: str) -> Any | None:
         """
         Fetches the value stored under `key`.
 
         Params:
-            key (str): the key to retreive the value from
+            key: the key to retreive the value from
 
         Returns:
-            str|None: the value read from the cache
+            the value read from the cache
 
         Raises:
             Base.connection_exceptions: if no connection to the underlying storage is active
         """
 
     @abstractmethod
-    def batch_get(self, keys):
+    def batch_get(self, keys: Sequence[str]) -> Sequence[Any | None]:
         """
         Fetches each value stored under its respective key in a list of `keys`.
 
         Params:
-            keys (Iterable<str>): the keys to retreive the values from
+            keys: the keys to retreive the values from
 
         Returns:
-            list<str|None>: the values read from the cache
+            the values read from the cache
 
         Raises:
             Base.connection_exceptions: if no connection to the underlying storage is active
         """
 
     @abstractmethod
-    def delete(self, key):
+    def delete(self, key: str) -> bool:
         """
         Removes the given cache `key`.
 
         Params:
-            key (str): the key to remove
+            key: the key to remove
 
         Returns:
-            bool: whether or not the operation succeeded
+            whether or not the operation succeeded
 
         Raises:
             Base.connection_exceptions: if no connection to the underlying storage is active
         """
 
     @abstractmethod
-    def batch_delete(self, keys):
+    def batch_delete(self, keys: Sequence[str]) -> bool:
         """
         Removes the cache of a given list of `keys`, ignores non-existing keys.
 
         Params:
-            keys (Iterable<str>): the keys to remove from the cache
+            keys: the keys to remove from the cache
 
         Returns:
-            bool: whether or not the operation succeeded
+            whether or not the operation succeeded
 
         Raises:
             Base.connection_exceptions: if no connection to the underlying storage is active
         """
 
     @abstractmethod
-    def exists(self, key):
+    def exists(self, key: str) -> bool:
         """
         Checks the existence of a given `key` in the storage.
 
         Params:
             key (str): the key to check the existence of
 
         Returns:
-            bool: whether or not the key exists
+            whether or not the key exists
 
         Raises:
             Base.connection_exceptions: if no connection to the underlying storage is active
         """
 
     @abstractmethod
-    def flush(self):
+    def flush(self) -> bool:
         """
         Flushes all keys and values from the adapter's storage.
 
         Returns:
-            bool: always True
+            always True
 
         Raises:
             Base.connection_exceptions: if no connection to the underlying storage is active
         """
 
     @abstractmethod
-    def ping(self):
+    def ping(self) -> bool:
         """
         Checks if a valid connection is setup with the underlying storage.
 
         Returns:
-            bool: always True
+            always True
 
         Raises:
             Base.connection_exceptions: if no connection to the underlying storage is active
         """
 
     @property
     @abstractmethod
-    def connection_exceptions(self):
+    def connection_exceptions(self) -> tuple[Exception, ...]:
         """
         Lists the exceptions raised by the adapter when a faulty/invalid connection is detected.
 
         Returns:
             tuple<Exception>: the list of exceptions
         """
```

### Comparing `flashback-2.1.0/flashback/caching/adapters/disk_adapter.py` & `flashback-2.2.0/flashback/caching/adapters/disk_adapter.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,108 +1,114 @@
+from __future__ import annotations
+
+from collections.abc import Sequence, Generator
 from contextlib import contextmanager
 from datetime import datetime, timedelta
 from fcntl import flock, LOCK_SH, LOCK_EX, LOCK_UN
+from typing import Any
 import shelve
+from shelve import Shelf
 import tempfile
 import uuid
 
 from .base import BaseAdapter
 
 
 class DiskAdapter(BaseAdapter):
     """
     Exposes a cache store using a locked shelf.
 
     See: https://docs.python.org/3/library/shelve.html.
     """
 
-    def __init__(self, **kwargs):
+    def __init__(self, **_kwargs) -> None:
         super().__init__()
 
         self._store_path = f"{tempfile.gettempdir()}/{uuid.uuid4()}"
 
-    def set(self, key, value, ttl):
+    def set(self, key: str, value: Any, ttl: int) -> bool:
         if ttl == -1:
             expiry = None
         else:
             expiry = datetime.timestamp(datetime.now() + timedelta(seconds=ttl))
 
         with self._open_locked_store(LOCK_EX) as store:
             store[key] = (value, expiry)
 
         return True
 
-    def batch_set(self, keys, values, ttls):
+    def batch_set(self, keys: Sequence[str], values: Sequence[Any], ttls: Sequence[int]) -> bool:
         now = datetime.now()
+        # TODO: use relativedelta
         expiries = [None if ttl == -1 else datetime.timestamp(now + timedelta(seconds=ttl)) for ttl in ttls]
 
         values = zip(values, expiries)
 
         with self._open_locked_store(LOCK_EX) as store:
             store.update(dict(zip(keys, values)))
 
         return True
 
-    def get(self, key):
+    def get(self, key: str) -> Any | None:
         self._evict()
 
         with self._open_locked_store(LOCK_SH) as store:
             return store.get(key, (None,))[0]
 
-    def batch_get(self, keys):
+    def batch_get(self, keys: Sequence[str]) -> Sequence[Any | None]:
         self._evict()
 
         with self._open_locked_store(LOCK_SH) as store:
             return [store.get(key, (None,))[0] for key in keys]
 
-    def delete(self, key):
+    def delete(self, key: str) -> bool:
         self._evict()
 
         with self._open_locked_store(LOCK_EX) as store:
             return bool(store.pop(key, False))
 
-    def batch_delete(self, keys):
+    def batch_delete(self, keys: Sequence[str]) -> bool:
         self._evict()
 
         with self._open_locked_store(LOCK_EX) as store:
             res = [bool(store.pop(key, False)) for key in keys]
 
         return False not in res
 
-    def exists(self, key):
+    def exists(self, key: str) -> bool:
         self._evict()
 
         with self._open_locked_store(LOCK_SH) as store:
             return key in store
 
-    def flush(self):
+    def flush(self) -> bool:
         with self._open_locked_store(LOCK_EX) as store:
             store.clear()
 
         return True
 
-    def ping(self):
+    def ping(self) -> bool:
         return True
 
     @property
-    def connection_exceptions(self):
+    def connection_exceptions(self) -> tuple[Exception, ...]:
         return ()
 
     @contextmanager
-    def _open_locked_store(self, mode):
+    def _open_locked_store(self, mode: int) -> Generator[Shelf[Any], None, None]:
         with open(f"{self._store_path}.lock", "w", encoding="utf-8") as lock:
             flock(lock.fileno(), mode)  # blocking until lock is acquired
 
             try:
                 with shelve.open(self._store_path, "c") as store:
                     yield store
             finally:
                 flock(lock.fileno(), LOCK_UN)
 
-    def _evict(self):
+    def _evict(self) -> None:
         now = datetime.timestamp(datetime.now())
 
         expired_keys = set()
 
         with self._open_locked_store(LOCK_EX) as store:
             for key, (_, expiry) in store.items():
                 if expiry is not None and expiry < now:
```

### Comparing `flashback-2.1.0/flashback/caching/adapters/memcached_adapter.py` & `flashback-2.2.0/flashback/caching/adapters/memcached_adapter.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,96 +1,89 @@
+from __future__ import annotations
+
+from collections.abc import Sequence
+from typing import Any
+
 from pymemcache.client.base import Client
-from pymemcache.exceptions import *  # pylint: disable=wildcard-import,unused-wildcard-import
+from pymemcache.exceptions import *  # noqa: F403
 
 from .base import BaseAdapter
 
 
 class MemcachedAdapter(BaseAdapter):
     """
     Exposes a cache store using Memcached.
 
     Exposes `pymemcache`'s exceptions.
     """
 
-    def __init__(self, host="localhost", port=11211, **kwargs):
+    def __init__(self, host: str = "localhost", port: int = 11211, **kwargs) -> None:
         super().__init__()
 
         self.store = Client((host, port), **kwargs)
 
-    def set(self, key, value, ttl):
+    def set(self, key: str, value: Any, ttl: int) -> bool:
         if ttl == -1:
             ttl = 0
 
         return self.store.set(key, value, expire=ttl)
 
-    def batch_set(self, keys, values, ttls):
+    def batch_set(self, keys: Sequence[str], values: Sequence[Any], ttls: Sequence[int]) -> bool:
         # There's two reasons to recode pymemcache.set_multi():
         # - It returns a list of keys that failed to be inserted, and the base expects a boolean
         # - It only allows a unique ttl for all keys
         commands = []
 
         ttls = [0 if ttl == -1 else ttl for ttl in ttls]
         for key, value, ttl in zip(keys, values, ttls):
-            ttl = self.store._check_integer(ttl, "expire")  # pylint: disable=protected-access
-            key = self.store.check_key(key)
-            value, flags = self.store.serde.serialize(key, value)
-
-            command = b"set " + key
-            command += b" " + str(flags).encode(self.store.encoding)
-            command += b" " + ttl
-            command += b" " + str(len(value)).encode(self.store.encoding) + b"\r\n"
-            command += value.encode(self.store.encoding) + b"\r\n"
+            stored_ttl = self.store._check_integer(ttl, "expire")  # noqa: SLF001
+            stored_key = self.store.check_key(key)
+            stored_value, stored_flags = self.store.serde.serialize(key, value)
+
+            command = b"set " + stored_key
+            command += b" " + str(stored_flags).encode(self.store.encoding)
+            command += b" " + stored_ttl
+            command += b" " + str(len(stored_value)).encode(self.store.encoding) + b"\r\n"
+            command += stored_value.encode(self.store.encoding) + b"\r\n"
             commands.append(command)
 
-        results = self.store._misc_cmd(commands, "set", False)  # pylint: disable=protected-access
-
-        for line in results:
-            if line == b"NOT_STORED":
-                return False
+        results = self.store._misc_cmd(commands, "set", False)  # noqa: SLF001
 
-        return True
+        return all(line != b"NOT_STORED" for line in results)
 
-    def get(self, key):
-        value = self.store.get(key)
+    def get(self, key: str) -> Any | None:
+        return self.store.get(key)
 
-        return value
-
-    def batch_get(self, keys):
+    def batch_get(self, keys: Sequence[str]) -> Sequence[Any | None]:
         key_to_value = self.store.get_multi(keys)
-        values = [key_to_value[key] if key in key_to_value else None for key in keys]
-
-        return values
+        return [key_to_value.get(key, None) for key in keys]
 
-    def delete(self, key):
+    def delete(self, key: str) -> bool:
         return self.store.delete(key, noreply=False)
 
-    def batch_delete(self, keys):
+    def batch_delete(self, keys: Sequence[str]) -> bool:
         # Here as well, pymemcache.delete_multi() always returns True
         commands = []
 
         for key in keys:
-            key = self.store.check_key(key)
+            stored_key = self.store.check_key(key)
 
-            command = b"delete " + key +  b"\r\n"
+            command = b"delete " + stored_key + b"\r\n"
             commands.append(command)
 
-        results = self.store._misc_cmd(commands, "delete", False)  # pylint: disable=protected-access
-
-        for line in results:
-            if line == b"NOT_FOUND":
-                return False
+        results = self.store._misc_cmd(commands, "delete", False)  # noqa: SLF001
 
-        return True
+        return all(line != b"NOT_FOUND" for line in results)
 
-    def exists(self, key):
+    def exists(self, key: str) -> bool:
         # Can't just cast to bool since we can store falsey values
         return self.store.get(key) is not None
 
-    def flush(self):
+    def flush(self) -> bool:
         return self.store.flush_all(noreply=False)
 
-    def ping(self):
+    def ping(self) -> bool:
         return bool(self.store.stats())
 
     @property
-    def connection_exceptions(self):
-        return (MemcacheUnexpectedCloseError, MemcacheServerError, MemcacheUnknownError)
+    def connection_exceptions(self) -> tuple[Exception, ...]:
+        return (MemcacheUnexpectedCloseError, MemcacheServerError, MemcacheUnknownError)  # noqa: F405
```

### Comparing `flashback-2.1.0/flashback/caching/adapters/redis_adapter.py` & `flashback-2.2.0/flashback/caching/adapters/redis_adapter.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,9 +1,14 @@
+from __future__ import annotations
+
+from collections.abc import Sequence
+from typing import Any
+
 from redis import Redis
-from redis.exceptions import *  # pylint: disable=wildcard-import,unused-wildcard-import,redefined-builtin
+from redis.exceptions import *  # noqa: F403
 from redis.exceptions import ConnectionError as RedisConnectionError
 from redis.exceptions import TimeoutError as RedisTimeoutError
 
 from .base import BaseAdapter
 
 
 class RedisAdapter(BaseAdapter):
@@ -19,55 +24,57 @@
         super().__init__()
 
         # We would pass `decode_responses=True` to redis to avoid decoding in `get` and `batch_get`
         # but mockredis does not support it as of 2020-04-24
         self._encoding = encoding
         self.store = Redis(host=host, port=port, db=db, encoding=encoding, **kwargs)
 
-    def set(self, key, value, ttl):
+    def set(self, key: str, value: Any, ttl: int) -> bool:
         if ttl == -1:
-            ttl = None
+            converted_ttl = None
+        else:
+            converted_ttl = ttl
 
-        return self.store.set(key, value, ex=ttl)
+        return self.store.set(key, value, ex=converted_ttl)
 
-    def batch_set(self, keys, values, ttls):
-        ttls = [None if ttl == -1 else ttl for ttl in ttls]
+    def batch_set(self, keys: Sequence[str], values: Sequence[Any], ttls: Sequence[int]) -> bool:
+        converted_ttls = [None if ttl == -1 else ttl for ttl in ttls]
 
         pipe = self.store.pipeline()
 
         pipe.mset(dict(zip(keys, values)))
-        for key, ttl in zip(keys, ttls):
+        for key, ttl in zip(keys, converted_ttls):
             if ttl is not None:
                 pipe.expire(key, ttl)
 
         return pipe.execute()
 
-    def get(self, key):
+    def get(self, key: str) -> Any | None:
         value = self.store.get(key)
 
         return value.decode(self._encoding) if value is not None else None
 
-    def batch_get(self, keys):
+    def batch_get(self, keys: Sequence[str]) -> Sequence[Any | None]:
         values = self.store.mget(keys)
 
         return [value.decode(self._encoding) if value is not None else None for value in values]
 
-    def delete(self, key):
+    def delete(self, key: str) -> bool:
         return bool(self.store.delete(key))
 
-    def batch_delete(self, keys):
+    def batch_delete(self, keys: Sequence[str]) -> bool:
         res = self.store.delete(*keys)
 
         return res == len(keys)
 
-    def exists(self, key):
+    def exists(self, key: str) -> bool:
         return self.store.exists(key)
 
-    def flush(self):
+    def flush(self) -> bool:
         return self.store.flushdb()
 
-    def ping(self):
+    def ping(self) -> bool:
         return self.store.ping()
 
     @property
-    def connection_exceptions(self):
-        return (RedisConnectionError, RedisTimeoutError, ResponseError)
+    def connection_exceptions(self) -> tuple[Exception, ...]:
+        return (RedisConnectionError, RedisTimeoutError, ResponseError)  # noqa: F405
```

### Comparing `flashback-2.1.0/flashback/caching/cache.py` & `flashback-2.2.0/flashback/caching/cache.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,11 @@
-# pylint: disable=no-member
+from __future__ import annotations
+
+from collections.abc import Sequence
+from typing import Any
 
 import json
 
 from ..importing import import_class_from_path
 
 
 class Cache:
@@ -48,21 +51,22 @@
         cache.ping()
         #=> True
 
         cache.flush()
         #=> True
         ```
     """
-    def __init__(self, adapter="memory", ttl=-1, flush=False, **kwargs):
+
+    def __init__(self, adapter: str = "memory", ttl: int = -1, flush: bool = False, **kwargs) -> None:
         """
         Params:
-            adapter (str): the adapter to use for the storage
-            ttl (int): the number of seconds before expiring the keys (default: -1 (never))
-            flush (bool): whether or not to flush the storage after connecting
-            kwargs (dict): every additional keyword arguments, forwarded to the adapter
+            adapter: the adapter to use for the storage
+            ttl: the number of seconds before expiring the keys (default: -1 (never))
+            flush: whether or not to flush the storage after connecting
+            kwargs: every additional keyword arguments, forwarded to the adapter
         """
         super().__init__()
 
         self.ttl = ttl
 
         try:
             adapter_class = import_class_from_path(f"{adapter}_adapter", ".adapters")
@@ -73,66 +77,66 @@
 
         if flush:
             self.flush()
 
         # Notifies that we have a new connection
         self.ping()
 
-    def set(self, key, value, ttl=None):
+    def set(self, key: str, value: Any, ttl: int | None = None) -> bool:
         """
         Sets `key` to `value`.
 
         Examples:
             ```python
             from flashback.caching import Cache
 
             cache = Cache()
 
             cache.set("key", "val")
             #=> True
             ```
 
         Params:
-            key (str): the key to set
-            value (str): the value to cache
-            ttl (int): the number of seconds before expiring the key (default: init ttl)
+            key: the key to set
+            value: the value to cache
+            ttl: the number of seconds before expiring the key (default: init ttl)
 
         Returns:
-            bool: whether or not the operation succeeded
+            whether or not the operation succeeded
         """
         json_value = json.dumps(self._convert_numeric(value))
 
         try:
             res = self.adapter.set(key, json_value, ttl=ttl or self.ttl)
         except self.adapter.connection_exceptions:
             res = False
 
         return res
 
-    def batch_set(self, keys, values, ttls=None):
+    def batch_set(self, keys: Sequence[str], values: Sequence[Any], ttls: Sequence[int] | None = None) -> bool:
         """
         Sets a batch of `keys` to their respective `values`.
 
         Examples:
             ```python
             from flashback.caching import Cache
 
             cache = Cache()
 
             cache.batch_set(["key1", "key2"], ["val1", "val2"])
             #=> True
             ```
 
         Params:
-            keys (Iterable<str>): the list of keys to set
-            values (Iterable<str>): the list of values to cache
-            ttls (Iterable<int>): the number of seconds before expiring the keys (default: init ttl)
+            keys: the list of keys to set
+            values: the list of values to cache
+            ttls: the number of seconds before expiring the keys (default: init ttl)
 
         Returns:
-            bool: whether or not the operation succeeded
+            whether or not the operation succeeded
 
         Raises:
             ValueError: if the lengths of the keys and values differ
         """
         if ttls is None:
             ttls = [self.ttl for _ in range(len(keys))]
 
@@ -144,15 +148,15 @@
         try:
             res = self.adapter.batch_set(keys, json_values, ttls=ttls)
         except self.adapter.connection_exceptions:
             res = False
 
         return res
 
-    def get(self, key):
+    def get(self, key: str) -> Any | None:
         """
         Fetches the value stored under `key`.
 
         Examples:
             ```python
             from flashback.caching import Cache
 
@@ -163,28 +167,28 @@
             #=> "val"
 
             cache.get("yek")
             #=> None
             ```
 
         Params:
-            key (str): the key to fetch the value from
+            key: the key to fetch the value from
 
         Returns:
-            str|None: the value read from the storage
+            the value read from the storage
         """
         try:
             json_value = self.adapter.get(key)
             value = self._decode_json(json_value)
         except self.adapter.connection_exceptions:
             value = None
 
         return value
 
-    def batch_get(self, keys):
+    def batch_get(self, keys: Sequence[str]) -> Sequence[Any | None]:
         """
         Fetches the values stored under `keys`.
 
         Examples:
             ```python
             from flashback.caching import Cache
 
@@ -192,28 +196,28 @@
             cache.set("key", "val")
 
             cache.batch_get(["key", "yek"])
             #=> ["val", None]
             ```
 
         Params:
-            keys (Iterable<str>): the keys to fetch the values from
+            keys: the keys to fetch the values from
 
         Returns:
-            list<str|None>: the values read from the storage
+            the values read from the storage
         """
         try:
             json_values = self.adapter.batch_get(keys)
             values = [self._decode_json(json_value) for json_value in json_values]
         except self.adapter.connection_exceptions:
             values = [None] * len(keys)
 
         return values
 
-    def delete(self, key):
+    def delete(self, key: str) -> bool:
         """
         Deletes the given `key` from the storage.
 
         Examples:
             ```python
             from flashback.caching import Cache
 
@@ -224,27 +228,27 @@
             #=> True
 
             cache.delete("yek")
             #=> False
             ```
 
         Params:
-            key (str): the key to remove
+            key: the key to remove
 
         Returns:
-            bool: whether or not the operation succeeded
+            whether or not the operation succeeded
         """
         try:
             res = self.adapter.delete(key)
         except self.adapter.connection_exceptions:
             res = False
 
         return res
 
-    def batch_delete(self, keys):
+    def batch_delete(self, keys: Sequence[str]) -> bool:
         """
         Deletes the given `keys` from the storage, ignoring non-existing keys.
 
         Examples:
             ```python
             from flashback.caching import Cache
 
@@ -255,27 +259,27 @@
             #=> True
 
             cache.batch_delete(["yek"])
             #=> False
             ```
 
         Params:
-            keys (Iterable<str>): the keys to remove from the cache
+            keys: the keys to remove from the cache
 
         Returns:
-            bool: whether or not the operation succeeded
+            whether or not the operation succeeded
         """
         try:
             res = self.adapter.batch_delete(keys)
         except self.adapter.connection_exceptions:
             res = False
 
         return res
 
-    def exists(self, key):
+    def exists(self, key: str) -> bool:
         """
         Checks whether or not the given `key` exists in the storage.
 
         Examples:
             ```python
             from flashback.caching import Cache
 
@@ -286,27 +290,27 @@
             #=> True
 
             cache.exists("yek")
             #=> False
             ```
 
         Params:
-            key (str): the key to check the existence of
+            key: the key to check the existence of
 
         Returns:
-            bool: whether or not the key exists
+            whether or not the key exists
         """
         try:
             res = self.adapter.exists(key)
         except self.adapter.connection_exceptions:
             res = False
 
         return res
 
-    def flush(self):
+    def flush(self) -> bool:
         """
         Flushes all keys from the storage.
 
         Examples:
             ```python
             from flashback.caching import Cache
 
@@ -314,50 +318,50 @@
             cache.set("key", "val")
 
             cache.flush()
             #=> True
             ```
 
         Returns:
-            bool: always True
+            always True
 
         Raises:
             flashback.caching.adapters.base.BaseAdapter.connection_exceptions: if no connection with the storage
         """
         return self.adapter.flush()
 
-    def ping(self):
+    def ping(self) -> bool:
         """
         Checks if a valid connection exists with the storage.
 
         Examples:
             ```python
             from flashback.caching import Cache
 
             cache = Cache()
 
             cache.ping()
             #=> True
             ```
 
         Returns:
-            bool: always True
+            always True
 
         Raises:
             flashback.caching.adapters.base.BaseAdapter.connection_exceptions: if no connection with the storage
         """
         return self.adapter.ping()
 
     @staticmethod
-    def _decode_json(json_value):
+    def _decode_json(json_value: str) -> Any:
         try:
             return json.loads(json_value)
         except TypeError:  # non-strings (e.g. None)
             return json_value
 
     @staticmethod
     def _convert_numeric(value):
         # We do not check if isinstance since bool is a subclass of int
-        if type(value) in {int, float, complex}:  # pylint: disable=unidiomatic-typecheck
+        if type(value) in {int, float, complex}:
             value = repr(value)
 
         return value
```

### Comparing `flashback-2.1.0/flashback/caching/cached.py` & `flashback-2.2.0/flashback/caching/cached.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,16 @@
-import inspect
+from collections.abc import Callable
 import functools
+import inspect
 import logging
 
 from .cache import Cache
 
 
-def cached(adapter="memory", **kwargs):
+def cached(adapter: str = "memory", **kwargs) -> Callable:
     """
     Caches the return of a callable under a type-aware key built with its arguments.
 
     Relies on the key building mechanism from `functools._make_key`.
 
     Examples:
         ```python
@@ -35,33 +36,33 @@
 
         func(1, 2)
         #=> Cache hit
         #=> 3
         ```
 
     Params:
-        adapter (str): the cache storage adapter to use
-        kwargs (dict): every keyword argument, forwarded to the cache adapter
+        adapter: the cache storage adapter to use
+        kwargs: every keyword argument, forwarded to the cache adapter
 
     Returns:
-        Callable: a wrapper used to decorate a callable
+        a wrapper used to decorate a callable
     """
     cache = Cache(adapter, **kwargs)
 
     def wrapper(func):
         # `.getmodule().__name__` returns the same value as `__name__` called from the module we
         # decorate.
         # Since `logging` is a singleton, everytime we call `logging.getLogger()` with the same
         # name, we receive the same logger, which "hides" this decorator as if the logging was
         # made from within the callable we decorate
         logger = logging.getLogger(inspect.getmodule(func).__name__)
 
         @functools.wraps(func)
         def inner(*args, **kwargs):
-            key = functools._make_key(args, kwargs, True)  # pylint: disable=protected-access
+            key = functools._make_key(args, kwargs, True)  # noqa: SLF001
             value = cache.get(key)
 
             if value is not None:
                 logger.debug("Cache hit")
 
                 return value
```

### Comparing `flashback-2.1.0/flashback/classproperty.py` & `flashback-2.2.0/flashback/classproperty.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,20 +1,24 @@
+from __future__ import annotations
+
+
 class ClassPropertyMetaclass(type):
     """
     Defines a metaclass to ensure the property is settable, to use as `flashback.classproperty.meta`.
     """
+
     def __setattr__(cls, key, value):
         obj = cls.__dict__.get(key, None)
         if isinstance(obj, classproperty):
             return obj.__set__(cls, value)
 
         return super().__setattr__(key, value)
 
 
-class classproperty:  # pylint: disable=invalid-name
+class classproperty:  # noqa: N801
     """
     Combines @classmethod and @property to define getters and setters on classes attributes.
 
     Any class that needs to use this @classproperty decorator must have classproperty.meta as
     metaclass to prevent attribute assignation via the class when no setter is defined.
 
     Adapted from https://stackoverflow.com/a/5191224.
@@ -46,27 +50,28 @@
 
         # Handles attribute assignation via the class
         Static.var = 3
         assert static_1.var == 3
         assert static_2.var == 3
         ```
     """
+
     meta = ClassPropertyMetaclass
 
     def __init__(self, func_get, func_set=None):
         """
         Params:
             func_get (Callable): the getter to decorate
             func_set (Callable): the setter to decorate
         """
-        if not isinstance(func_get, (classmethod, staticmethod)):
+        if not isinstance(func_get, (classmethod, staticmethod)):  # noqa: UP038
             func_get = classmethod(func_get)
 
         # Explicitly checks against None to avoid converting it to a classmethod
-        if func_set is not None and not isinstance(func_set, (classmethod, staticmethod)):
+        if func_set is not None and not isinstance(func_set, (classmethod, staticmethod)):  # noqa: UP038
             func_set = classmethod(func_set)
 
         self.func_get = func_get
         self.func_set = func_set
 
     def __get__(self, obj, cls=None):
         if cls is None:
@@ -82,13 +87,13 @@
         else:
             cls = obj
             obj = None
 
         return self.func_set.__get__(obj, cls)(value)
 
     def setter(self, func):
-        if not isinstance(func, (classmethod, staticmethod)):
+        if not isinstance(func, (classmethod, staticmethod)):  # noqa: UP038
             func = classmethod(func)
 
         self.func_set = func
 
         return self
```

### Comparing `flashback-2.1.0/flashback/debugging/caller.py` & `flashback-2.2.0/flashback/debugging/caller.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,21 +1,26 @@
+from __future__ import annotations
+
+from collections.abc import Callable
+from typing import TextIO
 import inspect
 import os
 import sys
 
 from .formatter import Formatter
-from .get_callable import get_callable
 from .get_call_context import get_call_context
+from .get_callable import get_callable
 from .get_frameinfo import get_frameinfo
 
 
 ANSI_DIM_START = "\x1b[2m"
 ANSI_DIM_END = "\x1b[0m"
 
-def caller(depth=2, context=5, output=sys.stderr):
+
+def caller(depth: int = 2, context: int = 5, output: TextIO = sys.stderr) -> Callable | None:
     """
     Prints debug information about the caller of the current callable being executed, and returns
     the caller object if found.
 
     Examples:
         ```python
         from flashback.debugging import caller
@@ -49,19 +54,20 @@
         #=> 12
         #=> 13 caller_instance = add(1, 2, 3)
 
         assert caller_instance == subtract
         ```
 
     Params:
-        depth (int): the depth to go back in the stack
-        context (int): the number of context lines around the call made to the callable to take
+        depth: the depth to go back in the stack
+        context: the number of context lines around the call made to the callable to take
+        output: where to write to
 
     Returns:
-        Callable|None: the callable calling if found
+        the callable calling if found
     """
     try:
         frameinfo = get_frameinfo(depth)
     except ValueError:
         print("Called by '__main__.<module>' (<unknown>:1):", file=output)
         print(f"{ANSI_DIM_START}No code context found{ANSI_DIM_END}", file=output)
 
@@ -72,15 +78,15 @@
 
     # Extract call context, with -context/+context lines of context at most
     call_context, call_context_lineno, call_boundaries = get_call_context(frameinfo, size=context)
 
     caller_instance = get_callable(frameinfo)
 
     module = inspect.getmodule(frameinfo.frame, _filename=filename)
-    module_name = module.__name__ if module else '__main__'
+    module_name = module.__name__ if module else "__main__"
     # From the found instance (if any), calls __qualname__. At worst, falls back to the frameinfo's
     # co_name. Having access to __qualname__ directly in the frame is in the works since 2011:
     # - https://bugs.python.org/issue12857
     # - https://bugs.python.org/issue13672
     function_name = caller_instance.__qualname__ if caller_instance else frameinfo.frame.f_code.co_name
 
     formatter = Formatter()
```

### Comparing `flashback-2.1.0/flashback/debugging/filters/call_highlight_filter.py` & `flashback-2.2.0/flashback/debugging/filters/call_highlight_filter.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,24 +1,30 @@
+from __future__ import annotations
+
+from collections.abc import Generator
+
 from pygments.filters import Filter
-from pygments.token import Name
+from pygments.token import Name, _TokenType
+from pygments.lexer import Lexer
 
 
 class CallHighlightFilter(Filter):
     """
     Modifies the token type of a Name to Name.Function if its value is followed by an opening
     parenthesis.
     """
-    def __init__(self, **kwargs):
+
+    def __init__(self, **kwargs) -> None:
         """
         Params:
             kwargs (dict): every additional keyword parameters
         """
         Filter.__init__(self, **kwargs)
 
-    def filter(self, lexer, stream):
+    def filter(self, _lexer: Lexer, stream: Generator) -> Generator[tuple[_TokenType, str], None, None]:
         """
         Iterates over the stream of tokens and searches for a name followed by an opening paren to
         change its type to Name.Function.
 
         Many colorscheme highlight calls, but pygments treats a function call as a simple Name,
         this filter fixes that.
 
@@ -26,19 +32,19 @@
         this filter takes the first item of the stream, stores it into a stack, and then iterates
         over the stream (now with an offset of 1), and makes a decision of token tx-1 based on its
         current token tx. Once the decision is made it adds back the token tx-1 and the token tx to
         the stack, and repeats the process. Once the stream is exhausted, it yields the content of
         the stack.
 
         Params:
-            lexer (pygments.lexer.Lexer): the lexer instance
-            stream (generator): the stream of couples tokentype-value
+            lexer: the lexer instance
+            stream: the stream of couples tokentype-value
 
         Yields:
-            tuple<pygments.token._TokenType, str>: the token type and token value
+            the token type and token value
         """
         try:
             stack = [next(stream)]
         except StopIteration:
             stack = []
 
         for ttype, value in stream:
```

### Comparing `flashback-2.1.0/flashback/debugging/filters/decorator_operator_filter.py` & `flashback-2.2.0/flashback/debugging/filters/decorator_operator_filter.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,37 +1,43 @@
+from __future__ import annotations
+
+from collections.abc import Generator
+
 from pygments.filters import Filter
-from pygments.token import Name, Operator
+from pygments.token import Name, Operator, _TokenType
+from pygments.lexer import Lexer
 
 
 class DecoratorOperatorFilter(Filter):
     """
     Extracts the '@' from a `pygments.token.Name.Decorator` to be a standalone
     `pygments.token.Operator`.
     """
+
     def __init__(self, **kwargs):
         """
         Params:
             kwargs (dict): every additional keyword parameters
         """
         Filter.__init__(self, **kwargs)
 
-    def filter(self, lexer, stream):
+    def filter(self, _lexer: Lexer, stream: Generator) -> Generator[tuple[_TokenType, str], None, None]:
         """
         Iterates over the stream of tokens and splits a `pygments.token.Name.Decorator: into two
         components.
 
         Some colorschemes handle the '@' as an operator, and the name of the decorator as a name,
         but pygments treat the whole thing as a decorator. This filter fixes this behaviour.
 
         Params:
-            lexer (pygments.lexer.Lexer): the lexer instance
-            stream (generator): the stream of couples tokentype-value
+            lexer: the lexer instance
+            stream: the stream of couples tokentype-value
 
         Yields:
-            tuple<pygments.token._TokenType, str>: the token type and token value
+            the token type and token value
         """
         for ttype, value in stream:
             if ttype is Name.Decorator:
-                yield Operator, '@'
+                yield Operator, "@"
                 yield Name.Decorator, value[1:]
             else:
                 yield ttype, value
```

### Comparing `flashback-2.1.0/flashback/debugging/filters/type_highlight_filter.py` & `flashback-2.2.0/flashback/debugging/filters/type_highlight_filter.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,35 +1,41 @@
+from __future__ import annotations
+
+from collections.abc import Generator
+
+from pygments.lexer import Lexer
 from pygments.filters import Filter
-from pygments.token import Name, Keyword
+from pygments.token import Name, Keyword, _TokenType
 
 
 class TypeHighlightFilter(Filter):
     """
     Modifies the token type of a Name token to Keyword.Type if its value appears in a list of values.
     """
-    def __init__(self, names, **kwargs):
+
+    def __init__(self, names: list[str], **kwargs) -> None:
         """
         Params:
-            names (Iterable<str>): the list of names to change the token type
-            kwargs (dict): every additional keyword parameters
+            names: the list of names to change the token type
+            kwargs: every additional keyword parameters
         """
         Filter.__init__(self, **kwargs)
 
         self.names = set(names)
 
-    def filter(self, lexer, stream):
+    def filter(self, _lexer: Lexer, stream: Generator) -> Generator[tuple[_TokenType, str], None, None]:
         """
         Iterates over the stream of tokens and modifies a token's type if its value appears in a
         list of names.
 
         Params:
-            lexer (pygments.lexer.Lexer): the lexer instance
-            stream (generator): the stream of couples tokentype-value
+            lexer: the lexer instance
+            stream: the stream of couples tokentype-value
 
         Yields:
-            tuple<pygments.token._TokenType, str>: the token type and token value
+            the token type and token value
         """
         for ttype, value in stream:
             if ttype in Name and value in self.names:
                 yield Keyword.Type, value
             else:
                 yield ttype, value
```

### Comparing `flashback-2.1.0/flashback/debugging/formatter.py` & `flashback-2.2.0/flashback/debugging/formatter.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,18 +1,26 @@
+from __future__ import annotations
+
+from collections import Counter, defaultdict, OrderedDict, deque
+from collections.abc import Sized, Iterable, Generator, Mapping
 from io import StringIO
-import inspect
 from textwrap import wrap
+from types import ModuleType, MethodType, FunctionType
+from typing import Any, ClassVar, TypeVar
+import inspect
 
 import pygments
 from pygments.formatters.terminal256 import Terminal256Formatter
 from pygments.lexers.python import PythonLexer
 
 from .filters import CallHighlightFilter, DecoratorOperatorFilter, TypeHighlightFilter
 from .styles import Jellybeans
 
+T = TypeVar("T")
+
 
 class Formatter:
     """
     Implements a formatter to prettify arguments received by `flashback.debugging.xp` and parsed
     by `flashback.debugging.parser`.
 
     Currently has special formatting for the following types:
@@ -22,39 +30,40 @@
         - module
         - type / ABCMeta
         - function / method
         - Generator
 
     Formats all other types via their __repr__ method.
     """
-    TYPE_TO_SYMBOLS = {
+
+    TYPE_TO_SYMBOLS: ClassVar[dict[str, tuple[str, str]]] = {
         "deque": ("deque([\n", "])"),
         "frozenset": ("frozenset({\n", "})"),
         "list": ("[\n", "]"),
         "set": ("{\n", "}"),
         "tuple": ("(\n", ")"),
         "Counter": ("Counter({\n", "})"),
         "defaultdict": ("defaultdict(_TYPE_, {\n", "})"),
         "dict": ("{\n", "}"),
         "OrderedDict": ("OrderedDict({\n", "})"),
     }
     DIM_START = "\033[2m"
     DIM_END = "\033[0m"
 
-    def __init__(self, indent_str="    "):
+    def __init__(self, indent_str: str = "    ") -> None:
         """
         Params:
             indent_str (str): the indentation string to use
         """
         self._indent_str = indent_str
         self._indent_str_len = len(indent_str)
 
-        self._width = None
+        self._width = 0
 
-        self._buffer = None
+        self._buffer = StringIO()
 
         self._code_lexer = PythonLexer(
             ensurenl=False,
             filters=[
                 DecoratorOperatorFilter(),
                 CallHighlightFilter(),
                 TypeHighlightFilter(
@@ -69,45 +78,52 @@
                         "list",
                         "object",
                         "set",
                         "str",
                         "tuple",
                     ],
                 ),
-            ]
+            ],
         )
         self._code_formatter = Terminal256Formatter(style=Jellybeans)
 
-    def format(self, filename, lineno, arguments, warning, width=120):
+    def format(  # noqa: PLR0913
+        self,
+        filename: str,
+        lineno: int,
+        arguments: list[tuple[str, T]],
+        warning: str | None,
+        width: int = 120,
+    ) -> str:
         """
         Formats the output of `Parser.parse` following the given style and width.
 
         Params:
-            filename (str): the filename from where `flashback.debugging.xp` has been called
-            lineno (int): the line number from where `flashback.debugging.xp` has been called
-            arguments (list<tuple>): the arguments to format, as name-value couples
-            warning (str): the error encountered when parsing the code or None
-            width (int): the maximum width before wrapping the output
+            filename: the filename from where `flashback.debugging.xp` has been called
+            lineno: the line number from where `flashback.debugging.xp` has been called
+            arguments: the arguments to format, as name-value couples
+            warning: the error encountered when parsing the code or None
+            width: the maximum width before wrapping the output
 
         Returns:
-            str: the formatted arguments, and location of the call to `flashback.debugging.xp`
+            the formatted arguments, and location of the call to `flashback.debugging.xp`
         """
         self._width = width
 
         # We need to use ANSI color coding because pygments can only highlight code
         content = f"\033[2m{filename}:{lineno}"
         if warning:
             content += f" ({warning})"
         content += "\033[0m\n"
 
         if len(arguments) == 0:
             return content[:-1]  # Remove the last newline
 
         arguments_content = []
-        for (name, value) in arguments:
+        for name, value in arguments:
             argument_content = f"  {name}:\n" if name is not None else ""
 
             # self._format is called recursively, so we use a stream
             # to progressively write the formatting without passing it around
             self._buffer = StringIO()
 
             self._format(value)
@@ -119,26 +135,26 @@
 
             arguments_content.append(argument_content)
 
         content += "\n".join(arguments_content)
 
         return content
 
-    def format_code(self, lines, start_lineno=1, highlight=None):
+    def format_code(self, lines: Sized, start_lineno: int = 1, highlight: tuple[int, int] | None = None) -> str:
         """
         Formats code with syntax highlighting and line numbers, with optional highlighting of
         specific range of lines.
 
         Params:
-            lines (Iterable<str>): the lines of code to render
-            start_lineno (int): the line number of the code's first line
-            highlight (tuple<int>): the start and end indices of the code to highlight
+            lines: the lines of code to render
+            start_lineno: the line number of the code's first line
+            highlight: the start and end indices of the code to highlight
 
         Returns:
-            str: the formatted and highlighted code
+            the formatted and highlighted code
         """
         linenos = list(range(start_lineno, start_lineno + len(lines) + 2))
 
         pad_len = len(str(max(linenos)))
         lines_with_linenos = []
         for lineno, line in zip(linenos, lines):
             lines_with_linenos.append(f"{lineno:{pad_len}} {line}")
@@ -160,36 +176,36 @@
             highlighted_lines.append(self._highlight("".join(lines_with_linenos[end:])))
             highlighted_lines.append(self.DIM_END)
 
             return "".join(highlighted_lines)
 
         return self._highlight("".join(lines_with_linenos))
 
-    def _format(self, value, current_indent=1, force_indent=True):
+    def _format(self, value: T, current_indent: int = 1, force_indent: bool = True) -> None:
         if force_indent:
             self._buffer.write(current_indent * self._indent_str)
 
         next_indent = current_indent + 1
 
         try:
             # Converts classes such as OrderedDict, Counter, etc.
             class_name = value.__class__.__name__
 
             method = getattr(self, f"_format_{class_name}")
             method(value, current_indent, next_indent)
         except AttributeError:
             self._format_raw(value, current_indent, next_indent)
 
-    def _format_ABCMeta(self, meta, _current_indent, _next_indent):  # pylint: disable=invalid-name
+    def _format_ABCMeta(self, meta, _current_indent: int, _next_indent: int) -> None:  # noqa: N802
         self._format_type(meta, _current_indent, _next_indent)
 
-    def _format_type(self, cls, _current_indent, _next_indent):
+    def _format_type(self, cls: type, _current_indent: int, _next_indent: int) -> None:
         self._buffer.write(" < ".join([x.__qualname__ for x in cls.__mro__]))
 
-    def _format_module(self, module, current_indent, next_indent):
+    def _format_module(self, module: ModuleType, current_indent: int, next_indent: int) -> None:
         prefix = current_indent * self._indent_str
         nested_prefix = next_indent * self._indent_str
         suffix = "\n"
 
         self._buffer.write("Name:\n")
         self._buffer.write(nested_prefix + module.__name__ + suffix)
         self._buffer.write(prefix + "Location:\n")
@@ -197,34 +213,34 @@
         self._buffer.write(prefix + "Contents:\n")
         nested_prefix += "- "
         for key, value in module.__dict__.items():
             if not key.startswith("_"):
                 content = f"{key} ({value.__class__.__name__})"
                 self._buffer.write(nested_prefix + content + suffix)
 
-    def _format_method(self, method, _current_indent, _next_indent):
+    def _format_method(self, method: MethodType, _current_indent: int, _next_indent: int) -> None:
         self._format_function(method, _current_indent, _next_indent)
 
-    def _format_function(self, function, _current_indent, _next_indent):
+    def _format_function(self, function: MethodType | FunctionType, _current_indent: int, _next_indent: int) -> None:
         self._buffer.write(function.__qualname__)
         self._buffer.write(str(inspect.signature(function)))
 
-    def _format_Counter(self, counter, current_indent, next_indent):  # pylint: disable=invalid-name
+    def _format_Counter(self, counter: Counter, current_indent: int, next_indent: int) -> None:  # noqa: N802
         self._format_mapping(counter, current_indent, next_indent)
 
-    def _format_defaultdict(self, default_dict, current_indent, next_indent):
+    def _format_defaultdict(self, default_dict: defaultdict, current_indent: int, next_indent: int) -> None:
         self._format_mapping(default_dict, current_indent, next_indent)
 
-    def _format_OrderedDict(self, ordered_dict, current_indent, next_indent):  # pylint: disable=invalid-name
+    def _format_OrderedDict(self, ordered_dict: OrderedDict, current_indent: int, next_indent: int) -> None:  # noqa: N802
         self._format_mapping(ordered_dict, current_indent, next_indent)
 
-    def _format_dict(self, dictionary, current_indent, next_indent):
+    def _format_dict(self, dictionary: dict, current_indent: int, next_indent: int) -> None:
         self._format_mapping(dictionary, current_indent, next_indent)
 
-    def _format_mapping(self, mapping, current_indent, next_indent):
+    def _format_mapping(self, mapping: Mapping, current_indent: int, next_indent: int) -> None:
         prefix = next_indent * self._indent_str
         separator = ": "
         suffix = ",\n"
         start, end = self.TYPE_TO_SYMBOLS[mapping.__class__.__name__]
 
         # We're be processing a defaultdict
         if "_TYPE_" in start:
@@ -235,43 +251,43 @@
             self._buffer.write(prefix)
             self._format(key, next_indent, False)
             self._buffer.write(separator)
             self._format(value, next_indent, False)
             self._buffer.write(suffix)
         self._buffer.write(current_indent * self._indent_str + end)
 
-    def _format_list(self, iterable, current_indent, next_indent):
+    def _format_list(self, iterable: list, current_indent: int, next_indent: int) -> None:
         self._format_iterables(iterable, current_indent, next_indent)
 
-    def _format_set(self, iterable, current_indent, next_indent):
+    def _format_set(self, iterable: set, current_indent: int, next_indent: int) -> None:
         self._format_iterables(iterable, current_indent, next_indent)
 
-    def _format_frozenset(self, iterable, current_indent, next_indent):
+    def _format_frozenset(self, iterable: frozenset, current_indent: int, next_indent: int) -> None:
         self._format_iterables(iterable, current_indent, next_indent)
 
-    def _format_tuple(self, iterable, current_indent, next_indent):
+    def _format_tuple(self, iterable: tuple, current_indent: int, next_indent: int) -> None:
         self._format_iterables(iterable, current_indent, next_indent)
 
-    def _format_deque(self, iterable, current_indent, next_indent):
+    def _format_deque(self, iterable: deque, current_indent: int, next_indent: int) -> None:
         self._format_iterables(iterable, current_indent, next_indent)
 
-    def _format_iterables(self, iterable, current_indent, next_indent):
+    def _format_iterables(self, iterable: Iterable, current_indent: int, next_indent: int) -> None:
         suffix = ",\n"
         start, end = self.TYPE_TO_SYMBOLS[iterable.__class__.__name__]
 
         self._buffer.write(start)
         for value in iterable:
             self._format(value, next_indent, True)
             self._buffer.write(suffix)
         self._buffer.write(current_indent * self._indent_str + end)
 
-    def _format_bytes(self, string, current_indent, next_indent):
+    def _format_bytes(self, string: bytes, current_indent: int, next_indent: int) -> None:
         self._format_str(string, current_indent, next_indent)
 
-    def _format_str(self, string, current_indent, next_indent):
+    def _format_str(self, string: bytes | str, current_indent: int, next_indent: int) -> None:
         # We substract 3 to take in account the quotes and the newline
         width = self._width - (next_indent * self._indent_str_len) - 3
 
         if len(string) <= width:
             self._buffer.write(repr(string))
         else:
             start = "(\n"
@@ -289,26 +305,26 @@
                 lines.append(line[begin:])
 
             self._buffer.write(start)
             for line in lines:
                 self._buffer.write(prefix + repr(line) + suffix)
             self._buffer.write(current_indent * self._indent_str + end)
 
-    def _format_generator(self, generator, current_indent, next_indent):
+    def _format_generator(self, generator: Generator, current_indent: int, next_indent: int) -> None:
         start = "(\n"
         suffix = ",\n"
         end = ")"
 
         self._buffer.write(start)
         for item in generator:
             self._format(item, next_indent, True)
             self._buffer.write(suffix)
         self._buffer.write(current_indent * self._indent_str + end)
 
-    def _format_raw(self, value, current_indent, next_indent):
+    def _format_raw(self, value: Any, current_indent: int, next_indent: int) -> None:
         representation = repr(value)
         lines = representation.splitlines(True)
 
         if len(lines) > 1 or (len(representation) + (current_indent * self._indent_str_len)) >= self._width:
             start = "(\n"
             prefix = next_indent * self._indent_str
             suffix = "\n"
@@ -320,9 +336,9 @@
                 sub_lines = wrap(line, wrap_at)
                 for sub_line in sub_lines:
                     self._buffer.write(prefix + sub_line + suffix)
             self._buffer.write(current_indent * self._indent_str + end)
         else:
             self._buffer.write(representation)
 
-    def _highlight(self, value):
+    def _highlight(self, value: str) -> str:
         return pygments.highlight(value, lexer=self._code_lexer, formatter=self._code_formatter)
```

### Comparing `flashback-2.1.0/flashback/debugging/get_call_context.py` & `flashback-2.2.0/flashback/debugging/get_call_context.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,18 @@
+from __future__ import annotations
+
 import ast
 import inspect
 from textwrap import dedent
 
 
-def get_call_context(frameinfo, size=5):
+def get_call_context(
+    frameinfo: inspect.FrameInfo,
+    size: int = 5,
+) -> tuple[list[str], int | None, tuple[int, int] | tuple[()]]:
     """
     Extracts the context surrounding the call statement of the given `frameinfo`, and returns its
     code, its first line number, and the boundaries of the call statement.
 
     Returns empty results if the frame has no code_context, or if the call is not found in the
     source file.
 
@@ -34,21 +39,21 @@
             "\n",
         ]
         assert context_line == 1
         assert call_boundaries == (3, 4)
         ```
 
     Params:
-        frameinfo (inspect.FrameInfo): the frameinfo to extract the context from
-        size (int): the number of lines surrounding the call statement to take as context
+        frameinfo: the frameinfo to extract the context from
+        size: the number of lines surrounding the call statement to take as context
 
     Returns:
-        list<str>: the context extracted with at most `size` context lines before and after
-        int|None: the line number of the context's first line
-        typle<int>: the start and end of the call statement, as indices of the returned context
+        the context extracted with at most `size` context lines before and after
+        the line number of the context's first line
+        the start and end of the call statement, as indices of the returned context
     """
     if not frameinfo.code_context:
         return [], None, ()
 
     try:
         source, _ = inspect.findsource(frameinfo.frame)
     except OSError:
@@ -62,15 +67,15 @@
     lineno = frameinfo.lineno
     index_start = lineno - 1
 
     for index_end in range(index_start + 1, len(source) + 1):
         call_line = dedent("".join(source[index_start:index_end]))
 
         try:
-            ast.parse(call_line, filename=frameinfo.filename).body[0].value  # pylint: disable=expression-not-assigned
+            ast.parse(call_line, filename=frameinfo.filename).body[0].value  # noqa: B018
 
             break
         except (SyntaxError, AttributeError):
             pass
 
     call_statement_len = call_line.count("\n")
```

### Comparing `flashback-2.1.0/flashback/debugging/get_callable.py` & `flashback-2.2.0/flashback/debugging/get_callable.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,14 @@
-def get_callable(frameinfo):
+from __future__ import annotations
+
+from collections.abc import Callable
+from inspect import FrameInfo
+
+
+def get_callable(frameinfo: FrameInfo) -> Callable | None:
     """
     Finds the callable being executed during the given `frameinfo`.
 
     Starts by using the co_name found in the frame, then looks for a 'self' or 'cls' in the
     locals (in this case, callable is a method). If no class object or instance exists, looks
     into the frameinfo's globals (in that case, callable is just a function).
 
@@ -38,18 +44,18 @@
 
         frameinfo = DummyClass.dummy_classmethod()
 
         assert get_callable(frameinfo) == DummyClass.dummy_classmethod
         ```
 
     Params:
-        frameinfo (inspect.FrameInfo): the frameinfo to extract the callable from
+        frameinfo: the frameinfo to extract the callable from
 
     Returns:
-        Callable|None: the callable instance if found
+        the callable instance if found
     """
     frame = frameinfo.frame
 
     function_name = frame.f_code.co_name
 
     caller_class = frame.f_locals.get("self", None)
     if caller_class is None:
```

### Comparing `flashback-2.1.0/flashback/debugging/get_frameinfo.py` & `flashback-2.2.0/flashback/debugging/get_frameinfo.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import inspect
 
-def get_frameinfo(depth=0, context=1):
+
+def get_frameinfo(depth: int = 0, context: int = 1) -> inspect.FrameInfo:
     """
     Finds the frame at `depth` and builds a `inspect.FrameInfo` from it.
 
     Executes 10 times faster than `inspect.stack()[depth]` if depth is superior to 1, else only 2
     times.
 
     Handles negative `depth` by returning the current frame from the caller's perspective, just
@@ -21,19 +22,19 @@
             return get_frameinfo()
 
         frameinfo = dummy_func()
         assert frameinfo.function == "dummy_func"
         ```
 
     Params:
-        depth (int): the depth at which to find the frame
-        context (int): the number of lines surrounding the frame to use in the traceback
+        depth: the depth at which to find the frame
+        context: the number of lines surrounding the frame to use in the traceback
 
     Returns:
-        inspect.FrameInfo: the FrameInfo object for the frame
+        the FrameInfo object for the frame
 
     Raises:
         ValueError: if `depth` is greater than the length of the call stack
     """
     # Could use `sys._getframe(1)` but safer to go through its wrapper
     frame = inspect.currentframe()
     # Skips the actual current frame (the execution of get_frame())
@@ -43,9 +44,9 @@
             raise ValueError("call stack is not deep enough")
 
         frame = frame.f_back
 
     if frame is None:
         raise ValueError("call stack is not deep enough")
 
-    frameinfo = (frame,) + inspect.getframeinfo(frame, context)
+    frameinfo = (frame,) + inspect.getframeinfo(frame, context)  # noqa: RUF005
     return inspect.FrameInfo(*frameinfo)
```

### Comparing `flashback-2.1.0/flashback/debugging/parser.py` & `flashback-2.2.0/flashback/debugging/parser.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,103 +1,119 @@
+from __future__ import annotations
+
+from collections.abc import Sequence
+from textwrap import dedent
+from typing import TypeVar
 import ast
+import inspect
 import os
-from textwrap import dedent
 
 import regex
 
 from .get_call_context import get_call_context
 from .get_frameinfo import get_frameinfo
 
+T = TypeVar("T")
+
 
 class Parser:
     """
     Implements a parser to extract the code context from which `flashback.debugging.xp` is called.
 
     First, goes back in the call stack to locate the call made to `flashback.debugging.xp`,
     then extracts the complete statement (handling multi-lines calls),
     and finds out the name and representation of the given arguments based on the identified snippet.
 
     If needed, flattens the multi-line parameters to use them as argument names, using
     `CRE_OPENING_BRACKET` and `CRE_CLOSING_BRACKET`.
     """
+
     COMPLEX_NODES = (
         ast.Attribute,
         ast.BoolOp,
         ast.BinOp,
         ast.Call,
         ast.Compare,
         ast.DictComp,
         ast.GeneratorExp,
         ast.IfExp,
         ast.ListComp,
         ast.Subscript,
-        ast.SetComp
+        ast.SetComp,
     )
     CRE_OPENING_BRACKET = regex.compile(r"(\{|\[|\()\s")
     CRE_CLOSING_BRACKET = regex.compile(r"\s(\}|\]|\))")
 
-    def __init__(self, _offset=2):
+    def __init__(self, _offset: int = 2) -> None:
         # This is useful for tests or direct call to `Parser.parse` (in that case use 1)
         self._offset = _offset
 
-    def parse(self, *arguments):
+    def parse(self, *arguments: T) -> tuple[str, int, Sequence[tuple[str | None, T]], str | None]:
         """
         Parses the arguments received from the code context in which `flashback.debugging.xp` has
         been called, and enriches the arguments values with their names (or representation).
 
         We must accept all arguments in a greedy way to emulate the behavior of
         `flashback.debugging.xp`, as we call directly this method when testing.
 
         Params:
-            arguments (tuple<Any>): every positional arguments
+            arguments: every positional arguments
 
         Returns:
-            str: the filename from where `flashback.debugging.xp` has been called
-            int: the line number from where `flashback.debugging.xp` has been called
-            list<tuple>: the arguments parsed, as name-value couples
-            str: the error encountered when parsing the code or None
+            the filename from where `flashback.debugging.xp` has been called
+            the line number from where `flashback.debugging.xp` has been called
+            the arguments parsed, as name-value couples
+            the error encountered when parsing the code or None
         """
         try:
             # We access [2] because an end-user call to xp() calls this code (thus, two layers of calls)
             # If this code would have been called directly by the end-user, we would need to access [1]
             frameinfo = get_frameinfo(self._offset)
 
             filename = os.path.relpath(frameinfo.filename)
             lineno = frameinfo.lineno
 
             node, code, warning = self._parse_call(frameinfo, filename)
             if node and code:
                 parsed_arguments = self._parse_arguments(node, code, arguments)
             else:  # parsing failed
                 parsed_arguments = self._default_arguments_parsing(arguments)
-        except Exception as e:  # pylint: disable=broad-except
+        except Exception as e:  # noqa: BLE001
             filename = "<unknown>"
             lineno = 0
             parsed_arguments = self._default_arguments_parsing(arguments)
             warning = f"error parsing code, {e} ({e.__class__.__name__})"
 
         return filename, lineno, parsed_arguments, warning
 
     @staticmethod
-    def _parse_call(frameinfo, filename):
+    def _parse_call(
+        frameinfo: inspect.FrameInfo,
+        filename: str,
+    ) -> tuple[ast.Call | None, list[str] | None, str | None]:
         context, _, boundaries = get_call_context(frameinfo)
         if not context:
             return None, None, "error parsing code, no code context found"
 
         call_statement = dedent("".join(context[slice(*boundaries)]))
 
         node = ast.parse(call_statement, filename=filename).body[0].value
         if not isinstance(node, ast.Call):
             return None, None, f"error parsing code, found ast.{node.__class__.__name__} instead of ast.Call"
 
         call_statement_lines = [line for line in call_statement.split("\n") if line]
 
         return node, call_statement_lines, None
 
-    def _parse_arguments(self, call_node, code_lines, arguments):  # pylint: disable=too-many-locals
+    def _parse_arguments(
+        self,
+        call_node: ast.Call,
+        code_lines: Sequence[str],
+        arguments: tuple[T, ...],
+    ) -> Sequence[tuple[str | None, T]]:
         parsed_arguments = []
 
         arguments_positions = self._get_arguments_positions(call_node, code_lines)
         for i, argument in enumerate(arguments):
             try:
                 arg_node = call_node.args[i]
             except IndexError:
@@ -125,65 +141,40 @@
                 parsed_arguments.append((argument_name, argument))
             else:
                 parsed_arguments.append((None, argument))
 
         return parsed_arguments
 
     @staticmethod
-    def _get_arguments_positions(call_node, code_lines):
-        # This whole method exist only because before python 3.8.0, the
-        # end_lineno and end_col_offset attribute are not given for all ast nodes (https://bugs.python.org/issue33416),
-        # so finding the position of a given argument is dependent on the following ones.
-        # Since 3.8.0, it's as simple as:
-        #     start_line = arg_node.lineno - 1
-        #     start_col = arg_node.col_offset
-        #     end_line = arg_node.end_lineno - 1
-        #     end_col = arg_node.end_col_offset
+    def _get_arguments_positions(call_node: ast.Call, code_lines: Sequence[str]) -> list[dict[str, int]]:
         arguments_positions = []
 
-        default_end_line = len(code_lines) - 1
-        default_end_col = -1
-        for i, arg_node in enumerate(call_node.args):
-            positions = {
-                "start_line": arg_node.lineno - 1,
-                "start_col": arg_node.col_offset,
-                "end_line": default_end_line,
-                "end_col": default_end_col
-            }
-            if isinstance(arg_node, (ast.ListComp, ast.GeneratorExp)):
-                positions["start_col"] -= 1
-
-            if i > 0:
-                arguments_positions[-1]["end_line"] = positions["start_line"]
-
-                # Handles cases where there is no space after the comma
-                try:
-                    comma_index = code_lines[positions["start_line"]][:positions["start_col"]].rindex(",")
-                    separator_len = positions["start_col"] - comma_index
-                except ValueError:
-                    # No comma found on this line, meaning we're multiline: ",\r"
-                    separator_len = 2
-
-                arguments_positions[-1]["end_col"] = positions["start_col"] - separator_len
-
-            arguments_positions.append(positions)
+        for arg_node in call_node.args:
+            arguments_positions.append(  # noqa: PERF401
+                {
+                    "start_line": arg_node.lineno - 1,
+                    "start_col": arg_node.col_offset,
+                    "end_line": (arg_node.end_lineno or arg_node.lineno) - 1,
+                    "end_col": arg_node.end_col_offset or arg_node.col_offset,
+                },
+            )
 
         if arguments_positions and call_node.keywords:
             kwarg_node = call_node.keywords[0]
 
             arguments_positions[-1]["end_line"] = kwarg_node.value.lineno - 1
 
             # Handles cases where there is no space after the comma
             try:
-                comma_index = code_lines[kwarg_node.value.lineno - 1][:kwarg_node.value.col_offset].rindex(",")
+                comma_index = code_lines[kwarg_node.value.lineno - 1][: kwarg_node.value.col_offset].rindex(",")
                 separator_len = kwarg_node.value.col_offset - comma_index
             except ValueError:
                 # No comma found on this line, meaning we're multiline: ",\r"
                 separator_len = kwarg_node.value.col_offset - 2
 
             arguments_positions[-1]["end_col"] = kwarg_node.value.col_offset - separator_len
 
         return arguments_positions
 
     @staticmethod
-    def _default_arguments_parsing(arguments):
+    def _default_arguments_parsing(arguments: tuple[T, ...]) -> Sequence[tuple[None, T]]:
         return [(None, argument) for argument in arguments]
```

### Comparing `flashback-2.1.0/flashback/debugging/profiled.py` & `flashback-2.2.0/flashback/debugging/profiled.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,12 +1,16 @@
+from __future__ import annotations
+
+from collections.abc import Callable
+from typing import Any, TextIO
 import cProfile
 import functools
 
 
-def profiled(output=None):
+def profiled(output: TextIO | None = None) -> Callable:
     """
     Profiles a call made to a callable and dump the stats to a file for further analysis.
 
     By default, prints the stats to a file called f"{func.__name__}.pstats", located in the folder
     from where it has been called.
 
     To visualize the stats collected during profiling, you can use:
@@ -52,20 +56,22 @@
 
     Params:
         output (str): the output to write the stats to
 
     Returns:
         Callable: a wrapper used to decorate a callable
     """
-    def wrapper(func):
+
+    def wrapper(func: Callable) -> Callable:
         @functools.wraps(func)
-        def inner(*args, **kwargs):
+        def inner(*args, **kwargs) -> Any:
             profiler = cProfile.Profile()
 
             result = profiler.runcall(func, *args, **kwargs)
 
             profiler.dump_stats(output or f"{func.__name__}.pstats")
 
             return result
 
         return inner
+
     return wrapper
```

### Comparing `flashback-2.1.0/flashback/debugging/styles/jellybeans.py` & `flashback-2.2.0/flashback/debugging/styles/jellybeans.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,84 +1,91 @@
+from __future__ import annotations
+
+from typing import ClassVar
+
 from pygments.style import Style
-from pygments.token import Comment, Generic, Keyword, Name, Number, \
-                           Operator, Punctuation, Literal, String, Token
+from pygments.token import (
+    Comment,
+    Generic,
+    Keyword,
+    Name,
+    Number,
+    Operator,
+    Punctuation,
+    Literal,
+    String,
+    Token,
+    _TokenType,
+)
 
 
 class Jellybeans(Style):
     """
     Implements the jellybeans.vim colorscheme for pygments.
 
     Inspired by:
 
     - https://github.com/cstrahan/pygments-styles/blob/master/themes/jellybeans.py
     """
+
     background_color = "#151515"
 
-    styles = {
+    styles: ClassVar[dict[_TokenType, str]] = {
         Comment: "#888888",
         Comment.Hashbang: "",
         Comment.Multiline: "",
         Comment.Preproc: "#8fbfdc",
         Comment.Single: "",
         Comment.Special: "",
-
         Generic.Deleted: "#220000 bg:#220000",
         Generic.Error: "bg:#902020",
         Generic.Heading: "#70b950 bold",
         Generic.Inserted: "bg:#032218",
         Generic.Output: "#808080 bg:#151515",
         Generic.Subheading: "#70b950 bold",
         Generic.Traceback: "bg:#902020",
-
         Keyword: "#8197bf",
         Keyword.Constant: "#cf6a4c",
         Keyword.Namespace: "#8fbfdc",
         Keyword.Type: "#8fbfdc",
-
         Name.Attribute: "#fad07a",
         Name.Builtin.Pseudo: "#c6b6ee",
         Name.Builtin: "#fad07a",
         Name.Class: "#fad07a",
         Name.Constant: "#cf6a4c",
         Name.Decorator: "#fad07a",
         Name.Entity: "#799d6a",
         Name.Exception: "#8fbfdc",
         Name.Function: "#fad07a",
         Name.Label: "#ffb964",
         Name.Namespace: "",
         Name.Other: "",
         Name.Tag: "#8197bf",
         Name.Variable: "",
-
         Number: "#cf6a4c",
         Number.Bin: "",
         Number.Float: "",
         Number.Hex: "",
         Number.Integer.Long: "",
         Number.Integer: "",
         Number.Oct: "",
-
         Operator: "#8197bf",
         Operator.Word: "",
-
         Punctuation: "",
-
         Literal: "",
         Literal.Date: "",
-
         String: "#99ad6a",
         String.Affix: "",
         String.Backtick: "",
         String.Char: "",
         String.Delimiter: "",
         String.Doc: "",
         String.Double: "",
         String.Escape: "",
         String.Heredoc: "",
         String.Interpol: "",
         String.Other: "",
         String.Regex: "",
         String.Single: "",
         String.Symbol: "",
-
         Token: "#e8e8d3",
     }
```

### Comparing `flashback-2.1.0/flashback/debugging/xp.py` & `flashback-2.2.0/flashback/debugging/xp.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,17 +1,21 @@
+from __future__ import annotations
+
+from typing import Any, TextIO
 import sys
 
 from .parser import Parser
 from .formatter import Formatter
 
 
 PARSER = Parser()
 FORMATTER = Formatter()
 
-def xp(*arguments, o=sys.stderr, f=True, w=120):  # pylint: disable=invalid-name
+
+def xp(*arguments: tuple[Any, ...], o: TextIO = sys.stderr, f: bool = True, w: int = 120) -> tuple[Any, ...] | None:
     """
     Provides a simple and concise way of printing for debugging purposes.
 
     Returns the arguments received, to allow chaining of calls, and inline debugging statements.
 
     Consumes generators to print them (be careful with infinite ones!).
 
@@ -61,21 +65,21 @@
         #=>     2 (int)
 
         assert result == 2
         #=> True
         ```
 
     Params:
-        arguments (tuple<Any>): every positional arguments
-        o (TextIO): the target output of print
-        f (bool): whether of not the output is flushed
-        w (int): the maximum width before wrapping the output
+        arguments: every positional arguments
+        o: the target output of print
+        f: whether of not the output is flushed
+        w: the maximum width before wrapping the output
 
     Returns:
-        Any:
+        the arguments or their results
     """
     filename, lineno, parsed_arguments, warning = PARSER.parse(*arguments)
     output = FORMATTER.format(filename, lineno, parsed_arguments, warning, width=w)
 
     print(output, file=o, flush=f)
 
     # Forwards the arguments received to the (possible) next operation
```

### Comparing `flashback-2.1.0/flashback/deprecated.py` & `flashback-2.2.0/flashback/deprecated.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,12 +1,15 @@
+from __future__ import annotations
+
+from collections.abc import Callable
 import functools
 import warnings
 
 
-def deprecated(since=None, until=None, reason=None):
+def deprecated(since: str | None = None, until: str | None = None, reason: str | None = None) -> Callable:
     """
     Warns when a deprecated callable is used.
 
     Examples:
         ```python
         from flashback import deprecated
 
@@ -22,21 +25,22 @@
             pass
 
         func()
         #=> func is deprecated since v2 and will be removed in v3 because it has moved.
         ```
 
     Params:
-        since (str): the date/version the callable was deprecated
-        until (str): the date/version the callable will be removed
-        reason (str): the reason of the deprecation
+        since: the date/version the callable was deprecated
+        until: the date/version the callable will be removed
+        reason: the reason of the deprecation
 
     Returns:
-        Callable: a wrapper used to decorate a callable
+        a wrapper used to decorate a callable
     """
+
     def wrapper(func):
         message = f"{func.__name__} is deprecated"
         if since:
             message += f" since {since}"
         if until:
             message += f" and will be removed in {until}"
         if reason:
```

### Comparing `flashback-2.1.0/flashback/encrypted_file.py` & `flashback-2.2.0/flashback/encrypted_file.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,7 +1,10 @@
+from __future__ import annotations
+
+from collections.abc import Callable
 import base64
 import os
 import secrets
 
 from cryptography.hazmat.primitives.ciphers import Cipher, algorithms, modes
 
 
@@ -36,35 +39,36 @@
         import pickle
         value = ""
         encrypted_file.write(value, serializer=pickle.dumps)
         assert encrypted_file.read(deserializer=pickle.loads) == value
         ```
 
     Params:
-        file_path (str): the path the file to encrypt
-        key_path (str): the path of the key used to encrypt the file
-        env_key_name (str): the name of the env var from which to fetch the encryption key (default: "ENCRYPTION_KEY")
+        file_path: the path the file to encrypt
+        key_path: the path of the key used to encrypt the file
+        env_key_name: the name of the env var from which to fetch the encryption key (default: "ENCRYPTION_KEY")
     """
+
     DEFAULT_ENV_KEY_NAME = "ENCRYPTION_KEY"
 
-    def __init__(self, file_path, key_path, env_key_name = DEFAULT_ENV_KEY_NAME):
+    def __init__(self, file_path: str, key_path: str, env_key_name: str = DEFAULT_ENV_KEY_NAME) -> None:
         self.file_path = os.path.realpath(os.path.expanduser(os.path.abspath(file_path)))
         self.key_path = os.path.realpath(os.path.expanduser(os.path.abspath(key_path)))
 
         self.env_key_name = env_key_name
 
         self.key = None
 
-    def init(self):
+    def init(self) -> tuple[str, str]:
         """
         Initializes the encryption key and encrypted file, and writes them
         to the `key_path` and `file_path` given at init.
 
         Returns:
-            Tuple<str, str>:
+            the key and contents
         """
         # Inits the key
         key = secrets.token_hex(16)
 
         with open(self.key_path, "w", encoding="utf-8") as outfile:
             outfile.write(key)
 
@@ -75,98 +79,97 @@
         # Inits the contents
         contents = ""
         with open(self.file_path, "wb") as outfile:
             outfile.write(self._encrypt(contents.encode("utf-8"), encrypted_key))
 
         return key, contents
 
-    def read(self, deserializer = lambda x: x.decode("utf-8")):
+    def read(self, deserializer: Callable[[bytes], str] | None = None) -> str:
         """
         Reads the contents (possibly deserialized with `deserializer`) of the file_path
         given at init, and decrypt them with the encryption key.
 
         Params:
-            deserializer (Callable): the deserializer to use on the contents (default: .decode("utf-8"))
+            deserializer: the deserializer to use on the contents (default: .decode("utf-8"))
 
         Returns:
-            Any:
+            the deserialized contents
 
         Raises:
             RuntimeError: if the file is not found at file_path
         """
         key = self.get_key()
 
         if not os.path.exists(self.file_path):
             raise RuntimeError(f"Missing encrypted file in {self.file_path}")
 
         with open(self.file_path, "rb") as infile:
             contents = self._decrypt(infile.read(), key)
 
-            if deserializer:
-                return deserializer(contents)
+            if deserializer is None:
+                return contents.decode("utf-8")
 
-            return contents
+            return deserializer(contents)
 
-    def write(self, contents, serializer = lambda x: x.encode("utf-8")):
+    def write(self, contents: str, serializer: Callable[[str], bytes] | None = None) -> None:
         """
         Writes the given `contents` (possibly serialized with `serializer`)
         after encrypting them with the encryption key to the file_path given at init.
 
         Params:
-            contents (str|bytes): the contents to write
-            serializer (Callable): the serializer to use on the contents (default: .encode("utf-8"))
+            contents: the contents to write
+            serializer: the serializer to use on the contents (default: .encode("utf-8"))
 
         Raises:
             RuntimeError: if the file is not found at file_path
         """
         key = self.get_key()
 
-        if serializer:
-            contents = serializer(contents)
-
-        if not isinstance(contents, bytes):
-            contents = bytes(contents, encoding="utf-8")
+        if serializer is None:
+            serialized_contents = contents.encode("utf-8")
+        else:
+            serialized_contents = serializer(contents)
 
         # Write on a temp file to avoid corrupting the
         # original file if an error happens
         tmp_path = f"{self.file_path}.tmp"
         with open(tmp_path, "wb") as outfile:
-            outfile.write(self._encrypt(contents, key))
+            outfile.write(self._encrypt(serialized_contents, key))
 
         os.rename(tmp_path, self.file_path)
 
-    def get_key(self):
+    def get_key(self) -> bytes:
         """
         Fetches the encryption key.
         First, checks if it has already been read, then checks in the environment,
         and finally, tries to read the file that should contain it.
 
         Returns:
-            bytes:
+            the encryption key
 
         Raises:
             RuntimeError: if the encryption key is not found in the env, and the the file
         """
         if self.key is not None:
             return self.key
 
         key = os.getenv(self.env_key_name)
         if key is None:
             if not os.path.exists(self.key_path):
                 raise RuntimeError(f"Missing encryption key in {self.key_path}")
 
-            with open(self.key_path, "r", encoding="utf-8") as infile:
+            with open(self.key_path, encoding="utf-8") as infile:
                 key = infile.read().strip()
 
         self.key = bytes.fromhex(key)
 
         return self.key
 
     @staticmethod
-    def _encrypt(value, key):
+    def _encrypt(value: bytes, key: bytes) -> bytes:
         # Constructs an AES-GCM Cipher object with the given key
         # and a randomly generated init_vector
         init_vector = os.urandom(12)
         encryptor = Cipher(
             algorithms.AES(key),
             modes.GCM(init_vector),
         ).encryptor()
@@ -174,21 +177,19 @@
         # Unused, but needed
         encryptor.authenticate_additional_data(b"")
 
         encrypted_value = encryptor.update(value)
         # Gives the tag
         encrypted_value += encryptor.finalize()
 
-        obfuscated_value = b"--".join([base64.b64encode(v) for v in [encrypted_value, init_vector, encryptor.tag]])
-
-        return obfuscated_value
+        return b"--".join([base64.b64encode(v) for v in [encrypted_value, init_vector, encryptor.tag]])
 
     @staticmethod
-    def _decrypt(obfuscated_value, key):
-        encrypted_value, init_vector, tag =  [base64.b64decode(v) for v in obfuscated_value.split(b"--")]
+    def _decrypt(obfuscated_value: bytes, key: bytes) -> bytes:
+        encrypted_value, init_vector, tag = (base64.b64decode(v) for v in obfuscated_value.split(b"--"))
 
         # Constructs a Cipher object with the key, init_vector, and the GCM tag
         # used to authenticate the message
         decryptor = Cipher(
             algorithms.AES(key),
             modes.GCM(init_vector, tag),
         ).decryptor()
```

### Comparing `flashback-2.1.0/flashback/formatting/__init__.py` & `flashback-2.2.0/flashback/formatting/__init__.py`

 * *Files identical despite different names*

### Comparing `flashback-2.1.0/flashback/formatting/_inflect.py` & `flashback-2.2.0/flashback/formatting/_inflect.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,13 +1,24 @@
+from __future__ import annotations
+
+from collections.abc import Callable
+
 import regex
 
 
-CRE_INFLECT_ONLY_PUNCT_SYM_NUM = regex.compile(r"^[\p{P}\p{S}\p{N}]+$", flags=regex.U)  # pylint: disable=no-member
+CRE_INFLECT_ONLY_PUNCT_SYM_NUM = regex.compile(r"^[\p{P}\p{S}\p{N}]+$", flags=regex.U)
 
-def _inflect(word, rules, categories, prepositions, base_case=str.lower):
+
+def _inflect(
+    word: str,
+    rules: list[tuple[str, str, str | None]],
+    categories: dict[str, set[str]],
+    prepositions: set[str],
+    base_case: Callable[[str], str] = str.lower,
+) -> str:
     word = base_case(str(word))
 
     if CRE_INFLECT_ONLY_PUNCT_SYM_NUM.search(word):
         return word
 
     # Recurses over compound words like mothers-in-law, eco-friendly, post-nap
     tokens = word.replace("-", " ").split(" ")
@@ -20,13 +31,12 @@
     # Applies rules
     for rule in rules:
         for suffix, inflection, category in rule:
             # A general rule
             if category is None:
                 if suffix.search(word) is not None:
                     return suffix.sub(inflection, word)
-            else:
-                if word in categories[category]:
-                    return suffix.sub(inflection, word)
+            elif word in categories[category]:
+                return suffix.sub(inflection, word)
 
     # Should never be reached, but just in case
     return word
```

### Comparing `flashback-2.1.0/flashback/formatting/camelize.py` & `flashback-2.2.0/flashback/formatting/camelize.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,15 +1,23 @@
+from __future__ import annotations
+
+from collections.abc import Iterable
+
 import regex
 
 from .snakeize import snakeize
 
 
-CRE_CAMELIZE = regex.compile(r"(?<!(?:^|-|_))[\-_](?![\-_])(.)", flags=regex.I)  # pylint: disable=no-member
+CRE_CAMELIZE = regex.compile(
+    r"(?<!(?:^|-|_))[\-_](?![\-_])(.)",
+    flags=regex.IGNORECASE,
+)
 
-def camelize(text, acronyms=None):
+
+def camelize(text: str, acronyms: Iterable[str] | None = None) -> str:
     """
     Transforms a text in any case to camelCase.
 
     Any character following a matched acronym will be capitalized.
 
     Examples:
         ```python
@@ -28,33 +36,31 @@
         #=> httphOst
 
         camelize("HTTPHost", acronyms=["HTTP"])
         #=> HTTPHost
         ```
 
     Params:
-        text (str): the text to transform into camelCase
-        acronyms (Iterable): a list of correctly cased acronyms to retain and case correctly
+        text: the text to transform into camelCase
+        acronyms: a list of correctly cased acronyms to retain and case correctly
 
     Returns:
-        str: the camel cased text
+        the camel cased text
     """
     text = snakeize(text, acronyms=acronyms)
 
     # Builds the pattern to handle acronyms
     if acronyms is None:
         lower2upper = {}
         acronyms_pattern = r"(?=$)^"
     else:
         lower2upper = {acronym.lower(): acronym for acronym in acronyms}
         acronyms_pattern = "|".join(sorted(acronyms, key=len, reverse=True))
 
-    acronyms_camelize_pattern = fr"({acronyms_pattern})(.|$)"
+    acronyms_camelize_pattern = rf"({acronyms_pattern})(.|$)"
 
     text = CRE_CAMELIZE.sub(lambda m: m.group()[1:].upper(), text)
 
-    def replace(m):
+    def replace(m: regex.Match) -> str:
         return lower2upper[m.group(1).lower()] + m.group(2).upper()
 
-    text = regex.sub(acronyms_camelize_pattern, replace, text, flags=regex.I)  # pylint: disable=no-member
-
-    return text
+    return regex.sub(acronyms_camelize_pattern, replace, text, flags=regex.IGNORECASE)
```

### Comparing `flashback-2.1.0/flashback/formatting/locales/de.py` & `flashback-2.2.0/flashback/formatting/locales/de.py`

 * *Files 13% similar despite different names*

```diff
@@ -7,31 +7,55 @@
 - https://github.com/clips/pattern/blob/master/pattern/text/de/inflect.py
 """
 
 import regex
 
 
 # Prepositions are used in compound words
-PREPOSITIONS = set((
-    "vor", "während", "bis zu",
-    "über", "hinter", "außer", "als", "aus", "zu",
-    "gegenüber", "unten", "für", "auf", "unter",
-    "nach", "unterhalb", "von", "onto", "bis",
-    "neben", "in", "bis",
-    "um", "besides", "über",
-    "at", "zwischen", "nahe", "seit", "mit", "ohne",
-    "quer", "dwars",
-    "jenseits", "aber", "sondern", "bei"
-))
+PREPOSITIONS = {
+    "vor",
+    "während",
+    "bis zu",
+    "über",
+    "hinter",
+    "außer",
+    "als",
+    "aus",
+    "zu",
+    "gegenüber",
+    "unten",
+    "für",
+    "auf",
+    "unter",
+    "nach",
+    "unterhalb",
+    "von",
+    "onto",
+    "bis",
+    "neben",
+    "in",
+    "um",
+    "besides",
+    "at",
+    "zwischen",
+    "nahe",
+    "seit",
+    "mit",
+    "ohne",
+    "quer",
+    "dwars",
+    "jenseits",
+    "aber",
+    "sondern",
+    "bei",
+}
 
 PLURAL_RULES = [
     # Indefinite articles and demonstratives
-    (
-        (r"^Diese[rs]$", "Diese", None),
-    ),
+    ((r"^Diese[rs]$", "Diese", None),),
     # Personal pronouns
     (
         (r"^Ich$", "Wir", None),
         (r"^Du$", "Ihr", None),
         (r"^Er$", "Sie", None),
         (r"^Sie$", "Sie", None),
         (r"^Es$", "Sie", None),
@@ -43,25 +67,37 @@
     (
         (r"$", "", "uninflected"),
         (r"$", "", "uncountable"),
         (r"$", "", "nationalities"),
         (r"^(Ge)", r"\1", None),
         (r"(gie)$", r"\1", None),
         (r"(au|ein|eit|er|[^i]en|[^i]el|chen|mus|tät|tik|tum|u)$", r"\1", None),
-        (r"(mie|rie|sis|rin|ein|age|ern|ber|ion|inn|ben|äse|eis|hme|iss|hen|fer|gie|fen|her|ker|nie|mer|ler|men|ass"
-         "|ner|per|rer|mus|abe|ter|ser|äle|hie|ger|tus|gen|ier|ver|zer)$", r"\1", None),
+        (
+            r"(mie|rie|sis|rin|ein|age|ern|ber|ion|inn|ben|äse|eis|hme|iss|hen|fer|gie|fen|her|ker|nie|mer|ler|men|ass"
+            "|ner|per|rer|mus|abe|ter|ser|äle|hie|ger|tus|gen|ier|ver|zer)$",
+            r"\1",
+            None,
+        ),
     ),
     # Irregular inflections for common suffixes
     (
-        (r"(abe|ade|age|ale|ame|ane|are|ase|ate|che|cke|ede|ene|ere|ese|ffe|hie|hle|hme|hne|hre|hse|hte|ide|ife|ihe"
-         "|ine|ise|ite|lge|lie|lle|mme|mpe|nde|nge|nie|nke|nne|nte|nze|ode|oge|one|ose|ote|pie|ppe|rbe|rde|rie|rke"
-         "|rre|rte|sie|sse|ste|tie|tte|tze|ube|ude|ufe|uge|ule|ume|use|ute)$", r"\1n", None),
-        (r"(ahr|akt|arn|bot|chs|ehl|eil|eim|eis|ekt|ell|erd|erk|ern|ert|ess|est|etz|eug"
-         "|ekt|eur|ich|ick|ieb|eif|weg|ohr|ord|rot|tag|nkt|mpf|nat|nst|off|oot|lar|ruf"
-         "|rzt|tiv|ieg|iel|iet|iff|ilm|ing|iss|itt|itz)$", r"\1e", None),
+        (
+            r"(abe|ade|age|ale|ame|ane|are|ase|ate|che|cke|ede|ene|ere|ese|ffe|hie|hle|hme|hne|hre|hse|hte|ide|ife|ihe"
+            "|ine|ise|ite|lge|lie|lle|mme|mpe|nde|nge|nie|nke|nne|nte|nze|ode|oge|one|ose|ote|pie|ppe|rbe|rde|rie|rke"
+            "|rre|rte|sie|sse|ste|tie|tte|tze|ube|ude|ufe|uge|ule|ume|use|ute)$",
+            r"\1n",
+            None,
+        ),
+        (
+            r"(ahr|akt|arn|bot|chs|ehl|eil|eim|eis|ekt|ell|erd|erk|ern|ert|ess|est|etz|eug"
+            "|ekt|eur|ich|ick|ieb|eif|weg|ohr|ord|rot|tag|nkt|mpf|nat|nst|off|oot|lar|ruf"
+            "|rzt|tiv|ieg|iel|iet|iff|ilm|ing|iss|itt|itz)$",
+            r"\1e",
+            None,
+        ),
         (r"(aat|ahn|ant|aph|lei|ift|ist|enz|hrt|ion|orm|rei|tur|tor|uhr|ung|or|ei|schaft)$", r"\1en", None),
         (r"(rin|tin)$", r"\1nen", None),
         (r"(eld|ild|ind)$", r"\1er", None),
         (r"o(lz|rn)$", r"ö\1er", None),
         (r"a(ch|mt|nn|tt|us)$", r"ä\1er", None),
         (r"a(ng|nk|tz|um)$", r"ä\1e", None),
         (r"o(ck|hn|pf)$", r"ö\1e", None),
@@ -80,34 +116,30 @@
         (r"(ück)$", r"\1e", None),
         (r"(in)$", r"\1nen", None),
         (r"o$", r"os", None),
         (r"a$", r"en", None),
         (r"e$", r"en", None),
     ),
     # Assume that the plural takes -e
-    (
-        (r"$", "e", None),
-    )
+    ((r"$", "e", None),),
 ]
 
 # For performance, compile the regular expressions once:
 PLURAL_RULES = [[(regex.compile(r[0]), r[1], r[2]) for r in grp] for grp in PLURAL_RULES]
 
 # Suffix categories
 PLURAL_CATEGORIES = {
-    "uninflected": set(()),
-    "uncountable": set(()),
-    "nationalities": set(()),
+    "uninflected": set(),
+    "uncountable": set(),
+    "nationalities": set(),
 }
 
 SINGULAR_RULES = [
     # Indefinite articles and demonstratives
-    (
-        (r"^Diese$", "Dieses", None),
-    ),
+    ((r"^Diese$", "Dieses", None),),
     # Personal pronouns
     (
         (r"^Wir$", "Ich", None),
         (r"^Ihr$", "Du", None),
         (r"^Sie$", "Er", None),
         (r"^Sie$", "Sie", None),
         (r"^Sie$", "Es", None),
@@ -119,56 +151,64 @@
     (
         (r"$", "", "uninflected"),
         (r"$", "", "uncountable"),
         (r"$", "", "nationalities"),
         (r"^(Ge)", r"\1", None),
         (r"(gie)$", r"\1", None),
         (r"(au|ein|eit|er|[^i]en|[^i]el|chen|mus|tät|tik|tum|u)$", r"\1", None),
-        (r"(mie|rie|sis|rin|ein|age|ern|ber|ion|inn|ben|äse|eis|hme|iss|hen|fer|gie|fen|her|ker"
-         "|nie|mer|ler|men|ass|ner|per|rer|mus|abe|ter|ser|äle|hie|ger|tus|gen|ier|ver|zer)$", r"\1", None),
+        (
+            r"(mie|rie|sis|rin|ein|age|ern|ber|ion|inn|ben|äse|eis|hme|iss|hen|fer|gie|fen|her|ker"
+            "|nie|mer|ler|men|ass|ner|per|rer|mus|abe|ter|ser|äle|hie|ger|tus|gen|ier|ver|zer)$",
+            r"\1",
+            None,
+        ),
     ),
     # Irregular plural forms
-    (
-        (r"^Löwen$", "Löwe", None),
-    ),
+    ((r"^Löwen$", "Löwe", None),),
     # Irregular inflections for common suffixes
     (
         (r"innen$", r"in", None),
         (r"nisse$", "nis", None),
         (r"(ück|ühl)e$", r"\1", None),
         (r"(ühre|üte|üre|üse)n$", r"\1", None),
         (r"ü(ch|rm|hn)er$", r"u\1", None),
         (r"ü(st|ft|ch|rf|ng|nd|ss|rm)e$", r"u\1", None),
         (r"ä(nz|dt|rt|ck|hn|nk|ft|st|nd|ll|ht|ut|ss|tz|ng|mm|uf|um)e$", r"a\1", None),
         (r"(one|oge|ode|obe|ole|ose|ote)n$", r"\1", None),
         (r"(z|l)üge$", "\1ug", None),
         (r"ö(ck|pf|hn|ss)e$", r"o\1", None),
         (r"(h|t)ö(f|n)e$", "\1o\2", None),
-        (r"(tte|mbe|lle|yse|rbe|hse|rve|rke|use|tie|ibe|ife|sse|gie|ete|rde|nce|ube|lbe|age|ane|ske|ede"
-         "|gge|nte|mme|ige|nke|ine|see|ule|hre|abe|uge|lie|ase|ade|die|are|tze|hie|nde|hme|ffe|rme|ste"
-         "|ame|hne|ume|nne|ale|mpe|mie|rte|rie|ude|lge|nge|ide|lke|ere|hle|ise|rne|pie|ihe|ese|äre|sie"
-         "|ive|ppe|ene|lfe|nie|une|cke)n$", r"\1", None),
-        (r"(tät|ahn|ent|hrt|ahl|uhr|sur|cht|kur|erz|sor|tat|ist|eit|rat|orm|ion|nis|ung|urt"
-         "|enz|aat|aph|tür|son|tor|ant|tur)en$", r"\1", None),
+        (
+            r"(tte|mbe|lle|yse|rbe|hse|rve|rke|use|tie|ibe|ife|sse|gie|ete|rde|nce|ube|lbe|age|ane|ske|ede"
+            "|gge|nte|mme|ige|nke|ine|see|ule|hre|abe|uge|lie|ase|ade|die|are|tze|hie|nde|hme|ffe|rme|ste"
+            "|ame|hne|ume|nne|ale|mpe|mie|rte|rie|ude|lge|nge|ide|lke|ere|hle|ise|rne|pie|ihe|ese|äre|sie"
+            "|ive|ppe|ene|lfe|nie|une|cke)n$",
+            r"\1",
+            None,
+        ),
+        (
+            r"(tät|ahn|ent|hrt|ahl|uhr|sur|cht|kur|erz|sor|tat|ist|eit|rat|orm|ion|nis|ung|urt"
+            "|enz|aat|aph|tür|son|tor|ant|tur)en$",
+            r"\1",
+            None,
+        ),
         (r"ö(rn|lz|ch|rt)er$", r"o\1", None),
         (r"güter$", "gut", None),
         (r"bäder$", "bad", None),
         (r"räder$", "rad", None),
         (r"räser$", "ras", None),
         (r"läser$", "las", None),
         (r"läge$", "lag", None),
         (r"läne$", "lan", None),
         (r"(r|h)aün$", r"\1a", None),
         (r"räge$", "rag", None),
         (r"ä(nd|ch|ul|tt|nn|us|mt)er$", r"\1", None),
     ),
     # Assume that the plural takes
-    (
-        (r"(?!<(rr|rv|nz))(nen|en|n|e|er|s)$", "", None),
-    )
+    ((r"(?!<(rr|rv|nz))(nen|en|n|e|er|s)$", "", None),),
 ]
 
 # For performance, compile the regular expressions only once:
 SINGULAR_RULES = [[(regex.compile(r[0]), r[1], r[2]) for r in grp] for grp in SINGULAR_RULES]
 
 # Suffix categories
 SINGULAR_CATEGORIES = {
```

### Comparing `flashback-2.1.0/flashback/formatting/locales/en.py` & `flashback-2.2.0/flashback/formatting/locales/en.py`

 * *Files 17% similar despite different names*

```diff
@@ -7,53 +7,84 @@
 - https://github.com/clips/pattern/blob/master/pattern/text/en/inflect.py
 """
 
 import regex
 
 
 # Prepositions are used in compound words
-PREPOSITIONS = set((
-    "about", "before", "during", "of", "till",
-    "above", "behind", "except", "off", "to",
-    "across", "below", "for", "on", "under",
-    "after", "beneath", "from", "onto", "until",
-    "among", "beside", "in", "out", "unto",
-    "around", "besides", "into", "over", "upon",
-    "as", "at", "between", "near", "since", "with", "without",
-    "athwart", "betwixt",
+PREPOSITIONS = {
+    "about",
+    "before",
+    "during",
+    "of",
+    "till",
+    "above",
+    "behind",
+    "except",
+    "off",
+    "to",
+    "across",
+    "below",
+    "for",
+    "on",
+    "under",
+    "after",
+    "beneath",
+    "from",
+    "onto",
+    "until",
+    "among",
+    "beside",
+    "in",
+    "out",
+    "unto",
+    "around",
+    "besides",
+    "into",
+    "over",
+    "upon",
+    "as",
+    "at",
+    "between",
+    "near",
+    "since",
+    "with",
+    "without",
+    "athwart",
+    "betwixt",
     "beyond",
     "but",
     "by",
-))
+}
 
 PLURAL_RULES = [
     # Indefinite articles and demonstratives
     (
         (r"^a$|^an$", "some", None),
         (r"^this$", "these", None),
         (r"^that$", "those", None),
-        (r"^any$", "all", None)
+        (r"^any$", "all", None),
     ),
     # Possessive adjectives
     (
         (r"^my$", "our", None),
         (r"^your$", "your", None),
         (r"^thy$", "your", None),
         (r"^her$|^his$", "their", None),
         (r"^its$", "their", None),
-        (r"^their$", "their", None)
+        (r"^their$", "their", None),
     ),
     # Possessive pronouns
     (
         (r"^mine$", "ours", None),
         (r"^yours$", "yours", None),
         (r"^thine$", "yours", None),
         (r"^her$|^his$", "theirs", None),
         (r"^its$", "theirs", None),
-        (r"^their$", "theirs", None)
+        (r"^their$", "theirs", None),
     ),
     # Personal pronouns
     (
         (r"^i$", "we", None),
         (r"^me$", "us", None),
         (r"^myself$", "ourselves", None),
         (r"^you$", "you", None),
@@ -64,15 +95,15 @@
         (r"^it$|^they$", "they", None),
         (r"^her$|^him$", "them", None),
         (r"^it$|^them$", "them", None),
         (r"^herself$", "themselves", None),
         (r"^himself$", "themselves", None),
         (r"^itself$", "themselves", None),
         (r"^themself$", "themselves", None),
-        (r"^oneself$", "oneselves", None)
+        (r"^oneself$", "oneselves", None),
     ),
     # Words that do not inflect
     (
         (r"$", "", "uninflected"),
         (r"$", "", "uncountable"),
         (r"$", "", "nationalities"),
         (r"series$", "series", None),
@@ -80,15 +111,15 @@
         (r"([- ])bass$", r"\1bass", None),
         (r"ois$", "ois", None),
         (r"sheep$", "sheep", None),
         (r"deer$", "deer", None),
         (r"pox$", "pox", None),
         (r"([a-z].*)ese$", r"\1ese", None),
         (r"itis$", "itis", None),
-        (r"(fruct|gluc|galact|lact|ket|malt|rib|sacchar|cellul)ose$", r"\1ose", None)
+        (r"(fruct|gluc|galact|lact|ket|malt|rib|sacchar|cellul)ose$", r"\1ose", None),
     ),
     # Irregular plural forms
     (
         (r"atlas$", "atlases", None),
         (r"child$", "children", None),
         (r"corpus$", "corpora", None),
         (r"ephemeris$", "ephemerides", None),
@@ -136,149 +167,335 @@
         (r"eau$", "eaux", None),
         (r"ieu$", "ieu", None),
         (r"([iay])nx$", r"\1nges", None),
         (r"is$", "ises", "is-ises"),
         (r"us$", "i", "us-i"),
         (r"us$", "uses", "us-uses"),
         (r"o$", "i", "o-i"),
-        (r"$", "im", "-im")
+        (r"$", "im", "-im"),
     ),
     # -ch, -sh and -ss and the s-singular group take -es in the plural
-    (
-        (r"([cs])h$", r"\1hes", None),
-        (r"ss$", "sses", None),
-        (r"x$", "xes", None),
-        (r"s$", "ses", "s-singular")
-    ),
+    ((r"([cs])h$", r"\1hes", None), (r"ss$", "sses", None), (r"x$", "xes", None), (r"s$", "ses", "s-singular")),
     # -f or -fe sometimes take -ves in the plural
     (
         (r"([aeo]l)f$", r"\1ves", None),
         (r"([^d]ea)f$", r"\1ves", None),
         (r"arf$", "arves", None),
         (r"([nlw]i)fe$", r"\1ves", None),
-        (r"(hoo|thie|shel)f$", r"\1ves", None)
+        (r"(hoo|thie|shel)f$", r"\1ves", None),
     ),
     # -y takes -ys if preceded by a vowel, -ies otherwise
-    (
-        (r"([aeiou])y$", r"\1ys", None),
-        (r"y$", "ies", None)
-    ),
+    ((r"([aeiou])y$", r"\1ys", None), (r"y$", "ies", None)),
     # -o sometimes takes -os, -oes otherwise. -o preceded by a vowel takes -os
-    (
-        (r"o$", "os", "o-os"),
-        (r"([aeiou])o$", r"\1os", None),
-        (r"o$", "oes", None)
-    ),
+    ((r"o$", "os", "o-os"), (r"([aeiou])o$", r"\1os", None), (r"o$", "oes", None)),
     # Assume that the plural takes -s
     (
         (r"(s)$", r"\1", None),
         (r"$", "s", None),
-    )
+    ),
 ]
 
 # For performance, compile the regular expressions once:
 PLURAL_RULES = [[(regex.compile(r[0]), r[1], r[2]) for r in grp] for grp in PLURAL_RULES]
 
 # Suffix categories
 PLURAL_CATEGORIES = {
-    "uninflected": set((
-        "the", "yes", "no", "this", "next", "old",
-        "beef", "bison", "debris", "headquarters", "news", "swine",
-        "bream", "diabetes", "herpes", "pincers", "trout",
-        "breeches", "djinn", "high-jinks", "pliers", "tuna",
-        "britches", "eland", "homework", "proceedings", "whiting",
-        "carp", "elk", "innings", "rabies", "wildebeest",
-        "chassis", "flounder", "jackanapes", "salmon",
-        "clippers", "gallows", "mackerel", "scissors",
-        "cod", "graffiti", "measles",
-        "contretemps", "mews", "shears", "wilderness",
-        "corps", "mumps", "species", "christmas", "georgia",
-        "north", "south", "east", "west", "jeans", "police",
-    )),
-    "uncountable": set((
-        "stamina", "advice", "fruit", "ketchup", "meat", "sand",
-        "bread", "furniture", "knowledge", "mustard", "software",
-        "butter", "garbage", "love", "news", "understanding",
-        "cannabis", "gravel", "luggage", "progress", "water",
-        "cheese", "happiness", "mathematics", "research",
-        "electricity", "information", "mayonnaise", "rice",
-        "equipment", "blood",
-    )),
-    "nationalities": set((
-        "german", "spanish", "british", "english", "scottish", "turkish", "dutch", "swiss",
-    )),
-    "s-singular": set((
-        "acropolis", "caddis", "dais", "glottis", "pathos",
-        "aegis", "canvas", "digitalis", "ibis", "pelvis",
-        "alias", "chaos", "epidermis", "lens", "polis",
-        "asbestos", "cosmos", "ethos", "mantis", "rhinoceros",
-        "bathos", "gas", "marquis", "sassafras",
-        "bias", "glottis", "metropolis", "trellis",
-    )),
-    "ex-ices": set((
-        "codex", "murex", "silex", "apex", "index", "pontifex", "vertex",
-        "cortex", "latex", "simplex", "vortex",
-    )),
-    "um-a": set((
-        "agendum", "candelabrum", "desideratum", "extremum", "stratum",
-        "bacterium", "datum", "erratum", "ovum", "aquarium", "emporium", "maximum", "optimum", "stadium",
-        "compendium", "enconium", "medium", "phylum", "trapezium",
-        "consortium", "gymnasium", "memorandum", "quantum", "ultimatum",
-        "cranium", "honorarium", "millenium", "rostrum", "vacuum",
-        "curriculum", "interregnum", "minimum", "spectrum", "velum",
-        "dictum", "lustrum", "momentum", "speculum",
-    )),
-    "on-a": set((
-        "aphelion", "hyperbaton", "perihelion",
-        "asyndeton", "noumenon", "phenomenon",
-        "criterion", "organon", "prolegomenon",
-    )),
-    "a-ae": set((
-        "alga", "alumna", "vertebra", "abscissa", "aurora", "hyperbola", "nebula",
-        "amoeba", "formula", "lacuna", "nova",
-        "antenna", "hydra", "medusa", "parabola",
-    )),
-    "is-ises": set((
-        "clitoris", "iris",
-    )),
-    "us-i": set((
-        "focus", "nimbus", "succubus",
-        "fungus", "nucleolus", "torus",
-        "genius", "radius", "umbilicus",
-        "incubus", "stylus", "uterus", "stimulus",
-    )),
-    "us-uses": set((
-        "apparatus", "hiatus", "plexus", "status",
-        "cantus", "impetus", "prospectus",
-        "coitus", "nexus", "sinus", "bus", "virus",
-    )),
-    "o-i": set((
-        "alto", "canto", "crescendo", "soprano",
-        "basso", "contralto", "tempo",
-    )),
-    "-im": set((
-        "cherub", "goy", "seraph",
-    )),
-    "o-os": set((
-        "albino", "dynamo", "guano", "lumbago", "photo", "piano", "solo",
-        "archipelago", "embryo", "inferno", "magneto", "pro",
-        "armadillo", "fiasco", "jumbo", "manifesto", "quarto",
-        "commando", "generalissimo", "medico", "rhino",
-        "ditto", "ghetto", "lingo", "octavo", "stylo",
-    )),
+    "uninflected": {
+        "the",
+        "yes",
+        "no",
+        "this",
+        "next",
+        "old",
+        "beef",
+        "bison",
+        "debris",
+        "headquarters",
+        "news",
+        "swine",
+        "bream",
+        "diabetes",
+        "herpes",
+        "pincers",
+        "trout",
+        "breeches",
+        "djinn",
+        "high-jinks",
+        "pliers",
+        "tuna",
+        "britches",
+        "eland",
+        "homework",
+        "proceedings",
+        "whiting",
+        "carp",
+        "elk",
+        "innings",
+        "rabies",
+        "wildebeest",
+        "chassis",
+        "flounder",
+        "jackanapes",
+        "salmon",
+        "clippers",
+        "gallows",
+        "mackerel",
+        "scissors",
+        "cod",
+        "graffiti",
+        "measles",
+        "contretemps",
+        "mews",
+        "shears",
+        "wilderness",
+        "corps",
+        "mumps",
+        "species",
+        "christmas",
+        "georgia",
+        "north",
+        "south",
+        "east",
+        "west",
+        "jeans",
+        "police",
+    },
+    "uncountable": {
+        "stamina",
+        "advice",
+        "fruit",
+        "ketchup",
+        "meat",
+        "sand",
+        "bread",
+        "furniture",
+        "knowledge",
+        "mustard",
+        "software",
+        "butter",
+        "garbage",
+        "love",
+        "news",
+        "understanding",
+        "cannabis",
+        "gravel",
+        "luggage",
+        "progress",
+        "water",
+        "cheese",
+        "happiness",
+        "mathematics",
+        "research",
+        "electricity",
+        "information",
+        "mayonnaise",
+        "rice",
+        "equipment",
+        "blood",
+    },
+    "nationalities": {
+        "german",
+        "spanish",
+        "british",
+        "english",
+        "scottish",
+        "turkish",
+        "dutch",
+        "swiss",
+    },
+    "s-singular": {
+        "acropolis",
+        "caddis",
+        "dais",
+        "glottis",
+        "pathos",
+        "aegis",
+        "canvas",
+        "digitalis",
+        "ibis",
+        "pelvis",
+        "alias",
+        "chaos",
+        "epidermis",
+        "lens",
+        "polis",
+        "asbestos",
+        "cosmos",
+        "ethos",
+        "mantis",
+        "rhinoceros",
+        "bathos",
+        "gas",
+        "marquis",
+        "sassafras",
+        "bias",
+        "metropolis",
+        "trellis",
+    },
+    "ex-ices": {
+        "codex",
+        "murex",
+        "silex",
+        "apex",
+        "index",
+        "pontifex",
+        "vertex",
+        "cortex",
+        "latex",
+        "simplex",
+        "vortex",
+    },
+    "um-a": {
+        "agendum",
+        "candelabrum",
+        "desideratum",
+        "extremum",
+        "stratum",
+        "bacterium",
+        "datum",
+        "erratum",
+        "ovum",
+        "aquarium",
+        "emporium",
+        "maximum",
+        "optimum",
+        "stadium",
+        "compendium",
+        "enconium",
+        "medium",
+        "phylum",
+        "trapezium",
+        "consortium",
+        "gymnasium",
+        "memorandum",
+        "quantum",
+        "ultimatum",
+        "cranium",
+        "honorarium",
+        "millenium",
+        "rostrum",
+        "vacuum",
+        "curriculum",
+        "interregnum",
+        "minimum",
+        "spectrum",
+        "velum",
+        "dictum",
+        "lustrum",
+        "momentum",
+        "speculum",
+    },
+    "on-a": {
+        "aphelion",
+        "hyperbaton",
+        "perihelion",
+        "asyndeton",
+        "noumenon",
+        "phenomenon",
+        "criterion",
+        "organon",
+        "prolegomenon",
+    },
+    "a-ae": {
+        "alga",
+        "alumna",
+        "vertebra",
+        "abscissa",
+        "aurora",
+        "hyperbola",
+        "nebula",
+        "amoeba",
+        "formula",
+        "lacuna",
+        "nova",
+        "antenna",
+        "hydra",
+        "medusa",
+        "parabola",
+    },
+    "is-ises": {
+        "clitoris",
+        "iris",
+    },
+    "us-i": {
+        "focus",
+        "nimbus",
+        "succubus",
+        "fungus",
+        "nucleolus",
+        "torus",
+        "genius",
+        "radius",
+        "umbilicus",
+        "incubus",
+        "stylus",
+        "uterus",
+        "stimulus",
+    },
+    "us-uses": {
+        "apparatus",
+        "hiatus",
+        "plexus",
+        "status",
+        "cantus",
+        "impetus",
+        "prospectus",
+        "coitus",
+        "nexus",
+        "sinus",
+        "bus",
+        "virus",
+    },
+    "o-i": {
+        "alto",
+        "canto",
+        "crescendo",
+        "soprano",
+        "basso",
+        "contralto",
+        "tempo",
+    },
+    "-im": {
+        "cherub",
+        "goy",
+        "seraph",
+    },
+    "o-os": {
+        "albino",
+        "dynamo",
+        "guano",
+        "lumbago",
+        "photo",
+        "piano",
+        "solo",
+        "archipelago",
+        "embryo",
+        "inferno",
+        "magneto",
+        "pro",
+        "armadillo",
+        "fiasco",
+        "jumbo",
+        "manifesto",
+        "quarto",
+        "commando",
+        "generalissimo",
+        "medico",
+        "rhino",
+        "ditto",
+        "ghetto",
+        "lingo",
+        "octavo",
+        "stylo",
+    },
 }
 
 SINGULAR_RULES = [
     # Indefinite articles and demonstratives
-    (
-        (r"^some$", "a", None),
-        (r"^these$", "this", None),
-        (r"^those$", "that", None),
-        (r"^all$", "any", None)
-    ),
+    ((r"^some$", "a", None), (r"^these$", "this", None), (r"^those$", "that", None), (r"^all$", "any", None)),
     # Possessive adjectives
     (
         (r"^our$", "my", None),
         (r"^your$", "your", None),
         (r"^their$", "its", None),
     ),
     # Possessive pronouns
@@ -294,15 +511,15 @@
         (r"^ourselves$", "myself", None),
         (r"^you$", "you", None),
         (r"^ye$", "thou", None),
         (r"^yourself$", "yourself", None),
         (r"^they$", "it", None),
         (r"^them$", "it", None),
         (r"^themselvesf$", "itself", None),
-        (r"^oneselves$", "oneself", None)
+        (r"^oneselves$", "oneself", None),
     ),
     # Words that do not inflect
     (
         (r"$", "", "uninflected"),
         (r"$", "", "uncountable"),
         (r"^(\d{2}(?:\d{2})?s)$", r"\1", None),
         (r"series$", "series", None),
@@ -310,15 +527,15 @@
         (r"([- ])bass$", r"\1bass", None),
         (r"ois$", "ois", None),
         (r"sheep$", "sheep", None),
         (r"deer$", "deer", None),
         (r"pox$", "pox", None),
         (r"([a-z].*)ese$", r"\1ese", None),
         (r"itis$", "itis", None),
-        (r"(fruct|gluc|galact|lact|ket|malt|rib|sacchar|cellul)ose$", r"\1ose", None)
+        (r"(fruct|gluc|galact|lact|ket|malt|rib|sacchar|cellul)ose$", r"\1ose", None),
     ),
     # Irregular plural forms
     (
         (r"atla(ntes|ses)$", "atlas", None),
         (r"children$", "child", None),
         (r"corpora$", "corpus", None),
         (r"corpuses$", "corpus", None),
@@ -351,15 +568,15 @@
         (r"men$", "man", None),
         (r"people$", "person", None),
         (r"([lm])ice$", r"\1ouse", None),
         (r"teeth$", "tooth", None),
         (r"geese$", "goose", None),
         (r"feet$", "foot", None),
         (r"zoa$", "zoon", None),
-        (r"([csx])es$", r"\1is", "is-es")
+        (r"([csx])es$", r"\1is", "is-es"),
     ),
     # Fully assimilated classical inflections
     (
         (r"ices$", "ex", "ex-ices"),
         (r"a$", "um", "um-a"),
         (r"a$", "on", "on-a"),
         (r"ae$", "a", "a-ae"),
@@ -374,119 +591,275 @@
         (r"i$", "us", "us-i"),
         (r"uses$", "us", "us-uses"),
         (r"i$", "o", "o-i"),
         (r"im$", "", "-im"),
         (r"ies$", "ie", "ie-ies"),
     ),
     # -ch, -sh and -ss and the s-singular group take -es in the plural
-    (
-        (r"([cs])hes$", r"\1h", None),
-        (r"sses$", "ss", None),
-        (r"xes$", "x", None),
-        (r"ses$", "s", "s-singular")
-    ),
+    ((r"([cs])hes$", r"\1h", None), (r"sses$", "ss", None), (r"xes$", "x", None), (r"ses$", "s", "s-singular")),
     # -f or -fe sometimes take -ves in the plural
     (
         (r"([aeo]l)ves$", r"\1f", None),
         (r"([^d]ea)ves$", r"\1f", None),
         (r"arves$", "arf", None),
         (r"([nlw]i)ves$", r"\1fe", None),
-        (r"(hoo|thie|shel)ves$", r"\1f", None)
+        (r"(hoo|thie|shel)ves$", r"\1f", None),
     ),
     # -y takes -ys if preceded by a vowel, -ies otherwise
-    (
-        (r"([aeiou])ys$", r"\1y", None),
-        (r"ies$", "y", None)
-    ),
+    ((r"([aeiou])ys$", r"\1y", None), (r"ies$", "y", None)),
     # -o sometimes takes -os, -oes otherwise. -o preceded by a vowel takes -os
-    (
-        (r"os$", "o", "o-os"),
-        (r"([aeiou])os$", r"\1o", None),
-        (r"oes$", "o", None)
-    ),
+    ((r"os$", "o", "o-os"), (r"([aeiou])os$", r"\1o", None), (r"oes$", "o", None)),
     # Assume that the plural takes -s
-    (
-        (r"(?<!s)s$", "", None),
-    )
+    ((r"(?<!s)s$", "", None),),
 ]
 
 # For performance, compile the regular expressions only once:
 SINGULAR_RULES = [[(regex.compile(r[0]), r[1], r[2]) for r in grp] for grp in SINGULAR_RULES]
 
 # Suffix categories
 SINGULAR_CATEGORIES = {
     "uninflected": PLURAL_CATEGORIES["uninflected"],
     "uncountable": PLURAL_CATEGORIES["uncountable"],
     "nationalities": PLURAL_CATEGORIES["nationalities"],
-    "s-singular": set((
-        "acropolises", "caddises", "daises", "glottises", "pathoses",
-        "aegises", "canvases", "digitalises", "ibises", "pelvises",
-        "aliases", "chaoses", "epidermises", "lenses", "polises",
-        "asbestoses", "cosmoses", "ethoses", "mantises", "rhinoceroses",
-        "bathoses", "gases", "marquises", "sassafrases",
-        "biases", "glottises", "metropolises", "trellises",
-    )),
-    "ie-ies": set((
-        "alergies", "cuties", "hoagies", "newbies", "softies", "veggies",
-        "aunties", "doggies", "hotties", "nighties", "sorties", "weenies",
-        "beanies", "eyries", "indies", "oldies", "stoolies", "yuppies",
-        "birdies", "freebies", "junkies", "pies", "sweeties", "zombies",
-        "bogies", "goonies", "laddies", "pixies", "techies",
-        "bombies", "groupies", "laramies", "quickies", "^ties",
-        "collies", "hankies", "lingeries", "reveries", "toughies",
-        "cookies", "hippies", "meanies", "rookies", "valkyries", "movies",
-    )),
-    "ex-ices": set((
-        "codices", "murices", "silices", "apices", "indices", "pontifices", "vertices",
-        "cortices", "latices", "simplices", "vortices",
-    )),
-    "um-a": set((
-        "agenda", "candelabra", "desiderata", "extrema", "strata",
-        "bacteria", "data", "errata", "ova", "aquaria", "emporia", "maxima", "optima", "stadia",
-        "compendia", "enconia", "media", "phyla", "trapezia",
-        "consortia", "gymnasia", "memoranda", "quanta", "ultimata",
-        "crania", "honoraria", "millenia", "rostra", "vacua",
-        "curricula", "interregna", "minima", "spectra", "vela",
-        "dicta", "lustra", "momenta", "specula",
-    )),
-    "on-a": set((
-        "aphelia", "hyperbata", "perihelia",
-        "asyndeta", "noumena", "phenomena",
-        "criteria", "organa", "prolegomena",
-    )),
-    "a-ae": set((
-        "algae", "alumnae", "vertebrae", "abscissae", "aurorae", "hyperbolae", "nebulae",
-        "amoebae", "formulae", "lacunae", "novae",
-        "antennae", "hydrae", "medusae", "parabolae",
-    )),
-    "is-ises": set((
-        "clitorises", "irises",
-    )),
-    "is-es": set((
-        "analyses", "bases", "diagnoses", "parentheses", "prognoses", "synopses", "theses",
-    )),
-    "us-i": set((
-        "foci", "nimbi", "succubi",
-        "fungi", "nucleoli", "tori",
-        "genii", "radii", "umbilici",
-        "incubi", "styli", "uteri", "stimuli",
-    )),
-    "us-uses": set((
-        "apparatuses", "hiatuses", "plexuses", "statuses",
-        "cantuses", "impetuses", "prospectuses",
-        "coituses", "nexuses", "sinuses", "buses", "viruses",
-    )),
-    "o-i": set((
-        "alti", "canti", "crescendi", "soprani",
-        "bassi", "contralti", "soli", "tempi",
-    )),
-    "-im": set((
-        "cherubim", "goyim", "seraphim",
-    )),
-    "o-os": set((
-        "albinos", "dynamos", "guanos", "lumbagos", "photos", "pianos", "solos",
-        "archipelagos", "embryos", "infernos", "magnetos", "pros",
-        "armadillos", "fiascos", "jumbos", "manifestos", "quartos",
-        "commandos", "generalissimos", "medicos", "rhinos",
-        "dittos", "ghettos", "lingos", "octavos", "stylos",
-    )),
+    "s-singular": {
+        "acropolises",
+        "caddises",
+        "daises",
+        "glottises",
+        "pathoses",
+        "aegises",
+        "canvases",
+        "digitalises",
+        "ibises",
+        "pelvises",
+        "aliases",
+        "chaoses",
+        "epidermises",
+        "lenses",
+        "polises",
+        "asbestoses",
+        "cosmoses",
+        "ethoses",
+        "mantises",
+        "rhinoceroses",
+        "bathoses",
+        "gases",
+        "marquises",
+        "sassafrases",
+        "biases",
+        "metropolises",
+        "trellises",
+    },
+    "ie-ies": {
+        "alergies",
+        "cuties",
+        "hoagies",
+        "newbies",
+        "softies",
+        "veggies",
+        "aunties",
+        "doggies",
+        "hotties",
+        "nighties",
+        "sorties",
+        "weenies",
+        "beanies",
+        "eyries",
+        "indies",
+        "oldies",
+        "stoolies",
+        "yuppies",
+        "birdies",
+        "freebies",
+        "junkies",
+        "pies",
+        "sweeties",
+        "zombies",
+        "bogies",
+        "goonies",
+        "laddies",
+        "pixies",
+        "techies",
+        "bombies",
+        "groupies",
+        "laramies",
+        "quickies",
+        "^ties",
+        "collies",
+        "hankies",
+        "lingeries",
+        "reveries",
+        "toughies",
+        "cookies",
+        "hippies",
+        "meanies",
+        "rookies",
+        "valkyries",
+        "movies",
+    },
+    "ex-ices": {
+        "codices",
+        "murices",
+        "silices",
+        "apices",
+        "indices",
+        "pontifices",
+        "vertices",
+        "cortices",
+        "latices",
+        "simplices",
+        "vortices",
+    },
+    "um-a": {
+        "agenda",
+        "candelabra",
+        "desiderata",
+        "extrema",
+        "strata",
+        "bacteria",
+        "data",
+        "errata",
+        "ova",
+        "aquaria",
+        "emporia",
+        "maxima",
+        "optima",
+        "stadia",
+        "compendia",
+        "enconia",
+        "media",
+        "phyla",
+        "trapezia",
+        "consortia",
+        "gymnasia",
+        "memoranda",
+        "quanta",
+        "ultimata",
+        "crania",
+        "honoraria",
+        "millenia",
+        "rostra",
+        "vacua",
+        "curricula",
+        "interregna",
+        "minima",
+        "spectra",
+        "vela",
+        "dicta",
+        "lustra",
+        "momenta",
+        "specula",
+    },
+    "on-a": {
+        "aphelia",
+        "hyperbata",
+        "perihelia",
+        "asyndeta",
+        "noumena",
+        "phenomena",
+        "criteria",
+        "organa",
+        "prolegomena",
+    },
+    "a-ae": {
+        "algae",
+        "alumnae",
+        "vertebrae",
+        "abscissae",
+        "aurorae",
+        "hyperbolae",
+        "nebulae",
+        "amoebae",
+        "formulae",
+        "lacunae",
+        "novae",
+        "antennae",
+        "hydrae",
+        "medusae",
+        "parabolae",
+    },
+    "is-ises": {
+        "clitorises",
+        "irises",
+    },
+    "is-es": {
+        "analyses",
+        "bases",
+        "diagnoses",
+        "parentheses",
+        "prognoses",
+        "synopses",
+        "theses",
+    },
+    "us-i": {
+        "foci",
+        "nimbi",
+        "succubi",
+        "fungi",
+        "nucleoli",
+        "tori",
+        "genii",
+        "radii",
+        "umbilici",
+        "incubi",
+        "styli",
+        "uteri",
+        "stimuli",
+    },
+    "us-uses": {
+        "apparatuses",
+        "hiatuses",
+        "plexuses",
+        "statuses",
+        "cantuses",
+        "impetuses",
+        "prospectuses",
+        "coituses",
+        "nexuses",
+        "sinuses",
+        "buses",
+        "viruses",
+    },
+    "o-i": {
+        "alti",
+        "canti",
+        "crescendi",
+        "soprani",
+        "bassi",
+        "contralti",
+        "soli",
+        "tempi",
+    },
+    "-im": {
+        "cherubim",
+        "goyim",
+        "seraphim",
+    },
+    "o-os": {
+        "albinos",
+        "dynamos",
+        "guanos",
+        "lumbagos",
+        "photos",
+        "pianos",
+        "solos",
+        "archipelagos",
+        "embryos",
+        "infernos",
+        "magnetos",
+        "pros",
+        "armadillos",
+        "fiascos",
+        "jumbos",
+        "manifestos",
+        "quartos",
+        "commandos",
+        "generalissimos",
+        "medicos",
+        "rhinos",
+        "dittos",
+        "ghettos",
+        "lingos",
+        "octavos",
+        "stylos",
+    },
 }
```

### Comparing `flashback-2.1.0/flashback/formatting/locales/es.py` & `flashback-2.2.0/flashback/formatting/locales/es.py`

 * *Files 5% similar despite different names*

```diff
@@ -7,40 +7,65 @@
 - https://github.com/clips/pattern/blob/master/pattern/text/es/inflect.py
 """
 
 import regex
 
 
 # Prepositions are used in compound words
-PREPOSITIONS = set((
-    "antes", "durante", "de", "para",
-    "en", "detrás", "delante", "adelante",
-    "través", "arriba", "bajo", "abajo",
-    "después", "dentro", "adentro", "fuera", "afuera", "cerca",
-    "entre", "además", "excepto", "alrededor",
-    "encima", "debajo", "por encima", "por debajo",
-    "espalda", "desde", "con", "sin", "como",
-    "hasta", "listo", "vía",
-    "por"
-))
+PREPOSITIONS = {
+    "antes",
+    "durante",
+    "de",
+    "para",
+    "en",
+    "detrás",
+    "delante",
+    "adelante",
+    "través",
+    "arriba",
+    "bajo",
+    "abajo",
+    "después",
+    "dentro",
+    "adentro",
+    "fuera",
+    "afuera",
+    "cerca",
+    "entre",
+    "además",
+    "excepto",
+    "alrededor",
+    "encima",
+    "debajo",
+    "por encima",
+    "por debajo",
+    "espalda",
+    "desde",
+    "con",
+    "sin",
+    "como",
+    "hasta",
+    "listo",
+    "vía",
+    "por",
+}
 
 PLURAL_RULES = [
     # Indefinite articles and demonstratives
     (
         (r"^un$", "unos", None),
         (r"^una$", "unas", None),
         (r"^el$", "los", None),
         (r"^la$", "las", None),
         (r"^(est[oae])$", r"\1s", None),
         (r"^(es[oae])$", r"\1s", None),
         (r"^(algun[oa])$", r"\1s", None),
     ),
     # Possessive adjectives
-    (
-    ),
+    (),
     # Possessive pronouns
     (
         (r"^(mí(s|[oa]))$", r"\1s", None),
         (r"^(tu(s|y[oa]))$", r"\1s", None),
         (r"^(su(s|y[oa]))$", r"\1s", None),
         (r"^(nuestr[oa])$", r"\1s", None),
         (r"^(vuestr[oa])$", r"\1s", None),
@@ -77,32 +102,36 @@
     (
         (r"(a|e|i|o|u|é)$", r"\1s", None),
         (r"(á|é|í|ó|ú)$", r"\1es", None),
         (r"és$", "eses", None),
         (r"z$", "ces", None),
     ),
     # Assume that the plural takes -es
-    (
-        (r"$", "es", None),
-    )
+    ((r"$", "es", None),),
 ]
 
 # For performance, compile the regular expressions once:
 PLURAL_RULES = [[(regex.compile(r[0]), r[1], r[2]) for r in grp] for grp in PLURAL_RULES]
 
 # Suffix categories
 PLURAL_CATEGORIES = {
-    "uninflected": set((
-    )),
-    "uncountable": set((
-        "poesía", "vino", "café", "harina", "detergente",
-        "pimienta", "leche", "ketchup", "sangre", "política",
-    )),
-    "nationalities": set((
-    )),
+    "uninflected": set(),
+    "uncountable": {
+        "poesía",
+        "vino",
+        "café",
+        "harina",
+        "detergente",
+        "pimienta",
+        "leche",
+        "ketchup",
+        "sangre",
+        "política",
+    },
+    "nationalities": set(),
 }
 
 
 SINGULAR_RULES = [
     # Indefinite articles and demonstratives
     (
         (r"^unos$", "un", None),
@@ -110,16 +139,15 @@
         (r"^los$", "el", None),
         (r"^las$", "la", None),
         (r"^(est[oae])s$", r"\1", None),
         (r"^(es[oae])s$", r"\1", None),
         (r"^(algun[oa])s$", r"\1", None),
     ),
     # Possessive adjectives
-    (
-    ),
+    (),
     # Possessive pronouns
     (
         (r"^(mí(s|[oa]))s$", r"\1", None),
         (r"^(tu(s|y[oa]))s$", r"\1", None),
         (r"^(su(s|y[oa]))s$", r"\1", None),
         (r"^(nuestr[oa])s$", r"\1", None),
         (r"^(vuestr[oa])s$", r"\1", None),
@@ -149,29 +177,24 @@
         (r"ones$", "ón", None),
         (r"unes$", "ún", None),
         (r"eses$", "és", None),
         (r"(br|i|j|t|zn)es$", r"\1e", None),
         (r"(esis|isis|osis)$", r"\1", None),
     ),
     # Irregular inflections for common suffixes
-    (
-        (r"ces$", "z", None),
-    ),
+    ((r"ces$", "z", None),),
     # Assume that the plural takes -es
     (
         (r"es$", "", None),
         (r"s$", "", None),
-    )
+    ),
 ]
 
 # For performance, compile the regular expressions once:
 SINGULAR_RULES = [[(regex.compile(r[0]), r[1], r[2]) for r in grp] for grp in SINGULAR_RULES]
 
 # Suffix categories
 SINGULAR_CATEGORIES = {
-    "uninflected": set((
-    )),
-    "uncountable": set((
-    )),
-    "nationalities": set((
-    ))
+    "uninflected": set(),
+    "uncountable": set(),
+    "nationalities": set(),
 }
```

### Comparing `flashback-2.1.0/flashback/formatting/ordinalize.py` & `flashback-2.2.0/flashback/formatting/ordinalize.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-def ordinalize(number):
+def ordinalize(number: int) -> str:
     """
     Transforms a number to its ordinal representation.
 
     Since this method should be mostly used in logging messages, only English is supported.
 
     Examples:
         ```python
@@ -15,18 +15,18 @@
         #=> "3rd"
 
         ordinalize(144)
         #=> "144th"
         ```
 
     Params:
-        number (int): the number to transform to an ordinal number
+        number: the number to transform to an ordinal number
 
     Returns:
-        str: the number with the correct ordinal suffix
+        the number with the correct ordinal suffix
     """
     number = int(number)
 
     if number == 1:
         suffix = "st"
     elif number == 2:
         suffix = "nd"
```

### Comparing `flashback-2.1.0/flashback/formatting/oxford_join.py` & `flashback-2.2.0/flashback/iterating/flatten.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,46 +1,42 @@
-def oxford_join(iterable, sep=", ", couple_sep=" and ", last_sep=", and ", quotes=False):
+from __future__ import annotations
+
+from collections.abc import Iterable
+from typing import TypeVar
+
+T = TypeVar("T")
+
+
+def flatten(iterable: Iterable[T]) -> tuple[T, ...]:
     """
-    Joins a list of string to a comma-separated sentence in a more english fashion than the
-    builtin `.join()`.
+    Unpacks nested iterables into the root `iterable`.
 
     Examples:
         ```python
-        from flashback.formatting import oxford_join
-
-        oxford_join("A", "B")
-        #=> "A and B"
+        from flashback.iterating import flatten
 
-        oxford_join("A", "B", "C")
-        #=> "A, B, and C"
+        for item in flatten(["a", ["b", ["c", "d"]], "e"]):
+            print(item)
+        #=> "a"
+        #=> "b"
+        #=> "c"
+        #=> "d"
+        #=> "e"
 
-        oxford_join("A", "B", "C", last_sep=", or ")
-        #=> "A, B, or C"
+        assert flatten([1, {2, 3}, (4,), range(5, 6)]) == (1, 2, 3, 4, 5)
         ```
 
     Params:
-        iterable (Iterable<Any>): the sequence holding the items to join
-        sep (str): the separator used when there is more than two items in the iterable
-        couple_sep (str): the separator to use if there is only two items in the iterable
-        last_sep (str): the separator to use for the last two items of the iterable
-        quotes (bool): whether or not to add quotes around each item of the iterable
+        iterable: the iterable to flatten
 
     Returns:
-        str: the joined strings
+        the flattened iterable
     """
-    if len(iterable) == 0:
-        return ""
-
-    if quotes:
-        iterable = [f"\"{item}\"" for item in iterable]
-    else:
-        iterable = [str(item) for item in iterable]
-
-    if len(iterable) == 1:
-        return iterable[0]
-
-    if len(iterable) == 2:
-        return couple_sep.join(iterable)
-
-    enumeration = sep.join(iterable[:-1])
+    items = []
+    for item in iterable:
+        if isinstance(item, Iterable) and not isinstance(item, str):
+            for nested_item in flatten(item):
+                items.append(nested_item)  # noqa: PERF402
+        else:
+            items.append(item)
 
-    return f"{enumeration}{last_sep}{iterable[-1]}"
+    return tuple(items)
```

### Comparing `flashback-2.1.0/flashback/formatting/parameterize.py` & `flashback-2.2.0/flashback/formatting/parameterize.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,15 +1,19 @@
 import regex
 
 from .transliterate import transliterate
 
 
-CRE_PARAMETERIZE_NON_ALPHANUM = regex.compile(r"[^a-z0-9\-_]+", flags=regex.I)  # pylint: disable=no-member
+CRE_PARAMETERIZE_NON_ALPHANUM = regex.compile(
+    r"[^a-z0-9\-_]+",
+    flags=regex.IGNORECASE,
+)
 
-def parameterize(text, sep="-", keep_case=False):
+
+def parameterize(text: str, sep: str = "-", keep_case: bool = False) -> str:
     """
     Replaces special characters in a text so that it may be used as part of an URL.
 
     Internally, uses `flashback.formatting.transliterate` to replace any unicode
     character by its ASCII equivalent.
 
     Examples:
@@ -26,20 +30,20 @@
         #=> "http-host"
 
         parameterize("Redis Server", sep="/")
         #=> "redis/server"
         ```
 
     Params:
-        text (str): the text to transform
-        sep (str): the separator to use as replacement
-        keep_case (bool): whether or not to keep the input case
+        text: the text to transform
+        sep: the separator to use as replacement
+        keep_case: whether or not to keep the input case
 
     Returns:
-        str: the parameterized text
+        the parameterized text
     """
     text = transliterate(text)
 
     # Turn unwanted chars into a separator
     text = CRE_PARAMETERIZE_NON_ALPHANUM.sub(sep, text)
 
     if sep:
```

### Comparing `flashback-2.1.0/flashback/formatting/pascalize.py` & `flashback-2.2.0/flashback/formatting/pascalize.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,20 @@
+from __future__ import annotations
+
+from collections.abc import Iterable
+
 import regex
 
 from .camelize import camelize
 
 
 CRE_PASCALIZE = regex.compile(r"^(?:_{1,2}|)([a-z\d])(?:[a-z\d]+)")
 
-def pascalize(text, acronyms=None):
+
+def pascalize(text: str, acronyms: Iterable[str] | None = None) -> str:
     """
     Transforms a text in any case to PascalCase.
 
     Any character following a matched acronym will be capitalized.
 
     Examples:
         ```python
@@ -28,23 +33,23 @@
         #=> "HttphOst"
 
         pascalize("HTTPHost", acronyms=["HTTP"])
         #=> "HTTPHost"
         ```
 
     Params:
-        text (str): the text to transform into PascalCase
-        acronyms (Iterable): a list of correctly cased acronyms to retain and case correctly
+        text: the text to transform into PascalCase
+        acronyms: a list of correctly cased acronyms to retain and case correctly
 
     Returns:
-        str: the pascal cased text
+        the pascal cased text
     """
     text = camelize(text, acronyms=acronyms)
 
-    def replace(m):
+    def replace(m: regex.Match) -> str:
         group = m.group()
 
         if "_" in group:
             underscore_index = group.rindex("_") + 1
             return group[:underscore_index] + group[underscore_index:].capitalize()
 
         return group.capitalize()
```

### Comparing `flashback-2.1.0/flashback/formatting/pluralize.py` & `flashback-2.2.0/flashback/formatting/pluralize.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from ..i16g import Locale
 from ._inflect import _inflect
 
 
-def pluralize(word, language="en"):
+def pluralize(word: str, language: str = "en") -> str:
     """
     Returns the plural form of the given word.
 
     Examples:
         ```python
         from flashback.formatting import pluralize
 
@@ -17,30 +17,29 @@
         #=> "databases-as-a-service"
 
         pluralize("réseau", language="fr")
         #=> "réseaux"
         ```
 
     Params:
-        word (str): the word to pluralize
-        language (str): the language to use to pluralize the word (ISO 639-1)
+        word: the word to pluralize
+        language: the language to use to pluralize the word (ISO 639-1)
 
     Returns:
-        str: the pluralized word
+        the pluralized word
     """
     locale = Locale.load(language, path=".locales")
 
     # TODO: find a way to put that in _inflect
-    if language == "en":
-        if word.endswith(("'", "'s")):
-            sub_word = word.rstrip("s")
-            sub_word = sub_word.rstrip("'")
-            sub_word = pluralize(sub_word)
+    if language == "en" and word.endswith(("'", "'s")):
+        sub_word = word.rstrip("s")
+        sub_word = sub_word.rstrip("'")
+        sub_word = pluralize(sub_word)
 
-            if sub_word.endswith("s"):
-                return f"{sub_word}'"
+        if sub_word.endswith("s"):
+            return f"{sub_word}'"
 
-            return f"{sub_word}'s"
+        return f"{sub_word}'s"
 
     base_case = str.lower if language != "de" else str.capitalize
 
     return _inflect(word, locale.PLURAL_RULES, locale.PLURAL_CATEGORIES, locale.PREPOSITIONS, base_case=base_case)
```

### Comparing `flashback-2.1.0/flashback/formatting/singularize.py` & `flashback-2.2.0/flashback/formatting/singularize.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from ..i16g import Locale
 from ._inflect import _inflect
 
 
-def singularize(word, language="en"):
+def singularize(word: str, language: str = "en") -> str:
     """
     Returns the singular form of the given word.
 
     Examples:
         ```python
         from flashback.formatting import singularize
 
@@ -26,21 +26,20 @@
 
     Returns:
         str: the singularized word
     """
     locale = Locale.load(language, path=".locales")
 
     # TODO: find a way to put that in _inflect
-    if language == "en":
-        if word.endswith(("'", "'s")):
-            sub_word = word.rstrip("s")
-            sub_word = sub_word.rstrip("'")
-            sub_word = singularize(sub_word)
+    if language == "en" and word.endswith(("'", "'s")):
+        sub_word = word.rstrip("s")
+        sub_word = sub_word.rstrip("'")
+        sub_word = singularize(sub_word)
 
-            if sub_word.endswith("s"):
-                return f"{sub_word}'"
+        if sub_word.endswith("s"):
+            return f"{sub_word}'"
 
-            return f"{sub_word}'s"
+        return f"{sub_word}'s"
 
     base_case = str.lower if language != "de" else str.capitalize
 
     return _inflect(word, locale.SINGULAR_RULES, locale.SINGULAR_CATEGORIES, locale.PREPOSITIONS, base_case=base_case)
```

### Comparing `flashback-2.1.0/flashback/formatting/snakeize.py` & `flashback-2.2.0/flashback/formatting/snakeize.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,15 +1,20 @@
+from __future__ import annotations
+
+from collections.abc import Iterable
+
 import regex
 
 
 CRE_SNAKEIZE_CAPITAL_WORDS = regex.compile(r"([A-Z\d]+)([A-Z][a-z])")
 CRE_SNAKEIZE_LOWER_WORDS = regex.compile(r"([a-z\d])([A-Z])")
 CRE_SNAKEIZE_UNDERSCORES = regex.compile(r"(?<!^)_(?=_.)")
 
-def snakeize(text, acronyms=None):
+
+def snakeize(text: str, acronyms: Iterable[str] | None = None) -> str:
     """
     Transforms a text in any case to snake_case.
 
     Does not mutilate protected names (names prefixed with '_') and dunder_names (names surrounded
     by '__').
 
     Examples:
@@ -29,35 +34,35 @@
         #=> "httph_ost"
 
         snakeize("HTTPHost", acronyms=["HTTP"])
         #=> "http_host"
         ```
 
     Params:
-        text (str): the text to transform into snake_case
-        acronyms (Iterable): a list of acronyms to treat as non-delimited single lowercase words
+        text: the text to transform into snake_case
+        acronyms: a list of acronyms to treat as non-delimited single lowercase words
 
     Returns:
-        str: the snake cased text
+        the snake cased text
     """
     text = str(text)
 
     acronyms_pattern = r"(?=$)^" if acronyms is None else "|".join(acronyms)
     acronyms_snakeize_pattern = rf"({acronyms_pattern})"
 
-    for match in regex.finditer(acronyms_snakeize_pattern, text, flags=regex.I):  # pylint: disable=no-member
+    for match in regex.finditer(acronyms_snakeize_pattern, text, flags=regex.IGNORECASE):
         parts = []
 
-        start = text[:match.start()]
+        start = text[: match.start()]
         if start:
             parts.append(start)
 
         parts.append(match.group(1))
 
-        end = text[match.end():]
+        end = text[match.end() :]
         if end:
             parts.append(end)
 
         text = "_".join(parts)
 
     text = CRE_SNAKEIZE_CAPITAL_WORDS.sub(r"\1_\2", text)
     text = CRE_SNAKEIZE_LOWER_WORDS.sub(r"\1_\2", text)
```

### Comparing `flashback-2.1.0/flashback/formatting/transliterate.py` & `flashback-2.2.0/flashback/formatting/transliterate.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from unidecode import unidecode
 
 
-def transliterate(text, keep_case=True):
+def transliterate(text: str, keep_case: bool = True) -> str:
     """
     Replaces unicode characters with their ASCII equivalent using unidecode
     (https://pypi.org/project/Unidecode/).
 
     Examples:
         ```python
         from flashback.formatting import transliterate
@@ -17,19 +17,19 @@
         #=> omrezje
 
         transliterate("Omrežje", keep_case=True)
         #=> Omrezje
         ```
 
     Params:
-        text (str): the text to transform from unicode to ASCII
-        keep_case (bool): whether or not to keep the input case
+        text: the text to transform from unicode to ASCII
+        keep_case: whether or not to keep the input case
 
     Returns:
-        str: the text using only ASCII characters
+        the text using only ASCII characters
     """
     text = str(text)
     text = unidecode(text)
 
     if keep_case:
         return text
```

### Comparing `flashback-2.1.0/flashback/formatting/truncate.py` & `flashback-2.2.0/flashback/formatting/truncate.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-def truncate(text, limit=120, suffix="..."):
+def truncate(text: str, limit: int = 120, suffix: str = "...") -> str:
     """
     Truncates the given text up to `limit` and fill its ending with `suffix`.
 
     Tries to find the latest space before the `limit` which is located in the second half of the
     text. If no space is found, truncates at the limit. Searching for a space in the second-half
     of the text avoids cases where the word going over the limit is very long, e.g.:
 
@@ -29,25 +29,25 @@
         #=> "Wonderful tool to use, bla bla bla"
 
         truncate("Hi there", limit=3, suffix="")
         #=> "Hi"
         ```
 
     Params:
-        text (str): the text to truncate
-        limit (int): the maximum length of the text
-        suffix (str): the suffix to append at the truncated text
+        text: the text to truncate
+        limit: the maximum length of the text
+        suffix: the suffix to append at the truncated text
 
     Returns
-        str: the truncated text
+        the truncated text
     """
     if len(text) <= limit:
         return text
 
-    truncated_text = text[:(limit - len(suffix))]
+    truncated_text = text[: (limit - len(suffix))]
     try:
         space_index = truncated_text.rindex(" ")
     except ValueError:
         space_index = -1
 
     if space_index < limit // 2:
         space_index = -1
```

### Comparing `flashback-2.1.0/flashback/i16g/locale.py` & `flashback-2.2.0/flashback/i16g/locale.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,14 @@
-import inspect
-from importlib import util, import_module
+from __future__ import annotations
 
-import regex
+from importlib import util, import_module
+from types import ModuleType
+from typing import ClassVar
+import inspect
+import re
 
 from ..debugging import get_frameinfo
 
 
 class Locale:
     """
     Defines a generic loader that finds, imports, caches, and returns constants used for
@@ -20,16 +23,18 @@
         assert simple_locale == "fr_FR"
 
         locale = Locale.load(simple_locale, ".locales")
 
         assert locale is not None
         ```
     """
-    __cache = {}
-    CRE_LOCALE = regex.compile(r"""
+
+    __cache: ClassVar[dict[str, ModuleType]] = {}
+    CRE_LOCALE = re.compile(
+        r"""
             ^
             (?P<language>
                 [a-z]{2}
             )
             (?:
                 [-_]
                 (?P<territory>
@@ -44,18 +49,20 @@
                         @
                         (?P<modifier>
                             .+
                         )
                     )
                 )?
             )?
-        """, regex.I + regex.X)  # pylint: disable=no-member
+        """,
+        re.IGNORECASE + re.VERBOSE,
+    )
 
     @classmethod
-    def load(cls, locale, path):
+    def load(cls, locale: str, path: str) -> ModuleType:
         """
         Loads a `locale` definition from a package `path` and exposes its contents.
 
         If the `path` is relative, it is transformed to absolute using the call stack.
 
         Generates locales candidates to use as fallback, e.g.: 'en_US.UTF-8' will yield 'en_us' and
         'en'. Then tries to import from the most to the least precise ('en_us', then 'en') until it
@@ -79,19 +86,19 @@
             #=> Whatever defined in fr_FR
 
             Locale.load("not-implemented", "conf.production")
             #=> NotImplementedError
             ```
 
         Params:
-            locale (str): the given locale
-            path (str): the path in which to find the locale definition
+            locale: the given locale
+            path: the path in which to find the locale definition
 
         Returns:
-            Module: the content of the loaded locale
+            the content of the loaded locale
 
         Raises:
             NotImplementedError: if the given locale implementation is not found
         """
         locale = cls.simplify(locale)
 
         candidate_locales = sorted({locale, locale.split("_")[0]}, key=len, reverse=True)
@@ -121,15 +128,15 @@
                 return imported_locale
             except ImportError:
                 pass
 
         raise NotImplementedError(f"locale {locale!r} is not implemented in {module_path}")
 
     @classmethod
-    def simplify(cls, locale):
+    def simplify(cls, locale: str) -> str:
         """
         Returns a simplified locale code for the given `locale`.
 
         Returns the locale code formatted as LANGUAGE_TERRITORY (e.g. 'en_US.UTF-8' to 'en_us'), or
         LANGUAGE (e.g. 'EN' to 'en') if the territory was not specified in the given locale.
 
         If it fails to normalize, returns the original name unchanged.
@@ -148,18 +155,18 @@
             #=> "fr"
 
             Locale.simplify("not-a-locale")
             #=> "not-a-locale"
             ```
 
         Params:
-            locale (str): the non-normalized locale string
+            locale: the non-normalized locale string
 
         Returns:
-            str: the lowercased locale containing at least the language
+            the lowercased locale containing at least the language
         """
         match = cls.CRE_LOCALE.match(locale)
         if not match:
             return locale
 
         # A language must be there, else execution would have stopped above
         simplified_locale = match.group("language").lower()
```

### Comparing `flashback-2.1.0/flashback/importing/import_class_from_path.py` & `flashback-2.2.0/flashback/importing/import_class_from_path.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 import inspect
-
 from importlib import util, import_module
 
 from ..debugging import get_frameinfo
 from ..formatting import pascalize
 
 
-def import_class_from_path(name, path):
+def import_class_from_path(name: str, path: str) -> type:
     """
     Imports a class from a relative or absolute path, and returns it.
 
     Similar to `from module import Class` if this statement returned the imported class.
 
     Examples:
         ```python
@@ -18,19 +17,19 @@
 
         borg_class = import_class_from_path("borg", "flashback")
 
         borg_class()
         ```
 
     Paramss:
-        name (str): the name of the class to import
-        path (str): the relative path in which to find the class to import
+        name: the name of the class to import
+        path: the relative path in which to find the class to import
 
     Returns:
-        Callable: the class from the imported module
+        the class from the imported module
 
     Raises:
         ImportError: if the requested module is not found
         ImportError: if a relative import beyond the top-level package is attempted
         AttributeError: if the class is not found in the imported module
     """
     if path.startswith("."):
```

### Comparing `flashback-2.1.0/flashback/importing/import_module_from_path.py` & `flashback-2.2.0/flashback/importing/import_module_from_path.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import inspect
 
 from importlib import util, import_module
 
 from ..debugging import get_frameinfo
 
 
-def import_module_from_path(name, path):
+def import_module_from_path(name: str, path: str) -> None:
     """
     Imports the contents of a module from a relative or absolute path and makes its content
     available for usage.
 
     Simulates `from module import *`.
 
     Examples:
@@ -18,20 +18,20 @@
 
         import_module_from_path("logging", "flashback")
 
         print(DEFAULT_CONSOLE_CONFIGURATION)
         ```
 
     Params:
-        name (str): the name of the module to import
-        path (str): the relative path in which to find the module to import
+        name: the name of the module to import
+        path: the relative path in which to find the module to import
 
     Raises:
         ImportError: if a relative import beyond the top-level package is attempted
-        ImportError: if the request module is not found
+        ImportError: if the requested module is not found
     """
     if path.startswith("."):
         caller_module = inspect.getmodule(get_frameinfo(1).frame)
         caller_package = caller_module.__package__
 
         module_path = util.resolve_name(path, caller_package)
     else:
```

### Comparing `flashback-2.1.0/flashback/iterating/chunks.py` & `flashback-2.2.0/flashback/iterating/chunks.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,13 +1,19 @@
+from __future__ import annotations
+
+from collections.abc import Iterable, Generator
 from itertools import islice
+from typing import Any, TypeVar
 
 from ..sentinel import Sentinel
 
+T = TypeVar("T")
+
 
-def chunks(iterable, size=2, pad=Sentinel):
+def chunks(iterable: Iterable[T], size: int = 2, pad: Any = Sentinel) -> Generator[tuple[T, ...], None, None]:
     """
     Iterates over an `iterable` by chunks of `size`.
 
     Handles infinite iterables.
 
     Examples:
         ```python
@@ -27,24 +33,24 @@
         #=> 40
         #=> 65
         #=> 90
         #=> ...
         ```
 
     Params:
-        iterable (Iterable<Any>): the iterable to chunk
-        size (int): the size of the chunks to produce
+        iterable: the iterable to chunk
+        size: the size of the chunks to produce
 
     Yields:
-        tuple<Any>: the extracted chunk
+        the extracted chunk
     """
     iterable = iter(iterable)
     chunk_generator = iter(lambda: tuple(islice(iterable, size)), ())
     if pad is Sentinel:
         yield from chunk_generator
     else:
         for chunk in chunk_generator:
             len_diff = size - len(chunk)
             if len_diff > 0:
-                chunk += (pad,) * len_diff
-
-            yield chunk
+                yield chunk + (pad,) * len_diff
+            else:
+                yield chunk
```

### Comparing `flashback-2.1.0/flashback/iterating/compact.py` & `flashback-2.2.0/flashback/iterating/compact.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,8 +1,16 @@
-def compact(iterable):
+from __future__ import annotations
+
+from collections.abc import Iterable
+from typing import TypeVar
+
+T = TypeVar("T")
+
+
+def compact(iterable: Iterable[T]) -> tuple[T, ...]:
     """
     Removes None items from `iterable`.
 
     Examples:
         ```python
         from flashback.iterating import compact
 
@@ -11,13 +19,13 @@
         #=> 1058
         #=> 85
         #=> 9264
         #=> 19475
         ```
 
     Params:
-        iterable (Iterable<Any>): the iterable to remove None from
+        iterable: the iterable to remove None from
 
     Returns:
-        tuple<Any>: the iterable without duplicates
+        the iterable without duplicates
     """
     return tuple(item for item in iterable if item is not None)
```

### Comparing `flashback-2.1.0/flashback/iterating/flat_map.py` & `flashback-2.2.0/flashback/iterating/flat_map.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,15 +1,19 @@
 from __future__ import annotations
 
-from typing import Any, Callable, Sequence
+from collections.abc import Callable, Iterable
+from typing import TypeVar
 
 from .flatten import flatten
 
+T = TypeVar("T")
+U = TypeVar("U")
 
-def flat_map(func: Callable[[Any], Any], iterable: Sequence[Any]) -> map:
+
+def flat_map(func: Callable[[T], U], iterable: Iterable[T]) -> map[U]:
     """
     Applies the function `func` to each item and nested item of `iterable`.
 
     Examples:
         ```python
         from flashback.iterating import flat_map
```

### Comparing `flashback-2.1.0/flashback/iterating/uniq.py` & `flashback-2.2.0/flashback/iterating/uniq.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,13 +1,17 @@
 from __future__ import annotations
 
-from typing import Any, Iterable
+from collections.abc import Iterable
 
+from typing import TypeVar
 
-def uniq(iterable: Iterable[Any]) -> tuple[Any]:
+T = TypeVar("T")
+
+
+def uniq(iterable: Iterable[T]) -> tuple[T, ...]:
     """
     Removes duplicates items from `iterable` while keeping their order.
 
     Examples:
         ```python
         from flashback.iterating import uniq
```

### Comparing `flashback-2.1.0/flashback/iterating/uniq_by.py` & `flashback-2.2.0/flashback/iterating/uniq_by.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,17 @@
 from __future__ import annotations
 
-from typing import Any, Callable, Iterable, Tuple
+from collections.abc import Callable, Iterable
 
+from typing import Any, TypeVar
 
-def uniq_by(iterable: Iterable[Any], func: Callable[[Any], Any]) -> Tuple[Any, ...]:
+T = TypeVar("T")
+
+
+def uniq_by(func: Callable[[T], Any], iterable: Iterable[T]) -> tuple[T, ...]:
     """
     Removes duplicates items from `iterable` based on a callable `func`, while keeping their order.
 
     Examples:
         ```python
         from flashback.iterating import uniq_by
```

### Comparing `flashback-2.1.0/flashback/logging/__init__.py` & `flashback-2.2.0/flashback/logging/__init__.py`

 * *Files identical despite different names*

### Comparing `flashback-2.1.0/flashback/logging/affixed_stream_handler.py` & `flashback-2.2.0/flashback/logging/affixed_stream_handler.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,10 @@
+from __future__ import annotations
+
+from io import TextIOWrapper
 import logging
 
 
 class AffixedStreamHandler(logging.StreamHandler):
     """
     Implements a custom handler that adds customizable prefix and suffix to the formatted record.
 
@@ -55,46 +58,47 @@
 
         logger.info("info message")
 
         second_stream.getvalue()
         #=> "_START_info message_END_"
         ```
     """
-    def __init__(self, stream=None, prefix="", suffix="\n"):
+
+    def __init__(self, stream: TextIOWrapper | None = None, prefix: str = "", suffix: str = "\n") -> None:
         """
         If stream is not specified, sys.stderr is used.
 
         Params:
-            stream (TextIOWrapper): the stream to write to
-            prefix (str): the prefix to prepend to the record
-            suffix (str): the suffix to append to the record
+            stream: the stream to write to
+            prefix: the prefix to prepend to the record
+            suffix: the suffix to append to the record
         """
         super().__init__(stream=stream)
 
         self.prefix = prefix
         self.suffix = suffix
 
-    def emit(self, record):
+    def emit(self, record: logging.LogRecord) -> None:
         """
         Writes a record to the stream after formatting it and affixing it with the configured
         prefix and suffix.
 
         If exception information is present, it is formatted using traceback.print_exception
         and appended to the stream. If the stream has an `encoding` attribute, it is used to
         determine how to do the output to the stream.
 
         Params:
-            record (logging.LogRecord): the record to format and write
+            record: the record to format and write
 
         Raises:
             RecursionError: if the maximum recursion depth is reached
         """
         try:
             msg = self.format(record)
             stream = self.stream
             # issue 35046: merged two stream.writes into one.
             stream.write(self.prefix + msg + self.suffix)
             self.flush()
         except RecursionError:  # See issue 36272
             raise
-        except Exception:  # pylint: disable=broad-except
+        except Exception:  # noqa: BLE001
             self.handleError(record)
```

### Comparing `flashback-2.1.0/flashback/logging/configurations.py` & `flashback-2.2.0/flashback/logging/configurations.py`

 * *Files 9% similar despite different names*

```diff
@@ -12,46 +12,43 @@
 ```python
 from flashback.logging import DEFAULT_CONSOLE_CONFIGURATION
 ```
 
 `disable_existing_loggers` is set to false for each configuration because it breaks the loggers
 created after using the configuration (see: https://gist.github.com/alanbriolat/d5ffe608b56c948533c6).
 """
+
 import inspect
 
 from ..debugging import get_frameinfo
 
 try:
     IMPORTER = inspect.getmodule(get_frameinfo(12).frame).__package__ or None
 except (IndexError, AttributeError):
     IMPORTER = None
 
 DEFAULT_CONSOLE_CONFIGURATION = {
     "version": 1,
     "disable_existing_loggers": False,
     "incremental": False,
-    "formatters": {
-        "default": {
-            "format": "%(asctime)s - %(name)s - %(processName)s - %(levelname)s - %(message)s"
-        }
-    },
+    "formatters": {"default": {"format": "%(asctime)s - %(name)s - %(processName)s - %(levelname)s - %(message)s"}},
     "filters": {},
     "handlers": {
         "console": {
             "level": "DEBUG",
             "class": "logging.StreamHandler",
-            "formatter": "default"
-        }
+            "formatter": "default",
+        },
     },
     "loggers": {
         IMPORTER: {
             "level": "DEBUG",
-            "handlers": ["console"]
-        }
-    }
+            "handlers": ["console"],
+        },
+    },
 }
 """
 A simple logger applicable for most logging context.
 
 Logs to stderr without filtering, and formats the message with `asctime`, `name`, `processName`,
 `levelname`, and `message`.
 """
@@ -62,83 +59,50 @@
     "incremental": False,
     "formatters": {},
     "filters": {},
     "handlers": {
         "console": {
             "level": "DEBUG",
             "class": "logging.StreamHandler",
-        }
+        },
     },
-    "loggers": {
-        IMPORTER: {
-            "level": "DEBUG",
-            "handlers": ["console"]
-        }
-    }
+    "loggers": {IMPORTER: {"level": "DEBUG", "handlers": ["console"]}},
 }
 """
 A Django-like logger (which basically does nothing).
 
 Logs to stderr without filtering, and formats the message with the default logging formatter.
 """
 
 FLASK_CONSOLE_CONFIGURATION = {
     "version": 1,
     "disable_existing_loggers": False,
     "incremental": False,
-    "formatters": {
-        "default": {
-            "format": "[%(asctime)s] %(levelname)s in %(module)s: %(message)s"
-        }
-    },
+    "formatters": {"default": {"format": "[%(asctime)s] %(levelname)s in %(module)s: %(message)s"}},
     "filters": {},
-    "handlers": {
-        "console": {
-            "level": "DEBUG",
-            "class": "logging.StreamHandler",
-            "formatter": "default"
-        }
-    },
-    "loggers": {
-        IMPORTER: {
-            "level": "DEBUG",
-            "handlers": ["console"]
-        }
-    }
+    "handlers": {"console": {"level": "DEBUG", "class": "logging.StreamHandler", "formatter": "default"}},
+    "loggers": {IMPORTER: {"level": "DEBUG", "handlers": ["console"]}},
 }
 """
 A Flask-like logger.
 
 Logs to stderr without filtering, and formats the message with `asctime`, `levelname`, `module`,
 and `message`.
 """
 
 PYRAMID_CONSOLE_CONFIGURATION = {
     "version": 1,
     "disable_existing_loggers": False,
     "incremental": False,
     "formatters": {
-        "default": {
-            "format": "%(asctime)s %(levelname)-5.5s [%(name)s:%(lineno)s][%(threadName)s] %(message)s"
-        }
+        "default": {"format": "%(asctime)s %(levelname)-5.5s [%(name)s:%(lineno)s][%(threadName)s] %(message)s"},
     },
     "filters": {},
-    "handlers": {
-        "console": {
-            "level": "DEBUG",
-            "class": "logging.StreamHandler",
-            "formatter": "default"
-        }
-    },
-    "loggers": {
-        IMPORTER: {
-            "level": "DEBUG",
-            "handlers": ["console"]
-        }
-    }
+    "handlers": {"console": {"level": "DEBUG", "class": "logging.StreamHandler", "formatter": "default"}},
+    "loggers": {IMPORTER: {"level": "DEBUG", "handlers": ["console"]}},
 }
 """
 A Pyramid-like logger.
 
 Logs to stderr without filtering, and formats the message with `asctime`, `levelname`, `name`,
 `lineno`, `threadName`, and `message`.
 """
@@ -146,31 +110,20 @@
 RAILS_CONSOLE_CONFIGURATION = {
     "version": 1,
     "disable_existing_loggers": False,
     "incremental": False,
     "formatters": {
         "default": {
             "format": "%(levelname)1.1s, [%(asctime)s.%(msecs)03d #%(process)d] %(levelname)8s -- : %(message)s",
-            "datefmt": "%Y-%m-%dT%H:%M:%S"
-        }
+            "datefmt": "%Y-%m-%dT%H:%M:%S",
+        },
     },
     "filters": {},
-    "handlers": {
-        "console": {
-            "level": "DEBUG",
-            "class": "logging.StreamHandler",
-            "formatter": "default"
-        }
-    },
-    "loggers": {
-        IMPORTER: {
-            "level": "DEBUG",
-            "handlers": ["console"]
-        }
-    }
+    "handlers": {"console": {"level": "DEBUG", "class": "logging.StreamHandler", "formatter": "default"}},
+    "loggers": {IMPORTER: {"level": "DEBUG", "handlers": ["console"]}},
 }
 """
 A Ruby-on-Rails-like logger.
 
 Logs to stderr without filtering, and formats the message with `asctime`, `msec`, `process`,
 `levelname`, and `message`.
 """
```

### Comparing `flashback-2.1.0/flashback/logging/muted.py` & `flashback-2.2.0/flashback/logging/muted.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,17 @@
+from __future__ import annotations
+
+from collections.abc import Iterable, Callable
+
 import functools
 import logging
 from logging import getLogger, Logger
 
 
-def muted(loggers=None):
+def muted(loggers: Iterable[str | Logger] | None = None) -> Callable:
     """
     Mutes all (or selected) loggers while executing a callable.
 
     By default, mute all loggers.
 
     Use 'None' as name for the root logger.
 
@@ -47,28 +51,29 @@
             how_logger.info("How are you?")
             bye_logger.info("Bye")
 
         muted_greetings()
         ```
 
     Params:
-        loggers (Iterable<str|logging.Logger>): the list of logger names or instances to mute
+        loggers: the list of logger names or instances to mute
 
     Returns:
-        Callable: a wrapper used to decorate a callable
+        a wrapper used to decorate a callable
     """
+
     def wrapper(func):
         def _filter(_record):
             return False
 
         @functools.wraps(func)
         def inner(*args, **kwargs):
             # Selects all loggers at each call to func because loggers can be created between calls
             if loggers is None:
-                selected_loggers = [getLogger(logger) for logger in logging.root.manager.loggerDict] + [logging.root] # pylint: disable=no-member
+                selected_loggers = [getLogger(logger) for logger in logging.root.manager.loggerDict] + [logging.root]
             else:
                 selected_loggers = [logger if isinstance(logger, Logger) else getLogger(logger) for logger in loggers]
 
             for logger in selected_loggers:
                 logger.addFilter(_filter)
 
             result = func(*args, **kwargs)
```

### Comparing `flashback-2.1.0/flashback/retryable.py` & `flashback-2.2.0/flashback/retryable.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,25 @@
+from __future__ import annotations
+
+from collections.abc import Callable
 import functools
 import inspect
 import logging
 import math
 import time
 
 from .formatting import ordinalize
 
 
-def retryable(max_retries=-1, plateau_after=10, reset_after=3600, exceptions=()):
+def retryable(
+    max_retries: int = -1,
+    plateau_after: int = 10,
+    reset_after: int = 3600,
+    exceptions: tuple[Exception, ...] = (),
+) -> Callable:
     """
     Retries to call a callable when a given exception is raised.
 
     The back-off starts at 0s and ends up at 60s after 10 retries:
     ```python
     0.15, 0.70, 1.65, 3.30, 6.15, 11.09, 19.63, 34.41, 60.0
     ```
@@ -43,22 +51,23 @@
         #=> Retrying for the 4th time in 3.30s
         #=> Caught TypeError
         #=> Retrying for the 5th time in 6.15s
         #=> ...
         ```
 
     Params:
-        max_retries (int): the max number of retries before raising the initial error
-        plateau_after (int): the number of retries after which to plateau the delay
-        reset_after (int): the number of seconds after which to reset the delay
-        exceptions (tuple<Exception>): the exceptions to trigger a retry on
+        max_retries: the max number of retries before raising the initial error
+        plateau_after: the number of retries after which to plateau the delay
+        reset_after: the number of seconds after which to reset the delay
+        exceptions: the exceptions to trigger a retry on
 
     Returns :
-        Callable: a wrapper used to decorate a callable
+        a wrapper used to decorate a callable
     """
+
     def wrapper(func):
         # `.getmodule().__name__` returns the same value as `__name__` called from the module we
         # decorate.
         # Since `logging` is a singleton, everytime we call `logging.getLogger()` with the same
         # name, we receive the same logger, which "hides" this decorator as if the logging was
         # made from within the callable we decorate
         logger = logging.getLogger(inspect.getmodule(func).__name__)
```

### Comparing `flashback-2.1.0/flashback/sampled.py` & `flashback-2.2.0/flashback/sampled.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,16 +1,19 @@
-import functools
+from __future__ import annotations
+
+from collections.abc import Callable
 from queue import Queue
+import functools
 import random
 import time
 
 from .formatting import oxford_join
 
 
-class sampled:  # pylint: disable=invalid-name
+class sampled:  # noqa: N801
     """
     Implements a way of sampling requests made to a callable.
 
     Currently implements three strategies:
 
     - constant
         - All calls are accepted (rate=0) or refused (rate=1) (default: 1)
@@ -56,24 +59,25 @@
             print("Called")
 
         decorated()
         decorated()
         #=> Called
         ```
     """
+
     STRATEGY_CONSTANT = "constant"
     STRATEGY_PROBABILISTIC = "probabilistic"
     STRATEGY_RATELIMITING = "ratelimiting"
     STRATEGIES = (
         STRATEGY_CONSTANT,
         STRATEGY_PROBABILISTIC,
         STRATEGY_RATELIMITING,
     )
 
-    def __init__(self, strategy="constant", rate=None):
+    def __init__(self, strategy: str = "constant", rate: float | None = None) -> None:
         """
         Params:
             strategy (str): the sampling strategy to use
             rate (int|float): the parameter to fine-tune the sampling strategy
         """
         if strategy == self.STRATEGY_CONSTANT:
             if rate is None:
@@ -103,28 +107,28 @@
             self._queue = Queue(maxsize=0)
 
             self.should_sample = self._sample_ratelimiting
         else:
             strategies_choices = oxford_join(self.STRATEGIES, last_sep=", or ")
             raise ValueError(f"invalid strategy {strategy!r}, expecting {strategies_choices}")
 
-    def __call__(self, func):
+    def __call__(self, func: Callable) -> Callable:
         @functools.wraps(func)
         def inner(*args, **kwargs):
             return func(*args, **kwargs) if self.should_sample() else None
 
         return inner
 
-    def _sample_constant(self):
+    def _sample_constant(self) -> float | None:
         return self._rate
 
-    def _sample_probabilistic(self):
+    def _sample_probabilistic(self) -> bool:
         return random.random() < self._rate
 
-    def _sample_ratelimiting(self):
+    def _sample_ratelimiting(self) -> bool:
         now = int(time.time())
 
         queue_size = self._queue.qsize()
         last_second = now - 1
         total_requests = 0
         for timestamp_index, timestamp in enumerate(self._queue.queue):
             if timestamp >= last_second:
```

### Comparing `flashback-2.1.0/flashback/sentinel.py` & `flashback-2.2.0/flashback/sentinel.py`

 * *Files 1% similar despite different names*

```diff
@@ -26,9 +26,10 @@
             print(item)
         #=> "abc"
         #=> None
         #=> "xyz"
         #=> StopIteration
         ```
     """
+
     def __new__(cls):
         return cls
```

### Comparing `flashback-2.1.0/flashback/singleton.py` & `flashback-2.2.0/flashback/singleton.py`

 * *Files 4% similar despite different names*

```diff
@@ -38,15 +38,16 @@
 
         assert loose_logger_1 == loose_logger_2
         assert loose_logger_1 is loose_logger_2
 
         assert logger_1 != loose_logger_1
         ```
     """
-    def __new__(mcs, name, bases, namespace, **_kwargs):
+
+    def __new__(mcs, name, bases, namespace, **_kwargs):  # noqa: N804 mcs = metaclass
         return super().__new__(mcs, name, bases, namespace)
 
     def __init__(cls, name, bases, attributes, strict=True):
         """
         Params:
             name (str): the name of the class to initialize
             bases (tuple): the bases classes of the class
@@ -56,15 +57,15 @@
         super().__init__(name, bases, attributes)
 
         cls.strict = strict
         cls._instances = {}
 
     def __call__(cls, *args, **kwargs):
         if cls.strict:
-            key = functools._make_key(args, kwargs, True)  # pylint: disable=protected-access
+            key = functools._make_key(args, kwargs, True)  # noqa: SLF001
         else:
             key = 0
 
         instance = cls._instances.get(key, None)
         if instance is None:
             instance = super().__call__(*args, **kwargs)
```

### Comparing `flashback-2.1.0/flashback/timed.py` & `flashback-2.2.0/flashback/timed.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,14 +1,15 @@
+from collections.abc import Callable
 import functools
 import inspect
 import logging
 import time
 
 
-def timed(func):
+def timed(func: Callable) -> Callable:
     """
     Logs the start and end of a function call, and records the time spent executing it.
 
     Examples:
         ```python
         from flashback import timed
 
@@ -19,18 +20,18 @@
         printer()
         #=> Started execution of printer
         #=> Executing
         #=> Completed execution of printer after 2.47955322265625e-05s
         ```
 
     Params:
-        func (Callable): the callable to time
+        func: the callable to time
 
     Returns:
-        Callable: a wrapper used to decorate a callable
+        a wrapper used to decorate a callable
     """
     # `.getmodule().__name__` returns the same value as `__name__` called from the module we
     # decorate.
     # Since `logging` is a singleton, everytime we call `logging.getLogger()` with the same
     # name, we receive the same logger, which "hides" this decorator as if the logging was
     # made from within the callable we decorate
     logger = logging.getLogger(inspect.getmodule(func).__name__)
```

### Comparing `flashback-2.1.0/flashback/timeoutable.py` & `flashback-2.2.0/flashback/timeoutable.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import functools
+from collections.abc import Callable
 import signal
 
 
-def timeoutable(seconds=5, message="execution timed out"):
+def timeoutable(seconds: int = 5, message: str = "execution timed out") -> Callable:
     """
     Times out a callable's execution if its runtime exceeds `seconds`.
 
     Examples:
         ```python
         import time
         from flashback import timeoutable
@@ -27,23 +28,24 @@
             return True
 
         slow()
         #=> TimeoutError: Execution timed out
         ```
 
     Params:
-        seconds (int): the number of seconds to wait before timing out
-        message (str): the custom message to display when timing out
+        seconds: the number of seconds to wait before timing out
+        message: the custom message to display when timing out
 
     Return:
-        Callable: a wrapper used to decorate a callable
+        a wrapper used to decorate a callable
 
     Raises:
         TimeoutError: if the callable's execution time is longer than `seconds`
     """
+
     def wrapper(func):
         def _sigalrm_handler(_signum, _frame):
             raise TimeoutError(message)
 
         @functools.wraps(func)
         def inner(*args, **kwargs):
             signal.signal(signal.SIGALRM, _sigalrm_handler)
```

### Comparing `flashback-2.1.0/flashback.egg-info/PKG-INFO` & `flashback-2.2.0/flashback.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flashback
-Version: 2.1.0
+Version: 2.2.0
 Summary: An utility library for python
 Home-page: https://github.com/PaulRenvoise/flashback
 Author: Paul Renvoisé
 Author-email: renvoisepaul@gmail.com
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
@@ -121,15 +121,15 @@
 The Pull Request template has a checklist containing everything you need to submit a new PR.
 
 Run the tests with `pytest`:
 ```bash
 pytest tests
 ```
 
-Run the lint with `pylint`:
+Run the lint with `ruff`:
 ```bash
-pylint flashback/ tests/
+ruff check flashback tests
 ```
 
 ## License
 
 Flashback is released under the [MIT License](https://tldrlegal.com/license/mit-license#summary).
```

### Comparing `flashback-2.1.0/flashback.egg-info/SOURCES.txt` & `flashback-2.2.0/flashback.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 CHANGELOG.md
 LICENSE
 MANIFEST.in
 README.md
+pyproject.toml
 requirements-dev.txt
 requirements-test.txt
 requirements.txt
 setup.py
 flashback/__init__.py
 flashback/borg.py
 flashback/classproperty.py
```

### Comparing `flashback-2.1.0/setup.py` & `flashback-2.2.0/setup.py`

 * *Files identical despite different names*

