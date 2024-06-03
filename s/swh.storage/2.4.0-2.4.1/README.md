# Comparing `tmp/swh_storage-2.4.0.tar.gz` & `tmp/swh_storage-2.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "swh_storage-2.4.0.tar", last modified: Thu May 23 13:05:40 2024, max compression
+gzip compressed data, was "swh_storage-2.4.1.tar", last modified: Mon Jun  3 13:12:34 2024, max compression
```

## Comparing `swh_storage-2.4.0.tar` & `swh_storage-2.4.1.tar`

### file list

```diff
@@ -1,402 +1,404 @@
-drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-05-23 13:05:40.973009 swh_storage-2.4.0/
--rw-r--r--   0 jenkins    (115) jenkins    (120)      352 2024-05-23 13:05:35.000000 swh_storage-2.4.0/.copier-answers.yml
--rw-r--r--   0 jenkins    (115) jenkins    (120)      158 2024-05-23 13:05:35.000000 swh_storage-2.4.0/.git-blame-ignore-revs
--rw-r--r--   0 jenkins    (115) jenkins    (120)      356 2024-05-23 13:05:35.000000 swh_storage-2.4.0/.gitignore
--rw-r--r--   0 jenkins    (115) jenkins    (120)     1453 2024-05-23 13:05:35.000000 swh_storage-2.4.0/.pre-commit-config.yaml
--rw-r--r--   0 jenkins    (115) jenkins    (120)      112 2024-05-23 13:05:35.000000 swh_storage-2.4.0/AUTHORS
--rw-r--r--   0 jenkins    (115) jenkins    (120)     3397 2024-05-23 13:05:35.000000 swh_storage-2.4.0/CODE_OF_CONDUCT.md
--rw-r--r--   0 jenkins    (115) jenkins    (120)       61 2024-05-23 13:05:35.000000 swh_storage-2.4.0/CONTRIBUTORS
--rw-r--r--   0 jenkins    (115) jenkins    (120)    35147 2024-05-23 13:05:35.000000 swh_storage-2.4.0/LICENSE
--rw-r--r--   0 jenkins    (115) jenkins    (120)      163 2024-05-23 13:05:35.000000 swh_storage-2.4.0/Makefile
--rw-r--r--   0 jenkins    (115) jenkins    (120)       72 2024-05-23 13:05:35.000000 swh_storage-2.4.0/Makefile.local
--rw-r--r--   0 jenkins    (115) jenkins    (120)     8493 2024-05-23 13:05:40.973009 swh_storage-2.4.0/PKG-INFO
--rw-r--r--   0 jenkins    (115) jenkins    (120)     6270 2024-05-23 13:05:35.000000 swh_storage-2.4.0/README.rst
-drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-05-23 13:05:40.897010 swh_storage-2.4.0/bin/
--rwxr-xr-x   0 jenkins    (115) jenkins    (120)     1240 2024-05-23 13:05:35.000000 swh_storage-2.4.0/bin/swh-storage-add-dir
--rw-r--r--   0 jenkins    (115) jenkins    (120)      294 2024-05-23 13:05:35.000000 swh_storage-2.4.0/conftest.py
-drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-05-23 13:05:40.897010 swh_storage-2.4.0/docs/
--rw-r--r--   0 jenkins    (115) jenkins    (120)       24 2024-05-23 13:05:35.000000 swh_storage-2.4.0/docs/.gitignore
--rw-r--r--   0 jenkins    (115) jenkins    (120)       48 2024-05-23 13:05:35.000000 swh_storage-2.4.0/docs/Makefile
--rw-r--r--   0 jenkins    (115) jenkins    (120)      530 2024-05-23 13:05:35.000000 swh_storage-2.4.0/docs/Makefile.local
-drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-05-23 13:05:40.901010 swh_storage-2.4.0/docs/_static/
--rw-r--r--   0 jenkins    (115) jenkins    (120)        0 2024-05-23 13:05:35.000000 swh_storage-2.4.0/docs/_static/.placeholder
-drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-05-23 13:05:40.901010 swh_storage-2.4.0/docs/_templates/
--rw-r--r--   0 jenkins    (115) jenkins    (120)        0 2024-05-23 13:05:35.000000 swh_storage-2.4.0/docs/_templates/.placeholder
--rw-r--r--   0 jenkins    (115) jenkins    (120)     2206 2024-05-23 13:05:35.000000 swh_storage-2.4.0/docs/archive-copies.rst
--rw-r--r--   0 jenkins    (115) jenkins    (120)      143 2024-05-23 13:05:35.000000 swh_storage-2.4.0/docs/cli.rst
--rw-r--r--   0 jenkins    (115) jenkins    (120)       43 2024-05-23 13:05:35.000000 swh_storage-2.4.0/docs/conf.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)    12947 2024-05-23 13:05:35.000000 swh_storage-2.4.0/docs/extrinsic-metadata-specification.rst
-drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-05-23 13:05:40.901010 swh_storage-2.4.0/docs/images/
--rw-r--r--   0 jenkins    (115) jenkins    (120)       12 2024-05-23 13:05:35.000000 swh_storage-2.4.0/docs/images/.gitignore
--rw-r--r--   0 jenkins    (115) jenkins    (120)      335 2024-05-23 13:05:35.000000 swh_storage-2.4.0/docs/images/Makefile
--rw-r--r--   0 jenkins    (115) jenkins    (120)     3031 2024-05-23 13:05:35.000000 swh_storage-2.4.0/docs/images/swh-archive-copies.dia
--rw-r--r--   0 jenkins    (115) jenkins    (120)     2843 2024-05-23 13:05:35.000000 swh_storage-2.4.0/docs/index.rst
--rw-r--r--   0 jenkins    (115) jenkins    (120)     3772 2024-05-23 13:05:35.000000 swh_storage-2.4.0/docs/object-masking.rst
--rw-r--r--   0 jenkins    (115) jenkins    (120)      268 2024-05-23 13:05:35.000000 swh_storage-2.4.0/docs/sql-storage.rst
--rw-r--r--   0 jenkins    (115) jenkins    (120)     1097 2024-05-23 13:05:35.000000 swh_storage-2.4.0/mypy.ini
--rw-r--r--   0 jenkins    (115) jenkins    (120)     2852 2024-05-23 13:05:35.000000 swh_storage-2.4.0/pyproject.toml
--rw-r--r--   0 jenkins    (115) jenkins    (120)      458 2024-05-23 13:05:35.000000 swh_storage-2.4.0/pytest.ini
--rw-r--r--   0 jenkins    (115) jenkins    (120)       19 2024-05-23 13:05:35.000000 swh_storage-2.4.0/requirements-swh-journal.txt
--rw-r--r--   0 jenkins    (115) jenkins    (120)       94 2024-05-23 13:05:35.000000 swh_storage-2.4.0/requirements-swh.txt
--rw-r--r--   0 jenkins    (115) jenkins    (120)      406 2024-05-23 13:05:35.000000 swh_storage-2.4.0/requirements-test.txt
--rw-r--r--   0 jenkins    (115) jenkins    (120)      189 2024-05-23 13:05:35.000000 swh_storage-2.4.0/requirements.txt
--rw-r--r--   0 jenkins    (115) jenkins    (120)      120 2024-05-23 13:05:40.973009 swh_storage-2.4.0/setup.cfg
-drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-05-23 13:05:40.901010 swh_storage-2.4.0/sql/
--rw-r--r--   0 jenkins    (115) jenkins    (120)       26 2024-05-23 13:05:35.000000 swh_storage-2.4.0/sql/.gitignore
--rw-r--r--   0 jenkins    (115) jenkins    (120)     1565 2024-05-23 13:05:35.000000 swh_storage-2.4.0/sql/Makefile
--rw-r--r--   0 jenkins    (115) jenkins    (120)     1094 2024-05-23 13:05:35.000000 swh_storage-2.4.0/sql/TODO
-drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-05-23 13:05:40.901010 swh_storage-2.4.0/sql/bin/
--rwxr-xr-x   0 jenkins    (115) jenkins    (120)     1701 2024-05-23 13:05:35.000000 swh_storage-2.4.0/sql/bin/db-upgrade
--rwxr-xr-x   0 jenkins    (115) jenkins    (120)      538 2024-05-23 13:05:35.000000 swh_storage-2.4.0/sql/bin/dot_add_content
--rw-r--r--   0 jenkins    (115) jenkins    (120)     2023 2024-05-23 13:05:35.000000 swh_storage-2.4.0/sql/clusters.dot
-drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-05-23 13:05:40.889010 swh_storage-2.4.0/sql/doc/
-drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-05-23 13:05:40.905010 swh_storage-2.4.0/sql/json/
--rw-r--r--   0 jenkins    (115) jenkins    (120)        8 2024-05-23 13:05:35.000000 swh_storage-2.4.0/sql/json/.gitignore
--rw-r--r--   0 jenkins    (115) jenkins    (120)      283 2024-05-23 13:05:35.000000 swh_storage-2.4.0/sql/json/Makefile
--rw-r--r--   0 jenkins    (115) jenkins    (120)      223 2024-05-23 13:05:35.000000 swh_storage-2.4.0/sql/json/entity.lister_metadata.schema.json
--rw-r--r--   0 jenkins    (115) jenkins    (120)      129 2024-05-23 13:05:35.000000 swh_storage-2.4.0/sql/json/entity.metadata.schema.json
--rw-r--r--   0 jenkins    (115) jenkins    (120)      223 2024-05-23 13:05:35.000000 swh_storage-2.4.0/sql/json/entity_history.lister_metadata.schema.json
--rw-r--r--   0 jenkins    (115) jenkins    (120)      137 2024-05-23 13:05:35.000000 swh_storage-2.4.0/sql/json/entity_history.metadata.schema.json
--rw-r--r--   0 jenkins    (115) jenkins    (120)      631 2024-05-23 13:05:35.000000 swh_storage-2.4.0/sql/json/fetch_history.result.schema.json
--rw-r--r--   0 jenkins    (115) jenkins    (120)      133 2024-05-23 13:05:35.000000 swh_storage-2.4.0/sql/json/list_history.result.schema.json
--rw-r--r--   0 jenkins    (115) jenkins    (120)      141 2024-05-23 13:05:35.000000 swh_storage-2.4.0/sql/json/listable_entity.list_params.schema.json
--rw-r--r--   0 jenkins    (115) jenkins    (120)      632 2024-05-23 13:05:35.000000 swh_storage-2.4.0/sql/json/origin_visit.metadata.json
--rw-r--r--   0 jenkins    (115) jenkins    (120)      252 2024-05-23 13:05:35.000000 swh_storage-2.4.0/sql/json/tool.tool_configuration.schema.json
-drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-05-23 13:05:40.889010 swh_storage-2.4.0/swh/
-drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-05-23 13:05:40.909010 swh_storage-2.4.0/swh/storage/
--rw-r--r--   0 jenkins    (115) jenkins    (120)     3478 2024-05-23 13:05:35.000000 swh_storage-2.4.0/swh/storage/__init__.py
-drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-05-23 13:05:40.909010 swh_storage-2.4.0/swh/storage/algos/
--rw-r--r--   0 jenkins    (115) jenkins    (120)        0 2024-05-23 13:05:35.000000 swh_storage-2.4.0/swh/storage/algos/__init__.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)    16246 2024-05-23 13:05:35.000000 swh_storage-2.4.0/swh/storage/algos/diff.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)    12947 2024-05-23 13:05:35.000000 swh_storage-2.4.0/swh/storage/algos/dir_iterators.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     3468 2024-05-23 13:05:35.000000 swh_storage-2.4.0/swh/storage/algos/directory.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     1487 2024-05-23 13:05:35.000000 swh_storage-2.4.0/swh/storage/algos/discovery.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     3280 2024-05-23 13:05:35.000000 swh_storage-2.4.0/swh/storage/algos/origin.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)    19935 2024-05-23 13:05:35.000000 swh_storage-2.4.0/swh/storage/algos/revisions_walker.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     6541 2024-05-23 13:05:35.000000 swh_storage-2.4.0/swh/storage/algos/snapshot.py
-drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-05-23 13:05:40.909010 swh_storage-2.4.0/swh/storage/api/
--rw-r--r--   0 jenkins    (115) jenkins    (120)        0 2024-05-23 13:05:35.000000 swh_storage-2.4.0/swh/storage/api/__init__.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     2051 2024-05-23 13:05:35.000000 swh_storage-2.4.0/swh/storage/api/client.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     4512 2024-05-23 13:05:35.000000 swh_storage-2.4.0/swh/storage/api/serializers.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     5403 2024-05-23 13:05:35.000000 swh_storage-2.4.0/swh/storage/api/server.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)    20586 2024-05-23 13:05:35.000000 swh_storage-2.4.0/swh/storage/backfill.py
-drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-05-23 13:05:40.913010 swh_storage-2.4.0/swh/storage/cassandra/
--rw-r--r--   0 jenkins    (115) jenkins    (120)      375 2024-05-23 13:05:35.000000 swh_storage-2.4.0/swh/storage/cassandra/__init__.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)      516 2024-05-23 13:05:35.000000 swh_storage-2.4.0/swh/storage/cassandra/common.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     5919 2024-05-23 13:05:35.000000 swh_storage-2.4.0/swh/storage/cassandra/converters.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)    62367 2024-05-23 13:05:35.000000 swh_storage-2.4.0/swh/storage/cassandra/cql.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)    10766 2024-05-23 13:05:35.000000 swh_storage-2.4.0/swh/storage/cassandra/model.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     9301 2024-05-23 13:05:35.000000 swh_storage-2.4.0/swh/storage/cassandra/schema.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)    86844 2024-05-23 13:05:35.000000 swh_storage-2.4.0/swh/storage/cassandra/storage.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)    14670 2024-05-23 13:05:35.000000 swh_storage-2.4.0/swh/storage/cli.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)      496 2024-05-23 13:05:35.000000 swh_storage-2.4.0/swh/storage/common.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     4056 2024-05-23 13:05:35.000000 swh_storage-2.4.0/swh/storage/exc.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     2010 2024-05-23 13:05:35.000000 swh_storage-2.4.0/swh/storage/fixer.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)    31355 2024-05-23 13:05:35.000000 swh_storage-2.4.0/swh/storage/in_memory.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)    58274 2024-05-23 13:05:35.000000 swh_storage-2.4.0/swh/storage/interface.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     5033 2024-05-23 13:05:35.000000 swh_storage-2.4.0/swh/storage/metrics.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)    48089 2024-05-23 13:05:35.000000 swh_storage-2.4.0/swh/storage/migrate_extrinsic_metadata.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     4245 2024-05-23 13:05:35.000000 swh_storage-2.4.0/swh/storage/objstorage.py
-drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-05-23 13:05:40.913010 swh_storage-2.4.0/swh/storage/postgresql/
--rw-r--r--   0 jenkins    (115) jenkins    (120)        0 2024-05-23 13:05:35.000000 swh_storage-2.4.0/swh/storage/postgresql/__init__.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)    12515 2024-05-23 13:05:35.000000 swh_storage-2.4.0/swh/storage/postgresql/converters.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)    65514 2024-05-23 13:05:35.000000 swh_storage-2.4.0/swh/storage/postgresql/db.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)    69921 2024-05-23 13:05:35.000000 swh_storage-2.4.0/swh/storage/postgresql/storage.py
-drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-05-23 13:05:40.913010 swh_storage-2.4.0/swh/storage/proxies/
--rw-r--r--   0 jenkins    (115) jenkins    (120)        0 2024-05-23 13:05:35.000000 swh_storage-2.4.0/swh/storage/proxies/__init__.py
-drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-05-23 13:05:40.913010 swh_storage-2.4.0/swh/storage/proxies/blocking/
--rw-r--r--   0 jenkins    (115) jenkins    (120)     4324 2024-05-23 13:05:35.000000 swh_storage-2.4.0/swh/storage/proxies/blocking/__init__.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)    11863 2024-05-23 13:05:35.000000 swh_storage-2.4.0/swh/storage/proxies/blocking/cli.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)    16395 2024-05-23 13:05:35.000000 swh_storage-2.4.0/swh/storage/proxies/blocking/db.py
-drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-05-23 13:05:40.913010 swh_storage-2.4.0/swh/storage/proxies/blocking/sql/
--rw-r--r--   0 jenkins    (115) jenkins    (120)       66 2024-05-23 13:05:35.000000 swh_storage-2.4.0/swh/storage/proxies/blocking/sql/10-superuser-init.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)     2665 2024-05-23 13:05:35.000000 swh_storage-2.4.0/swh/storage/proxies/blocking/sql/30-schema.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)      324 2024-05-23 13:05:35.000000 swh_storage-2.4.0/swh/storage/proxies/blocking/sql/60-indexes.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)    12690 2024-05-23 13:05:35.000000 swh_storage-2.4.0/swh/storage/proxies/buffer.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     2033 2024-05-23 13:05:35.000000 swh_storage-2.4.0/swh/storage/proxies/counter.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     5120 2024-05-23 13:05:35.000000 swh_storage-2.4.0/swh/storage/proxies/filter.py
-drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-05-23 13:05:40.917009 swh_storage-2.4.0/swh/storage/proxies/masking/
--rw-r--r--   0 jenkins    (115) jenkins    (120)    18649 2024-05-23 13:05:35.000000 swh_storage-2.4.0/swh/storage/proxies/masking/__init__.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)    13661 2024-05-23 13:05:35.000000 swh_storage-2.4.0/swh/storage/proxies/masking/cli.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)    14347 2024-05-23 13:05:35.000000 swh_storage-2.4.0/swh/storage/proxies/masking/db.py
-drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-05-23 13:05:40.917009 swh_storage-2.4.0/swh/storage/proxies/masking/sql/
--rw-r--r--   0 jenkins    (115) jenkins    (120)       66 2024-05-23 13:05:35.000000 swh_storage-2.4.0/swh/storage/proxies/masking/sql/10-superuser-init.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)      220 2024-05-23 13:05:35.000000 swh_storage-2.4.0/swh/storage/proxies/masking/sql/20-types.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)     1989 2024-05-23 13:05:35.000000 swh_storage-2.4.0/swh/storage/proxies/masking/sql/30-schema.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)      334 2024-05-23 13:05:35.000000 swh_storage-2.4.0/swh/storage/proxies/masking/sql/60-indexes.sql
-drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-05-23 13:05:40.917009 swh_storage-2.4.0/swh/storage/proxies/masking/sql/upgrades/
--rw-r--r--   0 jenkins    (115) jenkins    (120)      336 2024-05-23 13:05:35.000000 swh_storage-2.4.0/swh/storage/proxies/masking/sql/upgrades/193.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)     4255 2024-05-23 13:05:35.000000 swh_storage-2.4.0/swh/storage/proxies/record_references.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     3229 2024-05-23 13:05:35.000000 swh_storage-2.4.0/swh/storage/proxies/retry.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     7058 2024-05-23 13:05:35.000000 swh_storage-2.4.0/swh/storage/proxies/tenacious.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     2586 2024-05-23 13:05:35.000000 swh_storage-2.4.0/swh/storage/proxies/validate.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)       27 2024-05-23 13:05:35.000000 swh_storage-2.4.0/swh/storage/py.typed
--rw-r--r--   0 jenkins    (115) jenkins    (120)    10170 2024-05-23 13:05:35.000000 swh_storage-2.4.0/swh/storage/pytest_plugin.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)    10225 2024-05-23 13:05:35.000000 swh_storage-2.4.0/swh/storage/replay.py
-drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-05-23 13:05:40.917009 swh_storage-2.4.0/swh/storage/sql/
--rw-r--r--   0 jenkins    (115) jenkins    (120)      758 2024-05-23 13:05:35.000000 swh_storage-2.4.0/swh/storage/sql/10-superuser-init.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)      984 2024-05-23 13:05:35.000000 swh_storage-2.4.0/swh/storage/sql/15-flavor.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)     1080 2024-05-23 13:05:35.000000 swh_storage-2.4.0/swh/storage/sql/20-enums.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)    24592 2024-05-23 13:05:35.000000 swh_storage-2.4.0/swh/storage/sql/30-schema.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)    34836 2024-05-23 13:05:35.000000 swh_storage-2.4.0/swh/storage/sql/40-funcs.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)    13835 2024-05-23 13:05:35.000000 swh_storage-2.4.0/swh/storage/sql/60-indexes.sql
-drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-05-23 13:05:40.917009 swh_storage-2.4.0/swh/storage/sql/logical_replication/
--rw-r--r--   0 jenkins    (115) jenkins    (120)     1380 2024-05-23 13:05:35.000000 swh_storage-2.4.0/swh/storage/sql/logical_replication/replication_source.sql
-drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-05-23 13:05:40.957009 swh_storage-2.4.0/swh/storage/sql/upgrades/
--rw-r--r--   0 jenkins    (115) jenkins    (120)     6750 2024-05-23 13:05:35.000000 swh_storage-2.4.0/swh/storage/sql/upgrades/015.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)      854 2024-05-23 13:05:35.000000 swh_storage-2.4.0/swh/storage/sql/upgrades/016.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)     6452 2024-05-23 13:05:35.000000 swh_storage-2.4.0/swh/storage/sql/upgrades/017.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)     2845 2024-05-23 13:05:35.000000 swh_storage-2.4.0/swh/storage/sql/upgrades/018.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)      999 2024-05-23 13:05:35.000000 swh_storage-2.4.0/swh/storage/sql/upgrades/019.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)     1416 2024-05-23 13:05:35.000000 swh_storage-2.4.0/swh/storage/sql/upgrades/020.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)     1464 2024-05-23 13:05:35.000000 swh_storage-2.4.0/swh/storage/sql/upgrades/021.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)     1607 2024-05-23 13:05:35.000000 swh_storage-2.4.0/swh/storage/sql/upgrades/022.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)     1561 2024-05-23 13:05:35.000000 swh_storage-2.4.0/swh/storage/sql/upgrades/023.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)     6282 2024-05-23 13:05:35.000000 swh_storage-2.4.0/swh/storage/sql/upgrades/024.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)     3272 2024-05-23 13:05:35.000000 swh_storage-2.4.0/swh/storage/sql/upgrades/025.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)      658 2024-05-23 13:05:35.000000 swh_storage-2.4.0/swh/storage/sql/upgrades/026.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)     9090 2024-05-23 13:05:35.000000 swh_storage-2.4.0/swh/storage/sql/upgrades/027.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)     1446 2024-05-23 13:05:35.000000 swh_storage-2.4.0/swh/storage/sql/upgrades/028.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)     2788 2024-05-23 13:05:35.000000 swh_storage-2.4.0/swh/storage/sql/upgrades/029.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)     1706 2024-05-23 13:05:35.000000 swh_storage-2.4.0/swh/storage/sql/upgrades/030.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)     4156 2024-05-23 13:05:35.000000 swh_storage-2.4.0/swh/storage/sql/upgrades/032.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)     1131 2024-05-23 13:05:35.000000 swh_storage-2.4.0/swh/storage/sql/upgrades/033.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)     2599 2024-05-23 13:05:35.000000 swh_storage-2.4.0/swh/storage/sql/upgrades/034.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)     1535 2024-05-23 13:05:35.000000 swh_storage-2.4.0/swh/storage/sql/upgrades/035.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)     2256 2024-05-23 13:05:35.000000 swh_storage-2.4.0/swh/storage/sql/upgrades/036.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)      654 2024-05-23 13:05:35.000000 swh_storage-2.4.0/swh/storage/sql/upgrades/037.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)     4588 2024-05-23 13:05:35.000000 swh_storage-2.4.0/swh/storage/sql/upgrades/038.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)     1659 2024-05-23 13:05:35.000000 swh_storage-2.4.0/swh/storage/sql/upgrades/039.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)      553 2024-05-23 13:05:35.000000 swh_storage-2.4.0/swh/storage/sql/upgrades/040.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)      542 2024-05-23 13:05:35.000000 swh_storage-2.4.0/swh/storage/sql/upgrades/041.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)      702 2024-05-23 13:05:35.000000 swh_storage-2.4.0/swh/storage/sql/upgrades/042.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)     2902 2024-05-23 13:05:35.000000 swh_storage-2.4.0/swh/storage/sql/upgrades/043.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)     2130 2024-05-23 13:05:35.000000 swh_storage-2.4.0/swh/storage/sql/upgrades/044.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)      465 2024-05-23 13:05:35.000000 swh_storage-2.4.0/swh/storage/sql/upgrades/045.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)     7305 2024-05-23 13:05:35.000000 swh_storage-2.4.0/swh/storage/sql/upgrades/046.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)     2649 2024-05-23 13:05:35.000000 swh_storage-2.4.0/swh/storage/sql/upgrades/047.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)     1795 2024-05-23 13:05:35.000000 swh_storage-2.4.0/swh/storage/sql/upgrades/048.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)     9599 2024-05-23 13:05:35.000000 swh_storage-2.4.0/swh/storage/sql/upgrades/049.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)     1688 2024-05-23 13:05:35.000000 swh_storage-2.4.0/swh/storage/sql/upgrades/050.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)     4279 2024-05-23 13:05:35.000000 swh_storage-2.4.0/swh/storage/sql/upgrades/051.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)     6016 2024-05-23 13:05:35.000000 swh_storage-2.4.0/swh/storage/sql/upgrades/052.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)      905 2024-05-23 13:05:35.000000 swh_storage-2.4.0/swh/storage/sql/upgrades/053.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)     3187 2024-05-23 13:05:35.000000 swh_storage-2.4.0/swh/storage/sql/upgrades/054.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)     2309 2024-05-23 13:05:35.000000 swh_storage-2.4.0/swh/storage/sql/upgrades/055.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)     2350 2024-05-23 13:05:35.000000 swh_storage-2.4.0/swh/storage/sql/upgrades/056.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)      729 2024-05-23 13:05:35.000000 swh_storage-2.4.0/swh/storage/sql/upgrades/057.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)     1428 2024-05-23 13:05:35.000000 swh_storage-2.4.0/swh/storage/sql/upgrades/058.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)     1528 2024-05-23 13:05:35.000000 swh_storage-2.4.0/swh/storage/sql/upgrades/059.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)     1428 2024-05-23 13:05:35.000000 swh_storage-2.4.0/swh/storage/sql/upgrades/060.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)      724 2024-05-23 13:05:35.000000 swh_storage-2.4.0/swh/storage/sql/upgrades/061.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)     1427 2024-05-23 13:05:35.000000 swh_storage-2.4.0/swh/storage/sql/upgrades/062.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)     2594 2024-05-23 13:05:35.000000 swh_storage-2.4.0/swh/storage/sql/upgrades/063.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)      604 2024-05-23 13:05:35.000000 swh_storage-2.4.0/swh/storage/sql/upgrades/064.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)     1664 2024-05-23 13:05:35.000000 swh_storage-2.4.0/swh/storage/sql/upgrades/065.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)      281 2024-05-23 13:05:35.000000 swh_storage-2.4.0/swh/storage/sql/upgrades/066.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)     1257 2024-05-23 13:05:35.000000 swh_storage-2.4.0/swh/storage/sql/upgrades/067.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)     8795 2024-05-23 13:05:35.000000 swh_storage-2.4.0/swh/storage/sql/upgrades/068.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)      618 2024-05-23 13:05:35.000000 swh_storage-2.4.0/swh/storage/sql/upgrades/069.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)      352 2024-05-23 13:05:35.000000 swh_storage-2.4.0/swh/storage/sql/upgrades/070.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)      687 2024-05-23 13:05:35.000000 swh_storage-2.4.0/swh/storage/sql/upgrades/071.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)     3843 2024-05-23 13:05:35.000000 swh_storage-2.4.0/swh/storage/sql/upgrades/072.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)     1940 2024-05-23 13:05:35.000000 swh_storage-2.4.0/swh/storage/sql/upgrades/073.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)     2662 2024-05-23 13:05:35.000000 swh_storage-2.4.0/swh/storage/sql/upgrades/074.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)     3067 2024-05-23 13:05:35.000000 swh_storage-2.4.0/swh/storage/sql/upgrades/075.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)      551 2024-05-23 13:05:35.000000 swh_storage-2.4.0/swh/storage/sql/upgrades/076.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)     1567 2024-05-23 13:05:35.000000 swh_storage-2.4.0/swh/storage/sql/upgrades/077.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)     3642 2024-05-23 13:05:35.000000 swh_storage-2.4.0/swh/storage/sql/upgrades/078.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)      997 2024-05-23 13:05:35.000000 swh_storage-2.4.0/swh/storage/sql/upgrades/079.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)      631 2024-05-23 13:05:35.000000 swh_storage-2.4.0/swh/storage/sql/upgrades/080.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)      608 2024-05-23 13:05:35.000000 swh_storage-2.4.0/swh/storage/sql/upgrades/081.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)     3043 2024-05-23 13:05:35.000000 swh_storage-2.4.0/swh/storage/sql/upgrades/082.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)     1834 2024-05-23 13:05:35.000000 swh_storage-2.4.0/swh/storage/sql/upgrades/083.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)     2392 2024-05-23 13:05:35.000000 swh_storage-2.4.0/swh/storage/sql/upgrades/084.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)     2388 2024-05-23 13:05:35.000000 swh_storage-2.4.0/swh/storage/sql/upgrades/085.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)     1249 2024-05-23 13:05:35.000000 swh_storage-2.4.0/swh/storage/sql/upgrades/086.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)     8777 2024-05-23 13:05:35.000000 swh_storage-2.4.0/swh/storage/sql/upgrades/087.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)     3567 2024-05-23 13:05:35.000000 swh_storage-2.4.0/swh/storage/sql/upgrades/088.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)     3788 2024-05-23 13:05:35.000000 swh_storage-2.4.0/swh/storage/sql/upgrades/089.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)    21174 2024-05-23 13:05:35.000000 swh_storage-2.4.0/swh/storage/sql/upgrades/090.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)      959 2024-05-23 13:05:35.000000 swh_storage-2.4.0/swh/storage/sql/upgrades/091.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)      925 2024-05-23 13:05:35.000000 swh_storage-2.4.0/swh/storage/sql/upgrades/092.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)     1795 2024-05-23 13:05:35.000000 swh_storage-2.4.0/swh/storage/sql/upgrades/093.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)      735 2024-05-23 13:05:35.000000 swh_storage-2.4.0/swh/storage/sql/upgrades/094.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)      726 2024-05-23 13:05:35.000000 swh_storage-2.4.0/swh/storage/sql/upgrades/095.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)     1137 2024-05-23 13:05:35.000000 swh_storage-2.4.0/swh/storage/sql/upgrades/096.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)    18174 2024-05-23 13:05:35.000000 swh_storage-2.4.0/swh/storage/sql/upgrades/097.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)      280 2024-05-23 13:05:35.000000 swh_storage-2.4.0/swh/storage/sql/upgrades/098.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)      875 2024-05-23 13:05:35.000000 swh_storage-2.4.0/swh/storage/sql/upgrades/099.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)     2055 2024-05-23 13:05:35.000000 swh_storage-2.4.0/swh/storage/sql/upgrades/100.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)     1037 2024-05-23 13:05:35.000000 swh_storage-2.4.0/swh/storage/sql/upgrades/101.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)     6608 2024-05-23 13:05:35.000000 swh_storage-2.4.0/swh/storage/sql/upgrades/102.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)     2399 2024-05-23 13:05:35.000000 swh_storage-2.4.0/swh/storage/sql/upgrades/103.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)     5055 2024-05-23 13:05:35.000000 swh_storage-2.4.0/swh/storage/sql/upgrades/104.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)     1078 2024-05-23 13:05:35.000000 swh_storage-2.4.0/swh/storage/sql/upgrades/105.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)    13015 2024-05-23 13:05:35.000000 swh_storage-2.4.0/swh/storage/sql/upgrades/106.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)     1755 2024-05-23 13:05:35.000000 swh_storage-2.4.0/swh/storage/sql/upgrades/107.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)     1427 2024-05-23 13:05:35.000000 swh_storage-2.4.0/swh/storage/sql/upgrades/108.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)      816 2024-05-23 13:05:35.000000 swh_storage-2.4.0/swh/storage/sql/upgrades/109.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)    13273 2024-05-23 13:05:35.000000 swh_storage-2.4.0/swh/storage/sql/upgrades/110.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)      784 2024-05-23 13:05:35.000000 swh_storage-2.4.0/swh/storage/sql/upgrades/111.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)     1620 2024-05-23 13:05:35.000000 swh_storage-2.4.0/swh/storage/sql/upgrades/112.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)     1142 2024-05-23 13:05:35.000000 swh_storage-2.4.0/swh/storage/sql/upgrades/113.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)     2334 2024-05-23 13:05:35.000000 swh_storage-2.4.0/swh/storage/sql/upgrades/114.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)     5180 2024-05-23 13:05:35.000000 swh_storage-2.4.0/swh/storage/sql/upgrades/115.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)      276 2024-05-23 13:05:35.000000 swh_storage-2.4.0/swh/storage/sql/upgrades/116.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)     1742 2024-05-23 13:05:35.000000 swh_storage-2.4.0/swh/storage/sql/upgrades/117.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)     2768 2024-05-23 13:05:35.000000 swh_storage-2.4.0/swh/storage/sql/upgrades/118.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)      850 2024-05-23 13:05:35.000000 swh_storage-2.4.0/swh/storage/sql/upgrades/119.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)     1062 2024-05-23 13:05:35.000000 swh_storage-2.4.0/swh/storage/sql/upgrades/120.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)      274 2024-05-23 13:05:35.000000 swh_storage-2.4.0/swh/storage/sql/upgrades/121.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)      366 2024-05-23 13:05:35.000000 swh_storage-2.4.0/swh/storage/sql/upgrades/122.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)     2107 2024-05-23 13:05:35.000000 swh_storage-2.4.0/swh/storage/sql/upgrades/123.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)     1371 2024-05-23 13:05:35.000000 swh_storage-2.4.0/swh/storage/sql/upgrades/124.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)     1302 2024-05-23 13:05:35.000000 swh_storage-2.4.0/swh/storage/sql/upgrades/125.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)      329 2024-05-23 13:05:35.000000 swh_storage-2.4.0/swh/storage/sql/upgrades/126.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)     1039 2024-05-23 13:05:35.000000 swh_storage-2.4.0/swh/storage/sql/upgrades/127.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)      609 2024-05-23 13:05:35.000000 swh_storage-2.4.0/swh/storage/sql/upgrades/128.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)      832 2024-05-23 13:05:35.000000 swh_storage-2.4.0/swh/storage/sql/upgrades/129.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)     1572 2024-05-23 13:05:35.000000 swh_storage-2.4.0/swh/storage/sql/upgrades/130.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)      401 2024-05-23 13:05:35.000000 swh_storage-2.4.0/swh/storage/sql/upgrades/131.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)      386 2024-05-23 13:05:35.000000 swh_storage-2.4.0/swh/storage/sql/upgrades/132.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)      425 2024-05-23 13:05:35.000000 swh_storage-2.4.0/swh/storage/sql/upgrades/133.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)     1626 2024-05-23 13:05:35.000000 swh_storage-2.4.0/swh/storage/sql/upgrades/134.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)      421 2024-05-23 13:05:35.000000 swh_storage-2.4.0/swh/storage/sql/upgrades/135.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)     1036 2024-05-23 13:05:35.000000 swh_storage-2.4.0/swh/storage/sql/upgrades/136.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)    10048 2024-05-23 13:05:35.000000 swh_storage-2.4.0/swh/storage/sql/upgrades/137.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)      926 2024-05-23 13:05:35.000000 swh_storage-2.4.0/swh/storage/sql/upgrades/138.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)      845 2024-05-23 13:05:35.000000 swh_storage-2.4.0/swh/storage/sql/upgrades/139.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)      456 2024-05-23 13:05:35.000000 swh_storage-2.4.0/swh/storage/sql/upgrades/140.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)      230 2024-05-23 13:05:35.000000 swh_storage-2.4.0/swh/storage/sql/upgrades/141.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)      239 2024-05-23 13:05:35.000000 swh_storage-2.4.0/swh/storage/sql/upgrades/142.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)     2897 2024-05-23 13:05:35.000000 swh_storage-2.4.0/swh/storage/sql/upgrades/143.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)      283 2024-05-23 13:05:35.000000 swh_storage-2.4.0/swh/storage/sql/upgrades/144.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)      275 2024-05-23 13:05:35.000000 swh_storage-2.4.0/swh/storage/sql/upgrades/145.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)     3340 2024-05-23 13:05:35.000000 swh_storage-2.4.0/swh/storage/sql/upgrades/146.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)     2676 2024-05-23 13:05:35.000000 swh_storage-2.4.0/swh/storage/sql/upgrades/147.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)     2168 2024-05-23 13:05:35.000000 swh_storage-2.4.0/swh/storage/sql/upgrades/148.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)     3849 2024-05-23 13:05:35.000000 swh_storage-2.4.0/swh/storage/sql/upgrades/149.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)      624 2024-05-23 13:05:35.000000 swh_storage-2.4.0/swh/storage/sql/upgrades/150.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)      373 2024-05-23 13:05:35.000000 swh_storage-2.4.0/swh/storage/sql/upgrades/151.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)      302 2024-05-23 13:05:35.000000 swh_storage-2.4.0/swh/storage/sql/upgrades/152.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)      462 2024-05-23 13:05:35.000000 swh_storage-2.4.0/swh/storage/sql/upgrades/153.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)     1546 2024-05-23 13:05:35.000000 swh_storage-2.4.0/swh/storage/sql/upgrades/154.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)     1044 2024-05-23 13:05:35.000000 swh_storage-2.4.0/swh/storage/sql/upgrades/155.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)      875 2024-05-23 13:05:35.000000 swh_storage-2.4.0/swh/storage/sql/upgrades/156.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)     2606 2024-05-23 13:05:35.000000 swh_storage-2.4.0/swh/storage/sql/upgrades/157.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)     3118 2024-05-23 13:05:35.000000 swh_storage-2.4.0/swh/storage/sql/upgrades/158.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)      727 2024-05-23 13:05:35.000000 swh_storage-2.4.0/swh/storage/sql/upgrades/159.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)     1353 2024-05-23 13:05:35.000000 swh_storage-2.4.0/swh/storage/sql/upgrades/160.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)      548 2024-05-23 13:05:35.000000 swh_storage-2.4.0/swh/storage/sql/upgrades/161.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)     2099 2024-05-23 13:05:35.000000 swh_storage-2.4.0/swh/storage/sql/upgrades/162.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)     1202 2024-05-23 13:05:35.000000 swh_storage-2.4.0/swh/storage/sql/upgrades/163.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)      304 2024-05-23 13:05:35.000000 swh_storage-2.4.0/swh/storage/sql/upgrades/164.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)      430 2024-05-23 13:05:35.000000 swh_storage-2.4.0/swh/storage/sql/upgrades/165.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)      306 2024-05-23 13:05:35.000000 swh_storage-2.4.0/swh/storage/sql/upgrades/166.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)      591 2024-05-23 13:05:35.000000 swh_storage-2.4.0/swh/storage/sql/upgrades/167.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)     1403 2024-05-23 13:05:35.000000 swh_storage-2.4.0/swh/storage/sql/upgrades/168.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)     1812 2024-05-23 13:05:35.000000 swh_storage-2.4.0/swh/storage/sql/upgrades/169.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)      614 2024-05-23 13:05:35.000000 swh_storage-2.4.0/swh/storage/sql/upgrades/170.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)      758 2024-05-23 13:05:35.000000 swh_storage-2.4.0/swh/storage/sql/upgrades/171.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)      873 2024-05-23 13:05:35.000000 swh_storage-2.4.0/swh/storage/sql/upgrades/172.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)      561 2024-05-23 13:05:35.000000 swh_storage-2.4.0/swh/storage/sql/upgrades/173.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)      324 2024-05-23 13:05:35.000000 swh_storage-2.4.0/swh/storage/sql/upgrades/174.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)     1294 2024-05-23 13:05:35.000000 swh_storage-2.4.0/swh/storage/sql/upgrades/175.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)      886 2024-05-23 13:05:35.000000 swh_storage-2.4.0/swh/storage/sql/upgrades/176.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)      256 2024-05-23 13:05:35.000000 swh_storage-2.4.0/swh/storage/sql/upgrades/177.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)      256 2024-05-23 13:05:35.000000 swh_storage-2.4.0/swh/storage/sql/upgrades/178.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)     6715 2024-05-23 13:05:35.000000 swh_storage-2.4.0/swh/storage/sql/upgrades/179.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)     3159 2024-05-23 13:05:35.000000 swh_storage-2.4.0/swh/storage/sql/upgrades/180.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)      661 2024-05-23 13:05:35.000000 swh_storage-2.4.0/swh/storage/sql/upgrades/181.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)     2782 2024-05-23 13:05:35.000000 swh_storage-2.4.0/swh/storage/sql/upgrades/182.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)     1715 2024-05-23 13:05:35.000000 swh_storage-2.4.0/swh/storage/sql/upgrades/183.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)      910 2024-05-23 13:05:35.000000 swh_storage-2.4.0/swh/storage/sql/upgrades/184.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)     1091 2024-05-23 13:05:35.000000 swh_storage-2.4.0/swh/storage/sql/upgrades/185.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)      356 2024-05-23 13:05:35.000000 swh_storage-2.4.0/swh/storage/sql/upgrades/186.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)     1601 2024-05-23 13:05:35.000000 swh_storage-2.4.0/swh/storage/sql/upgrades/187.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)     1045 2024-05-23 13:05:35.000000 swh_storage-2.4.0/swh/storage/sql/upgrades/188.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)      616 2024-05-23 13:05:35.000000 swh_storage-2.4.0/swh/storage/sql/upgrades/189.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)     1105 2024-05-23 13:05:35.000000 swh_storage-2.4.0/swh/storage/sql/upgrades/190.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)     1751 2024-05-23 13:05:35.000000 swh_storage-2.4.0/swh/storage/sql/upgrades/191.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)      162 2024-05-23 13:05:35.000000 swh_storage-2.4.0/swh/storage/sql/upgrades/192.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)     1731 2024-05-23 13:05:35.000000 swh_storage-2.4.0/swh/storage/sql/upgrades/193.sql
-drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-05-23 13:05:40.965009 swh_storage-2.4.0/swh/storage/tests/
--rw-r--r--   0 jenkins    (115) jenkins    (120)      356 2024-05-23 13:05:35.000000 swh_storage-2.4.0/swh/storage/tests/__init__.py
-drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-05-23 13:05:40.965009 swh_storage-2.4.0/swh/storage/tests/algos/
--rw-r--r--   0 jenkins    (115) jenkins    (120)        0 2024-05-23 13:05:35.000000 swh_storage-2.4.0/swh/storage/tests/algos/__init__.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)    12969 2024-05-23 13:05:35.000000 swh_storage-2.4.0/swh/storage/tests/algos/test_diff.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     5545 2024-05-23 13:05:35.000000 swh_storage-2.4.0/swh/storage/tests/algos/test_dir_iterator.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     7293 2024-05-23 13:05:35.000000 swh_storage-2.4.0/swh/storage/tests/algos/test_directory.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     2284 2024-05-23 13:05:35.000000 swh_storage-2.4.0/swh/storage/tests/algos/test_discovery.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)    11595 2024-05-23 13:05:35.000000 swh_storage-2.4.0/swh/storage/tests/algos/test_origin.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)    18297 2024-05-23 13:05:35.000000 swh_storage-2.4.0/swh/storage/tests/algos/test_revisions_walker.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)    13956 2024-05-23 13:05:35.000000 swh_storage-2.4.0/swh/storage/tests/algos/test_snapshot.py
-drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-05-23 13:05:40.965009 swh_storage-2.4.0/swh/storage/tests/blocking/
--rw-r--r--   0 jenkins    (115) jenkins    (120)        0 2024-05-23 13:05:35.000000 swh_storage-2.4.0/swh/storage/tests/blocking/__init__.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     1094 2024-05-23 13:05:35.000000 swh_storage-2.4.0/swh/storage/tests/blocking/conftest.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)    18586 2024-05-23 13:05:35.000000 swh_storage-2.4.0/swh/storage/tests/blocking/test_cli.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     9375 2024-05-23 13:05:35.000000 swh_storage-2.4.0/swh/storage/tests/blocking/test_db.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)    21189 2024-05-23 13:05:35.000000 swh_storage-2.4.0/swh/storage/tests/blocking/test_proxy.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     2801 2024-05-23 13:05:35.000000 swh_storage-2.4.0/swh/storage/tests/blocking/test_proxy_blocking.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     1074 2024-05-23 13:05:35.000000 swh_storage-2.4.0/swh/storage/tests/blocking/test_proxy_no_blocking.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     2790 2024-05-23 13:05:35.000000 swh_storage-2.4.0/swh/storage/tests/conftest.py
-drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-05-23 13:05:40.965009 swh_storage-2.4.0/swh/storage/tests/data/
--rw-r--r--   0 jenkins    (115) jenkins    (120)      189 2024-05-23 13:05:35.000000 swh_storage-2.4.0/swh/storage/tests/data/storage.yml
-drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-05-23 13:05:40.969009 swh_storage-2.4.0/swh/storage/tests/masking/
--rw-r--r--   0 jenkins    (115) jenkins    (120)        0 2024-05-23 13:05:35.000000 swh_storage-2.4.0/swh/storage/tests/masking/__init__.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     1076 2024-05-23 13:05:35.000000 swh_storage-2.4.0/swh/storage/tests/masking/conftest.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)    19842 2024-05-23 13:05:35.000000 swh_storage-2.4.0/swh/storage/tests/masking/test_cli.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)    10967 2024-05-23 13:05:35.000000 swh_storage-2.4.0/swh/storage/tests/masking/test_db.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)    30500 2024-05-23 13:05:35.000000 swh_storage-2.4.0/swh/storage/tests/masking/test_proxy.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     5872 2024-05-23 13:05:35.000000 swh_storage-2.4.0/swh/storage/tests/masking/test_proxy_masking.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)      960 2024-05-23 13:05:35.000000 swh_storage-2.4.0/swh/storage/tests/masking/test_proxy_no_masking.py
-drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-05-23 13:05:40.969009 swh_storage-2.4.0/swh/storage/tests/migrate_extrinsic_metadata/
--rw-r--r--   0 jenkins    (115) jenkins    (120)    11035 2024-05-23 13:05:35.000000 swh_storage-2.4.0/swh/storage/tests/migrate_extrinsic_metadata/test_cran.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)    20328 2024-05-23 13:05:35.000000 swh_storage-2.4.0/swh/storage/tests/migrate_extrinsic_metadata/test_debian.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)    52095 2024-05-23 13:05:35.000000 swh_storage-2.4.0/swh/storage/tests/migrate_extrinsic_metadata/test_deposit.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     3702 2024-05-23 13:05:35.000000 swh_storage-2.4.0/swh/storage/tests/migrate_extrinsic_metadata/test_gnu.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     4246 2024-05-23 13:05:35.000000 swh_storage-2.4.0/swh/storage/tests/migrate_extrinsic_metadata/test_nixguix.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)    15543 2024-05-23 13:05:35.000000 swh_storage-2.4.0/swh/storage/tests/migrate_extrinsic_metadata/test_npm.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)    25053 2024-05-23 13:05:35.000000 swh_storage-2.4.0/swh/storage/tests/migrate_extrinsic_metadata/test_pypi.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)    27741 2024-05-23 13:05:35.000000 swh_storage-2.4.0/swh/storage/tests/storage_data.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)   235382 2024-05-23 13:05:35.000000 swh_storage-2.4.0/swh/storage/tests/storage_tests.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     6103 2024-05-23 13:05:35.000000 swh_storage-2.4.0/swh/storage/tests/test_api_client.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)    14820 2024-05-23 13:05:35.000000 swh_storage-2.4.0/swh/storage/tests/test_backfill.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)    24799 2024-05-23 13:05:35.000000 swh_storage-2.4.0/swh/storage/tests/test_buffer.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)    29473 2024-05-23 13:05:35.000000 swh_storage-2.4.0/swh/storage/tests/test_cassandra.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     5495 2024-05-23 13:05:35.000000 swh_storage-2.4.0/swh/storage/tests/test_cassandra_converters.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)    12438 2024-05-23 13:05:35.000000 swh_storage-2.4.0/swh/storage/tests/test_cassandra_migration.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)    13326 2024-05-23 13:05:35.000000 swh_storage-2.4.0/swh/storage/tests/test_cli.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     1887 2024-05-23 13:05:35.000000 swh_storage-2.4.0/swh/storage/tests/test_counter.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     2360 2024-05-23 13:05:35.000000 swh_storage-2.4.0/swh/storage/tests/test_exception.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     5260 2024-05-23 13:05:35.000000 swh_storage-2.4.0/swh/storage/tests/test_filter.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     4188 2024-05-23 13:05:35.000000 swh_storage-2.4.0/swh/storage/tests/test_in_memory.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     8745 2024-05-23 13:05:35.000000 swh_storage-2.4.0/swh/storage/tests/test_init.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     4944 2024-05-23 13:05:35.000000 swh_storage-2.4.0/swh/storage/tests/test_kafka_writer.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     4698 2024-05-23 13:05:35.000000 swh_storage-2.4.0/swh/storage/tests/test_metrics.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)    20071 2024-05-23 13:05:35.000000 swh_storage-2.4.0/swh/storage/tests/test_postgresql.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)    12253 2024-05-23 13:05:35.000000 swh_storage-2.4.0/swh/storage/tests/test_postgresql_converters.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     1399 2024-05-23 13:05:35.000000 swh_storage-2.4.0/swh/storage/tests/test_postgresql_flavor_mirror.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     1423 2024-05-23 13:05:35.000000 swh_storage-2.4.0/swh/storage/tests/test_postgresql_flavor_readreplica.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)      669 2024-05-23 13:05:35.000000 swh_storage-2.4.0/swh/storage/tests/test_pytest_plugin.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     8582 2024-05-23 13:05:35.000000 swh_storage-2.4.0/swh/storage/tests/test_record_references.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)    23199 2024-05-23 13:05:35.000000 swh_storage-2.4.0/swh/storage/tests/test_replay.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     8212 2024-05-23 13:05:35.000000 swh_storage-2.4.0/swh/storage/tests/test_retry.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     1589 2024-05-23 13:05:35.000000 swh_storage-2.4.0/swh/storage/tests/test_revision_bw_compat.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     1346 2024-05-23 13:05:35.000000 swh_storage-2.4.0/swh/storage/tests/test_serializers.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     3323 2024-05-23 13:05:35.000000 swh_storage-2.4.0/swh/storage/tests/test_server.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     1186 2024-05-23 13:05:35.000000 swh_storage-2.4.0/swh/storage/tests/test_storage_data.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)    14141 2024-05-23 13:05:35.000000 swh_storage-2.4.0/swh/storage/tests/test_tenacious.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     4755 2024-05-23 13:05:35.000000 swh_storage-2.4.0/swh/storage/tests/test_utils.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     4515 2024-05-23 13:05:35.000000 swh_storage-2.4.0/swh/storage/tests/test_validate.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     3700 2024-05-23 13:05:35.000000 swh_storage-2.4.0/swh/storage/utils.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     4030 2024-05-23 13:05:35.000000 swh_storage-2.4.0/swh/storage/writer.py
-drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-05-23 13:05:40.969009 swh_storage-2.4.0/swh.storage.egg-info/
--rw-r--r--   0 jenkins    (115) jenkins    (120)     8493 2024-05-23 13:05:40.000000 swh_storage-2.4.0/swh.storage.egg-info/PKG-INFO
--rw-r--r--   0 jenkins    (115) jenkins    (120)    12124 2024-05-23 13:05:40.000000 swh_storage-2.4.0/swh.storage.egg-info/SOURCES.txt
--rw-r--r--   0 jenkins    (115) jenkins    (120)        1 2024-05-23 13:05:40.000000 swh_storage-2.4.0/swh.storage.egg-info/dependency_links.txt
--rw-r--r--   0 jenkins    (115) jenkins    (120)     1007 2024-05-23 13:05:40.000000 swh_storage-2.4.0/swh.storage.egg-info/entry_points.txt
--rw-r--r--   0 jenkins    (115) jenkins    (120)      488 2024-05-23 13:05:40.000000 swh_storage-2.4.0/swh.storage.egg-info/requires.txt
--rw-r--r--   0 jenkins    (115) jenkins    (120)        4 2024-05-23 13:05:40.000000 swh_storage-2.4.0/swh.storage.egg-info/top_level.txt
--rw-r--r--   0 jenkins    (115) jenkins    (120)     1264 2024-05-23 13:05:35.000000 swh_storage-2.4.0/tox.ini
+drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-06-03 13:12:34.638767 swh_storage-2.4.1/
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      352 2024-06-03 13:12:28.000000 swh_storage-2.4.1/.copier-answers.yml
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      158 2024-06-03 13:12:28.000000 swh_storage-2.4.1/.git-blame-ignore-revs
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      356 2024-06-03 13:12:28.000000 swh_storage-2.4.1/.gitignore
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     1453 2024-06-03 13:12:28.000000 swh_storage-2.4.1/.pre-commit-config.yaml
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      112 2024-06-03 13:12:28.000000 swh_storage-2.4.1/AUTHORS
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     3397 2024-06-03 13:12:28.000000 swh_storage-2.4.1/CODE_OF_CONDUCT.md
+-rw-r--r--   0 jenkins    (115) jenkins    (120)       61 2024-06-03 13:12:28.000000 swh_storage-2.4.1/CONTRIBUTORS
+-rw-r--r--   0 jenkins    (115) jenkins    (120)    35147 2024-06-03 13:12:28.000000 swh_storage-2.4.1/LICENSE
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      163 2024-06-03 13:12:28.000000 swh_storage-2.4.1/Makefile
+-rw-r--r--   0 jenkins    (115) jenkins    (120)       72 2024-06-03 13:12:28.000000 swh_storage-2.4.1/Makefile.local
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     8546 2024-06-03 13:12:34.638767 swh_storage-2.4.1/PKG-INFO
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     6270 2024-06-03 13:12:28.000000 swh_storage-2.4.1/README.rst
+drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-06-03 13:12:34.542768 swh_storage-2.4.1/bin/
+-rwxr-xr-x   0 jenkins    (115) jenkins    (120)     1240 2024-06-03 13:12:28.000000 swh_storage-2.4.1/bin/swh-storage-add-dir
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      294 2024-06-03 13:12:28.000000 swh_storage-2.4.1/conftest.py
+drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-06-03 13:12:34.546768 swh_storage-2.4.1/docs/
+-rw-r--r--   0 jenkins    (115) jenkins    (120)       24 2024-06-03 13:12:28.000000 swh_storage-2.4.1/docs/.gitignore
+-rw-r--r--   0 jenkins    (115) jenkins    (120)       48 2024-06-03 13:12:28.000000 swh_storage-2.4.1/docs/Makefile
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      530 2024-06-03 13:12:28.000000 swh_storage-2.4.1/docs/Makefile.local
+drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-06-03 13:12:34.546768 swh_storage-2.4.1/docs/_static/
+-rw-r--r--   0 jenkins    (115) jenkins    (120)        0 2024-06-03 13:12:28.000000 swh_storage-2.4.1/docs/_static/.placeholder
+drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-06-03 13:12:34.546768 swh_storage-2.4.1/docs/_templates/
+-rw-r--r--   0 jenkins    (115) jenkins    (120)        0 2024-06-03 13:12:28.000000 swh_storage-2.4.1/docs/_templates/.placeholder
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     2206 2024-06-03 13:12:28.000000 swh_storage-2.4.1/docs/archive-copies.rst
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      143 2024-06-03 13:12:28.000000 swh_storage-2.4.1/docs/cli.rst
+-rw-r--r--   0 jenkins    (115) jenkins    (120)       43 2024-06-03 13:12:28.000000 swh_storage-2.4.1/docs/conf.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)    12947 2024-06-03 13:12:28.000000 swh_storage-2.4.1/docs/extrinsic-metadata-specification.rst
+drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-06-03 13:12:34.546768 swh_storage-2.4.1/docs/images/
+-rw-r--r--   0 jenkins    (115) jenkins    (120)       12 2024-06-03 13:12:28.000000 swh_storage-2.4.1/docs/images/.gitignore
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      335 2024-06-03 13:12:28.000000 swh_storage-2.4.1/docs/images/Makefile
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     3031 2024-06-03 13:12:28.000000 swh_storage-2.4.1/docs/images/swh-archive-copies.dia
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     2843 2024-06-03 13:12:28.000000 swh_storage-2.4.1/docs/index.rst
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     3772 2024-06-03 13:12:28.000000 swh_storage-2.4.1/docs/object-masking.rst
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      268 2024-06-03 13:12:28.000000 swh_storage-2.4.1/docs/sql-storage.rst
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     1097 2024-06-03 13:12:28.000000 swh_storage-2.4.1/mypy.ini
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     2852 2024-06-03 13:12:28.000000 swh_storage-2.4.1/pyproject.toml
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      458 2024-06-03 13:12:28.000000 swh_storage-2.4.1/pytest.ini
+-rw-r--r--   0 jenkins    (115) jenkins    (120)       19 2024-06-03 13:12:28.000000 swh_storage-2.4.1/requirements-swh-journal.txt
+-rw-r--r--   0 jenkins    (115) jenkins    (120)       94 2024-06-03 13:12:28.000000 swh_storage-2.4.1/requirements-swh.txt
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      424 2024-06-03 13:12:28.000000 swh_storage-2.4.1/requirements-test.txt
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      189 2024-06-03 13:12:28.000000 swh_storage-2.4.1/requirements.txt
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      120 2024-06-03 13:12:34.638767 swh_storage-2.4.1/setup.cfg
+drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-06-03 13:12:34.550768 swh_storage-2.4.1/sql/
+-rw-r--r--   0 jenkins    (115) jenkins    (120)       26 2024-06-03 13:12:28.000000 swh_storage-2.4.1/sql/.gitignore
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     1565 2024-06-03 13:12:28.000000 swh_storage-2.4.1/sql/Makefile
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     1094 2024-06-03 13:12:28.000000 swh_storage-2.4.1/sql/TODO
+drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-06-03 13:12:34.550768 swh_storage-2.4.1/sql/bin/
+-rwxr-xr-x   0 jenkins    (115) jenkins    (120)     1701 2024-06-03 13:12:28.000000 swh_storage-2.4.1/sql/bin/db-upgrade
+-rwxr-xr-x   0 jenkins    (115) jenkins    (120)      538 2024-06-03 13:12:28.000000 swh_storage-2.4.1/sql/bin/dot_add_content
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     2023 2024-06-03 13:12:28.000000 swh_storage-2.4.1/sql/clusters.dot
+drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-06-03 13:12:34.534768 swh_storage-2.4.1/sql/doc/
+drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-06-03 13:12:34.554768 swh_storage-2.4.1/sql/json/
+-rw-r--r--   0 jenkins    (115) jenkins    (120)        8 2024-06-03 13:12:28.000000 swh_storage-2.4.1/sql/json/.gitignore
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      283 2024-06-03 13:12:28.000000 swh_storage-2.4.1/sql/json/Makefile
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      223 2024-06-03 13:12:28.000000 swh_storage-2.4.1/sql/json/entity.lister_metadata.schema.json
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      129 2024-06-03 13:12:28.000000 swh_storage-2.4.1/sql/json/entity.metadata.schema.json
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      223 2024-06-03 13:12:28.000000 swh_storage-2.4.1/sql/json/entity_history.lister_metadata.schema.json
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      137 2024-06-03 13:12:28.000000 swh_storage-2.4.1/sql/json/entity_history.metadata.schema.json
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      631 2024-06-03 13:12:28.000000 swh_storage-2.4.1/sql/json/fetch_history.result.schema.json
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      133 2024-06-03 13:12:28.000000 swh_storage-2.4.1/sql/json/list_history.result.schema.json
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      141 2024-06-03 13:12:28.000000 swh_storage-2.4.1/sql/json/listable_entity.list_params.schema.json
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      632 2024-06-03 13:12:28.000000 swh_storage-2.4.1/sql/json/origin_visit.metadata.json
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      252 2024-06-03 13:12:28.000000 swh_storage-2.4.1/sql/json/tool.tool_configuration.schema.json
+drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-06-03 13:12:34.534768 swh_storage-2.4.1/swh/
+drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-06-03 13:12:34.558768 swh_storage-2.4.1/swh/storage/
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     3509 2024-06-03 13:12:28.000000 swh_storage-2.4.1/swh/storage/__init__.py
+drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-06-03 13:12:34.562768 swh_storage-2.4.1/swh/storage/algos/
+-rw-r--r--   0 jenkins    (115) jenkins    (120)        0 2024-06-03 13:12:28.000000 swh_storage-2.4.1/swh/storage/algos/__init__.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)    16246 2024-06-03 13:12:28.000000 swh_storage-2.4.1/swh/storage/algos/diff.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)    12947 2024-06-03 13:12:28.000000 swh_storage-2.4.1/swh/storage/algos/dir_iterators.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     3468 2024-06-03 13:12:28.000000 swh_storage-2.4.1/swh/storage/algos/directory.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     1487 2024-06-03 13:12:28.000000 swh_storage-2.4.1/swh/storage/algos/discovery.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     3280 2024-06-03 13:12:28.000000 swh_storage-2.4.1/swh/storage/algos/origin.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)    19935 2024-06-03 13:12:28.000000 swh_storage-2.4.1/swh/storage/algos/revisions_walker.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     6710 2024-06-03 13:12:28.000000 swh_storage-2.4.1/swh/storage/algos/snapshot.py
+drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-06-03 13:12:34.562768 swh_storage-2.4.1/swh/storage/api/
+-rw-r--r--   0 jenkins    (115) jenkins    (120)        0 2024-06-03 13:12:28.000000 swh_storage-2.4.1/swh/storage/api/__init__.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     2051 2024-06-03 13:12:28.000000 swh_storage-2.4.1/swh/storage/api/client.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     4512 2024-06-03 13:12:28.000000 swh_storage-2.4.1/swh/storage/api/serializers.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     5403 2024-06-03 13:12:28.000000 swh_storage-2.4.1/swh/storage/api/server.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)    20586 2024-06-03 13:12:28.000000 swh_storage-2.4.1/swh/storage/backfill.py
+drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-06-03 13:12:34.562768 swh_storage-2.4.1/swh/storage/cassandra/
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      375 2024-06-03 13:12:28.000000 swh_storage-2.4.1/swh/storage/cassandra/__init__.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      516 2024-06-03 13:12:28.000000 swh_storage-2.4.1/swh/storage/cassandra/common.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     5919 2024-06-03 13:12:28.000000 swh_storage-2.4.1/swh/storage/cassandra/converters.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)    62367 2024-06-03 13:12:28.000000 swh_storage-2.4.1/swh/storage/cassandra/cql.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)    10776 2024-06-03 13:12:28.000000 swh_storage-2.4.1/swh/storage/cassandra/model.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     9301 2024-06-03 13:12:28.000000 swh_storage-2.4.1/swh/storage/cassandra/schema.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)    86852 2024-06-03 13:12:28.000000 swh_storage-2.4.1/swh/storage/cassandra/storage.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)    14879 2024-06-03 13:12:28.000000 swh_storage-2.4.1/swh/storage/cli.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      496 2024-06-03 13:12:28.000000 swh_storage-2.4.1/swh/storage/common.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     4056 2024-06-03 13:12:28.000000 swh_storage-2.4.1/swh/storage/exc.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     2010 2024-06-03 13:12:28.000000 swh_storage-2.4.1/swh/storage/fixer.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)    31355 2024-06-03 13:12:28.000000 swh_storage-2.4.1/swh/storage/in_memory.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)    58274 2024-06-03 13:12:28.000000 swh_storage-2.4.1/swh/storage/interface.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     5033 2024-06-03 13:12:28.000000 swh_storage-2.4.1/swh/storage/metrics.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)    48089 2024-06-03 13:12:28.000000 swh_storage-2.4.1/swh/storage/migrate_extrinsic_metadata.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     4281 2024-06-03 13:12:28.000000 swh_storage-2.4.1/swh/storage/objstorage.py
+drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-06-03 13:12:34.566768 swh_storage-2.4.1/swh/storage/postgresql/
+-rw-r--r--   0 jenkins    (115) jenkins    (120)        0 2024-06-03 13:12:28.000000 swh_storage-2.4.1/swh/storage/postgresql/__init__.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)    12515 2024-06-03 13:12:28.000000 swh_storage-2.4.1/swh/storage/postgresql/converters.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)    65514 2024-06-03 13:12:28.000000 swh_storage-2.4.1/swh/storage/postgresql/db.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)    70068 2024-06-03 13:12:28.000000 swh_storage-2.4.1/swh/storage/postgresql/storage.py
+drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-06-03 13:12:34.566768 swh_storage-2.4.1/swh/storage/proxies/
+-rw-r--r--   0 jenkins    (115) jenkins    (120)        0 2024-06-03 13:12:28.000000 swh_storage-2.4.1/swh/storage/proxies/__init__.py
+drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-06-03 13:12:34.566768 swh_storage-2.4.1/swh/storage/proxies/blocking/
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     4324 2024-06-03 13:12:28.000000 swh_storage-2.4.1/swh/storage/proxies/blocking/__init__.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)    12167 2024-06-03 13:12:28.000000 swh_storage-2.4.1/swh/storage/proxies/blocking/cli.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)    15952 2024-06-03 13:12:28.000000 swh_storage-2.4.1/swh/storage/proxies/blocking/db.py
+drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-06-03 13:12:34.570767 swh_storage-2.4.1/swh/storage/proxies/blocking/sql/
+-rw-r--r--   0 jenkins    (115) jenkins    (120)       66 2024-06-03 13:12:28.000000 swh_storage-2.4.1/swh/storage/proxies/blocking/sql/10-superuser-init.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     2665 2024-06-03 13:12:28.000000 swh_storage-2.4.1/swh/storage/proxies/blocking/sql/30-schema.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      324 2024-06-03 13:12:28.000000 swh_storage-2.4.1/swh/storage/proxies/blocking/sql/60-indexes.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)    12690 2024-06-03 13:12:28.000000 swh_storage-2.4.1/swh/storage/proxies/buffer.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     2067 2024-06-03 13:12:28.000000 swh_storage-2.4.1/swh/storage/proxies/counter.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     5154 2024-06-03 13:12:28.000000 swh_storage-2.4.1/swh/storage/proxies/filter.py
+drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-06-03 13:12:34.570767 swh_storage-2.4.1/swh/storage/proxies/masking/
+-rw-r--r--   0 jenkins    (115) jenkins    (120)    24196 2024-06-03 13:12:28.000000 swh_storage-2.4.1/swh/storage/proxies/masking/__init__.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)    13661 2024-06-03 13:12:28.000000 swh_storage-2.4.1/swh/storage/proxies/masking/cli.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)    15895 2024-06-03 13:12:28.000000 swh_storage-2.4.1/swh/storage/proxies/masking/db.py
+drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-06-03 13:12:34.570767 swh_storage-2.4.1/swh/storage/proxies/masking/sql/
+-rw-r--r--   0 jenkins    (115) jenkins    (120)       66 2024-06-03 13:12:28.000000 swh_storage-2.4.1/swh/storage/proxies/masking/sql/10-superuser-init.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      220 2024-06-03 13:12:28.000000 swh_storage-2.4.1/swh/storage/proxies/masking/sql/20-types.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     2510 2024-06-03 13:12:28.000000 swh_storage-2.4.1/swh/storage/proxies/masking/sql/30-schema.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      334 2024-06-03 13:12:28.000000 swh_storage-2.4.1/swh/storage/proxies/masking/sql/60-indexes.sql
+drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-06-03 13:12:34.570767 swh_storage-2.4.1/swh/storage/proxies/masking/sql/upgrades/
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      336 2024-06-03 13:12:28.000000 swh_storage-2.4.1/swh/storage/proxies/masking/sql/upgrades/193.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      600 2024-06-03 13:12:28.000000 swh_storage-2.4.1/swh/storage/proxies/masking/sql/upgrades/194.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     4255 2024-06-03 13:12:28.000000 swh_storage-2.4.1/swh/storage/proxies/record_references.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     3255 2024-06-03 13:12:28.000000 swh_storage-2.4.1/swh/storage/proxies/retry.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     7058 2024-06-03 13:12:28.000000 swh_storage-2.4.1/swh/storage/proxies/tenacious.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     2620 2024-06-03 13:12:28.000000 swh_storage-2.4.1/swh/storage/proxies/validate.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)       27 2024-06-03 13:12:28.000000 swh_storage-2.4.1/swh/storage/py.typed
+-rw-r--r--   0 jenkins    (115) jenkins    (120)    10170 2024-06-03 13:12:28.000000 swh_storage-2.4.1/swh/storage/pytest_plugin.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)    10225 2024-06-03 13:12:28.000000 swh_storage-2.4.1/swh/storage/replay.py
+drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-06-03 13:12:34.574767 swh_storage-2.4.1/swh/storage/sql/
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      758 2024-06-03 13:12:28.000000 swh_storage-2.4.1/swh/storage/sql/10-superuser-init.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      984 2024-06-03 13:12:28.000000 swh_storage-2.4.1/swh/storage/sql/15-flavor.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     1080 2024-06-03 13:12:28.000000 swh_storage-2.4.1/swh/storage/sql/20-enums.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)    24592 2024-06-03 13:12:28.000000 swh_storage-2.4.1/swh/storage/sql/30-schema.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)    34836 2024-06-03 13:12:28.000000 swh_storage-2.4.1/swh/storage/sql/40-funcs.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)    13835 2024-06-03 13:12:28.000000 swh_storage-2.4.1/swh/storage/sql/60-indexes.sql
+drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-06-03 13:12:34.574767 swh_storage-2.4.1/swh/storage/sql/logical_replication/
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     1380 2024-06-03 13:12:28.000000 swh_storage-2.4.1/swh/storage/sql/logical_replication/replication_source.sql
+drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-06-03 13:12:34.618767 swh_storage-2.4.1/swh/storage/sql/upgrades/
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     6750 2024-06-03 13:12:28.000000 swh_storage-2.4.1/swh/storage/sql/upgrades/015.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      854 2024-06-03 13:12:28.000000 swh_storage-2.4.1/swh/storage/sql/upgrades/016.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     6452 2024-06-03 13:12:28.000000 swh_storage-2.4.1/swh/storage/sql/upgrades/017.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     2845 2024-06-03 13:12:28.000000 swh_storage-2.4.1/swh/storage/sql/upgrades/018.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      999 2024-06-03 13:12:28.000000 swh_storage-2.4.1/swh/storage/sql/upgrades/019.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     1416 2024-06-03 13:12:28.000000 swh_storage-2.4.1/swh/storage/sql/upgrades/020.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     1464 2024-06-03 13:12:28.000000 swh_storage-2.4.1/swh/storage/sql/upgrades/021.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     1607 2024-06-03 13:12:28.000000 swh_storage-2.4.1/swh/storage/sql/upgrades/022.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     1561 2024-06-03 13:12:28.000000 swh_storage-2.4.1/swh/storage/sql/upgrades/023.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     6282 2024-06-03 13:12:28.000000 swh_storage-2.4.1/swh/storage/sql/upgrades/024.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     3272 2024-06-03 13:12:28.000000 swh_storage-2.4.1/swh/storage/sql/upgrades/025.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      658 2024-06-03 13:12:28.000000 swh_storage-2.4.1/swh/storage/sql/upgrades/026.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     9090 2024-06-03 13:12:28.000000 swh_storage-2.4.1/swh/storage/sql/upgrades/027.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     1446 2024-06-03 13:12:28.000000 swh_storage-2.4.1/swh/storage/sql/upgrades/028.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     2788 2024-06-03 13:12:28.000000 swh_storage-2.4.1/swh/storage/sql/upgrades/029.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     1706 2024-06-03 13:12:28.000000 swh_storage-2.4.1/swh/storage/sql/upgrades/030.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     4156 2024-06-03 13:12:28.000000 swh_storage-2.4.1/swh/storage/sql/upgrades/032.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     1131 2024-06-03 13:12:28.000000 swh_storage-2.4.1/swh/storage/sql/upgrades/033.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     2599 2024-06-03 13:12:28.000000 swh_storage-2.4.1/swh/storage/sql/upgrades/034.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     1535 2024-06-03 13:12:28.000000 swh_storage-2.4.1/swh/storage/sql/upgrades/035.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     2256 2024-06-03 13:12:28.000000 swh_storage-2.4.1/swh/storage/sql/upgrades/036.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      654 2024-06-03 13:12:28.000000 swh_storage-2.4.1/swh/storage/sql/upgrades/037.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     4588 2024-06-03 13:12:28.000000 swh_storage-2.4.1/swh/storage/sql/upgrades/038.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     1659 2024-06-03 13:12:28.000000 swh_storage-2.4.1/swh/storage/sql/upgrades/039.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      553 2024-06-03 13:12:28.000000 swh_storage-2.4.1/swh/storage/sql/upgrades/040.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      542 2024-06-03 13:12:28.000000 swh_storage-2.4.1/swh/storage/sql/upgrades/041.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      702 2024-06-03 13:12:28.000000 swh_storage-2.4.1/swh/storage/sql/upgrades/042.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     2902 2024-06-03 13:12:28.000000 swh_storage-2.4.1/swh/storage/sql/upgrades/043.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     2130 2024-06-03 13:12:28.000000 swh_storage-2.4.1/swh/storage/sql/upgrades/044.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      465 2024-06-03 13:12:28.000000 swh_storage-2.4.1/swh/storage/sql/upgrades/045.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     7305 2024-06-03 13:12:28.000000 swh_storage-2.4.1/swh/storage/sql/upgrades/046.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     2649 2024-06-03 13:12:28.000000 swh_storage-2.4.1/swh/storage/sql/upgrades/047.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     1795 2024-06-03 13:12:28.000000 swh_storage-2.4.1/swh/storage/sql/upgrades/048.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     9599 2024-06-03 13:12:28.000000 swh_storage-2.4.1/swh/storage/sql/upgrades/049.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     1688 2024-06-03 13:12:28.000000 swh_storage-2.4.1/swh/storage/sql/upgrades/050.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     4279 2024-06-03 13:12:28.000000 swh_storage-2.4.1/swh/storage/sql/upgrades/051.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     6016 2024-06-03 13:12:28.000000 swh_storage-2.4.1/swh/storage/sql/upgrades/052.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      905 2024-06-03 13:12:28.000000 swh_storage-2.4.1/swh/storage/sql/upgrades/053.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     3187 2024-06-03 13:12:28.000000 swh_storage-2.4.1/swh/storage/sql/upgrades/054.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     2309 2024-06-03 13:12:28.000000 swh_storage-2.4.1/swh/storage/sql/upgrades/055.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     2350 2024-06-03 13:12:28.000000 swh_storage-2.4.1/swh/storage/sql/upgrades/056.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      729 2024-06-03 13:12:28.000000 swh_storage-2.4.1/swh/storage/sql/upgrades/057.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     1428 2024-06-03 13:12:28.000000 swh_storage-2.4.1/swh/storage/sql/upgrades/058.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     1528 2024-06-03 13:12:28.000000 swh_storage-2.4.1/swh/storage/sql/upgrades/059.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     1428 2024-06-03 13:12:28.000000 swh_storage-2.4.1/swh/storage/sql/upgrades/060.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      724 2024-06-03 13:12:28.000000 swh_storage-2.4.1/swh/storage/sql/upgrades/061.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     1427 2024-06-03 13:12:28.000000 swh_storage-2.4.1/swh/storage/sql/upgrades/062.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     2594 2024-06-03 13:12:28.000000 swh_storage-2.4.1/swh/storage/sql/upgrades/063.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      604 2024-06-03 13:12:28.000000 swh_storage-2.4.1/swh/storage/sql/upgrades/064.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     1664 2024-06-03 13:12:28.000000 swh_storage-2.4.1/swh/storage/sql/upgrades/065.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      281 2024-06-03 13:12:28.000000 swh_storage-2.4.1/swh/storage/sql/upgrades/066.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     1257 2024-06-03 13:12:28.000000 swh_storage-2.4.1/swh/storage/sql/upgrades/067.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     8795 2024-06-03 13:12:28.000000 swh_storage-2.4.1/swh/storage/sql/upgrades/068.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      618 2024-06-03 13:12:28.000000 swh_storage-2.4.1/swh/storage/sql/upgrades/069.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      352 2024-06-03 13:12:28.000000 swh_storage-2.4.1/swh/storage/sql/upgrades/070.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      687 2024-06-03 13:12:28.000000 swh_storage-2.4.1/swh/storage/sql/upgrades/071.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     3843 2024-06-03 13:12:28.000000 swh_storage-2.4.1/swh/storage/sql/upgrades/072.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     1940 2024-06-03 13:12:28.000000 swh_storage-2.4.1/swh/storage/sql/upgrades/073.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     2662 2024-06-03 13:12:28.000000 swh_storage-2.4.1/swh/storage/sql/upgrades/074.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     3067 2024-06-03 13:12:28.000000 swh_storage-2.4.1/swh/storage/sql/upgrades/075.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      551 2024-06-03 13:12:28.000000 swh_storage-2.4.1/swh/storage/sql/upgrades/076.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     1567 2024-06-03 13:12:28.000000 swh_storage-2.4.1/swh/storage/sql/upgrades/077.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     3642 2024-06-03 13:12:28.000000 swh_storage-2.4.1/swh/storage/sql/upgrades/078.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      997 2024-06-03 13:12:28.000000 swh_storage-2.4.1/swh/storage/sql/upgrades/079.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      631 2024-06-03 13:12:28.000000 swh_storage-2.4.1/swh/storage/sql/upgrades/080.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      608 2024-06-03 13:12:28.000000 swh_storage-2.4.1/swh/storage/sql/upgrades/081.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     3043 2024-06-03 13:12:28.000000 swh_storage-2.4.1/swh/storage/sql/upgrades/082.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     1834 2024-06-03 13:12:28.000000 swh_storage-2.4.1/swh/storage/sql/upgrades/083.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     2392 2024-06-03 13:12:28.000000 swh_storage-2.4.1/swh/storage/sql/upgrades/084.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     2388 2024-06-03 13:12:28.000000 swh_storage-2.4.1/swh/storage/sql/upgrades/085.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     1249 2024-06-03 13:12:28.000000 swh_storage-2.4.1/swh/storage/sql/upgrades/086.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     8777 2024-06-03 13:12:28.000000 swh_storage-2.4.1/swh/storage/sql/upgrades/087.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     3567 2024-06-03 13:12:28.000000 swh_storage-2.4.1/swh/storage/sql/upgrades/088.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     3788 2024-06-03 13:12:28.000000 swh_storage-2.4.1/swh/storage/sql/upgrades/089.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)    21174 2024-06-03 13:12:28.000000 swh_storage-2.4.1/swh/storage/sql/upgrades/090.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      959 2024-06-03 13:12:28.000000 swh_storage-2.4.1/swh/storage/sql/upgrades/091.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      925 2024-06-03 13:12:28.000000 swh_storage-2.4.1/swh/storage/sql/upgrades/092.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     1795 2024-06-03 13:12:28.000000 swh_storage-2.4.1/swh/storage/sql/upgrades/093.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      735 2024-06-03 13:12:28.000000 swh_storage-2.4.1/swh/storage/sql/upgrades/094.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      726 2024-06-03 13:12:28.000000 swh_storage-2.4.1/swh/storage/sql/upgrades/095.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     1137 2024-06-03 13:12:28.000000 swh_storage-2.4.1/swh/storage/sql/upgrades/096.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)    18174 2024-06-03 13:12:28.000000 swh_storage-2.4.1/swh/storage/sql/upgrades/097.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      280 2024-06-03 13:12:28.000000 swh_storage-2.4.1/swh/storage/sql/upgrades/098.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      875 2024-06-03 13:12:28.000000 swh_storage-2.4.1/swh/storage/sql/upgrades/099.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     2055 2024-06-03 13:12:28.000000 swh_storage-2.4.1/swh/storage/sql/upgrades/100.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     1037 2024-06-03 13:12:28.000000 swh_storage-2.4.1/swh/storage/sql/upgrades/101.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     6608 2024-06-03 13:12:28.000000 swh_storage-2.4.1/swh/storage/sql/upgrades/102.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     2399 2024-06-03 13:12:28.000000 swh_storage-2.4.1/swh/storage/sql/upgrades/103.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     5055 2024-06-03 13:12:28.000000 swh_storage-2.4.1/swh/storage/sql/upgrades/104.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     1078 2024-06-03 13:12:28.000000 swh_storage-2.4.1/swh/storage/sql/upgrades/105.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)    13015 2024-06-03 13:12:28.000000 swh_storage-2.4.1/swh/storage/sql/upgrades/106.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     1755 2024-06-03 13:12:28.000000 swh_storage-2.4.1/swh/storage/sql/upgrades/107.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     1427 2024-06-03 13:12:28.000000 swh_storage-2.4.1/swh/storage/sql/upgrades/108.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      816 2024-06-03 13:12:28.000000 swh_storage-2.4.1/swh/storage/sql/upgrades/109.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)    13273 2024-06-03 13:12:28.000000 swh_storage-2.4.1/swh/storage/sql/upgrades/110.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      784 2024-06-03 13:12:28.000000 swh_storage-2.4.1/swh/storage/sql/upgrades/111.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     1620 2024-06-03 13:12:28.000000 swh_storage-2.4.1/swh/storage/sql/upgrades/112.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     1142 2024-06-03 13:12:28.000000 swh_storage-2.4.1/swh/storage/sql/upgrades/113.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     2334 2024-06-03 13:12:28.000000 swh_storage-2.4.1/swh/storage/sql/upgrades/114.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     5180 2024-06-03 13:12:28.000000 swh_storage-2.4.1/swh/storage/sql/upgrades/115.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      276 2024-06-03 13:12:28.000000 swh_storage-2.4.1/swh/storage/sql/upgrades/116.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     1742 2024-06-03 13:12:28.000000 swh_storage-2.4.1/swh/storage/sql/upgrades/117.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     2768 2024-06-03 13:12:28.000000 swh_storage-2.4.1/swh/storage/sql/upgrades/118.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      850 2024-06-03 13:12:28.000000 swh_storage-2.4.1/swh/storage/sql/upgrades/119.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     1062 2024-06-03 13:12:28.000000 swh_storage-2.4.1/swh/storage/sql/upgrades/120.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      274 2024-06-03 13:12:28.000000 swh_storage-2.4.1/swh/storage/sql/upgrades/121.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      366 2024-06-03 13:12:28.000000 swh_storage-2.4.1/swh/storage/sql/upgrades/122.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     2107 2024-06-03 13:12:28.000000 swh_storage-2.4.1/swh/storage/sql/upgrades/123.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     1371 2024-06-03 13:12:28.000000 swh_storage-2.4.1/swh/storage/sql/upgrades/124.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     1302 2024-06-03 13:12:28.000000 swh_storage-2.4.1/swh/storage/sql/upgrades/125.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      329 2024-06-03 13:12:28.000000 swh_storage-2.4.1/swh/storage/sql/upgrades/126.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     1039 2024-06-03 13:12:28.000000 swh_storage-2.4.1/swh/storage/sql/upgrades/127.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      609 2024-06-03 13:12:28.000000 swh_storage-2.4.1/swh/storage/sql/upgrades/128.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      832 2024-06-03 13:12:28.000000 swh_storage-2.4.1/swh/storage/sql/upgrades/129.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     1572 2024-06-03 13:12:28.000000 swh_storage-2.4.1/swh/storage/sql/upgrades/130.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      401 2024-06-03 13:12:28.000000 swh_storage-2.4.1/swh/storage/sql/upgrades/131.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      386 2024-06-03 13:12:28.000000 swh_storage-2.4.1/swh/storage/sql/upgrades/132.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      425 2024-06-03 13:12:28.000000 swh_storage-2.4.1/swh/storage/sql/upgrades/133.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     1626 2024-06-03 13:12:28.000000 swh_storage-2.4.1/swh/storage/sql/upgrades/134.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      421 2024-06-03 13:12:28.000000 swh_storage-2.4.1/swh/storage/sql/upgrades/135.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     1036 2024-06-03 13:12:28.000000 swh_storage-2.4.1/swh/storage/sql/upgrades/136.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)    10048 2024-06-03 13:12:28.000000 swh_storage-2.4.1/swh/storage/sql/upgrades/137.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      926 2024-06-03 13:12:28.000000 swh_storage-2.4.1/swh/storage/sql/upgrades/138.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      845 2024-06-03 13:12:28.000000 swh_storage-2.4.1/swh/storage/sql/upgrades/139.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      456 2024-06-03 13:12:28.000000 swh_storage-2.4.1/swh/storage/sql/upgrades/140.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      230 2024-06-03 13:12:28.000000 swh_storage-2.4.1/swh/storage/sql/upgrades/141.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      239 2024-06-03 13:12:28.000000 swh_storage-2.4.1/swh/storage/sql/upgrades/142.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     2897 2024-06-03 13:12:28.000000 swh_storage-2.4.1/swh/storage/sql/upgrades/143.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      283 2024-06-03 13:12:28.000000 swh_storage-2.4.1/swh/storage/sql/upgrades/144.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      275 2024-06-03 13:12:28.000000 swh_storage-2.4.1/swh/storage/sql/upgrades/145.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     3340 2024-06-03 13:12:28.000000 swh_storage-2.4.1/swh/storage/sql/upgrades/146.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     2676 2024-06-03 13:12:28.000000 swh_storage-2.4.1/swh/storage/sql/upgrades/147.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     2168 2024-06-03 13:12:28.000000 swh_storage-2.4.1/swh/storage/sql/upgrades/148.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     3849 2024-06-03 13:12:28.000000 swh_storage-2.4.1/swh/storage/sql/upgrades/149.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      624 2024-06-03 13:12:28.000000 swh_storage-2.4.1/swh/storage/sql/upgrades/150.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      373 2024-06-03 13:12:28.000000 swh_storage-2.4.1/swh/storage/sql/upgrades/151.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      302 2024-06-03 13:12:28.000000 swh_storage-2.4.1/swh/storage/sql/upgrades/152.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      462 2024-06-03 13:12:28.000000 swh_storage-2.4.1/swh/storage/sql/upgrades/153.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     1546 2024-06-03 13:12:28.000000 swh_storage-2.4.1/swh/storage/sql/upgrades/154.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     1044 2024-06-03 13:12:28.000000 swh_storage-2.4.1/swh/storage/sql/upgrades/155.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      875 2024-06-03 13:12:28.000000 swh_storage-2.4.1/swh/storage/sql/upgrades/156.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     2606 2024-06-03 13:12:28.000000 swh_storage-2.4.1/swh/storage/sql/upgrades/157.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     3118 2024-06-03 13:12:28.000000 swh_storage-2.4.1/swh/storage/sql/upgrades/158.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      727 2024-06-03 13:12:28.000000 swh_storage-2.4.1/swh/storage/sql/upgrades/159.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     1353 2024-06-03 13:12:28.000000 swh_storage-2.4.1/swh/storage/sql/upgrades/160.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      548 2024-06-03 13:12:28.000000 swh_storage-2.4.1/swh/storage/sql/upgrades/161.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     2099 2024-06-03 13:12:28.000000 swh_storage-2.4.1/swh/storage/sql/upgrades/162.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     1202 2024-06-03 13:12:28.000000 swh_storage-2.4.1/swh/storage/sql/upgrades/163.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      304 2024-06-03 13:12:28.000000 swh_storage-2.4.1/swh/storage/sql/upgrades/164.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      430 2024-06-03 13:12:28.000000 swh_storage-2.4.1/swh/storage/sql/upgrades/165.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      306 2024-06-03 13:12:28.000000 swh_storage-2.4.1/swh/storage/sql/upgrades/166.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      591 2024-06-03 13:12:28.000000 swh_storage-2.4.1/swh/storage/sql/upgrades/167.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     1403 2024-06-03 13:12:28.000000 swh_storage-2.4.1/swh/storage/sql/upgrades/168.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     1812 2024-06-03 13:12:28.000000 swh_storage-2.4.1/swh/storage/sql/upgrades/169.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      614 2024-06-03 13:12:28.000000 swh_storage-2.4.1/swh/storage/sql/upgrades/170.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      758 2024-06-03 13:12:28.000000 swh_storage-2.4.1/swh/storage/sql/upgrades/171.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      873 2024-06-03 13:12:28.000000 swh_storage-2.4.1/swh/storage/sql/upgrades/172.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      561 2024-06-03 13:12:28.000000 swh_storage-2.4.1/swh/storage/sql/upgrades/173.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      324 2024-06-03 13:12:28.000000 swh_storage-2.4.1/swh/storage/sql/upgrades/174.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     1294 2024-06-03 13:12:28.000000 swh_storage-2.4.1/swh/storage/sql/upgrades/175.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      886 2024-06-03 13:12:28.000000 swh_storage-2.4.1/swh/storage/sql/upgrades/176.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      256 2024-06-03 13:12:28.000000 swh_storage-2.4.1/swh/storage/sql/upgrades/177.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      256 2024-06-03 13:12:28.000000 swh_storage-2.4.1/swh/storage/sql/upgrades/178.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     6715 2024-06-03 13:12:28.000000 swh_storage-2.4.1/swh/storage/sql/upgrades/179.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     3159 2024-06-03 13:12:28.000000 swh_storage-2.4.1/swh/storage/sql/upgrades/180.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      661 2024-06-03 13:12:28.000000 swh_storage-2.4.1/swh/storage/sql/upgrades/181.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     2782 2024-06-03 13:12:28.000000 swh_storage-2.4.1/swh/storage/sql/upgrades/182.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     1715 2024-06-03 13:12:28.000000 swh_storage-2.4.1/swh/storage/sql/upgrades/183.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      910 2024-06-03 13:12:28.000000 swh_storage-2.4.1/swh/storage/sql/upgrades/184.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     1091 2024-06-03 13:12:28.000000 swh_storage-2.4.1/swh/storage/sql/upgrades/185.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      356 2024-06-03 13:12:28.000000 swh_storage-2.4.1/swh/storage/sql/upgrades/186.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     1601 2024-06-03 13:12:28.000000 swh_storage-2.4.1/swh/storage/sql/upgrades/187.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     1045 2024-06-03 13:12:28.000000 swh_storage-2.4.1/swh/storage/sql/upgrades/188.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      616 2024-06-03 13:12:28.000000 swh_storage-2.4.1/swh/storage/sql/upgrades/189.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     1105 2024-06-03 13:12:28.000000 swh_storage-2.4.1/swh/storage/sql/upgrades/190.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     1751 2024-06-03 13:12:28.000000 swh_storage-2.4.1/swh/storage/sql/upgrades/191.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      162 2024-06-03 13:12:28.000000 swh_storage-2.4.1/swh/storage/sql/upgrades/192.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     1731 2024-06-03 13:12:28.000000 swh_storage-2.4.1/swh/storage/sql/upgrades/193.sql
+drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-06-03 13:12:34.626767 swh_storage-2.4.1/swh/storage/tests/
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      356 2024-06-03 13:12:28.000000 swh_storage-2.4.1/swh/storage/tests/__init__.py
+drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-06-03 13:12:34.630767 swh_storage-2.4.1/swh/storage/tests/algos/
+-rw-r--r--   0 jenkins    (115) jenkins    (120)        0 2024-06-03 13:12:28.000000 swh_storage-2.4.1/swh/storage/tests/algos/__init__.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)    12969 2024-06-03 13:12:28.000000 swh_storage-2.4.1/swh/storage/tests/algos/test_diff.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     5545 2024-06-03 13:12:28.000000 swh_storage-2.4.1/swh/storage/tests/algos/test_dir_iterator.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     7293 2024-06-03 13:12:28.000000 swh_storage-2.4.1/swh/storage/tests/algos/test_directory.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     2284 2024-06-03 13:12:28.000000 swh_storage-2.4.1/swh/storage/tests/algos/test_discovery.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)    11595 2024-06-03 13:12:28.000000 swh_storage-2.4.1/swh/storage/tests/algos/test_origin.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)    18297 2024-06-03 13:12:28.000000 swh_storage-2.4.1/swh/storage/tests/algos/test_revisions_walker.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)    15458 2024-06-03 13:12:28.000000 swh_storage-2.4.1/swh/storage/tests/algos/test_snapshot.py
+drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-06-03 13:12:34.630767 swh_storage-2.4.1/swh/storage/tests/blocking/
+-rw-r--r--   0 jenkins    (115) jenkins    (120)        0 2024-06-03 13:12:28.000000 swh_storage-2.4.1/swh/storage/tests/blocking/__init__.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     1094 2024-06-03 13:12:28.000000 swh_storage-2.4.1/swh/storage/tests/blocking/conftest.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)    18586 2024-06-03 13:12:28.000000 swh_storage-2.4.1/swh/storage/tests/blocking/test_cli.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)    11675 2024-06-03 13:12:28.000000 swh_storage-2.4.1/swh/storage/tests/blocking/test_db.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)    21189 2024-06-03 13:12:28.000000 swh_storage-2.4.1/swh/storage/tests/blocking/test_proxy.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     2801 2024-06-03 13:12:28.000000 swh_storage-2.4.1/swh/storage/tests/blocking/test_proxy_blocking.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     1074 2024-06-03 13:12:28.000000 swh_storage-2.4.1/swh/storage/tests/blocking/test_proxy_no_blocking.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     2790 2024-06-03 13:12:28.000000 swh_storage-2.4.1/swh/storage/tests/conftest.py
+drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-06-03 13:12:34.630767 swh_storage-2.4.1/swh/storage/tests/data/
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      189 2024-06-03 13:12:28.000000 swh_storage-2.4.1/swh/storage/tests/data/storage.yml
+drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-06-03 13:12:34.634767 swh_storage-2.4.1/swh/storage/tests/masking/
+-rw-r--r--   0 jenkins    (115) jenkins    (120)        0 2024-06-03 13:12:28.000000 swh_storage-2.4.1/swh/storage/tests/masking/__init__.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     1495 2024-06-03 13:12:28.000000 swh_storage-2.4.1/swh/storage/tests/masking/conftest.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)    19842 2024-06-03 13:12:28.000000 swh_storage-2.4.1/swh/storage/tests/masking/test_cli.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)    11513 2024-06-03 13:12:28.000000 swh_storage-2.4.1/swh/storage/tests/masking/test_db.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)    30174 2024-06-03 13:12:28.000000 swh_storage-2.4.1/swh/storage/tests/masking/test_proxy.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     5708 2024-06-03 13:12:28.000000 swh_storage-2.4.1/swh/storage/tests/masking/test_proxy_masking.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      708 2024-06-03 13:12:28.000000 swh_storage-2.4.1/swh/storage/tests/masking/test_proxy_passthrough.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)    10537 2024-06-03 13:12:28.000000 swh_storage-2.4.1/swh/storage/tests/masking/test_proxy_patching.py
+drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-06-03 13:12:34.634767 swh_storage-2.4.1/swh/storage/tests/migrate_extrinsic_metadata/
+-rw-r--r--   0 jenkins    (115) jenkins    (120)    11035 2024-06-03 13:12:28.000000 swh_storage-2.4.1/swh/storage/tests/migrate_extrinsic_metadata/test_cran.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)    20328 2024-06-03 13:12:28.000000 swh_storage-2.4.1/swh/storage/tests/migrate_extrinsic_metadata/test_debian.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)    52095 2024-06-03 13:12:28.000000 swh_storage-2.4.1/swh/storage/tests/migrate_extrinsic_metadata/test_deposit.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     3702 2024-06-03 13:12:28.000000 swh_storage-2.4.1/swh/storage/tests/migrate_extrinsic_metadata/test_gnu.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     4246 2024-06-03 13:12:28.000000 swh_storage-2.4.1/swh/storage/tests/migrate_extrinsic_metadata/test_nixguix.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)    15543 2024-06-03 13:12:28.000000 swh_storage-2.4.1/swh/storage/tests/migrate_extrinsic_metadata/test_npm.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)    25053 2024-06-03 13:12:28.000000 swh_storage-2.4.1/swh/storage/tests/migrate_extrinsic_metadata/test_pypi.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)    27741 2024-06-03 13:12:28.000000 swh_storage-2.4.1/swh/storage/tests/storage_data.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)   235382 2024-06-03 13:12:28.000000 swh_storage-2.4.1/swh/storage/tests/storage_tests.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     6103 2024-06-03 13:12:28.000000 swh_storage-2.4.1/swh/storage/tests/test_api_client.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)    14820 2024-06-03 13:12:28.000000 swh_storage-2.4.1/swh/storage/tests/test_backfill.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)    24799 2024-06-03 13:12:28.000000 swh_storage-2.4.1/swh/storage/tests/test_buffer.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)    29547 2024-06-03 13:12:28.000000 swh_storage-2.4.1/swh/storage/tests/test_cassandra.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     5495 2024-06-03 13:12:28.000000 swh_storage-2.4.1/swh/storage/tests/test_cassandra_converters.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)    12438 2024-06-03 13:12:28.000000 swh_storage-2.4.1/swh/storage/tests/test_cassandra_migration.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)    13326 2024-06-03 13:12:28.000000 swh_storage-2.4.1/swh/storage/tests/test_cli.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     1887 2024-06-03 13:12:28.000000 swh_storage-2.4.1/swh/storage/tests/test_counter.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     2360 2024-06-03 13:12:28.000000 swh_storage-2.4.1/swh/storage/tests/test_exception.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     5260 2024-06-03 13:12:28.000000 swh_storage-2.4.1/swh/storage/tests/test_filter.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     4188 2024-06-03 13:12:28.000000 swh_storage-2.4.1/swh/storage/tests/test_in_memory.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     8745 2024-06-03 13:12:28.000000 swh_storage-2.4.1/swh/storage/tests/test_init.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     4944 2024-06-03 13:12:28.000000 swh_storage-2.4.1/swh/storage/tests/test_kafka_writer.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     4698 2024-06-03 13:12:28.000000 swh_storage-2.4.1/swh/storage/tests/test_metrics.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)    20071 2024-06-03 13:12:28.000000 swh_storage-2.4.1/swh/storage/tests/test_postgresql.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)    12253 2024-06-03 13:12:28.000000 swh_storage-2.4.1/swh/storage/tests/test_postgresql_converters.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     1399 2024-06-03 13:12:28.000000 swh_storage-2.4.1/swh/storage/tests/test_postgresql_flavor_mirror.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     1423 2024-06-03 13:12:28.000000 swh_storage-2.4.1/swh/storage/tests/test_postgresql_flavor_readreplica.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      669 2024-06-03 13:12:28.000000 swh_storage-2.4.1/swh/storage/tests/test_pytest_plugin.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     8582 2024-06-03 13:12:28.000000 swh_storage-2.4.1/swh/storage/tests/test_record_references.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)    23487 2024-06-03 13:12:28.000000 swh_storage-2.4.1/swh/storage/tests/test_replay.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     8212 2024-06-03 13:12:28.000000 swh_storage-2.4.1/swh/storage/tests/test_retry.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     1589 2024-06-03 13:12:28.000000 swh_storage-2.4.1/swh/storage/tests/test_revision_bw_compat.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     1346 2024-06-03 13:12:28.000000 swh_storage-2.4.1/swh/storage/tests/test_serializers.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     3323 2024-06-03 13:12:28.000000 swh_storage-2.4.1/swh/storage/tests/test_server.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     1186 2024-06-03 13:12:28.000000 swh_storage-2.4.1/swh/storage/tests/test_storage_data.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)    14141 2024-06-03 13:12:28.000000 swh_storage-2.4.1/swh/storage/tests/test_tenacious.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     4755 2024-06-03 13:12:28.000000 swh_storage-2.4.1/swh/storage/tests/test_utils.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     4515 2024-06-03 13:12:28.000000 swh_storage-2.4.1/swh/storage/tests/test_validate.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     3700 2024-06-03 13:12:28.000000 swh_storage-2.4.1/swh/storage/utils.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     4235 2024-06-03 13:12:28.000000 swh_storage-2.4.1/swh/storage/writer.py
+drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-06-03 13:12:34.634767 swh_storage-2.4.1/swh.storage.egg-info/
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     8546 2024-06-03 13:12:34.000000 swh_storage-2.4.1/swh.storage.egg-info/PKG-INFO
+-rw-r--r--   0 jenkins    (115) jenkins    (120)    12223 2024-06-03 13:12:34.000000 swh_storage-2.4.1/swh.storage.egg-info/SOURCES.txt
+-rw-r--r--   0 jenkins    (115) jenkins    (120)        1 2024-06-03 13:12:34.000000 swh_storage-2.4.1/swh.storage.egg-info/dependency_links.txt
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     1007 2024-06-03 13:12:34.000000 swh_storage-2.4.1/swh.storage.egg-info/entry_points.txt
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      506 2024-06-03 13:12:34.000000 swh_storage-2.4.1/swh.storage.egg-info/requires.txt
+-rw-r--r--   0 jenkins    (115) jenkins    (120)        4 2024-06-03 13:12:34.000000 swh_storage-2.4.1/swh.storage.egg-info/top_level.txt
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     1264 2024-06-03 13:12:28.000000 swh_storage-2.4.1/tox.ini
```

### Comparing `swh_storage-2.4.0/.pre-commit-config.yaml` & `swh_storage-2.4.1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `swh_storage-2.4.0/CODE_OF_CONDUCT.md` & `swh_storage-2.4.1/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `swh_storage-2.4.0/LICENSE` & `swh_storage-2.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `swh_storage-2.4.0/PKG-INFO` & `swh_storage-2.4.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: swh.storage
-Version: 2.4.0
+Version: 2.4.1
 Summary: Software Heritage storage manager
 Author-email: Software Heritage developers <swh-devel@inria.fr>
 Project-URL: Homepage, https://gitlab.softwareheritage.org/swh/devel/swh-storage
 Project-URL: Bug Reports, https://gitlab.softwareheritage.org/swh/devel/swh-storage/-/issues
 Project-URL: Funding, https://www.softwareheritage.org/donate
 Project-URL: Documentation, https://docs.softwareheritage.org/devel/swh-storage/
 Project-URL: Source, https://gitlab.softwareheritage.org/swh/devel/swh-storage.git
@@ -34,14 +34,15 @@
 Provides-Extra: testing
 Requires-Dist: hypothesis>=3.11.0; extra == "testing"
 Requires-Dist: pytest>=8.1; extra == "testing"
 Requires-Dist: pytest-mock; extra == "testing"
 Requires-Dist: swh.core[testing]>=3.0.0; extra == "testing"
 Requires-Dist: swh.model[testing]>=6.13.0; extra == "testing"
 Requires-Dist: pytz; extra == "testing"
+Requires-Dist: pytest-postgresql; extra == "testing"
 Requires-Dist: pytest-redis; extra == "testing"
 Requires-Dist: pytest-xdist; extra == "testing"
 Requires-Dist: types-python-dateutil; extra == "testing"
 Requires-Dist: types-pytz; extra == "testing"
 Requires-Dist: types-pyyaml; extra == "testing"
 Requires-Dist: types-redis; extra == "testing"
 Requires-Dist: types-requests; extra == "testing"
```

### Comparing `swh_storage-2.4.0/README.rst` & `swh_storage-2.4.1/README.rst`

 * *Files identical despite different names*

### Comparing `swh_storage-2.4.0/bin/swh-storage-add-dir` & `swh_storage-2.4.1/bin/swh-storage-add-dir`

 * *Files identical despite different names*

### Comparing `swh_storage-2.4.0/docs/Makefile.local` & `swh_storage-2.4.1/docs/Makefile.local`

 * *Files identical despite different names*

### Comparing `swh_storage-2.4.0/docs/archive-copies.rst` & `swh_storage-2.4.1/docs/archive-copies.rst`

 * *Files identical despite different names*

### Comparing `swh_storage-2.4.0/docs/extrinsic-metadata-specification.rst` & `swh_storage-2.4.1/docs/extrinsic-metadata-specification.rst`

 * *Files identical despite different names*

### Comparing `swh_storage-2.4.0/docs/images/swh-archive-copies.dia` & `swh_storage-2.4.1/docs/images/swh-archive-copies.dia`

 * *Files identical despite different names*

### Comparing `swh_storage-2.4.0/docs/index.rst` & `swh_storage-2.4.1/docs/index.rst`

 * *Files identical despite different names*

### Comparing `swh_storage-2.4.0/docs/object-masking.rst` & `swh_storage-2.4.1/docs/object-masking.rst`

 * *Files identical despite different names*

### Comparing `swh_storage-2.4.0/mypy.ini` & `swh_storage-2.4.1/mypy.ini`

 * *Files identical despite different names*

### Comparing `swh_storage-2.4.0/pyproject.toml` & `swh_storage-2.4.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `swh_storage-2.4.0/sql/Makefile` & `swh_storage-2.4.1/sql/Makefile`

 * *Files identical despite different names*

### Comparing `swh_storage-2.4.0/sql/TODO` & `swh_storage-2.4.1/sql/TODO`

 * *Files identical despite different names*

### Comparing `swh_storage-2.4.0/sql/bin/db-upgrade` & `swh_storage-2.4.1/sql/bin/db-upgrade`

 * *Files identical despite different names*

### Comparing `swh_storage-2.4.0/sql/bin/dot_add_content` & `swh_storage-2.4.1/sql/bin/dot_add_content`

 * *Files identical despite different names*

### Comparing `swh_storage-2.4.0/sql/clusters.dot` & `swh_storage-2.4.1/sql/clusters.dot`

 * *Files identical despite different names*

### Comparing `swh_storage-2.4.0/sql/json/fetch_history.result.schema.json` & `swh_storage-2.4.1/sql/json/fetch_history.result.schema.json`

 * *Files identical despite different names*

### Comparing `swh_storage-2.4.0/sql/json/origin_visit.metadata.json` & `swh_storage-2.4.1/sql/json/origin_visit.metadata.json`

 * *Files identical despite different names*

### Comparing `swh_storage-2.4.0/swh/storage/__init__.py` & `swh_storage-2.4.1/swh/storage/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,14 +7,17 @@
 from typing import TYPE_CHECKING, Any, Dict, List
 import warnings
 
 if TYPE_CHECKING:
     from .interface import StorageInterface
 
 
+StorageSpec = Dict[str, Any]
+
+
 def get_storage(cls: str, **kwargs) -> "StorageInterface":
     """Get a storage object of class ``cls`` with arguments ``**kwargs``.
     ``cls`` must be one of the ``swh.storage.classes`` `entry-points
     <https://setuptools.pypa.io/en/latest/userguide/entry_point.html>`_
 
     Args:
         cls (str):
```

### Comparing `swh_storage-2.4.0/swh/storage/algos/diff.py` & `swh_storage-2.4.1/swh/storage/algos/diff.py`

 * *Files identical despite different names*

### Comparing `swh_storage-2.4.0/swh/storage/algos/dir_iterators.py` & `swh_storage-2.4.1/swh/storage/algos/dir_iterators.py`

 * *Files identical despite different names*

### Comparing `swh_storage-2.4.0/swh/storage/algos/directory.py` & `swh_storage-2.4.1/swh/storage/algos/directory.py`

 * *Files identical despite different names*

### Comparing `swh_storage-2.4.0/swh/storage/algos/discovery.py` & `swh_storage-2.4.1/swh/storage/algos/discovery.py`

 * *Files identical despite different names*

### Comparing `swh_storage-2.4.0/swh/storage/algos/origin.py` & `swh_storage-2.4.1/swh/storage/algos/origin.py`

 * *Files identical despite different names*

### Comparing `swh_storage-2.4.0/swh/storage/algos/revisions_walker.py` & `swh_storage-2.4.1/swh/storage/algos/revisions_walker.py`

 * *Files identical despite different names*

### Comparing `swh_storage-2.4.0/swh/storage/algos/snapshot.py` & `swh_storage-2.4.1/swh/storage/algos/snapshot.py`

 * *Files 2% similar despite different names*

```diff
@@ -50,14 +50,15 @@
 
 
 def snapshot_get_latest(
     storage: StorageInterface,
     origin: str,
     allowed_statuses: Optional[List[str]] = None,
     branches_count: Optional[int] = None,
+    visit_type: Optional[str] = None,
 ) -> Optional[Snapshot]:
     """Get the latest snapshot for the given origin, optionally only from visits that have
     one of the given allowed_statuses.
 
     The branches of the snapshot are iterated in the lexicographical
     order of their names.
 
@@ -67,27 +68,30 @@
         allowed_statuses: list of visit statuses considered
             to find the latest snapshot for the visit. For instance,
             ``allowed_statuses=['full']`` will only consider visits that
             have successfully run to completion.
         branches_count: Optional parameter to retrieve snapshot with all branches
             (default behavior when None) or not. If set to positive number, the snapshot
             will be partial with only that number of branches.
+        visit_type: Optional parameter to retrieve snapshot produced by a specific
+            visit type
 
     Raises:
         ValueError if branches_count is not a positive value
 
     Returns:
         The snapshot object if one is found matching the criteria or None.
 
     """
     visit_status = origin_get_latest_visit_status(
         storage,
         origin,
         allowed_statuses=allowed_statuses,
         require_snapshot=True,
+        type=visit_type,
     )
     if not visit_status:
         return None
 
     snapshot_id = visit_status.snapshot
     if not snapshot_id:
         return None
```

### Comparing `swh_storage-2.4.0/swh/storage/api/client.py` & `swh_storage-2.4.1/swh/storage/api/client.py`

 * *Files identical despite different names*

### Comparing `swh_storage-2.4.0/swh/storage/api/serializers.py` & `swh_storage-2.4.1/swh/storage/api/serializers.py`

 * *Files identical despite different names*

### Comparing `swh_storage-2.4.0/swh/storage/api/server.py` & `swh_storage-2.4.1/swh/storage/api/server.py`

 * *Files identical despite different names*

### Comparing `swh_storage-2.4.0/swh/storage/backfill.py` & `swh_storage-2.4.1/swh/storage/backfill.py`

 * *Files identical despite different names*

### Comparing `swh_storage-2.4.0/swh/storage/cassandra/common.py` & `swh_storage-2.4.1/swh/storage/cassandra/common.py`

 * *Files identical despite different names*

### Comparing `swh_storage-2.4.0/swh/storage/cassandra/converters.py` & `swh_storage-2.4.1/swh/storage/cassandra/converters.py`

 * *Files identical despite different names*

### Comparing `swh_storage-2.4.0/swh/storage/cassandra/cql.py` & `swh_storage-2.4.1/swh/storage/cassandra/cql.py`

 * *Files identical despite different names*

### Comparing `swh_storage-2.4.0/swh/storage/cassandra/model.py` & `swh_storage-2.4.1/swh/storage/cassandra/model.py`

 * *Files 0% similar despite different names*

```diff
@@ -92,15 +92,15 @@
     )
 
     sha1: bytes
     sha1_git: bytes
     sha256: bytes
     blake2s256: bytes
     length: int
-    ctime: datetime.datetime
+    ctime: Optional[datetime.datetime]
     """creation time, i.e. time of (first) injection into the storage"""
     status: str
 
 
 @dataclasses.dataclass
 class SkippedContentRow(BaseRow):
     TABLE = "skipped_content"
```

### Comparing `swh_storage-2.4.0/swh/storage/cassandra/schema.py` & `swh_storage-2.4.1/swh/storage/cassandra/schema.py`

 * *Files identical despite different names*

### Comparing `swh_storage-2.4.0/swh/storage/cassandra/storage.py` & `swh_storage-2.4.1/swh/storage/cassandra/storage.py`

 * *Files 0% similar despite different names*

```diff
@@ -231,15 +231,15 @@
     def keyspace(self) -> str:
         return self._keyspace
 
     @property
     def port(self) -> int:
         return self._port
 
-    def _set_cql_runner(self):
+    def _set_cql_runner(self) -> None:
         """Used by tests when they need to reset the CqlRunner"""
         self._cql_runner: CqlRunner = CqlRunner(
             self._hosts,
             self._keyspace,
             self._port,
             self._consistency_level,
             self._auth_provider,
```

### Comparing `swh_storage-2.4.0/swh/storage/cli.py` & `swh_storage-2.4.1/swh/storage/cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # License: GNU General Public License version 3, or any later version
 # See top-level LICENSE file for more information
 
 # WARNING: do not import unnecessary things here to keep cli startup time under
 # control
 import logging
 import os
-from typing import Dict, Optional, Tuple
+from typing import IO, Callable, Dict, Optional, Tuple, Union, cast
 
 import click
 
 from swh.core.cli import CONTEXT_SETTINGS
 from swh.core.cli import swh as swh_cli_group
 
 try:
@@ -223,15 +223,20 @@
     type=click.File("r"),
     help=(
         "File of SWHIDs of objects that are known to have invalid hashes "
         "but still need to be replayed."
     ),
 )
 @click.pass_context
-def replay(ctx, stop_after_objects, object_types, invalid_hashes_file):
+def replay(
+    ctx: click.Context,
+    stop_after_objects: int,
+    object_types: str,
+    invalid_hashes_file: IO,
+):
     """Fill a Storage by reading a Journal.
 
     This is typically used for a mirror configuration, reading the Software
     Heritage kafka journal to retrieve objects of the Software Heritage main
     storage to feed a replication storage. There can be several 'replayers'
     filling a Storage as long as they use the same `group-id`.
 
@@ -287,45 +292,50 @@
 
     if not validate and reporter:
         ctx.fail(
             "Invalid configuration: you cannot have 'error_reporter' set if "
             "'privileged' is False; we cannot validate anonymized objects."
         )
 
-    known_mismatched_hashes: Optional[Tuple[Tuple[str, bytes]]] = None
+    KMH = Optional[Tuple[Tuple[str, bytes, bytes]]]
+
+    known_mismatched_hashes: KMH = None
     if validate and invalid_hashes_file:
         inv_obj_ids = (
             row.strip().split(",") for row in invalid_hashes_file if row.strip()
         )
         swhids = (
             (CoreSWHID.from_string(swhid.strip()), bytes.fromhex(computed_id.strip()))
             for swhid, computed_id in inv_obj_ids
         )
 
-        known_mismatched_hashes = tuple(
-            (swhid.object_type.name.lower(), swhid.object_id, computed_id)
-            for swhid, computed_id in swhids
+        known_mismatched_hashes = cast(
+            KMH,
+            tuple(
+                (swhid.object_type.name.lower(), swhid.object_id, computed_id)
+                for swhid, computed_id in swhids
+            ),
         )
 
     deserializer = ModelObjectDeserializer(
-        reporter=reporter,
+        reporter=cast(Union[Callable[[str, bytes], None], None], reporter),
         validate=validate,
         known_mismatched_hashes=known_mismatched_hashes,
     )
 
     client_cfg["value_deserializer"] = deserializer.convert
     if object_types:
         client_cfg["object_types"] = object_types
     if stop_after_objects:
         client_cfg["stop_after_objects"] = stop_after_objects
 
     try:
         client = get_journal_client(**client_cfg)
     except ValueError as exc:
-        ctx.fail(exc)
+        ctx.fail(str(exc))
 
     worker_fn = functools.partial(process_replay_objects, storage=storage)
 
     if notify:
         notify("READY=1")
 
     try:
```

### Comparing `swh_storage-2.4.0/swh/storage/exc.py` & `swh_storage-2.4.1/swh/storage/exc.py`

 * *Files identical despite different names*

### Comparing `swh_storage-2.4.0/swh/storage/fixer.py` & `swh_storage-2.4.1/swh/storage/fixer.py`

 * *Files identical despite different names*

### Comparing `swh_storage-2.4.0/swh/storage/in_memory.py` & `swh_storage-2.4.1/swh/storage/in_memory.py`

 * *Files identical despite different names*

### Comparing `swh_storage-2.4.0/swh/storage/interface.py` & `swh_storage-2.4.1/swh/storage/interface.py`

 * *Files identical despite different names*

### Comparing `swh_storage-2.4.0/swh/storage/metrics.py` & `swh_storage-2.4.1/swh/storage/metrics.py`

 * *Files identical despite different names*

### Comparing `swh_storage-2.4.0/swh/storage/migrate_extrinsic_metadata.py` & `swh_storage-2.4.1/swh/storage/migrate_extrinsic_metadata.py`

 * *Files identical despite different names*

### Comparing `swh_storage-2.4.0/swh/storage/objstorage.py` & `swh_storage-2.4.1/swh/storage/objstorage.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,26 +7,26 @@
 import warnings
 
 from swh.model.hashutil import DEFAULT_ALGORITHMS
 from swh.model.model import Content, MissingData, Sha1
 from swh.objstorage.exc import ObjNotFoundError
 from swh.objstorage.factory import get_objstorage
 from swh.objstorage.interface import CompositeObjId
-from swh.storage.interface import HashDict
+from swh.storage.interface import HashDict, StorageInterface
 
 from .exc import StorageArgumentException
 
 
 class ObjStorage:
     """Objstorage collaborator in charge of adding objects to
     the objstorage.
 
     """
 
-    def __init__(self, storage, objstorage_config: Optional[Dict]):
+    def __init__(self, storage: StorageInterface, objstorage_config: Optional[Dict]):
         self.storage = storage
         self.warn_usage = False
         if objstorage_config is None:
             objstorage_config = {"cls": "noop"}
             self.warn_usage = True
         self.objstorage = get_objstorage(**objstorage_config)
```

### Comparing `swh_storage-2.4.0/swh/storage/postgresql/converters.py` & `swh_storage-2.4.1/swh/storage/postgresql/converters.py`

 * *Files identical despite different names*

### Comparing `swh_storage-2.4.0/swh/storage/postgresql/db.py` & `swh_storage-2.4.1/swh/storage/postgresql/db.py`

 * *Files identical despite different names*

### Comparing `swh_storage-2.4.0/swh/storage/postgresql/storage.py` & `swh_storage-2.4.1/swh/storage/postgresql/storage.py`

 * *Files 0% similar despite different names*

```diff
@@ -369,4003 +369,4012 @@
 00001700: 656e 636f 6d70 6173 7369 6e67 2044 4220  encompassing DB 
 00001710: 616e 6420 6f62 6a65 6374 2073 746f 7261  and object stora
 00001720: 6765 2222 220a 0a20 2020 2063 7572 7265  ge"""..    curre
 00001730: 6e74 5f76 6572 7369 6f6e 3a20 696e 7420  nt_version: int 
 00001740: 3d20 3139 330a 0a20 2020 2064 6566 205f  = 193..    def _
 00001750: 5f69 6e69 745f 5f28 0a20 2020 2020 2020  _init__(.       
 00001760: 2073 656c 662c 0a20 2020 2020 2020 2064   self,.        d
-00001770: 622c 0a20 2020 2020 2020 206f 626a 7374  b,.        objst
-00001780: 6f72 6167 653d 4e6f 6e65 2c0a 2020 2020  orage=None,.    
-00001790: 2020 2020 6d69 6e5f 706f 6f6c 5f63 6f6e      min_pool_con
-000017a0: 6e73 3d31 2c0a 2020 2020 2020 2020 6d61  ns=1,.        ma
-000017b0: 785f 706f 6f6c 5f63 6f6e 6e73 3d31 302c  x_pool_conns=10,
-000017c0: 0a20 2020 2020 2020 206a 6f75 726e 616c  .        journal
-000017d0: 5f77 7269 7465 723d 4e6f 6e65 2c0a 2020  _writer=None,.  
-000017e0: 2020 2020 2020 7175 6572 795f 6f70 7469        query_opti
-000017f0: 6f6e 733d 4e6f 6e65 2c0a 2020 2020 293a  ons=None,.    ):
-00001800: 0a20 2020 2020 2020 2022 2222 496e 7374  .        """Inst
-00001810: 616e 7469 6174 6520 6120 7374 6f72 6167  antiate a storag
-00001820: 6520 696e 7374 616e 6365 2062 6163 6b65  e instance backe
-00001830: 6420 6279 2061 2050 6f73 7467 7265 5351  d by a PostgreSQ
-00001840: 4c20 6461 7461 6261 7365 2061 6e64 2061  L database and a
-00001850: 6e0a 2020 2020 2020 2020 6f62 6a73 746f  n.        objsto
-00001860: 7261 6765 2e0a 0a20 2020 2020 2020 2057  rage...        W
-00001870: 6865 6e20 6060 6462 6060 2069 7320 7061  hen ``db`` is pa
-00001880: 7373 6564 2061 7320 6120 636f 6e6e 6563  ssed as a connec
-00001890: 7469 6f6e 2073 7472 696e 672c 2074 6865  tion string, the
-000018a0: 6e20 7468 6973 206d 6f64 756c 6520 6175  n this module au
-000018b0: 746f 6d61 7469 6361 6c6c 790a 2020 2020  tomatically.    
-000018c0: 2020 2020 6d61 6e61 6765 7320 6120 636f      manages a co
-000018d0: 6e6e 6563 7469 6f6e 2070 6f6f 6c20 6265  nnection pool be
-000018e0: 7477 6565 6e20 6060 6d69 6e5f 706f 6f6c  tween ``min_pool
-000018f0: 5f63 6f6e 6e73 6060 2061 6e64 2060 606d  _conns`` and ``m
-00001900: 6178 5f70 6f6f 6c5f 636f 6e6e 7360 602e  ax_pool_conns``.
-00001910: 0a20 2020 2020 2020 2057 6865 6e20 6060  .        When ``
-00001920: 6462 6060 2069 7320 616e 2065 7870 6c69  db`` is an expli
-00001930: 6369 7420 7073 7963 6f70 6732 2063 6f6e  cit psycopg2 con
-00001940: 6e65 6374 696f 6e2c 2074 6865 6e20 6060  nection, then ``
-00001950: 6d69 6e5f 706f 6f6c 5f63 6f6e 6e73 6060  min_pool_conns``
-00001960: 2061 6e64 0a20 2020 2020 2020 2060 606d   and.        ``m
-00001970: 6178 5f70 6f6f 6c5f 636f 6e6e 7360 6020  ax_pool_conns`` 
-00001980: 6172 6520 6967 6e6f 7265 6420 616e 6420  are ignored and 
-00001990: 7468 6520 636f 6e6e 6563 7469 6f6e 2069  the connection i
-000019a0: 7320 7573 6564 2064 6972 6563 746c 792e  s used directly.
-000019b0: 0a0a 2020 2020 2020 2020 4172 6773 3a0a  ..        Args:.
-000019c0: 2020 2020 2020 2020 2020 2020 6462 3a20              db: 
-000019d0: 6569 7468 6572 2061 206c 6962 7071 2063  either a libpq c
-000019e0: 6f6e 6e65 6374 696f 6e20 7374 7269 6e67  onnection string
-000019f0: 2c20 6f72 2061 2070 7379 636f 7067 3220  , or a psycopg2 
-00001a00: 636f 6e6e 6563 7469 6f6e 0a20 2020 2020  connection.     
-00001a10: 2020 2020 2020 206f 626a 7374 6f72 6167         objstorag
-00001a20: 653a 2063 6f6e 6669 6775 7261 7469 6f6e  e: configuration
-00001a30: 2066 6f72 2074 6865 2062 6163 6b65 6e64   for the backend
-00001a40: 203a 636c 6173 733a 604f 626a 5374 6f72   :class:`ObjStor
-00001a50: 6167 6560 3b20 6966 2075 6e73 6574 2c0a  age`; if unset,.
-00001a60: 2020 2020 2020 2020 2020 2020 2020 2075                 u
-00001a70: 7365 2061 204e 6f6f 704f 626a 5374 6f72  se a NoopObjStor
-00001a80: 6167 650a 2020 2020 2020 2020 2020 2020  age.            
-00001a90: 6d69 6e5f 706f 6f6c 5f63 6f6e 6e73 3a20  min_pool_conns: 
-00001aa0: 6d69 6e20 6e75 6d62 6572 206f 6620 636f  min number of co
-00001ab0: 6e6e 6563 7469 6f6e 7320 696e 2074 6865  nnections in the
-00001ac0: 2070 7379 636f 7067 3220 706f 6f6c 0a20   psycopg2 pool. 
-00001ad0: 2020 2020 2020 2020 2020 206d 6178 5f70             max_p
-00001ae0: 6f6f 6c5f 636f 6e6e 733a 206d 6178 206e  ool_conns: max n
-00001af0: 756d 6265 7220 6f66 2063 6f6e 6e65 6374  umber of connect
-00001b00: 696f 6e73 2069 6e20 7468 6520 7073 7963  ions in the psyc
-00001b10: 6f70 6732 2070 6f6f 6c0a 2020 2020 2020  opg2 pool.      
-00001b20: 2020 2020 2020 6a6f 7572 6e61 6c5f 7772        journal_wr
-00001b30: 6974 6572 3a20 636f 6e66 6967 7572 6174  iter: configurat
-00001b40: 696f 6e20 666f 7220 7468 6520 3a63 6c61  ion for the :cla
-00001b50: 7373 3a60 4a6f 7572 6e61 6c57 7269 7465  ss:`JournalWrite
-00001b60: 7260 0a20 2020 2020 2020 2020 2020 2071  r`.            q
-00001b70: 7565 7279 5f6f 7074 696f 6e73 3a20 636f  uery_options: co
-00001b80: 6e66 6967 7572 6174 696f 6e20 666f 7220  nfiguration for 
-00001b90: 7468 6520 7371 6c20 636f 6e6e 6563 7469  the sql connecti
-00001ba0: 6f6e 733b 206b 6579 7320 6f66 2074 6865  ons; keys of the
-00001bb0: 2064 6963 7420 6172 650a 2020 2020 2020   dict are.      
-00001bc0: 2020 2020 2020 2020 2074 6865 206d 6574           the met
-00001bd0: 686f 6420 6e61 6d65 7320 6465 636f 7261  hod names decora
-00001be0: 7465 6420 7769 7468 203a 6675 6e63 3a60  ted with :func:`
-00001bf0: 6462 5f74 7261 6e73 6163 7469 6f6e 6020  db_transaction` 
-00001c00: 6f72 0a20 2020 2020 2020 2020 2020 2020  or.             
-00001c10: 2020 3a66 756e 633a 6064 625f 7472 616e    :func:`db_tran
-00001c20: 7361 6374 696f 6e5f 6765 6e65 7261 746f  saction_generato
-00001c30: 7260 2028 6567 2e20 3a66 756e 633a 6063  r` (eg. :func:`c
-00001c40: 6f6e 7465 6e74 5f66 696e 6460 292c 2061  ontent_find`), a
-00001c50: 6e64 2076 616c 7565 730a 2020 2020 2020  nd values.      
-00001c60: 2020 2020 2020 2020 2061 7265 2064 6963           are dic
-00001c70: 7473 2028 636f 6e66 6967 5f6e 616d 652c  ts (config_name,
-00001c80: 2063 6f6e 6669 675f 7661 6c75 6529 2075   config_value) u
-00001c90: 7365 6420 746f 2063 6f6e 6669 6775 7265  sed to configure
-00001ca0: 2074 6865 2073 716c 0a20 2020 2020 2020   the sql.       
-00001cb0: 2020 2020 2020 2020 636f 6e6e 6563 7469          connecti
-00001cc0: 6f6e 2066 6f72 2074 6865 206d 6574 686f  on for the metho
-00001cd0: 645f 6e61 6d65 2e20 466f 7220 6578 616d  d_name. For exam
-00001ce0: 706c 652c 2075 7369 6e67 3a3a 0a0a 2020  ple, using::..  
-00001cf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001d00: 7b22 636f 6e74 656e 745f 6765 7422 3a20  {"content_get": 
-00001d10: 7b22 7374 6174 656d 656e 745f 7469 6d65  {"statement_time
-00001d20: 6f75 7422 3a20 3530 3030 7d7d 0a0a 2020  out": 5000}}..  
-00001d30: 2020 2020 2020 2020 2020 2020 2077 696c               wil
-00001d40: 6c20 6f76 6572 7269 6465 2074 6865 2064  l override the d
-00001d50: 6566 6175 6c74 2073 7461 7465 6d65 6e74  efault statement
-00001d60: 2074 696d 656f 7574 2066 6f72 2074 6865   timeout for the
-00001d70: 203a 6675 6e63 3a60 636f 6e74 656e 745f   :func:`content_
-00001d80: 6765 7460 0a20 2020 2020 2020 2020 2020  get`.           
-00001d90: 2020 2020 656e 6470 6f69 6e74 2066 726f      endpoint fro
-00001da0: 6d20 3530 306d 7320 746f 2035 3030 306d  m 500ms to 5000m
-00001db0: 732e 0a0a 2020 2020 2020 2020 2020 2020  s...            
-00001dc0: 2020 2053 6565 203a 6d6f 643a 6073 7768     See :mod:`swh
-00001dd0: 2e63 6f72 652e 6462 2e63 6f6d 6d6f 6e60  .core.db.common`
-00001de0: 2066 6f72 206d 6f72 6520 6465 7461 696c   for more detail
-00001df0: 732e 0a0a 2020 2020 2020 2020 2222 220a  s...        """.
-00001e00: 0a20 2020 2020 2020 2074 7279 3a0a 2020  .        try:.  
-00001e10: 2020 2020 2020 2020 2020 6966 2069 7369            if isi
-00001e20: 6e73 7461 6e63 6528 6462 2c20 7073 7963  nstance(db, psyc
-00001e30: 6f70 6732 2e65 7874 656e 7369 6f6e 732e  opg2.extensions.
-00001e40: 636f 6e6e 6563 7469 6f6e 293a 0a20 2020  connection):.   
-00001e50: 2020 2020 2020 2020 2020 2020 2073 656c               sel
-00001e60: 662e 5f70 6f6f 6c20 3d20 4e6f 6e65 0a20  f._pool = None. 
-00001e70: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-00001e80: 656c 662e 5f64 6220 3d20 4462 2864 6229  elf._db = Db(db)
-00001e90: 0a0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00001ea0: 2020 2320 5365 6520 636f 6d6d 656e 7420    # See comment 
-00001eb0: 6265 6c6f 770a 2020 2020 2020 2020 2020  below.          
-00001ec0: 2020 2020 2020 7365 6c66 2e5f 6462 2e63        self._db.c
-00001ed0: 7572 736f 7228 292e 6578 6563 7574 6528  ursor().execute(
-00001ee0: 2253 4554 2054 494d 4520 5a4f 4e45 2027  "SET TIME ZONE '
-00001ef0: 5554 4327 2229 0a20 2020 2020 2020 2020  UTC'").         
-00001f00: 2020 2065 6c73 653a 0a20 2020 2020 2020     else:.       
-00001f10: 2020 2020 2020 2020 2073 656c 662e 5f70           self._p
-00001f20: 6f6f 6c20 3d20 7073 7963 6f70 6732 2e70  ool = psycopg2.p
-00001f30: 6f6f 6c2e 5468 7265 6164 6564 436f 6e6e  ool.ThreadedConn
-00001f40: 6563 7469 6f6e 506f 6f6c 280a 2020 2020  ectionPool(.    
-00001f50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001f60: 6d69 6e5f 706f 6f6c 5f63 6f6e 6e73 2c20  min_pool_conns, 
-00001f70: 6d61 785f 706f 6f6c 5f63 6f6e 6e73 2c20  max_pool_conns, 
-00001f80: 6462 0a20 2020 2020 2020 2020 2020 2020  db.             
-00001f90: 2020 2029 0a20 2020 2020 2020 2020 2020     ).           
-00001fa0: 2020 2020 2073 656c 662e 5f64 6220 3d20       self._db = 
-00001fb0: 4e6f 6e65 0a20 2020 2020 2020 2065 7863  None.        exc
-00001fc0: 6570 7420 7073 7963 6f70 6732 2e4f 7065  ept psycopg2.Ope
-00001fd0: 7261 7469 6f6e 616c 4572 726f 7220 6173  rationalError as
-00001fe0: 2065 3a0a 2020 2020 2020 2020 2020 2020   e:.            
-00001ff0: 7261 6973 6520 5374 6f72 6167 6544 4245  raise StorageDBE
-00002000: 7272 6f72 2865 290a 2020 2020 2020 2020  rror(e).        
-00002010: 7365 6c66 2e6a 6f75 726e 616c 5f77 7269  self.journal_wri
-00002020: 7465 7220 3d20 4a6f 7572 6e61 6c57 7269  ter = JournalWri
-00002030: 7465 7228 6a6f 7572 6e61 6c5f 7772 6974  ter(journal_writ
-00002040: 6572 290a 2020 2020 2020 2020 7365 6c66  er).        self
-00002050: 2e6f 626a 7374 6f72 6167 6520 3d20 4f62  .objstorage = Ob
-00002060: 6a53 746f 7261 6765 2873 656c 662c 206f  jStorage(self, o
-00002070: 626a 7374 6f72 6167 6529 0a20 2020 2020  bjstorage).     
-00002080: 2020 2073 656c 662e 7175 6572 795f 6f70     self.query_op
-00002090: 7469 6f6e 7320 3d20 7175 6572 795f 6f70  tions = query_op
-000020a0: 7469 6f6e 730a 2020 2020 2020 2020 7365  tions.        se
-000020b0: 6c66 2e5f 666c 6176 6f72 3a20 4f70 7469  lf._flavor: Opti
-000020c0: 6f6e 616c 5b73 7472 5d20 3d20 4e6f 6e65  onal[str] = None
-000020d0: 0a0a 2020 2020 2323 2323 2323 2323 2323  ..    ##########
-000020e0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-000020f0: 0a20 2020 2023 2055 7469 6c69 7469 6573  .    # Utilities
-00002100: 0a20 2020 2023 2323 2323 2323 2323 2323  .    ###########
-00002110: 2323 2323 2323 2323 2323 2323 2323 230a  ###############.
-00002120: 0a20 2020 2064 6566 2067 6574 5f64 6228  .    def get_db(
-00002130: 7365 6c66 293a 0a20 2020 2020 2020 2069  self):.        i
-00002140: 6620 7365 6c66 2e5f 6462 3a0a 2020 2020  f self._db:.    
-00002150: 2020 2020 2020 2020 7265 7475 726e 2073          return s
-00002160: 656c 662e 5f64 620a 2020 2020 2020 2020  elf._db.        
-00002170: 656c 7365 3a0a 2020 2020 2020 2020 2020  else:.          
-00002180: 2020 6462 203d 2044 622e 6672 6f6d 5f70    db = Db.from_p
-00002190: 6f6f 6c28 7365 6c66 2e5f 706f 6f6c 290a  ool(self._pool).
-000021a0: 0a20 2020 2020 2020 2020 2020 2023 2057  .            # W
-000021b0: 6f72 6b61 726f 756e 6420 666f 7220 7073  orkaround for ps
-000021c0: 7963 6f70 6732 203c 2032 2e39 2e30 206e  ycopg2 < 2.9.0 n
-000021d0: 6f74 2068 616e 646c 696e 6720 6672 6163  ot handling frac
-000021e0: 7469 6f6e 616c 2074 696d 657a 6f6e 6573  tional timezones
-000021f0: 2c0a 2020 2020 2020 2020 2020 2020 2320  ,.            # 
-00002200: 7768 6963 6820 6d61 7920 6861 7070 656e  which may happen
-00002210: 206f 6e20 6f6c 6420 7265 7669 7369 6f6e   on old revision
-00002220: 2f72 656c 6561 7365 2064 6174 6573 206f  /release dates o
-00002230: 6e20 7379 7374 656d 7320 636f 6e66 6967  n systems config
-00002240: 7572 6564 0a20 2020 2020 2020 2020 2020  ured.           
-00002250: 2023 2077 6974 6820 6e6f 6e2d 5554 4320   # with non-UTC 
-00002260: 7469 6d65 7a6f 6e65 732e 0a20 2020 2020  timezones..     
-00002270: 2020 2020 2020 2023 2068 7474 7073 3a2f         # https:/
-00002280: 2f77 7777 2e70 7379 636f 7067 2e6f 7267  /www.psycopg.org
-00002290: 2f64 6f63 732f 7573 6167 652e 6874 6d6c  /docs/usage.html
-000022a0: 2374 696d 652d 7a6f 6e65 732d 6861 6e64  #time-zones-hand
-000022b0: 6c69 6e67 0a20 2020 2020 2020 2020 2020  ling.           
-000022c0: 2064 622e 6375 7273 6f72 2829 2e65 7865   db.cursor().exe
-000022d0: 6375 7465 2822 5345 5420 5449 4d45 205a  cute("SET TIME Z
-000022e0: 4f4e 4520 2755 5443 2722 290a 0a20 2020  ONE 'UTC'")..   
-000022f0: 2020 2020 2020 2020 2072 6574 7572 6e20           return 
-00002300: 6462 0a0a 2020 2020 6465 6620 7075 745f  db..    def put_
-00002310: 6462 2873 656c 662c 2064 6229 3a0a 2020  db(self, db):.  
-00002320: 2020 2020 2020 6966 2064 6220 6973 206e        if db is n
-00002330: 6f74 2073 656c 662e 5f64 623a 0a20 2020  ot self._db:.   
-00002340: 2020 2020 2020 2020 2064 622e 7075 745f           db.put_
-00002350: 636f 6e6e 2829 0a0a 2020 2020 4063 6f6e  conn()..    @con
-00002360: 7465 7874 6d61 6e61 6765 720a 2020 2020  textmanager.    
-00002370: 6465 6620 6462 2873 656c 6629 3a0a 2020  def db(self):.  
-00002380: 2020 2020 2020 6462 203d 204e 6f6e 650a        db = None.
-00002390: 2020 2020 2020 2020 7472 793a 0a20 2020          try:.   
-000023a0: 2020 2020 2020 2020 2064 6220 3d20 7365           db = se
-000023b0: 6c66 2e67 6574 5f64 6228 290a 2020 2020  lf.get_db().    
-000023c0: 2020 2020 2020 2020 7969 656c 6420 6462          yield db
-000023d0: 0a20 2020 2020 2020 2066 696e 616c 6c79  .        finally
-000023e0: 3a0a 2020 2020 2020 2020 2020 2020 6966  :.            if
-000023f0: 2064 623a 0a20 2020 2020 2020 2020 2020   db:.           
-00002400: 2020 2020 2073 656c 662e 7075 745f 6462       self.put_db
-00002410: 2864 6229 0a0a 2020 2020 4064 625f 7472  (db)..    @db_tr
-00002420: 616e 7361 6374 696f 6e28 290a 2020 2020  ansaction().    
-00002430: 6465 6620 6765 745f 666c 6176 6f72 2873  def get_flavor(s
-00002440: 656c 662c 202a 2c20 6462 3a20 4462 2c20  elf, *, db: Db, 
-00002450: 6375 723d 4e6f 6e65 2920 2d3e 2073 7472  cur=None) -> str
-00002460: 3a0a 2020 2020 2020 2020 666c 6176 6f72  :.        flavor
-00002470: 203d 2073 7768 5f64 625f 666c 6176 6f72   = swh_db_flavor
-00002480: 2864 622e 636f 6e6e 2e64 736e 290a 2020  (db.conn.dsn).  
-00002490: 2020 2020 2020 6173 7365 7274 2066 6c61        assert fla
-000024a0: 766f 7220 6973 206e 6f74 204e 6f6e 650a  vor is not None.
-000024b0: 2020 2020 2020 2020 7265 7475 726e 2066          return f
-000024c0: 6c61 766f 720a 0a20 2020 2040 7072 6f70  lavor..    @prop
-000024d0: 6572 7479 0a20 2020 2064 6566 2066 6c61  erty.    def fla
-000024e0: 766f 7228 7365 6c66 2920 2d3e 2073 7472  vor(self) -> str
-000024f0: 3a0a 2020 2020 2020 2020 6966 2073 656c  :.        if sel
-00002500: 662e 5f66 6c61 766f 7220 6973 204e 6f6e  f._flavor is Non
-00002510: 653a 0a20 2020 2020 2020 2020 2020 2073  e:.            s
-00002520: 656c 662e 5f66 6c61 766f 7220 3d20 7365  elf._flavor = se
-00002530: 6c66 2e67 6574 5f66 6c61 766f 7228 290a  lf.get_flavor().
-00002540: 2020 2020 2020 2020 6173 7365 7274 2073          assert s
-00002550: 656c 662e 5f66 6c61 766f 7220 6973 206e  elf._flavor is n
-00002560: 6f74 204e 6f6e 650a 2020 2020 2020 2020  ot None.        
-00002570: 7265 7475 726e 2073 656c 662e 5f66 6c61  return self._fla
-00002580: 766f 720a 0a20 2020 2040 6462 5f74 7261  vor..    @db_tra
-00002590: 6e73 6163 7469 6f6e 2829 0a20 2020 2064  nsaction().    d
-000025a0: 6566 2063 6865 636b 5f63 6f6e 6669 6728  ef check_config(
-000025b0: 7365 6c66 2c20 2a2c 2063 6865 636b 5f77  self, *, check_w
-000025c0: 7269 7465 3a20 626f 6f6c 2c20 6462 3a20  rite: bool, db: 
-000025d0: 4462 2c20 6375 723d 4e6f 6e65 2920 2d3e  Db, cur=None) ->
-000025e0: 2062 6f6f 6c3a 0a20 2020 2020 2020 2069   bool:.        i
-000025f0: 6620 6e6f 7420 7365 6c66 2e6f 626a 7374  f not self.objst
-00002600: 6f72 6167 652e 6368 6563 6b5f 636f 6e66  orage.check_conf
-00002610: 6967 2863 6865 636b 5f77 7269 7465 3d63  ig(check_write=c
-00002620: 6865 636b 5f77 7269 7465 293a 0a20 2020  heck_write):.   
-00002630: 2020 2020 2020 2020 2072 6574 7572 6e20           return 
-00002640: 4661 6c73 650a 0a20 2020 2020 2020 2064  False..        d
-00002650: 6276 6572 7369 6f6e 203d 2073 7768 5f64  bversion = swh_d
-00002660: 625f 7665 7273 696f 6e28 6462 2e63 6f6e  b_version(db.con
-00002670: 6e2e 6473 6e29 0a20 2020 2020 2020 2069  n.dsn).        i
-00002680: 6620 6462 7665 7273 696f 6e20 213d 2073  f dbversion != s
-00002690: 656c 662e 6375 7272 656e 745f 7665 7273  elf.current_vers
-000026a0: 696f 6e3a 0a20 2020 2020 2020 2020 2020  ion:.           
-000026b0: 206c 6f67 6765 722e 7761 726e 696e 6728   logger.warning(
-000026c0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000026d0: 2022 6461 7461 6261 7365 2064 6276 6572   "database dbver
-000026e0: 7369 6f6e 2028 2573 2920 213d 2025 7320  sion (%s) != %s 
-000026f0: 6375 7272 656e 745f 7665 7273 696f 6e20  current_version 
-00002700: 2825 7329 222c 0a20 2020 2020 2020 2020  (%s)",.         
-00002710: 2020 2020 2020 2064 6276 6572 7369 6f6e         dbversion
-00002720: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-00002730: 2020 5f5f 6e61 6d65 5f5f 2c0a 2020 2020    __name__,.    
-00002740: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-00002750: 2e63 7572 7265 6e74 5f76 6572 7369 6f6e  .current_version
-00002760: 2c0a 2020 2020 2020 2020 2020 2020 290a  ,.            ).
-00002770: 2020 2020 2020 2020 2020 2020 7265 7475              retu
-00002780: 726e 2046 616c 7365 0a0a 2020 2020 2020  rn False..      
-00002790: 2020 2320 4368 6563 6b20 7065 726d 6973    # Check permis
-000027a0: 7369 6f6e 7320 6f6e 206f 6e65 206f 6620  sions on one of 
-000027b0: 7468 6520 7461 626c 6573 0a20 2020 2020  the tables.     
-000027c0: 2020 2063 6865 636b 203d 2022 494e 5345     check = "INSE
-000027d0: 5254 2220 6966 2063 6865 636b 5f77 7269  RT" if check_wri
-000027e0: 7465 2065 6c73 6520 2253 454c 4543 5422  te else "SELECT"
-000027f0: 0a0a 2020 2020 2020 2020 6375 722e 6578  ..        cur.ex
-00002800: 6563 7574 6528 2273 656c 6563 7420 6861  ecute("select ha
-00002810: 735f 7461 626c 655f 7072 6976 696c 6567  s_table_privileg
-00002820: 6528 6375 7272 656e 745f 7573 6572 2c20  e(current_user, 
-00002830: 2763 6f6e 7465 6e74 272c 2025 7329 222c  'content', %s)",
-00002840: 2028 6368 6563 6b2c 2929 0a20 2020 2020   (check,)).     
-00002850: 2020 2072 6574 7572 6e20 6375 722e 6665     return cur.fe
-00002860: 7463 686f 6e65 2829 5b30 5d0a 0a20 2020  tchone()[0]..   
-00002870: 2023 2323 2323 2323 2323 2323 2323 2323   ###############
-00002880: 2323 2323 2323 2323 2323 230a 2020 2020  ###########.    
-00002890: 2320 436f 6e74 656e 740a 2020 2020 2323  # Content.    ##
-000028a0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-000028b0: 2323 2323 2323 2323 0a0a 2020 2020 6465  ########..    de
-000028c0: 6620 5f63 6f6e 7465 6e74 5f75 6e69 7175  f _content_uniqu
-000028d0: 655f 6b65 7928 7365 6c66 2c20 6861 7368  e_key(self, hash
-000028e0: 2c20 6462 293a 0a20 2020 2020 2020 2022  , db):.        "
-000028f0: 2222 4769 7665 6e20 6120 6861 7368 2028  ""Given a hash (
-00002900: 7475 706c 6520 6f72 2064 6963 7429 2c20  tuple or dict), 
-00002910: 7265 7475 726e 2061 2075 6e69 7175 6520  return a unique 
-00002920: 6b65 7920 6672 6f6d 2074 6865 0a20 2020  key from the.   
-00002930: 2020 2020 2061 6767 7265 6761 7469 6f6e       aggregation
-00002940: 206f 6620 6b65 7973 2e0a 0a20 2020 2020   of keys...     
-00002950: 2020 2022 2222 0a20 2020 2020 2020 206b     """.        k
-00002960: 6579 7320 3d20 6462 2e63 6f6e 7465 6e74  eys = db.content
-00002970: 5f68 6173 685f 6b65 7973 0a20 2020 2020  _hash_keys.     
-00002980: 2020 2069 6620 6973 696e 7374 616e 6365     if isinstance
-00002990: 2868 6173 682c 2074 7570 6c65 293a 0a20  (hash, tuple):. 
-000029a0: 2020 2020 2020 2020 2020 2072 6574 7572             retur
-000029b0: 6e20 6861 7368 0a20 2020 2020 2020 2072  n hash.        r
-000029c0: 6574 7572 6e20 7475 706c 6528 5b68 6173  eturn tuple([has
-000029d0: 685b 6b5d 2066 6f72 206b 2069 6e20 6b65  h[k] for k in ke
-000029e0: 7973 5d29 0a0a 2020 2020 6465 6620 5f63  ys])..    def _c
-000029f0: 6f6e 7465 6e74 5f61 6464 5f6d 6574 6164  ontent_add_metad
-00002a00: 6174 6128 7365 6c66 2c20 6462 2c20 6375  ata(self, db, cu
-00002a10: 722c 2063 6f6e 7465 6e74 293a 0a20 2020  r, content):.   
-00002a20: 2020 2020 2022 2222 4164 6420 636f 6e74       """Add cont
-00002a30: 656e 7420 746f 2074 6865 2070 6f73 7467  ent to the postg
-00002a40: 7265 7371 6c20 6461 7461 6261 7365 2062  resql database b
-00002a50: 7574 206e 6f74 2074 6865 206f 626a 6563  ut not the objec
-00002a60: 7420 7374 6f72 6167 652e 2222 220a 2020  t storage.""".  
-00002a70: 2020 2020 2020 2320 6372 6561 7465 2074        # create t
-00002a80: 656d 706f 7261 7279 2074 6162 6c65 2066  emporary table f
-00002a90: 6f72 206d 6574 6164 6174 6120 696e 6a65  or metadata inje
-00002aa0: 6374 696f 6e0a 2020 2020 2020 2020 6462  ction.        db
-00002ab0: 2e6d 6b74 656d 7028 2263 6f6e 7465 6e74  .mktemp("content
-00002ac0: 222c 2063 7572 290a 0a20 2020 2020 2020  ", cur)..       
-00002ad0: 2064 622e 636f 7079 5f74 6f28 0a20 2020   db.copy_to(.   
-00002ae0: 2020 2020 2020 2020 2028 632e 746f 5f64           (c.to_d
-00002af0: 6963 7428 2920 666f 7220 6320 696e 2063  ict() for c in c
-00002b00: 6f6e 7465 6e74 292c 2022 746d 705f 636f  ontent), "tmp_co
-00002b10: 6e74 656e 7422 2c20 6462 2e63 6f6e 7465  ntent", db.conte
-00002b20: 6e74 5f61 6464 5f6b 6579 732c 2063 7572  nt_add_keys, cur
-00002b30: 0a20 2020 2020 2020 2029 0a0a 2020 2020  .        )..    
-00002b40: 2020 2020 2320 6d6f 7665 206d 6574 6164      # move metad
-00002b50: 6174 6120 696e 2070 6c61 6365 0a20 2020  ata in place.   
-00002b60: 2020 2020 2074 7279 3a0a 2020 2020 2020       try:.      
-00002b70: 2020 2020 2020 6462 2e63 6f6e 7465 6e74        db.content
-00002b80: 5f61 6464 5f66 726f 6d5f 7465 6d70 2863  _add_from_temp(c
-00002b90: 7572 290a 2020 2020 2020 2020 6578 6365  ur).        exce
-00002ba0: 7074 2070 7379 636f 7067 322e 496e 7465  pt psycopg2.Inte
-00002bb0: 6772 6974 7945 7272 6f72 2061 7320 653a  grityError as e:
-00002bc0: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
-00002bd0: 652e 6469 6167 2e73 716c 7374 6174 6520  e.diag.sqlstate 
-00002be0: 3d3d 2022 3233 3530 3522 2061 6e64 2065  == "23505" and e
-00002bf0: 2e64 6961 672e 7461 626c 655f 6e61 6d65  .diag.table_name
-00002c00: 203d 3d20 2263 6f6e 7465 6e74 223a 0a20   == "content":. 
-00002c10: 2020 2020 2020 2020 2020 2020 2020 206d                 m
-00002c20: 6573 7361 6765 5f64 6574 6169 6c20 3d20  essage_detail = 
-00002c30: 652e 6469 6167 2e6d 6573 7361 6765 5f64  e.diag.message_d
-00002c40: 6574 6169 6c0a 2020 2020 2020 2020 2020  etail.          
-00002c50: 2020 2020 2020 6966 206d 6573 7361 6765        if message
-00002c60: 5f64 6574 6169 6c3a 0a20 2020 2020 2020  _detail:.       
-00002c70: 2020 2020 2020 2020 2020 2020 2068 6173               has
-00002c80: 685f 6e61 6d65 2c20 6861 7368 5f69 6420  h_name, hash_id 
-00002c90: 3d20 6578 7472 6163 745f 636f 6c6c 6973  = extract_collis
-00002ca0: 696f 6e5f 6861 7368 286d 6573 7361 6765  ion_hash(message
-00002cb0: 5f64 6574 6169 6c29 0a20 2020 2020 2020  _detail).       
-00002cc0: 2020 2020 2020 2020 2020 2020 2063 6f6c               col
-00002cd0: 6c69 7369 6f6e 5f63 6f6e 7465 6e74 735f  lision_contents_
-00002ce0: 6861 7368 6573 203d 205b 0a20 2020 2020  hashes = [.     
-00002cf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002d00: 2020 2063 2e68 6173 6865 7328 2920 666f     c.hashes() fo
-00002d10: 7220 6320 696e 2063 6f6e 7465 6e74 2069  r c in content i
-00002d20: 6620 632e 6765 745f 6861 7368 2868 6173  f c.get_hash(has
-00002d30: 685f 6e61 6d65 2920 3d3d 2068 6173 685f  h_name) == hash_
-00002d40: 6964 0a20 2020 2020 2020 2020 2020 2020  id.             
-00002d50: 2020 2020 2020 205d 0a20 2020 2020 2020         ].       
-00002d60: 2020 2020 2020 2020 2065 6c73 653a 0a20           else:. 
-00002d70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002d80: 2020 2063 6f6e 7374 7261 696e 745f 746f     constraint_to
-00002d90: 5f68 6173 685f 6e61 6d65 203d 207b 0a20  _hash_name = {. 
-00002da0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002db0: 2020 2020 2020 2022 636f 6e74 656e 745f         "content_
-00002dc0: 706b 6579 223a 2022 7368 6131 222c 0a20  pkey": "sha1",. 
-00002dd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002de0: 2020 2020 2020 2022 636f 6e74 656e 745f         "content_
-00002df0: 7368 6131 5f67 6974 5f69 6478 223a 2022  sha1_git_idx": "
-00002e00: 7368 6131 5f67 6974 222c 0a20 2020 2020  sha1_git",.     
-00002e10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002e20: 2020 2022 636f 6e74 656e 745f 7368 6132     "content_sha2
-00002e30: 3536 5f69 6478 223a 2022 7368 6132 3536  56_idx": "sha256
-00002e40: 222c 0a20 2020 2020 2020 2020 2020 2020  ",.             
-00002e50: 2020 2020 2020 207d 0a20 2020 2020 2020         }.       
-00002e60: 2020 2020 2020 2020 2020 2020 2068 6173               has
-00002e70: 685f 6e61 6d65 203d 2063 6f6e 7374 7261  h_name = constra
-00002e80: 696e 745f 746f 5f68 6173 685f 6e61 6d65  int_to_hash_name
-00002e90: 2e67 6574 2865 2e64 6961 672e 636f 6e73  .get(e.diag.cons
-00002ea0: 7472 6169 6e74 5f6e 616d 6529 0a20 2020  traint_name).   
-00002eb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002ec0: 2068 6173 685f 6964 203d 204e 6f6e 650a   hash_id = None.
-00002ed0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002ee0: 2020 2020 636f 6c6c 6973 696f 6e5f 636f      collision_co
-00002ef0: 6e74 656e 7473 5f68 6173 6865 7320 3d20  ntents_hashes = 
-00002f00: 4e6f 6e65 0a0a 2020 2020 2020 2020 2020  None..          
-00002f10: 2020 2020 2020 7261 6973 6520 4861 7368        raise Hash
-00002f20: 436f 6c6c 6973 696f 6e28 0a20 2020 2020  Collision(.     
-00002f30: 2020 2020 2020 2020 2020 2020 2020 2068                 h
-00002f40: 6173 685f 6e61 6d65 2c20 6861 7368 5f69  ash_name, hash_i
-00002f50: 642c 2063 6f6c 6c69 7369 6f6e 5f63 6f6e  d, collision_con
-00002f60: 7465 6e74 735f 6861 7368 6573 0a20 2020  tents_hashes.   
-00002f70: 2020 2020 2020 2020 2020 2020 2029 2066               ) f
-00002f80: 726f 6d20 4e6f 6e65 0a20 2020 2020 2020  rom None.       
-00002f90: 2020 2020 2065 6c73 653a 0a20 2020 2020       else:.     
-00002fa0: 2020 2020 2020 2020 2020 2072 6169 7365             raise
-00002fb0: 0a0a 2020 2020 6465 6620 636f 6e74 656e  ..    def conten
-00002fc0: 745f 6164 6428 7365 6c66 2c20 636f 6e74  t_add(self, cont
-00002fd0: 656e 743a 204c 6973 745b 436f 6e74 656e  ent: List[Conten
-00002fe0: 745d 2920 2d3e 2044 6963 745b 7374 722c  t]) -> Dict[str,
-00002ff0: 2069 6e74 5d3a 0a20 2020 2020 2020 2063   int]:.        c
-00003000: 7469 6d65 203d 206e 6f77 2829 0a0a 2020  time = now()..  
-00003010: 2020 2020 2020 636f 6e74 656e 7473 203d        contents =
-00003020: 205b 6174 7472 2e65 766f 6c76 6528 632c   [attr.evolve(c,
-00003030: 2063 7469 6d65 3d63 7469 6d65 2920 666f   ctime=ctime) fo
-00003040: 7220 6320 696e 2063 6f6e 7465 6e74 5d0a  r c in content].
-00003050: 0a20 2020 2020 2020 2023 204d 7573 7420  .        # Must 
-00003060: 6164 6420 746f 2074 6865 206f 626a 7374  add to the objst
-00003070: 6f72 6167 6520 6265 666f 7265 2074 6865  orage before the
-00003080: 2044 4220 616e 6420 6a6f 7572 6e61 6c2e   DB and journal.
-00003090: 204f 7468 6572 7769 7365 3a0a 2020 2020   Otherwise:.    
-000030a0: 2020 2020 2320 312e 2069 6e20 6361 7365      # 1. in case
-000030b0: 206f 6620 6120 6372 6173 6820 7468 6520   of a crash the 
-000030c0: 4442 206d 6179 2022 6265 6c69 6576 6522  DB may "believe"
-000030d0: 2077 6520 6861 7665 2074 6865 2063 6f6e   we have the con
-000030e0: 7465 6e74 2c20 6275 740a 2020 2020 2020  tent, but.      
-000030f0: 2020 2320 2020 2077 6520 6469 646e 2774    #    we didn't
-00003100: 2068 6176 6520 7469 6d65 2074 6f20 7772   have time to wr
-00003110: 6974 6520 746f 2074 6865 206f 626a 7374  ite to the objst
-00003120: 6f72 6167 6520 6265 666f 7265 2074 6865  orage before the
-00003130: 2063 7261 7368 0a20 2020 2020 2020 2023   crash.        #
-00003140: 2032 2e20 7468 6520 6f62 6a73 746f 7261   2. the objstora
-00003150: 6765 206d 6972 726f 7269 6e67 2c20 7768  ge mirroring, wh
-00003160: 6963 6820 7265 6164 7320 6672 6f6d 2074  ich reads from t
-00003170: 6865 206a 6f75 726e 616c 2c20 6d61 7920  he journal, may 
-00003180: 6174 7465 6d70 7420 746f 0a20 2020 2020  attempt to.     
-00003190: 2020 2023 2020 2020 7265 6164 2066 726f     #    read fro
-000031a0: 6d20 7468 6520 6f62 6a73 746f 7261 6765  m the objstorage
-000031b0: 2062 6566 6f72 6520 7765 2066 696e 6973   before we finis
-000031c0: 6865 6420 7772 6974 696e 6720 6974 0a20  hed writing it. 
-000031d0: 2020 2020 2020 206f 626a 7374 6f72 6167         objstorag
-000031e0: 655f 7375 6d6d 6172 7920 3d20 7365 6c66  e_summary = self
-000031f0: 2e6f 626a 7374 6f72 6167 652e 636f 6e74  .objstorage.cont
-00003200: 656e 745f 6164 6428 636f 6e74 656e 7473  ent_add(contents
-00003210: 290a 0a20 2020 2020 2020 2077 6974 6820  )..        with 
-00003220: 7365 6c66 2e64 6228 2920 6173 2064 623a  self.db() as db:
-00003230: 0a20 2020 2020 2020 2020 2020 2077 6974  .            wit
-00003240: 6820 6462 2e74 7261 6e73 6163 7469 6f6e  h db.transaction
-00003250: 2829 2061 7320 6375 723a 0a20 2020 2020  () as cur:.     
-00003260: 2020 2020 2020 2020 2020 206d 6973 7369             missi
-00003270: 6e67 203d 2073 6574 280a 2020 2020 2020  ng = set(.      
-00003280: 2020 2020 2020 2020 2020 2020 2020 7365                se
-00003290: 6c66 2e63 6f6e 7465 6e74 5f6d 6973 7369  lf.content_missi
-000032a0: 6e67 280a 2020 2020 2020 2020 2020 2020  ng(.            
-000032b0: 2020 2020 2020 2020 2020 2020 5b63 2e74              [c.t
-000032c0: 6f5f 6469 6374 2829 2066 6f72 2063 2069  o_dict() for c i
-000032d0: 6e20 636f 6e74 656e 7473 5d2c 0a20 2020  n contents],.   
-000032e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000032f0: 2020 2020 206b 6579 5f68 6173 683d 2273       key_hash="s
-00003300: 6861 315f 6769 7422 2c0a 2020 2020 2020  ha1_git",.      
+00001770: 623a 2055 6e69 6f6e 5b73 7472 2c20 4462  b: Union[str, Db
+00001780: 5d2c 0a20 2020 2020 2020 206f 626a 7374  ],.        objst
+00001790: 6f72 6167 653a 204f 7074 696f 6e61 6c5b  orage: Optional[
+000017a0: 4469 6374 5d20 3d20 4e6f 6e65 2c0a 2020  Dict] = None,.  
+000017b0: 2020 2020 2020 6d69 6e5f 706f 6f6c 5f63        min_pool_c
+000017c0: 6f6e 6e73 3a20 696e 7420 3d20 312c 0a20  onns: int = 1,. 
+000017d0: 2020 2020 2020 206d 6178 5f70 6f6f 6c5f         max_pool_
+000017e0: 636f 6e6e 733a 2069 6e74 203d 2031 302c  conns: int = 10,
+000017f0: 0a20 2020 2020 2020 206a 6f75 726e 616c  .        journal
+00001800: 5f77 7269 7465 723a 204f 7074 696f 6e61  _writer: Optiona
+00001810: 6c5b 4469 6374 5b73 7472 2c20 416e 795d  l[Dict[str, Any]
+00001820: 5d20 3d20 4e6f 6e65 2c0a 2020 2020 2020  ] = None,.      
+00001830: 2020 7175 6572 795f 6f70 7469 6f6e 733a    query_options:
+00001840: 204f 7074 696f 6e61 6c5b 4469 6374 5b73   Optional[Dict[s
+00001850: 7472 2c20 4469 6374 5b73 7472 2c20 416e  tr, Dict[str, An
+00001860: 795d 5d5d 203d 204e 6f6e 652c 0a20 2020  y]]] = None,.   
+00001870: 2029 3a0a 2020 2020 2020 2020 2222 2249   ):.        """I
+00001880: 6e73 7461 6e74 6961 7465 2061 2073 746f  nstantiate a sto
+00001890: 7261 6765 2069 6e73 7461 6e63 6520 6261  rage instance ba
+000018a0: 636b 6564 2062 7920 6120 506f 7374 6772  cked by a Postgr
+000018b0: 6553 514c 2064 6174 6162 6173 6520 616e  eSQL database an
+000018c0: 6420 616e 0a20 2020 2020 2020 206f 626a  d an.        obj
+000018d0: 7374 6f72 6167 652e 0a0a 2020 2020 2020  storage...      
+000018e0: 2020 5768 656e 2060 6064 6260 6020 6973    When ``db`` is
+000018f0: 2070 6173 7365 6420 6173 2061 2063 6f6e   passed as a con
+00001900: 6e65 6374 696f 6e20 7374 7269 6e67 2c20  nection string, 
+00001910: 7468 656e 2074 6869 7320 6d6f 6475 6c65  then this module
+00001920: 2061 7574 6f6d 6174 6963 616c 6c79 0a20   automatically. 
+00001930: 2020 2020 2020 206d 616e 6167 6573 2061         manages a
+00001940: 2063 6f6e 6e65 6374 696f 6e20 706f 6f6c   connection pool
+00001950: 2062 6574 7765 656e 2060 606d 696e 5f70   between ``min_p
+00001960: 6f6f 6c5f 636f 6e6e 7360 6020 616e 6420  ool_conns`` and 
+00001970: 6060 6d61 785f 706f 6f6c 5f63 6f6e 6e73  ``max_pool_conns
+00001980: 6060 2e0a 2020 2020 2020 2020 5768 656e  ``..        When
+00001990: 2060 6064 6260 6020 6973 2061 6e20 6578   ``db`` is an ex
+000019a0: 706c 6963 6974 2070 7379 636f 7067 3220  plicit psycopg2 
+000019b0: 636f 6e6e 6563 7469 6f6e 2c20 7468 656e  connection, then
+000019c0: 2060 606d 696e 5f70 6f6f 6c5f 636f 6e6e   ``min_pool_conn
+000019d0: 7360 6020 616e 640a 2020 2020 2020 2020  s`` and.        
+000019e0: 6060 6d61 785f 706f 6f6c 5f63 6f6e 6e73  ``max_pool_conns
+000019f0: 6060 2061 7265 2069 676e 6f72 6564 2061  `` are ignored a
+00001a00: 6e64 2074 6865 2063 6f6e 6e65 6374 696f  nd the connectio
+00001a10: 6e20 6973 2075 7365 6420 6469 7265 6374  n is used direct
+00001a20: 6c79 2e0a 0a20 2020 2020 2020 2041 7267  ly...        Arg
+00001a30: 733a 0a20 2020 2020 2020 2020 2020 2064  s:.            d
+00001a40: 623a 2065 6974 6865 7220 6120 6c69 6270  b: either a libp
+00001a50: 7120 636f 6e6e 6563 7469 6f6e 2073 7472  q connection str
+00001a60: 696e 672c 206f 7220 6120 7073 7963 6f70  ing, or a psycop
+00001a70: 6732 2063 6f6e 6e65 6374 696f 6e0a 2020  g2 connection.  
+00001a80: 2020 2020 2020 2020 2020 6f62 6a73 746f            objsto
+00001a90: 7261 6765 3a20 636f 6e66 6967 7572 6174  rage: configurat
+00001aa0: 696f 6e20 666f 7220 7468 6520 6261 636b  ion for the back
+00001ab0: 656e 6420 3a63 6c61 7373 3a60 4f62 6a53  end :class:`ObjS
+00001ac0: 746f 7261 6765 603b 2069 6620 756e 7365  torage`; if unse
+00001ad0: 742c 0a20 2020 2020 2020 2020 2020 2020  t,.             
+00001ae0: 2020 7573 6520 6120 4e6f 6f70 4f62 6a53    use a NoopObjS
+00001af0: 746f 7261 6765 0a20 2020 2020 2020 2020  torage.         
+00001b00: 2020 206d 696e 5f70 6f6f 6c5f 636f 6e6e     min_pool_conn
+00001b10: 733a 206d 696e 206e 756d 6265 7220 6f66  s: min number of
+00001b20: 2063 6f6e 6e65 6374 696f 6e73 2069 6e20   connections in 
+00001b30: 7468 6520 7073 7963 6f70 6732 2070 6f6f  the psycopg2 poo
+00001b40: 6c0a 2020 2020 2020 2020 2020 2020 6d61  l.            ma
+00001b50: 785f 706f 6f6c 5f63 6f6e 6e73 3a20 6d61  x_pool_conns: ma
+00001b60: 7820 6e75 6d62 6572 206f 6620 636f 6e6e  x number of conn
+00001b70: 6563 7469 6f6e 7320 696e 2074 6865 2070  ections in the p
+00001b80: 7379 636f 7067 3220 706f 6f6c 0a20 2020  sycopg2 pool.   
+00001b90: 2020 2020 2020 2020 206a 6f75 726e 616c           journal
+00001ba0: 5f77 7269 7465 723a 2063 6f6e 6669 6775  _writer: configu
+00001bb0: 7261 7469 6f6e 2066 6f72 2074 6865 203a  ration for the :
+00001bc0: 636c 6173 733a 604a 6f75 726e 616c 5772  class:`JournalWr
+00001bd0: 6974 6572 600a 2020 2020 2020 2020 2020  iter`.          
+00001be0: 2020 7175 6572 795f 6f70 7469 6f6e 733a    query_options:
+00001bf0: 2063 6f6e 6669 6775 7261 7469 6f6e 2066   configuration f
+00001c00: 6f72 2074 6865 2073 716c 2063 6f6e 6e65  or the sql conne
+00001c10: 6374 696f 6e73 3b20 6b65 7973 206f 6620  ctions; keys of 
+00001c20: 7468 6520 6469 6374 2061 7265 0a20 2020  the dict are.   
+00001c30: 2020 2020 2020 2020 2020 2020 7468 6520              the 
+00001c40: 6d65 7468 6f64 206e 616d 6573 2064 6563  method names dec
+00001c50: 6f72 6174 6564 2077 6974 6820 3a66 756e  orated with :fun
+00001c60: 633a 6064 625f 7472 616e 7361 6374 696f  c:`db_transactio
+00001c70: 6e60 206f 720a 2020 2020 2020 2020 2020  n` or.          
+00001c80: 2020 2020 203a 6675 6e63 3a60 6462 5f74       :func:`db_t
+00001c90: 7261 6e73 6163 7469 6f6e 5f67 656e 6572  ransaction_gener
+00001ca0: 6174 6f72 6020 2865 672e 203a 6675 6e63  ator` (eg. :func
+00001cb0: 3a60 636f 6e74 656e 745f 6669 6e64 6029  :`content_find`)
+00001cc0: 2c20 616e 6420 7661 6c75 6573 0a20 2020  , and values.   
+00001cd0: 2020 2020 2020 2020 2020 2020 6172 6520              are 
+00001ce0: 6469 6374 7320 2863 6f6e 6669 675f 6e61  dicts (config_na
+00001cf0: 6d65 2c20 636f 6e66 6967 5f76 616c 7565  me, config_value
+00001d00: 2920 7573 6564 2074 6f20 636f 6e66 6967  ) used to config
+00001d10: 7572 6520 7468 6520 7371 6c0a 2020 2020  ure the sql.    
+00001d20: 2020 2020 2020 2020 2020 2063 6f6e 6e65             conne
+00001d30: 6374 696f 6e20 666f 7220 7468 6520 6d65  ction for the me
+00001d40: 7468 6f64 5f6e 616d 652e 2046 6f72 2065  thod_name. For e
+00001d50: 7861 6d70 6c65 2c20 7573 696e 673a 3a0a  xample, using::.
+00001d60: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00001d70: 2020 207b 2263 6f6e 7465 6e74 5f67 6574     {"content_get
+00001d80: 223a 207b 2273 7461 7465 6d65 6e74 5f74  ": {"statement_t
+00001d90: 696d 656f 7574 223a 2035 3030 307d 7d0a  imeout": 5000}}.
+00001da0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00001db0: 7769 6c6c 206f 7665 7272 6964 6520 7468  will override th
+00001dc0: 6520 6465 6661 756c 7420 7374 6174 656d  e default statem
+00001dd0: 656e 7420 7469 6d65 6f75 7420 666f 7220  ent timeout for 
+00001de0: 7468 6520 3a66 756e 633a 6063 6f6e 7465  the :func:`conte
+00001df0: 6e74 5f67 6574 600a 2020 2020 2020 2020  nt_get`.        
+00001e00: 2020 2020 2020 2065 6e64 706f 696e 7420         endpoint 
+00001e10: 6672 6f6d 2035 3030 6d73 2074 6f20 3530  from 500ms to 50
+00001e20: 3030 6d73 2e0a 0a20 2020 2020 2020 2020  00ms...         
+00001e30: 2020 2020 2020 5365 6520 3a6d 6f64 3a60        See :mod:`
+00001e40: 7377 682e 636f 7265 2e64 622e 636f 6d6d  swh.core.db.comm
+00001e50: 6f6e 6020 666f 7220 6d6f 7265 2064 6574  on` for more det
+00001e60: 6169 6c73 2e0a 0a20 2020 2020 2020 2022  ails...        "
+00001e70: 2222 0a0a 2020 2020 2020 2020 7365 6c66  ""..        self
+00001e80: 2e5f 6462 3a20 4f70 7469 6f6e 616c 5b44  ._db: Optional[D
+00001e90: 625d 0a0a 2020 2020 2020 2020 7472 793a  b]..        try:
+00001ea0: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
+00001eb0: 6973 696e 7374 616e 6365 2864 622c 2070  isinstance(db, p
+00001ec0: 7379 636f 7067 322e 6578 7465 6e73 696f  sycopg2.extensio
+00001ed0: 6e73 2e63 6f6e 6e65 6374 696f 6e29 3a0a  ns.connection):.
+00001ee0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001ef0: 7365 6c66 2e5f 706f 6f6c 203d 204e 6f6e  self._pool = Non
+00001f00: 650a 2020 2020 2020 2020 2020 2020 2020  e.              
+00001f10: 2020 7365 6c66 2e5f 6462 203d 2044 6228    self._db = Db(
+00001f20: 6462 290a 0a20 2020 2020 2020 2020 2020  db)..           
+00001f30: 2020 2020 2023 2053 6565 2063 6f6d 6d65       # See comme
+00001f40: 6e74 2062 656c 6f77 0a20 2020 2020 2020  nt below.       
+00001f50: 2020 2020 2020 2020 2073 656c 662e 5f64           self._d
+00001f60: 622e 6375 7273 6f72 2829 2e65 7865 6375  b.cursor().execu
+00001f70: 7465 2822 5345 5420 5449 4d45 205a 4f4e  te("SET TIME ZON
+00001f80: 4520 2755 5443 2722 290a 2020 2020 2020  E 'UTC'").      
+00001f90: 2020 2020 2020 656c 7365 3a0a 2020 2020        else:.    
+00001fa0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+00001fb0: 2e5f 706f 6f6c 203d 2070 7379 636f 7067  ._pool = psycopg
+00001fc0: 322e 706f 6f6c 2e54 6872 6561 6465 6443  2.pool.ThreadedC
+00001fd0: 6f6e 6e65 6374 696f 6e50 6f6f 6c28 0a20  onnectionPool(. 
+00001fe0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001ff0: 2020 206d 696e 5f70 6f6f 6c5f 636f 6e6e     min_pool_conn
+00002000: 732c 206d 6178 5f70 6f6f 6c5f 636f 6e6e  s, max_pool_conn
+00002010: 732c 2064 620a 2020 2020 2020 2020 2020  s, db.          
+00002020: 2020 2020 2020 290a 2020 2020 2020 2020        ).        
+00002030: 2020 2020 2020 2020 7365 6c66 2e5f 6462          self._db
+00002040: 203d 204e 6f6e 650a 2020 2020 2020 2020   = None.        
+00002050: 6578 6365 7074 2070 7379 636f 7067 322e  except psycopg2.
+00002060: 4f70 6572 6174 696f 6e61 6c45 7272 6f72  OperationalError
+00002070: 2061 7320 653a 0a20 2020 2020 2020 2020   as e:.         
+00002080: 2020 2072 6169 7365 2053 746f 7261 6765     raise Storage
+00002090: 4442 4572 726f 7228 6529 0a20 2020 2020  DBError(e).     
+000020a0: 2020 2073 656c 662e 6a6f 7572 6e61 6c5f     self.journal_
+000020b0: 7772 6974 6572 203d 204a 6f75 726e 616c  writer = Journal
+000020c0: 5772 6974 6572 286a 6f75 726e 616c 5f77  Writer(journal_w
+000020d0: 7269 7465 7229 0a20 2020 2020 2020 2073  riter).        s
+000020e0: 656c 662e 6f62 6a73 746f 7261 6765 203d  elf.objstorage =
+000020f0: 204f 626a 5374 6f72 6167 6528 7365 6c66   ObjStorage(self
+00002100: 2c20 6f62 6a73 746f 7261 6765 290a 2020  , objstorage).  
+00002110: 2020 2020 2020 7365 6c66 2e71 7565 7279        self.query
+00002120: 5f6f 7074 696f 6e73 203d 2071 7565 7279  _options = query
+00002130: 5f6f 7074 696f 6e73 0a20 2020 2020 2020  _options.       
+00002140: 2073 656c 662e 5f66 6c61 766f 723a 204f   self._flavor: O
+00002150: 7074 696f 6e61 6c5b 7374 725d 203d 204e  ptional[str] = N
+00002160: 6f6e 650a 0a20 2020 2023 2323 2323 2323  one..    #######
+00002170: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00002180: 2323 230a 2020 2020 2320 5574 696c 6974  ###.    # Utilit
+00002190: 6965 730a 2020 2020 2323 2323 2323 2323  ies.    ########
+000021a0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+000021b0: 2323 0a0a 2020 2020 6465 6620 6765 745f  ##..    def get_
+000021c0: 6462 2873 656c 6629 3a0a 2020 2020 2020  db(self):.      
+000021d0: 2020 6966 2073 656c 662e 5f64 623a 0a20    if self._db:. 
+000021e0: 2020 2020 2020 2020 2020 2072 6574 7572             retur
+000021f0: 6e20 7365 6c66 2e5f 6462 0a20 2020 2020  n self._db.     
+00002200: 2020 2065 6c73 653a 0a20 2020 2020 2020     else:.       
+00002210: 2020 2020 2064 6220 3d20 4462 2e66 726f       db = Db.fro
+00002220: 6d5f 706f 6f6c 2873 656c 662e 5f70 6f6f  m_pool(self._poo
+00002230: 6c29 0a0a 2020 2020 2020 2020 2020 2020  l)..            
+00002240: 2320 576f 726b 6172 6f75 6e64 2066 6f72  # Workaround for
+00002250: 2070 7379 636f 7067 3220 3c20 322e 392e   psycopg2 < 2.9.
+00002260: 3020 6e6f 7420 6861 6e64 6c69 6e67 2066  0 not handling f
+00002270: 7261 6374 696f 6e61 6c20 7469 6d65 7a6f  ractional timezo
+00002280: 6e65 732c 0a20 2020 2020 2020 2020 2020  nes,.           
+00002290: 2023 2077 6869 6368 206d 6179 2068 6170   # which may hap
+000022a0: 7065 6e20 6f6e 206f 6c64 2072 6576 6973  pen on old revis
+000022b0: 696f 6e2f 7265 6c65 6173 6520 6461 7465  ion/release date
+000022c0: 7320 6f6e 2073 7973 7465 6d73 2063 6f6e  s on systems con
+000022d0: 6669 6775 7265 640a 2020 2020 2020 2020  figured.        
+000022e0: 2020 2020 2320 7769 7468 206e 6f6e 2d55      # with non-U
+000022f0: 5443 2074 696d 657a 6f6e 6573 2e0a 2020  TC timezones..  
+00002300: 2020 2020 2020 2020 2020 2320 6874 7470            # http
+00002310: 733a 2f2f 7777 772e 7073 7963 6f70 672e  s://www.psycopg.
+00002320: 6f72 672f 646f 6373 2f75 7361 6765 2e68  org/docs/usage.h
+00002330: 746d 6c23 7469 6d65 2d7a 6f6e 6573 2d68  tml#time-zones-h
+00002340: 616e 646c 696e 670a 2020 2020 2020 2020  andling.        
+00002350: 2020 2020 6462 2e63 7572 736f 7228 292e      db.cursor().
+00002360: 6578 6563 7574 6528 2253 4554 2054 494d  execute("SET TIM
+00002370: 4520 5a4f 4e45 2027 5554 4327 2229 0a0a  E ZONE 'UTC'")..
+00002380: 2020 2020 2020 2020 2020 2020 7265 7475              retu
+00002390: 726e 2064 620a 0a20 2020 2064 6566 2070  rn db..    def p
+000023a0: 7574 5f64 6228 7365 6c66 2c20 6462 293a  ut_db(self, db):
+000023b0: 0a20 2020 2020 2020 2069 6620 6462 2069  .        if db i
+000023c0: 7320 6e6f 7420 7365 6c66 2e5f 6462 3a0a  s not self._db:.
+000023d0: 2020 2020 2020 2020 2020 2020 6462 2e70              db.p
+000023e0: 7574 5f63 6f6e 6e28 290a 0a20 2020 2040  ut_conn()..    @
+000023f0: 636f 6e74 6578 746d 616e 6167 6572 0a20  contextmanager. 
+00002400: 2020 2064 6566 2064 6228 7365 6c66 293a     def db(self):
+00002410: 0a20 2020 2020 2020 2064 6220 3d20 4e6f  .        db = No
+00002420: 6e65 0a20 2020 2020 2020 2074 7279 3a0a  ne.        try:.
+00002430: 2020 2020 2020 2020 2020 2020 6462 203d              db =
+00002440: 2073 656c 662e 6765 745f 6462 2829 0a20   self.get_db(). 
+00002450: 2020 2020 2020 2020 2020 2079 6965 6c64             yield
+00002460: 2064 620a 2020 2020 2020 2020 6669 6e61   db.        fina
+00002470: 6c6c 793a 0a20 2020 2020 2020 2020 2020  lly:.           
+00002480: 2069 6620 6462 3a0a 2020 2020 2020 2020   if db:.        
+00002490: 2020 2020 2020 2020 7365 6c66 2e70 7574          self.put
+000024a0: 5f64 6228 6462 290a 0a20 2020 2040 6462  _db(db)..    @db
+000024b0: 5f74 7261 6e73 6163 7469 6f6e 2829 0a20  _transaction(). 
+000024c0: 2020 2064 6566 2067 6574 5f66 6c61 766f     def get_flavo
+000024d0: 7228 7365 6c66 2c20 2a2c 2064 623a 2044  r(self, *, db: D
+000024e0: 622c 2063 7572 3d4e 6f6e 6529 202d 3e20  b, cur=None) -> 
+000024f0: 7374 723a 0a20 2020 2020 2020 2066 6c61  str:.        fla
+00002500: 766f 7220 3d20 7377 685f 6462 5f66 6c61  vor = swh_db_fla
+00002510: 766f 7228 6462 2e63 6f6e 6e2e 6473 6e29  vor(db.conn.dsn)
+00002520: 0a20 2020 2020 2020 2061 7373 6572 7420  .        assert 
+00002530: 666c 6176 6f72 2069 7320 6e6f 7420 4e6f  flavor is not No
+00002540: 6e65 0a20 2020 2020 2020 2072 6574 7572  ne.        retur
+00002550: 6e20 666c 6176 6f72 0a0a 2020 2020 4070  n flavor..    @p
+00002560: 726f 7065 7274 790a 2020 2020 6465 6620  roperty.    def 
+00002570: 666c 6176 6f72 2873 656c 6629 202d 3e20  flavor(self) -> 
+00002580: 7374 723a 0a20 2020 2020 2020 2069 6620  str:.        if 
+00002590: 7365 6c66 2e5f 666c 6176 6f72 2069 7320  self._flavor is 
+000025a0: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
+000025b0: 2020 7365 6c66 2e5f 666c 6176 6f72 203d    self._flavor =
+000025c0: 2073 656c 662e 6765 745f 666c 6176 6f72   self.get_flavor
+000025d0: 2829 0a20 2020 2020 2020 2061 7373 6572  ().        asser
+000025e0: 7420 7365 6c66 2e5f 666c 6176 6f72 2069  t self._flavor i
+000025f0: 7320 6e6f 7420 4e6f 6e65 0a20 2020 2020  s not None.     
+00002600: 2020 2072 6574 7572 6e20 7365 6c66 2e5f     return self._
+00002610: 666c 6176 6f72 0a0a 2020 2020 4064 625f  flavor..    @db_
+00002620: 7472 616e 7361 6374 696f 6e28 290a 2020  transaction().  
+00002630: 2020 6465 6620 6368 6563 6b5f 636f 6e66    def check_conf
+00002640: 6967 2873 656c 662c 202a 2c20 6368 6563  ig(self, *, chec
+00002650: 6b5f 7772 6974 653a 2062 6f6f 6c2c 2064  k_write: bool, d
+00002660: 623a 2044 622c 2063 7572 3d4e 6f6e 6529  b: Db, cur=None)
+00002670: 202d 3e20 626f 6f6c 3a0a 2020 2020 2020   -> bool:.      
+00002680: 2020 6966 206e 6f74 2073 656c 662e 6f62    if not self.ob
+00002690: 6a73 746f 7261 6765 2e63 6865 636b 5f63  jstorage.check_c
+000026a0: 6f6e 6669 6728 6368 6563 6b5f 7772 6974  onfig(check_writ
+000026b0: 653d 6368 6563 6b5f 7772 6974 6529 3a0a  e=check_write):.
+000026c0: 2020 2020 2020 2020 2020 2020 7265 7475              retu
+000026d0: 726e 2046 616c 7365 0a0a 2020 2020 2020  rn False..      
+000026e0: 2020 6462 7665 7273 696f 6e20 3d20 7377    dbversion = sw
+000026f0: 685f 6462 5f76 6572 7369 6f6e 2864 622e  h_db_version(db.
+00002700: 636f 6e6e 2e64 736e 290a 2020 2020 2020  conn.dsn).      
+00002710: 2020 6966 2064 6276 6572 7369 6f6e 2021    if dbversion !
+00002720: 3d20 7365 6c66 2e63 7572 7265 6e74 5f76  = self.current_v
+00002730: 6572 7369 6f6e 3a0a 2020 2020 2020 2020  ersion:.        
+00002740: 2020 2020 6c6f 6767 6572 2e77 6172 6e69      logger.warni
+00002750: 6e67 280a 2020 2020 2020 2020 2020 2020  ng(.            
+00002760: 2020 2020 2264 6174 6162 6173 6520 6462      "database db
+00002770: 7665 7273 696f 6e20 2825 7329 2021 3d20  version (%s) != 
+00002780: 2573 2063 7572 7265 6e74 5f76 6572 7369  %s current_versi
+00002790: 6f6e 2028 2573 2922 2c0a 2020 2020 2020  on (%s)",.      
+000027a0: 2020 2020 2020 2020 2020 6462 7665 7273            dbvers
+000027b0: 696f 6e2c 0a20 2020 2020 2020 2020 2020  ion,.           
+000027c0: 2020 2020 205f 5f6e 616d 655f 5f2c 0a20       __name__,. 
+000027d0: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+000027e0: 656c 662e 6375 7272 656e 745f 7665 7273  elf.current_vers
+000027f0: 696f 6e2c 0a20 2020 2020 2020 2020 2020  ion,.           
+00002800: 2029 0a20 2020 2020 2020 2020 2020 2072   ).            r
+00002810: 6574 7572 6e20 4661 6c73 650a 0a20 2020  eturn False..   
+00002820: 2020 2020 2023 2043 6865 636b 2070 6572       # Check per
+00002830: 6d69 7373 696f 6e73 206f 6e20 6f6e 6520  missions on one 
+00002840: 6f66 2074 6865 2074 6162 6c65 730a 2020  of the tables.  
+00002850: 2020 2020 2020 6368 6563 6b20 3d20 2249        check = "I
+00002860: 4e53 4552 5422 2069 6620 6368 6563 6b5f  NSERT" if check_
+00002870: 7772 6974 6520 656c 7365 2022 5345 4c45  write else "SELE
+00002880: 4354 220a 0a20 2020 2020 2020 2063 7572  CT"..        cur
+00002890: 2e65 7865 6375 7465 2822 7365 6c65 6374  .execute("select
+000028a0: 2068 6173 5f74 6162 6c65 5f70 7269 7669   has_table_privi
+000028b0: 6c65 6765 2863 7572 7265 6e74 5f75 7365  lege(current_use
+000028c0: 722c 2027 636f 6e74 656e 7427 2c20 2573  r, 'content', %s
+000028d0: 2922 2c20 2863 6865 636b 2c29 290a 2020  )", (check,)).  
+000028e0: 2020 2020 2020 7265 7475 726e 2063 7572        return cur
+000028f0: 2e66 6574 6368 6f6e 6528 295b 305d 0a0a  .fetchone()[0]..
+00002900: 2020 2020 2323 2323 2323 2323 2323 2323      ############
+00002910: 2323 2323 2323 2323 2323 2323 2323 0a20  ##############. 
+00002920: 2020 2023 2043 6f6e 7465 6e74 0a20 2020     # Content.   
+00002930: 2023 2323 2323 2323 2323 2323 2323 2323   ###############
+00002940: 2323 2323 2323 2323 2323 230a 0a20 2020  ###########..   
+00002950: 2064 6566 205f 636f 6e74 656e 745f 756e   def _content_un
+00002960: 6971 7565 5f6b 6579 2873 656c 662c 2068  ique_key(self, h
+00002970: 6173 682c 2064 6229 3a0a 2020 2020 2020  ash, db):.      
+00002980: 2020 2222 2247 6976 656e 2061 2068 6173    """Given a has
+00002990: 6820 2874 7570 6c65 206f 7220 6469 6374  h (tuple or dict
+000029a0: 292c 2072 6574 7572 6e20 6120 756e 6971  ), return a uniq
+000029b0: 7565 206b 6579 2066 726f 6d20 7468 650a  ue key from the.
+000029c0: 2020 2020 2020 2020 6167 6772 6567 6174          aggregat
+000029d0: 696f 6e20 6f66 206b 6579 732e 0a0a 2020  ion of keys...  
+000029e0: 2020 2020 2020 2222 220a 2020 2020 2020        """.      
+000029f0: 2020 6b65 7973 203d 2064 622e 636f 6e74    keys = db.cont
+00002a00: 656e 745f 6861 7368 5f6b 6579 730a 2020  ent_hash_keys.  
+00002a10: 2020 2020 2020 6966 2069 7369 6e73 7461        if isinsta
+00002a20: 6e63 6528 6861 7368 2c20 7475 706c 6529  nce(hash, tuple)
+00002a30: 3a0a 2020 2020 2020 2020 2020 2020 7265  :.            re
+00002a40: 7475 726e 2068 6173 680a 2020 2020 2020  turn hash.      
+00002a50: 2020 7265 7475 726e 2074 7570 6c65 285b    return tuple([
+00002a60: 6861 7368 5b6b 5d20 666f 7220 6b20 696e  hash[k] for k in
+00002a70: 206b 6579 735d 290a 0a20 2020 2064 6566   keys])..    def
+00002a80: 205f 636f 6e74 656e 745f 6164 645f 6d65   _content_add_me
+00002a90: 7461 6461 7461 2873 656c 662c 2064 622c  tadata(self, db,
+00002aa0: 2063 7572 2c20 636f 6e74 656e 7429 3a0a   cur, content):.
+00002ab0: 2020 2020 2020 2020 2222 2241 6464 2063          """Add c
+00002ac0: 6f6e 7465 6e74 2074 6f20 7468 6520 706f  ontent to the po
+00002ad0: 7374 6772 6573 716c 2064 6174 6162 6173  stgresql databas
+00002ae0: 6520 6275 7420 6e6f 7420 7468 6520 6f62  e but not the ob
+00002af0: 6a65 6374 2073 746f 7261 6765 2e22 2222  ject storage."""
+00002b00: 0a20 2020 2020 2020 2023 2063 7265 6174  .        # creat
+00002b10: 6520 7465 6d70 6f72 6172 7920 7461 626c  e temporary tabl
+00002b20: 6520 666f 7220 6d65 7461 6461 7461 2069  e for metadata i
+00002b30: 6e6a 6563 7469 6f6e 0a20 2020 2020 2020  njection.       
+00002b40: 2064 622e 6d6b 7465 6d70 2822 636f 6e74   db.mktemp("cont
+00002b50: 656e 7422 2c20 6375 7229 0a0a 2020 2020  ent", cur)..    
+00002b60: 2020 2020 6462 2e63 6f70 795f 746f 280a      db.copy_to(.
+00002b70: 2020 2020 2020 2020 2020 2020 2863 2e74              (c.t
+00002b80: 6f5f 6469 6374 2829 2066 6f72 2063 2069  o_dict() for c i
+00002b90: 6e20 636f 6e74 656e 7429 2c20 2274 6d70  n content), "tmp
+00002ba0: 5f63 6f6e 7465 6e74 222c 2064 622e 636f  _content", db.co
+00002bb0: 6e74 656e 745f 6164 645f 6b65 7973 2c20  ntent_add_keys, 
+00002bc0: 6375 720a 2020 2020 2020 2020 290a 0a20  cur.        ).. 
+00002bd0: 2020 2020 2020 2023 206d 6f76 6520 6d65         # move me
+00002be0: 7461 6461 7461 2069 6e20 706c 6163 650a  tadata in place.
+00002bf0: 2020 2020 2020 2020 7472 793a 0a20 2020          try:.   
+00002c00: 2020 2020 2020 2020 2064 622e 636f 6e74           db.cont
+00002c10: 656e 745f 6164 645f 6672 6f6d 5f74 656d  ent_add_from_tem
+00002c20: 7028 6375 7229 0a20 2020 2020 2020 2065  p(cur).        e
+00002c30: 7863 6570 7420 7073 7963 6f70 6732 2e49  xcept psycopg2.I
+00002c40: 6e74 6567 7269 7479 4572 726f 7220 6173  ntegrityError as
+00002c50: 2065 3a0a 2020 2020 2020 2020 2020 2020   e:.            
+00002c60: 6966 2065 2e64 6961 672e 7371 6c73 7461  if e.diag.sqlsta
+00002c70: 7465 203d 3d20 2232 3335 3035 2220 616e  te == "23505" an
+00002c80: 6420 652e 6469 6167 2e74 6162 6c65 5f6e  d e.diag.table_n
+00002c90: 616d 6520 3d3d 2022 636f 6e74 656e 7422  ame == "content"
+00002ca0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+00002cb0: 2020 6d65 7373 6167 655f 6465 7461 696c    message_detail
+00002cc0: 203d 2065 2e64 6961 672e 6d65 7373 6167   = e.diag.messag
+00002cd0: 655f 6465 7461 696c 0a20 2020 2020 2020  e_detail.       
+00002ce0: 2020 2020 2020 2020 2069 6620 6d65 7373           if mess
+00002cf0: 6167 655f 6465 7461 696c 3a0a 2020 2020  age_detail:.    
+00002d00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002d10: 6861 7368 5f6e 616d 652c 2068 6173 685f  hash_name, hash_
+00002d20: 6964 203d 2065 7874 7261 6374 5f63 6f6c  id = extract_col
+00002d30: 6c69 7369 6f6e 5f68 6173 6828 6d65 7373  lision_hash(mess
+00002d40: 6167 655f 6465 7461 696c 290a 2020 2020  age_detail).    
+00002d50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002d60: 636f 6c6c 6973 696f 6e5f 636f 6e74 656e  collision_conten
+00002d70: 7473 5f68 6173 6865 7320 3d20 5b0a 2020  ts_hashes = [.  
+00002d80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002d90: 2020 2020 2020 632e 6861 7368 6573 2829        c.hashes()
+00002da0: 2066 6f72 2063 2069 6e20 636f 6e74 656e   for c in conten
+00002db0: 7420 6966 2063 2e67 6574 5f68 6173 6828  t if c.get_hash(
+00002dc0: 6861 7368 5f6e 616d 6529 203d 3d20 6861  hash_name) == ha
+00002dd0: 7368 5f69 640a 2020 2020 2020 2020 2020  sh_id.          
+00002de0: 2020 2020 2020 2020 2020 5d0a 2020 2020            ].    
+00002df0: 2020 2020 2020 2020 2020 2020 656c 7365              else
+00002e00: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+00002e10: 2020 2020 2020 636f 6e73 7472 6169 6e74        constraint
+00002e20: 5f74 6f5f 6861 7368 5f6e 616d 6520 3d20  _to_hash_name = 
+00002e30: 7b0a 2020 2020 2020 2020 2020 2020 2020  {.              
+00002e40: 2020 2020 2020 2020 2020 2263 6f6e 7465            "conte
+00002e50: 6e74 5f70 6b65 7922 3a20 2273 6861 3122  nt_pkey": "sha1"
+00002e60: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+00002e70: 2020 2020 2020 2020 2020 2263 6f6e 7465            "conte
+00002e80: 6e74 5f73 6861 315f 6769 745f 6964 7822  nt_sha1_git_idx"
+00002e90: 3a20 2273 6861 315f 6769 7422 2c0a 2020  : "sha1_git",.  
+00002ea0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002eb0: 2020 2020 2020 2263 6f6e 7465 6e74 5f73        "content_s
+00002ec0: 6861 3235 365f 6964 7822 3a20 2273 6861  ha256_idx": "sha
+00002ed0: 3235 3622 2c0a 2020 2020 2020 2020 2020  256",.          
+00002ee0: 2020 2020 2020 2020 2020 7d0a 2020 2020            }.    
+00002ef0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002f00: 6861 7368 5f6e 616d 6520 3d20 636f 6e73  hash_name = cons
+00002f10: 7472 6169 6e74 5f74 6f5f 6861 7368 5f6e  traint_to_hash_n
+00002f20: 616d 652e 6765 7428 652e 6469 6167 2e63  ame.get(e.diag.c
+00002f30: 6f6e 7374 7261 696e 745f 6e61 6d65 290a  onstraint_name).
+00002f40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002f50: 2020 2020 6861 7368 5f69 6420 3d20 4e6f      hash_id = No
+00002f60: 6e65 0a20 2020 2020 2020 2020 2020 2020  ne.             
+00002f70: 2020 2020 2020 2063 6f6c 6c69 7369 6f6e         collision
+00002f80: 5f63 6f6e 7465 6e74 735f 6861 7368 6573  _contents_hashes
+00002f90: 203d 204e 6f6e 650a 0a20 2020 2020 2020   = None..       
+00002fa0: 2020 2020 2020 2020 2072 6169 7365 2048           raise H
+00002fb0: 6173 6843 6f6c 6c69 7369 6f6e 280a 2020  ashCollision(.  
+00002fc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002fd0: 2020 6861 7368 5f6e 616d 652c 2068 6173    hash_name, has
+00002fe0: 685f 6964 2c20 636f 6c6c 6973 696f 6e5f  h_id, collision_
+00002ff0: 636f 6e74 656e 7473 5f68 6173 6865 730a  contents_hashes.
+00003000: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003010: 2920 6672 6f6d 204e 6f6e 650a 2020 2020  ) from None.    
+00003020: 2020 2020 2020 2020 656c 7365 3a0a 2020          else:.  
+00003030: 2020 2020 2020 2020 2020 2020 2020 7261                ra
+00003040: 6973 650a 0a20 2020 2064 6566 2063 6f6e  ise..    def con
+00003050: 7465 6e74 5f61 6464 2873 656c 662c 2063  tent_add(self, c
+00003060: 6f6e 7465 6e74 3a20 4c69 7374 5b43 6f6e  ontent: List[Con
+00003070: 7465 6e74 5d29 202d 3e20 4469 6374 5b73  tent]) -> Dict[s
+00003080: 7472 2c20 696e 745d 3a0a 2020 2020 2020  tr, int]:.      
+00003090: 2020 6374 696d 6520 3d20 6e6f 7728 290a    ctime = now().
+000030a0: 0a20 2020 2020 2020 2063 6f6e 7465 6e74  .        content
+000030b0: 7320 3d20 5b61 7474 722e 6576 6f6c 7665  s = [attr.evolve
+000030c0: 2863 2c20 6374 696d 653d 6374 696d 6529  (c, ctime=ctime)
+000030d0: 2066 6f72 2063 2069 6e20 636f 6e74 656e   for c in conten
+000030e0: 745d 0a0a 2020 2020 2020 2020 2320 4d75  t]..        # Mu
+000030f0: 7374 2061 6464 2074 6f20 7468 6520 6f62  st add to the ob
+00003100: 6a73 746f 7261 6765 2062 6566 6f72 6520  jstorage before 
+00003110: 7468 6520 4442 2061 6e64 206a 6f75 726e  the DB and journ
+00003120: 616c 2e20 4f74 6865 7277 6973 653a 0a20  al. Otherwise:. 
+00003130: 2020 2020 2020 2023 2031 2e20 696e 2063         # 1. in c
+00003140: 6173 6520 6f66 2061 2063 7261 7368 2074  ase of a crash t
+00003150: 6865 2044 4220 6d61 7920 2262 656c 6965  he DB may "belie
+00003160: 7665 2220 7765 2068 6176 6520 7468 6520  ve" we have the 
+00003170: 636f 6e74 656e 742c 2062 7574 0a20 2020  content, but.   
+00003180: 2020 2020 2023 2020 2020 7765 2064 6964       #    we did
+00003190: 6e27 7420 6861 7665 2074 696d 6520 746f  n't have time to
+000031a0: 2077 7269 7465 2074 6f20 7468 6520 6f62   write to the ob
+000031b0: 6a73 746f 7261 6765 2062 6566 6f72 6520  jstorage before 
+000031c0: 7468 6520 6372 6173 680a 2020 2020 2020  the crash.      
+000031d0: 2020 2320 322e 2074 6865 206f 626a 7374    # 2. the objst
+000031e0: 6f72 6167 6520 6d69 7272 6f72 696e 672c  orage mirroring,
+000031f0: 2077 6869 6368 2072 6561 6473 2066 726f   which reads fro
+00003200: 6d20 7468 6520 6a6f 7572 6e61 6c2c 206d  m the journal, m
+00003210: 6179 2061 7474 656d 7074 2074 6f0a 2020  ay attempt to.  
+00003220: 2020 2020 2020 2320 2020 2072 6561 6420        #    read 
+00003230: 6672 6f6d 2074 6865 206f 626a 7374 6f72  from the objstor
+00003240: 6167 6520 6265 666f 7265 2077 6520 6669  age before we fi
+00003250: 6e69 7368 6564 2077 7269 7469 6e67 2069  nished writing i
+00003260: 740a 2020 2020 2020 2020 6f62 6a73 746f  t.        objsto
+00003270: 7261 6765 5f73 756d 6d61 7279 203d 2073  rage_summary = s
+00003280: 656c 662e 6f62 6a73 746f 7261 6765 2e63  elf.objstorage.c
+00003290: 6f6e 7465 6e74 5f61 6464 2863 6f6e 7465  ontent_add(conte
+000032a0: 6e74 7329 0a0a 2020 2020 2020 2020 7769  nts)..        wi
+000032b0: 7468 2073 656c 662e 6462 2829 2061 7320  th self.db() as 
+000032c0: 6462 3a0a 2020 2020 2020 2020 2020 2020  db:.            
+000032d0: 7769 7468 2064 622e 7472 616e 7361 6374  with db.transact
+000032e0: 696f 6e28 2920 6173 2063 7572 3a0a 2020  ion() as cur:.  
+000032f0: 2020 2020 2020 2020 2020 2020 2020 6d69                mi
+00003300: 7373 696e 6720 3d20 7365 7428 0a20 2020  ssing = set(.   
 00003310: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003320: 2020 6462 3d64 622c 0a20 2020 2020 2020    db=db,.       
-00003330: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003340: 2063 7572 3d63 7572 2c0a 2020 2020 2020   cur=cur,.      
-00003350: 2020 2020 2020 2020 2020 2020 2020 290a                ).
-00003360: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003370: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
-00003380: 2020 636f 6e74 656e 7473 203d 205b 6320    contents = [c 
-00003390: 666f 7220 6320 696e 2063 6f6e 7465 6e74  for c in content
-000033a0: 7320 6966 2063 2e73 6861 315f 6769 7420  s if c.sha1_git 
-000033b0: 696e 206d 6973 7369 6e67 5d0a 0a20 2020  in missing]..   
-000033c0: 2020 2020 2020 2020 2020 2020 2073 656c               sel
-000033d0: 662e 6a6f 7572 6e61 6c5f 7772 6974 6572  f.journal_writer
-000033e0: 2e63 6f6e 7465 6e74 5f61 6464 2863 6f6e  .content_add(con
-000033f0: 7465 6e74 7329 0a20 2020 2020 2020 2020  tents).         
-00003400: 2020 2020 2020 2073 656c 662e 5f63 6f6e         self._con
-00003410: 7465 6e74 5f61 6464 5f6d 6574 6164 6174  tent_add_metadat
-00003420: 6128 6462 2c20 6375 722c 2063 6f6e 7465  a(db, cur, conte
-00003430: 6e74 7329 0a0a 2020 2020 2020 2020 7265  nts)..        re
-00003440: 7475 726e 207b 0a20 2020 2020 2020 2020  turn {.         
-00003450: 2020 2022 636f 6e74 656e 743a 6164 6422     "content:add"
-00003460: 3a20 6c65 6e28 636f 6e74 656e 7473 292c  : len(contents),
-00003470: 0a20 2020 2020 2020 2020 2020 2022 636f  .            "co
-00003480: 6e74 656e 743a 6164 643a 6279 7465 7322  ntent:add:bytes"
-00003490: 3a20 6f62 6a73 746f 7261 6765 5f73 756d  : objstorage_sum
-000034a0: 6d61 7279 5b22 636f 6e74 656e 743a 6164  mary["content:ad
-000034b0: 643a 6279 7465 7322 5d2c 0a20 2020 2020  d:bytes"],.     
-000034c0: 2020 207d 0a0a 2020 2020 4064 625f 7472     }..    @db_tr
-000034d0: 616e 7361 6374 696f 6e28 290a 2020 2020  ansaction().    
-000034e0: 6465 6620 636f 6e74 656e 745f 7570 6461  def content_upda
-000034f0: 7465 280a 2020 2020 2020 2020 7365 6c66  te(.        self
-00003500: 2c20 636f 6e74 656e 7473 3a20 4c69 7374  , contents: List
-00003510: 5b44 6963 745b 7374 722c 2041 6e79 5d5d  [Dict[str, Any]]
-00003520: 2c20 6b65 7973 3a20 4c69 7374 5b73 7472  , keys: List[str
-00003530: 5d20 3d20 5b5d 2c20 2a2c 2064 623a 2044  ] = [], *, db: D
-00003540: 622c 2063 7572 3d4e 6f6e 650a 2020 2020  b, cur=None.    
-00003550: 2920 2d3e 204e 6f6e 653a 0a20 2020 2020  ) -> None:.     
-00003560: 2020 2023 2054 4f44 4f3a 2041 6464 2061     # TODO: Add a
-00003570: 2063 6865 636b 206f 6e20 696e 7075 7420   check on input 
-00003580: 6b65 7973 2e20 486f 7720 746f 2070 726f  keys. How to pro
-00003590: 7065 726c 7920 696d 706c 656d 656e 740a  perly implement.
-000035a0: 2020 2020 2020 2020 2320 7468 6973 3f20          # this? 
-000035b0: 5765 2064 6f6e 2774 206b 6e6f 7720 7965  We don't know ye
-000035c0: 7420 7468 6520 6e65 7720 636f 6c75 6d6e  t the new column
-000035d0: 732e 0a20 2020 2020 2020 2073 656c 662e  s..        self.
-000035e0: 6a6f 7572 6e61 6c5f 7772 6974 6572 2e63  journal_writer.c
-000035f0: 6f6e 7465 6e74 5f75 7064 6174 6528 636f  ontent_update(co
-00003600: 6e74 656e 7473 290a 0a20 2020 2020 2020  ntents)..       
-00003610: 2064 622e 6d6b 7465 6d70 2822 636f 6e74   db.mktemp("cont
-00003620: 656e 7422 2c20 6375 7229 0a20 2020 2020  ent", cur).     
-00003630: 2020 2073 656c 6563 745f 6b65 7973 203d     select_keys =
-00003640: 206c 6973 7428 7365 7428 6462 2e63 6f6e   list(set(db.con
-00003650: 7465 6e74 5f67 6574 5f6d 6574 6164 6174  tent_get_metadat
-00003660: 615f 6b65 7973 292e 756e 696f 6e28 7365  a_keys).union(se
-00003670: 7428 6b65 7973 2929 290a 2020 2020 2020  t(keys))).      
-00003680: 2020 7769 7468 2063 6f6e 7665 7274 5f76    with convert_v
-00003690: 616c 6964 6174 696f 6e5f 6578 6365 7074  alidation_except
-000036a0: 696f 6e73 2829 3a0a 2020 2020 2020 2020  ions():.        
-000036b0: 2020 2020 6462 2e63 6f70 795f 746f 2863      db.copy_to(c
-000036c0: 6f6e 7465 6e74 732c 2022 746d 705f 636f  ontents, "tmp_co
-000036d0: 6e74 656e 7422 2c20 7365 6c65 6374 5f6b  ntent", select_k
-000036e0: 6579 732c 2063 7572 290a 2020 2020 2020  eys, cur).      
-000036f0: 2020 2020 2020 6462 2e63 6f6e 7465 6e74        db.content
-00003700: 5f75 7064 6174 655f 6672 6f6d 5f74 656d  _update_from_tem
-00003710: 7028 6b65 7973 5f74 6f5f 7570 6461 7465  p(keys_to_update
-00003720: 3d6b 6579 732c 2063 7572 3d63 7572 290a  =keys, cur=cur).
-00003730: 0a20 2020 2040 6462 5f74 7261 6e73 6163  .    @db_transac
-00003740: 7469 6f6e 2829 0a20 2020 2064 6566 2063  tion().    def c
-00003750: 6f6e 7465 6e74 5f61 6464 5f6d 6574 6164  ontent_add_metad
-00003760: 6174 6128 0a20 2020 2020 2020 2073 656c  ata(.        sel
-00003770: 662c 2063 6f6e 7465 6e74 3a20 4c69 7374  f, content: List
-00003780: 5b43 6f6e 7465 6e74 5d2c 202a 2c20 6462  [Content], *, db
-00003790: 3a20 4462 2c20 6375 723d 4e6f 6e65 0a20  : Db, cur=None. 
-000037a0: 2020 2029 202d 3e20 4469 6374 5b73 7472     ) -> Dict[str
-000037b0: 2c20 696e 745d 3a0a 2020 2020 2020 2020  , int]:.        
-000037c0: 6d69 7373 696e 6720 3d20 7365 7428 0a20  missing = set(. 
-000037d0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-000037e0: 636f 6e74 656e 745f 6d69 7373 696e 6728  content_missing(
-000037f0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00003800: 205b 632e 746f 5f64 6963 7428 2920 666f   [c.to_dict() fo
-00003810: 7220 6320 696e 2063 6f6e 7465 6e74 5d2c  r c in content],
-00003820: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00003830: 206b 6579 5f68 6173 683d 2273 6861 315f   key_hash="sha1_
-00003840: 6769 7422 2c0a 2020 2020 2020 2020 2020  git",.          
-00003850: 2020 2020 2020 6462 3d64 622c 0a20 2020        db=db,.   
-00003860: 2020 2020 2020 2020 2020 2020 2063 7572               cur
-00003870: 3d63 7572 2c0a 2020 2020 2020 2020 2020  =cur,.          
-00003880: 2020 290a 2020 2020 2020 2020 290a 2020    ).        ).  
-00003890: 2020 2020 2020 636f 6e74 656e 7473 203d        contents =
-000038a0: 205b 6320 666f 7220 6320 696e 2063 6f6e   [c for c in con
-000038b0: 7465 6e74 2069 6620 632e 7368 6131 5f67  tent if c.sha1_g
-000038c0: 6974 2069 6e20 6d69 7373 696e 675d 0a0a  it in missing]..
-000038d0: 2020 2020 2020 2020 7365 6c66 2e6a 6f75          self.jou
-000038e0: 726e 616c 5f77 7269 7465 722e 636f 6e74  rnal_writer.cont
-000038f0: 656e 745f 6164 645f 6d65 7461 6461 7461  ent_add_metadata
-00003900: 2863 6f6e 7465 6e74 7329 0a20 2020 2020  (contents).     
-00003910: 2020 2073 656c 662e 5f63 6f6e 7465 6e74     self._content
-00003920: 5f61 6464 5f6d 6574 6164 6174 6128 6462  _add_metadata(db
-00003930: 2c20 6375 722c 2063 6f6e 7465 6e74 7329  , cur, contents)
-00003940: 0a0a 2020 2020 2020 2020 7265 7475 726e  ..        return
-00003950: 207b 0a20 2020 2020 2020 2020 2020 2022   {.            "
-00003960: 636f 6e74 656e 743a 6164 6422 3a20 6c65  content:add": le
-00003970: 6e28 636f 6e74 656e 7473 292c 0a20 2020  n(contents),.   
-00003980: 2020 2020 207d 0a0a 2020 2020 6465 6620       }..    def 
-00003990: 636f 6e74 656e 745f 6765 745f 6461 7461  content_get_data
-000039a0: 2873 656c 662c 2063 6f6e 7465 6e74 3a20  (self, content: 
-000039b0: 556e 696f 6e5b 4861 7368 4469 6374 2c20  Union[HashDict, 
-000039c0: 5368 6131 5d29 202d 3e20 4f70 7469 6f6e  Sha1]) -> Option
-000039d0: 616c 5b62 7974 6573 5d3a 0a20 2020 2020  al[bytes]:.     
-000039e0: 2020 2023 2046 4958 4d45 3a20 4d61 6b65     # FIXME: Make
-000039f0: 2074 6869 7320 6d65 7468 6f64 2073 7570   this method sup
-00003a00: 706f 7274 2073 6c69 6369 6e67 2074 6865  port slicing the
-00003a10: 2060 6461 7461 600a 2020 2020 2020 2020   `data`.        
-00003a20: 7265 7475 726e 2073 656c 662e 6f62 6a73  return self.objs
-00003a30: 746f 7261 6765 2e63 6f6e 7465 6e74 5f67  torage.content_g
-00003a40: 6574 2863 6f6e 7465 6e74 290a 0a20 2020  et(content)..   
-00003a50: 2040 6462 5f74 7261 6e73 6163 7469 6f6e   @db_transaction
-00003a60: 2829 0a20 2020 2064 6566 2063 6f6e 7465  ().    def conte
-00003a70: 6e74 5f67 6574 5f70 6172 7469 7469 6f6e  nt_get_partition
-00003a80: 280a 2020 2020 2020 2020 7365 6c66 2c0a  (.        self,.
-00003a90: 2020 2020 2020 2020 7061 7274 6974 696f          partitio
-00003aa0: 6e5f 6964 3a20 696e 742c 0a20 2020 2020  n_id: int,.     
-00003ab0: 2020 206e 625f 7061 7274 6974 696f 6e73     nb_partitions
-00003ac0: 3a20 696e 742c 0a20 2020 2020 2020 2070  : int,.        p
-00003ad0: 6167 655f 746f 6b65 6e3a 204f 7074 696f  age_token: Optio
-00003ae0: 6e61 6c5b 7374 725d 203d 204e 6f6e 652c  nal[str] = None,
-00003af0: 0a20 2020 2020 2020 206c 696d 6974 3a20  .        limit: 
-00003b00: 696e 7420 3d20 3130 3030 2c0a 2020 2020  int = 1000,.    
-00003b10: 2020 2020 2a2c 0a20 2020 2020 2020 2064      *,.        d
-00003b20: 623a 2044 622c 0a20 2020 2020 2020 2063  b: Db,.        c
-00003b30: 7572 3d4e 6f6e 652c 0a20 2020 2029 202d  ur=None,.    ) -
-00003b40: 3e20 5061 6765 6452 6573 756c 745b 436f  > PagedResult[Co
-00003b50: 6e74 656e 745d 3a0a 2020 2020 2020 2020  ntent]:.        
-00003b60: 7265 7475 726e 205f 6765 745f 7061 6769  return _get_pagi
-00003b70: 6e61 7465 645f 7368 6131 5f70 6172 7469  nated_sha1_parti
-00003b80: 7469 6f6e 280a 2020 2020 2020 2020 2020  tion(.          
-00003b90: 2020 6375 722c 0a20 2020 2020 2020 2020    cur,.         
-00003ba0: 2020 2070 6172 7469 7469 6f6e 5f69 642c     partition_id,
-00003bb0: 0a20 2020 2020 2020 2020 2020 206e 625f  .            nb_
-00003bc0: 7061 7274 6974 696f 6e73 2c0a 2020 2020  partitions,.    
-00003bd0: 2020 2020 2020 2020 7061 6765 5f74 6f6b          page_tok
-00003be0: 656e 2c0a 2020 2020 2020 2020 2020 2020  en,.            
-00003bf0: 6c69 6d69 742c 0a20 2020 2020 2020 2020  limit,.         
-00003c00: 2020 2064 622e 636f 6e74 656e 745f 6765     db.content_ge
-00003c10: 745f 7261 6e67 652c 0a20 2020 2020 2020  t_range,.       
-00003c20: 2020 2020 206c 616d 6264 6120 726f 773a       lambda row:
-00003c30: 2043 6f6e 7465 6e74 282a 2a64 6963 7428   Content(**dict(
-00003c40: 7a69 7028 6462 2e63 6f6e 7465 6e74 5f67  zip(db.content_g
-00003c50: 6574 5f6d 6574 6164 6174 615f 6b65 7973  et_metadata_keys
-00003c60: 2c20 726f 7729 2929 2c0a 2020 2020 2020  , row))),.      
-00003c70: 2020 2020 2020 6c61 6d62 6461 2072 6f77        lambda row
-00003c80: 3a20 726f 772e 7368 6131 2c0a 2020 2020  : row.sha1,.    
-00003c90: 2020 2020 290a 0a20 2020 2040 6462 5f74      )..    @db_t
-00003ca0: 7261 6e73 6163 7469 6f6e 2873 7461 7465  ransaction(state
-00003cb0: 6d65 6e74 5f74 696d 656f 7574 3d35 3030  ment_timeout=500
-00003cc0: 290a 2020 2020 6465 6620 636f 6e74 656e  ).    def conten
-00003cd0: 745f 6765 7428 0a20 2020 2020 2020 2073  t_get(.        s
-00003ce0: 656c 662c 2063 6f6e 7465 6e74 733a 204c  elf, contents: L
-00003cf0: 6973 745b 6279 7465 735d 2c20 616c 676f  ist[bytes], algo
-00003d00: 3a20 7374 7220 3d20 2273 6861 3122 2c20  : str = "sha1", 
-00003d10: 2a2c 2064 623a 2044 622c 2063 7572 3d4e  *, db: Db, cur=N
-00003d20: 6f6e 650a 2020 2020 2920 2d3e 204c 6973  one.    ) -> Lis
-00003d30: 745b 4f70 7469 6f6e 616c 5b43 6f6e 7465  t[Optional[Conte
-00003d40: 6e74 5d5d 3a0a 2020 2020 2020 2020 636f  nt]]:.        co
-00003d50: 6e74 656e 7473 5f62 795f 6861 7368 3a20  ntents_by_hash: 
-00003d60: 4469 6374 5b62 7974 6573 2c20 4f70 7469  Dict[bytes, Opti
-00003d70: 6f6e 616c 5b43 6f6e 7465 6e74 5d5d 203d  onal[Content]] =
-00003d80: 207b 7d0a 2020 2020 2020 2020 6966 2061   {}.        if a
-00003d90: 6c67 6f20 6e6f 7420 696e 2044 4546 4155  lgo not in DEFAU
-00003da0: 4c54 5f41 4c47 4f52 4954 484d 533a 0a20  LT_ALGORITHMS:. 
-00003db0: 2020 2020 2020 2020 2020 2072 6169 7365             raise
-00003dc0: 2053 746f 7261 6765 4172 6775 6d65 6e74   StorageArgument
-00003dd0: 4578 6365 7074 696f 6e28 0a20 2020 2020  Exception(.     
-00003de0: 2020 2020 2020 2020 2020 2022 616c 676f             "algo
-00003df0: 2073 686f 756c 6420 6265 206f 6e65 206f   should be one o
-00003e00: 6620 7b27 2c27 2e6a 6f69 6e28 4445 4641  f {','.join(DEFA
-00003e10: 554c 545f 414c 474f 5249 5448 4d53 297d  ULT_ALGORITHMS)}
-00003e20: 220a 2020 2020 2020 2020 2020 2020 290a  ".            ).
-00003e30: 0a20 2020 2020 2020 2072 6f77 7320 3d20  .        rows = 
-00003e40: 6462 2e63 6f6e 7465 6e74 5f67 6574 5f6d  db.content_get_m
-00003e50: 6574 6164 6174 615f 6672 6f6d 5f68 6173  etadata_from_has
-00003e60: 6865 7328 636f 6e74 656e 7473 2c20 616c  hes(contents, al
-00003e70: 676f 2c20 6375 7229 0a20 2020 2020 2020  go, cur).       
-00003e80: 206b 6579 203d 206f 7065 7261 746f 722e   key = operator.
-00003e90: 6174 7472 6765 7474 6572 2861 6c67 6f29  attrgetter(algo)
-00003ea0: 0a0a 2020 2020 2020 2020 666f 7220 726f  ..        for ro
-00003eb0: 7720 696e 2072 6f77 733a 0a20 2020 2020  w in rows:.     
-00003ec0: 2020 2020 2020 2072 6f77 5f64 203d 2064         row_d = d
-00003ed0: 6963 7428 7a69 7028 6462 2e63 6f6e 7465  ict(zip(db.conte
-00003ee0: 6e74 5f67 6574 5f6d 6574 6164 6174 615f  nt_get_metadata_
-00003ef0: 6b65 7973 2c20 726f 7729 290a 2020 2020  keys, row)).    
-00003f00: 2020 2020 2020 2020 636f 6e74 656e 7420          content 
-00003f10: 3d20 436f 6e74 656e 7428 2a2a 726f 775f  = Content(**row_
-00003f20: 6429 0a20 2020 2020 2020 2020 2020 2063  d).            c
-00003f30: 6f6e 7465 6e74 735f 6279 5f68 6173 685b  ontents_by_hash[
-00003f40: 6b65 7928 636f 6e74 656e 7429 5d20 3d20  key(content)] = 
-00003f50: 636f 6e74 656e 740a 0a20 2020 2020 2020  content..       
-00003f60: 2072 6574 7572 6e20 5b63 6f6e 7465 6e74   return [content
-00003f70: 735f 6279 5f68 6173 682e 6765 7428 7368  s_by_hash.get(sh
-00003f80: 6131 2920 666f 7220 7368 6131 2069 6e20  a1) for sha1 in 
-00003f90: 636f 6e74 656e 7473 5d0a 0a20 2020 2040  contents]..    @
-00003fa0: 6462 5f74 7261 6e73 6163 7469 6f6e 5f67  db_transaction_g
-00003fb0: 656e 6572 6174 6f72 2829 0a20 2020 2064  enerator().    d
-00003fc0: 6566 2063 6f6e 7465 6e74 5f6d 6973 7369  ef content_missi
-00003fd0: 6e67 280a 2020 2020 2020 2020 7365 6c66  ng(.        self
-00003fe0: 2c0a 2020 2020 2020 2020 636f 6e74 656e  ,.        conten
-00003ff0: 7473 3a20 4c69 7374 5b48 6173 6844 6963  ts: List[HashDic
-00004000: 745d 2c0a 2020 2020 2020 2020 6b65 795f  t],.        key_
-00004010: 6861 7368 3a20 7374 7220 3d20 2273 6861  hash: str = "sha
-00004020: 3122 2c0a 2020 2020 2020 2020 2a2c 0a20  1",.        *,. 
-00004030: 2020 2020 2020 2064 623a 2044 622c 0a20         db: Db,. 
-00004040: 2020 2020 2020 2063 7572 3d4e 6f6e 652c         cur=None,
-00004050: 0a20 2020 2029 202d 3e20 4974 6572 6162  .    ) -> Iterab
-00004060: 6c65 5b62 7974 6573 5d3a 0a20 2020 2020  le[bytes]:.     
-00004070: 2020 2069 6620 6b65 795f 6861 7368 206e     if key_hash n
-00004080: 6f74 2069 6e20 4445 4641 554c 545f 414c  ot in DEFAULT_AL
-00004090: 474f 5249 5448 4d53 3a0a 2020 2020 2020  GORITHMS:.      
-000040a0: 2020 2020 2020 7261 6973 6520 5374 6f72        raise Stor
-000040b0: 6167 6541 7267 756d 656e 7445 7863 6570  ageArgumentExcep
-000040c0: 7469 6f6e 280a 2020 2020 2020 2020 2020  tion(.          
-000040d0: 2020 2020 2020 226b 6579 5f68 6173 6820        "key_hash 
-000040e0: 7368 6f75 6c64 2062 6520 6f6e 6520 6f66  should be one of
-000040f0: 207b 272c 272e 6a6f 696e 2844 4546 4155   {','.join(DEFAU
-00004100: 4c54 5f41 4c47 4f52 4954 484d 5329 7d22  LT_ALGORITHMS)}"
-00004110: 0a20 2020 2020 2020 2020 2020 2029 0a0a  .            )..
-00004120: 2020 2020 2020 2020 6b65 7973 203d 2064          keys = d
-00004130: 622e 636f 6e74 656e 745f 6861 7368 5f6b  b.content_hash_k
-00004140: 6579 730a 2020 2020 2020 2020 6b65 795f  eys.        key_
-00004150: 6861 7368 5f69 6478 203d 206b 6579 732e  hash_idx = keys.
-00004160: 696e 6465 7828 6b65 795f 6861 7368 290a  index(key_hash).
-00004170: 0a20 2020 2020 2020 2066 6f72 206f 626a  .        for obj
-00004180: 2069 6e20 6462 2e63 6f6e 7465 6e74 5f6d   in db.content_m
-00004190: 6973 7369 6e67 5f66 726f 6d5f 6c69 7374  issing_from_list
-000041a0: 2863 6f6e 7465 6e74 732c 2063 7572 293a  (contents, cur):
-000041b0: 0a20 2020 2020 2020 2020 2020 2079 6965  .            yie
-000041c0: 6c64 206f 626a 5b6b 6579 5f68 6173 685f  ld obj[key_hash_
-000041d0: 6964 785d 0a0a 2020 2020 4064 625f 7472  idx]..    @db_tr
-000041e0: 616e 7361 6374 696f 6e5f 6765 6e65 7261  ansaction_genera
-000041f0: 746f 7228 290a 2020 2020 6465 6620 636f  tor().    def co
-00004200: 6e74 656e 745f 6d69 7373 696e 675f 7065  ntent_missing_pe
-00004210: 725f 7368 6131 280a 2020 2020 2020 2020  r_sha1(.        
-00004220: 7365 6c66 2c20 636f 6e74 656e 7473 3a20  self, contents: 
-00004230: 4c69 7374 5b62 7974 6573 5d2c 202a 2c20  List[bytes], *, 
-00004240: 6462 3a20 4462 2c20 6375 723d 4e6f 6e65  db: Db, cur=None
-00004250: 0a20 2020 2029 202d 3e20 4974 6572 6162  .    ) -> Iterab
-00004260: 6c65 5b62 7974 6573 5d3a 0a20 2020 2020  le[bytes]:.     
-00004270: 2020 2066 6f72 206f 626a 2069 6e20 6462     for obj in db
-00004280: 2e63 6f6e 7465 6e74 5f6d 6973 7369 6e67  .content_missing
-00004290: 5f70 6572 5f73 6861 3128 636f 6e74 656e  _per_sha1(conten
-000042a0: 7473 2c20 6375 7229 3a0a 2020 2020 2020  ts, cur):.      
-000042b0: 2020 2020 2020 7969 656c 6420 6f62 6a5b        yield obj[
-000042c0: 305d 0a0a 2020 2020 4064 625f 7472 616e  0]..    @db_tran
-000042d0: 7361 6374 696f 6e5f 6765 6e65 7261 746f  saction_generato
-000042e0: 7228 290a 2020 2020 6465 6620 636f 6e74  r().    def cont
-000042f0: 656e 745f 6d69 7373 696e 675f 7065 725f  ent_missing_per_
-00004300: 7368 6131 5f67 6974 280a 2020 2020 2020  sha1_git(.      
-00004310: 2020 7365 6c66 2c20 636f 6e74 656e 7473    self, contents
-00004320: 3a20 4c69 7374 5b62 7974 6573 5d2c 202a  : List[bytes], *
-00004330: 2c20 6462 3a20 4462 2c20 6375 723d 4e6f  , db: Db, cur=No
-00004340: 6e65 0a20 2020 2029 202d 3e20 4974 6572  ne.    ) -> Iter
-00004350: 6162 6c65 5b53 6861 3147 6974 5d3a 0a20  able[Sha1Git]:. 
-00004360: 2020 2020 2020 2066 6f72 206f 626a 2069         for obj i
-00004370: 6e20 6462 2e63 6f6e 7465 6e74 5f6d 6973  n db.content_mis
-00004380: 7369 6e67 5f70 6572 5f73 6861 315f 6769  sing_per_sha1_gi
-00004390: 7428 636f 6e74 656e 7473 2c20 6375 7229  t(contents, cur)
-000043a0: 3a0a 2020 2020 2020 2020 2020 2020 7969  :.            yi
-000043b0: 656c 6420 6f62 6a5b 305d 0a0a 2020 2020  eld obj[0]..    
-000043c0: 4064 625f 7472 616e 7361 6374 696f 6e28  @db_transaction(
-000043d0: 290a 2020 2020 6465 6620 636f 6e74 656e  ).    def conten
-000043e0: 745f 6669 6e64 2873 656c 662c 2063 6f6e  t_find(self, con
-000043f0: 7465 6e74 3a20 4861 7368 4469 6374 2c20  tent: HashDict, 
-00004400: 2a2c 2064 623a 2044 622c 2063 7572 3d4e  *, db: Db, cur=N
-00004410: 6f6e 6529 202d 3e20 4c69 7374 5b43 6f6e  one) -> List[Con
-00004420: 7465 6e74 5d3a 0a20 2020 2020 2020 2069  tent]:.        i
-00004430: 6620 6e6f 7420 7365 7428 636f 6e74 656e  f not set(conten
-00004440: 7429 2e69 6e74 6572 7365 6374 696f 6e28  t).intersection(
-00004450: 4445 4641 554c 545f 414c 474f 5249 5448  DEFAULT_ALGORITH
-00004460: 4d53 293a 0a20 2020 2020 2020 2020 2020  MS):.           
-00004470: 2072 6169 7365 2053 746f 7261 6765 4172   raise StorageAr
-00004480: 6775 6d65 6e74 4578 6365 7074 696f 6e28  gumentException(
-00004490: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000044a0: 2022 636f 6e74 656e 7420 6b65 7973 206d   "content keys m
-000044b0: 7573 7420 636f 6e74 6169 6e20 6174 206c  ust contain at l
-000044c0: 6561 7374 206f 6e65 2022 0a20 2020 2020  east one ".     
-000044d0: 2020 2020 2020 2020 2020 2066 226f 663a             f"of:
-000044e0: 207b 272c 2027 2e6a 6f69 6e28 736f 7274   {', '.join(sort
-000044f0: 6564 2844 4546 4155 4c54 5f41 4c47 4f52  ed(DEFAULT_ALGOR
-00004500: 4954 484d 5329 297d 220a 2020 2020 2020  ITHMS))}".      
-00004510: 2020 2020 2020 290a 0a20 2020 2020 2020        )..       
-00004520: 2072 6f77 7320 3d20 6462 2e63 6f6e 7465   rows = db.conte
-00004530: 6e74 5f66 696e 6428 0a20 2020 2020 2020  nt_find(.       
-00004540: 2020 2020 2073 6861 313d 636f 6e74 656e       sha1=conten
-00004550: 742e 6765 7428 2273 6861 3122 292c 0a20  t.get("sha1"),. 
-00004560: 2020 2020 2020 2020 2020 2073 6861 315f             sha1_
-00004570: 6769 743d 636f 6e74 656e 742e 6765 7428  git=content.get(
-00004580: 2273 6861 315f 6769 7422 292c 0a20 2020  "sha1_git"),.   
-00004590: 2020 2020 2020 2020 2073 6861 3235 363d           sha256=
-000045a0: 636f 6e74 656e 742e 6765 7428 2273 6861  content.get("sha
-000045b0: 3235 3622 292c 0a20 2020 2020 2020 2020  256"),.         
-000045c0: 2020 2062 6c61 6b65 3273 3235 363d 636f     blake2s256=co
-000045d0: 6e74 656e 742e 6765 7428 2262 6c61 6b65  ntent.get("blake
-000045e0: 3273 3235 3622 292c 0a20 2020 2020 2020  2s256"),.       
-000045f0: 2020 2020 2063 7572 3d63 7572 2c0a 2020       cur=cur,.  
-00004600: 2020 2020 2020 290a 2020 2020 2020 2020        ).        
-00004610: 636f 6e74 656e 7473 203d 205b 5d0a 2020  contents = [].  
-00004620: 2020 2020 2020 666f 7220 726f 7720 696e        for row in
-00004630: 2072 6f77 733a 0a20 2020 2020 2020 2020   rows:.         
-00004640: 2020 2072 6f77 5f64 203d 2064 6963 7428     row_d = dict(
-00004650: 7a69 7028 6462 2e63 6f6e 7465 6e74 5f66  zip(db.content_f
-00004660: 696e 645f 636f 6c73 2c20 726f 7729 290a  ind_cols, row)).
-00004670: 2020 2020 2020 2020 2020 2020 636f 6e74              cont
-00004680: 656e 7473 2e61 7070 656e 6428 436f 6e74  ents.append(Cont
-00004690: 656e 7428 2a2a 726f 775f 6429 290a 2020  ent(**row_d)).  
-000046a0: 2020 2020 2020 7265 7475 726e 2063 6f6e        return con
-000046b0: 7465 6e74 730a 0a20 2020 2040 6462 5f74  tents..    @db_t
-000046c0: 7261 6e73 6163 7469 6f6e 2829 0a20 2020  ransaction().   
-000046d0: 2064 6566 2063 6f6e 7465 6e74 5f67 6574   def content_get
-000046e0: 5f72 616e 646f 6d28 7365 6c66 2c20 2a2c  _random(self, *,
-000046f0: 2064 623a 2044 622c 2063 7572 3d4e 6f6e   db: Db, cur=Non
-00004700: 6529 202d 3e20 5368 6131 4769 743a 0a20  e) -> Sha1Git:. 
-00004710: 2020 2020 2020 2072 6574 7572 6e20 6462         return db
-00004720: 2e63 6f6e 7465 6e74 5f67 6574 5f72 616e  .content_get_ran
-00004730: 646f 6d28 6375 7229 0a0a 2020 2020 2323  dom(cur)..    ##
-00004740: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00004750: 2323 2323 2323 2323 0a20 2020 2023 2053  ########.    # S
-00004760: 6b69 7070 6564 436f 6e74 656e 740a 2020  kippedContent.  
-00004770: 2020 2323 2323 2323 2323 2323 2323 2323    ##############
-00004780: 2323 2323 2323 2323 2323 2323 0a0a 2020  ############..  
-00004790: 2020 4073 7461 7469 636d 6574 686f 640a    @staticmethod.
-000047a0: 2020 2020 6465 6620 5f73 6b69 7070 6564      def _skipped
-000047b0: 5f63 6f6e 7465 6e74 5f6e 6f72 6d61 6c69  _content_normali
-000047c0: 7a65 2864 293a 0a20 2020 2020 2020 2064  ze(d):.        d
-000047d0: 203d 2064 2e63 6f70 7928 290a 0a20 2020   = d.copy()..   
-000047e0: 2020 2020 2069 6620 642e 6765 7428 2273       if d.get("s
-000047f0: 7461 7475 7322 2920 6973 204e 6f6e 653a  tatus") is None:
-00004800: 0a20 2020 2020 2020 2020 2020 2064 5b22  .            d["
-00004810: 7374 6174 7573 225d 203d 2022 6162 7365  status"] = "abse
-00004820: 6e74 220a 0a20 2020 2020 2020 2069 6620  nt"..        if 
-00004830: 642e 6765 7428 226c 656e 6774 6822 2920  d.get("length") 
-00004840: 6973 204e 6f6e 653a 0a20 2020 2020 2020  is None:.       
-00004850: 2020 2020 2064 5b22 6c65 6e67 7468 225d       d["length"]
-00004860: 203d 202d 310a 0a20 2020 2020 2020 2072   = -1..        r
-00004870: 6574 7572 6e20 640a 0a20 2020 2064 6566  eturn d..    def
-00004880: 205f 736b 6970 7065 645f 636f 6e74 656e   _skipped_conten
-00004890: 745f 6164 645f 6d65 7461 6461 7461 2873  t_add_metadata(s
-000048a0: 656c 662c 2064 622c 2063 7572 2c20 636f  elf, db, cur, co
-000048b0: 6e74 656e 743a 204c 6973 745b 536b 6970  ntent: List[Skip
-000048c0: 7065 6443 6f6e 7465 6e74 5d29 3a0a 2020  pedContent]):.  
-000048d0: 2020 2020 2020 6f72 6967 696e 5f69 6473        origin_ids
-000048e0: 203d 2064 622e 6f72 6967 696e 5f69 645f   = db.origin_id_
-000048f0: 6765 745f 6279 5f75 726c 285b 636f 6e74  get_by_url([cont
-00004900: 2e6f 7269 6769 6e20 666f 7220 636f 6e74  .origin for cont
-00004910: 2069 6e20 636f 6e74 656e 745d 2c20 6375   in content], cu
-00004920: 723d 6375 7229 0a20 2020 2020 2020 2063  r=cur).        c
-00004930: 6f6e 7465 6e74 203d 205b 0a20 2020 2020  ontent = [.     
-00004940: 2020 2020 2020 2061 7474 722e 6576 6f6c         attr.evol
-00004950: 7665 2863 2c20 6f72 6967 696e 3d6f 7269  ve(c, origin=ori
-00004960: 6769 6e5f 6964 290a 2020 2020 2020 2020  gin_id).        
-00004970: 2020 2020 666f 7220 2863 2c20 6f72 6967      for (c, orig
-00004980: 696e 5f69 6429 2069 6e20 7a69 7028 636f  in_id) in zip(co
-00004990: 6e74 656e 742c 206f 7269 6769 6e5f 6964  ntent, origin_id
-000049a0: 7329 0a20 2020 2020 2020 205d 0a20 2020  s).        ].   
-000049b0: 2020 2020 2064 622e 6d6b 7465 6d70 2822       db.mktemp("
-000049c0: 736b 6970 7065 645f 636f 6e74 656e 7422  skipped_content"
-000049d0: 2c20 6375 7229 0a20 2020 2020 2020 2064  , cur).        d
-000049e0: 622e 636f 7079 5f74 6f28 0a20 2020 2020  b.copy_to(.     
-000049f0: 2020 2020 2020 205b 632e 746f 5f64 6963         [c.to_dic
-00004a00: 7428 2920 666f 7220 6320 696e 2063 6f6e  t() for c in con
-00004a10: 7465 6e74 5d2c 0a20 2020 2020 2020 2020  tent],.         
-00004a20: 2020 2022 746d 705f 736b 6970 7065 645f     "tmp_skipped_
-00004a30: 636f 6e74 656e 7422 2c0a 2020 2020 2020  content",.      
-00004a40: 2020 2020 2020 6462 2e73 6b69 7070 6564        db.skipped
-00004a50: 5f63 6f6e 7465 6e74 5f6b 6579 732c 0a20  _content_keys,. 
-00004a60: 2020 2020 2020 2020 2020 2063 7572 2c0a             cur,.
-00004a70: 2020 2020 2020 2020 290a 0a20 2020 2020          )..     
-00004a80: 2020 2023 206d 6f76 6520 6d65 7461 6461     # move metada
-00004a90: 7461 2069 6e20 706c 6163 650a 2020 2020  ta in place.    
-00004aa0: 2020 2020 6462 2e73 6b69 7070 6564 5f63      db.skipped_c
-00004ab0: 6f6e 7465 6e74 5f61 6464 5f66 726f 6d5f  ontent_add_from_
-00004ac0: 7465 6d70 2863 7572 290a 0a20 2020 2040  temp(cur)..    @
-00004ad0: 6462 5f74 7261 6e73 6163 7469 6f6e 2829  db_transaction()
-00004ae0: 0a20 2020 2064 6566 2073 6b69 7070 6564  .    def skipped
-00004af0: 5f63 6f6e 7465 6e74 5f61 6464 280a 2020  _content_add(.  
-00004b00: 2020 2020 2020 7365 6c66 2c20 636f 6e74        self, cont
-00004b10: 656e 743a 204c 6973 745b 536b 6970 7065  ent: List[Skippe
-00004b20: 6443 6f6e 7465 6e74 5d2c 202a 2c20 6462  dContent], *, db
-00004b30: 3a20 4462 2c20 6375 723d 4e6f 6e65 0a20  : Db, cur=None. 
-00004b40: 2020 2029 202d 3e20 4469 6374 5b73 7472     ) -> Dict[str
-00004b50: 2c20 696e 745d 3a0a 2020 2020 2020 2020  , int]:.        
-00004b60: 6374 696d 6520 3d20 6e6f 7728 290a 2020  ctime = now().  
-00004b70: 2020 2020 2020 636f 6e74 656e 7420 3d20        content = 
-00004b80: 5b61 7474 722e 6576 6f6c 7665 2863 2c20  [attr.evolve(c, 
-00004b90: 6374 696d 653d 6374 696d 6529 2066 6f72  ctime=ctime) for
-00004ba0: 2063 2069 6e20 636f 6e74 656e 745d 0a0a   c in content]..
-00004bb0: 2020 2020 2020 2020 6d69 7373 696e 675f          missing_
-00004bc0: 636f 6e74 656e 7473 203d 2073 656c 662e  contents = self.
-00004bd0: 736b 6970 7065 645f 636f 6e74 656e 745f  skipped_content_
-00004be0: 6d69 7373 696e 6728 0a20 2020 2020 2020  missing(.       
-00004bf0: 2020 2020 2028 632e 746f 5f64 6963 7428       (c.to_dict(
-00004c00: 2920 666f 7220 6320 696e 2063 6f6e 7465  ) for c in conte
-00004c10: 6e74 292c 0a20 2020 2020 2020 2020 2020  nt),.           
-00004c20: 2064 623d 6462 2c0a 2020 2020 2020 2020   db=db,.        
-00004c30: 2020 2020 6375 723d 6375 722c 0a20 2020      cur=cur,.   
-00004c40: 2020 2020 2029 0a20 2020 2020 2020 2063       ).        c
-00004c50: 6f6e 7465 6e74 203d 205b 0a20 2020 2020  ontent = [.     
-00004c60: 2020 2020 2020 2063 0a20 2020 2020 2020         c.       
-00004c70: 2020 2020 2066 6f72 2063 2069 6e20 636f       for c in co
-00004c80: 6e74 656e 740a 2020 2020 2020 2020 2020  ntent.          
-00004c90: 2020 6966 2061 6e79 280a 2020 2020 2020    if any(.      
-00004ca0: 2020 2020 2020 2020 2020 616c 6c28 0a20            all(. 
-00004cb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004cc0: 2020 2063 2e67 6574 5f68 6173 6828 616c     c.get_hash(al
-00004cd0: 676f 2920 3d3d 206d 6973 7369 6e67 5f63  go) == missing_c
-00004ce0: 6f6e 7465 6e74 2e67 6574 2861 6c67 6f29  ontent.get(algo)
-00004cf0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00004d00: 2020 2020 2066 6f72 2061 6c67 6f20 696e       for algo in
-00004d10: 2044 4546 4155 4c54 5f41 4c47 4f52 4954   DEFAULT_ALGORIT
-00004d20: 484d 530a 2020 2020 2020 2020 2020 2020  HMS.            
-00004d30: 2020 2020 290a 2020 2020 2020 2020 2020      ).          
-00004d40: 2020 2020 2020 666f 7220 6d69 7373 696e        for missin
-00004d50: 675f 636f 6e74 656e 7420 696e 206d 6973  g_content in mis
-00004d60: 7369 6e67 5f63 6f6e 7465 6e74 730a 2020  sing_contents.  
-00004d70: 2020 2020 2020 2020 2020 290a 2020 2020            ).    
-00004d80: 2020 2020 5d0a 0a20 2020 2020 2020 2073      ]..        s
-00004d90: 656c 662e 6a6f 7572 6e61 6c5f 7772 6974  elf.journal_writ
-00004da0: 6572 2e73 6b69 7070 6564 5f63 6f6e 7465  er.skipped_conte
-00004db0: 6e74 5f61 6464 2863 6f6e 7465 6e74 290a  nt_add(content).
-00004dc0: 2020 2020 2020 2020 7365 6c66 2e5f 736b          self._sk
-00004dd0: 6970 7065 645f 636f 6e74 656e 745f 6164  ipped_content_ad
-00004de0: 645f 6d65 7461 6461 7461 2864 622c 2063  d_metadata(db, c
-00004df0: 7572 2c20 636f 6e74 656e 7429 0a0a 2020  ur, content)..  
-00004e00: 2020 2020 2020 7265 7475 726e 207b 0a20        return {. 
-00004e10: 2020 2020 2020 2020 2020 2022 736b 6970             "skip
-00004e20: 7065 645f 636f 6e74 656e 743a 6164 6422  ped_content:add"
-00004e30: 3a20 6c65 6e28 636f 6e74 656e 7429 2c0a  : len(content),.
-00004e40: 2020 2020 2020 2020 7d0a 0a20 2020 2040          }..    @
-00004e50: 6462 5f74 7261 6e73 6163 7469 6f6e 2829  db_transaction()
-00004e60: 0a20 2020 2064 6566 2073 6b69 7070 6564  .    def skipped
-00004e70: 5f63 6f6e 7465 6e74 5f66 696e 6428 0a20  _content_find(. 
-00004e80: 2020 2020 2020 2073 656c 662c 2063 6f6e         self, con
-00004e90: 7465 6e74 3a20 4861 7368 4469 6374 2c20  tent: HashDict, 
-00004ea0: 2a2c 2064 623a 2044 622c 2063 7572 3d4e  *, db: Db, cur=N
-00004eb0: 6f6e 650a 2020 2020 2920 2d3e 204c 6973  one.    ) -> Lis
-00004ec0: 745b 536b 6970 7065 6443 6f6e 7465 6e74  t[SkippedContent
-00004ed0: 5d3a 0a20 2020 2020 2020 2069 6620 6e6f  ]:.        if no
-00004ee0: 7420 7365 7428 636f 6e74 656e 7429 2e69  t set(content).i
-00004ef0: 6e74 6572 7365 6374 696f 6e28 4445 4641  ntersection(DEFA
-00004f00: 554c 545f 414c 474f 5249 5448 4d53 293a  ULT_ALGORITHMS):
-00004f10: 0a20 2020 2020 2020 2020 2020 2072 6169  .            rai
-00004f20: 7365 2053 746f 7261 6765 4172 6775 6d65  se StorageArgume
-00004f30: 6e74 4578 6365 7074 696f 6e28 0a20 2020  ntException(.   
-00004f40: 2020 2020 2020 2020 2020 2020 2022 636f               "co
-00004f50: 6e74 656e 7420 6b65 7973 206d 7573 7420  ntent keys must 
-00004f60: 636f 6e74 6169 6e20 6174 206c 6561 7374  contain at least
-00004f70: 206f 6e65 2022 0a20 2020 2020 2020 2020   one ".         
-00004f80: 2020 2020 2020 2066 226f 663a 207b 272c         f"of: {',
-00004f90: 2027 2e6a 6f69 6e28 736f 7274 6564 2844   '.join(sorted(D
-00004fa0: 4546 4155 4c54 5f41 4c47 4f52 4954 484d  EFAULT_ALGORITHM
-00004fb0: 5329 297d 220a 2020 2020 2020 2020 2020  S))}".          
-00004fc0: 2020 290a 0a20 2020 2020 2020 2072 6f77    )..        row
-00004fd0: 7320 3d20 6462 2e73 6b69 7070 6564 5f63  s = db.skipped_c
-00004fe0: 6f6e 7465 6e74 5f66 696e 6428 0a20 2020  ontent_find(.   
-00004ff0: 2020 2020 2020 2020 2073 6861 313d 636f           sha1=co
-00005000: 6e74 656e 742e 6765 7428 2273 6861 3122  ntent.get("sha1"
-00005010: 292c 0a20 2020 2020 2020 2020 2020 2073  ),.            s
-00005020: 6861 315f 6769 743d 636f 6e74 656e 742e  ha1_git=content.
-00005030: 6765 7428 2273 6861 315f 6769 7422 292c  get("sha1_git"),
-00005040: 0a20 2020 2020 2020 2020 2020 2073 6861  .            sha
-00005050: 3235 363d 636f 6e74 656e 742e 6765 7428  256=content.get(
-00005060: 2273 6861 3235 3622 292c 0a20 2020 2020  "sha256"),.     
-00005070: 2020 2020 2020 2062 6c61 6b65 3273 3235         blake2s25
-00005080: 363d 636f 6e74 656e 742e 6765 7428 2262  6=content.get("b
-00005090: 6c61 6b65 3273 3235 3622 292c 0a20 2020  lake2s256"),.   
-000050a0: 2020 2020 2020 2020 2063 7572 3d63 7572           cur=cur
-000050b0: 2c0a 2020 2020 2020 2020 290a 2020 2020  ,.        ).    
-000050c0: 2020 2020 736b 6970 7065 645f 636f 6e74      skipped_cont
-000050d0: 656e 7473 203d 205b 5d0a 2020 2020 2020  ents = [].      
-000050e0: 2020 666f 7220 726f 7720 696e 2072 6f77    for row in row
-000050f0: 733a 0a20 2020 2020 2020 2020 2020 2072  s:.            r
-00005100: 6f77 5f64 203d 2064 6963 7428 7a69 7028  ow_d = dict(zip(
-00005110: 6462 2e73 6b69 7070 6564 5f63 6f6e 7465  db.skipped_conte
-00005120: 6e74 5f66 696e 645f 636f 6c73 2c20 726f  nt_find_cols, ro
-00005130: 7729 290a 2020 2020 2020 2020 2020 2020  w)).            
-00005140: 736b 6970 7065 645f 636f 6e74 656e 7473  skipped_contents
-00005150: 2e61 7070 656e 6428 536b 6970 7065 6443  .append(SkippedC
-00005160: 6f6e 7465 6e74 282a 2a72 6f77 5f64 2929  ontent(**row_d))
-00005170: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
-00005180: 736b 6970 7065 645f 636f 6e74 656e 7473  skipped_contents
-00005190: 0a0a 2020 2020 4064 625f 7472 616e 7361  ..    @db_transa
-000051a0: 6374 696f 6e5f 6765 6e65 7261 746f 7228  ction_generator(
-000051b0: 290a 2020 2020 6465 6620 736b 6970 7065  ).    def skippe
-000051c0: 645f 636f 6e74 656e 745f 6d69 7373 696e  d_content_missin
-000051d0: 6728 0a20 2020 2020 2020 2073 656c 662c  g(.        self,
-000051e0: 2063 6f6e 7465 6e74 733a 204c 6973 745b   contents: List[
-000051f0: 4469 6374 5b73 7472 2c20 416e 795d 5d2c  Dict[str, Any]],
-00005200: 202a 2c20 6462 3a20 4462 2c20 6375 723d   *, db: Db, cur=
-00005210: 4e6f 6e65 0a20 2020 2029 202d 3e20 4974  None.    ) -> It
-00005220: 6572 6162 6c65 5b44 6963 745b 7374 722c  erable[Dict[str,
-00005230: 2041 6e79 5d5d 3a0a 2020 2020 2020 2020   Any]]:.        
-00005240: 636f 6e74 656e 7473 203d 206c 6973 7428  contents = list(
-00005250: 636f 6e74 656e 7473 290a 2020 2020 2020  contents).      
-00005260: 2020 666f 7220 636f 6e74 656e 7420 696e    for content in
-00005270: 2064 622e 736b 6970 7065 645f 636f 6e74   db.skipped_cont
-00005280: 656e 745f 6d69 7373 696e 6728 636f 6e74  ent_missing(cont
-00005290: 656e 7473 2c20 6375 7229 3a0a 2020 2020  ents, cur):.    
-000052a0: 2020 2020 2020 2020 7969 656c 6420 7b0a          yield {.
-000052b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000052c0: 616c 676f 3a20 6861 7368 0a20 2020 2020  algo: hash.     
-000052d0: 2020 2020 2020 2020 2020 2066 6f72 2028             for (
-000052e0: 616c 676f 2c20 6861 7368 2920 696e 207a  algo, hash) in z
-000052f0: 6970 2864 622e 636f 6e74 656e 745f 6861  ip(db.content_ha
-00005300: 7368 5f6b 6579 732c 2063 6f6e 7465 6e74  sh_keys, content
-00005310: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
-00005320: 2020 6966 2068 6173 680a 2020 2020 2020    if hash.      
-00005330: 2020 2020 2020 7d0a 0a20 2020 2023 2323        }..    ###
-00005340: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00005350: 2323 2323 2323 230a 2020 2020 2320 4469  #######.    # Di
-00005360: 7265 6374 6f72 790a 2020 2020 2323 2323  rectory.    ####
-00005370: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00005380: 2323 2323 2323 0a0a 2020 2020 4064 625f  ######..    @db_
-00005390: 7472 616e 7361 6374 696f 6e28 290a 2020  transaction().  
-000053a0: 2020 6465 6620 6469 7265 6374 6f72 795f    def directory_
-000053b0: 6164 6428 0a20 2020 2020 2020 2073 656c  add(.        sel
-000053c0: 662c 2064 6972 6563 746f 7269 6573 3a20  f, directories: 
-000053d0: 4c69 7374 5b44 6972 6563 746f 7279 5d2c  List[Directory],
-000053e0: 202a 2c20 6462 3a20 4462 2c20 6375 723d   *, db: Db, cur=
-000053f0: 4e6f 6e65 0a20 2020 2029 202d 3e20 4469  None.    ) -> Di
-00005400: 6374 5b73 7472 2c20 696e 745d 3a0a 2020  ct[str, int]:.  
-00005410: 2020 2020 2020 7375 6d6d 6172 7920 3d20        summary = 
-00005420: 7b22 6469 7265 6374 6f72 793a 6164 6422  {"directory:add"
-00005430: 3a20 307d 0a0a 2020 2020 2020 2020 6469  : 0}..        di
-00005440: 7273 203d 2073 6574 2829 0a20 2020 2020  rs = set().     
-00005450: 2020 2064 6972 5f65 6e74 7269 6573 3a20     dir_entries: 
-00005460: 4469 6374 5b73 7472 2c20 6465 6661 756c  Dict[str, defaul
-00005470: 7464 6963 745d 203d 207b 0a20 2020 2020  tdict] = {.     
-00005480: 2020 2020 2020 2022 6669 6c65 223a 2064         "file": d
-00005490: 6566 6175 6c74 6469 6374 286c 6973 7429  efaultdict(list)
-000054a0: 2c0a 2020 2020 2020 2020 2020 2020 2264  ,.            "d
-000054b0: 6972 223a 2064 6566 6175 6c74 6469 6374  ir": defaultdict
-000054c0: 286c 6973 7429 2c0a 2020 2020 2020 2020  (list),.        
-000054d0: 2020 2020 2272 6576 223a 2064 6566 6175      "rev": defau
-000054e0: 6c74 6469 6374 286c 6973 7429 2c0a 2020  ltdict(list),.  
-000054f0: 2020 2020 2020 7d0a 0a20 2020 2020 2020        }..       
-00005500: 2066 6f72 2063 7572 5f64 6972 2069 6e20   for cur_dir in 
-00005510: 6469 7265 6374 6f72 6965 733a 0a20 2020  directories:.   
-00005520: 2020 2020 2020 2020 2064 6972 5f69 6420           dir_id 
-00005530: 3d20 6375 725f 6469 722e 6964 0a20 2020  = cur_dir.id.   
-00005540: 2020 2020 2020 2020 2064 6972 732e 6164           dirs.ad
-00005550: 6428 6469 725f 6964 290a 2020 2020 2020  d(dir_id).      
-00005560: 2020 2020 2020 666f 7220 7372 635f 656e        for src_en
-00005570: 7472 7920 696e 2063 7572 5f64 6972 2e65  try in cur_dir.e
-00005580: 6e74 7269 6573 3a0a 2020 2020 2020 2020  ntries:.        
-00005590: 2020 2020 2020 2020 656e 7472 7920 3d20          entry = 
-000055a0: 7372 635f 656e 7472 792e 746f 5f64 6963  src_entry.to_dic
-000055b0: 7428 290a 2020 2020 2020 2020 2020 2020  t().            
-000055c0: 2020 2020 656e 7472 795b 2264 6972 5f69      entry["dir_i
-000055d0: 6422 5d20 3d20 6469 725f 6964 0a20 2020  d"] = dir_id.   
-000055e0: 2020 2020 2020 2020 2020 2020 2064 6972               dir
-000055f0: 5f65 6e74 7269 6573 5b65 6e74 7279 5b22  _entries[entry["
-00005600: 7479 7065 225d 5d5b 6469 725f 6964 5d2e  type"]][dir_id].
-00005610: 6170 7065 6e64 2865 6e74 7279 290a 0a20  append(entry).. 
-00005620: 2020 2020 2020 2064 6972 735f 6d69 7373         dirs_miss
-00005630: 696e 6720 3d20 7365 7428 7365 6c66 2e64  ing = set(self.d
-00005640: 6972 6563 746f 7279 5f6d 6973 7369 6e67  irectory_missing
-00005650: 2864 6972 732c 2064 623d 6462 2c20 6375  (dirs, db=db, cu
-00005660: 723d 6375 7229 290a 2020 2020 2020 2020  r=cur)).        
-00005670: 6966 206e 6f74 2064 6972 735f 6d69 7373  if not dirs_miss
-00005680: 696e 673a 0a20 2020 2020 2020 2020 2020  ing:.           
-00005690: 2072 6574 7572 6e20 7375 6d6d 6172 790a   return summary.
-000056a0: 0a20 2020 2020 2020 2073 656c 662e 6a6f  .        self.jo
-000056b0: 7572 6e61 6c5f 7772 6974 6572 2e64 6972  urnal_writer.dir
-000056c0: 6563 746f 7279 5f61 6464 280a 2020 2020  ectory_add(.    
-000056d0: 2020 2020 2020 2020 6469 725f 2066 6f72          dir_ for
-000056e0: 2064 6972 5f20 696e 2064 6972 6563 746f   dir_ in directo
-000056f0: 7269 6573 2069 6620 6469 725f 2e69 6420  ries if dir_.id 
-00005700: 696e 2064 6972 735f 6d69 7373 696e 670a  in dirs_missing.
-00005710: 2020 2020 2020 2020 290a 0a20 2020 2020          )..     
-00005720: 2020 2023 2043 6f70 7920 6469 7265 6374     # Copy direct
-00005730: 6f72 7920 6d65 7461 6461 7461 0a20 2020  ory metadata.   
-00005740: 2020 2020 2064 6972 735f 6d69 7373 696e       dirs_missin
-00005750: 675f 6469 6374 203d 2028 0a20 2020 2020  g_dict = (.     
-00005760: 2020 2020 2020 207b 2269 6422 3a20 6469         {"id": di
-00005770: 725f 2e69 642c 2022 7261 775f 6d61 6e69  r_.id, "raw_mani
-00005780: 6665 7374 223a 2064 6972 5f2e 7261 775f  fest": dir_.raw_
-00005790: 6d61 6e69 6665 7374 7d0a 2020 2020 2020  manifest}.      
-000057a0: 2020 2020 2020 666f 7220 6469 725f 2069        for dir_ i
-000057b0: 6e20 6469 7265 6374 6f72 6965 730a 2020  n directories.  
-000057c0: 2020 2020 2020 2020 2020 6966 2064 6972            if dir
-000057d0: 5f2e 6964 2069 6e20 6469 7273 5f6d 6973  _.id in dirs_mis
-000057e0: 7369 6e67 0a20 2020 2020 2020 2029 0a20  sing.        ). 
-000057f0: 2020 2020 2020 2064 622e 6d6b 7465 6d70         db.mktemp
-00005800: 2822 6469 7265 6374 6f72 7922 2c20 6375  ("directory", cu
-00005810: 7229 0a20 2020 2020 2020 2064 622e 636f  r).        db.co
-00005820: 7079 5f74 6f28 6469 7273 5f6d 6973 7369  py_to(dirs_missi
-00005830: 6e67 5f64 6963 742c 2022 746d 705f 6469  ng_dict, "tmp_di
-00005840: 7265 6374 6f72 7922 2c20 5b22 6964 222c  rectory", ["id",
-00005850: 2022 7261 775f 6d61 6e69 6665 7374 225d   "raw_manifest"]
-00005860: 2c20 6375 7229 0a0a 2020 2020 2020 2020  , cur)..        
-00005870: 2320 436f 7079 2065 6e74 7269 6573 0a20  # Copy entries. 
-00005880: 2020 2020 2020 2066 6f72 2065 6e74 7279         for entry
-00005890: 5f74 7970 652c 2065 6e74 7279 5f6c 6973  _type, entry_lis
-000058a0: 7420 696e 2064 6972 5f65 6e74 7269 6573  t in dir_entries
-000058b0: 2e69 7465 6d73 2829 3a0a 2020 2020 2020  .items():.      
-000058c0: 2020 2020 2020 656e 7472 6965 7320 3d20        entries = 
-000058d0: 6974 6572 746f 6f6c 732e 6368 6169 6e2e  itertools.chain.
-000058e0: 6672 6f6d 5f69 7465 7261 626c 6528 0a20  from_iterable(. 
-000058f0: 2020 2020 2020 2020 2020 2020 2020 2065                 e
-00005900: 6e74 7269 6573 5f66 6f72 5f64 6972 0a20  ntries_for_dir. 
-00005910: 2020 2020 2020 2020 2020 2020 2020 2066                 f
-00005920: 6f72 2064 6972 5f69 642c 2065 6e74 7269  or dir_id, entri
-00005930: 6573 5f66 6f72 5f64 6972 2069 6e20 656e  es_for_dir in en
-00005940: 7472 795f 6c69 7374 2e69 7465 6d73 2829  try_list.items()
-00005950: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00005960: 2069 6620 6469 725f 6964 2069 6e20 6469   if dir_id in di
-00005970: 7273 5f6d 6973 7369 6e67 0a20 2020 2020  rs_missing.     
-00005980: 2020 2020 2020 2029 0a0a 2020 2020 2020         )..      
-00005990: 2020 2020 2020 6462 2e6d 6b74 656d 705f        db.mktemp_
-000059a0: 6469 725f 656e 7472 7928 656e 7472 795f  dir_entry(entry_
-000059b0: 7479 7065 290a 0a20 2020 2020 2020 2020  type)..         
-000059c0: 2020 2064 622e 636f 7079 5f74 6f28 0a20     db.copy_to(. 
-000059d0: 2020 2020 2020 2020 2020 2020 2020 2065                 e
-000059e0: 6e74 7269 6573 2c0a 2020 2020 2020 2020  ntries,.        
-000059f0: 2020 2020 2020 2020 2274 6d70 5f64 6972          "tmp_dir
-00005a00: 6563 746f 7279 5f65 6e74 7279 5f25 7322  ectory_entry_%s"
-00005a10: 2025 2065 6e74 7279 5f74 7970 652c 0a20   % entry_type,. 
-00005a20: 2020 2020 2020 2020 2020 2020 2020 205b                 [
-00005a30: 2274 6172 6765 7422 2c20 226e 616d 6522  "target", "name"
-00005a40: 2c20 2270 6572 6d73 222c 2022 6469 725f  , "perms", "dir_
-00005a50: 6964 225d 2c0a 2020 2020 2020 2020 2020  id"],.          
-00005a60: 2020 2020 2020 6375 722c 0a20 2020 2020        cur,.     
-00005a70: 2020 2020 2020 2029 0a0a 2020 2020 2020         )..      
-00005a80: 2020 2320 446f 2074 6865 2066 696e 616c    # Do the final
-00005a90: 2063 6f70 790a 2020 2020 2020 2020 6462   copy.        db
-00005aa0: 2e64 6972 6563 746f 7279 5f61 6464 5f66  .directory_add_f
-00005ab0: 726f 6d5f 7465 6d70 2863 7572 290a 2020  rom_temp(cur).  
-00005ac0: 2020 2020 2020 7375 6d6d 6172 795b 2264        summary["d
-00005ad0: 6972 6563 746f 7279 3a61 6464 225d 203d  irectory:add"] =
-00005ae0: 206c 656e 2864 6972 735f 6d69 7373 696e   len(dirs_missin
-00005af0: 6729 0a0a 2020 2020 2020 2020 7265 7475  g)..        retu
-00005b00: 726e 2073 756d 6d61 7279 0a0a 2020 2020  rn summary..    
-00005b10: 4064 625f 7472 616e 7361 6374 696f 6e5f  @db_transaction_
-00005b20: 6765 6e65 7261 746f 7228 290a 2020 2020  generator().    
-00005b30: 6465 6620 6469 7265 6374 6f72 795f 6d69  def directory_mi
-00005b40: 7373 696e 6728 0a20 2020 2020 2020 2073  ssing(.        s
-00005b50: 656c 662c 2064 6972 6563 746f 7269 6573  elf, directories
-00005b60: 3a20 4c69 7374 5b53 6861 3147 6974 5d2c  : List[Sha1Git],
-00005b70: 202a 2c20 6462 3a20 4462 2c20 6375 723d   *, db: Db, cur=
-00005b80: 4e6f 6e65 0a20 2020 2029 202d 3e20 4974  None.    ) -> It
-00005b90: 6572 6162 6c65 5b53 6861 3147 6974 5d3a  erable[Sha1Git]:
-00005ba0: 0a20 2020 2020 2020 2066 6f72 206f 626a  .        for obj
-00005bb0: 2069 6e20 6462 2e64 6972 6563 746f 7279   in db.directory
-00005bc0: 5f6d 6973 7369 6e67 5f66 726f 6d5f 6c69  _missing_from_li
-00005bd0: 7374 2864 6972 6563 746f 7269 6573 2c20  st(directories, 
-00005be0: 6375 7229 3a0a 2020 2020 2020 2020 2020  cur):.          
-00005bf0: 2020 7969 656c 6420 6f62 6a5b 305d 0a0a    yield obj[0]..
-00005c00: 2020 2020 4064 625f 7472 616e 7361 6374      @db_transact
-00005c10: 696f 6e5f 6765 6e65 7261 746f 7228 7374  ion_generator(st
-00005c20: 6174 656d 656e 745f 7469 6d65 6f75 743d  atement_timeout=
-00005c30: 3230 3030 3029 0a20 2020 2064 6566 2064  20000).    def d
-00005c40: 6972 6563 746f 7279 5f6c 7328 0a20 2020  irectory_ls(.   
-00005c50: 2020 2020 2073 656c 662c 2064 6972 6563       self, direc
-00005c60: 746f 7279 3a20 5368 6131 4769 742c 2072  tory: Sha1Git, r
-00005c70: 6563 7572 7369 7665 3a20 626f 6f6c 203d  ecursive: bool =
-00005c80: 2046 616c 7365 2c20 2a2c 2064 623a 2044   False, *, db: D
-00005c90: 622c 2063 7572 3d4e 6f6e 650a 2020 2020  b, cur=None.    
-00005ca0: 2920 2d3e 2049 7465 7261 626c 655b 4469  ) -> Iterable[Di
-00005cb0: 6374 5b73 7472 2c20 416e 795d 5d3a 0a20  ct[str, Any]]:. 
-00005cc0: 2020 2020 2020 2069 6620 7265 6375 7273         if recurs
-00005cd0: 6976 653a 0a20 2020 2020 2020 2020 2020  ive:.           
-00005ce0: 2072 6573 5f67 656e 203d 2064 622e 6469   res_gen = db.di
-00005cf0: 7265 6374 6f72 795f 7761 6c6b 2864 6972  rectory_walk(dir
-00005d00: 6563 746f 7279 2c20 6375 723d 6375 7229  ectory, cur=cur)
-00005d10: 0a20 2020 2020 2020 2065 6c73 653a 0a20  .        else:. 
-00005d20: 2020 2020 2020 2020 2020 2072 6573 5f67             res_g
-00005d30: 656e 203d 2064 622e 6469 7265 6374 6f72  en = db.director
-00005d40: 795f 7761 6c6b 5f6f 6e65 2864 6972 6563  y_walk_one(direc
-00005d50: 746f 7279 2c20 6375 723d 6375 7229 0a0a  tory, cur=cur)..
-00005d60: 2020 2020 2020 2020 666f 7220 6c69 6e65          for line
-00005d70: 2069 6e20 7265 735f 6765 6e3a 0a20 2020   in res_gen:.   
-00005d80: 2020 2020 2020 2020 2079 6965 6c64 2064           yield d
-00005d90: 6963 7428 7a69 7028 6462 2e64 6972 6563  ict(zip(db.direc
-00005da0: 746f 7279 5f6c 735f 636f 6c73 2c20 6c69  tory_ls_cols, li
-00005db0: 6e65 2929 0a0a 2020 2020 4064 625f 7472  ne))..    @db_tr
-00005dc0: 616e 7361 6374 696f 6e28 7374 6174 656d  ansaction(statem
-00005dd0: 656e 745f 7469 6d65 6f75 743d 3430 3030  ent_timeout=4000
-00005de0: 290a 2020 2020 6465 6620 6469 7265 6374  ).    def direct
-00005df0: 6f72 795f 656e 7472 795f 6765 745f 6279  ory_entry_get_by
-00005e00: 5f70 6174 6828 0a20 2020 2020 2020 2073  _path(.        s
-00005e10: 656c 662c 2064 6972 6563 746f 7279 3a20  elf, directory: 
-00005e20: 5368 6131 4769 742c 2070 6174 6873 3a20  Sha1Git, paths: 
-00005e30: 4c69 7374 5b62 7974 6573 5d2c 202a 2c20  List[bytes], *, 
-00005e40: 6462 3a20 4462 2c20 6375 723d 4e6f 6e65  db: Db, cur=None
-00005e50: 0a20 2020 2029 202d 3e20 4f70 7469 6f6e  .    ) -> Option
-00005e60: 616c 5b44 6963 745b 7374 722c 2041 6e79  al[Dict[str, Any
-00005e70: 5d5d 3a0a 2020 2020 2020 2020 7265 7320  ]]:.        res 
-00005e80: 3d20 6462 2e64 6972 6563 746f 7279 5f65  = db.directory_e
-00005e90: 6e74 7279 5f67 6574 5f62 795f 7061 7468  ntry_get_by_path
-00005ea0: 2864 6972 6563 746f 7279 2c20 7061 7468  (directory, path
-00005eb0: 732c 2063 7572 290a 2020 2020 2020 2020  s, cur).        
-00005ec0: 7265 7475 726e 2064 6963 7428 7a69 7028  return dict(zip(
-00005ed0: 6462 2e64 6972 6563 746f 7279 5f6c 735f  db.directory_ls_
-00005ee0: 636f 6c73 2c20 7265 7329 2920 6966 2072  cols, res)) if r
-00005ef0: 6573 2065 6c73 6520 4e6f 6e65 0a0a 2020  es else None..  
-00005f00: 2020 4064 625f 7472 616e 7361 6374 696f    @db_transactio
-00005f10: 6e28 290a 2020 2020 6465 6620 6469 7265  n().    def dire
-00005f20: 6374 6f72 795f 6765 745f 7261 6e64 6f6d  ctory_get_random
-00005f30: 2873 656c 662c 202a 2c20 6462 3a20 4462  (self, *, db: Db
-00005f40: 2c20 6375 723d 4e6f 6e65 2920 2d3e 2053  , cur=None) -> S
-00005f50: 6861 3147 6974 3a0a 2020 2020 2020 2020  ha1Git:.        
-00005f60: 7265 7475 726e 2064 622e 6469 7265 6374  return db.direct
-00005f70: 6f72 795f 6765 745f 7261 6e64 6f6d 2863  ory_get_random(c
-00005f80: 7572 290a 0a20 2020 2040 6462 5f74 7261  ur)..    @db_tra
-00005f90: 6e73 6163 7469 6f6e 2829 0a20 2020 2064  nsaction().    d
-00005fa0: 6566 2064 6972 6563 746f 7279 5f67 6574  ef directory_get
-00005fb0: 5f65 6e74 7269 6573 280a 2020 2020 2020  _entries(.      
-00005fc0: 2020 7365 6c66 2c0a 2020 2020 2020 2020    self,.        
-00005fd0: 6469 7265 6374 6f72 795f 6964 3a20 5368  directory_id: Sh
-00005fe0: 6131 4769 742c 0a20 2020 2020 2020 2070  a1Git,.        p
-00005ff0: 6167 655f 746f 6b65 6e3a 204f 7074 696f  age_token: Optio
-00006000: 6e61 6c5b 6279 7465 735d 203d 204e 6f6e  nal[bytes] = Non
-00006010: 652c 0a20 2020 2020 2020 206c 696d 6974  e,.        limit
-00006020: 3a20 696e 7420 3d20 3130 3030 2c0a 2020  : int = 1000,.  
-00006030: 2020 2020 2020 2a2c 0a20 2020 2020 2020        *,.       
-00006040: 2064 623a 2044 622c 0a20 2020 2020 2020   db: Db,.       
-00006050: 2063 7572 3d4e 6f6e 652c 0a20 2020 2029   cur=None,.    )
-00006060: 202d 3e20 4f70 7469 6f6e 616c 5b50 6167   -> Optional[Pag
-00006070: 6564 5265 7375 6c74 5b44 6972 6563 746f  edResult[Directo
-00006080: 7279 456e 7472 795d 5d3a 0a20 2020 2020  ryEntry]]:.     
-00006090: 2020 2069 6620 6c69 7374 2873 656c 662e     if list(self.
-000060a0: 6469 7265 6374 6f72 795f 6d69 7373 696e  directory_missin
-000060b0: 6728 5b64 6972 6563 746f 7279 5f69 645d  g([directory_id]
-000060c0: 2c20 6462 3d64 622c 2063 7572 3d63 7572  , db=db, cur=cur
-000060d0: 2929 3a0a 2020 2020 2020 2020 2020 2020  )):.            
-000060e0: 7265 7475 726e 204e 6f6e 650a 0a20 2020  return None..   
-000060f0: 2020 2020 2069 6620 7061 6765 5f74 6f6b       if page_tok
-00006100: 656e 2069 7320 6e6f 7420 4e6f 6e65 3a0a  en is not None:.
-00006110: 2020 2020 2020 2020 2020 2020 7261 6973              rais
-00006120: 6520 5374 6f72 6167 6541 7267 756d 656e  e StorageArgumen
-00006130: 7445 7863 6570 7469 6f6e 2822 556e 7375  tException("Unsu
-00006140: 7070 6f72 7465 6420 7061 6765 2074 6f6b  pported page tok
-00006150: 656e 2229 0a0a 2020 2020 2020 2020 2320  en")..        # 
-00006160: 544f 444f 3a20 6163 7475 616c 6c79 2070  TODO: actually p
-00006170: 6167 696e 6174 650a 2020 2020 2020 2020  aginate.        
-00006180: 726f 7773 203d 2064 622e 6469 7265 6374  rows = db.direct
-00006190: 6f72 795f 6765 745f 656e 7472 6965 7328  ory_get_entries(
-000061a0: 6469 7265 6374 6f72 795f 6964 2c20 6375  directory_id, cu
-000061b0: 723d 6375 7229 0a20 2020 2020 2020 2072  r=cur).        r
-000061c0: 6574 7572 6e20 5061 6765 6452 6573 756c  eturn PagedResul
-000061d0: 7428 0a20 2020 2020 2020 2020 2020 2072  t(.            r
-000061e0: 6573 756c 7473 3d5b 0a20 2020 2020 2020  esults=[.       
-000061f0: 2020 2020 2020 2020 2044 6972 6563 746f           Directo
-00006200: 7279 456e 7472 7928 2a2a 6469 6374 287a  ryEntry(**dict(z
-00006210: 6970 2864 622e 6469 7265 6374 6f72 795f  ip(db.directory_
-00006220: 6765 745f 656e 7472 6965 735f 636f 6c73  get_entries_cols
-00006230: 2c20 726f 7729 2929 0a20 2020 2020 2020  , row))).       
-00006240: 2020 2020 2020 2020 2066 6f72 2072 6f77           for row
-00006250: 2069 6e20 726f 7773 0a20 2020 2020 2020   in rows.       
-00006260: 2020 2020 205d 2c0a 2020 2020 2020 2020       ],.        
-00006270: 2020 2020 6e65 7874 5f70 6167 655f 746f      next_page_to
-00006280: 6b65 6e3d 4e6f 6e65 2c0a 2020 2020 2020  ken=None,.      
-00006290: 2020 290a 0a20 2020 2040 6462 5f74 7261    )..    @db_tra
-000062a0: 6e73 6163 7469 6f6e 2829 0a20 2020 2064  nsaction().    d
-000062b0: 6566 2064 6972 6563 746f 7279 5f67 6574  ef directory_get
-000062c0: 5f72 6177 5f6d 616e 6966 6573 7428 0a20  _raw_manifest(. 
-000062d0: 2020 2020 2020 2073 656c 662c 2064 6972         self, dir
-000062e0: 6563 746f 7279 5f69 6473 3a20 4c69 7374  ectory_ids: List
-000062f0: 5b53 6861 3147 6974 5d2c 202a 2c20 6462  [Sha1Git], *, db
-00006300: 3a20 4462 2c20 6375 723d 4e6f 6e65 0a20  : Db, cur=None. 
-00006310: 2020 2029 202d 3e20 4469 6374 5b53 6861     ) -> Dict[Sha
-00006320: 3147 6974 2c20 4f70 7469 6f6e 616c 5b62  1Git, Optional[b
-00006330: 7974 6573 5d5d 3a0a 2020 2020 2020 2020  ytes]]:.        
-00006340: 7265 7475 726e 2064 6963 7428 6462 2e64  return dict(db.d
-00006350: 6972 6563 746f 7279 5f67 6574 5f72 6177  irectory_get_raw
-00006360: 5f6d 616e 6966 6573 7428 6469 7265 6374  _manifest(direct
-00006370: 6f72 795f 6964 732c 2063 7572 3d63 7572  ory_ids, cur=cur
-00006380: 2929 0a0a 2020 2020 4064 625f 7472 616e  ))..    @db_tran
-00006390: 7361 6374 696f 6e28 290a 2020 2020 6465  saction().    de
-000063a0: 6620 6469 7265 6374 6f72 795f 6765 745f  f directory_get_
-000063b0: 6964 5f70 6172 7469 7469 6f6e 280a 2020  id_partition(.  
-000063c0: 2020 2020 2020 7365 6c66 2c0a 2020 2020        self,.    
-000063d0: 2020 2020 7061 7274 6974 696f 6e5f 6964      partition_id
-000063e0: 3a20 696e 742c 0a20 2020 2020 2020 206e  : int,.        n
-000063f0: 625f 7061 7274 6974 696f 6e73 3a20 696e  b_partitions: in
-00006400: 742c 0a20 2020 2020 2020 2070 6167 655f  t,.        page_
-00006410: 746f 6b65 6e3a 204f 7074 696f 6e61 6c5b  token: Optional[
-00006420: 7374 725d 203d 204e 6f6e 652c 0a20 2020  str] = None,.   
-00006430: 2020 2020 206c 696d 6974 3a20 696e 7420       limit: int 
-00006440: 3d20 3130 3030 2c0a 2020 2020 2020 2020  = 1000,.        
-00006450: 2a2c 0a20 2020 2020 2020 2064 623a 2044  *,.        db: D
-00006460: 622c 0a20 2020 2020 2020 2063 7572 3d4e  b,.        cur=N
-00006470: 6f6e 652c 0a20 2020 2029 202d 3e20 5061  one,.    ) -> Pa
-00006480: 6765 6452 6573 756c 745b 5368 6131 4769  gedResult[Sha1Gi
-00006490: 745d 3a0a 2020 2020 2020 2020 7265 7475  t]:.        retu
-000064a0: 726e 205f 6765 745f 7061 6769 6e61 7465  rn _get_paginate
-000064b0: 645f 7368 6131 5f70 6172 7469 7469 6f6e  d_sha1_partition
-000064c0: 280a 2020 2020 2020 2020 2020 2020 6375  (.            cu
-000064d0: 722c 0a20 2020 2020 2020 2020 2020 2070  r,.            p
-000064e0: 6172 7469 7469 6f6e 5f69 642c 0a20 2020  artition_id,.   
-000064f0: 2020 2020 2020 2020 206e 625f 7061 7274           nb_part
-00006500: 6974 696f 6e73 2c0a 2020 2020 2020 2020  itions,.        
-00006510: 2020 2020 7061 6765 5f74 6f6b 656e 2c0a      page_token,.
-00006520: 2020 2020 2020 2020 2020 2020 6c69 6d69              limi
-00006530: 742c 0a20 2020 2020 2020 2020 2020 2064  t,.            d
-00006540: 622e 6469 7265 6374 6f72 795f 6765 745f  b.directory_get_
-00006550: 6964 5f72 616e 6765 2c0a 2020 2020 2020  id_range,.      
-00006560: 2020 2020 2020 6f70 6572 6174 6f72 2e69        operator.i
-00006570: 7465 6d67 6574 7465 7228 3029 2c0a 2020  temgetter(0),.  
-00006580: 2020 2020 2020 2020 2020 6c61 6d62 6461            lambda
-00006590: 2069 645f 3a20 6964 5f2c 0a20 2020 2020   id_: id_,.     
-000065a0: 2020 2029 0a0a 2020 2020 2323 2323 2323     )..    ######
-000065b0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-000065c0: 2323 2323 0a20 2020 2023 2052 6576 6973  ####.    # Revis
-000065d0: 696f 6e0a 2020 2020 2323 2323 2323 2323  ion.    ########
-000065e0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-000065f0: 2323 0a0a 2020 2020 4064 625f 7472 616e  ##..    @db_tran
-00006600: 7361 6374 696f 6e28 290a 2020 2020 6465  saction().    de
-00006610: 6620 7265 7669 7369 6f6e 5f61 6464 280a  f revision_add(.
-00006620: 2020 2020 2020 2020 7365 6c66 2c20 7265          self, re
-00006630: 7669 7369 6f6e 733a 204c 6973 745b 5265  visions: List[Re
-00006640: 7669 7369 6f6e 5d2c 202a 2c20 6462 3a20  vision], *, db: 
-00006650: 4462 2c20 6375 723d 4e6f 6e65 0a20 2020  Db, cur=None.   
-00006660: 2029 202d 3e20 4469 6374 5b73 7472 2c20   ) -> Dict[str, 
-00006670: 696e 745d 3a0a 2020 2020 2020 2020 7375  int]:.        su
-00006680: 6d6d 6172 7920 3d20 7b22 7265 7669 7369  mmary = {"revisi
-00006690: 6f6e 3a61 6464 223a 2030 7d0a 0a20 2020  on:add": 0}..   
-000066a0: 2020 2020 2072 6576 6973 696f 6e73 5f6d       revisions_m
-000066b0: 6973 7369 6e67 203d 2073 6574 280a 2020  issing = set(.  
-000066c0: 2020 2020 2020 2020 2020 7365 6c66 2e72            self.r
-000066d0: 6576 6973 696f 6e5f 6d69 7373 696e 6728  evision_missing(
-000066e0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000066f0: 2073 6574 2872 6576 6973 696f 6e2e 6964   set(revision.id
-00006700: 2066 6f72 2072 6576 6973 696f 6e20 696e   for revision in
-00006710: 2072 6576 6973 696f 6e73 292c 2064 623d   revisions), db=
-00006720: 6462 2c20 6375 723d 6375 720a 2020 2020  db, cur=cur.    
-00006730: 2020 2020 2020 2020 290a 2020 2020 2020          ).      
-00006740: 2020 290a 0a20 2020 2020 2020 2069 6620    )..        if 
-00006750: 6e6f 7420 7265 7669 7369 6f6e 735f 6d69  not revisions_mi
-00006760: 7373 696e 673a 0a20 2020 2020 2020 2020  ssing:.         
-00006770: 2020 2072 6574 7572 6e20 7375 6d6d 6172     return summar
-00006780: 790a 0a20 2020 2020 2020 2064 622e 6d6b  y..        db.mk
-00006790: 7465 6d70 5f72 6576 6973 696f 6e28 6375  temp_revision(cu
-000067a0: 7229 0a0a 2020 2020 2020 2020 7265 7669  r)..        revi
-000067b0: 7369 6f6e 735f 6669 6c74 6572 6564 203d  sions_filtered =
-000067c0: 205b 0a20 2020 2020 2020 2020 2020 2072   [.            r
-000067d0: 6576 6973 696f 6e20 666f 7220 7265 7669  evision for revi
-000067e0: 7369 6f6e 2069 6e20 7265 7669 7369 6f6e  sion in revision
-000067f0: 7320 6966 2072 6576 6973 696f 6e2e 6964  s if revision.id
-00006800: 2069 6e20 7265 7669 7369 6f6e 735f 6d69   in revisions_mi
-00006810: 7373 696e 670a 2020 2020 2020 2020 5d0a  ssing.        ].
-00006820: 0a20 2020 2020 2020 2073 656c 662e 6a6f  .        self.jo
-00006830: 7572 6e61 6c5f 7772 6974 6572 2e72 6576  urnal_writer.rev
-00006840: 6973 696f 6e5f 6164 6428 7265 7669 7369  ision_add(revisi
-00006850: 6f6e 735f 6669 6c74 6572 6564 290a 0a20  ons_filtered).. 
-00006860: 2020 2020 2020 2064 625f 7265 7669 7369         db_revisi
-00006870: 6f6e 735f 6669 6c74 6572 6564 203d 206c  ons_filtered = l
-00006880: 6973 7428 6d61 7028 636f 6e76 6572 7465  ist(map(converte
-00006890: 7273 2e72 6576 6973 696f 6e5f 746f 5f64  rs.revision_to_d
-000068a0: 622c 2072 6576 6973 696f 6e73 5f66 696c  b, revisions_fil
-000068b0: 7465 7265 6429 290a 0a20 2020 2020 2020  tered))..       
-000068c0: 2070 6172 656e 7473 5f66 696c 7465 7265   parents_filtere
-000068d0: 643a 204c 6973 745b 4469 6374 5b73 7472  d: List[Dict[str
-000068e0: 2c20 416e 795d 5d20 3d20 5b5d 0a0a 2020  , Any]] = []..  
-000068f0: 2020 2020 2020 7769 7468 2063 6f6e 7665        with conve
-00006900: 7274 5f76 616c 6964 6174 696f 6e5f 6578  rt_validation_ex
-00006910: 6365 7074 696f 6e73 2829 3a0a 2020 2020  ceptions():.    
-00006920: 2020 2020 2020 2020 6462 2e63 6f70 795f          db.copy_
-00006930: 746f 280a 2020 2020 2020 2020 2020 2020  to(.            
-00006940: 2020 2020 6462 5f72 6576 6973 696f 6e73      db_revisions
-00006950: 5f66 696c 7465 7265 642c 0a20 2020 2020  _filtered,.     
-00006960: 2020 2020 2020 2020 2020 2022 746d 705f             "tmp_
-00006970: 7265 7669 7369 6f6e 222c 0a20 2020 2020  revision",.     
-00006980: 2020 2020 2020 2020 2020 2064 622e 7265             db.re
-00006990: 7669 7369 6f6e 5f61 6464 5f63 6f6c 732c  vision_add_cols,
-000069a0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000069b0: 2063 7572 2c0a 2020 2020 2020 2020 2020   cur,.          
-000069c0: 2020 2020 2020 6c61 6d62 6461 2072 6576        lambda rev
-000069d0: 3a20 7061 7265 6e74 735f 6669 6c74 6572  : parents_filter
-000069e0: 6564 2e65 7874 656e 6428 7265 765b 2270  ed.extend(rev["p
-000069f0: 6172 656e 7473 225d 292c 0a20 2020 2020  arents"]),.     
-00006a00: 2020 2020 2020 2029 0a0a 2020 2020 2020         )..      
-00006a10: 2020 2020 2020 6462 2e72 6576 6973 696f        db.revisio
-00006a20: 6e5f 6164 645f 6672 6f6d 5f74 656d 7028  n_add_from_temp(
-00006a30: 6375 7229 0a0a 2020 2020 2020 2020 2020  cur)..          
-00006a40: 2020 6462 2e63 6f70 795f 746f 280a 2020    db.copy_to(.  
-00006a50: 2020 2020 2020 2020 2020 2020 2020 7061                pa
-00006a60: 7265 6e74 735f 6669 6c74 6572 6564 2c0a  rents_filtered,.
-00006a70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006a80: 2272 6576 6973 696f 6e5f 6869 7374 6f72  "revision_histor
-00006a90: 7922 2c0a 2020 2020 2020 2020 2020 2020  y",.            
-00006aa0: 2020 2020 5b22 6964 222c 2022 7061 7265      ["id", "pare
-00006ab0: 6e74 5f69 6422 2c20 2270 6172 656e 745f  nt_id", "parent_
-00006ac0: 7261 6e6b 225d 2c0a 2020 2020 2020 2020  rank"],.        
-00006ad0: 2020 2020 2020 2020 6375 722c 0a20 2020          cur,.   
-00006ae0: 2020 2020 2020 2020 2029 0a0a 2020 2020           )..    
-00006af0: 2020 2020 7265 7475 726e 207b 2272 6576      return {"rev
-00006b00: 6973 696f 6e3a 6164 6422 3a20 6c65 6e28  ision:add": len(
-00006b10: 7265 7669 7369 6f6e 735f 6d69 7373 696e  revisions_missin
-00006b20: 6729 7d0a 0a20 2020 2040 6462 5f74 7261  g)}..    @db_tra
-00006b30: 6e73 6163 7469 6f6e 5f67 656e 6572 6174  nsaction_generat
-00006b40: 6f72 2829 0a20 2020 2064 6566 2072 6576  or().    def rev
-00006b50: 6973 696f 6e5f 6d69 7373 696e 6728 0a20  ision_missing(. 
-00006b60: 2020 2020 2020 2073 656c 662c 2072 6576         self, rev
-00006b70: 6973 696f 6e73 3a20 4c69 7374 5b53 6861  isions: List[Sha
-00006b80: 3147 6974 5d2c 202a 2c20 6462 3a20 4462  1Git], *, db: Db
-00006b90: 2c20 6375 723d 4e6f 6e65 0a20 2020 2029  , cur=None.    )
-00006ba0: 202d 3e20 4974 6572 6162 6c65 5b53 6861   -> Iterable[Sha
-00006bb0: 3147 6974 5d3a 0a20 2020 2020 2020 2069  1Git]:.        i
-00006bc0: 6620 6e6f 7420 7265 7669 7369 6f6e 733a  f not revisions:
-00006bd0: 0a20 2020 2020 2020 2020 2020 2072 6574  .            ret
-00006be0: 7572 6e20 4e6f 6e65 0a0a 2020 2020 2020  urn None..      
-00006bf0: 2020 666f 7220 6f62 6a20 696e 2064 622e    for obj in db.
-00006c00: 7265 7669 7369 6f6e 5f6d 6973 7369 6e67  revision_missing
-00006c10: 5f66 726f 6d5f 6c69 7374 2872 6576 6973  _from_list(revis
-00006c20: 696f 6e73 2c20 6375 7229 3a0a 2020 2020  ions, cur):.    
-00006c30: 2020 2020 2020 2020 7969 656c 6420 6f62          yield ob
-00006c40: 6a5b 305d 0a0a 2020 2020 4064 625f 7472  j[0]..    @db_tr
-00006c50: 616e 7361 6374 696f 6e28 290a 2020 2020  ansaction().    
-00006c60: 6465 6620 7265 7669 7369 6f6e 5f67 6574  def revision_get
-00006c70: 5f70 6172 7469 7469 6f6e 280a 2020 2020  _partition(.    
-00006c80: 2020 2020 7365 6c66 2c0a 2020 2020 2020      self,.      
-00006c90: 2020 7061 7274 6974 696f 6e5f 6964 3a20    partition_id: 
-00006ca0: 696e 742c 0a20 2020 2020 2020 206e 625f  int,.        nb_
-00006cb0: 7061 7274 6974 696f 6e73 3a20 696e 742c  partitions: int,
-00006cc0: 0a20 2020 2020 2020 2070 6167 655f 746f  .        page_to
-00006cd0: 6b65 6e3a 204f 7074 696f 6e61 6c5b 7374  ken: Optional[st
-00006ce0: 725d 203d 204e 6f6e 652c 0a20 2020 2020  r] = None,.     
-00006cf0: 2020 206c 696d 6974 3a20 696e 7420 3d20     limit: int = 
-00006d00: 3130 3030 2c0a 2020 2020 2020 2020 2a2c  1000,.        *,
-00006d10: 0a20 2020 2020 2020 2064 623a 2044 622c  .        db: Db,
-00006d20: 0a20 2020 2020 2020 2063 7572 3d4e 6f6e  .        cur=Non
-00006d30: 652c 0a20 2020 2029 202d 3e20 5061 6765  e,.    ) -> Page
-00006d40: 6452 6573 756c 745b 5265 7669 7369 6f6e  dResult[Revision
-00006d50: 5d3a 0a20 2020 2020 2020 2072 6574 7572  ]:.        retur
-00006d60: 6e20 5f67 6574 5f70 6167 696e 6174 6564  n _get_paginated
-00006d70: 5f73 6861 315f 7061 7274 6974 696f 6e28  _sha1_partition(
-00006d80: 0a20 2020 2020 2020 2020 2020 2063 7572  .            cur
-00006d90: 2c0a 2020 2020 2020 2020 2020 2020 7061  ,.            pa
-00006da0: 7274 6974 696f 6e5f 6964 2c0a 2020 2020  rtition_id,.    
-00006db0: 2020 2020 2020 2020 6e62 5f70 6172 7469          nb_parti
-00006dc0: 7469 6f6e 732c 0a20 2020 2020 2020 2020  tions,.         
-00006dd0: 2020 2070 6167 655f 746f 6b65 6e2c 0a20     page_token,. 
-00006de0: 2020 2020 2020 2020 2020 206c 696d 6974             limit
-00006df0: 2c0a 2020 2020 2020 2020 2020 2020 6462  ,.            db
-00006e00: 2e72 6576 6973 696f 6e5f 6765 745f 7261  .revision_get_ra
-00006e10: 6e67 652c 0a20 2020 2020 2020 2020 2020  nge,.           
-00006e20: 206c 616d 6264 6120 726f 773a 2063 6f6e   lambda row: con
-00006e30: 7665 7274 6572 732e 6462 5f74 6f5f 7265  verters.db_to_re
-00006e40: 7669 7369 6f6e 2864 6963 7428 7a69 7028  vision(dict(zip(
-00006e50: 6462 2e72 6576 6973 696f 6e5f 6765 745f  db.revision_get_
-00006e60: 636f 6c73 2c20 726f 7729 2929 2c0a 2020  cols, row))),.  
-00006e70: 2020 2020 2020 290a 0a20 2020 2040 6462        )..    @db
-00006e80: 5f74 7261 6e73 6163 7469 6f6e 2873 7461  _transaction(sta
-00006e90: 7465 6d65 6e74 5f74 696d 656f 7574 3d32  tement_timeout=2
-00006ea0: 3030 3029 0a20 2020 2064 6566 2072 6576  000).    def rev
-00006eb0: 6973 696f 6e5f 6765 7428 0a20 2020 2020  ision_get(.     
-00006ec0: 2020 2073 656c 662c 0a20 2020 2020 2020     self,.       
-00006ed0: 2072 6576 6973 696f 6e5f 6964 733a 204c   revision_ids: L
-00006ee0: 6973 745b 5368 6131 4769 745d 2c0a 2020  ist[Sha1Git],.  
-00006ef0: 2020 2020 2020 6967 6e6f 7265 5f64 6973        ignore_dis
-00006f00: 706c 6179 6e61 6d65 3a20 626f 6f6c 203d  playname: bool =
-00006f10: 2046 616c 7365 2c0a 2020 2020 2020 2020   False,.        
-00006f20: 2a2c 0a20 2020 2020 2020 2064 623a 2044  *,.        db: D
-00006f30: 622c 0a20 2020 2020 2020 2063 7572 3d4e  b,.        cur=N
-00006f40: 6f6e 652c 0a20 2020 2029 202d 3e20 4c69  one,.    ) -> Li
-00006f50: 7374 5b4f 7074 696f 6e61 6c5b 5265 7669  st[Optional[Revi
-00006f60: 7369 6f6e 5d5d 3a0a 2020 2020 2020 2020  sion]]:.        
-00006f70: 7265 7669 7369 6f6e 7320 3d20 5b5d 0a20  revisions = []. 
-00006f80: 2020 2020 2020 2066 6f72 206c 696e 6520         for line 
-00006f90: 696e 2064 622e 7265 7669 7369 6f6e 5f67  in db.revision_g
-00006fa0: 6574 5f66 726f 6d5f 6c69 7374 2872 6576  et_from_list(rev
-00006fb0: 6973 696f 6e5f 6964 732c 2069 676e 6f72  ision_ids, ignor
-00006fc0: 655f 6469 7370 6c61 796e 616d 652c 2063  e_displayname, c
-00006fd0: 7572 293a 0a20 2020 2020 2020 2020 2020  ur):.           
-00006fe0: 2072 6576 6973 696f 6e20 3d20 636f 6e76   revision = conv
-00006ff0: 6572 7465 7273 2e64 625f 746f 5f6f 7074  erters.db_to_opt
-00007000: 696f 6e61 6c5f 7265 7669 7369 6f6e 280a  ional_revision(.
-00007010: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007020: 6469 6374 287a 6970 2864 622e 7265 7669  dict(zip(db.revi
-00007030: 7369 6f6e 5f67 6574 5f63 6f6c 732c 206c  sion_get_cols, l
-00007040: 696e 6529 290a 2020 2020 2020 2020 2020  ine)).          
-00007050: 2020 290a 2020 2020 2020 2020 2020 2020    ).            
-00007060: 7265 7669 7369 6f6e 732e 6170 7065 6e64  revisions.append
-00007070: 2872 6576 6973 696f 6e29 0a0a 2020 2020  (revision)..    
-00007080: 2020 2020 7265 7475 726e 2072 6576 6973      return revis
-00007090: 696f 6e73 0a0a 2020 2020 4064 625f 7472  ions..    @db_tr
-000070a0: 616e 7361 6374 696f 6e5f 6765 6e65 7261  ansaction_genera
-000070b0: 746f 7228 7374 6174 656d 656e 745f 7469  tor(statement_ti
-000070c0: 6d65 6f75 743d 3230 3030 290a 2020 2020  meout=2000).    
-000070d0: 6465 6620 7265 7669 7369 6f6e 5f6c 6f67  def revision_log
-000070e0: 280a 2020 2020 2020 2020 7365 6c66 2c0a  (.        self,.
-000070f0: 2020 2020 2020 2020 7265 7669 7369 6f6e          revision
-00007100: 733a 204c 6973 745b 5368 6131 4769 745d  s: List[Sha1Git]
-00007110: 2c0a 2020 2020 2020 2020 6967 6e6f 7265  ,.        ignore
-00007120: 5f64 6973 706c 6179 6e61 6d65 3a20 626f  _displayname: bo
-00007130: 6f6c 203d 2046 616c 7365 2c0a 2020 2020  ol = False,.    
-00007140: 2020 2020 6c69 6d69 743a 204f 7074 696f      limit: Optio
-00007150: 6e61 6c5b 696e 745d 203d 204e 6f6e 652c  nal[int] = None,
-00007160: 0a20 2020 2020 2020 202a 2c0a 2020 2020  .        *,.    
-00007170: 2020 2020 6462 3a20 4462 2c0a 2020 2020      db: Db,.    
-00007180: 2020 2020 6375 723d 4e6f 6e65 2c0a 2020      cur=None,.  
-00007190: 2020 2920 2d3e 2049 7465 7261 626c 655b    ) -> Iterable[
-000071a0: 4f70 7469 6f6e 616c 5b44 6963 745b 7374  Optional[Dict[st
-000071b0: 722c 2041 6e79 5d5d 5d3a 0a20 2020 2020  r, Any]]]:.     
-000071c0: 2020 2066 6f72 206c 696e 6520 696e 2064     for line in d
-000071d0: 622e 7265 7669 7369 6f6e 5f6c 6f67 280a  b.revision_log(.
-000071e0: 2020 2020 2020 2020 2020 2020 7265 7669              revi
-000071f0: 7369 6f6e 732c 2069 676e 6f72 655f 6469  sions, ignore_di
-00007200: 7370 6c61 796e 616d 653d 6967 6e6f 7265  splayname=ignore
-00007210: 5f64 6973 706c 6179 6e61 6d65 2c20 6c69  _displayname, li
-00007220: 6d69 743d 6c69 6d69 742c 2063 7572 3d63  mit=limit, cur=c
-00007230: 7572 0a20 2020 2020 2020 2029 3a0a 2020  ur.        ):.  
-00007240: 2020 2020 2020 2020 2020 6461 7461 203d            data =
-00007250: 2063 6f6e 7665 7274 6572 732e 6462 5f74   converters.db_t
-00007260: 6f5f 7265 7669 7369 6f6e 2864 6963 7428  o_revision(dict(
-00007270: 7a69 7028 6462 2e72 6576 6973 696f 6e5f  zip(db.revision_
-00007280: 6765 745f 636f 6c73 2c20 6c69 6e65 2929  get_cols, line))
-00007290: 290a 2020 2020 2020 2020 2020 2020 6966  ).            if
-000072a0: 206e 6f74 2064 6174 613a 0a20 2020 2020   not data:.     
-000072b0: 2020 2020 2020 2020 2020 2079 6965 6c64             yield
-000072c0: 204e 6f6e 650a 2020 2020 2020 2020 2020   None.          
-000072d0: 2020 2020 2020 636f 6e74 696e 7565 0a20        continue. 
-000072e0: 2020 2020 2020 2020 2020 2079 6965 6c64             yield
-000072f0: 2064 6174 612e 746f 5f64 6963 7428 290a   data.to_dict().
-00007300: 0a20 2020 2040 6462 5f74 7261 6e73 6163  .    @db_transac
-00007310: 7469 6f6e 5f67 656e 6572 6174 6f72 2873  tion_generator(s
-00007320: 7461 7465 6d65 6e74 5f74 696d 656f 7574  tatement_timeout
-00007330: 3d32 3030 3029 0a20 2020 2064 6566 2072  =2000).    def r
-00007340: 6576 6973 696f 6e5f 7368 6f72 746c 6f67  evision_shortlog
-00007350: 280a 2020 2020 2020 2020 7365 6c66 2c20  (.        self, 
-00007360: 7265 7669 7369 6f6e 733a 204c 6973 745b  revisions: List[
-00007370: 5368 6131 4769 745d 2c20 6c69 6d69 743a  Sha1Git], limit:
-00007380: 204f 7074 696f 6e61 6c5b 696e 745d 203d   Optional[int] =
-00007390: 204e 6f6e 652c 202a 2c20 6462 3a20 4462   None, *, db: Db
-000073a0: 2c20 6375 723d 4e6f 6e65 0a20 2020 2029  , cur=None.    )
-000073b0: 202d 3e20 4974 6572 6162 6c65 5b4f 7074   -> Iterable[Opt
-000073c0: 696f 6e61 6c5b 5475 706c 655b 5368 6131  ional[Tuple[Sha1
-000073d0: 4769 742c 2054 7570 6c65 5b53 6861 3147  Git, Tuple[Sha1G
-000073e0: 6974 2c20 2e2e 2e5d 5d5d 5d3a 0a20 2020  it, ...]]]]:.   
-000073f0: 2020 2020 2079 6965 6c64 2066 726f 6d20       yield from 
-00007400: 6462 2e72 6576 6973 696f 6e5f 7368 6f72  db.revision_shor
-00007410: 746c 6f67 2872 6576 6973 696f 6e73 2c20  tlog(revisions, 
-00007420: 6c69 6d69 742c 2063 7572 290a 0a20 2020  limit, cur)..   
-00007430: 2040 6462 5f74 7261 6e73 6163 7469 6f6e   @db_transaction
-00007440: 2829 0a20 2020 2064 6566 2072 6576 6973  ().    def revis
-00007450: 696f 6e5f 6765 745f 7261 6e64 6f6d 2873  ion_get_random(s
-00007460: 656c 662c 202a 2c20 6462 3a20 4462 2c20  elf, *, db: Db, 
-00007470: 6375 723d 4e6f 6e65 2920 2d3e 2053 6861  cur=None) -> Sha
-00007480: 3147 6974 3a0a 2020 2020 2020 2020 7265  1Git:.        re
-00007490: 7475 726e 2064 622e 7265 7669 7369 6f6e  turn db.revision
-000074a0: 5f67 6574 5f72 616e 646f 6d28 6375 7229  _get_random(cur)
-000074b0: 0a0a 2020 2020 2323 2323 2323 2323 2323  ..    ##########
-000074c0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-000074d0: 0a20 2020 2023 2045 7874 4944 0a20 2020  .    # ExtID.   
-000074e0: 2023 2323 2323 2323 2323 2323 2323 2323   ###############
-000074f0: 2323 2323 2323 2323 2323 230a 0a20 2020  ###########..   
-00007500: 2040 6462 5f74 7261 6e73 6163 7469 6f6e   @db_transaction
-00007510: 2829 0a20 2020 2064 6566 2065 7874 6964  ().    def extid
-00007520: 5f67 6574 5f66 726f 6d5f 6578 7469 6428  _get_from_extid(
-00007530: 0a20 2020 2020 2020 2073 656c 662c 0a20  .        self,. 
-00007540: 2020 2020 2020 2069 645f 7479 7065 3a20         id_type: 
-00007550: 7374 722c 0a20 2020 2020 2020 2069 6473  str,.        ids
-00007560: 3a20 4c69 7374 5b62 7974 6573 5d2c 0a20  : List[bytes],. 
-00007570: 2020 2020 2020 2076 6572 7369 6f6e 3a20         version: 
-00007580: 4f70 7469 6f6e 616c 5b69 6e74 5d20 3d20  Optional[int] = 
-00007590: 4e6f 6e65 2c0a 2020 2020 2020 2020 2a2c  None,.        *,
-000075a0: 0a20 2020 2020 2020 2064 623a 2044 622c  .        db: Db,
-000075b0: 0a20 2020 2020 2020 2063 7572 3d4e 6f6e  .        cur=Non
-000075c0: 652c 0a20 2020 2029 202d 3e20 4c69 7374  e,.    ) -> List
-000075d0: 5b45 7874 4944 5d3a 0a20 2020 2020 2020  [ExtID]:.       
-000075e0: 2065 7874 6964 7320 3d20 5b5d 0a20 2020   extids = [].   
-000075f0: 2020 2020 2066 6f72 2072 6f77 2069 6e20       for row in 
-00007600: 6462 2e65 7874 6964 5f67 6574 5f66 726f  db.extid_get_fro
-00007610: 6d5f 6578 7469 645f 6c69 7374 2869 645f  m_extid_list(id_
-00007620: 7479 7065 2c20 6964 732c 2076 6572 7369  type, ids, versi
-00007630: 6f6e 3d76 6572 7369 6f6e 2c20 6375 723d  on=version, cur=
-00007640: 6375 7229 3a0a 2020 2020 2020 2020 2020  cur):.          
-00007650: 2020 6966 2072 6f77 5b30 5d20 6973 206e    if row[0] is n
-00007660: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
-00007670: 2020 2020 2020 2020 2065 7874 6964 732e           extids.
-00007680: 6170 7065 6e64 2863 6f6e 7665 7274 6572  append(converter
-00007690: 732e 6462 5f74 6f5f 6578 7469 6428 6469  s.db_to_extid(di
-000076a0: 6374 287a 6970 2864 622e 6578 7469 645f  ct(zip(db.extid_
-000076b0: 636f 6c73 2c20 726f 7729 2929 290a 2020  cols, row)))).  
-000076c0: 2020 2020 2020 7265 7475 726e 2065 7874        return ext
-000076d0: 6964 730a 0a20 2020 2040 6462 5f74 7261  ids..    @db_tra
-000076e0: 6e73 6163 7469 6f6e 2829 0a20 2020 2064  nsaction().    d
-000076f0: 6566 2065 7874 6964 5f67 6574 5f66 726f  ef extid_get_fro
-00007700: 6d5f 7461 7267 6574 280a 2020 2020 2020  m_target(.      
-00007710: 2020 7365 6c66 2c0a 2020 2020 2020 2020    self,.        
-00007720: 7461 7267 6574 5f74 7970 653a 204f 626a  target_type: Obj
-00007730: 6563 7454 7970 652c 0a20 2020 2020 2020  ectType,.       
-00007740: 2069 6473 3a20 4c69 7374 5b53 6861 3147   ids: List[Sha1G
-00007750: 6974 5d2c 0a20 2020 2020 2020 2065 7874  it],.        ext
-00007760: 6964 5f74 7970 653a 204f 7074 696f 6e61  id_type: Optiona
-00007770: 6c5b 7374 725d 203d 204e 6f6e 652c 0a20  l[str] = None,. 
-00007780: 2020 2020 2020 2065 7874 6964 5f76 6572         extid_ver
-00007790: 7369 6f6e 3a20 4f70 7469 6f6e 616c 5b69  sion: Optional[i
-000077a0: 6e74 5d20 3d20 4e6f 6e65 2c0a 2020 2020  nt] = None,.    
-000077b0: 2020 2020 2a2c 0a20 2020 2020 2020 2064      *,.        d
-000077c0: 623a 2044 622c 0a20 2020 2020 2020 2063  b: Db,.        c
-000077d0: 7572 3d4e 6f6e 652c 0a20 2020 2029 202d  ur=None,.    ) -
-000077e0: 3e20 4c69 7374 5b45 7874 4944 5d3a 0a20  > List[ExtID]:. 
-000077f0: 2020 2020 2020 2065 7874 6964 7320 3d20         extids = 
-00007800: 5b5d 0a20 2020 2020 2020 2069 6620 2865  [].        if (e
-00007810: 7874 6964 5f76 6572 7369 6f6e 2069 7320  xtid_version is 
-00007820: 6e6f 7420 4e6f 6e65 2061 6e64 2065 7874  not None and ext
-00007830: 6964 5f74 7970 6520 6973 204e 6f6e 6529  id_type is None)
-00007840: 206f 7220 280a 2020 2020 2020 2020 2020   or (.          
-00007850: 2020 6578 7469 645f 7665 7273 696f 6e20    extid_version 
-00007860: 6973 204e 6f6e 6520 616e 6420 6578 7469  is None and exti
-00007870: 645f 7479 7065 2069 7320 6e6f 7420 4e6f  d_type is not No
-00007880: 6e65 0a20 2020 2020 2020 2029 3a0a 2020  ne.        ):.  
-00007890: 2020 2020 2020 2020 2020 7261 6973 6520            raise 
-000078a0: 5661 6c75 6545 7272 6f72 2822 596f 7520  ValueError("You 
-000078b0: 6d75 7374 2070 726f 7669 6465 2062 6f74  must provide bot
-000078c0: 6820 6578 7469 645f 7479 7065 2061 6e64  h extid_type and
-000078d0: 2065 7874 6964 5f76 6572 7369 6f6e 2229   extid_version")
-000078e0: 0a0a 2020 2020 2020 2020 666f 7220 726f  ..        for ro
-000078f0: 7720 696e 2064 622e 6578 7469 645f 6765  w in db.extid_ge
-00007900: 745f 6672 6f6d 5f73 7768 6964 5f6c 6973  t_from_swhid_lis
-00007910: 7428 0a20 2020 2020 2020 2020 2020 2074  t(.            t
-00007920: 6172 6765 745f 7479 7065 2e76 616c 7565  arget_type.value
-00007930: 2c0a 2020 2020 2020 2020 2020 2020 6964  ,.            id
-00007940: 732c 0a20 2020 2020 2020 2020 2020 2065  s,.            e
-00007950: 7874 6964 5f76 6572 7369 6f6e 3d65 7874  xtid_version=ext
-00007960: 6964 5f76 6572 7369 6f6e 2c0a 2020 2020  id_version,.    
-00007970: 2020 2020 2020 2020 6578 7469 645f 7479          extid_ty
-00007980: 7065 3d65 7874 6964 5f74 7970 652c 0a20  pe=extid_type,. 
-00007990: 2020 2020 2020 2020 2020 2063 7572 3d63             cur=c
-000079a0: 7572 2c0a 2020 2020 2020 2020 293a 0a20  ur,.        ):. 
-000079b0: 2020 2020 2020 2020 2020 2069 6620 726f             if ro
-000079c0: 775b 305d 2069 7320 6e6f 7420 4e6f 6e65  w[0] is not None
-000079d0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-000079e0: 2020 6578 7469 6473 2e61 7070 656e 6428    extids.append(
-000079f0: 636f 6e76 6572 7465 7273 2e64 625f 746f  converters.db_to
-00007a00: 5f65 7874 6964 2864 6963 7428 7a69 7028  _extid(dict(zip(
-00007a10: 6462 2e65 7874 6964 5f63 6f6c 732c 2072  db.extid_cols, r
-00007a20: 6f77 2929 2929 0a20 2020 2020 2020 2072  ow)))).        r
-00007a30: 6574 7572 6e20 6578 7469 6473 0a0a 2020  eturn extids..  
-00007a40: 2020 4064 625f 7472 616e 7361 6374 696f    @db_transactio
-00007a50: 6e28 290a 2020 2020 6465 6620 6578 7469  n().    def exti
-00007a60: 645f 6164 6428 7365 6c66 2c20 6964 733a  d_add(self, ids:
-00007a70: 204c 6973 745b 4578 7449 445d 2c20 2a2c   List[ExtID], *,
-00007a80: 2064 623a 2044 622c 2063 7572 3d4e 6f6e   db: Db, cur=Non
-00007a90: 6529 202d 3e20 4469 6374 5b73 7472 2c20  e) -> Dict[str, 
-00007aa0: 696e 745d 3a0a 2020 2020 2020 2020 6578  int]:.        ex
-00007ab0: 7469 6420 3d20 5b0a 2020 2020 2020 2020  tid = [.        
-00007ac0: 2020 2020 7b0a 2020 2020 2020 2020 2020      {.          
-00007ad0: 2020 2020 2020 2265 7874 6964 223a 2065        "extid": e
-00007ae0: 7874 6964 2e65 7874 6964 2c0a 2020 2020  xtid.extid,.    
-00007af0: 2020 2020 2020 2020 2020 2020 2265 7874              "ext
-00007b00: 6964 5f74 7970 6522 3a20 6578 7469 642e  id_type": extid.
-00007b10: 6578 7469 645f 7479 7065 2c0a 2020 2020  extid_type,.    
-00007b20: 2020 2020 2020 2020 2020 2020 2265 7874              "ext
-00007b30: 6964 5f76 6572 7369 6f6e 223a 2067 6574  id_version": get
-00007b40: 6174 7472 2865 7874 6964 2c20 2265 7874  attr(extid, "ext
-00007b50: 6964 5f76 6572 7369 6f6e 222c 2030 292c  id_version", 0),
-00007b60: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00007b70: 2022 7461 7267 6574 223a 2065 7874 6964   "target": extid
-00007b80: 2e74 6172 6765 742e 6f62 6a65 6374 5f69  .target.object_i
-00007b90: 642c 0a20 2020 2020 2020 2020 2020 2020  d,.             
-00007ba0: 2020 2022 7461 7267 6574 5f74 7970 6522     "target_type"
-00007bb0: 3a20 6578 7469 642e 7461 7267 6574 2e6f  : extid.target.o
-00007bc0: 626a 6563 745f 7479 7065 2e6e 616d 652e  bject_type.name.
-00007bd0: 6c6f 7765 7228 292c 2020 2320 6172 6768  lower(),  # argh
-00007be0: 680a 2020 2020 2020 2020 2020 2020 7d0a  h.            }.
-00007bf0: 2020 2020 2020 2020 2020 2020 666f 7220              for 
-00007c00: 6578 7469 6420 696e 2069 6473 0a20 2020  extid in ids.   
-00007c10: 2020 2020 205d 0a20 2020 2020 2020 2064       ].        d
-00007c20: 622e 6d6b 7465 6d70 2822 6578 7469 6422  b.mktemp("extid"
-00007c30: 2c20 6375 7229 0a0a 2020 2020 2020 2020  , cur)..        
-00007c40: 7365 6c66 2e6a 6f75 726e 616c 5f77 7269  self.journal_wri
-00007c50: 7465 722e 6578 7469 645f 6164 6428 6964  ter.extid_add(id
-00007c60: 7329 0a0a 2020 2020 2020 2020 6462 2e63  s)..        db.c
-00007c70: 6f70 795f 746f 2865 7874 6964 2c20 2274  opy_to(extid, "t
-00007c80: 6d70 5f65 7874 6964 222c 2064 622e 6578  mp_extid", db.ex
-00007c90: 7469 645f 636f 6c73 2c20 6375 7229 0a0a  tid_cols, cur)..
-00007ca0: 2020 2020 2020 2020 2320 6d6f 7665 206d          # move m
-00007cb0: 6574 6164 6174 6120 696e 2070 6c61 6365  etadata in place
-00007cc0: 0a20 2020 2020 2020 2064 622e 6578 7469  .        db.exti
-00007cd0: 645f 6164 645f 6672 6f6d 5f74 656d 7028  d_add_from_temp(
-00007ce0: 6375 7229 0a0a 2020 2020 2020 2020 7265  cur)..        re
-00007cf0: 7475 726e 207b 2265 7874 6964 3a61 6464  turn {"extid:add
-00007d00: 223a 206c 656e 2865 7874 6964 297d 0a0a  ": len(extid)}..
-00007d10: 2020 2020 2323 2323 2323 2323 2323 2323      ############
-00007d20: 2323 2323 2323 2323 2323 2323 2323 0a20  ##############. 
-00007d30: 2020 2023 2052 656c 6561 7365 0a20 2020     # Release.   
-00007d40: 2023 2323 2323 2323 2323 2323 2323 2323   ###############
-00007d50: 2323 2323 2323 2323 2323 230a 0a20 2020  ###########..   
-00007d60: 2040 6462 5f74 7261 6e73 6163 7469 6f6e   @db_transaction
-00007d70: 2829 0a20 2020 2064 6566 2072 656c 6561  ().    def relea
-00007d80: 7365 5f61 6464 280a 2020 2020 2020 2020  se_add(.        
-00007d90: 7365 6c66 2c20 7265 6c65 6173 6573 3a20  self, releases: 
-00007da0: 4c69 7374 5b52 656c 6561 7365 5d2c 202a  List[Release], *
-00007db0: 2c20 6462 3a20 4462 2c20 6375 723d 4e6f  , db: Db, cur=No
-00007dc0: 6e65 0a20 2020 2029 202d 3e20 4469 6374  ne.    ) -> Dict
-00007dd0: 5b73 7472 2c20 696e 745d 3a0a 2020 2020  [str, int]:.    
-00007de0: 2020 2020 7375 6d6d 6172 7920 3d20 7b22      summary = {"
-00007df0: 7265 6c65 6173 653a 6164 6422 3a20 307d  release:add": 0}
-00007e00: 0a0a 2020 2020 2020 2020 7265 6c65 6173  ..        releas
-00007e10: 655f 6964 7320 3d20 7365 7428 7265 6c65  e_ids = set(rele
-00007e20: 6173 652e 6964 2066 6f72 2072 656c 6561  ase.id for relea
-00007e30: 7365 2069 6e20 7265 6c65 6173 6573 290a  se in releases).
-00007e40: 2020 2020 2020 2020 7265 6c65 6173 6573          releases
-00007e50: 5f6d 6973 7369 6e67 203d 2073 6574 2873  _missing = set(s
-00007e60: 656c 662e 7265 6c65 6173 655f 6d69 7373  elf.release_miss
-00007e70: 696e 6728 7265 6c65 6173 655f 6964 732c  ing(release_ids,
-00007e80: 2064 623d 6462 2c20 6375 723d 6375 7229   db=db, cur=cur)
-00007e90: 290a 0a20 2020 2020 2020 2069 6620 6e6f  )..        if no
-00007ea0: 7420 7265 6c65 6173 6573 5f6d 6973 7369  t releases_missi
-00007eb0: 6e67 3a0a 2020 2020 2020 2020 2020 2020  ng:.            
-00007ec0: 7265 7475 726e 2073 756d 6d61 7279 0a0a  return summary..
-00007ed0: 2020 2020 2020 2020 6462 2e6d 6b74 656d          db.mktem
-00007ee0: 705f 7265 6c65 6173 6528 6375 7229 0a0a  p_release(cur)..
-00007ef0: 2020 2020 2020 2020 7265 6c65 6173 6573          releases
-00007f00: 5f66 696c 7465 7265 6420 3d20 5b0a 2020  _filtered = [.  
-00007f10: 2020 2020 2020 2020 2020 7265 6c65 6173            releas
-00007f20: 6520 666f 7220 7265 6c65 6173 6520 696e  e for release in
-00007f30: 2072 656c 6561 7365 7320 6966 2072 656c   releases if rel
-00007f40: 6561 7365 2e69 6420 696e 2072 656c 6561  ease.id in relea
-00007f50: 7365 735f 6d69 7373 696e 670a 2020 2020  ses_missing.    
-00007f60: 2020 2020 5d0a 0a20 2020 2020 2020 2073      ]..        s
-00007f70: 656c 662e 6a6f 7572 6e61 6c5f 7772 6974  elf.journal_writ
-00007f80: 6572 2e72 656c 6561 7365 5f61 6464 2872  er.release_add(r
-00007f90: 656c 6561 7365 735f 6669 6c74 6572 6564  eleases_filtered
-00007fa0: 290a 0a20 2020 2020 2020 2064 625f 7265  )..        db_re
-00007fb0: 6c65 6173 6573 5f66 696c 7465 7265 6420  leases_filtered 
-00007fc0: 3d20 6c69 7374 286d 6170 2863 6f6e 7665  = list(map(conve
-00007fd0: 7274 6572 732e 7265 6c65 6173 655f 746f  rters.release_to
-00007fe0: 5f64 622c 2072 656c 6561 7365 735f 6669  _db, releases_fi
-00007ff0: 6c74 6572 6564 2929 0a0a 2020 2020 2020  ltered))..      
-00008000: 2020 7769 7468 2063 6f6e 7665 7274 5f76    with convert_v
-00008010: 616c 6964 6174 696f 6e5f 6578 6365 7074  alidation_except
-00008020: 696f 6e73 2829 3a0a 2020 2020 2020 2020  ions():.        
-00008030: 2020 2020 6462 2e63 6f70 795f 746f 2864      db.copy_to(d
-00008040: 625f 7265 6c65 6173 6573 5f66 696c 7465  b_releases_filte
-00008050: 7265 642c 2022 746d 705f 7265 6c65 6173  red, "tmp_releas
-00008060: 6522 2c20 6462 2e72 656c 6561 7365 5f61  e", db.release_a
-00008070: 6464 5f63 6f6c 732c 2063 7572 290a 0a20  dd_cols, cur).. 
-00008080: 2020 2020 2020 2020 2020 2064 622e 7265             db.re
-00008090: 6c65 6173 655f 6164 645f 6672 6f6d 5f74  lease_add_from_t
-000080a0: 656d 7028 6375 7229 0a0a 2020 2020 2020  emp(cur)..      
-000080b0: 2020 7265 7475 726e 207b 2272 656c 6561    return {"relea
-000080c0: 7365 3a61 6464 223a 206c 656e 2872 656c  se:add": len(rel
-000080d0: 6561 7365 735f 6d69 7373 696e 6729 7d0a  eases_missing)}.
-000080e0: 0a20 2020 2040 6462 5f74 7261 6e73 6163  .    @db_transac
-000080f0: 7469 6f6e 5f67 656e 6572 6174 6f72 2829  tion_generator()
-00008100: 0a20 2020 2064 6566 2072 656c 6561 7365  .    def release
-00008110: 5f6d 6973 7369 6e67 280a 2020 2020 2020  _missing(.      
-00008120: 2020 7365 6c66 2c20 7265 6c65 6173 6573    self, releases
-00008130: 3a20 4c69 7374 5b53 6861 3147 6974 5d2c  : List[Sha1Git],
-00008140: 202a 2c20 6462 3a20 4462 2c20 6375 723d   *, db: Db, cur=
-00008150: 4e6f 6e65 0a20 2020 2029 202d 3e20 4974  None.    ) -> It
-00008160: 6572 6162 6c65 5b53 6861 3147 6974 5d3a  erable[Sha1Git]:
-00008170: 0a20 2020 2020 2020 2069 6620 6e6f 7420  .        if not 
-00008180: 7265 6c65 6173 6573 3a0a 2020 2020 2020  releases:.      
-00008190: 2020 2020 2020 7265 7475 726e 0a0a 2020        return..  
-000081a0: 2020 2020 2020 666f 7220 6f62 6a20 696e        for obj in
-000081b0: 2064 622e 7265 6c65 6173 655f 6d69 7373   db.release_miss
-000081c0: 696e 675f 6672 6f6d 5f6c 6973 7428 7265  ing_from_list(re
-000081d0: 6c65 6173 6573 2c20 6375 7229 3a0a 2020  leases, cur):.  
-000081e0: 2020 2020 2020 2020 2020 7969 656c 6420            yield 
-000081f0: 6f62 6a5b 305d 0a0a 2020 2020 4064 625f  obj[0]..    @db_
-00008200: 7472 616e 7361 6374 696f 6e28 7374 6174  transaction(stat
-00008210: 656d 656e 745f 7469 6d65 6f75 743d 3130  ement_timeout=10
-00008220: 3030 290a 2020 2020 6465 6620 7265 6c65  00).    def rele
-00008230: 6173 655f 6765 7428 0a20 2020 2020 2020  ase_get(.       
-00008240: 2073 656c 662c 0a20 2020 2020 2020 2072   self,.        r
-00008250: 656c 6561 7365 733a 204c 6973 745b 5368  eleases: List[Sh
-00008260: 6131 4769 745d 2c0a 2020 2020 2020 2020  a1Git],.        
-00008270: 6967 6e6f 7265 5f64 6973 706c 6179 6e61  ignore_displayna
-00008280: 6d65 3a20 626f 6f6c 203d 2046 616c 7365  me: bool = False
-00008290: 2c0a 2020 2020 2020 2020 2a2c 0a20 2020  ,.        *,.   
-000082a0: 2020 2020 2064 623a 2044 622c 0a20 2020       db: Db,.   
-000082b0: 2020 2020 2063 7572 3d4e 6f6e 652c 0a20       cur=None,. 
-000082c0: 2020 2029 202d 3e20 4c69 7374 5b4f 7074     ) -> List[Opt
-000082d0: 696f 6e61 6c5b 5265 6c65 6173 655d 5d3a  ional[Release]]:
-000082e0: 0a20 2020 2020 2020 2072 656c 7320 3d20  .        rels = 
-000082f0: 5b5d 0a20 2020 2020 2020 2066 6f72 2072  [].        for r
-00008300: 656c 6561 7365 2069 6e20 6462 2e72 656c  elease in db.rel
-00008310: 6561 7365 5f67 6574 5f66 726f 6d5f 6c69  ease_get_from_li
-00008320: 7374 2872 656c 6561 7365 732c 2069 676e  st(releases, ign
-00008330: 6f72 655f 6469 7370 6c61 796e 616d 652c  ore_displayname,
-00008340: 2063 7572 293a 0a20 2020 2020 2020 2020   cur):.         
-00008350: 2020 2072 656c 203d 2063 6f6e 7665 7274     rel = convert
-00008360: 6572 732e 6462 5f74 6f5f 6f70 7469 6f6e  ers.db_to_option
-00008370: 616c 5f72 656c 6561 7365 280a 2020 2020  al_release(.    
-00008380: 2020 2020 2020 2020 2020 2020 6469 6374              dict
-00008390: 287a 6970 2864 622e 7265 6c65 6173 655f  (zip(db.release_
-000083a0: 6765 745f 636f 6c73 2c20 7265 6c65 6173  get_cols, releas
-000083b0: 6529 290a 2020 2020 2020 2020 2020 2020  e)).            
-000083c0: 290a 2020 2020 2020 2020 2020 2020 7265  ).            re
-000083d0: 6c73 2e61 7070 656e 6428 7265 6c29 0a20  ls.append(rel). 
-000083e0: 2020 2020 2020 2072 6574 7572 6e20 7265         return re
-000083f0: 6c73 0a0a 2020 2020 4064 625f 7472 616e  ls..    @db_tran
-00008400: 7361 6374 696f 6e28 290a 2020 2020 6465  saction().    de
-00008410: 6620 7265 6c65 6173 655f 6765 745f 7061  f release_get_pa
-00008420: 7274 6974 696f 6e28 0a20 2020 2020 2020  rtition(.       
-00008430: 2073 656c 662c 0a20 2020 2020 2020 2070   self,.        p
-00008440: 6172 7469 7469 6f6e 5f69 643a 2069 6e74  artition_id: int
-00008450: 2c0a 2020 2020 2020 2020 6e62 5f70 6172  ,.        nb_par
-00008460: 7469 7469 6f6e 733a 2069 6e74 2c0a 2020  titions: int,.  
-00008470: 2020 2020 2020 7061 6765 5f74 6f6b 656e        page_token
-00008480: 3a20 4f70 7469 6f6e 616c 5b73 7472 5d20  : Optional[str] 
-00008490: 3d20 4e6f 6e65 2c0a 2020 2020 2020 2020  = None,.        
-000084a0: 6c69 6d69 743a 2069 6e74 203d 2031 3030  limit: int = 100
-000084b0: 302c 0a20 2020 2020 2020 202a 2c0a 2020  0,.        *,.  
-000084c0: 2020 2020 2020 6462 3a20 4462 2c0a 2020        db: Db,.  
-000084d0: 2020 2020 2020 6375 723d 4e6f 6e65 2c0a        cur=None,.
-000084e0: 2020 2020 2920 2d3e 2050 6167 6564 5265      ) -> PagedRe
-000084f0: 7375 6c74 5b52 656c 6561 7365 5d3a 0a20  sult[Release]:. 
-00008500: 2020 2020 2020 2072 6574 7572 6e20 5f67         return _g
-00008510: 6574 5f70 6167 696e 6174 6564 5f73 6861  et_paginated_sha
-00008520: 315f 7061 7274 6974 696f 6e28 0a20 2020  1_partition(.   
-00008530: 2020 2020 2020 2020 2063 7572 2c0a 2020           cur,.  
-00008540: 2020 2020 2020 2020 2020 7061 7274 6974            partit
-00008550: 696f 6e5f 6964 2c0a 2020 2020 2020 2020  ion_id,.        
-00008560: 2020 2020 6e62 5f70 6172 7469 7469 6f6e      nb_partition
-00008570: 732c 0a20 2020 2020 2020 2020 2020 2070  s,.            p
-00008580: 6167 655f 746f 6b65 6e2c 0a20 2020 2020  age_token,.     
-00008590: 2020 2020 2020 206c 696d 6974 2c0a 2020         limit,.  
-000085a0: 2020 2020 2020 2020 2020 6462 2e72 656c            db.rel
-000085b0: 6561 7365 5f67 6574 5f72 616e 6765 2c0a  ease_get_range,.
-000085c0: 2020 2020 2020 2020 2020 2020 6c61 6d62              lamb
-000085d0: 6461 2072 6f77 3a20 636f 6e76 6572 7465  da row: converte
-000085e0: 7273 2e64 625f 746f 5f72 656c 6561 7365  rs.db_to_release
-000085f0: 2864 6963 7428 7a69 7028 6462 2e72 656c  (dict(zip(db.rel
-00008600: 6561 7365 5f67 6574 5f63 6f6c 732c 2072  ease_get_cols, r
-00008610: 6f77 2929 292c 0a20 2020 2020 2020 2029  ow))),.        )
-00008620: 0a0a 2020 2020 4064 625f 7472 616e 7361  ..    @db_transa
-00008630: 6374 696f 6e28 290a 2020 2020 6465 6620  ction().    def 
-00008640: 7265 6c65 6173 655f 6765 745f 7261 6e64  release_get_rand
-00008650: 6f6d 2873 656c 662c 202a 2c20 6462 3a20  om(self, *, db: 
-00008660: 4462 2c20 6375 723d 4e6f 6e65 2920 2d3e  Db, cur=None) ->
-00008670: 2053 6861 3147 6974 3a0a 2020 2020 2020   Sha1Git:.      
-00008680: 2020 7265 7475 726e 2064 622e 7265 6c65    return db.rele
-00008690: 6173 655f 6765 745f 7261 6e64 6f6d 2863  ase_get_random(c
-000086a0: 7572 290a 0a20 2020 2023 2323 2323 2323  ur)..    #######
-000086b0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-000086c0: 2323 230a 2020 2020 2320 536e 6170 7368  ###.    # Snapsh
-000086d0: 6f74 0a20 2020 2023 2323 2323 2323 2323  ot.    #########
-000086e0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-000086f0: 230a 0a20 2020 2040 6462 5f74 7261 6e73  #..    @db_trans
-00008700: 6163 7469 6f6e 2829 0a20 2020 2064 6566  action().    def
-00008710: 2073 6e61 7073 686f 745f 6164 6428 0a20   snapshot_add(. 
-00008720: 2020 2020 2020 2073 656c 662c 2073 6e61         self, sna
-00008730: 7073 686f 7473 3a20 4c69 7374 5b53 6e61  pshots: List[Sna
-00008740: 7073 686f 745d 2c20 2a2c 2064 623a 2044  pshot], *, db: D
-00008750: 622c 2063 7572 3d4e 6f6e 650a 2020 2020  b, cur=None.    
-00008760: 2920 2d3e 2044 6963 745b 7374 722c 2069  ) -> Dict[str, i
-00008770: 6e74 5d3a 0a20 2020 2020 2020 2063 7265  nt]:.        cre
-00008780: 6174 6564 5f74 656d 705f 7461 626c 6520  ated_temp_table 
-00008790: 3d20 4661 6c73 650a 0a20 2020 2020 2020  = False..       
-000087a0: 2063 6f75 6e74 203d 2030 0a20 2020 2020   count = 0.     
-000087b0: 2020 2066 6f72 2073 6e61 7073 686f 7420     for snapshot 
-000087c0: 696e 2073 6e61 7073 686f 7473 3a0a 2020  in snapshots:.  
-000087d0: 2020 2020 2020 2020 2020 6966 206e 6f74            if not
-000087e0: 2064 622e 736e 6170 7368 6f74 5f65 7869   db.snapshot_exi
-000087f0: 7374 7328 736e 6170 7368 6f74 2e69 642c  sts(snapshot.id,
-00008800: 2063 7572 293a 0a20 2020 2020 2020 2020   cur):.         
-00008810: 2020 2020 2020 2069 6620 6e6f 7420 6372         if not cr
-00008820: 6561 7465 645f 7465 6d70 5f74 6162 6c65  eated_temp_table
-00008830: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-00008840: 2020 2020 2020 6462 2e6d 6b74 656d 705f        db.mktemp_
-00008850: 736e 6170 7368 6f74 5f62 7261 6e63 6828  snapshot_branch(
-00008860: 6375 7229 0a20 2020 2020 2020 2020 2020  cur).           
-00008870: 2020 2020 2020 2020 2063 7265 6174 6564           created
-00008880: 5f74 656d 705f 7461 626c 6520 3d20 5472  _temp_table = Tr
-00008890: 7565 0a0a 2020 2020 2020 2020 2020 2020  ue..            
-000088a0: 2020 2020 7769 7468 2063 6f6e 7665 7274      with convert
-000088b0: 5f76 616c 6964 6174 696f 6e5f 6578 6365  _validation_exce
-000088c0: 7074 696f 6e73 2829 3a0a 2020 2020 2020  ptions():.      
-000088d0: 2020 2020 2020 2020 2020 2020 2020 6462                db
-000088e0: 2e63 6f70 795f 746f 280a 2020 2020 2020  .copy_to(.      
-000088f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008900: 2020 280a 2020 2020 2020 2020 2020 2020    (.            
-00008910: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008920: 7b0a 2020 2020 2020 2020 2020 2020 2020  {.              
-00008930: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008940: 2020 226e 616d 6522 3a20 6e61 6d65 2c0a    "name": name,.
-00008950: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003320: 2073 656c 662e 636f 6e74 656e 745f 6d69   self.content_mi
+00003330: 7373 696e 6728 0a20 2020 2020 2020 2020  ssing(.         
+00003340: 2020 2020 2020 2020 2020 2020 2020 205b                 [
+00003350: 632e 746f 5f64 6963 7428 2920 666f 7220  c.to_dict() for 
+00003360: 6320 696e 2063 6f6e 7465 6e74 735d 2c0a  c in contents],.
+00003370: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003380: 2020 2020 2020 2020 6b65 795f 6861 7368          key_hash
+00003390: 3d22 7368 6131 5f67 6974 222c 0a20 2020  ="sha1_git",.   
+000033a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000033b0: 2020 2020 2064 623d 6462 2c0a 2020 2020       db=db,.    
+000033c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000033d0: 2020 2020 6375 723d 6375 722c 0a20 2020      cur=cur,.   
+000033e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000033f0: 2029 0a20 2020 2020 2020 2020 2020 2020   ).             
+00003400: 2020 2029 0a20 2020 2020 2020 2020 2020     ).           
+00003410: 2020 2020 2063 6f6e 7465 6e74 7320 3d20       contents = 
+00003420: 5b63 2066 6f72 2063 2069 6e20 636f 6e74  [c for c in cont
+00003430: 656e 7473 2069 6620 632e 7368 6131 5f67  ents if c.sha1_g
+00003440: 6974 2069 6e20 6d69 7373 696e 675d 0a0a  it in missing]..
+00003450: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003460: 7365 6c66 2e6a 6f75 726e 616c 5f77 7269  self.journal_wri
+00003470: 7465 722e 636f 6e74 656e 745f 6164 6428  ter.content_add(
+00003480: 636f 6e74 656e 7473 290a 2020 2020 2020  contents).      
+00003490: 2020 2020 2020 2020 2020 7365 6c66 2e5f            self._
+000034a0: 636f 6e74 656e 745f 6164 645f 6d65 7461  content_add_meta
+000034b0: 6461 7461 2864 622c 2063 7572 2c20 636f  data(db, cur, co
+000034c0: 6e74 656e 7473 290a 0a20 2020 2020 2020  ntents)..       
+000034d0: 2072 6574 7572 6e20 7b0a 2020 2020 2020   return {.      
+000034e0: 2020 2020 2020 2263 6f6e 7465 6e74 3a61        "content:a
+000034f0: 6464 223a 206c 656e 2863 6f6e 7465 6e74  dd": len(content
+00003500: 7329 2c0a 2020 2020 2020 2020 2020 2020  s),.            
+00003510: 2263 6f6e 7465 6e74 3a61 6464 3a62 7974  "content:add:byt
+00003520: 6573 223a 206f 626a 7374 6f72 6167 655f  es": objstorage_
+00003530: 7375 6d6d 6172 795b 2263 6f6e 7465 6e74  summary["content
+00003540: 3a61 6464 3a62 7974 6573 225d 2c0a 2020  :add:bytes"],.  
+00003550: 2020 2020 2020 7d0a 0a20 2020 2040 6462        }..    @db
+00003560: 5f74 7261 6e73 6163 7469 6f6e 2829 0a20  _transaction(). 
+00003570: 2020 2064 6566 2063 6f6e 7465 6e74 5f75     def content_u
+00003580: 7064 6174 6528 0a20 2020 2020 2020 2073  pdate(.        s
+00003590: 656c 662c 2063 6f6e 7465 6e74 733a 204c  elf, contents: L
+000035a0: 6973 745b 4469 6374 5b73 7472 2c20 416e  ist[Dict[str, An
+000035b0: 795d 5d2c 206b 6579 733a 204c 6973 745b  y]], keys: List[
+000035c0: 7374 725d 203d 205b 5d2c 202a 2c20 6462  str] = [], *, db
+000035d0: 3a20 4462 2c20 6375 723d 4e6f 6e65 0a20  : Db, cur=None. 
+000035e0: 2020 2029 202d 3e20 4e6f 6e65 3a0a 2020     ) -> None:.  
+000035f0: 2020 2020 2020 2320 544f 444f 3a20 4164        # TODO: Ad
+00003600: 6420 6120 6368 6563 6b20 6f6e 2069 6e70  d a check on inp
+00003610: 7574 206b 6579 732e 2048 6f77 2074 6f20  ut keys. How to 
+00003620: 7072 6f70 6572 6c79 2069 6d70 6c65 6d65  properly impleme
+00003630: 6e74 0a20 2020 2020 2020 2023 2074 6869  nt.        # thi
+00003640: 733f 2057 6520 646f 6e27 7420 6b6e 6f77  s? We don't know
+00003650: 2079 6574 2074 6865 206e 6577 2063 6f6c   yet the new col
+00003660: 756d 6e73 2e0a 2020 2020 2020 2020 7365  umns..        se
+00003670: 6c66 2e6a 6f75 726e 616c 5f77 7269 7465  lf.journal_write
+00003680: 722e 636f 6e74 656e 745f 7570 6461 7465  r.content_update
+00003690: 2863 6f6e 7465 6e74 7329 0a0a 2020 2020  (contents)..    
+000036a0: 2020 2020 6462 2e6d 6b74 656d 7028 2263      db.mktemp("c
+000036b0: 6f6e 7465 6e74 222c 2063 7572 290a 2020  ontent", cur).  
+000036c0: 2020 2020 2020 7365 6c65 6374 5f6b 6579        select_key
+000036d0: 7320 3d20 6c69 7374 2873 6574 2864 622e  s = list(set(db.
+000036e0: 636f 6e74 656e 745f 6765 745f 6d65 7461  content_get_meta
+000036f0: 6461 7461 5f6b 6579 7329 2e75 6e69 6f6e  data_keys).union
+00003700: 2873 6574 286b 6579 7329 2929 0a20 2020  (set(keys))).   
+00003710: 2020 2020 2077 6974 6820 636f 6e76 6572       with conver
+00003720: 745f 7661 6c69 6461 7469 6f6e 5f65 7863  t_validation_exc
+00003730: 6570 7469 6f6e 7328 293a 0a20 2020 2020  eptions():.     
+00003740: 2020 2020 2020 2064 622e 636f 7079 5f74         db.copy_t
+00003750: 6f28 636f 6e74 656e 7473 2c20 2274 6d70  o(contents, "tmp
+00003760: 5f63 6f6e 7465 6e74 222c 2073 656c 6563  _content", selec
+00003770: 745f 6b65 7973 2c20 6375 7229 0a20 2020  t_keys, cur).   
+00003780: 2020 2020 2020 2020 2064 622e 636f 6e74           db.cont
+00003790: 656e 745f 7570 6461 7465 5f66 726f 6d5f  ent_update_from_
+000037a0: 7465 6d70 286b 6579 735f 746f 5f75 7064  temp(keys_to_upd
+000037b0: 6174 653d 6b65 7973 2c20 6375 723d 6375  ate=keys, cur=cu
+000037c0: 7229 0a0a 2020 2020 4064 625f 7472 616e  r)..    @db_tran
+000037d0: 7361 6374 696f 6e28 290a 2020 2020 6465  saction().    de
+000037e0: 6620 636f 6e74 656e 745f 6164 645f 6d65  f content_add_me
+000037f0: 7461 6461 7461 280a 2020 2020 2020 2020  tadata(.        
+00003800: 7365 6c66 2c20 636f 6e74 656e 743a 204c  self, content: L
+00003810: 6973 745b 436f 6e74 656e 745d 2c20 2a2c  ist[Content], *,
+00003820: 2064 623a 2044 622c 2063 7572 3d4e 6f6e   db: Db, cur=Non
+00003830: 650a 2020 2020 2920 2d3e 2044 6963 745b  e.    ) -> Dict[
+00003840: 7374 722c 2069 6e74 5d3a 0a20 2020 2020  str, int]:.     
+00003850: 2020 206d 6973 7369 6e67 203d 2073 6574     missing = set
+00003860: 280a 2020 2020 2020 2020 2020 2020 7365  (.            se
+00003870: 6c66 2e63 6f6e 7465 6e74 5f6d 6973 7369  lf.content_missi
+00003880: 6e67 280a 2020 2020 2020 2020 2020 2020  ng(.            
+00003890: 2020 2020 5b63 2e74 6f5f 6469 6374 2829      [c.to_dict()
+000038a0: 2066 6f72 2063 2069 6e20 636f 6e74 656e   for c in conten
+000038b0: 745d 2c0a 2020 2020 2020 2020 2020 2020  t],.            
+000038c0: 2020 2020 6b65 795f 6861 7368 3d22 7368      key_hash="sh
+000038d0: 6131 5f67 6974 222c 0a20 2020 2020 2020  a1_git",.       
+000038e0: 2020 2020 2020 2020 2064 623d 6462 2c0a           db=db,.
+000038f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003900: 6375 723d 6375 722c 0a20 2020 2020 2020  cur=cur,.       
+00003910: 2020 2020 2029 0a20 2020 2020 2020 2029       ).        )
+00003920: 0a20 2020 2020 2020 2063 6f6e 7465 6e74  .        content
+00003930: 7320 3d20 5b63 2066 6f72 2063 2069 6e20  s = [c for c in 
+00003940: 636f 6e74 656e 7420 6966 2063 2e73 6861  content if c.sha
+00003950: 315f 6769 7420 696e 206d 6973 7369 6e67  1_git in missing
+00003960: 5d0a 0a20 2020 2020 2020 2073 656c 662e  ]..        self.
+00003970: 6a6f 7572 6e61 6c5f 7772 6974 6572 2e63  journal_writer.c
+00003980: 6f6e 7465 6e74 5f61 6464 5f6d 6574 6164  ontent_add_metad
+00003990: 6174 6128 636f 6e74 656e 7473 290a 2020  ata(contents).  
+000039a0: 2020 2020 2020 7365 6c66 2e5f 636f 6e74        self._cont
+000039b0: 656e 745f 6164 645f 6d65 7461 6461 7461  ent_add_metadata
+000039c0: 2864 622c 2063 7572 2c20 636f 6e74 656e  (db, cur, conten
+000039d0: 7473 290a 0a20 2020 2020 2020 2072 6574  ts)..        ret
+000039e0: 7572 6e20 7b0a 2020 2020 2020 2020 2020  urn {.          
+000039f0: 2020 2263 6f6e 7465 6e74 3a61 6464 223a    "content:add":
+00003a00: 206c 656e 2863 6f6e 7465 6e74 7329 2c0a   len(contents),.
+00003a10: 2020 2020 2020 2020 7d0a 0a20 2020 2064          }..    d
+00003a20: 6566 2063 6f6e 7465 6e74 5f67 6574 5f64  ef content_get_d
+00003a30: 6174 6128 7365 6c66 2c20 636f 6e74 656e  ata(self, conten
+00003a40: 743a 2055 6e69 6f6e 5b48 6173 6844 6963  t: Union[HashDic
+00003a50: 742c 2053 6861 315d 2920 2d3e 204f 7074  t, Sha1]) -> Opt
+00003a60: 696f 6e61 6c5b 6279 7465 735d 3a0a 2020  ional[bytes]:.  
+00003a70: 2020 2020 2020 2320 4649 584d 453a 204d        # FIXME: M
+00003a80: 616b 6520 7468 6973 206d 6574 686f 6420  ake this method 
+00003a90: 7375 7070 6f72 7420 736c 6963 696e 6720  support slicing 
+00003aa0: 7468 6520 6064 6174 6160 0a20 2020 2020  the `data`.     
+00003ab0: 2020 2072 6574 7572 6e20 7365 6c66 2e6f     return self.o
+00003ac0: 626a 7374 6f72 6167 652e 636f 6e74 656e  bjstorage.conten
+00003ad0: 745f 6765 7428 636f 6e74 656e 7429 0a0a  t_get(content)..
+00003ae0: 2020 2020 4064 625f 7472 616e 7361 6374      @db_transact
+00003af0: 696f 6e28 290a 2020 2020 6465 6620 636f  ion().    def co
+00003b00: 6e74 656e 745f 6765 745f 7061 7274 6974  ntent_get_partit
+00003b10: 696f 6e28 0a20 2020 2020 2020 2073 656c  ion(.        sel
+00003b20: 662c 0a20 2020 2020 2020 2070 6172 7469  f,.        parti
+00003b30: 7469 6f6e 5f69 643a 2069 6e74 2c0a 2020  tion_id: int,.  
+00003b40: 2020 2020 2020 6e62 5f70 6172 7469 7469        nb_partiti
+00003b50: 6f6e 733a 2069 6e74 2c0a 2020 2020 2020  ons: int,.      
+00003b60: 2020 7061 6765 5f74 6f6b 656e 3a20 4f70    page_token: Op
+00003b70: 7469 6f6e 616c 5b73 7472 5d20 3d20 4e6f  tional[str] = No
+00003b80: 6e65 2c0a 2020 2020 2020 2020 6c69 6d69  ne,.        limi
+00003b90: 743a 2069 6e74 203d 2031 3030 302c 0a20  t: int = 1000,. 
+00003ba0: 2020 2020 2020 202a 2c0a 2020 2020 2020         *,.      
+00003bb0: 2020 6462 3a20 4462 2c0a 2020 2020 2020    db: Db,.      
+00003bc0: 2020 6375 723d 4e6f 6e65 2c0a 2020 2020    cur=None,.    
+00003bd0: 2920 2d3e 2050 6167 6564 5265 7375 6c74  ) -> PagedResult
+00003be0: 5b43 6f6e 7465 6e74 5d3a 0a20 2020 2020  [Content]:.     
+00003bf0: 2020 2072 6574 7572 6e20 5f67 6574 5f70     return _get_p
+00003c00: 6167 696e 6174 6564 5f73 6861 315f 7061  aginated_sha1_pa
+00003c10: 7274 6974 696f 6e28 0a20 2020 2020 2020  rtition(.       
+00003c20: 2020 2020 2063 7572 2c0a 2020 2020 2020       cur,.      
+00003c30: 2020 2020 2020 7061 7274 6974 696f 6e5f        partition_
+00003c40: 6964 2c0a 2020 2020 2020 2020 2020 2020  id,.            
+00003c50: 6e62 5f70 6172 7469 7469 6f6e 732c 0a20  nb_partitions,. 
+00003c60: 2020 2020 2020 2020 2020 2070 6167 655f             page_
+00003c70: 746f 6b65 6e2c 0a20 2020 2020 2020 2020  token,.         
+00003c80: 2020 206c 696d 6974 2c0a 2020 2020 2020     limit,.      
+00003c90: 2020 2020 2020 6462 2e63 6f6e 7465 6e74        db.content
+00003ca0: 5f67 6574 5f72 616e 6765 2c0a 2020 2020  _get_range,.    
+00003cb0: 2020 2020 2020 2020 6c61 6d62 6461 2072          lambda r
+00003cc0: 6f77 3a20 436f 6e74 656e 7428 2a2a 6469  ow: Content(**di
+00003cd0: 6374 287a 6970 2864 622e 636f 6e74 656e  ct(zip(db.conten
+00003ce0: 745f 6765 745f 6d65 7461 6461 7461 5f6b  t_get_metadata_k
+00003cf0: 6579 732c 2072 6f77 2929 292c 0a20 2020  eys, row))),.   
+00003d00: 2020 2020 2020 2020 206c 616d 6264 6120           lambda 
+00003d10: 726f 773a 2072 6f77 2e73 6861 312c 0a20  row: row.sha1,. 
+00003d20: 2020 2020 2020 2029 0a0a 2020 2020 4064         )..    @d
+00003d30: 625f 7472 616e 7361 6374 696f 6e28 7374  b_transaction(st
+00003d40: 6174 656d 656e 745f 7469 6d65 6f75 743d  atement_timeout=
+00003d50: 3530 3029 0a20 2020 2064 6566 2063 6f6e  500).    def con
+00003d60: 7465 6e74 5f67 6574 280a 2020 2020 2020  tent_get(.      
+00003d70: 2020 7365 6c66 2c20 636f 6e74 656e 7473    self, contents
+00003d80: 3a20 4c69 7374 5b62 7974 6573 5d2c 2061  : List[bytes], a
+00003d90: 6c67 6f3a 2073 7472 203d 2022 7368 6131  lgo: str = "sha1
+00003da0: 222c 202a 2c20 6462 3a20 4462 2c20 6375  ", *, db: Db, cu
+00003db0: 723d 4e6f 6e65 0a20 2020 2029 202d 3e20  r=None.    ) -> 
+00003dc0: 4c69 7374 5b4f 7074 696f 6e61 6c5b 436f  List[Optional[Co
+00003dd0: 6e74 656e 745d 5d3a 0a20 2020 2020 2020  ntent]]:.       
+00003de0: 2063 6f6e 7465 6e74 735f 6279 5f68 6173   contents_by_has
+00003df0: 683a 2044 6963 745b 6279 7465 732c 204f  h: Dict[bytes, O
+00003e00: 7074 696f 6e61 6c5b 436f 6e74 656e 745d  ptional[Content]
+00003e10: 5d20 3d20 7b7d 0a20 2020 2020 2020 2069  ] = {}.        i
+00003e20: 6620 616c 676f 206e 6f74 2069 6e20 4445  f algo not in DE
+00003e30: 4641 554c 545f 414c 474f 5249 5448 4d53  FAULT_ALGORITHMS
+00003e40: 3a0a 2020 2020 2020 2020 2020 2020 7261  :.            ra
+00003e50: 6973 6520 5374 6f72 6167 6541 7267 756d  ise StorageArgum
+00003e60: 656e 7445 7863 6570 7469 6f6e 280a 2020  entException(.  
+00003e70: 2020 2020 2020 2020 2020 2020 2020 2261                "a
+00003e80: 6c67 6f20 7368 6f75 6c64 2062 6520 6f6e  lgo should be on
+00003e90: 6520 6f66 207b 272c 272e 6a6f 696e 2844  e of {','.join(D
+00003ea0: 4546 4155 4c54 5f41 4c47 4f52 4954 484d  EFAULT_ALGORITHM
+00003eb0: 5329 7d22 0a20 2020 2020 2020 2020 2020  S)}".           
+00003ec0: 2029 0a0a 2020 2020 2020 2020 726f 7773   )..        rows
+00003ed0: 203d 2064 622e 636f 6e74 656e 745f 6765   = db.content_ge
+00003ee0: 745f 6d65 7461 6461 7461 5f66 726f 6d5f  t_metadata_from_
+00003ef0: 6861 7368 6573 2863 6f6e 7465 6e74 732c  hashes(contents,
+00003f00: 2061 6c67 6f2c 2063 7572 290a 2020 2020   algo, cur).    
+00003f10: 2020 2020 6b65 7920 3d20 6f70 6572 6174      key = operat
+00003f20: 6f72 2e61 7474 7267 6574 7465 7228 616c  or.attrgetter(al
+00003f30: 676f 290a 0a20 2020 2020 2020 2066 6f72  go)..        for
+00003f40: 2072 6f77 2069 6e20 726f 7773 3a0a 2020   row in rows:.  
+00003f50: 2020 2020 2020 2020 2020 726f 775f 6420            row_d 
+00003f60: 3d20 6469 6374 287a 6970 2864 622e 636f  = dict(zip(db.co
+00003f70: 6e74 656e 745f 6765 745f 6d65 7461 6461  ntent_get_metada
+00003f80: 7461 5f6b 6579 732c 2072 6f77 2929 0a20  ta_keys, row)). 
+00003f90: 2020 2020 2020 2020 2020 2063 6f6e 7465             conte
+00003fa0: 6e74 203d 2043 6f6e 7465 6e74 282a 2a72  nt = Content(**r
+00003fb0: 6f77 5f64 290a 2020 2020 2020 2020 2020  ow_d).          
+00003fc0: 2020 636f 6e74 656e 7473 5f62 795f 6861    contents_by_ha
+00003fd0: 7368 5b6b 6579 2863 6f6e 7465 6e74 295d  sh[key(content)]
+00003fe0: 203d 2063 6f6e 7465 6e74 0a0a 2020 2020   = content..    
+00003ff0: 2020 2020 7265 7475 726e 205b 636f 6e74      return [cont
+00004000: 656e 7473 5f62 795f 6861 7368 2e67 6574  ents_by_hash.get
+00004010: 2873 6861 3129 2066 6f72 2073 6861 3120  (sha1) for sha1 
+00004020: 696e 2063 6f6e 7465 6e74 735d 0a0a 2020  in contents]..  
+00004030: 2020 4064 625f 7472 616e 7361 6374 696f    @db_transactio
+00004040: 6e5f 6765 6e65 7261 746f 7228 290a 2020  n_generator().  
+00004050: 2020 6465 6620 636f 6e74 656e 745f 6d69    def content_mi
+00004060: 7373 696e 6728 0a20 2020 2020 2020 2073  ssing(.        s
+00004070: 656c 662c 0a20 2020 2020 2020 2063 6f6e  elf,.        con
+00004080: 7465 6e74 733a 204c 6973 745b 4861 7368  tents: List[Hash
+00004090: 4469 6374 5d2c 0a20 2020 2020 2020 206b  Dict],.        k
+000040a0: 6579 5f68 6173 683a 2073 7472 203d 2022  ey_hash: str = "
+000040b0: 7368 6131 222c 0a20 2020 2020 2020 202a  sha1",.        *
+000040c0: 2c0a 2020 2020 2020 2020 6462 3a20 4462  ,.        db: Db
+000040d0: 2c0a 2020 2020 2020 2020 6375 723d 4e6f  ,.        cur=No
+000040e0: 6e65 2c0a 2020 2020 2920 2d3e 2049 7465  ne,.    ) -> Ite
+000040f0: 7261 626c 655b 6279 7465 735d 3a0a 2020  rable[bytes]:.  
+00004100: 2020 2020 2020 6966 206b 6579 5f68 6173        if key_has
+00004110: 6820 6e6f 7420 696e 2044 4546 4155 4c54  h not in DEFAULT
+00004120: 5f41 4c47 4f52 4954 484d 533a 0a20 2020  _ALGORITHMS:.   
+00004130: 2020 2020 2020 2020 2072 6169 7365 2053           raise S
+00004140: 746f 7261 6765 4172 6775 6d65 6e74 4578  torageArgumentEx
+00004150: 6365 7074 696f 6e28 0a20 2020 2020 2020  ception(.       
+00004160: 2020 2020 2020 2020 2022 6b65 795f 6861           "key_ha
+00004170: 7368 2073 686f 756c 6420 6265 206f 6e65  sh should be one
+00004180: 206f 6620 7b27 2c27 2e6a 6f69 6e28 4445   of {','.join(DE
+00004190: 4641 554c 545f 414c 474f 5249 5448 4d53  FAULT_ALGORITHMS
+000041a0: 297d 220a 2020 2020 2020 2020 2020 2020  )}".            
+000041b0: 290a 0a20 2020 2020 2020 206b 6579 7320  )..        keys 
+000041c0: 3d20 6462 2e63 6f6e 7465 6e74 5f68 6173  = db.content_has
+000041d0: 685f 6b65 7973 0a20 2020 2020 2020 206b  h_keys.        k
+000041e0: 6579 5f68 6173 685f 6964 7820 3d20 6b65  ey_hash_idx = ke
+000041f0: 7973 2e69 6e64 6578 286b 6579 5f68 6173  ys.index(key_has
+00004200: 6829 0a0a 2020 2020 2020 2020 666f 7220  h)..        for 
+00004210: 6f62 6a20 696e 2064 622e 636f 6e74 656e  obj in db.conten
+00004220: 745f 6d69 7373 696e 675f 6672 6f6d 5f6c  t_missing_from_l
+00004230: 6973 7428 636f 6e74 656e 7473 2c20 6375  ist(contents, cu
+00004240: 7229 3a0a 2020 2020 2020 2020 2020 2020  r):.            
+00004250: 7969 656c 6420 6f62 6a5b 6b65 795f 6861  yield obj[key_ha
+00004260: 7368 5f69 6478 5d0a 0a20 2020 2040 6462  sh_idx]..    @db
+00004270: 5f74 7261 6e73 6163 7469 6f6e 5f67 656e  _transaction_gen
+00004280: 6572 6174 6f72 2829 0a20 2020 2064 6566  erator().    def
+00004290: 2063 6f6e 7465 6e74 5f6d 6973 7369 6e67   content_missing
+000042a0: 5f70 6572 5f73 6861 3128 0a20 2020 2020  _per_sha1(.     
+000042b0: 2020 2073 656c 662c 2063 6f6e 7465 6e74     self, content
+000042c0: 733a 204c 6973 745b 6279 7465 735d 2c20  s: List[bytes], 
+000042d0: 2a2c 2064 623a 2044 622c 2063 7572 3d4e  *, db: Db, cur=N
+000042e0: 6f6e 650a 2020 2020 2920 2d3e 2049 7465  one.    ) -> Ite
+000042f0: 7261 626c 655b 6279 7465 735d 3a0a 2020  rable[bytes]:.  
+00004300: 2020 2020 2020 666f 7220 6f62 6a20 696e        for obj in
+00004310: 2064 622e 636f 6e74 656e 745f 6d69 7373   db.content_miss
+00004320: 696e 675f 7065 725f 7368 6131 2863 6f6e  ing_per_sha1(con
+00004330: 7465 6e74 732c 2063 7572 293a 0a20 2020  tents, cur):.   
+00004340: 2020 2020 2020 2020 2079 6965 6c64 206f           yield o
+00004350: 626a 5b30 5d0a 0a20 2020 2040 6462 5f74  bj[0]..    @db_t
+00004360: 7261 6e73 6163 7469 6f6e 5f67 656e 6572  ransaction_gener
+00004370: 6174 6f72 2829 0a20 2020 2064 6566 2063  ator().    def c
+00004380: 6f6e 7465 6e74 5f6d 6973 7369 6e67 5f70  ontent_missing_p
+00004390: 6572 5f73 6861 315f 6769 7428 0a20 2020  er_sha1_git(.   
+000043a0: 2020 2020 2073 656c 662c 2063 6f6e 7465       self, conte
+000043b0: 6e74 733a 204c 6973 745b 6279 7465 735d  nts: List[bytes]
+000043c0: 2c20 2a2c 2064 623a 2044 622c 2063 7572  , *, db: Db, cur
+000043d0: 3d4e 6f6e 650a 2020 2020 2920 2d3e 2049  =None.    ) -> I
+000043e0: 7465 7261 626c 655b 5368 6131 4769 745d  terable[Sha1Git]
+000043f0: 3a0a 2020 2020 2020 2020 666f 7220 6f62  :.        for ob
+00004400: 6a20 696e 2064 622e 636f 6e74 656e 745f  j in db.content_
+00004410: 6d69 7373 696e 675f 7065 725f 7368 6131  missing_per_sha1
+00004420: 5f67 6974 2863 6f6e 7465 6e74 732c 2063  _git(contents, c
+00004430: 7572 293a 0a20 2020 2020 2020 2020 2020  ur):.           
+00004440: 2079 6965 6c64 206f 626a 5b30 5d0a 0a20   yield obj[0].. 
+00004450: 2020 2040 6462 5f74 7261 6e73 6163 7469     @db_transacti
+00004460: 6f6e 2829 0a20 2020 2064 6566 2063 6f6e  on().    def con
+00004470: 7465 6e74 5f66 696e 6428 7365 6c66 2c20  tent_find(self, 
+00004480: 636f 6e74 656e 743a 2048 6173 6844 6963  content: HashDic
+00004490: 742c 202a 2c20 6462 3a20 4462 2c20 6375  t, *, db: Db, cu
+000044a0: 723d 4e6f 6e65 2920 2d3e 204c 6973 745b  r=None) -> List[
+000044b0: 436f 6e74 656e 745d 3a0a 2020 2020 2020  Content]:.      
+000044c0: 2020 6966 206e 6f74 2073 6574 2863 6f6e    if not set(con
+000044d0: 7465 6e74 292e 696e 7465 7273 6563 7469  tent).intersecti
+000044e0: 6f6e 2844 4546 4155 4c54 5f41 4c47 4f52  on(DEFAULT_ALGOR
+000044f0: 4954 484d 5329 3a0a 2020 2020 2020 2020  ITHMS):.        
+00004500: 2020 2020 7261 6973 6520 5374 6f72 6167      raise Storag
+00004510: 6541 7267 756d 656e 7445 7863 6570 7469  eArgumentExcepti
+00004520: 6f6e 280a 2020 2020 2020 2020 2020 2020  on(.            
+00004530: 2020 2020 2263 6f6e 7465 6e74 206b 6579      "content key
+00004540: 7320 6d75 7374 2063 6f6e 7461 696e 2061  s must contain a
+00004550: 7420 6c65 6173 7420 6f6e 6520 220a 2020  t least one ".  
+00004560: 2020 2020 2020 2020 2020 2020 2020 6622                f"
+00004570: 6f66 3a20 7b27 2c20 272e 6a6f 696e 2873  of: {', '.join(s
+00004580: 6f72 7465 6428 4445 4641 554c 545f 414c  orted(DEFAULT_AL
+00004590: 474f 5249 5448 4d53 2929 7d22 0a20 2020  GORITHMS))}".   
+000045a0: 2020 2020 2020 2020 2029 0a0a 2020 2020           )..    
+000045b0: 2020 2020 726f 7773 203d 2064 622e 636f      rows = db.co
+000045c0: 6e74 656e 745f 6669 6e64 280a 2020 2020  ntent_find(.    
+000045d0: 2020 2020 2020 2020 7368 6131 3d63 6f6e          sha1=con
+000045e0: 7465 6e74 2e67 6574 2822 7368 6131 2229  tent.get("sha1")
+000045f0: 2c0a 2020 2020 2020 2020 2020 2020 7368  ,.            sh
+00004600: 6131 5f67 6974 3d63 6f6e 7465 6e74 2e67  a1_git=content.g
+00004610: 6574 2822 7368 6131 5f67 6974 2229 2c0a  et("sha1_git"),.
+00004620: 2020 2020 2020 2020 2020 2020 7368 6132              sha2
+00004630: 3536 3d63 6f6e 7465 6e74 2e67 6574 2822  56=content.get("
+00004640: 7368 6132 3536 2229 2c0a 2020 2020 2020  sha256"),.      
+00004650: 2020 2020 2020 626c 616b 6532 7332 3536        blake2s256
+00004660: 3d63 6f6e 7465 6e74 2e67 6574 2822 626c  =content.get("bl
+00004670: 616b 6532 7332 3536 2229 2c0a 2020 2020  ake2s256"),.    
+00004680: 2020 2020 2020 2020 6375 723d 6375 722c          cur=cur,
+00004690: 0a20 2020 2020 2020 2029 0a20 2020 2020  .        ).     
+000046a0: 2020 2063 6f6e 7465 6e74 7320 3d20 5b5d     contents = []
+000046b0: 0a20 2020 2020 2020 2066 6f72 2072 6f77  .        for row
+000046c0: 2069 6e20 726f 7773 3a0a 2020 2020 2020   in rows:.      
+000046d0: 2020 2020 2020 726f 775f 6420 3d20 6469        row_d = di
+000046e0: 6374 287a 6970 2864 622e 636f 6e74 656e  ct(zip(db.conten
+000046f0: 745f 6669 6e64 5f63 6f6c 732c 2072 6f77  t_find_cols, row
+00004700: 2929 0a20 2020 2020 2020 2020 2020 2063  )).            c
+00004710: 6f6e 7465 6e74 732e 6170 7065 6e64 2843  ontents.append(C
+00004720: 6f6e 7465 6e74 282a 2a72 6f77 5f64 2929  ontent(**row_d))
+00004730: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
+00004740: 636f 6e74 656e 7473 0a0a 2020 2020 4064  contents..    @d
+00004750: 625f 7472 616e 7361 6374 696f 6e28 290a  b_transaction().
+00004760: 2020 2020 6465 6620 636f 6e74 656e 745f      def content_
+00004770: 6765 745f 7261 6e64 6f6d 2873 656c 662c  get_random(self,
+00004780: 202a 2c20 6462 3a20 4462 2c20 6375 723d   *, db: Db, cur=
+00004790: 4e6f 6e65 2920 2d3e 2053 6861 3147 6974  None) -> Sha1Git
+000047a0: 3a0a 2020 2020 2020 2020 7265 7475 726e  :.        return
+000047b0: 2064 622e 636f 6e74 656e 745f 6765 745f   db.content_get_
+000047c0: 7261 6e64 6f6d 2863 7572 290a 0a20 2020  random(cur)..   
+000047d0: 2023 2323 2323 2323 2323 2323 2323 2323   ###############
+000047e0: 2323 2323 2323 2323 2323 230a 2020 2020  ###########.    
+000047f0: 2320 536b 6970 7065 6443 6f6e 7465 6e74  # SkippedContent
+00004800: 0a20 2020 2023 2323 2323 2323 2323 2323  .    ###########
+00004810: 2323 2323 2323 2323 2323 2323 2323 230a  ###############.
+00004820: 0a20 2020 2040 7374 6174 6963 6d65 7468  .    @staticmeth
+00004830: 6f64 0a20 2020 2064 6566 205f 736b 6970  od.    def _skip
+00004840: 7065 645f 636f 6e74 656e 745f 6e6f 726d  ped_content_norm
+00004850: 616c 697a 6528 6429 3a0a 2020 2020 2020  alize(d):.      
+00004860: 2020 6420 3d20 642e 636f 7079 2829 0a0a    d = d.copy()..
+00004870: 2020 2020 2020 2020 6966 2064 2e67 6574          if d.get
+00004880: 2822 7374 6174 7573 2229 2069 7320 4e6f  ("status") is No
+00004890: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
+000048a0: 645b 2273 7461 7475 7322 5d20 3d20 2261  d["status"] = "a
+000048b0: 6273 656e 7422 0a0a 2020 2020 2020 2020  bsent"..        
+000048c0: 6966 2064 2e67 6574 2822 6c65 6e67 7468  if d.get("length
+000048d0: 2229 2069 7320 4e6f 6e65 3a0a 2020 2020  ") is None:.    
+000048e0: 2020 2020 2020 2020 645b 226c 656e 6774          d["lengt
+000048f0: 6822 5d20 3d20 2d31 0a0a 2020 2020 2020  h"] = -1..      
+00004900: 2020 7265 7475 726e 2064 0a0a 2020 2020    return d..    
+00004910: 6465 6620 5f73 6b69 7070 6564 5f63 6f6e  def _skipped_con
+00004920: 7465 6e74 5f61 6464 5f6d 6574 6164 6174  tent_add_metadat
+00004930: 6128 7365 6c66 2c20 6462 2c20 6375 722c  a(self, db, cur,
+00004940: 2063 6f6e 7465 6e74 3a20 4c69 7374 5b53   content: List[S
+00004950: 6b69 7070 6564 436f 6e74 656e 745d 293a  kippedContent]):
+00004960: 0a20 2020 2020 2020 206f 7269 6769 6e5f  .        origin_
+00004970: 6964 7320 3d20 6462 2e6f 7269 6769 6e5f  ids = db.origin_
+00004980: 6964 5f67 6574 5f62 795f 7572 6c28 5b63  id_get_by_url([c
+00004990: 6f6e 742e 6f72 6967 696e 2066 6f72 2063  ont.origin for c
+000049a0: 6f6e 7420 696e 2063 6f6e 7465 6e74 5d2c  ont in content],
+000049b0: 2063 7572 3d63 7572 290a 2020 2020 2020   cur=cur).      
+000049c0: 2020 636f 6e74 656e 7420 3d20 5b0a 2020    content = [.  
+000049d0: 2020 2020 2020 2020 2020 6174 7472 2e65            attr.e
+000049e0: 766f 6c76 6528 632c 206f 7269 6769 6e3d  volve(c, origin=
+000049f0: 6f72 6967 696e 5f69 6429 0a20 2020 2020  origin_id).     
+00004a00: 2020 2020 2020 2066 6f72 2028 632c 206f         for (c, o
+00004a10: 7269 6769 6e5f 6964 2920 696e 207a 6970  rigin_id) in zip
+00004a20: 2863 6f6e 7465 6e74 2c20 6f72 6967 696e  (content, origin
+00004a30: 5f69 6473 290a 2020 2020 2020 2020 5d0a  _ids).        ].
+00004a40: 2020 2020 2020 2020 6462 2e6d 6b74 656d          db.mktem
+00004a50: 7028 2273 6b69 7070 6564 5f63 6f6e 7465  p("skipped_conte
+00004a60: 6e74 222c 2063 7572 290a 2020 2020 2020  nt", cur).      
+00004a70: 2020 6462 2e63 6f70 795f 746f 280a 2020    db.copy_to(.  
+00004a80: 2020 2020 2020 2020 2020 5b63 2e74 6f5f            [c.to_
+00004a90: 6469 6374 2829 2066 6f72 2063 2069 6e20  dict() for c in 
+00004aa0: 636f 6e74 656e 745d 2c0a 2020 2020 2020  content],.      
+00004ab0: 2020 2020 2020 2274 6d70 5f73 6b69 7070        "tmp_skipp
+00004ac0: 6564 5f63 6f6e 7465 6e74 222c 0a20 2020  ed_content",.   
+00004ad0: 2020 2020 2020 2020 2064 622e 736b 6970           db.skip
+00004ae0: 7065 645f 636f 6e74 656e 745f 6b65 7973  ped_content_keys
+00004af0: 2c0a 2020 2020 2020 2020 2020 2020 6375  ,.            cu
+00004b00: 722c 0a20 2020 2020 2020 2029 0a0a 2020  r,.        )..  
+00004b10: 2020 2020 2020 2320 6d6f 7665 206d 6574        # move met
+00004b20: 6164 6174 6120 696e 2070 6c61 6365 0a20  adata in place. 
+00004b30: 2020 2020 2020 2064 622e 736b 6970 7065         db.skippe
+00004b40: 645f 636f 6e74 656e 745f 6164 645f 6672  d_content_add_fr
+00004b50: 6f6d 5f74 656d 7028 6375 7229 0a0a 2020  om_temp(cur)..  
+00004b60: 2020 4064 625f 7472 616e 7361 6374 696f    @db_transactio
+00004b70: 6e28 290a 2020 2020 6465 6620 736b 6970  n().    def skip
+00004b80: 7065 645f 636f 6e74 656e 745f 6164 6428  ped_content_add(
+00004b90: 0a20 2020 2020 2020 2073 656c 662c 2063  .        self, c
+00004ba0: 6f6e 7465 6e74 3a20 4c69 7374 5b53 6b69  ontent: List[Ski
+00004bb0: 7070 6564 436f 6e74 656e 745d 2c20 2a2c  ppedContent], *,
+00004bc0: 2064 623a 2044 622c 2063 7572 3d4e 6f6e   db: Db, cur=Non
+00004bd0: 650a 2020 2020 2920 2d3e 2044 6963 745b  e.    ) -> Dict[
+00004be0: 7374 722c 2069 6e74 5d3a 0a20 2020 2020  str, int]:.     
+00004bf0: 2020 2063 7469 6d65 203d 206e 6f77 2829     ctime = now()
+00004c00: 0a20 2020 2020 2020 2063 6f6e 7465 6e74  .        content
+00004c10: 203d 205b 6174 7472 2e65 766f 6c76 6528   = [attr.evolve(
+00004c20: 632c 2063 7469 6d65 3d63 7469 6d65 2920  c, ctime=ctime) 
+00004c30: 666f 7220 6320 696e 2063 6f6e 7465 6e74  for c in content
+00004c40: 5d0a 0a20 2020 2020 2020 206d 6973 7369  ]..        missi
+00004c50: 6e67 5f63 6f6e 7465 6e74 7320 3d20 7365  ng_contents = se
+00004c60: 6c66 2e73 6b69 7070 6564 5f63 6f6e 7465  lf.skipped_conte
+00004c70: 6e74 5f6d 6973 7369 6e67 280a 2020 2020  nt_missing(.    
+00004c80: 2020 2020 2020 2020 2863 2e74 6f5f 6469          (c.to_di
+00004c90: 6374 2829 2066 6f72 2063 2069 6e20 636f  ct() for c in co
+00004ca0: 6e74 656e 7429 2c0a 2020 2020 2020 2020  ntent),.        
+00004cb0: 2020 2020 6462 3d64 622c 0a20 2020 2020      db=db,.     
+00004cc0: 2020 2020 2020 2063 7572 3d63 7572 2c0a         cur=cur,.
+00004cd0: 2020 2020 2020 2020 290a 2020 2020 2020          ).      
+00004ce0: 2020 636f 6e74 656e 7420 3d20 5b0a 2020    content = [.  
+00004cf0: 2020 2020 2020 2020 2020 630a 2020 2020            c.    
+00004d00: 2020 2020 2020 2020 666f 7220 6320 696e          for c in
+00004d10: 2063 6f6e 7465 6e74 0a20 2020 2020 2020   content.       
+00004d20: 2020 2020 2069 6620 616e 7928 0a20 2020       if any(.   
+00004d30: 2020 2020 2020 2020 2020 2020 2061 6c6c               all
+00004d40: 280a 2020 2020 2020 2020 2020 2020 2020  (.              
+00004d50: 2020 2020 2020 632e 6765 745f 6861 7368        c.get_hash
+00004d60: 2861 6c67 6f29 203d 3d20 6d69 7373 696e  (algo) == missin
+00004d70: 675f 636f 6e74 656e 742e 6765 7428 616c  g_content.get(al
+00004d80: 676f 290a 2020 2020 2020 2020 2020 2020  go).            
+00004d90: 2020 2020 2020 2020 666f 7220 616c 676f          for algo
+00004da0: 2069 6e20 4445 4641 554c 545f 414c 474f   in DEFAULT_ALGO
+00004db0: 5249 5448 4d53 0a20 2020 2020 2020 2020  RITHMS.         
+00004dc0: 2020 2020 2020 2029 0a20 2020 2020 2020         ).       
+00004dd0: 2020 2020 2020 2020 2066 6f72 206d 6973           for mis
+00004de0: 7369 6e67 5f63 6f6e 7465 6e74 2069 6e20  sing_content in 
+00004df0: 6d69 7373 696e 675f 636f 6e74 656e 7473  missing_contents
+00004e00: 0a20 2020 2020 2020 2020 2020 2029 0a20  .            ). 
+00004e10: 2020 2020 2020 205d 0a0a 2020 2020 2020         ]..      
+00004e20: 2020 7365 6c66 2e6a 6f75 726e 616c 5f77    self.journal_w
+00004e30: 7269 7465 722e 736b 6970 7065 645f 636f  riter.skipped_co
+00004e40: 6e74 656e 745f 6164 6428 636f 6e74 656e  ntent_add(conten
+00004e50: 7429 0a20 2020 2020 2020 2073 656c 662e  t).        self.
+00004e60: 5f73 6b69 7070 6564 5f63 6f6e 7465 6e74  _skipped_content
+00004e70: 5f61 6464 5f6d 6574 6164 6174 6128 6462  _add_metadata(db
+00004e80: 2c20 6375 722c 2063 6f6e 7465 6e74 290a  , cur, content).
+00004e90: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
+00004ea0: 7b0a 2020 2020 2020 2020 2020 2020 2273  {.            "s
+00004eb0: 6b69 7070 6564 5f63 6f6e 7465 6e74 3a61  kipped_content:a
+00004ec0: 6464 223a 206c 656e 2863 6f6e 7465 6e74  dd": len(content
+00004ed0: 292c 0a20 2020 2020 2020 207d 0a0a 2020  ),.        }..  
+00004ee0: 2020 4064 625f 7472 616e 7361 6374 696f    @db_transactio
+00004ef0: 6e28 290a 2020 2020 6465 6620 736b 6970  n().    def skip
+00004f00: 7065 645f 636f 6e74 656e 745f 6669 6e64  ped_content_find
+00004f10: 280a 2020 2020 2020 2020 7365 6c66 2c20  (.        self, 
+00004f20: 636f 6e74 656e 743a 2048 6173 6844 6963  content: HashDic
+00004f30: 742c 202a 2c20 6462 3a20 4462 2c20 6375  t, *, db: Db, cu
+00004f40: 723d 4e6f 6e65 0a20 2020 2029 202d 3e20  r=None.    ) -> 
+00004f50: 4c69 7374 5b53 6b69 7070 6564 436f 6e74  List[SkippedCont
+00004f60: 656e 745d 3a0a 2020 2020 2020 2020 6966  ent]:.        if
+00004f70: 206e 6f74 2073 6574 2863 6f6e 7465 6e74   not set(content
+00004f80: 292e 696e 7465 7273 6563 7469 6f6e 2844  ).intersection(D
+00004f90: 4546 4155 4c54 5f41 4c47 4f52 4954 484d  EFAULT_ALGORITHM
+00004fa0: 5329 3a0a 2020 2020 2020 2020 2020 2020  S):.            
+00004fb0: 7261 6973 6520 5374 6f72 6167 6541 7267  raise StorageArg
+00004fc0: 756d 656e 7445 7863 6570 7469 6f6e 280a  umentException(.
+00004fd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004fe0: 2263 6f6e 7465 6e74 206b 6579 7320 6d75  "content keys mu
+00004ff0: 7374 2063 6f6e 7461 696e 2061 7420 6c65  st contain at le
+00005000: 6173 7420 6f6e 6520 220a 2020 2020 2020  ast one ".      
+00005010: 2020 2020 2020 2020 2020 6622 6f66 3a20            f"of: 
+00005020: 7b27 2c20 272e 6a6f 696e 2873 6f72 7465  {', '.join(sorte
+00005030: 6428 4445 4641 554c 545f 414c 474f 5249  d(DEFAULT_ALGORI
+00005040: 5448 4d53 2929 7d22 0a20 2020 2020 2020  THMS))}".       
+00005050: 2020 2020 2029 0a0a 2020 2020 2020 2020       )..        
+00005060: 726f 7773 203d 2064 622e 736b 6970 7065  rows = db.skippe
+00005070: 645f 636f 6e74 656e 745f 6669 6e64 280a  d_content_find(.
+00005080: 2020 2020 2020 2020 2020 2020 7368 6131              sha1
+00005090: 3d63 6f6e 7465 6e74 2e67 6574 2822 7368  =content.get("sh
+000050a0: 6131 2229 2c0a 2020 2020 2020 2020 2020  a1"),.          
+000050b0: 2020 7368 6131 5f67 6974 3d63 6f6e 7465    sha1_git=conte
+000050c0: 6e74 2e67 6574 2822 7368 6131 5f67 6974  nt.get("sha1_git
+000050d0: 2229 2c0a 2020 2020 2020 2020 2020 2020  "),.            
+000050e0: 7368 6132 3536 3d63 6f6e 7465 6e74 2e67  sha256=content.g
+000050f0: 6574 2822 7368 6132 3536 2229 2c0a 2020  et("sha256"),.  
+00005100: 2020 2020 2020 2020 2020 626c 616b 6532            blake2
+00005110: 7332 3536 3d63 6f6e 7465 6e74 2e67 6574  s256=content.get
+00005120: 2822 626c 616b 6532 7332 3536 2229 2c0a  ("blake2s256"),.
+00005130: 2020 2020 2020 2020 2020 2020 6375 723d              cur=
+00005140: 6375 722c 0a20 2020 2020 2020 2029 0a20  cur,.        ). 
+00005150: 2020 2020 2020 2073 6b69 7070 6564 5f63         skipped_c
+00005160: 6f6e 7465 6e74 7320 3d20 5b5d 0a20 2020  ontents = [].   
+00005170: 2020 2020 2066 6f72 2072 6f77 2069 6e20       for row in 
+00005180: 726f 7773 3a0a 2020 2020 2020 2020 2020  rows:.          
+00005190: 2020 726f 775f 6420 3d20 6469 6374 287a    row_d = dict(z
+000051a0: 6970 2864 622e 736b 6970 7065 645f 636f  ip(db.skipped_co
+000051b0: 6e74 656e 745f 6669 6e64 5f63 6f6c 732c  ntent_find_cols,
+000051c0: 2072 6f77 2929 0a20 2020 2020 2020 2020   row)).         
+000051d0: 2020 2073 6b69 7070 6564 5f63 6f6e 7465     skipped_conte
+000051e0: 6e74 732e 6170 7065 6e64 2853 6b69 7070  nts.append(Skipp
+000051f0: 6564 436f 6e74 656e 7428 2a2a 726f 775f  edContent(**row_
+00005200: 6429 290a 2020 2020 2020 2020 7265 7475  d)).        retu
+00005210: 726e 2073 6b69 7070 6564 5f63 6f6e 7465  rn skipped_conte
+00005220: 6e74 730a 0a20 2020 2040 6462 5f74 7261  nts..    @db_tra
+00005230: 6e73 6163 7469 6f6e 5f67 656e 6572 6174  nsaction_generat
+00005240: 6f72 2829 0a20 2020 2064 6566 2073 6b69  or().    def ski
+00005250: 7070 6564 5f63 6f6e 7465 6e74 5f6d 6973  pped_content_mis
+00005260: 7369 6e67 280a 2020 2020 2020 2020 7365  sing(.        se
+00005270: 6c66 2c20 636f 6e74 656e 7473 3a20 4c69  lf, contents: Li
+00005280: 7374 5b44 6963 745b 7374 722c 2041 6e79  st[Dict[str, Any
+00005290: 5d5d 2c20 2a2c 2064 623a 2044 622c 2063  ]], *, db: Db, c
+000052a0: 7572 3d4e 6f6e 650a 2020 2020 2920 2d3e  ur=None.    ) ->
+000052b0: 2049 7465 7261 626c 655b 4469 6374 5b73   Iterable[Dict[s
+000052c0: 7472 2c20 416e 795d 5d3a 0a20 2020 2020  tr, Any]]:.     
+000052d0: 2020 2063 6f6e 7465 6e74 7320 3d20 6c69     contents = li
+000052e0: 7374 2863 6f6e 7465 6e74 7329 0a20 2020  st(contents).   
+000052f0: 2020 2020 2066 6f72 2063 6f6e 7465 6e74       for content
+00005300: 2069 6e20 6462 2e73 6b69 7070 6564 5f63   in db.skipped_c
+00005310: 6f6e 7465 6e74 5f6d 6973 7369 6e67 2863  ontent_missing(c
+00005320: 6f6e 7465 6e74 732c 2063 7572 293a 0a20  ontents, cur):. 
+00005330: 2020 2020 2020 2020 2020 2079 6965 6c64             yield
+00005340: 207b 0a20 2020 2020 2020 2020 2020 2020   {.             
+00005350: 2020 2061 6c67 6f3a 2068 6173 680a 2020     algo: hash.  
+00005360: 2020 2020 2020 2020 2020 2020 2020 666f                fo
+00005370: 7220 2861 6c67 6f2c 2068 6173 6829 2069  r (algo, hash) i
+00005380: 6e20 7a69 7028 6462 2e63 6f6e 7465 6e74  n zip(db.content
+00005390: 5f68 6173 685f 6b65 7973 2c20 636f 6e74  _hash_keys, cont
+000053a0: 656e 7429 0a20 2020 2020 2020 2020 2020  ent).           
+000053b0: 2020 2020 2069 6620 6861 7368 0a20 2020       if hash.   
+000053c0: 2020 2020 2020 2020 207d 0a0a 2020 2020           }..    
+000053d0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+000053e0: 2323 2323 2323 2323 2323 0a20 2020 2023  ##########.    #
+000053f0: 2044 6972 6563 746f 7279 0a20 2020 2023   Directory.    #
+00005400: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00005410: 2323 2323 2323 2323 230a 0a20 2020 2040  #########..    @
+00005420: 6462 5f74 7261 6e73 6163 7469 6f6e 2829  db_transaction()
+00005430: 0a20 2020 2064 6566 2064 6972 6563 746f  .    def directo
+00005440: 7279 5f61 6464 280a 2020 2020 2020 2020  ry_add(.        
+00005450: 7365 6c66 2c20 6469 7265 6374 6f72 6965  self, directorie
+00005460: 733a 204c 6973 745b 4469 7265 6374 6f72  s: List[Director
+00005470: 795d 2c20 2a2c 2064 623a 2044 622c 2063  y], *, db: Db, c
+00005480: 7572 3d4e 6f6e 650a 2020 2020 2920 2d3e  ur=None.    ) ->
+00005490: 2044 6963 745b 7374 722c 2069 6e74 5d3a   Dict[str, int]:
+000054a0: 0a20 2020 2020 2020 2073 756d 6d61 7279  .        summary
+000054b0: 203d 207b 2264 6972 6563 746f 7279 3a61   = {"directory:a
+000054c0: 6464 223a 2030 7d0a 0a20 2020 2020 2020  dd": 0}..       
+000054d0: 2064 6972 7320 3d20 7365 7428 290a 2020   dirs = set().  
+000054e0: 2020 2020 2020 6469 725f 656e 7472 6965        dir_entrie
+000054f0: 733a 2044 6963 745b 7374 722c 2064 6566  s: Dict[str, def
+00005500: 6175 6c74 6469 6374 5d20 3d20 7b0a 2020  aultdict] = {.  
+00005510: 2020 2020 2020 2020 2020 2266 696c 6522            "file"
+00005520: 3a20 6465 6661 756c 7464 6963 7428 6c69  : defaultdict(li
+00005530: 7374 292c 0a20 2020 2020 2020 2020 2020  st),.           
+00005540: 2022 6469 7222 3a20 6465 6661 756c 7464   "dir": defaultd
+00005550: 6963 7428 6c69 7374 292c 0a20 2020 2020  ict(list),.     
+00005560: 2020 2020 2020 2022 7265 7622 3a20 6465         "rev": de
+00005570: 6661 756c 7464 6963 7428 6c69 7374 292c  faultdict(list),
+00005580: 0a20 2020 2020 2020 207d 0a0a 2020 2020  .        }..    
+00005590: 2020 2020 666f 7220 6375 725f 6469 7220      for cur_dir 
+000055a0: 696e 2064 6972 6563 746f 7269 6573 3a0a  in directories:.
+000055b0: 2020 2020 2020 2020 2020 2020 6469 725f              dir_
+000055c0: 6964 203d 2063 7572 5f64 6972 2e69 640a  id = cur_dir.id.
+000055d0: 2020 2020 2020 2020 2020 2020 6469 7273              dirs
+000055e0: 2e61 6464 2864 6972 5f69 6429 0a20 2020  .add(dir_id).   
+000055f0: 2020 2020 2020 2020 2066 6f72 2073 7263           for src
+00005600: 5f65 6e74 7279 2069 6e20 6375 725f 6469  _entry in cur_di
+00005610: 722e 656e 7472 6965 733a 0a20 2020 2020  r.entries:.     
+00005620: 2020 2020 2020 2020 2020 2065 6e74 7279             entry
+00005630: 203d 2073 7263 5f65 6e74 7279 2e74 6f5f   = src_entry.to_
+00005640: 6469 6374 2829 0a20 2020 2020 2020 2020  dict().         
+00005650: 2020 2020 2020 2065 6e74 7279 5b22 6469         entry["di
+00005660: 725f 6964 225d 203d 2064 6972 5f69 640a  r_id"] = dir_id.
+00005670: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005680: 6469 725f 656e 7472 6965 735b 656e 7472  dir_entries[entr
+00005690: 795b 2274 7970 6522 5d5d 5b64 6972 5f69  y["type"]][dir_i
+000056a0: 645d 2e61 7070 656e 6428 656e 7472 7929  d].append(entry)
+000056b0: 0a0a 2020 2020 2020 2020 6469 7273 5f6d  ..        dirs_m
+000056c0: 6973 7369 6e67 203d 2073 6574 2873 656c  issing = set(sel
+000056d0: 662e 6469 7265 6374 6f72 795f 6d69 7373  f.directory_miss
+000056e0: 696e 6728 6469 7273 2c20 6462 3d64 622c  ing(dirs, db=db,
+000056f0: 2063 7572 3d63 7572 2929 0a20 2020 2020   cur=cur)).     
+00005700: 2020 2069 6620 6e6f 7420 6469 7273 5f6d     if not dirs_m
+00005710: 6973 7369 6e67 3a0a 2020 2020 2020 2020  issing:.        
+00005720: 2020 2020 7265 7475 726e 2073 756d 6d61      return summa
+00005730: 7279 0a0a 2020 2020 2020 2020 7365 6c66  ry..        self
+00005740: 2e6a 6f75 726e 616c 5f77 7269 7465 722e  .journal_writer.
+00005750: 6469 7265 6374 6f72 795f 6164 6428 0a20  directory_add(. 
+00005760: 2020 2020 2020 2020 2020 2064 6972 5f20             dir_ 
+00005770: 666f 7220 6469 725f 2069 6e20 6469 7265  for dir_ in dire
+00005780: 6374 6f72 6965 7320 6966 2064 6972 5f2e  ctories if dir_.
+00005790: 6964 2069 6e20 6469 7273 5f6d 6973 7369  id in dirs_missi
+000057a0: 6e67 0a20 2020 2020 2020 2029 0a0a 2020  ng.        )..  
+000057b0: 2020 2020 2020 2320 436f 7079 2064 6972        # Copy dir
+000057c0: 6563 746f 7279 206d 6574 6164 6174 610a  ectory metadata.
+000057d0: 2020 2020 2020 2020 6469 7273 5f6d 6973          dirs_mis
+000057e0: 7369 6e67 5f64 6963 7420 3d20 280a 2020  sing_dict = (.  
+000057f0: 2020 2020 2020 2020 2020 7b22 6964 223a            {"id":
+00005800: 2064 6972 5f2e 6964 2c20 2272 6177 5f6d   dir_.id, "raw_m
+00005810: 616e 6966 6573 7422 3a20 6469 725f 2e72  anifest": dir_.r
+00005820: 6177 5f6d 616e 6966 6573 747d 0a20 2020  aw_manifest}.   
+00005830: 2020 2020 2020 2020 2066 6f72 2064 6972           for dir
+00005840: 5f20 696e 2064 6972 6563 746f 7269 6573  _ in directories
+00005850: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
+00005860: 6469 725f 2e69 6420 696e 2064 6972 735f  dir_.id in dirs_
+00005870: 6d69 7373 696e 670a 2020 2020 2020 2020  missing.        
+00005880: 290a 2020 2020 2020 2020 6462 2e6d 6b74  ).        db.mkt
+00005890: 656d 7028 2264 6972 6563 746f 7279 222c  emp("directory",
+000058a0: 2063 7572 290a 2020 2020 2020 2020 6462   cur).        db
+000058b0: 2e63 6f70 795f 746f 2864 6972 735f 6d69  .copy_to(dirs_mi
+000058c0: 7373 696e 675f 6469 6374 2c20 2274 6d70  ssing_dict, "tmp
+000058d0: 5f64 6972 6563 746f 7279 222c 205b 2269  _directory", ["i
+000058e0: 6422 2c20 2272 6177 5f6d 616e 6966 6573  d", "raw_manifes
+000058f0: 7422 5d2c 2063 7572 290a 0a20 2020 2020  t"], cur)..     
+00005900: 2020 2023 2043 6f70 7920 656e 7472 6965     # Copy entrie
+00005910: 730a 2020 2020 2020 2020 666f 7220 656e  s.        for en
+00005920: 7472 795f 7479 7065 2c20 656e 7472 795f  try_type, entry_
+00005930: 6c69 7374 2069 6e20 6469 725f 656e 7472  list in dir_entr
+00005940: 6965 732e 6974 656d 7328 293a 0a20 2020  ies.items():.   
+00005950: 2020 2020 2020 2020 2065 6e74 7269 6573           entries
+00005960: 203d 2069 7465 7274 6f6f 6c73 2e63 6861   = itertools.cha
+00005970: 696e 2e66 726f 6d5f 6974 6572 6162 6c65  in.from_iterable
+00005980: 280a 2020 2020 2020 2020 2020 2020 2020  (.              
+00005990: 2020 656e 7472 6965 735f 666f 725f 6469    entries_for_di
+000059a0: 720a 2020 2020 2020 2020 2020 2020 2020  r.              
+000059b0: 2020 666f 7220 6469 725f 6964 2c20 656e    for dir_id, en
+000059c0: 7472 6965 735f 666f 725f 6469 7220 696e  tries_for_dir in
+000059d0: 2065 6e74 7279 5f6c 6973 742e 6974 656d   entry_list.item
+000059e0: 7328 290a 2020 2020 2020 2020 2020 2020  s().            
+000059f0: 2020 2020 6966 2064 6972 5f69 6420 696e      if dir_id in
+00005a00: 2064 6972 735f 6d69 7373 696e 670a 2020   dirs_missing.  
+00005a10: 2020 2020 2020 2020 2020 290a 0a20 2020            )..   
+00005a20: 2020 2020 2020 2020 2064 622e 6d6b 7465           db.mkte
+00005a30: 6d70 5f64 6972 5f65 6e74 7279 2865 6e74  mp_dir_entry(ent
+00005a40: 7279 5f74 7970 6529 0a0a 2020 2020 2020  ry_type)..      
+00005a50: 2020 2020 2020 6462 2e63 6f70 795f 746f        db.copy_to
+00005a60: 280a 2020 2020 2020 2020 2020 2020 2020  (.              
+00005a70: 2020 656e 7472 6965 732c 0a20 2020 2020    entries,.     
+00005a80: 2020 2020 2020 2020 2020 2022 746d 705f             "tmp_
+00005a90: 6469 7265 6374 6f72 795f 656e 7472 795f  directory_entry_
+00005aa0: 2573 2220 2520 656e 7472 795f 7479 7065  %s" % entry_type
+00005ab0: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+00005ac0: 2020 5b22 7461 7267 6574 222c 2022 6e61    ["target", "na
+00005ad0: 6d65 222c 2022 7065 726d 7322 2c20 2264  me", "perms", "d
+00005ae0: 6972 5f69 6422 5d2c 0a20 2020 2020 2020  ir_id"],.       
+00005af0: 2020 2020 2020 2020 2063 7572 2c0a 2020           cur,.  
+00005b00: 2020 2020 2020 2020 2020 290a 0a20 2020            )..   
+00005b10: 2020 2020 2023 2044 6f20 7468 6520 6669       # Do the fi
+00005b20: 6e61 6c20 636f 7079 0a20 2020 2020 2020  nal copy.       
+00005b30: 2064 622e 6469 7265 6374 6f72 795f 6164   db.directory_ad
+00005b40: 645f 6672 6f6d 5f74 656d 7028 6375 7229  d_from_temp(cur)
+00005b50: 0a20 2020 2020 2020 2073 756d 6d61 7279  .        summary
+00005b60: 5b22 6469 7265 6374 6f72 793a 6164 6422  ["directory:add"
+00005b70: 5d20 3d20 6c65 6e28 6469 7273 5f6d 6973  ] = len(dirs_mis
+00005b80: 7369 6e67 290a 0a20 2020 2020 2020 2072  sing)..        r
+00005b90: 6574 7572 6e20 7375 6d6d 6172 790a 0a20  eturn summary.. 
+00005ba0: 2020 2040 6462 5f74 7261 6e73 6163 7469     @db_transacti
+00005bb0: 6f6e 5f67 656e 6572 6174 6f72 2829 0a20  on_generator(). 
+00005bc0: 2020 2064 6566 2064 6972 6563 746f 7279     def directory
+00005bd0: 5f6d 6973 7369 6e67 280a 2020 2020 2020  _missing(.      
+00005be0: 2020 7365 6c66 2c20 6469 7265 6374 6f72    self, director
+00005bf0: 6965 733a 204c 6973 745b 5368 6131 4769  ies: List[Sha1Gi
+00005c00: 745d 2c20 2a2c 2064 623a 2044 622c 2063  t], *, db: Db, c
+00005c10: 7572 3d4e 6f6e 650a 2020 2020 2920 2d3e  ur=None.    ) ->
+00005c20: 2049 7465 7261 626c 655b 5368 6131 4769   Iterable[Sha1Gi
+00005c30: 745d 3a0a 2020 2020 2020 2020 666f 7220  t]:.        for 
+00005c40: 6f62 6a20 696e 2064 622e 6469 7265 6374  obj in db.direct
+00005c50: 6f72 795f 6d69 7373 696e 675f 6672 6f6d  ory_missing_from
+00005c60: 5f6c 6973 7428 6469 7265 6374 6f72 6965  _list(directorie
+00005c70: 732c 2063 7572 293a 0a20 2020 2020 2020  s, cur):.       
+00005c80: 2020 2020 2079 6965 6c64 206f 626a 5b30       yield obj[0
+00005c90: 5d0a 0a20 2020 2040 6462 5f74 7261 6e73  ]..    @db_trans
+00005ca0: 6163 7469 6f6e 5f67 656e 6572 6174 6f72  action_generator
+00005cb0: 2873 7461 7465 6d65 6e74 5f74 696d 656f  (statement_timeo
+00005cc0: 7574 3d32 3030 3030 290a 2020 2020 6465  ut=20000).    de
+00005cd0: 6620 6469 7265 6374 6f72 795f 6c73 280a  f directory_ls(.
+00005ce0: 2020 2020 2020 2020 7365 6c66 2c20 6469          self, di
+00005cf0: 7265 6374 6f72 793a 2053 6861 3147 6974  rectory: Sha1Git
+00005d00: 2c20 7265 6375 7273 6976 653a 2062 6f6f  , recursive: boo
+00005d10: 6c20 3d20 4661 6c73 652c 202a 2c20 6462  l = False, *, db
+00005d20: 3a20 4462 2c20 6375 723d 4e6f 6e65 0a20  : Db, cur=None. 
+00005d30: 2020 2029 202d 3e20 4974 6572 6162 6c65     ) -> Iterable
+00005d40: 5b44 6963 745b 7374 722c 2041 6e79 5d5d  [Dict[str, Any]]
+00005d50: 3a0a 2020 2020 2020 2020 6966 2072 6563  :.        if rec
+00005d60: 7572 7369 7665 3a0a 2020 2020 2020 2020  ursive:.        
+00005d70: 2020 2020 7265 735f 6765 6e20 3d20 6462      res_gen = db
+00005d80: 2e64 6972 6563 746f 7279 5f77 616c 6b28  .directory_walk(
+00005d90: 6469 7265 6374 6f72 792c 2063 7572 3d63  directory, cur=c
+00005da0: 7572 290a 2020 2020 2020 2020 656c 7365  ur).        else
+00005db0: 3a0a 2020 2020 2020 2020 2020 2020 7265  :.            re
+00005dc0: 735f 6765 6e20 3d20 6462 2e64 6972 6563  s_gen = db.direc
+00005dd0: 746f 7279 5f77 616c 6b5f 6f6e 6528 6469  tory_walk_one(di
+00005de0: 7265 6374 6f72 792c 2063 7572 3d63 7572  rectory, cur=cur
+00005df0: 290a 0a20 2020 2020 2020 2066 6f72 206c  )..        for l
+00005e00: 696e 6520 696e 2072 6573 5f67 656e 3a0a  ine in res_gen:.
+00005e10: 2020 2020 2020 2020 2020 2020 7969 656c              yiel
+00005e20: 6420 6469 6374 287a 6970 2864 622e 6469  d dict(zip(db.di
+00005e30: 7265 6374 6f72 795f 6c73 5f63 6f6c 732c  rectory_ls_cols,
+00005e40: 206c 696e 6529 290a 0a20 2020 2040 6462   line))..    @db
+00005e50: 5f74 7261 6e73 6163 7469 6f6e 2873 7461  _transaction(sta
+00005e60: 7465 6d65 6e74 5f74 696d 656f 7574 3d34  tement_timeout=4
+00005e70: 3030 3029 0a20 2020 2064 6566 2064 6972  000).    def dir
+00005e80: 6563 746f 7279 5f65 6e74 7279 5f67 6574  ectory_entry_get
+00005e90: 5f62 795f 7061 7468 280a 2020 2020 2020  _by_path(.      
+00005ea0: 2020 7365 6c66 2c20 6469 7265 6374 6f72    self, director
+00005eb0: 793a 2053 6861 3147 6974 2c20 7061 7468  y: Sha1Git, path
+00005ec0: 733a 204c 6973 745b 6279 7465 735d 2c20  s: List[bytes], 
+00005ed0: 2a2c 2064 623a 2044 622c 2063 7572 3d4e  *, db: Db, cur=N
+00005ee0: 6f6e 650a 2020 2020 2920 2d3e 204f 7074  one.    ) -> Opt
+00005ef0: 696f 6e61 6c5b 4469 6374 5b73 7472 2c20  ional[Dict[str, 
+00005f00: 416e 795d 5d3a 0a20 2020 2020 2020 2072  Any]]:.        r
+00005f10: 6573 203d 2064 622e 6469 7265 6374 6f72  es = db.director
+00005f20: 795f 656e 7472 795f 6765 745f 6279 5f70  y_entry_get_by_p
+00005f30: 6174 6828 6469 7265 6374 6f72 792c 2070  ath(directory, p
+00005f40: 6174 6873 2c20 6375 7229 0a20 2020 2020  aths, cur).     
+00005f50: 2020 2072 6574 7572 6e20 6469 6374 287a     return dict(z
+00005f60: 6970 2864 622e 6469 7265 6374 6f72 795f  ip(db.directory_
+00005f70: 6c73 5f63 6f6c 732c 2072 6573 2929 2069  ls_cols, res)) i
+00005f80: 6620 7265 7320 656c 7365 204e 6f6e 650a  f res else None.
+00005f90: 0a20 2020 2040 6462 5f74 7261 6e73 6163  .    @db_transac
+00005fa0: 7469 6f6e 2829 0a20 2020 2064 6566 2064  tion().    def d
+00005fb0: 6972 6563 746f 7279 5f67 6574 5f72 616e  irectory_get_ran
+00005fc0: 646f 6d28 7365 6c66 2c20 2a2c 2064 623a  dom(self, *, db:
+00005fd0: 2044 622c 2063 7572 3d4e 6f6e 6529 202d   Db, cur=None) -
+00005fe0: 3e20 5368 6131 4769 743a 0a20 2020 2020  > Sha1Git:.     
+00005ff0: 2020 2072 6574 7572 6e20 6462 2e64 6972     return db.dir
+00006000: 6563 746f 7279 5f67 6574 5f72 616e 646f  ectory_get_rando
+00006010: 6d28 6375 7229 0a0a 2020 2020 4064 625f  m(cur)..    @db_
+00006020: 7472 616e 7361 6374 696f 6e28 290a 2020  transaction().  
+00006030: 2020 6465 6620 6469 7265 6374 6f72 795f    def directory_
+00006040: 6765 745f 656e 7472 6965 7328 0a20 2020  get_entries(.   
+00006050: 2020 2020 2073 656c 662c 0a20 2020 2020       self,.     
+00006060: 2020 2064 6972 6563 746f 7279 5f69 643a     directory_id:
+00006070: 2053 6861 3147 6974 2c0a 2020 2020 2020   Sha1Git,.      
+00006080: 2020 7061 6765 5f74 6f6b 656e 3a20 4f70    page_token: Op
+00006090: 7469 6f6e 616c 5b62 7974 6573 5d20 3d20  tional[bytes] = 
+000060a0: 4e6f 6e65 2c0a 2020 2020 2020 2020 6c69  None,.        li
+000060b0: 6d69 743a 2069 6e74 203d 2031 3030 302c  mit: int = 1000,
+000060c0: 0a20 2020 2020 2020 202a 2c0a 2020 2020  .        *,.    
+000060d0: 2020 2020 6462 3a20 4462 2c0a 2020 2020      db: Db,.    
+000060e0: 2020 2020 6375 723d 4e6f 6e65 2c0a 2020      cur=None,.  
+000060f0: 2020 2920 2d3e 204f 7074 696f 6e61 6c5b    ) -> Optional[
+00006100: 5061 6765 6452 6573 756c 745b 4469 7265  PagedResult[Dire
+00006110: 6374 6f72 7945 6e74 7279 5d5d 3a0a 2020  ctoryEntry]]:.  
+00006120: 2020 2020 2020 6966 206c 6973 7428 7365        if list(se
+00006130: 6c66 2e64 6972 6563 746f 7279 5f6d 6973  lf.directory_mis
+00006140: 7369 6e67 285b 6469 7265 6374 6f72 795f  sing([directory_
+00006150: 6964 5d2c 2064 623d 6462 2c20 6375 723d  id], db=db, cur=
+00006160: 6375 7229 293a 0a20 2020 2020 2020 2020  cur)):.         
+00006170: 2020 2072 6574 7572 6e20 4e6f 6e65 0a0a     return None..
+00006180: 2020 2020 2020 2020 6966 2070 6167 655f          if page_
+00006190: 746f 6b65 6e20 6973 206e 6f74 204e 6f6e  token is not Non
+000061a0: 653a 0a20 2020 2020 2020 2020 2020 2072  e:.            r
+000061b0: 6169 7365 2053 746f 7261 6765 4172 6775  aise StorageArgu
+000061c0: 6d65 6e74 4578 6365 7074 696f 6e28 2255  mentException("U
+000061d0: 6e73 7570 706f 7274 6564 2070 6167 6520  nsupported page 
+000061e0: 746f 6b65 6e22 290a 0a20 2020 2020 2020  token")..       
+000061f0: 2023 2054 4f44 4f3a 2061 6374 7561 6c6c   # TODO: actuall
+00006200: 7920 7061 6769 6e61 7465 0a20 2020 2020  y paginate.     
+00006210: 2020 2072 6f77 7320 3d20 6462 2e64 6972     rows = db.dir
+00006220: 6563 746f 7279 5f67 6574 5f65 6e74 7269  ectory_get_entri
+00006230: 6573 2864 6972 6563 746f 7279 5f69 642c  es(directory_id,
+00006240: 2063 7572 3d63 7572 290a 2020 2020 2020   cur=cur).      
+00006250: 2020 7265 7475 726e 2050 6167 6564 5265    return PagedRe
+00006260: 7375 6c74 280a 2020 2020 2020 2020 2020  sult(.          
+00006270: 2020 7265 7375 6c74 733d 5b0a 2020 2020    results=[.    
+00006280: 2020 2020 2020 2020 2020 2020 4469 7265              Dire
+00006290: 6374 6f72 7945 6e74 7279 282a 2a64 6963  ctoryEntry(**dic
+000062a0: 7428 7a69 7028 6462 2e64 6972 6563 746f  t(zip(db.directo
+000062b0: 7279 5f67 6574 5f65 6e74 7269 6573 5f63  ry_get_entries_c
+000062c0: 6f6c 732c 2072 6f77 2929 290a 2020 2020  ols, row))).    
+000062d0: 2020 2020 2020 2020 2020 2020 666f 7220              for 
+000062e0: 726f 7720 696e 2072 6f77 730a 2020 2020  row in rows.    
+000062f0: 2020 2020 2020 2020 5d2c 0a20 2020 2020          ],.     
+00006300: 2020 2020 2020 206e 6578 745f 7061 6765         next_page
+00006310: 5f74 6f6b 656e 3d4e 6f6e 652c 0a20 2020  _token=None,.   
+00006320: 2020 2020 2029 0a0a 2020 2020 4064 625f       )..    @db_
+00006330: 7472 616e 7361 6374 696f 6e28 290a 2020  transaction().  
+00006340: 2020 6465 6620 6469 7265 6374 6f72 795f    def directory_
+00006350: 6765 745f 7261 775f 6d61 6e69 6665 7374  get_raw_manifest
+00006360: 280a 2020 2020 2020 2020 7365 6c66 2c20  (.        self, 
+00006370: 6469 7265 6374 6f72 795f 6964 733a 204c  directory_ids: L
+00006380: 6973 745b 5368 6131 4769 745d 2c20 2a2c  ist[Sha1Git], *,
+00006390: 2064 623a 2044 622c 2063 7572 3d4e 6f6e   db: Db, cur=Non
+000063a0: 650a 2020 2020 2920 2d3e 2044 6963 745b  e.    ) -> Dict[
+000063b0: 5368 6131 4769 742c 204f 7074 696f 6e61  Sha1Git, Optiona
+000063c0: 6c5b 6279 7465 735d 5d3a 0a20 2020 2020  l[bytes]]:.     
+000063d0: 2020 2072 6574 7572 6e20 6469 6374 2864     return dict(d
+000063e0: 622e 6469 7265 6374 6f72 795f 6765 745f  b.directory_get_
+000063f0: 7261 775f 6d61 6e69 6665 7374 2864 6972  raw_manifest(dir
+00006400: 6563 746f 7279 5f69 6473 2c20 6375 723d  ectory_ids, cur=
+00006410: 6375 7229 290a 0a20 2020 2040 6462 5f74  cur))..    @db_t
+00006420: 7261 6e73 6163 7469 6f6e 2829 0a20 2020  ransaction().   
+00006430: 2064 6566 2064 6972 6563 746f 7279 5f67   def directory_g
+00006440: 6574 5f69 645f 7061 7274 6974 696f 6e28  et_id_partition(
+00006450: 0a20 2020 2020 2020 2073 656c 662c 0a20  .        self,. 
+00006460: 2020 2020 2020 2070 6172 7469 7469 6f6e         partition
+00006470: 5f69 643a 2069 6e74 2c0a 2020 2020 2020  _id: int,.      
+00006480: 2020 6e62 5f70 6172 7469 7469 6f6e 733a    nb_partitions:
+00006490: 2069 6e74 2c0a 2020 2020 2020 2020 7061   int,.        pa
+000064a0: 6765 5f74 6f6b 656e 3a20 4f70 7469 6f6e  ge_token: Option
+000064b0: 616c 5b73 7472 5d20 3d20 4e6f 6e65 2c0a  al[str] = None,.
+000064c0: 2020 2020 2020 2020 6c69 6d69 743a 2069          limit: i
+000064d0: 6e74 203d 2031 3030 302c 0a20 2020 2020  nt = 1000,.     
+000064e0: 2020 202a 2c0a 2020 2020 2020 2020 6462     *,.        db
+000064f0: 3a20 4462 2c0a 2020 2020 2020 2020 6375  : Db,.        cu
+00006500: 723d 4e6f 6e65 2c0a 2020 2020 2920 2d3e  r=None,.    ) ->
+00006510: 2050 6167 6564 5265 7375 6c74 5b53 6861   PagedResult[Sha
+00006520: 3147 6974 5d3a 0a20 2020 2020 2020 2072  1Git]:.        r
+00006530: 6574 7572 6e20 5f67 6574 5f70 6167 696e  eturn _get_pagin
+00006540: 6174 6564 5f73 6861 315f 7061 7274 6974  ated_sha1_partit
+00006550: 696f 6e28 0a20 2020 2020 2020 2020 2020  ion(.           
+00006560: 2063 7572 2c0a 2020 2020 2020 2020 2020   cur,.          
+00006570: 2020 7061 7274 6974 696f 6e5f 6964 2c0a    partition_id,.
+00006580: 2020 2020 2020 2020 2020 2020 6e62 5f70              nb_p
+00006590: 6172 7469 7469 6f6e 732c 0a20 2020 2020  artitions,.     
+000065a0: 2020 2020 2020 2070 6167 655f 746f 6b65         page_toke
+000065b0: 6e2c 0a20 2020 2020 2020 2020 2020 206c  n,.            l
+000065c0: 696d 6974 2c0a 2020 2020 2020 2020 2020  imit,.          
+000065d0: 2020 6462 2e64 6972 6563 746f 7279 5f67    db.directory_g
+000065e0: 6574 5f69 645f 7261 6e67 652c 0a20 2020  et_id_range,.   
+000065f0: 2020 2020 2020 2020 206f 7065 7261 746f           operato
+00006600: 722e 6974 656d 6765 7474 6572 2830 292c  r.itemgetter(0),
+00006610: 0a20 2020 2020 2020 2020 2020 206c 616d  .            lam
+00006620: 6264 6120 6964 5f3a 2069 645f 2c0a 2020  bda id_: id_,.  
+00006630: 2020 2020 2020 290a 0a20 2020 2023 2323        )..    ###
+00006640: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00006650: 2323 2323 2323 230a 2020 2020 2320 5265  #######.    # Re
+00006660: 7669 7369 6f6e 0a20 2020 2023 2323 2323  vision.    #####
+00006670: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00006680: 2323 2323 230a 0a20 2020 2040 6462 5f74  #####..    @db_t
+00006690: 7261 6e73 6163 7469 6f6e 2829 0a20 2020  ransaction().   
+000066a0: 2064 6566 2072 6576 6973 696f 6e5f 6164   def revision_ad
+000066b0: 6428 0a20 2020 2020 2020 2073 656c 662c  d(.        self,
+000066c0: 2072 6576 6973 696f 6e73 3a20 4c69 7374   revisions: List
+000066d0: 5b52 6576 6973 696f 6e5d 2c20 2a2c 2064  [Revision], *, d
+000066e0: 623a 2044 622c 2063 7572 3d4e 6f6e 650a  b: Db, cur=None.
+000066f0: 2020 2020 2920 2d3e 2044 6963 745b 7374      ) -> Dict[st
+00006700: 722c 2069 6e74 5d3a 0a20 2020 2020 2020  r, int]:.       
+00006710: 2073 756d 6d61 7279 203d 207b 2272 6576   summary = {"rev
+00006720: 6973 696f 6e3a 6164 6422 3a20 307d 0a0a  ision:add": 0}..
+00006730: 2020 2020 2020 2020 7265 7669 7369 6f6e          revision
+00006740: 735f 6d69 7373 696e 6720 3d20 7365 7428  s_missing = set(
+00006750: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
+00006760: 662e 7265 7669 7369 6f6e 5f6d 6973 7369  f.revision_missi
+00006770: 6e67 280a 2020 2020 2020 2020 2020 2020  ng(.            
+00006780: 2020 2020 7365 7428 7265 7669 7369 6f6e      set(revision
+00006790: 2e69 6420 666f 7220 7265 7669 7369 6f6e  .id for revision
+000067a0: 2069 6e20 7265 7669 7369 6f6e 7329 2c20   in revisions), 
+000067b0: 6462 3d64 622c 2063 7572 3d63 7572 0a20  db=db, cur=cur. 
+000067c0: 2020 2020 2020 2020 2020 2029 0a20 2020             ).   
+000067d0: 2020 2020 2029 0a0a 2020 2020 2020 2020       )..        
+000067e0: 6966 206e 6f74 2072 6576 6973 696f 6e73  if not revisions
+000067f0: 5f6d 6973 7369 6e67 3a0a 2020 2020 2020  _missing:.      
+00006800: 2020 2020 2020 7265 7475 726e 2073 756d        return sum
+00006810: 6d61 7279 0a0a 2020 2020 2020 2020 6462  mary..        db
+00006820: 2e6d 6b74 656d 705f 7265 7669 7369 6f6e  .mktemp_revision
+00006830: 2863 7572 290a 0a20 2020 2020 2020 2072  (cur)..        r
+00006840: 6576 6973 696f 6e73 5f66 696c 7465 7265  evisions_filtere
+00006850: 6420 3d20 5b0a 2020 2020 2020 2020 2020  d = [.          
+00006860: 2020 7265 7669 7369 6f6e 2066 6f72 2072    revision for r
+00006870: 6576 6973 696f 6e20 696e 2072 6576 6973  evision in revis
+00006880: 696f 6e73 2069 6620 7265 7669 7369 6f6e  ions if revision
+00006890: 2e69 6420 696e 2072 6576 6973 696f 6e73  .id in revisions
+000068a0: 5f6d 6973 7369 6e67 0a20 2020 2020 2020  _missing.       
+000068b0: 205d 0a0a 2020 2020 2020 2020 7365 6c66   ]..        self
+000068c0: 2e6a 6f75 726e 616c 5f77 7269 7465 722e  .journal_writer.
+000068d0: 7265 7669 7369 6f6e 5f61 6464 2872 6576  revision_add(rev
+000068e0: 6973 696f 6e73 5f66 696c 7465 7265 6429  isions_filtered)
+000068f0: 0a0a 2020 2020 2020 2020 6462 5f72 6576  ..        db_rev
+00006900: 6973 696f 6e73 5f66 696c 7465 7265 6420  isions_filtered 
+00006910: 3d20 6c69 7374 286d 6170 2863 6f6e 7665  = list(map(conve
+00006920: 7274 6572 732e 7265 7669 7369 6f6e 5f74  rters.revision_t
+00006930: 6f5f 6462 2c20 7265 7669 7369 6f6e 735f  o_db, revisions_
+00006940: 6669 6c74 6572 6564 2929 0a0a 2020 2020  filtered))..    
+00006950: 2020 2020 7061 7265 6e74 735f 6669 6c74      parents_filt
+00006960: 6572 6564 3a20 4c69 7374 5b44 6963 745b  ered: List[Dict[
+00006970: 7374 722c 2041 6e79 5d5d 203d 205b 5d0a  str, Any]] = [].
+00006980: 0a20 2020 2020 2020 2077 6974 6820 636f  .        with co
+00006990: 6e76 6572 745f 7661 6c69 6461 7469 6f6e  nvert_validation
+000069a0: 5f65 7863 6570 7469 6f6e 7328 293a 0a20  _exceptions():. 
+000069b0: 2020 2020 2020 2020 2020 2064 622e 636f             db.co
+000069c0: 7079 5f74 6f28 0a20 2020 2020 2020 2020  py_to(.         
+000069d0: 2020 2020 2020 2064 625f 7265 7669 7369         db_revisi
+000069e0: 6f6e 735f 6669 6c74 6572 6564 2c0a 2020  ons_filtered,.  
+000069f0: 2020 2020 2020 2020 2020 2020 2020 2274                "t
+00006a00: 6d70 5f72 6576 6973 696f 6e22 2c0a 2020  mp_revision",.  
+00006a10: 2020 2020 2020 2020 2020 2020 2020 6462                db
+00006a20: 2e72 6576 6973 696f 6e5f 6164 645f 636f  .revision_add_co
+00006a30: 6c73 2c0a 2020 2020 2020 2020 2020 2020  ls,.            
+00006a40: 2020 2020 6375 722c 0a20 2020 2020 2020      cur,.       
+00006a50: 2020 2020 2020 2020 206c 616d 6264 6120           lambda 
+00006a60: 7265 763a 2070 6172 656e 7473 5f66 696c  rev: parents_fil
+00006a70: 7465 7265 642e 6578 7465 6e64 2872 6576  tered.extend(rev
+00006a80: 5b22 7061 7265 6e74 7322 5d29 2c0a 2020  ["parents"]),.  
+00006a90: 2020 2020 2020 2020 2020 290a 0a20 2020            )..   
+00006aa0: 2020 2020 2020 2020 2064 622e 7265 7669           db.revi
+00006ab0: 7369 6f6e 5f61 6464 5f66 726f 6d5f 7465  sion_add_from_te
+00006ac0: 6d70 2863 7572 290a 0a20 2020 2020 2020  mp(cur)..       
+00006ad0: 2020 2020 2064 622e 636f 7079 5f74 6f28       db.copy_to(
+00006ae0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00006af0: 2070 6172 656e 7473 5f66 696c 7465 7265   parents_filtere
+00006b00: 642c 0a20 2020 2020 2020 2020 2020 2020  d,.             
+00006b10: 2020 2022 7265 7669 7369 6f6e 5f68 6973     "revision_his
+00006b20: 746f 7279 222c 0a20 2020 2020 2020 2020  tory",.         
+00006b30: 2020 2020 2020 205b 2269 6422 2c20 2270         ["id", "p
+00006b40: 6172 656e 745f 6964 222c 2022 7061 7265  arent_id", "pare
+00006b50: 6e74 5f72 616e 6b22 5d2c 0a20 2020 2020  nt_rank"],.     
+00006b60: 2020 2020 2020 2020 2020 2063 7572 2c0a             cur,.
+00006b70: 2020 2020 2020 2020 2020 2020 290a 0a20              ).. 
+00006b80: 2020 2020 2020 2072 6574 7572 6e20 7b22         return {"
+00006b90: 7265 7669 7369 6f6e 3a61 6464 223a 206c  revision:add": l
+00006ba0: 656e 2872 6576 6973 696f 6e73 5f6d 6973  en(revisions_mis
+00006bb0: 7369 6e67 297d 0a0a 2020 2020 4064 625f  sing)}..    @db_
+00006bc0: 7472 616e 7361 6374 696f 6e5f 6765 6e65  transaction_gene
+00006bd0: 7261 746f 7228 290a 2020 2020 6465 6620  rator().    def 
+00006be0: 7265 7669 7369 6f6e 5f6d 6973 7369 6e67  revision_missing
+00006bf0: 280a 2020 2020 2020 2020 7365 6c66 2c20  (.        self, 
+00006c00: 7265 7669 7369 6f6e 733a 204c 6973 745b  revisions: List[
+00006c10: 5368 6131 4769 745d 2c20 2a2c 2064 623a  Sha1Git], *, db:
+00006c20: 2044 622c 2063 7572 3d4e 6f6e 650a 2020   Db, cur=None.  
+00006c30: 2020 2920 2d3e 2049 7465 7261 626c 655b    ) -> Iterable[
+00006c40: 5368 6131 4769 745d 3a0a 2020 2020 2020  Sha1Git]:.      
+00006c50: 2020 6966 206e 6f74 2072 6576 6973 696f    if not revisio
+00006c60: 6e73 3a0a 2020 2020 2020 2020 2020 2020  ns:.            
+00006c70: 7265 7475 726e 204e 6f6e 650a 0a20 2020  return None..   
+00006c80: 2020 2020 2066 6f72 206f 626a 2069 6e20       for obj in 
+00006c90: 6462 2e72 6576 6973 696f 6e5f 6d69 7373  db.revision_miss
+00006ca0: 696e 675f 6672 6f6d 5f6c 6973 7428 7265  ing_from_list(re
+00006cb0: 7669 7369 6f6e 732c 2063 7572 293a 0a20  visions, cur):. 
+00006cc0: 2020 2020 2020 2020 2020 2079 6965 6c64             yield
+00006cd0: 206f 626a 5b30 5d0a 0a20 2020 2040 6462   obj[0]..    @db
+00006ce0: 5f74 7261 6e73 6163 7469 6f6e 2829 0a20  _transaction(). 
+00006cf0: 2020 2064 6566 2072 6576 6973 696f 6e5f     def revision_
+00006d00: 6765 745f 7061 7274 6974 696f 6e28 0a20  get_partition(. 
+00006d10: 2020 2020 2020 2073 656c 662c 0a20 2020         self,.   
+00006d20: 2020 2020 2070 6172 7469 7469 6f6e 5f69       partition_i
+00006d30: 643a 2069 6e74 2c0a 2020 2020 2020 2020  d: int,.        
+00006d40: 6e62 5f70 6172 7469 7469 6f6e 733a 2069  nb_partitions: i
+00006d50: 6e74 2c0a 2020 2020 2020 2020 7061 6765  nt,.        page
+00006d60: 5f74 6f6b 656e 3a20 4f70 7469 6f6e 616c  _token: Optional
+00006d70: 5b73 7472 5d20 3d20 4e6f 6e65 2c0a 2020  [str] = None,.  
+00006d80: 2020 2020 2020 6c69 6d69 743a 2069 6e74        limit: int
+00006d90: 203d 2031 3030 302c 0a20 2020 2020 2020   = 1000,.       
+00006da0: 202a 2c0a 2020 2020 2020 2020 6462 3a20   *,.        db: 
+00006db0: 4462 2c0a 2020 2020 2020 2020 6375 723d  Db,.        cur=
+00006dc0: 4e6f 6e65 2c0a 2020 2020 2920 2d3e 2050  None,.    ) -> P
+00006dd0: 6167 6564 5265 7375 6c74 5b52 6576 6973  agedResult[Revis
+00006de0: 696f 6e5d 3a0a 2020 2020 2020 2020 7265  ion]:.        re
+00006df0: 7475 726e 205f 6765 745f 7061 6769 6e61  turn _get_pagina
+00006e00: 7465 645f 7368 6131 5f70 6172 7469 7469  ted_sha1_partiti
+00006e10: 6f6e 280a 2020 2020 2020 2020 2020 2020  on(.            
+00006e20: 6375 722c 0a20 2020 2020 2020 2020 2020  cur,.           
+00006e30: 2070 6172 7469 7469 6f6e 5f69 642c 0a20   partition_id,. 
+00006e40: 2020 2020 2020 2020 2020 206e 625f 7061             nb_pa
+00006e50: 7274 6974 696f 6e73 2c0a 2020 2020 2020  rtitions,.      
+00006e60: 2020 2020 2020 7061 6765 5f74 6f6b 656e        page_token
+00006e70: 2c0a 2020 2020 2020 2020 2020 2020 6c69  ,.            li
+00006e80: 6d69 742c 0a20 2020 2020 2020 2020 2020  mit,.           
+00006e90: 2064 622e 7265 7669 7369 6f6e 5f67 6574   db.revision_get
+00006ea0: 5f72 616e 6765 2c0a 2020 2020 2020 2020  _range,.        
+00006eb0: 2020 2020 6c61 6d62 6461 2072 6f77 3a20      lambda row: 
+00006ec0: 636f 6e76 6572 7465 7273 2e64 625f 746f  converters.db_to
+00006ed0: 5f72 6576 6973 696f 6e28 6469 6374 287a  _revision(dict(z
+00006ee0: 6970 2864 622e 7265 7669 7369 6f6e 5f67  ip(db.revision_g
+00006ef0: 6574 5f63 6f6c 732c 2072 6f77 2929 292c  et_cols, row))),
+00006f00: 0a20 2020 2020 2020 2029 0a0a 2020 2020  .        )..    
+00006f10: 4064 625f 7472 616e 7361 6374 696f 6e28  @db_transaction(
+00006f20: 7374 6174 656d 656e 745f 7469 6d65 6f75  statement_timeou
+00006f30: 743d 3230 3030 290a 2020 2020 6465 6620  t=2000).    def 
+00006f40: 7265 7669 7369 6f6e 5f67 6574 280a 2020  revision_get(.  
+00006f50: 2020 2020 2020 7365 6c66 2c0a 2020 2020        self,.    
+00006f60: 2020 2020 7265 7669 7369 6f6e 5f69 6473      revision_ids
+00006f70: 3a20 4c69 7374 5b53 6861 3147 6974 5d2c  : List[Sha1Git],
+00006f80: 0a20 2020 2020 2020 2069 676e 6f72 655f  .        ignore_
+00006f90: 6469 7370 6c61 796e 616d 653a 2062 6f6f  displayname: boo
+00006fa0: 6c20 3d20 4661 6c73 652c 0a20 2020 2020  l = False,.     
+00006fb0: 2020 202a 2c0a 2020 2020 2020 2020 6462     *,.        db
+00006fc0: 3a20 4462 2c0a 2020 2020 2020 2020 6375  : Db,.        cu
+00006fd0: 723d 4e6f 6e65 2c0a 2020 2020 2920 2d3e  r=None,.    ) ->
+00006fe0: 204c 6973 745b 4f70 7469 6f6e 616c 5b52   List[Optional[R
+00006ff0: 6576 6973 696f 6e5d 5d3a 0a20 2020 2020  evision]]:.     
+00007000: 2020 2072 6576 6973 696f 6e73 203d 205b     revisions = [
+00007010: 5d0a 2020 2020 2020 2020 666f 7220 6c69  ].        for li
+00007020: 6e65 2069 6e20 6462 2e72 6576 6973 696f  ne in db.revisio
+00007030: 6e5f 6765 745f 6672 6f6d 5f6c 6973 7428  n_get_from_list(
+00007040: 7265 7669 7369 6f6e 5f69 6473 2c20 6967  revision_ids, ig
+00007050: 6e6f 7265 5f64 6973 706c 6179 6e61 6d65  nore_displayname
+00007060: 2c20 6375 7229 3a0a 2020 2020 2020 2020  , cur):.        
+00007070: 2020 2020 7265 7669 7369 6f6e 203d 2063      revision = c
+00007080: 6f6e 7665 7274 6572 732e 6462 5f74 6f5f  onverters.db_to_
+00007090: 6f70 7469 6f6e 616c 5f72 6576 6973 696f  optional_revisio
+000070a0: 6e28 0a20 2020 2020 2020 2020 2020 2020  n(.             
+000070b0: 2020 2064 6963 7428 7a69 7028 6462 2e72     dict(zip(db.r
+000070c0: 6576 6973 696f 6e5f 6765 745f 636f 6c73  evision_get_cols
+000070d0: 2c20 6c69 6e65 2929 0a20 2020 2020 2020  , line)).       
+000070e0: 2020 2020 2029 0a20 2020 2020 2020 2020       ).         
+000070f0: 2020 2072 6576 6973 696f 6e73 2e61 7070     revisions.app
+00007100: 656e 6428 7265 7669 7369 6f6e 290a 0a20  end(revision).. 
+00007110: 2020 2020 2020 2072 6574 7572 6e20 7265         return re
+00007120: 7669 7369 6f6e 730a 0a20 2020 2040 6462  visions..    @db
+00007130: 5f74 7261 6e73 6163 7469 6f6e 5f67 656e  _transaction_gen
+00007140: 6572 6174 6f72 2873 7461 7465 6d65 6e74  erator(statement
+00007150: 5f74 696d 656f 7574 3d32 3030 3029 0a20  _timeout=2000). 
+00007160: 2020 2064 6566 2072 6576 6973 696f 6e5f     def revision_
+00007170: 6c6f 6728 0a20 2020 2020 2020 2073 656c  log(.        sel
+00007180: 662c 0a20 2020 2020 2020 2072 6576 6973  f,.        revis
+00007190: 696f 6e73 3a20 4c69 7374 5b53 6861 3147  ions: List[Sha1G
+000071a0: 6974 5d2c 0a20 2020 2020 2020 2069 676e  it],.        ign
+000071b0: 6f72 655f 6469 7370 6c61 796e 616d 653a  ore_displayname:
+000071c0: 2062 6f6f 6c20 3d20 4661 6c73 652c 0a20   bool = False,. 
+000071d0: 2020 2020 2020 206c 696d 6974 3a20 4f70         limit: Op
+000071e0: 7469 6f6e 616c 5b69 6e74 5d20 3d20 4e6f  tional[int] = No
+000071f0: 6e65 2c0a 2020 2020 2020 2020 2a2c 0a20  ne,.        *,. 
+00007200: 2020 2020 2020 2064 623a 2044 622c 0a20         db: Db,. 
+00007210: 2020 2020 2020 2063 7572 3d4e 6f6e 652c         cur=None,
+00007220: 0a20 2020 2029 202d 3e20 4974 6572 6162  .    ) -> Iterab
+00007230: 6c65 5b4f 7074 696f 6e61 6c5b 4469 6374  le[Optional[Dict
+00007240: 5b73 7472 2c20 416e 795d 5d5d 3a0a 2020  [str, Any]]]:.  
+00007250: 2020 2020 2020 666f 7220 6c69 6e65 2069        for line i
+00007260: 6e20 6462 2e72 6576 6973 696f 6e5f 6c6f  n db.revision_lo
+00007270: 6728 0a20 2020 2020 2020 2020 2020 2072  g(.            r
+00007280: 6576 6973 696f 6e73 2c20 6967 6e6f 7265  evisions, ignore
+00007290: 5f64 6973 706c 6179 6e61 6d65 3d69 676e  _displayname=ign
+000072a0: 6f72 655f 6469 7370 6c61 796e 616d 652c  ore_displayname,
+000072b0: 206c 696d 6974 3d6c 696d 6974 2c20 6375   limit=limit, cu
+000072c0: 723d 6375 720a 2020 2020 2020 2020 293a  r=cur.        ):
+000072d0: 0a20 2020 2020 2020 2020 2020 2064 6174  .            dat
+000072e0: 6120 3d20 636f 6e76 6572 7465 7273 2e64  a = converters.d
+000072f0: 625f 746f 5f72 6576 6973 696f 6e28 6469  b_to_revision(di
+00007300: 6374 287a 6970 2864 622e 7265 7669 7369  ct(zip(db.revisi
+00007310: 6f6e 5f67 6574 5f63 6f6c 732c 206c 696e  on_get_cols, lin
+00007320: 6529 2929 0a20 2020 2020 2020 2020 2020  e))).           
+00007330: 2069 6620 6e6f 7420 6461 7461 3a0a 2020   if not data:.  
+00007340: 2020 2020 2020 2020 2020 2020 2020 7969                yi
+00007350: 656c 6420 4e6f 6e65 0a20 2020 2020 2020  eld None.       
+00007360: 2020 2020 2020 2020 2063 6f6e 7469 6e75           continu
+00007370: 650a 2020 2020 2020 2020 2020 2020 7969  e.            yi
+00007380: 656c 6420 6461 7461 2e74 6f5f 6469 6374  eld data.to_dict
+00007390: 2829 0a0a 2020 2020 4064 625f 7472 616e  ()..    @db_tran
+000073a0: 7361 6374 696f 6e5f 6765 6e65 7261 746f  saction_generato
+000073b0: 7228 7374 6174 656d 656e 745f 7469 6d65  r(statement_time
+000073c0: 6f75 743d 3230 3030 290a 2020 2020 6465  out=2000).    de
+000073d0: 6620 7265 7669 7369 6f6e 5f73 686f 7274  f revision_short
+000073e0: 6c6f 6728 0a20 2020 2020 2020 2073 656c  log(.        sel
+000073f0: 662c 2072 6576 6973 696f 6e73 3a20 4c69  f, revisions: Li
+00007400: 7374 5b53 6861 3147 6974 5d2c 206c 696d  st[Sha1Git], lim
+00007410: 6974 3a20 4f70 7469 6f6e 616c 5b69 6e74  it: Optional[int
+00007420: 5d20 3d20 4e6f 6e65 2c20 2a2c 2064 623a  ] = None, *, db:
+00007430: 2044 622c 2063 7572 3d4e 6f6e 650a 2020   Db, cur=None.  
+00007440: 2020 2920 2d3e 2049 7465 7261 626c 655b    ) -> Iterable[
+00007450: 4f70 7469 6f6e 616c 5b54 7570 6c65 5b53  Optional[Tuple[S
+00007460: 6861 3147 6974 2c20 5475 706c 655b 5368  ha1Git, Tuple[Sh
+00007470: 6131 4769 742c 202e 2e2e 5d5d 5d5d 3a0a  a1Git, ...]]]]:.
+00007480: 2020 2020 2020 2020 7969 656c 6420 6672          yield fr
+00007490: 6f6d 2064 622e 7265 7669 7369 6f6e 5f73  om db.revision_s
+000074a0: 686f 7274 6c6f 6728 7265 7669 7369 6f6e  hortlog(revision
+000074b0: 732c 206c 696d 6974 2c20 6375 7229 0a0a  s, limit, cur)..
+000074c0: 2020 2020 4064 625f 7472 616e 7361 6374      @db_transact
+000074d0: 696f 6e28 290a 2020 2020 6465 6620 7265  ion().    def re
+000074e0: 7669 7369 6f6e 5f67 6574 5f72 616e 646f  vision_get_rando
+000074f0: 6d28 7365 6c66 2c20 2a2c 2064 623a 2044  m(self, *, db: D
+00007500: 622c 2063 7572 3d4e 6f6e 6529 202d 3e20  b, cur=None) -> 
+00007510: 5368 6131 4769 743a 0a20 2020 2020 2020  Sha1Git:.       
+00007520: 2072 6574 7572 6e20 6462 2e72 6576 6973   return db.revis
+00007530: 696f 6e5f 6765 745f 7261 6e64 6f6d 2863  ion_get_random(c
+00007540: 7572 290a 0a20 2020 2023 2323 2323 2323  ur)..    #######
+00007550: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00007560: 2323 230a 2020 2020 2320 4578 7449 440a  ###.    # ExtID.
+00007570: 2020 2020 2323 2323 2323 2323 2323 2323      ############
+00007580: 2323 2323 2323 2323 2323 2323 2323 0a0a  ##############..
+00007590: 2020 2020 4064 625f 7472 616e 7361 6374      @db_transact
+000075a0: 696f 6e28 290a 2020 2020 6465 6620 6578  ion().    def ex
+000075b0: 7469 645f 6765 745f 6672 6f6d 5f65 7874  tid_get_from_ext
+000075c0: 6964 280a 2020 2020 2020 2020 7365 6c66  id(.        self
+000075d0: 2c0a 2020 2020 2020 2020 6964 5f74 7970  ,.        id_typ
+000075e0: 653a 2073 7472 2c0a 2020 2020 2020 2020  e: str,.        
+000075f0: 6964 733a 204c 6973 745b 6279 7465 735d  ids: List[bytes]
+00007600: 2c0a 2020 2020 2020 2020 7665 7273 696f  ,.        versio
+00007610: 6e3a 204f 7074 696f 6e61 6c5b 696e 745d  n: Optional[int]
+00007620: 203d 204e 6f6e 652c 0a20 2020 2020 2020   = None,.       
+00007630: 202a 2c0a 2020 2020 2020 2020 6462 3a20   *,.        db: 
+00007640: 4462 2c0a 2020 2020 2020 2020 6375 723d  Db,.        cur=
+00007650: 4e6f 6e65 2c0a 2020 2020 2920 2d3e 204c  None,.    ) -> L
+00007660: 6973 745b 4578 7449 445d 3a0a 2020 2020  ist[ExtID]:.    
+00007670: 2020 2020 6578 7469 6473 203d 205b 5d0a      extids = [].
+00007680: 2020 2020 2020 2020 666f 7220 726f 7720          for row 
+00007690: 696e 2064 622e 6578 7469 645f 6765 745f  in db.extid_get_
+000076a0: 6672 6f6d 5f65 7874 6964 5f6c 6973 7428  from_extid_list(
+000076b0: 6964 5f74 7970 652c 2069 6473 2c20 7665  id_type, ids, ve
+000076c0: 7273 696f 6e3d 7665 7273 696f 6e2c 2063  rsion=version, c
+000076d0: 7572 3d63 7572 293a 0a20 2020 2020 2020  ur=cur):.       
+000076e0: 2020 2020 2069 6620 726f 775b 305d 2069       if row[0] i
+000076f0: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
+00007700: 2020 2020 2020 2020 2020 2020 6578 7469              exti
+00007710: 6473 2e61 7070 656e 6428 636f 6e76 6572  ds.append(conver
+00007720: 7465 7273 2e64 625f 746f 5f65 7874 6964  ters.db_to_extid
+00007730: 2864 6963 7428 7a69 7028 6462 2e65 7874  (dict(zip(db.ext
+00007740: 6964 5f63 6f6c 732c 2072 6f77 2929 2929  id_cols, row))))
+00007750: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
+00007760: 6578 7469 6473 0a0a 2020 2020 4064 625f  extids..    @db_
+00007770: 7472 616e 7361 6374 696f 6e28 290a 2020  transaction().  
+00007780: 2020 6465 6620 6578 7469 645f 6765 745f    def extid_get_
+00007790: 6672 6f6d 5f74 6172 6765 7428 0a20 2020  from_target(.   
+000077a0: 2020 2020 2073 656c 662c 0a20 2020 2020       self,.     
+000077b0: 2020 2074 6172 6765 745f 7479 7065 3a20     target_type: 
+000077c0: 4f62 6a65 6374 5479 7065 2c0a 2020 2020  ObjectType,.    
+000077d0: 2020 2020 6964 733a 204c 6973 745b 5368      ids: List[Sh
+000077e0: 6131 4769 745d 2c0a 2020 2020 2020 2020  a1Git],.        
+000077f0: 6578 7469 645f 7479 7065 3a20 4f70 7469  extid_type: Opti
+00007800: 6f6e 616c 5b73 7472 5d20 3d20 4e6f 6e65  onal[str] = None
+00007810: 2c0a 2020 2020 2020 2020 6578 7469 645f  ,.        extid_
+00007820: 7665 7273 696f 6e3a 204f 7074 696f 6e61  version: Optiona
+00007830: 6c5b 696e 745d 203d 204e 6f6e 652c 0a20  l[int] = None,. 
+00007840: 2020 2020 2020 202a 2c0a 2020 2020 2020         *,.      
+00007850: 2020 6462 3a20 4462 2c0a 2020 2020 2020    db: Db,.      
+00007860: 2020 6375 723d 4e6f 6e65 2c0a 2020 2020    cur=None,.    
+00007870: 2920 2d3e 204c 6973 745b 4578 7449 445d  ) -> List[ExtID]
+00007880: 3a0a 2020 2020 2020 2020 6578 7469 6473  :.        extids
+00007890: 203d 205b 5d0a 2020 2020 2020 2020 6966   = [].        if
+000078a0: 2028 6578 7469 645f 7665 7273 696f 6e20   (extid_version 
+000078b0: 6973 206e 6f74 204e 6f6e 6520 616e 6420  is not None and 
+000078c0: 6578 7469 645f 7479 7065 2069 7320 4e6f  extid_type is No
+000078d0: 6e65 2920 6f72 2028 0a20 2020 2020 2020  ne) or (.       
+000078e0: 2020 2020 2065 7874 6964 5f76 6572 7369       extid_versi
+000078f0: 6f6e 2069 7320 4e6f 6e65 2061 6e64 2065  on is None and e
+00007900: 7874 6964 5f74 7970 6520 6973 206e 6f74  xtid_type is not
+00007910: 204e 6f6e 650a 2020 2020 2020 2020 293a   None.        ):
+00007920: 0a20 2020 2020 2020 2020 2020 2072 6169  .            rai
+00007930: 7365 2056 616c 7565 4572 726f 7228 2259  se ValueError("Y
+00007940: 6f75 206d 7573 7420 7072 6f76 6964 6520  ou must provide 
+00007950: 626f 7468 2065 7874 6964 5f74 7970 6520  both extid_type 
+00007960: 616e 6420 6578 7469 645f 7665 7273 696f  and extid_versio
+00007970: 6e22 290a 0a20 2020 2020 2020 2066 6f72  n")..        for
+00007980: 2072 6f77 2069 6e20 6462 2e65 7874 6964   row in db.extid
+00007990: 5f67 6574 5f66 726f 6d5f 7377 6869 645f  _get_from_swhid_
+000079a0: 6c69 7374 280a 2020 2020 2020 2020 2020  list(.          
+000079b0: 2020 7461 7267 6574 5f74 7970 652e 7661    target_type.va
+000079c0: 6c75 652c 0a20 2020 2020 2020 2020 2020  lue,.           
+000079d0: 2069 6473 2c0a 2020 2020 2020 2020 2020   ids,.          
+000079e0: 2020 6578 7469 645f 7665 7273 696f 6e3d    extid_version=
+000079f0: 6578 7469 645f 7665 7273 696f 6e2c 0a20  extid_version,. 
+00007a00: 2020 2020 2020 2020 2020 2065 7874 6964             extid
+00007a10: 5f74 7970 653d 6578 7469 645f 7479 7065  _type=extid_type
+00007a20: 2c0a 2020 2020 2020 2020 2020 2020 6375  ,.            cu
+00007a30: 723d 6375 722c 0a20 2020 2020 2020 2029  r=cur,.        )
+00007a40: 3a0a 2020 2020 2020 2020 2020 2020 6966  :.            if
+00007a50: 2072 6f77 5b30 5d20 6973 206e 6f74 204e   row[0] is not N
+00007a60: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
+00007a70: 2020 2020 2065 7874 6964 732e 6170 7065       extids.appe
+00007a80: 6e64 2863 6f6e 7665 7274 6572 732e 6462  nd(converters.db
+00007a90: 5f74 6f5f 6578 7469 6428 6469 6374 287a  _to_extid(dict(z
+00007aa0: 6970 2864 622e 6578 7469 645f 636f 6c73  ip(db.extid_cols
+00007ab0: 2c20 726f 7729 2929 290a 2020 2020 2020  , row)))).      
+00007ac0: 2020 7265 7475 726e 2065 7874 6964 730a    return extids.
+00007ad0: 0a20 2020 2040 6462 5f74 7261 6e73 6163  .    @db_transac
+00007ae0: 7469 6f6e 2829 0a20 2020 2064 6566 2065  tion().    def e
+00007af0: 7874 6964 5f61 6464 2873 656c 662c 2069  xtid_add(self, i
+00007b00: 6473 3a20 4c69 7374 5b45 7874 4944 5d2c  ds: List[ExtID],
+00007b10: 202a 2c20 6462 3a20 4462 2c20 6375 723d   *, db: Db, cur=
+00007b20: 4e6f 6e65 2920 2d3e 2044 6963 745b 7374  None) -> Dict[st
+00007b30: 722c 2069 6e74 5d3a 0a20 2020 2020 2020  r, int]:.       
+00007b40: 2065 7874 6964 203d 205b 0a20 2020 2020   extid = [.     
+00007b50: 2020 2020 2020 207b 0a20 2020 2020 2020         {.       
+00007b60: 2020 2020 2020 2020 2022 6578 7469 6422           "extid"
+00007b70: 3a20 6578 7469 642e 6578 7469 642c 0a20  : extid.extid,. 
+00007b80: 2020 2020 2020 2020 2020 2020 2020 2022                 "
+00007b90: 6578 7469 645f 7479 7065 223a 2065 7874  extid_type": ext
+00007ba0: 6964 2e65 7874 6964 5f74 7970 652c 0a20  id.extid_type,. 
+00007bb0: 2020 2020 2020 2020 2020 2020 2020 2022                 "
+00007bc0: 6578 7469 645f 7665 7273 696f 6e22 3a20  extid_version": 
+00007bd0: 6765 7461 7474 7228 6578 7469 642c 2022  getattr(extid, "
+00007be0: 6578 7469 645f 7665 7273 696f 6e22 2c20  extid_version", 
+00007bf0: 3029 2c0a 2020 2020 2020 2020 2020 2020  0),.            
+00007c00: 2020 2020 2274 6172 6765 7422 3a20 6578      "target": ex
+00007c10: 7469 642e 7461 7267 6574 2e6f 626a 6563  tid.target.objec
+00007c20: 745f 6964 2c0a 2020 2020 2020 2020 2020  t_id,.          
+00007c30: 2020 2020 2020 2274 6172 6765 745f 7479        "target_ty
+00007c40: 7065 223a 2065 7874 6964 2e74 6172 6765  pe": extid.targe
+00007c50: 742e 6f62 6a65 6374 5f74 7970 652e 6e61  t.object_type.na
+00007c60: 6d65 2e6c 6f77 6572 2829 2c20 2023 2061  me.lower(),  # a
+00007c70: 7267 6868 0a20 2020 2020 2020 2020 2020  rghh.           
+00007c80: 207d 0a20 2020 2020 2020 2020 2020 2066   }.            f
+00007c90: 6f72 2065 7874 6964 2069 6e20 6964 730a  or extid in ids.
+00007ca0: 2020 2020 2020 2020 5d0a 2020 2020 2020          ].      
+00007cb0: 2020 6462 2e6d 6b74 656d 7028 2265 7874    db.mktemp("ext
+00007cc0: 6964 222c 2063 7572 290a 0a20 2020 2020  id", cur)..     
+00007cd0: 2020 2073 656c 662e 6a6f 7572 6e61 6c5f     self.journal_
+00007ce0: 7772 6974 6572 2e65 7874 6964 5f61 6464  writer.extid_add
+00007cf0: 2869 6473 290a 0a20 2020 2020 2020 2064  (ids)..        d
+00007d00: 622e 636f 7079 5f74 6f28 6578 7469 642c  b.copy_to(extid,
+00007d10: 2022 746d 705f 6578 7469 6422 2c20 6462   "tmp_extid", db
+00007d20: 2e65 7874 6964 5f63 6f6c 732c 2063 7572  .extid_cols, cur
+00007d30: 290a 0a20 2020 2020 2020 2023 206d 6f76  )..        # mov
+00007d40: 6520 6d65 7461 6461 7461 2069 6e20 706c  e metadata in pl
+00007d50: 6163 650a 2020 2020 2020 2020 6462 2e65  ace.        db.e
+00007d60: 7874 6964 5f61 6464 5f66 726f 6d5f 7465  xtid_add_from_te
+00007d70: 6d70 2863 7572 290a 0a20 2020 2020 2020  mp(cur)..       
+00007d80: 2072 6574 7572 6e20 7b22 6578 7469 643a   return {"extid:
+00007d90: 6164 6422 3a20 6c65 6e28 6578 7469 6429  add": len(extid)
+00007da0: 7d0a 0a20 2020 2023 2323 2323 2323 2323  }..    #########
+00007db0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00007dc0: 230a 2020 2020 2320 5265 6c65 6173 650a  #.    # Release.
+00007dd0: 2020 2020 2323 2323 2323 2323 2323 2323      ############
+00007de0: 2323 2323 2323 2323 2323 2323 2323 0a0a  ##############..
+00007df0: 2020 2020 4064 625f 7472 616e 7361 6374      @db_transact
+00007e00: 696f 6e28 290a 2020 2020 6465 6620 7265  ion().    def re
+00007e10: 6c65 6173 655f 6164 6428 0a20 2020 2020  lease_add(.     
+00007e20: 2020 2073 656c 662c 2072 656c 6561 7365     self, release
+00007e30: 733a 204c 6973 745b 5265 6c65 6173 655d  s: List[Release]
+00007e40: 2c20 2a2c 2064 623a 2044 622c 2063 7572  , *, db: Db, cur
+00007e50: 3d4e 6f6e 650a 2020 2020 2920 2d3e 2044  =None.    ) -> D
+00007e60: 6963 745b 7374 722c 2069 6e74 5d3a 0a20  ict[str, int]:. 
+00007e70: 2020 2020 2020 2073 756d 6d61 7279 203d         summary =
+00007e80: 207b 2272 656c 6561 7365 3a61 6464 223a   {"release:add":
+00007e90: 2030 7d0a 0a20 2020 2020 2020 2072 656c   0}..        rel
+00007ea0: 6561 7365 5f69 6473 203d 2073 6574 2872  ease_ids = set(r
+00007eb0: 656c 6561 7365 2e69 6420 666f 7220 7265  elease.id for re
+00007ec0: 6c65 6173 6520 696e 2072 656c 6561 7365  lease in release
+00007ed0: 7329 0a20 2020 2020 2020 2072 656c 6561  s).        relea
+00007ee0: 7365 735f 6d69 7373 696e 6720 3d20 7365  ses_missing = se
+00007ef0: 7428 7365 6c66 2e72 656c 6561 7365 5f6d  t(self.release_m
+00007f00: 6973 7369 6e67 2872 656c 6561 7365 5f69  issing(release_i
+00007f10: 6473 2c20 6462 3d64 622c 2063 7572 3d63  ds, db=db, cur=c
+00007f20: 7572 2929 0a0a 2020 2020 2020 2020 6966  ur))..        if
+00007f30: 206e 6f74 2072 656c 6561 7365 735f 6d69   not releases_mi
+00007f40: 7373 696e 673a 0a20 2020 2020 2020 2020  ssing:.         
+00007f50: 2020 2072 6574 7572 6e20 7375 6d6d 6172     return summar
+00007f60: 790a 0a20 2020 2020 2020 2064 622e 6d6b  y..        db.mk
+00007f70: 7465 6d70 5f72 656c 6561 7365 2863 7572  temp_release(cur
+00007f80: 290a 0a20 2020 2020 2020 2072 656c 6561  )..        relea
+00007f90: 7365 735f 6669 6c74 6572 6564 203d 205b  ses_filtered = [
+00007fa0: 0a20 2020 2020 2020 2020 2020 2072 656c  .            rel
+00007fb0: 6561 7365 2066 6f72 2072 656c 6561 7365  ease for release
+00007fc0: 2069 6e20 7265 6c65 6173 6573 2069 6620   in releases if 
+00007fd0: 7265 6c65 6173 652e 6964 2069 6e20 7265  release.id in re
+00007fe0: 6c65 6173 6573 5f6d 6973 7369 6e67 0a20  leases_missing. 
+00007ff0: 2020 2020 2020 205d 0a0a 2020 2020 2020         ]..      
+00008000: 2020 7365 6c66 2e6a 6f75 726e 616c 5f77    self.journal_w
+00008010: 7269 7465 722e 7265 6c65 6173 655f 6164  riter.release_ad
+00008020: 6428 7265 6c65 6173 6573 5f66 696c 7465  d(releases_filte
+00008030: 7265 6429 0a0a 2020 2020 2020 2020 6462  red)..        db
+00008040: 5f72 656c 6561 7365 735f 6669 6c74 6572  _releases_filter
+00008050: 6564 203d 206c 6973 7428 6d61 7028 636f  ed = list(map(co
+00008060: 6e76 6572 7465 7273 2e72 656c 6561 7365  nverters.release
+00008070: 5f74 6f5f 6462 2c20 7265 6c65 6173 6573  _to_db, releases
+00008080: 5f66 696c 7465 7265 6429 290a 0a20 2020  _filtered))..   
+00008090: 2020 2020 2077 6974 6820 636f 6e76 6572       with conver
+000080a0: 745f 7661 6c69 6461 7469 6f6e 5f65 7863  t_validation_exc
+000080b0: 6570 7469 6f6e 7328 293a 0a20 2020 2020  eptions():.     
+000080c0: 2020 2020 2020 2064 622e 636f 7079 5f74         db.copy_t
+000080d0: 6f28 6462 5f72 656c 6561 7365 735f 6669  o(db_releases_fi
+000080e0: 6c74 6572 6564 2c20 2274 6d70 5f72 656c  ltered, "tmp_rel
+000080f0: 6561 7365 222c 2064 622e 7265 6c65 6173  ease", db.releas
+00008100: 655f 6164 645f 636f 6c73 2c20 6375 7229  e_add_cols, cur)
+00008110: 0a0a 2020 2020 2020 2020 2020 2020 6462  ..            db
+00008120: 2e72 656c 6561 7365 5f61 6464 5f66 726f  .release_add_fro
+00008130: 6d5f 7465 6d70 2863 7572 290a 0a20 2020  m_temp(cur)..   
+00008140: 2020 2020 2072 6574 7572 6e20 7b22 7265       return {"re
+00008150: 6c65 6173 653a 6164 6422 3a20 6c65 6e28  lease:add": len(
+00008160: 7265 6c65 6173 6573 5f6d 6973 7369 6e67  releases_missing
+00008170: 297d 0a0a 2020 2020 4064 625f 7472 616e  )}..    @db_tran
+00008180: 7361 6374 696f 6e5f 6765 6e65 7261 746f  saction_generato
+00008190: 7228 290a 2020 2020 6465 6620 7265 6c65  r().    def rele
+000081a0: 6173 655f 6d69 7373 696e 6728 0a20 2020  ase_missing(.   
+000081b0: 2020 2020 2073 656c 662c 2072 656c 6561       self, relea
+000081c0: 7365 733a 204c 6973 745b 5368 6131 4769  ses: List[Sha1Gi
+000081d0: 745d 2c20 2a2c 2064 623a 2044 622c 2063  t], *, db: Db, c
+000081e0: 7572 3d4e 6f6e 650a 2020 2020 2920 2d3e  ur=None.    ) ->
+000081f0: 2049 7465 7261 626c 655b 5368 6131 4769   Iterable[Sha1Gi
+00008200: 745d 3a0a 2020 2020 2020 2020 6966 206e  t]:.        if n
+00008210: 6f74 2072 656c 6561 7365 733a 0a20 2020  ot releases:.   
+00008220: 2020 2020 2020 2020 2072 6574 7572 6e0a           return.
+00008230: 0a20 2020 2020 2020 2066 6f72 206f 626a  .        for obj
+00008240: 2069 6e20 6462 2e72 656c 6561 7365 5f6d   in db.release_m
+00008250: 6973 7369 6e67 5f66 726f 6d5f 6c69 7374  issing_from_list
+00008260: 2872 656c 6561 7365 732c 2063 7572 293a  (releases, cur):
+00008270: 0a20 2020 2020 2020 2020 2020 2079 6965  .            yie
+00008280: 6c64 206f 626a 5b30 5d0a 0a20 2020 2040  ld obj[0]..    @
+00008290: 6462 5f74 7261 6e73 6163 7469 6f6e 2873  db_transaction(s
+000082a0: 7461 7465 6d65 6e74 5f74 696d 656f 7574  tatement_timeout
+000082b0: 3d31 3030 3029 0a20 2020 2064 6566 2072  =1000).    def r
+000082c0: 656c 6561 7365 5f67 6574 280a 2020 2020  elease_get(.    
+000082d0: 2020 2020 7365 6c66 2c0a 2020 2020 2020      self,.      
+000082e0: 2020 7265 6c65 6173 6573 3a20 4c69 7374    releases: List
+000082f0: 5b53 6861 3147 6974 5d2c 0a20 2020 2020  [Sha1Git],.     
+00008300: 2020 2069 676e 6f72 655f 6469 7370 6c61     ignore_displa
+00008310: 796e 616d 653a 2062 6f6f 6c20 3d20 4661  yname: bool = Fa
+00008320: 6c73 652c 0a20 2020 2020 2020 202a 2c0a  lse,.        *,.
+00008330: 2020 2020 2020 2020 6462 3a20 4462 2c0a          db: Db,.
+00008340: 2020 2020 2020 2020 6375 723d 4e6f 6e65          cur=None
+00008350: 2c0a 2020 2020 2920 2d3e 204c 6973 745b  ,.    ) -> List[
+00008360: 4f70 7469 6f6e 616c 5b52 656c 6561 7365  Optional[Release
+00008370: 5d5d 3a0a 2020 2020 2020 2020 7265 6c73  ]]:.        rels
+00008380: 203d 205b 5d0a 2020 2020 2020 2020 666f   = [].        fo
+00008390: 7220 7265 6c65 6173 6520 696e 2064 622e  r release in db.
+000083a0: 7265 6c65 6173 655f 6765 745f 6672 6f6d  release_get_from
+000083b0: 5f6c 6973 7428 7265 6c65 6173 6573 2c20  _list(releases, 
+000083c0: 6967 6e6f 7265 5f64 6973 706c 6179 6e61  ignore_displayna
+000083d0: 6d65 2c20 6375 7229 3a0a 2020 2020 2020  me, cur):.      
+000083e0: 2020 2020 2020 7265 6c20 3d20 636f 6e76        rel = conv
+000083f0: 6572 7465 7273 2e64 625f 746f 5f6f 7074  erters.db_to_opt
+00008400: 696f 6e61 6c5f 7265 6c65 6173 6528 0a20  ional_release(. 
+00008410: 2020 2020 2020 2020 2020 2020 2020 2064                 d
+00008420: 6963 7428 7a69 7028 6462 2e72 656c 6561  ict(zip(db.relea
+00008430: 7365 5f67 6574 5f63 6f6c 732c 2072 656c  se_get_cols, rel
+00008440: 6561 7365 2929 0a20 2020 2020 2020 2020  ease)).         
+00008450: 2020 2029 0a20 2020 2020 2020 2020 2020     ).           
+00008460: 2072 656c 732e 6170 7065 6e64 2872 656c   rels.append(rel
+00008470: 290a 2020 2020 2020 2020 7265 7475 726e  ).        return
+00008480: 2072 656c 730a 0a20 2020 2040 6462 5f74   rels..    @db_t
+00008490: 7261 6e73 6163 7469 6f6e 2829 0a20 2020  ransaction().   
+000084a0: 2064 6566 2072 656c 6561 7365 5f67 6574   def release_get
+000084b0: 5f70 6172 7469 7469 6f6e 280a 2020 2020  _partition(.    
+000084c0: 2020 2020 7365 6c66 2c0a 2020 2020 2020      self,.      
+000084d0: 2020 7061 7274 6974 696f 6e5f 6964 3a20    partition_id: 
+000084e0: 696e 742c 0a20 2020 2020 2020 206e 625f  int,.        nb_
+000084f0: 7061 7274 6974 696f 6e73 3a20 696e 742c  partitions: int,
+00008500: 0a20 2020 2020 2020 2070 6167 655f 746f  .        page_to
+00008510: 6b65 6e3a 204f 7074 696f 6e61 6c5b 7374  ken: Optional[st
+00008520: 725d 203d 204e 6f6e 652c 0a20 2020 2020  r] = None,.     
+00008530: 2020 206c 696d 6974 3a20 696e 7420 3d20     limit: int = 
+00008540: 3130 3030 2c0a 2020 2020 2020 2020 2a2c  1000,.        *,
+00008550: 0a20 2020 2020 2020 2064 623a 2044 622c  .        db: Db,
+00008560: 0a20 2020 2020 2020 2063 7572 3d4e 6f6e  .        cur=Non
+00008570: 652c 0a20 2020 2029 202d 3e20 5061 6765  e,.    ) -> Page
+00008580: 6452 6573 756c 745b 5265 6c65 6173 655d  dResult[Release]
+00008590: 3a0a 2020 2020 2020 2020 7265 7475 726e  :.        return
+000085a0: 205f 6765 745f 7061 6769 6e61 7465 645f   _get_paginated_
+000085b0: 7368 6131 5f70 6172 7469 7469 6f6e 280a  sha1_partition(.
+000085c0: 2020 2020 2020 2020 2020 2020 6375 722c              cur,
+000085d0: 0a20 2020 2020 2020 2020 2020 2070 6172  .            par
+000085e0: 7469 7469 6f6e 5f69 642c 0a20 2020 2020  tition_id,.     
+000085f0: 2020 2020 2020 206e 625f 7061 7274 6974         nb_partit
+00008600: 696f 6e73 2c0a 2020 2020 2020 2020 2020  ions,.          
+00008610: 2020 7061 6765 5f74 6f6b 656e 2c0a 2020    page_token,.  
+00008620: 2020 2020 2020 2020 2020 6c69 6d69 742c            limit,
+00008630: 0a20 2020 2020 2020 2020 2020 2064 622e  .            db.
+00008640: 7265 6c65 6173 655f 6765 745f 7261 6e67  release_get_rang
+00008650: 652c 0a20 2020 2020 2020 2020 2020 206c  e,.            l
+00008660: 616d 6264 6120 726f 773a 2063 6f6e 7665  ambda row: conve
+00008670: 7274 6572 732e 6462 5f74 6f5f 7265 6c65  rters.db_to_rele
+00008680: 6173 6528 6469 6374 287a 6970 2864 622e  ase(dict(zip(db.
+00008690: 7265 6c65 6173 655f 6765 745f 636f 6c73  release_get_cols
+000086a0: 2c20 726f 7729 2929 2c0a 2020 2020 2020  , row))),.      
+000086b0: 2020 290a 0a20 2020 2040 6462 5f74 7261    )..    @db_tra
+000086c0: 6e73 6163 7469 6f6e 2829 0a20 2020 2064  nsaction().    d
+000086d0: 6566 2072 656c 6561 7365 5f67 6574 5f72  ef release_get_r
+000086e0: 616e 646f 6d28 7365 6c66 2c20 2a2c 2064  andom(self, *, d
+000086f0: 623a 2044 622c 2063 7572 3d4e 6f6e 6529  b: Db, cur=None)
+00008700: 202d 3e20 5368 6131 4769 743a 0a20 2020   -> Sha1Git:.   
+00008710: 2020 2020 2072 6574 7572 6e20 6462 2e72       return db.r
+00008720: 656c 6561 7365 5f67 6574 5f72 616e 646f  elease_get_rando
+00008730: 6d28 6375 7229 0a0a 2020 2020 2323 2323  m(cur)..    ####
+00008740: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00008750: 2323 2323 2323 0a20 2020 2023 2053 6e61  ######.    # Sna
+00008760: 7073 686f 740a 2020 2020 2323 2323 2323  pshot.    ######
+00008770: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00008780: 2323 2323 0a0a 2020 2020 4064 625f 7472  ####..    @db_tr
+00008790: 616e 7361 6374 696f 6e28 290a 2020 2020  ansaction().    
+000087a0: 6465 6620 736e 6170 7368 6f74 5f61 6464  def snapshot_add
+000087b0: 280a 2020 2020 2020 2020 7365 6c66 2c20  (.        self, 
+000087c0: 736e 6170 7368 6f74 733a 204c 6973 745b  snapshots: List[
+000087d0: 536e 6170 7368 6f74 5d2c 202a 2c20 6462  Snapshot], *, db
+000087e0: 3a20 4462 2c20 6375 723d 4e6f 6e65 0a20  : Db, cur=None. 
+000087f0: 2020 2029 202d 3e20 4469 6374 5b73 7472     ) -> Dict[str
+00008800: 2c20 696e 745d 3a0a 2020 2020 2020 2020  , int]:.        
+00008810: 6372 6561 7465 645f 7465 6d70 5f74 6162  created_temp_tab
+00008820: 6c65 203d 2046 616c 7365 0a0a 2020 2020  le = False..    
+00008830: 2020 2020 636f 756e 7420 3d20 300a 2020      count = 0.  
+00008840: 2020 2020 2020 666f 7220 736e 6170 7368        for snapsh
+00008850: 6f74 2069 6e20 736e 6170 7368 6f74 733a  ot in snapshots:
+00008860: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
+00008870: 6e6f 7420 6462 2e73 6e61 7073 686f 745f  not db.snapshot_
+00008880: 6578 6973 7473 2873 6e61 7073 686f 742e  exists(snapshot.
+00008890: 6964 2c20 6375 7229 3a0a 2020 2020 2020  id, cur):.      
+000088a0: 2020 2020 2020 2020 2020 6966 206e 6f74            if not
+000088b0: 2063 7265 6174 6564 5f74 656d 705f 7461   created_temp_ta
+000088c0: 626c 653a 0a20 2020 2020 2020 2020 2020  ble:.           
+000088d0: 2020 2020 2020 2020 2064 622e 6d6b 7465           db.mkte
+000088e0: 6d70 5f73 6e61 7073 686f 745f 6272 616e  mp_snapshot_bran
+000088f0: 6368 2863 7572 290a 2020 2020 2020 2020  ch(cur).        
+00008900: 2020 2020 2020 2020 2020 2020 6372 6561              crea
+00008910: 7465 645f 7465 6d70 5f74 6162 6c65 203d  ted_temp_table =
+00008920: 2054 7275 650a 0a20 2020 2020 2020 2020   True..         
+00008930: 2020 2020 2020 2077 6974 6820 636f 6e76         with conv
+00008940: 6572 745f 7661 6c69 6461 7469 6f6e 5f65  ert_validation_e
+00008950: 7863 6570 7469 6f6e 7328 293a 0a20 2020  xceptions():.   
 00008960: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008970: 2274 6172 6765 7422 3a20 696e 666f 2e74  "target": info.t
-00008980: 6172 6765 7420 6966 2069 6e66 6f20 656c  arget if info el
-00008990: 7365 204e 6f6e 652c 0a20 2020 2020 2020  se None,.       
+00008970: 2064 622e 636f 7079 5f74 6f28 0a20 2020   db.copy_to(.   
+00008980: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008990: 2020 2020 2028 0a20 2020 2020 2020 2020       (.         
 000089a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000089b0: 2020 2020 2020 2020 2022 7461 7267 6574           "target
-000089c0: 5f74 7970 6522 3a20 280a 2020 2020 2020  _type": (.      
-000089d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000089e0: 2020 2020 2020 2020 2020 2020 2020 696e                in
-000089f0: 666f 2e74 6172 6765 745f 7479 7065 2e76  fo.target_type.v
-00008a00: 616c 7565 2069 6620 696e 666f 2065 6c73  alue if info els
-00008a10: 6520 4e6f 6e65 0a20 2020 2020 2020 2020  e None.         
-00008a20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008a30: 2020 2020 2020 2029 2c0a 2020 2020 2020         ),.      
-00008a40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008a50: 2020 2020 2020 7d0a 2020 2020 2020 2020        }.        
+000089b0: 2020 207b 0a20 2020 2020 2020 2020 2020     {.           
+000089c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000089d0: 2020 2020 2022 6e61 6d65 223a 206e 616d       "name": nam
+000089e0: 652c 0a20 2020 2020 2020 2020 2020 2020  e,.             
+000089f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008a00: 2020 2022 7461 7267 6574 223a 2069 6e66     "target": inf
+00008a10: 6f2e 7461 7267 6574 2069 6620 696e 666f  o.target if info
+00008a20: 2065 6c73 6520 4e6f 6e65 2c0a 2020 2020   else None,.    
+00008a30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008a40: 2020 2020 2020 2020 2020 2020 2274 6172              "tar
+00008a50: 6765 745f 7479 7065 223a 2028 0a20 2020  get_type": (.   
 00008a60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008a70: 2020 2020 666f 7220 6e61 6d65 2c20 696e      for name, in
-00008a80: 666f 2069 6e20 736e 6170 7368 6f74 2e62  fo in snapshot.b
-00008a90: 7261 6e63 6865 732e 6974 656d 7328 290a  ranches.items().
-00008aa0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008ab0: 2020 2020 2020 2020 292c 0a20 2020 2020          ),.     
-00008ac0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008ad0: 2020 2022 746d 705f 736e 6170 7368 6f74     "tmp_snapshot
-00008ae0: 5f62 7261 6e63 6822 2c0a 2020 2020 2020  _branch",.      
+00008a70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008a80: 2069 6e66 6f2e 7461 7267 6574 5f74 7970   info.target_typ
+00008a90: 652e 7661 6c75 6520 6966 2069 6e66 6f20  e.value if info 
+00008aa0: 656c 7365 204e 6f6e 650a 2020 2020 2020  else None.      
+00008ab0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008ac0: 2020 2020 2020 2020 2020 292c 0a20 2020            ),.   
+00008ad0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008ae0: 2020 2020 2020 2020 207d 0a20 2020 2020           }.     
 00008af0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008b00: 2020 5b22 6e61 6d65 222c 2022 7461 7267    ["name", "targ
-00008b10: 6574 222c 2022 7461 7267 6574 5f74 7970  et", "target_typ
-00008b20: 6522 5d2c 0a20 2020 2020 2020 2020 2020  e"],.           
-00008b30: 2020 2020 2020 2020 2020 2020 2063 7572               cur
-00008b40: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-00008b50: 2020 2020 2020 290a 0a20 2020 2020 2020        )..       
-00008b60: 2020 2020 2020 2020 2073 656c 662e 6a6f           self.jo
-00008b70: 7572 6e61 6c5f 7772 6974 6572 2e73 6e61  urnal_writer.sna
-00008b80: 7073 686f 745f 6164 6428 5b73 6e61 7073  pshot_add([snaps
-00008b90: 686f 745d 290a 0a20 2020 2020 2020 2020  hot])..         
-00008ba0: 2020 2020 2020 2064 622e 736e 6170 7368         db.snapsh
-00008bb0: 6f74 5f61 6464 2873 6e61 7073 686f 742e  ot_add(snapshot.
-00008bc0: 6964 2c20 6375 7229 0a20 2020 2020 2020  id, cur).       
-00008bd0: 2020 2020 2020 2020 2063 6f75 6e74 202b           count +
-00008be0: 3d20 310a 0a20 2020 2020 2020 2072 6574  = 1..        ret
-00008bf0: 7572 6e20 7b22 736e 6170 7368 6f74 3a61  urn {"snapshot:a
-00008c00: 6464 223a 2063 6f75 6e74 7d0a 0a20 2020  dd": count}..   
-00008c10: 2040 6462 5f74 7261 6e73 6163 7469 6f6e   @db_transaction
-00008c20: 5f67 656e 6572 6174 6f72 2829 0a20 2020  _generator().   
-00008c30: 2064 6566 2073 6e61 7073 686f 745f 6d69   def snapshot_mi
-00008c40: 7373 696e 6728 0a20 2020 2020 2020 2073  ssing(.        s
-00008c50: 656c 662c 2073 6e61 7073 686f 7473 3a20  elf, snapshots: 
-00008c60: 4c69 7374 5b53 6861 3147 6974 5d2c 202a  List[Sha1Git], *
-00008c70: 2c20 6462 3a20 4462 2c20 6375 723d 4e6f  , db: Db, cur=No
-00008c80: 6e65 0a20 2020 2029 202d 3e20 4974 6572  ne.    ) -> Iter
-00008c90: 6162 6c65 5b53 6861 3147 6974 5d3a 0a20  able[Sha1Git]:. 
-00008ca0: 2020 2020 2020 2066 6f72 206f 626a 2069         for obj i
-00008cb0: 6e20 6462 2e73 6e61 7073 686f 745f 6d69  n db.snapshot_mi
-00008cc0: 7373 696e 675f 6672 6f6d 5f6c 6973 7428  ssing_from_list(
-00008cd0: 736e 6170 7368 6f74 732c 2063 7572 293a  snapshots, cur):
-00008ce0: 0a20 2020 2020 2020 2020 2020 2079 6965  .            yie
-00008cf0: 6c64 206f 626a 5b30 5d0a 0a20 2020 2040  ld obj[0]..    @
-00008d00: 6462 5f74 7261 6e73 6163 7469 6f6e 2873  db_transaction(s
-00008d10: 7461 7465 6d65 6e74 5f74 696d 656f 7574  tatement_timeout
-00008d20: 3d32 3030 3029 0a20 2020 2064 6566 2073  =2000).    def s
-00008d30: 6e61 7073 686f 745f 6765 7428 0a20 2020  napshot_get(.   
-00008d40: 2020 2020 2073 656c 662c 2073 6e61 7073       self, snaps
-00008d50: 686f 745f 6964 3a20 5368 6131 4769 742c  hot_id: Sha1Git,
-00008d60: 202a 2c20 6462 3a20 4462 2c20 6375 723d   *, db: Db, cur=
-00008d70: 4e6f 6e65 0a20 2020 2029 202d 3e20 4f70  None.    ) -> Op
-00008d80: 7469 6f6e 616c 5b44 6963 745b 7374 722c  tional[Dict[str,
-00008d90: 2041 6e79 5d5d 3a0a 2020 2020 2020 2020   Any]]:.        
-00008da0: 6420 3d20 7365 6c66 2e73 6e61 7073 686f  d = self.snapsho
-00008db0: 745f 6765 745f 6272 616e 6368 6573 2873  t_get_branches(s
-00008dc0: 6e61 7073 686f 745f 6964 290a 2020 2020  napshot_id).    
-00008dd0: 2020 2020 6966 2064 2069 7320 4e6f 6e65      if d is None
-00008de0: 3a0a 2020 2020 2020 2020 2020 2020 7265  :.            re
-00008df0: 7475 726e 2064 0a20 2020 2020 2020 2072  turn d.        r
-00008e00: 6574 7572 6e20 7b0a 2020 2020 2020 2020  eturn {.        
-00008e10: 2020 2020 2269 6422 3a20 645b 2269 6422      "id": d["id"
-00008e20: 5d2c 0a20 2020 2020 2020 2020 2020 2022  ],.            "
-00008e30: 6272 616e 6368 6573 223a 207b 0a20 2020  branches": {.   
-00008e40: 2020 2020 2020 2020 2020 2020 206e 616d               nam
-00008e50: 653a 2062 7261 6e63 682e 746f 5f64 6963  e: branch.to_dic
-00008e60: 7428 2920 6966 2062 7261 6e63 6820 656c  t() if branch el
-00008e70: 7365 204e 6f6e 650a 2020 2020 2020 2020  se None.        
-00008e80: 2020 2020 2020 2020 666f 7220 286e 616d          for (nam
-00008e90: 652c 2062 7261 6e63 6829 2069 6e20 645b  e, branch) in d[
-00008ea0: 2262 7261 6e63 6865 7322 5d2e 6974 656d  "branches"].item
-00008eb0: 7328 290a 2020 2020 2020 2020 2020 2020  s().            
-00008ec0: 7d2c 0a20 2020 2020 2020 2020 2020 2022  },.            "
-00008ed0: 6e65 7874 5f62 7261 6e63 6822 3a20 645b  next_branch": d[
-00008ee0: 226e 6578 745f 6272 616e 6368 225d 2c0a  "next_branch"],.
-00008ef0: 2020 2020 2020 2020 7d0a 0a20 2020 2040          }..    @
-00008f00: 6462 5f74 7261 6e73 6163 7469 6f6e 2829  db_transaction()
-00008f10: 0a20 2020 2064 6566 2073 6e61 7073 686f  .    def snapsho
-00008f20: 745f 6765 745f 6964 5f70 6172 7469 7469  t_get_id_partiti
-00008f30: 6f6e 280a 2020 2020 2020 2020 7365 6c66  on(.        self
-00008f40: 2c0a 2020 2020 2020 2020 7061 7274 6974  ,.        partit
-00008f50: 696f 6e5f 6964 3a20 696e 742c 0a20 2020  ion_id: int,.   
-00008f60: 2020 2020 206e 625f 7061 7274 6974 696f       nb_partitio
-00008f70: 6e73 3a20 696e 742c 0a20 2020 2020 2020  ns: int,.       
-00008f80: 2070 6167 655f 746f 6b65 6e3a 204f 7074   page_token: Opt
-00008f90: 696f 6e61 6c5b 7374 725d 203d 204e 6f6e  ional[str] = Non
-00008fa0: 652c 0a20 2020 2020 2020 206c 696d 6974  e,.        limit
-00008fb0: 3a20 696e 7420 3d20 3130 3030 2c0a 2020  : int = 1000,.  
-00008fc0: 2020 2020 2020 2a2c 0a20 2020 2020 2020        *,.       
-00008fd0: 2064 623a 2044 622c 0a20 2020 2020 2020   db: Db,.       
-00008fe0: 2063 7572 3d4e 6f6e 652c 0a20 2020 2029   cur=None,.    )
-00008ff0: 202d 3e20 5061 6765 6452 6573 756c 745b   -> PagedResult[
-00009000: 5368 6131 4769 745d 3a0a 2020 2020 2020  Sha1Git]:.      
-00009010: 2020 7265 7475 726e 205f 6765 745f 7061    return _get_pa
-00009020: 6769 6e61 7465 645f 7368 6131 5f70 6172  ginated_sha1_par
-00009030: 7469 7469 6f6e 280a 2020 2020 2020 2020  tition(.        
-00009040: 2020 2020 6375 722c 0a20 2020 2020 2020      cur,.       
-00009050: 2020 2020 2070 6172 7469 7469 6f6e 5f69       partition_i
-00009060: 642c 0a20 2020 2020 2020 2020 2020 206e  d,.            n
-00009070: 625f 7061 7274 6974 696f 6e73 2c0a 2020  b_partitions,.  
-00009080: 2020 2020 2020 2020 2020 7061 6765 5f74            page_t
-00009090: 6f6b 656e 2c0a 2020 2020 2020 2020 2020  oken,.          
-000090a0: 2020 6c69 6d69 742c 0a20 2020 2020 2020    limit,.       
-000090b0: 2020 2020 2064 622e 736e 6170 7368 6f74       db.snapshot
-000090c0: 5f67 6574 5f69 645f 7261 6e67 652c 0a20  _get_id_range,. 
-000090d0: 2020 2020 2020 2020 2020 206f 7065 7261             opera
-000090e0: 746f 722e 6974 656d 6765 7474 6572 2830  tor.itemgetter(0
-000090f0: 292c 0a20 2020 2020 2020 2020 2020 206c  ),.            l
-00009100: 616d 6264 6120 6964 5f3a 2069 645f 2c0a  ambda id_: id_,.
-00009110: 2020 2020 2020 2020 290a 0a20 2020 2040          )..    @
-00009120: 6462 5f74 7261 6e73 6163 7469 6f6e 2873  db_transaction(s
-00009130: 7461 7465 6d65 6e74 5f74 696d 656f 7574  tatement_timeout
-00009140: 3d32 3030 3029 0a20 2020 2064 6566 2073  =2000).    def s
-00009150: 6e61 7073 686f 745f 636f 756e 745f 6272  napshot_count_br
-00009160: 616e 6368 6573 280a 2020 2020 2020 2020  anches(.        
-00009170: 7365 6c66 2c0a 2020 2020 2020 2020 736e  self,.        sn
-00009180: 6170 7368 6f74 5f69 643a 2053 6861 3147  apshot_id: Sha1G
-00009190: 6974 2c0a 2020 2020 2020 2020 6272 616e  it,.        bran
-000091a0: 6368 5f6e 616d 655f 6578 636c 7564 655f  ch_name_exclude_
-000091b0: 7072 6566 6978 3a20 4f70 7469 6f6e 616c  prefix: Optional
-000091c0: 5b62 7974 6573 5d20 3d20 4e6f 6e65 2c0a  [bytes] = None,.
-000091d0: 2020 2020 2020 2020 2a2c 0a20 2020 2020          *,.     
-000091e0: 2020 2064 623a 2044 622c 0a20 2020 2020     db: Db,.     
-000091f0: 2020 2063 7572 3d4e 6f6e 652c 0a20 2020     cur=None,.   
-00009200: 2029 202d 3e20 4f70 7469 6f6e 616c 5b44   ) -> Optional[D
-00009210: 6963 745b 4f70 7469 6f6e 616c 5b73 7472  ict[Optional[str
-00009220: 5d2c 2069 6e74 5d5d 3a0a 2020 2020 2020  ], int]]:.      
-00009230: 2020 7265 7475 726e 2064 6963 7428 0a20    return dict(. 
-00009240: 2020 2020 2020 2020 2020 205b 0a20 2020             [.   
-00009250: 2020 2020 2020 2020 2020 2020 2062 630a               bc.
-00009260: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009270: 666f 7220 6263 2069 6e20 6462 2e73 6e61  for bc in db.sna
-00009280: 7073 686f 745f 636f 756e 745f 6272 616e  pshot_count_bran
-00009290: 6368 6573 280a 2020 2020 2020 2020 2020  ches(.          
-000092a0: 2020 2020 2020 2020 2020 736e 6170 7368            snapsh
-000092b0: 6f74 5f69 642c 0a20 2020 2020 2020 2020  ot_id,.         
-000092c0: 2020 2020 2020 2020 2020 2062 7261 6e63             branc
-000092d0: 685f 6e61 6d65 5f65 7863 6c75 6465 5f70  h_name_exclude_p
-000092e0: 7265 6669 782c 0a20 2020 2020 2020 2020  refix,.         
-000092f0: 2020 2020 2020 2020 2020 2063 7572 2c0a             cur,.
-00009300: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009310: 290a 2020 2020 2020 2020 2020 2020 5d0a  ).            ].
-00009320: 2020 2020 2020 2020 290a 0a20 2020 2040          )..    @
-00009330: 6462 5f74 7261 6e73 6163 7469 6f6e 2873  db_transaction(s
-00009340: 7461 7465 6d65 6e74 5f74 696d 656f 7574  tatement_timeout
-00009350: 3d32 3030 3029 0a20 2020 2064 6566 2073  =2000).    def s
-00009360: 6e61 7073 686f 745f 6765 745f 6272 616e  napshot_get_bran
-00009370: 6368 6573 280a 2020 2020 2020 2020 7365  ches(.        se
-00009380: 6c66 2c0a 2020 2020 2020 2020 736e 6170  lf,.        snap
-00009390: 7368 6f74 5f69 643a 2053 6861 3147 6974  shot_id: Sha1Git
-000093a0: 2c0a 2020 2020 2020 2020 6272 616e 6368  ,.        branch
-000093b0: 6573 5f66 726f 6d3a 2062 7974 6573 203d  es_from: bytes =
-000093c0: 2062 2222 2c0a 2020 2020 2020 2020 6272   b"",.        br
-000093d0: 616e 6368 6573 5f63 6f75 6e74 3a20 696e  anches_count: in
-000093e0: 7420 3d20 3130 3030 2c0a 2020 2020 2020  t = 1000,.      
-000093f0: 2020 7461 7267 6574 5f74 7970 6573 3a20    target_types: 
-00009400: 4f70 7469 6f6e 616c 5b4c 6973 745b 7374  Optional[List[st
-00009410: 725d 5d20 3d20 4e6f 6e65 2c0a 2020 2020  r]] = None,.    
-00009420: 2020 2020 6272 616e 6368 5f6e 616d 655f      branch_name_
-00009430: 696e 636c 7564 655f 7375 6273 7472 696e  include_substrin
-00009440: 673a 204f 7074 696f 6e61 6c5b 6279 7465  g: Optional[byte
-00009450: 735d 203d 204e 6f6e 652c 0a20 2020 2020  s] = None,.     
-00009460: 2020 2062 7261 6e63 685f 6e61 6d65 5f65     branch_name_e
-00009470: 7863 6c75 6465 5f70 7265 6669 783a 204f  xclude_prefix: O
-00009480: 7074 696f 6e61 6c5b 6279 7465 735d 203d  ptional[bytes] =
-00009490: 204e 6f6e 652c 0a20 2020 2020 2020 202a   None,.        *
-000094a0: 2c0a 2020 2020 2020 2020 6462 3a20 4462  ,.        db: Db
-000094b0: 2c0a 2020 2020 2020 2020 6375 723d 4e6f  ,.        cur=No
-000094c0: 6e65 2c0a 2020 2020 2920 2d3e 204f 7074  ne,.    ) -> Opt
-000094d0: 696f 6e61 6c5b 5061 7274 6961 6c42 7261  ional[PartialBra
-000094e0: 6e63 6865 735d 3a0a 2020 2020 2020 2020  nches]:.        
-000094f0: 6966 2073 6e61 7073 686f 745f 6964 203d  if snapshot_id =
-00009500: 3d20 454d 5054 595f 534e 4150 5348 4f54  = EMPTY_SNAPSHOT
-00009510: 5f49 443a 0a20 2020 2020 2020 2020 2020  _ID:.           
-00009520: 2072 6574 7572 6e20 5061 7274 6961 6c42   return PartialB
-00009530: 7261 6e63 6865 7328 0a20 2020 2020 2020  ranches(.       
-00009540: 2020 2020 2020 2020 2069 643d 736e 6170           id=snap
-00009550: 7368 6f74 5f69 642c 0a20 2020 2020 2020  shot_id,.       
-00009560: 2020 2020 2020 2020 2062 7261 6e63 6865           branche
-00009570: 733d 7b7d 2c0a 2020 2020 2020 2020 2020  s={},.          
-00009580: 2020 2020 2020 6e65 7874 5f62 7261 6e63        next_branc
-00009590: 683d 4e6f 6e65 2c0a 2020 2020 2020 2020  h=None,.        
-000095a0: 2020 2020 290a 0a20 2020 2020 2020 2069      )..        i
-000095b0: 6620 6c69 7374 2873 656c 662e 736e 6170  f list(self.snap
-000095c0: 7368 6f74 5f6d 6973 7369 6e67 285b 736e  shot_missing([sn
-000095d0: 6170 7368 6f74 5f69 645d 2929 3a0a 2020  apshot_id])):.  
-000095e0: 2020 2020 2020 2020 2020 7265 7475 726e            return
-000095f0: 204e 6f6e 650a 0a20 2020 2020 2020 2062   None..        b
-00009600: 7261 6e63 6865 7320 3d20 7b7d 0a20 2020  ranches = {}.   
-00009610: 2020 2020 206e 6578 745f 6272 616e 6368       next_branch
-00009620: 203d 204e 6f6e 650a 0a20 2020 2020 2020   = None..       
-00009630: 2066 6574 6368 6564 5f62 7261 6e63 6865   fetched_branche
-00009640: 7320 3d20 6c69 7374 280a 2020 2020 2020  s = list(.      
-00009650: 2020 2020 2020 6462 2e73 6e61 7073 686f        db.snapsho
-00009660: 745f 6765 745f 6279 5f69 6428 0a20 2020  t_get_by_id(.   
-00009670: 2020 2020 2020 2020 2020 2020 2073 6e61               sna
-00009680: 7073 686f 745f 6964 2c0a 2020 2020 2020  pshot_id,.      
-00009690: 2020 2020 2020 2020 2020 6272 616e 6368            branch
-000096a0: 6573 5f66 726f 6d3d 6272 616e 6368 6573  es_from=branches
-000096b0: 5f66 726f 6d2c 0a20 2020 2020 2020 2020  _from,.         
-000096c0: 2020 2020 2020 2023 2074 6865 2075 6e64         # the und
-000096d0: 6572 6c79 696e 6720 5351 4c20 7175 6572  erlying SQL quer
-000096e0: 7920 6361 6e20 6265 2071 7569 7465 2065  y can be quite e
-000096f0: 7870 656e 7369 7665 2074 6f20 6578 6563  xpensive to exec
-00009700: 7574 6520 666f 7220 736d 616c 6c0a 2020  ute for small.  
-00009710: 2020 2020 2020 2020 2020 2020 2020 2320                # 
-00009720: 6272 616e 6368 6573 5f63 6f75 6e74 2076  branches_count v
-00009730: 616c 7565 2c20 736f 2077 6520 656e 7375  alue, so we ensu
-00009740: 7265 2061 206d 696e 696d 756d 2062 7261  re a minimum bra
-00009750: 6e63 6865 7320 6c69 6d69 7420 6f66 2031  nches limit of 1
-00009760: 3020 666f 720a 2020 2020 2020 2020 2020  0 for.          
-00009770: 2020 2020 2020 2320 6f70 7469 6d61 6c20        # optimal 
-00009780: 7065 7266 6f72 6d61 6e63 6573 0a20 2020  performances.   
-00009790: 2020 2020 2020 2020 2020 2020 2062 7261               bra
-000097a0: 6e63 6865 735f 636f 756e 743d 6d61 7828  nches_count=max(
-000097b0: 6272 616e 6368 6573 5f63 6f75 6e74 202b  branches_count +
-000097c0: 2031 2c20 3130 292c 0a20 2020 2020 2020   1, 10),.       
-000097d0: 2020 2020 2020 2020 2074 6172 6765 745f           target_
-000097e0: 7479 7065 733d 7461 7267 6574 5f74 7970  types=target_typ
-000097f0: 6573 2c0a 2020 2020 2020 2020 2020 2020  es,.            
-00009800: 2020 2020 6272 616e 6368 5f6e 616d 655f      branch_name_
-00009810: 696e 636c 7564 655f 7375 6273 7472 696e  include_substrin
-00009820: 673d 6272 616e 6368 5f6e 616d 655f 696e  g=branch_name_in
-00009830: 636c 7564 655f 7375 6273 7472 696e 672c  clude_substring,
-00009840: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00009850: 2062 7261 6e63 685f 6e61 6d65 5f65 7863   branch_name_exc
-00009860: 6c75 6465 5f70 7265 6669 783d 6272 616e  lude_prefix=bran
-00009870: 6368 5f6e 616d 655f 6578 636c 7564 655f  ch_name_exclude_
-00009880: 7072 6566 6978 2c0a 2020 2020 2020 2020  prefix,.        
-00009890: 2020 2020 2020 2020 6375 723d 6375 722c          cur=cur,
-000098a0: 0a20 2020 2020 2020 2020 2020 2029 0a20  .            ). 
-000098b0: 2020 2020 2020 2029 0a20 2020 2020 2020         ).       
-000098c0: 2066 6f72 2072 6f77 2069 6e20 6665 7463   for row in fetc
-000098d0: 6865 645f 6272 616e 6368 6573 5b3a 6272  hed_branches[:br
-000098e0: 616e 6368 6573 5f63 6f75 6e74 5d3a 0a20  anches_count]:. 
-000098f0: 2020 2020 2020 2020 2020 2062 7261 6e63             branc
-00009900: 685f 6420 3d20 6469 6374 287a 6970 2864  h_d = dict(zip(d
-00009910: 622e 736e 6170 7368 6f74 5f67 6574 5f63  b.snapshot_get_c
-00009920: 6f6c 732c 2072 6f77 2929 0a20 2020 2020  ols, row)).     
-00009930: 2020 2020 2020 2064 656c 2062 7261 6e63         del branc
-00009940: 685f 645b 2273 6e61 7073 686f 745f 6964  h_d["snapshot_id
-00009950: 225d 0a20 2020 2020 2020 2020 2020 206e  "].            n
-00009960: 616d 6520 3d20 6272 616e 6368 5f64 2e70  ame = branch_d.p
-00009970: 6f70 2822 6e61 6d65 2229 0a20 2020 2020  op("name").     
-00009980: 2020 2020 2020 2069 6620 6272 616e 6368         if branch
-00009990: 5f64 5b22 7461 7267 6574 225d 2069 7320  _d["target"] is 
-000099a0: 4e6f 6e65 2061 6e64 2062 7261 6e63 685f  None and branch_
-000099b0: 645b 2274 6172 6765 745f 7479 7065 225d  d["target_type"]
-000099c0: 2069 7320 4e6f 6e65 3a0a 2020 2020 2020   is None:.      
-000099d0: 2020 2020 2020 2020 2020 6272 616e 6368            branch
-000099e0: 203d 204e 6f6e 650a 2020 2020 2020 2020   = None.        
-000099f0: 2020 2020 656c 7365 3a0a 2020 2020 2020      else:.      
-00009a00: 2020 2020 2020 2020 2020 6173 7365 7274            assert
-00009a10: 2062 7261 6e63 685f 645b 2274 6172 6765   branch_d["targe
-00009a20: 745f 7479 7065 225d 2069 7320 6e6f 7420  t_type"] is not 
-00009a30: 4e6f 6e65 0a20 2020 2020 2020 2020 2020  None.           
-00009a40: 2020 2020 2062 7261 6e63 6820 3d20 536e       branch = Sn
-00009a50: 6170 7368 6f74 4272 616e 6368 280a 2020  apshotBranch(.  
-00009a60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009a70: 2020 7461 7267 6574 3d62 7261 6e63 685f    target=branch_
-00009a80: 645b 2274 6172 6765 7422 5d2c 0a20 2020  d["target"],.   
-00009a90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009aa0: 2074 6172 6765 745f 7479 7065 3d53 6e61   target_type=Sna
-00009ab0: 7073 686f 7454 6172 6765 7454 7970 6528  pshotTargetType(
-00009ac0: 6272 616e 6368 5f64 5b22 7461 7267 6574  branch_d["target
-00009ad0: 5f74 7970 6522 5d29 2c0a 2020 2020 2020  _type"]),.      
-00009ae0: 2020 2020 2020 2020 2020 290a 2020 2020            ).    
-00009af0: 2020 2020 2020 2020 6272 616e 6368 6573          branches
-00009b00: 5b6e 616d 655d 203d 2062 7261 6e63 680a  [name] = branch.
-00009b10: 0a20 2020 2020 2020 2069 6620 6c65 6e28  .        if len(
-00009b20: 6665 7463 6865 645f 6272 616e 6368 6573  fetched_branches
-00009b30: 2920 3e20 6272 616e 6368 6573 5f63 6f75  ) > branches_cou
-00009b40: 6e74 3a0a 2020 2020 2020 2020 2020 2020  nt:.            
-00009b50: 6e65 7874 5f62 7261 6e63 6820 3d20 6469  next_branch = di
-00009b60: 6374 280a 2020 2020 2020 2020 2020 2020  ct(.            
-00009b70: 2020 2020 7a69 7028 6462 2e73 6e61 7073      zip(db.snaps
-00009b80: 686f 745f 6765 745f 636f 6c73 2c20 6665  hot_get_cols, fe
-00009b90: 7463 6865 645f 6272 616e 6368 6573 5b62  tched_branches[b
-00009ba0: 7261 6e63 6865 735f 636f 756e 745d 290a  ranches_count]).
-00009bb0: 2020 2020 2020 2020 2020 2020 295b 226e              )["n
-00009bc0: 616d 6522 5d0a 0a20 2020 2020 2020 2072  ame"]..        r
-00009bd0: 6574 7572 6e20 5061 7274 6961 6c42 7261  eturn PartialBra
-00009be0: 6e63 6865 7328 0a20 2020 2020 2020 2020  nches(.         
-00009bf0: 2020 2069 643d 736e 6170 7368 6f74 5f69     id=snapshot_i
-00009c00: 642c 0a20 2020 2020 2020 2020 2020 2062  d,.            b
-00009c10: 7261 6e63 6865 733d 6272 616e 6368 6573  ranches=branches
-00009c20: 2c0a 2020 2020 2020 2020 2020 2020 6e65  ,.            ne
-00009c30: 7874 5f62 7261 6e63 683d 6e65 7874 5f62  xt_branch=next_b
-00009c40: 7261 6e63 682c 0a20 2020 2020 2020 2029  ranch,.        )
-00009c50: 0a0a 2020 2020 4064 625f 7472 616e 7361  ..    @db_transa
-00009c60: 6374 696f 6e28 290a 2020 2020 6465 6620  ction().    def 
-00009c70: 736e 6170 7368 6f74 5f67 6574 5f72 616e  snapshot_get_ran
-00009c80: 646f 6d28 7365 6c66 2c20 2a2c 2064 623a  dom(self, *, db:
-00009c90: 2044 622c 2063 7572 3d4e 6f6e 6529 202d   Db, cur=None) -
-00009ca0: 3e20 5368 6131 4769 743a 0a20 2020 2020  > Sha1Git:.     
-00009cb0: 2020 2072 6574 7572 6e20 6462 2e73 6e61     return db.sna
-00009cc0: 7073 686f 745f 6765 745f 7261 6e64 6f6d  pshot_get_random
-00009cd0: 2863 7572 290a 0a20 2020 2040 6462 5f74  (cur)..    @db_t
-00009ce0: 7261 6e73 6163 7469 6f6e 2873 7461 7465  ransaction(state
-00009cf0: 6d65 6e74 5f74 696d 656f 7574 3d32 3030  ment_timeout=200
-00009d00: 3029 0a20 2020 2064 6566 2073 6e61 7073  0).    def snaps
-00009d10: 686f 745f 6272 616e 6368 5f67 6574 5f62  hot_branch_get_b
-00009d20: 795f 6e61 6d65 280a 2020 2020 2020 2020  y_name(.        
-00009d30: 7365 6c66 2c0a 2020 2020 2020 2020 736e  self,.        sn
-00009d40: 6170 7368 6f74 5f69 643a 2053 6861 3147  apshot_id: Sha1G
-00009d50: 6974 2c0a 2020 2020 2020 2020 6272 616e  it,.        bran
-00009d60: 6368 5f6e 616d 653a 2062 7974 6573 2c0a  ch_name: bytes,.
-00009d70: 2020 2020 2020 2020 6462 3a20 4462 2c0a          db: Db,.
-00009d80: 2020 2020 2020 2020 6375 723d 4e6f 6e65          cur=None
-00009d90: 2c0a 2020 2020 2020 2020 666f 6c6c 6f77  ,.        follow
-00009da0: 5f61 6c69 6173 5f63 6861 696e 3a20 626f  _alias_chain: bo
-00009db0: 6f6c 203d 2054 7275 652c 0a20 2020 2020  ol = True,.     
-00009dc0: 2020 206d 6178 5f61 6c69 6173 5f63 6861     max_alias_cha
-00009dd0: 696e 5f6c 656e 6774 683a 2069 6e74 203d  in_length: int =
-00009de0: 2031 3030 2c0a 2020 2020 2920 2d3e 204f   100,.    ) -> O
-00009df0: 7074 696f 6e61 6c5b 536e 6170 7368 6f74  ptional[Snapshot
-00009e00: 4272 616e 6368 4279 4e61 6d65 5265 7370  BranchByNameResp
-00009e10: 6f6e 7365 5d3a 0a20 2020 2020 2020 2069  onse]:.        i
-00009e20: 6620 6c69 7374 2873 656c 662e 736e 6170  f list(self.snap
-00009e30: 7368 6f74 5f6d 6973 7369 6e67 285b 736e  shot_missing([sn
-00009e40: 6170 7368 6f74 5f69 645d 2929 3a0a 2020  apshot_id])):.  
-00009e50: 2020 2020 2020 2020 2020 7265 7475 726e            return
-00009e60: 204e 6f6e 650a 0a20 2020 2020 2020 2069   None..        i
-00009e70: 6620 736e 6170 7368 6f74 5f69 6420 3d3d  f snapshot_id ==
-00009e80: 2045 4d50 5459 5f53 4e41 5053 484f 545f   EMPTY_SNAPSHOT_
-00009e90: 4944 3a0a 2020 2020 2020 2020 2020 2020  ID:.            
-00009ea0: 7265 7475 726e 2053 6e61 7073 686f 7442  return SnapshotB
-00009eb0: 7261 6e63 6842 794e 616d 6552 6573 706f  ranchByNameRespo
-00009ec0: 6e73 6528 0a20 2020 2020 2020 2020 2020  nse(.           
-00009ed0: 2020 2020 2062 7261 6e63 685f 666f 756e       branch_foun
-00009ee0: 643d 4661 6c73 652c 0a20 2020 2020 2020  d=False,.       
-00009ef0: 2020 2020 2020 2020 2074 6172 6765 743d           target=
-00009f00: 4e6f 6e65 2c0a 2020 2020 2020 2020 2020  None,.          
-00009f10: 2020 2020 2020 616c 6961 7365 735f 666f        aliases_fo
-00009f20: 6c6c 6f77 6564 3d5b 5d2c 0a20 2020 2020  llowed=[],.     
-00009f30: 2020 2020 2020 2029 0a0a 2020 2020 2020         )..      
-00009f40: 2020 636f 6c73 5f74 6f5f 6665 7463 6820    cols_to_fetch 
-00009f50: 3d20 5b22 7461 7267 6574 222c 2022 7461  = ["target", "ta
-00009f60: 7267 6574 5f74 7970 6522 5d0a 2020 2020  rget_type"].    
-00009f70: 2020 2020 7265 736f 6c76 655f 6368 6169      resolve_chai
-00009f80: 6e3a 204c 6973 745b 6279 7465 735d 203d  n: List[bytes] =
-00009f90: 205b 5d0a 2020 2020 2020 2020 7768 696c   [].        whil
-00009fa0: 6520 5472 7565 3a0a 2020 2020 2020 2020  e True:.        
-00009fb0: 2020 2020 6272 616e 6368 203d 2064 622e      branch = db.
-00009fc0: 736e 6170 7368 6f74 5f62 7261 6e63 685f  snapshot_branch_
-00009fd0: 6765 745f 6279 5f6e 616d 6528 0a20 2020  get_by_name(.   
-00009fe0: 2020 2020 2020 2020 2020 2020 2063 6f6c               col
-00009ff0: 735f 746f 5f66 6574 6368 3d63 6f6c 735f  s_to_fetch=cols_
-0000a000: 746f 5f66 6574 6368 2c0a 2020 2020 2020  to_fetch,.      
-0000a010: 2020 2020 2020 2020 2020 736e 6170 7368            snapsh
-0000a020: 6f74 5f69 643d 736e 6170 7368 6f74 5f69  ot_id=snapshot_i
-0000a030: 642c 0a20 2020 2020 2020 2020 2020 2020  d,.             
-0000a040: 2020 2062 7261 6e63 685f 6e61 6d65 3d62     branch_name=b
-0000a050: 7261 6e63 685f 6e61 6d65 2c0a 2020 2020  ranch_name,.    
-0000a060: 2020 2020 2020 2020 2020 2020 6375 723d              cur=
-0000a070: 6375 722c 0a20 2020 2020 2020 2020 2020  cur,.           
-0000a080: 2029 0a20 2020 2020 2020 2020 2020 2069   ).            i
-0000a090: 6620 6272 616e 6368 2069 7320 4e6f 6e65  f branch is None
-0000a0a0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-0000a0b0: 2020 2320 7461 7267 6574 2062 7261 6e63    # target branc
-0000a0c0: 6820 6973 204e 6f6e 652c 2074 6865 7265  h is None, there
-0000a0d0: 2063 6f75 6c64 2062 6520 6974 656d 7320   could be items 
-0000a0e0: 696e 2061 6c69 6173 6573 5f66 6f6c 6c6f  in aliases_follo
-0000a0f0: 7765 640a 2020 2020 2020 2020 2020 2020  wed.            
-0000a100: 2020 2020 7461 7267 6574 203d 204e 6f6e      target = Non
-0000a110: 650a 2020 2020 2020 2020 2020 2020 2020  e.              
-0000a120: 2020 6272 6561 6b0a 2020 2020 2020 2020    break.        
-0000a130: 2020 2020 6272 616e 6368 5f64 203d 2064      branch_d = d
-0000a140: 6963 7428 7a69 7028 636f 6c73 5f74 6f5f  ict(zip(cols_to_
-0000a150: 6665 7463 682c 2062 7261 6e63 6829 290a  fetch, branch)).
-0000a160: 2020 2020 2020 2020 2020 2020 7265 736f              reso
-0000a170: 6c76 655f 6368 6169 6e2e 6170 7065 6e64  lve_chain.append
-0000a180: 2862 7261 6e63 685f 6e61 6d65 290a 2020  (branch_name).  
-0000a190: 2020 2020 2020 2020 2020 6966 2028 0a20            if (. 
-0000a1a0: 2020 2020 2020 2020 2020 2020 2020 2062                 b
-0000a1b0: 7261 6e63 685f 645b 2274 6172 6765 745f  ranch_d["target_
-0000a1c0: 7479 7065 225d 2021 3d20 536e 6170 7368  type"] != Snapsh
-0000a1d0: 6f74 5461 7267 6574 5479 7065 2e41 4c49  otTargetType.ALI
-0000a1e0: 4153 2e76 616c 7565 0a20 2020 2020 2020  AS.value.       
-0000a1f0: 2020 2020 2020 2020 206f 7220 6e6f 7420           or not 
-0000a200: 666f 6c6c 6f77 5f61 6c69 6173 5f63 6861  follow_alias_cha
-0000a210: 696e 0a20 2020 2020 2020 2020 2020 2029  in.            )
-0000a220: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-0000a230: 2020 2320 6669 7273 7420 6e6f 6e20 616c    # first non al
-0000a240: 6961 7320 6272 616e 6368 206f 7220 7468  ias branch or th
-0000a250: 6520 6669 7273 7420 6272 616e 6368 2077  e first branch w
-0000a260: 6865 6e20 666f 6c6c 6f77 5f61 6c69 6173  hen follow_alias
-0000a270: 5f63 6861 696e 2069 7320 4661 6c73 650a  _chain is False.
-0000a280: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a290: 7461 7267 6574 203d 2028 0a20 2020 2020  target = (.     
-0000a2a0: 2020 2020 2020 2020 2020 2020 2020 2053                 S
-0000a2b0: 6e61 7073 686f 7442 7261 6e63 6828 0a20  napshotBranch(. 
-0000a2c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a2d0: 2020 2020 2020 2074 6172 6765 743d 6272         target=br
-0000a2e0: 616e 6368 5f64 5b22 7461 7267 6574 225d  anch_d["target"]
-0000a2f0: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-0000a300: 2020 2020 2020 2020 2020 7461 7267 6574            target
-0000a310: 5f74 7970 653d 536e 6170 7368 6f74 5461  _type=SnapshotTa
-0000a320: 7267 6574 5479 7065 2862 7261 6e63 685f  rgetType(branch_
-0000a330: 645b 2274 6172 6765 745f 7479 7065 225d  d["target_type"]
-0000a340: 292c 0a20 2020 2020 2020 2020 2020 2020  ),.             
-0000a350: 2020 2020 2020 2029 0a20 2020 2020 2020         ).       
-0000a360: 2020 2020 2020 2020 2020 2020 2069 6620               if 
-0000a370: 6272 616e 6368 5f64 5b22 7461 7267 6574  branch_d["target
-0000a380: 225d 0a20 2020 2020 2020 2020 2020 2020  "].             
-0000a390: 2020 2020 2020 2065 6c73 6520 4e6f 6e65         else None
-0000a3a0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000a3b0: 2029 0a20 2020 2020 2020 2020 2020 2020   ).             
-0000a3c0: 2020 2062 7265 616b 0a20 2020 2020 2020     break.       
-0000a3d0: 2020 2020 2065 6c69 6620 280a 2020 2020       elif (.    
-0000a3e0: 2020 2020 2020 2020 2020 2020 2320 4369              # Ci
-0000a3f0: 7263 756c 6172 2072 6566 6572 656e 6365  rcular reference
-0000a400: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000a410: 2072 6573 6f6c 7665 5f63 6861 696e 2e63   resolve_chain.c
-0000a420: 6f75 6e74 2862 7261 6e63 685f 6e61 6d65  ount(branch_name
-0000a430: 2920 3e20 310a 2020 2020 2020 2020 2020  ) > 1.          
-0000a440: 2020 2020 2020 2320 546f 6f20 6d61 6e79        # Too many
-0000a450: 2072 652d 6469 7265 6374 730a 2020 2020   re-directs.    
-0000a460: 2020 2020 2020 2020 2020 2020 6f72 206c              or l
-0000a470: 656e 2872 6573 6f6c 7665 5f63 6861 696e  en(resolve_chain
-0000a480: 2920 3e3d 206d 6178 5f61 6c69 6173 5f63  ) >= max_alias_c
-0000a490: 6861 696e 5f6c 656e 6774 680a 2020 2020  hain_length.    
-0000a4a0: 2020 2020 2020 2020 293a 0a20 2020 2020          ):.     
-0000a4b0: 2020 2020 2020 2020 2020 2074 6172 6765             targe
-0000a4c0: 7420 3d20 4e6f 6e65 0a20 2020 2020 2020  t = None.       
-0000a4d0: 2020 2020 2020 2020 2062 7265 616b 0a20           break. 
-0000a4e0: 2020 2020 2020 2020 2020 2023 2042 7261             # Bra
-0000a4f0: 6e63 6820 6861 7320 6120 6e6f 6e2d 4e6f  nch has a non-No
-0000a500: 6e65 2074 6172 6765 7420 7769 7468 2074  ne target with t
-0000a510: 7970 6520 616c 6961 730a 2020 2020 2020  ype alias.      
-0000a520: 2020 2020 2020 6272 616e 6368 5f6e 616d        branch_nam
-0000a530: 6520 3d20 6272 616e 6368 5f64 5b22 7461  e = branch_d["ta
-0000a540: 7267 6574 225d 0a0a 2020 2020 2020 2020  rget"]..        
-0000a550: 7265 7475 726e 2053 6e61 7073 686f 7442  return SnapshotB
-0000a560: 7261 6e63 6842 794e 616d 6552 6573 706f  ranchByNameRespo
-0000a570: 6e73 6528 0a20 2020 2020 2020 2020 2020  nse(.           
-0000a580: 2023 2072 6573 6f6c 7665 5f63 6869 616e   # resolve_chian
-0000a590: 2068 6173 2069 7465 6d73 2c20 6272 6163   has items, brac
-0000a5a0: 685f 666f 756e 6420 6d75 7374 2062 6520  h_found must be 
-0000a5b0: 5472 7565 0a20 2020 2020 2020 2020 2020  True.           
-0000a5c0: 2062 7261 6e63 685f 666f 756e 643d 626f   branch_found=bo
-0000a5d0: 6f6c 2872 6573 6f6c 7665 5f63 6861 696e  ol(resolve_chain
-0000a5e0: 292c 0a20 2020 2020 2020 2020 2020 2074  ),.            t
-0000a5f0: 6172 6765 743d 7461 7267 6574 2c0a 2020  arget=target,.  
-0000a600: 2020 2020 2020 2020 2020 616c 6961 7365            aliase
-0000a610: 735f 666f 6c6c 6f77 6564 3d72 6573 6f6c  s_followed=resol
-0000a620: 7665 5f63 6861 696e 2c0a 2020 2020 2020  ve_chain,.      
-0000a630: 2020 290a 0a20 2020 2023 2323 2323 2323    )..    #######
-0000a640: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-0000a650: 2323 230a 2020 2020 2320 4f72 6967 696e  ###.    # Origin
-0000a660: 5669 7369 7420 616e 6420 4f72 6967 696e  Visit and Origin
-0000a670: 5669 7369 7453 7461 7475 730a 2020 2020  VisitStatus.    
-0000a680: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-0000a690: 2323 2323 2323 2323 2323 0a0a 2020 2020  ##########..    
-0000a6a0: 4064 625f 7472 616e 7361 6374 696f 6e28  @db_transaction(
-0000a6b0: 290a 2020 2020 6465 6620 6f72 6967 696e  ).    def origin
-0000a6c0: 5f76 6973 6974 5f61 6464 280a 2020 2020  _visit_add(.    
-0000a6d0: 2020 2020 7365 6c66 2c20 7669 7369 7473      self, visits
-0000a6e0: 3a20 4c69 7374 5b4f 7269 6769 6e56 6973  : List[OriginVis
-0000a6f0: 6974 5d2c 202a 2c20 6462 3a20 4462 2c20  it], *, db: Db, 
-0000a700: 6375 723d 4e6f 6e65 0a20 2020 2029 202d  cur=None.    ) -
-0000a710: 3e20 4974 6572 6162 6c65 5b4f 7269 6769  > Iterable[Origi
-0000a720: 6e56 6973 6974 5d3a 0a20 2020 2020 2020  nVisit]:.       
-0000a730: 2066 6f72 2076 6973 6974 2069 6e20 7669   for visit in vi
-0000a740: 7369 7473 3a0a 2020 2020 2020 2020 2020  sits:.          
-0000a750: 2020 6f72 6967 696e 203d 2073 656c 662e    origin = self.
-0000a760: 6f72 6967 696e 5f67 6574 285b 7669 7369  origin_get([visi
-0000a770: 742e 6f72 6967 696e 5d2c 2064 623d 6462  t.origin], db=db
-0000a780: 2c20 6375 723d 6375 7229 5b30 5d0a 2020  , cur=cur)[0].  
-0000a790: 2020 2020 2020 2020 2020 6966 206e 6f74            if not
-0000a7a0: 206f 7269 6769 6e3a 2020 2320 4361 6e6e   origin:  # Cann
-0000a7b0: 6f74 2061 6464 2061 2076 6973 6974 2077  ot add a visit w
-0000a7c0: 6974 686f 7574 2061 6e20 6f72 6967 696e  ithout an origin
-0000a7d0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000a7e0: 2072 6169 7365 2053 746f 7261 6765 4172   raise StorageAr
-0000a7f0: 6775 6d65 6e74 4578 6365 7074 696f 6e28  gumentException(
-0000a800: 2255 6e6b 6e6f 776e 206f 7269 6769 6e20  "Unknown origin 
-0000a810: 2573 222c 2076 6973 6974 2e6f 7269 6769  %s", visit.origi
-0000a820: 6e29 0a0a 2020 2020 2020 2020 616c 6c5f  n)..        all_
-0000a830: 7669 7369 7473 203d 205b 5d0a 2020 2020  visits = [].    
-0000a840: 2020 2020 666f 7220 7669 7369 7420 696e      for visit in
-0000a850: 2076 6973 6974 733a 0a20 2020 2020 2020   visits:.       
-0000a860: 2020 2020 2069 6620 7669 7369 742e 7669       if visit.vi
-0000a870: 7369 743a 0a20 2020 2020 2020 2020 2020  sit:.           
-0000a880: 2020 2020 2073 656c 662e 6a6f 7572 6e61       self.journa
-0000a890: 6c5f 7772 6974 6572 2e6f 7269 6769 6e5f  l_writer.origin_
-0000a8a0: 7669 7369 745f 6164 6428 5b76 6973 6974  visit_add([visit
-0000a8b0: 5d29 0a20 2020 2020 2020 2020 2020 2020  ]).             
-0000a8c0: 2020 2064 622e 6f72 6967 696e 5f76 6973     db.origin_vis
-0000a8d0: 6974 5f61 6464 5f77 6974 685f 6964 2876  it_add_with_id(v
-0000a8e0: 6973 6974 2c20 6375 723d 6375 7229 0a20  isit, cur=cur). 
-0000a8f0: 2020 2020 2020 2020 2020 2065 6c73 653a             else:
-0000a900: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000a910: 2023 2076 6973 6974 5f69 6420 6973 206e   # visit_id is n
-0000a920: 6f74 2067 6976 656e 2c20 6974 206e 6565  ot given, it nee
-0000a930: 6473 2074 6f20 6265 2073 6574 2062 7920  ds to be set by 
-0000a940: 7468 6520 6462 0a20 2020 2020 2020 2020  the db.         
-0000a950: 2020 2020 2020 2077 6974 6820 636f 6e76         with conv
-0000a960: 6572 745f 7661 6c69 6461 7469 6f6e 5f65  ert_validation_e
-0000a970: 7863 6570 7469 6f6e 7328 293a 0a20 2020  xceptions():.   
-0000a980: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a990: 2076 6973 6974 5f69 6420 3d20 6462 2e6f   visit_id = db.o
-0000a9a0: 7269 6769 6e5f 7669 7369 745f 6164 6428  rigin_visit_add(
-0000a9b0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000a9c0: 2020 2020 2020 2020 2076 6973 6974 2e6f           visit.o
-0000a9d0: 7269 6769 6e2c 2076 6973 6974 2e64 6174  rigin, visit.dat
-0000a9e0: 652c 2076 6973 6974 2e74 7970 652c 2063  e, visit.type, c
-0000a9f0: 7572 3d63 7572 0a20 2020 2020 2020 2020  ur=cur.         
-0000aa00: 2020 2020 2020 2020 2020 2029 0a20 2020             ).   
-0000aa10: 2020 2020 2020 2020 2020 2020 2076 6973               vis
-0000aa20: 6974 203d 2061 7474 722e 6576 6f6c 7665  it = attr.evolve
-0000aa30: 2876 6973 6974 2c20 7669 7369 743d 7669  (visit, visit=vi
-0000aa40: 7369 745f 6964 290a 2020 2020 2020 2020  sit_id).        
-0000aa50: 2020 2020 2020 2020 2320 466f 7263 6564          # Forced
-0000aa60: 2074 6f20 7772 6974 6520 696e 2074 6865   to write in the
-0000aa70: 206a 6f75 726e 616c 2061 6674 6572 2074   journal after t
-0000aa80: 6865 2064 6220 2873 696e 6365 2069 7473  he db (since its
-0000aa90: 2074 6865 2064 620a 2020 2020 2020 2020   the db.        
-0000aaa0: 2020 2020 2020 2020 2320 6361 6c6c 2074          # call t
-0000aab0: 6861 7420 7365 7420 7468 6520 7669 7369  hat set the visi
-0000aac0: 7420 6964 290a 2020 2020 2020 2020 2020  t id).          
-0000aad0: 2020 2020 2020 7365 6c66 2e6a 6f75 726e        self.journ
-0000aae0: 616c 5f77 7269 7465 722e 6f72 6967 696e  al_writer.origin
-0000aaf0: 5f76 6973 6974 5f61 6464 285b 7669 7369  _visit_add([visi
-0000ab00: 745d 290a 2020 2020 2020 2020 2020 2020  t]).            
-0000ab10: 2020 2020 2320 496e 2074 6869 7320 6361      # In this ca
-0000ab20: 7365 2c20 7765 2061 6c73 6f20 7761 6e74  se, we also want
-0000ab30: 2074 6f20 6372 6561 7465 2074 6865 2069   to create the i
-0000ab40: 6e69 7469 616c 204f 5653 206f 626a 6563  nitial OVS objec
-0000ab50: 740a 2020 2020 2020 2020 2020 2020 2020  t.              
-0000ab60: 2020 7669 7369 745f 7374 6174 7573 203d    visit_status =
-0000ab70: 204f 7269 6769 6e56 6973 6974 5374 6174   OriginVisitStat
-0000ab80: 7573 280a 2020 2020 2020 2020 2020 2020  us(.            
-0000ab90: 2020 2020 2020 2020 6f72 6967 696e 3d76          origin=v
-0000aba0: 6973 6974 2e6f 7269 6769 6e2c 0a20 2020  isit.origin,.   
-0000abb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000abc0: 2076 6973 6974 3d76 6973 6974 5f69 642c   visit=visit_id,
-0000abd0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000abe0: 2020 2020 2064 6174 653d 7669 7369 742e       date=visit.
-0000abf0: 6461 7465 2c0a 2020 2020 2020 2020 2020  date,.          
-0000ac00: 2020 2020 2020 2020 2020 7479 7065 3d76            type=v
-0000ac10: 6973 6974 2e74 7970 652c 0a20 2020 2020  isit.type,.     
-0000ac20: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-0000ac30: 7461 7475 733d 2263 7265 6174 6564 222c  tatus="created",
-0000ac40: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000ac50: 2020 2020 2073 6e61 7073 686f 743d 4e6f       snapshot=No
-0000ac60: 6e65 2c0a 2020 2020 2020 2020 2020 2020  ne,.            
-0000ac70: 2020 2020 290a 2020 2020 2020 2020 2020      ).          
-0000ac80: 2020 2020 2020 7365 6c66 2e5f 6f72 6967        self._orig
-0000ac90: 696e 5f76 6973 6974 5f73 7461 7475 735f  in_visit_status_
-0000aca0: 6164 6428 7669 7369 745f 7374 6174 7573  add(visit_status
-0000acb0: 2c20 6462 3d64 622c 2063 7572 3d63 7572  , db=db, cur=cur
-0000acc0: 290a 2020 2020 2020 2020 2020 2020 6173  ).            as
-0000acd0: 7365 7274 2076 6973 6974 2e76 6973 6974  sert visit.visit
-0000ace0: 2069 7320 6e6f 7420 4e6f 6e65 0a20 2020   is not None.   
-0000acf0: 2020 2020 2020 2020 2061 6c6c 5f76 6973           all_vis
-0000ad00: 6974 732e 6170 7065 6e64 2876 6973 6974  its.append(visit
-0000ad10: 290a 0a20 2020 2020 2020 2072 6574 7572  )..        retur
-0000ad20: 6e20 616c 6c5f 7669 7369 7473 0a0a 2020  n all_visits..  
-0000ad30: 2020 6465 6620 5f6f 7269 6769 6e5f 7669    def _origin_vi
-0000ad40: 7369 745f 7374 6174 7573 5f61 6464 280a  sit_status_add(.
-0000ad50: 2020 2020 2020 2020 7365 6c66 2c20 7669          self, vi
-0000ad60: 7369 745f 7374 6174 7573 3a20 4f72 6967  sit_status: Orig
-0000ad70: 696e 5669 7369 7453 7461 7475 732c 2064  inVisitStatus, d
-0000ad80: 622c 2063 7572 0a20 2020 2029 202d 3e20  b, cur.    ) -> 
-0000ad90: 4e6f 6e65 3a0a 2020 2020 2020 2020 2222  None:.        ""
-0000ada0: 2241 6464 2061 6e20 6f72 6967 696e 2076  "Add an origin v
-0000adb0: 6973 6974 2073 7461 7475 7322 2222 0a20  isit status""". 
-0000adc0: 2020 2020 2020 2073 656c 662e 6a6f 7572         self.jour
-0000add0: 6e61 6c5f 7772 6974 6572 2e6f 7269 6769  nal_writer.origi
-0000ade0: 6e5f 7669 7369 745f 7374 6174 7573 5f61  n_visit_status_a
-0000adf0: 6464 285b 7669 7369 745f 7374 6174 7573  dd([visit_status
-0000ae00: 5d29 0a20 2020 2020 2020 2064 622e 6f72  ]).        db.or
-0000ae10: 6967 696e 5f76 6973 6974 5f73 7461 7475  igin_visit_statu
-0000ae20: 735f 6164 6428 7669 7369 745f 7374 6174  s_add(visit_stat
-0000ae30: 7573 2c20 6375 723d 6375 7229 0a0a 2020  us, cur=cur)..  
-0000ae40: 2020 4064 625f 7472 616e 7361 6374 696f    @db_transactio
-0000ae50: 6e28 290a 2020 2020 6465 6620 6f72 6967  n().    def orig
-0000ae60: 696e 5f76 6973 6974 5f73 7461 7475 735f  in_visit_status_
-0000ae70: 6164 6428 0a20 2020 2020 2020 2073 656c  add(.        sel
-0000ae80: 662c 0a20 2020 2020 2020 2076 6973 6974  f,.        visit
-0000ae90: 5f73 7461 7475 7365 733a 204c 6973 745b  _statuses: List[
-0000aea0: 4f72 6967 696e 5669 7369 7453 7461 7475  OriginVisitStatu
-0000aeb0: 735d 2c0a 2020 2020 2020 2020 2a2c 0a20  s],.        *,. 
-0000aec0: 2020 2020 2020 2064 623a 2044 622c 0a20         db: Db,. 
-0000aed0: 2020 2020 2020 2063 7572 3d4e 6f6e 652c         cur=None,
-0000aee0: 0a20 2020 2029 202d 3e20 4469 6374 5b73  .    ) -> Dict[s
-0000aef0: 7472 2c20 696e 745d 3a0a 2020 2020 2020  tr, int]:.      
-0000af00: 2020 7669 7369 745f 7374 6174 7573 6573    visit_statuses
-0000af10: 5f20 3d20 5b5d 0a0a 2020 2020 2020 2020  _ = []..        
-0000af20: 2320 4669 7273 7420 726f 756e 6420 746f  # First round to
-0000af30: 2063 6865 636b 2065 7869 7374 656e 6365   check existence
-0000af40: 2028 6661 696c 2065 6172 6c79 2069 6620   (fail early if 
-0000af50: 616e 7920 6973 206b 6f29 0a20 2020 2020  any is ko).     
-0000af60: 2020 2066 6f72 2076 6973 6974 5f73 7461     for visit_sta
-0000af70: 7475 7320 696e 2076 6973 6974 5f73 7461  tus in visit_sta
-0000af80: 7475 7365 733a 0a20 2020 2020 2020 2020  tuses:.         
-0000af90: 2020 206f 7269 6769 6e5f 7572 6c20 3d20     origin_url = 
-0000afa0: 7365 6c66 2e6f 7269 6769 6e5f 6765 7428  self.origin_get(
-0000afb0: 5b76 6973 6974 5f73 7461 7475 732e 6f72  [visit_status.or
-0000afc0: 6967 696e 5d2c 2064 623d 6462 2c20 6375  igin], db=db, cu
-0000afd0: 723d 6375 7229 5b30 5d0a 2020 2020 2020  r=cur)[0].      
-0000afe0: 2020 2020 2020 6966 206e 6f74 206f 7269        if not ori
-0000aff0: 6769 6e5f 7572 6c3a 0a20 2020 2020 2020  gin_url:.       
-0000b000: 2020 2020 2020 2020 2072 6169 7365 2053           raise S
-0000b010: 746f 7261 6765 4172 6775 6d65 6e74 4578  torageArgumentEx
-0000b020: 6365 7074 696f 6e28 6622 556e 6b6e 6f77  ception(f"Unknow
-0000b030: 6e20 6f72 6967 696e 207b 7669 7369 745f  n origin {visit_
-0000b040: 7374 6174 7573 2e6f 7269 6769 6e7d 2229  status.origin}")
-0000b050: 0a0a 2020 2020 2020 2020 2020 2020 6966  ..            if
-0000b060: 2076 6973 6974 5f73 7461 7475 732e 7479   visit_status.ty
-0000b070: 7065 2069 7320 4e6f 6e65 3a0a 2020 2020  pe is None:.    
-0000b080: 2020 2020 2020 2020 2020 2020 6f72 6967              orig
-0000b090: 696e 5f76 6973 6974 203d 2073 656c 662e  in_visit = self.
-0000b0a0: 6f72 6967 696e 5f76 6973 6974 5f67 6574  origin_visit_get
-0000b0b0: 5f62 7928 0a20 2020 2020 2020 2020 2020  _by(.           
-0000b0c0: 2020 2020 2020 2020 2076 6973 6974 5f73           visit_s
-0000b0d0: 7461 7475 732e 6f72 6967 696e 2c20 7669  tatus.origin, vi
-0000b0e0: 7369 745f 7374 6174 7573 2e76 6973 6974  sit_status.visit
-0000b0f0: 2c20 6462 3d64 622c 2063 7572 3d63 7572  , db=db, cur=cur
-0000b100: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000b110: 2029 0a20 2020 2020 2020 2020 2020 2020   ).             
-0000b120: 2020 2069 6620 6f72 6967 696e 5f76 6973     if origin_vis
-0000b130: 6974 2069 7320 4e6f 6e65 3a0a 2020 2020  it is None:.    
-0000b140: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b150: 7261 6973 6520 5374 6f72 6167 6541 7267  raise StorageArg
-0000b160: 756d 656e 7445 7863 6570 7469 6f6e 280a  umentException(.
-0000b170: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b180: 2020 2020 2020 2020 6622 556e 6b6e 6f77          f"Unknow
-0000b190: 6e20 6f72 6967 696e 2076 6973 6974 207b  n origin visit {
-0000b1a0: 7669 7369 745f 7374 6174 7573 2e76 6973  visit_status.vis
-0000b1b0: 6974 7d20 220a 2020 2020 2020 2020 2020  it} ".          
-0000b1c0: 2020 2020 2020 2020 2020 2020 2020 6622                f"
-0000b1d0: 6f66 206f 7269 6769 6e20 7b76 6973 6974  of origin {visit
-0000b1e0: 5f73 7461 7475 732e 6f72 6967 696e 7d22  _status.origin}"
-0000b1f0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000b200: 2020 2020 2029 0a0a 2020 2020 2020 2020       )..        
-0000b210: 2020 2020 2020 2020 6f72 6967 696e 5f76          origin_v
-0000b220: 6973 6974 5f73 7461 7475 7320 3d20 6174  isit_status = at
-0000b230: 7472 2e65 766f 6c76 6528 7669 7369 745f  tr.evolve(visit_
-0000b240: 7374 6174 7573 2c20 7479 7065 3d6f 7269  status, type=ori
-0000b250: 6769 6e5f 7669 7369 742e 7479 7065 290a  gin_visit.type).
-0000b260: 2020 2020 2020 2020 2020 2020 656c 7365              else
-0000b270: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-0000b280: 2020 6f72 6967 696e 5f76 6973 6974 5f73    origin_visit_s
-0000b290: 7461 7475 7320 3d20 7669 7369 745f 7374  tatus = visit_st
-0000b2a0: 6174 7573 0a0a 2020 2020 2020 2020 2020  atus..          
-0000b2b0: 2020 7669 7369 745f 7374 6174 7573 6573    visit_statuses
-0000b2c0: 5f2e 6170 7065 6e64 286f 7269 6769 6e5f  _.append(origin_
-0000b2d0: 7669 7369 745f 7374 6174 7573 290a 0a20  visit_status).. 
-0000b2e0: 2020 2020 2020 2066 6f72 2076 6973 6974         for visit
-0000b2f0: 5f73 7461 7475 7320 696e 2076 6973 6974  _status in visit
-0000b300: 5f73 7461 7475 7365 735f 3a0a 2020 2020  _statuses_:.    
-0000b310: 2020 2020 2020 2020 7365 6c66 2e5f 6f72          self._or
-0000b320: 6967 696e 5f76 6973 6974 5f73 7461 7475  igin_visit_statu
-0000b330: 735f 6164 6428 7669 7369 745f 7374 6174  s_add(visit_stat
-0000b340: 7573 2c20 6462 2c20 6375 7229 0a20 2020  us, db, cur).   
-0000b350: 2020 2020 2072 6574 7572 6e20 7b22 6f72       return {"or
-0000b360: 6967 696e 5f76 6973 6974 5f73 7461 7475  igin_visit_statu
-0000b370: 733a 6164 6422 3a20 6c65 6e28 7669 7369  s:add": len(visi
-0000b380: 745f 7374 6174 7573 6573 5f29 7d0a 0a20  t_statuses_)}.. 
-0000b390: 2020 2040 6462 5f74 7261 6e73 6163 7469     @db_transacti
-0000b3a0: 6f6e 2829 0a20 2020 2064 6566 206f 7269  on().    def ori
-0000b3b0: 6769 6e5f 7669 7369 745f 7374 6174 7573  gin_visit_status
-0000b3c0: 5f67 6574 5f6c 6174 6573 7428 0a20 2020  _get_latest(.   
-0000b3d0: 2020 2020 2073 656c 662c 0a20 2020 2020       self,.     
-0000b3e0: 2020 206f 7269 6769 6e5f 7572 6c3a 2073     origin_url: s
-0000b3f0: 7472 2c0a 2020 2020 2020 2020 7669 7369  tr,.        visi
-0000b400: 743a 2069 6e74 2c0a 2020 2020 2020 2020  t: int,.        
-0000b410: 616c 6c6f 7765 645f 7374 6174 7573 6573  allowed_statuses
-0000b420: 3a20 4f70 7469 6f6e 616c 5b4c 6973 745b  : Optional[List[
-0000b430: 7374 725d 5d20 3d20 4e6f 6e65 2c0a 2020  str]] = None,.  
-0000b440: 2020 2020 2020 7265 7175 6972 655f 736e        require_sn
-0000b450: 6170 7368 6f74 3a20 626f 6f6c 203d 2046  apshot: bool = F
-0000b460: 616c 7365 2c0a 2020 2020 2020 2020 2a2c  alse,.        *,
-0000b470: 0a20 2020 2020 2020 2064 623a 2044 622c  .        db: Db,
-0000b480: 0a20 2020 2020 2020 2063 7572 3d4e 6f6e  .        cur=Non
-0000b490: 652c 0a20 2020 2029 202d 3e20 4f70 7469  e,.    ) -> Opti
-0000b4a0: 6f6e 616c 5b4f 7269 6769 6e56 6973 6974  onal[OriginVisit
-0000b4b0: 5374 6174 7573 5d3a 0a20 2020 2020 2020  Status]:.       
-0000b4c0: 2069 6620 616c 6c6f 7765 645f 7374 6174   if allowed_stat
-0000b4d0: 7573 6573 2061 6e64 206e 6f74 2073 6574  uses and not set
-0000b4e0: 2861 6c6c 6f77 6564 5f73 7461 7475 7365  (allowed_statuse
-0000b4f0: 7329 2e69 6e74 6572 7365 6374 696f 6e28  s).intersection(
-0000b500: 5649 5349 545f 5354 4154 5553 4553 293a  VISIT_STATUSES):
-0000b510: 0a20 2020 2020 2020 2020 2020 2072 6169  .            rai
-0000b520: 7365 2053 746f 7261 6765 4172 6775 6d65  se StorageArgume
-0000b530: 6e74 4578 6365 7074 696f 6e28 0a20 2020  ntException(.   
-0000b540: 2020 2020 2020 2020 2020 2020 2066 2255               f"U
-0000b550: 6e6b 6e6f 776e 2061 6c6c 6f77 6564 2073  nknown allowed s
-0000b560: 7461 7475 7365 7320 7b27 2c27 2e6a 6f69  tatuses {','.joi
-0000b570: 6e28 616c 6c6f 7765 645f 7374 6174 7573  n(allowed_status
-0000b580: 6573 297d 2c20 6f6e 6c79 2022 0a20 2020  es)}, only ".   
-0000b590: 2020 2020 2020 2020 2020 2020 2066 227b               f"{
-0000b5a0: 272c 272e 6a6f 696e 2856 4953 4954 5f53  ','.join(VISIT_S
-0000b5b0: 5441 5455 5345 5329 7d20 6175 7468 6f72  TATUSES)} author
-0000b5c0: 697a 6564 220a 2020 2020 2020 2020 2020  ized".          
-0000b5d0: 2020 290a 0a20 2020 2020 2020 2072 6f77    )..        row
-0000b5e0: 5f64 203d 2064 622e 6f72 6967 696e 5f76  _d = db.origin_v
-0000b5f0: 6973 6974 5f73 7461 7475 735f 6765 745f  isit_status_get_
-0000b600: 6c61 7465 7374 280a 2020 2020 2020 2020  latest(.        
-0000b610: 2020 2020 6f72 6967 696e 5f75 726c 2c20      origin_url, 
-0000b620: 7669 7369 742c 2061 6c6c 6f77 6564 5f73  visit, allowed_s
-0000b630: 7461 7475 7365 732c 2072 6571 7569 7265  tatuses, require
-0000b640: 5f73 6e61 7073 686f 742c 2063 7572 3d63  _snapshot, cur=c
-0000b650: 7572 0a20 2020 2020 2020 2029 0a20 2020  ur.        ).   
-0000b660: 2020 2020 2069 6620 6e6f 7420 726f 775f       if not row_
-0000b670: 643a 0a20 2020 2020 2020 2020 2020 2072  d:.            r
-0000b680: 6574 7572 6e20 4e6f 6e65 0a20 2020 2020  eturn None.     
-0000b690: 2020 2072 6574 7572 6e20 4f72 6967 696e     return Origin
-0000b6a0: 5669 7369 7453 7461 7475 7328 2a2a 726f  VisitStatus(**ro
-0000b6b0: 775f 6429 0a0a 2020 2020 4064 625f 7472  w_d)..    @db_tr
-0000b6c0: 616e 7361 6374 696f 6e28 7374 6174 656d  ansaction(statem
-0000b6d0: 656e 745f 7469 6d65 6f75 743d 3530 3029  ent_timeout=500)
-0000b6e0: 0a20 2020 2064 6566 206f 7269 6769 6e5f  .    def origin_
-0000b6f0: 7669 7369 745f 6765 7428 0a20 2020 2020  visit_get(.     
-0000b700: 2020 2073 656c 662c 0a20 2020 2020 2020     self,.       
-0000b710: 206f 7269 6769 6e3a 2073 7472 2c0a 2020   origin: str,.  
-0000b720: 2020 2020 2020 7061 6765 5f74 6f6b 656e        page_token
-0000b730: 3a20 4f70 7469 6f6e 616c 5b73 7472 5d20  : Optional[str] 
-0000b740: 3d20 4e6f 6e65 2c0a 2020 2020 2020 2020  = None,.        
-0000b750: 6f72 6465 723a 204c 6973 744f 7264 6572  order: ListOrder
-0000b760: 203d 204c 6973 744f 7264 6572 2e41 5343   = ListOrder.ASC
-0000b770: 2c0a 2020 2020 2020 2020 6c69 6d69 743a  ,.        limit:
-0000b780: 2069 6e74 203d 2031 302c 0a20 2020 2020   int = 10,.     
-0000b790: 2020 202a 2c0a 2020 2020 2020 2020 6462     *,.        db
-0000b7a0: 3a20 4462 2c0a 2020 2020 2020 2020 6375  : Db,.        cu
-0000b7b0: 723d 4e6f 6e65 2c0a 2020 2020 2920 2d3e  r=None,.    ) ->
-0000b7c0: 2050 6167 6564 5265 7375 6c74 5b4f 7269   PagedResult[Ori
-0000b7d0: 6769 6e56 6973 6974 5d3a 0a20 2020 2020  ginVisit]:.     
-0000b7e0: 2020 2070 6167 655f 746f 6b65 6e20 3d20     page_token = 
-0000b7f0: 7061 6765 5f74 6f6b 656e 206f 7220 2230  page_token or "0
-0000b800: 220a 2020 2020 2020 2020 6966 206e 6f74  ".        if not
-0000b810: 2069 7369 6e73 7461 6e63 6528 6f72 6465   isinstance(orde
-0000b820: 722c 204c 6973 744f 7264 6572 293a 0a20  r, ListOrder):. 
-0000b830: 2020 2020 2020 2020 2020 2072 6169 7365             raise
-0000b840: 2053 746f 7261 6765 4172 6775 6d65 6e74   StorageArgument
-0000b850: 4578 6365 7074 696f 6e28 226f 7264 6572  Exception("order
-0000b860: 206d 7573 7420 6265 2061 204c 6973 744f   must be a ListO
-0000b870: 7264 6572 2076 616c 7565 2229 0a20 2020  rder value").   
-0000b880: 2020 2020 2069 6620 6e6f 7420 6973 696e       if not isin
-0000b890: 7374 616e 6365 2870 6167 655f 746f 6b65  stance(page_toke
-0000b8a0: 6e2c 2073 7472 293a 0a20 2020 2020 2020  n, str):.       
-0000b8b0: 2020 2020 2072 6169 7365 2053 746f 7261       raise Stora
-0000b8c0: 6765 4172 6775 6d65 6e74 4578 6365 7074  geArgumentExcept
-0000b8d0: 696f 6e28 2270 6167 655f 746f 6b65 6e20  ion("page_token 
-0000b8e0: 6d75 7374 2062 6520 6120 7374 7269 6e67  must be a string
-0000b8f0: 2e22 290a 0a20 2020 2020 2020 206e 6578  .")..        nex
-0000b900: 745f 7061 6765 5f74 6f6b 656e 203d 204e  t_page_token = N
-0000b910: 6f6e 650a 2020 2020 2020 2020 7669 7369  one.        visi
-0000b920: 745f 6672 6f6d 203d 2069 6e74 2870 6167  t_from = int(pag
-0000b930: 655f 746f 6b65 6e29 0a20 2020 2020 2020  e_token).       
-0000b940: 2076 6973 6974 733a 204c 6973 745b 4f72   visits: List[Or
-0000b950: 6967 696e 5669 7369 745d 203d 205b 5d0a  iginVisit] = [].
-0000b960: 2020 2020 2020 2020 6578 7472 615f 6c69          extra_li
-0000b970: 6d69 7420 3d20 6c69 6d69 7420 2b20 310a  mit = limit + 1.
-0000b980: 2020 2020 2020 2020 666f 7220 726f 7720          for row 
-0000b990: 696e 2064 622e 6f72 6967 696e 5f76 6973  in db.origin_vis
-0000b9a0: 6974 5f67 6574 5f72 616e 6765 280a 2020  it_get_range(.  
-0000b9b0: 2020 2020 2020 2020 2020 6f72 6967 696e            origin
-0000b9c0: 2c20 7669 7369 745f 6672 6f6d 3d76 6973  , visit_from=vis
-0000b9d0: 6974 5f66 726f 6d2c 206f 7264 6572 3d6f  it_from, order=o
-0000b9e0: 7264 6572 2c20 6c69 6d69 743d 6578 7472  rder, limit=extr
-0000b9f0: 615f 6c69 6d69 742c 2063 7572 3d63 7572  a_limit, cur=cur
-0000ba00: 0a20 2020 2020 2020 2029 3a0a 2020 2020  .        ):.    
-0000ba10: 2020 2020 2020 2020 726f 775f 6420 3d20          row_d = 
-0000ba20: 6469 6374 287a 6970 2864 622e 6f72 6967  dict(zip(db.orig
-0000ba30: 696e 5f76 6973 6974 5f63 6f6c 732c 2072  in_visit_cols, r
-0000ba40: 6f77 2929 0a20 2020 2020 2020 2020 2020  ow)).           
-0000ba50: 2076 6973 6974 732e 6170 7065 6e64 280a   visits.append(.
-0000ba60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ba70: 4f72 6967 696e 5669 7369 7428 0a20 2020  OriginVisit(.   
-0000ba80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ba90: 206f 7269 6769 6e3d 726f 775f 645b 226f   origin=row_d["o
-0000baa0: 7269 6769 6e22 5d2c 0a20 2020 2020 2020  rigin"],.       
-0000bab0: 2020 2020 2020 2020 2020 2020 2076 6973               vis
-0000bac0: 6974 3d72 6f77 5f64 5b22 7669 7369 7422  it=row_d["visit"
-0000bad0: 5d2c 0a20 2020 2020 2020 2020 2020 2020  ],.             
-0000bae0: 2020 2020 2020 2064 6174 653d 726f 775f         date=row_
-0000baf0: 645b 2264 6174 6522 5d2c 0a20 2020 2020  d["date"],.     
-0000bb00: 2020 2020 2020 2020 2020 2020 2020 2074                 t
-0000bb10: 7970 653d 726f 775f 645b 2274 7970 6522  ype=row_d["type"
-0000bb20: 5d2c 0a20 2020 2020 2020 2020 2020 2020  ],.             
-0000bb30: 2020 2029 0a20 2020 2020 2020 2020 2020     ).           
-0000bb40: 2029 0a0a 2020 2020 2020 2020 6173 7365   )..        asse
-0000bb50: 7274 206c 656e 2876 6973 6974 7329 203c  rt len(visits) <
-0000bb60: 3d20 6578 7472 615f 6c69 6d69 740a 0a20  = extra_limit.. 
-0000bb70: 2020 2020 2020 2069 6620 6c65 6e28 7669         if len(vi
-0000bb80: 7369 7473 2920 3d3d 2065 7874 7261 5f6c  sits) == extra_l
-0000bb90: 696d 6974 3a0a 2020 2020 2020 2020 2020  imit:.          
-0000bba0: 2020 7669 7369 7473 203d 2076 6973 6974    visits = visit
-0000bbb0: 735b 3a6c 696d 6974 5d0a 2020 2020 2020  s[:limit].      
-0000bbc0: 2020 2020 2020 6e65 7874 5f70 6167 655f        next_page_
-0000bbd0: 746f 6b65 6e20 3d20 7374 7228 7669 7369  token = str(visi
-0000bbe0: 7473 5b2d 315d 2e76 6973 6974 290a 0a20  ts[-1].visit).. 
-0000bbf0: 2020 2020 2020 2072 6574 7572 6e20 5061         return Pa
-0000bc00: 6765 6452 6573 756c 7428 7265 7375 6c74  gedResult(result
-0000bc10: 733d 7669 7369 7473 2c20 6e65 7874 5f70  s=visits, next_p
-0000bc20: 6167 655f 746f 6b65 6e3d 6e65 7874 5f70  age_token=next_p
-0000bc30: 6167 655f 746f 6b65 6e29 0a0a 2020 2020  age_token)..    
-0000bc40: 4064 625f 7472 616e 7361 6374 696f 6e28  @db_transaction(
-0000bc50: 7374 6174 656d 656e 745f 7469 6d65 6f75  statement_timeou
-0000bc60: 743d 3230 3030 290a 2020 2020 6465 6620  t=2000).    def 
-0000bc70: 6f72 6967 696e 5f76 6973 6974 5f67 6574  origin_visit_get
-0000bc80: 5f77 6974 685f 7374 6174 7573 6573 280a  _with_statuses(.
-0000bc90: 2020 2020 2020 2020 7365 6c66 2c0a 2020          self,.  
-0000bca0: 2020 2020 2020 6f72 6967 696e 3a20 7374        origin: st
-0000bcb0: 722c 0a20 2020 2020 2020 2061 6c6c 6f77  r,.        allow
-0000bcc0: 6564 5f73 7461 7475 7365 733a 204f 7074  ed_statuses: Opt
-0000bcd0: 696f 6e61 6c5b 4c69 7374 5b73 7472 5d5d  ional[List[str]]
-0000bce0: 203d 204e 6f6e 652c 0a20 2020 2020 2020   = None,.       
-0000bcf0: 2072 6571 7569 7265 5f73 6e61 7073 686f   require_snapsho
-0000bd00: 743a 2062 6f6f 6c20 3d20 4661 6c73 652c  t: bool = False,
-0000bd10: 0a20 2020 2020 2020 2070 6167 655f 746f  .        page_to
-0000bd20: 6b65 6e3a 204f 7074 696f 6e61 6c5b 7374  ken: Optional[st
-0000bd30: 725d 203d 204e 6f6e 652c 0a20 2020 2020  r] = None,.     
-0000bd40: 2020 206f 7264 6572 3a20 4c69 7374 4f72     order: ListOr
-0000bd50: 6465 7220 3d20 4c69 7374 4f72 6465 722e  der = ListOrder.
-0000bd60: 4153 432c 0a20 2020 2020 2020 206c 696d  ASC,.        lim
-0000bd70: 6974 3a20 696e 7420 3d20 3130 2c0a 2020  it: int = 10,.  
-0000bd80: 2020 2020 2020 2a2c 0a20 2020 2020 2020        *,.       
-0000bd90: 2064 623a 2044 622c 0a20 2020 2020 2020   db: Db,.       
-0000bda0: 2063 7572 3d4e 6f6e 652c 0a20 2020 2029   cur=None,.    )
-0000bdb0: 202d 3e20 5061 6765 6452 6573 756c 745b   -> PagedResult[
-0000bdc0: 4f72 6967 696e 5669 7369 7457 6974 6853  OriginVisitWithS
-0000bdd0: 7461 7475 7365 735d 3a0a 2020 2020 2020  tatuses]:.      
-0000bde0: 2020 7061 6765 5f74 6f6b 656e 203d 2070    page_token = p
-0000bdf0: 6167 655f 746f 6b65 6e20 6f72 2022 3022  age_token or "0"
-0000be00: 0a20 2020 2020 2020 2069 6620 6e6f 7420  .        if not 
-0000be10: 6973 696e 7374 616e 6365 286f 7264 6572  isinstance(order
-0000be20: 2c20 4c69 7374 4f72 6465 7229 3a0a 2020  , ListOrder):.  
-0000be30: 2020 2020 2020 2020 2020 7261 6973 6520            raise 
-0000be40: 5374 6f72 6167 6541 7267 756d 656e 7445  StorageArgumentE
-0000be50: 7863 6570 7469 6f6e 2822 6f72 6465 7220  xception("order 
-0000be60: 6d75 7374 2062 6520 6120 4c69 7374 4f72  must be a ListOr
-0000be70: 6465 7220 7661 6c75 6522 290a 2020 2020  der value").    
-0000be80: 2020 2020 6966 206e 6f74 2069 7369 6e73      if not isins
-0000be90: 7461 6e63 6528 7061 6765 5f74 6f6b 656e  tance(page_token
-0000bea0: 2c20 7374 7229 3a0a 2020 2020 2020 2020  , str):.        
-0000beb0: 2020 2020 7261 6973 6520 5374 6f72 6167      raise Storag
-0000bec0: 6541 7267 756d 656e 7445 7863 6570 7469  eArgumentExcepti
-0000bed0: 6f6e 2822 7061 6765 5f74 6f6b 656e 206d  on("page_token m
-0000bee0: 7573 7420 6265 2061 2073 7472 696e 672e  ust be a string.
-0000bef0: 2229 0a0a 2020 2020 2020 2020 2320 4669  ")..        # Fi
-0000bf00: 7273 7420 6765 7420 7669 7369 7473 2028  rst get visits (
-0000bf10: 706c 7573 206f 6e65 2073 6f20 7765 2063  plus one so we c
-0000bf20: 616e 2075 7365 2069 7420 6173 2074 6865  an use it as the
-0000bf30: 206e 6578 7420 7061 6765 2074 6f6b 656e   next page token
-0000bf40: 2069 6620 616e 7929 0a20 2020 2020 2020   if any).       
-0000bf50: 2076 6973 6974 735f 7061 6765 203d 2073   visits_page = s
-0000bf60: 656c 662e 6f72 6967 696e 5f76 6973 6974  elf.origin_visit
-0000bf70: 5f67 6574 280a 2020 2020 2020 2020 2020  _get(.          
-0000bf80: 2020 6f72 6967 696e 3d6f 7269 6769 6e2c    origin=origin,
-0000bf90: 0a20 2020 2020 2020 2020 2020 2070 6167  .            pag
-0000bfa0: 655f 746f 6b65 6e3d 7061 6765 5f74 6f6b  e_token=page_tok
-0000bfb0: 656e 2c0a 2020 2020 2020 2020 2020 2020  en,.            
-0000bfc0: 6f72 6465 723d 6f72 6465 722c 0a20 2020  order=order,.   
-0000bfd0: 2020 2020 2020 2020 206c 696d 6974 3d6c           limit=l
-0000bfe0: 696d 6974 2c0a 2020 2020 2020 2020 2020  imit,.          
-0000bff0: 2020 6462 3d64 622c 0a20 2020 2020 2020    db=db,.       
-0000c000: 2020 2020 2063 7572 3d63 7572 2c0a 2020       cur=cur,.  
-0000c010: 2020 2020 2020 290a 0a20 2020 2020 2020        )..       
-0000c020: 2076 6973 6974 7320 3d20 7669 7369 7473   visits = visits
-0000c030: 5f70 6167 652e 7265 7375 6c74 730a 2020  _page.results.  
-0000c040: 2020 2020 2020 6e65 7874 5f70 6167 655f        next_page_
-0000c050: 746f 6b65 6e20 3d20 7669 7369 7473 5f70  token = visits_p
-0000c060: 6167 652e 6e65 7874 5f70 6167 655f 746f  age.next_page_to
-0000c070: 6b65 6e0a 0a20 2020 2020 2020 2069 6620  ken..        if 
-0000c080: 7669 7369 7473 3a0a 2020 2020 2020 2020  visits:.        
-0000c090: 2020 2020 7669 7369 745f 6672 6f6d 203d      visit_from =
-0000c0a0: 206d 696e 2876 6973 6974 735b 305d 2e76   min(visits[0].v
-0000c0b0: 6973 6974 2c20 7669 7369 7473 5b2d 315d  isit, visits[-1]
-0000c0c0: 2e76 6973 6974 290a 2020 2020 2020 2020  .visit).        
-0000c0d0: 2020 2020 7669 7369 745f 746f 203d 206d      visit_to = m
-0000c0e0: 6178 2876 6973 6974 735b 305d 2e76 6973  ax(visits[0].vis
-0000c0f0: 6974 2c20 7669 7369 7473 5b2d 315d 2e76  it, visits[-1].v
-0000c100: 6973 6974 290a 0a20 2020 2020 2020 2020  isit)..         
-0000c110: 2020 2023 2054 6865 6e2c 2066 6574 6368     # Then, fetch
-0000c120: 2061 6c6c 2073 7461 7475 7365 7320 6173   all statuses as
-0000c130: 736f 6369 6174 6564 2074 6f20 7468 6573  sociated to thes
-0000c140: 6520 7669 7369 7473 0a20 2020 2020 2020  e visits.       
-0000c150: 2020 2020 2076 6973 6974 5f73 7461 7475       visit_statu
-0000c160: 7365 733a 2044 6963 745b 696e 742c 204c  ses: Dict[int, L
-0000c170: 6973 745b 4f72 6967 696e 5669 7369 7453  ist[OriginVisitS
-0000c180: 7461 7475 735d 5d20 3d20 6465 6661 756c  tatus]] = defaul
-0000c190: 7464 6963 7428 6c69 7374 290a 2020 2020  tdict(list).    
-0000c1a0: 2020 2020 2020 2020 666f 7220 726f 7720          for row 
-0000c1b0: 696e 2064 622e 6f72 6967 696e 5f76 6973  in db.origin_vis
-0000c1c0: 6974 5f73 7461 7475 735f 6765 745f 616c  it_status_get_al
-0000c1d0: 6c5f 696e 5f72 616e 6765 280a 2020 2020  l_in_range(.    
-0000c1e0: 2020 2020 2020 2020 2020 2020 6f72 6967              orig
-0000c1f0: 696e 2c0a 2020 2020 2020 2020 2020 2020  in,.            
-0000c200: 2020 2020 616c 6c6f 7765 645f 7374 6174      allowed_stat
-0000c210: 7573 6573 2c0a 2020 2020 2020 2020 2020  uses,.          
-0000c220: 2020 2020 2020 7265 7175 6972 655f 736e        require_sn
-0000c230: 6170 7368 6f74 2c0a 2020 2020 2020 2020  apshot,.        
-0000c240: 2020 2020 2020 2020 7669 7369 745f 6672          visit_fr
-0000c250: 6f6d 3d76 6973 6974 5f66 726f 6d2c 0a20  om=visit_from,. 
-0000c260: 2020 2020 2020 2020 2020 2020 2020 2076                 v
-0000c270: 6973 6974 5f74 6f3d 7669 7369 745f 746f  isit_to=visit_to
-0000c280: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-0000c290: 2020 6375 723d 6375 722c 0a20 2020 2020    cur=cur,.     
-0000c2a0: 2020 2020 2020 2029 3a0a 2020 2020 2020         ):.      
-0000c2b0: 2020 2020 2020 2020 2020 726f 775f 6420            row_d 
-0000c2c0: 3d20 6469 6374 287a 6970 2864 622e 6f72  = dict(zip(db.or
-0000c2d0: 6967 696e 5f76 6973 6974 5f73 7461 7475  igin_visit_statu
-0000c2e0: 735f 636f 6c73 2c20 726f 7729 290a 0a20  s_cols, row)).. 
-0000c2f0: 2020 2020 2020 2020 2020 2020 2020 2076                 v
-0000c300: 6973 6974 5f73 7461 7475 7365 735b 726f  isit_statuses[ro
-0000c310: 775f 645b 2276 6973 6974 225d 5d2e 6170  w_d["visit"]].ap
-0000c320: 7065 6e64 284f 7269 6769 6e56 6973 6974  pend(OriginVisit
-0000c330: 5374 6174 7573 282a 2a72 6f77 5f64 2929  Status(**row_d))
-0000c340: 0a0a 2020 2020 2020 2020 7265 7375 6c74  ..        result
-0000c350: 7320 3d20 5b0a 2020 2020 2020 2020 2020  s = [.          
-0000c360: 2020 4f72 6967 696e 5669 7369 7457 6974    OriginVisitWit
-0000c370: 6853 7461 7475 7365 7328 7669 7369 743d  hStatuses(visit=
-0000c380: 7669 7369 742c 2073 7461 7475 7365 733d  visit, statuses=
-0000c390: 7669 7369 745f 7374 6174 7573 6573 5b76  visit_statuses[v
-0000c3a0: 6973 6974 2e76 6973 6974 5d29 0a20 2020  isit.visit]).   
-0000c3b0: 2020 2020 2020 2020 2066 6f72 2076 6973           for vis
-0000c3c0: 6974 2069 6e20 7669 7369 7473 0a20 2020  it in visits.   
-0000c3d0: 2020 2020 205d 0a0a 2020 2020 2020 2020       ]..        
-0000c3e0: 7265 7475 726e 2050 6167 6564 5265 7375  return PagedResu
-0000c3f0: 6c74 2872 6573 756c 7473 3d72 6573 756c  lt(results=resul
-0000c400: 7473 2c20 6e65 7874 5f70 6167 655f 746f  ts, next_page_to
-0000c410: 6b65 6e3d 6e65 7874 5f70 6167 655f 746f  ken=next_page_to
-0000c420: 6b65 6e29 0a0a 2020 2020 4064 625f 7472  ken)..    @db_tr
-0000c430: 616e 7361 6374 696f 6e28 7374 6174 656d  ansaction(statem
-0000c440: 656e 745f 7469 6d65 6f75 743d 3230 3030  ent_timeout=2000
-0000c450: 290a 2020 2020 6465 6620 6f72 6967 696e  ).    def origin
-0000c460: 5f76 6973 6974 5f66 696e 645f 6279 5f64  _visit_find_by_d
-0000c470: 6174 6528 0a20 2020 2020 2020 2073 656c  ate(.        sel
-0000c480: 662c 0a20 2020 2020 2020 206f 7269 6769  f,.        origi
-0000c490: 6e3a 2073 7472 2c0a 2020 2020 2020 2020  n: str,.        
-0000c4a0: 7669 7369 745f 6461 7465 3a20 6461 7465  visit_date: date
-0000c4b0: 7469 6d65 2e64 6174 6574 696d 652c 0a20  time.datetime,. 
-0000c4c0: 2020 2020 2020 2074 7970 653a 204f 7074         type: Opt
-0000c4d0: 696f 6e61 6c5b 7374 725d 203d 204e 6f6e  ional[str] = Non
-0000c4e0: 652c 0a20 2020 2020 2020 202a 2c0a 2020  e,.        *,.  
-0000c4f0: 2020 2020 2020 6462 3a20 4462 2c0a 2020        db: Db,.  
-0000c500: 2020 2020 2020 6375 723d 4e6f 6e65 2c0a        cur=None,.
-0000c510: 2020 2020 2920 2d3e 204f 7074 696f 6e61      ) -> Optiona
-0000c520: 6c5b 4f72 6967 696e 5669 7369 745d 3a0a  l[OriginVisit]:.
-0000c530: 2020 2020 2020 2020 726f 775f 6420 3d20          row_d = 
-0000c540: 6462 2e6f 7269 6769 6e5f 7669 7369 745f  db.origin_visit_
-0000c550: 6669 6e64 5f62 795f 6461 7465 286f 7269  find_by_date(ori
-0000c560: 6769 6e2c 2076 6973 6974 5f64 6174 652c  gin, visit_date,
-0000c570: 2074 7970 653d 7479 7065 2c20 6375 723d   type=type, cur=
-0000c580: 6375 7229 0a20 2020 2020 2020 2069 6620  cur).        if 
-0000c590: 6e6f 7420 726f 775f 643a 0a20 2020 2020  not row_d:.     
-0000c5a0: 2020 2020 2020 2072 6574 7572 6e20 4e6f         return No
-0000c5b0: 6e65 0a20 2020 2020 2020 2072 6574 7572  ne.        retur
-0000c5c0: 6e20 4f72 6967 696e 5669 7369 7428 0a20  n OriginVisit(. 
-0000c5d0: 2020 2020 2020 2020 2020 206f 7269 6769             origi
-0000c5e0: 6e3d 726f 775f 645b 226f 7269 6769 6e22  n=row_d["origin"
-0000c5f0: 5d2c 0a20 2020 2020 2020 2020 2020 2076  ],.            v
-0000c600: 6973 6974 3d72 6f77 5f64 5b22 7669 7369  isit=row_d["visi
-0000c610: 7422 5d2c 0a20 2020 2020 2020 2020 2020  t"],.           
-0000c620: 2064 6174 653d 726f 775f 645b 2264 6174   date=row_d["dat
-0000c630: 6522 5d2c 0a20 2020 2020 2020 2020 2020  e"],.           
-0000c640: 2074 7970 653d 726f 775f 645b 2274 7970   type=row_d["typ
-0000c650: 6522 5d2c 0a20 2020 2020 2020 2029 0a0a  e"],.        )..
-0000c660: 2020 2020 4064 625f 7472 616e 7361 6374      @db_transact
-0000c670: 696f 6e28 7374 6174 656d 656e 745f 7469  ion(statement_ti
-0000c680: 6d65 6f75 743d 3530 3029 0a20 2020 2064  meout=500).    d
-0000c690: 6566 206f 7269 6769 6e5f 7669 7369 745f  ef origin_visit_
-0000c6a0: 6765 745f 6279 280a 2020 2020 2020 2020  get_by(.        
-0000c6b0: 7365 6c66 2c20 6f72 6967 696e 3a20 7374  self, origin: st
-0000c6c0: 722c 2076 6973 6974 3a20 696e 742c 202a  r, visit: int, *
-0000c6d0: 2c20 6462 3a20 4462 2c20 6375 723d 4e6f  , db: Db, cur=No
-0000c6e0: 6e65 0a20 2020 2029 202d 3e20 4f70 7469  ne.    ) -> Opti
-0000c6f0: 6f6e 616c 5b4f 7269 6769 6e56 6973 6974  onal[OriginVisit
-0000c700: 5d3a 0a20 2020 2020 2020 2072 6f77 203d  ]:.        row =
-0000c710: 2064 622e 6f72 6967 696e 5f76 6973 6974   db.origin_visit
-0000c720: 5f67 6574 286f 7269 6769 6e2c 2076 6973  _get(origin, vis
-0000c730: 6974 2c20 6375 7229 0a20 2020 2020 2020  it, cur).       
-0000c740: 2069 6620 726f 773a 0a20 2020 2020 2020   if row:.       
-0000c750: 2020 2020 2072 6f77 5f64 203d 2064 6963       row_d = dic
-0000c760: 7428 7a69 7028 6462 2e6f 7269 6769 6e5f  t(zip(db.origin_
-0000c770: 7669 7369 745f 6765 745f 636f 6c73 2c20  visit_get_cols, 
-0000c780: 726f 7729 290a 2020 2020 2020 2020 2020  row)).          
-0000c790: 2020 7265 7475 726e 204f 7269 6769 6e56    return OriginV
-0000c7a0: 6973 6974 280a 2020 2020 2020 2020 2020  isit(.          
-0000c7b0: 2020 2020 2020 6f72 6967 696e 3d72 6f77        origin=row
-0000c7c0: 5f64 5b22 6f72 6967 696e 225d 2c0a 2020  _d["origin"],.  
-0000c7d0: 2020 2020 2020 2020 2020 2020 2020 7669                vi
-0000c7e0: 7369 743d 726f 775f 645b 2276 6973 6974  sit=row_d["visit
-0000c7f0: 225d 2c0a 2020 2020 2020 2020 2020 2020  "],.            
-0000c800: 2020 2020 6461 7465 3d72 6f77 5f64 5b22      date=row_d["
-0000c810: 6461 7465 225d 2c0a 2020 2020 2020 2020  date"],.        
-0000c820: 2020 2020 2020 2020 7479 7065 3d72 6f77          type=row
-0000c830: 5f64 5b22 7479 7065 225d 2c0a 2020 2020  _d["type"],.    
-0000c840: 2020 2020 2020 2020 290a 2020 2020 2020          ).      
-0000c850: 2020 7265 7475 726e 204e 6f6e 650a 0a20    return None.. 
-0000c860: 2020 2040 6462 5f74 7261 6e73 6163 7469     @db_transacti
-0000c870: 6f6e 2873 7461 7465 6d65 6e74 5f74 696d  on(statement_tim
-0000c880: 656f 7574 3d34 3030 3029 0a20 2020 2064  eout=4000).    d
-0000c890: 6566 206f 7269 6769 6e5f 7669 7369 745f  ef origin_visit_
-0000c8a0: 6765 745f 6c61 7465 7374 280a 2020 2020  get_latest(.    
-0000c8b0: 2020 2020 7365 6c66 2c0a 2020 2020 2020      self,.      
-0000c8c0: 2020 6f72 6967 696e 3a20 7374 722c 0a20    origin: str,. 
-0000c8d0: 2020 2020 2020 2074 7970 653a 204f 7074         type: Opt
-0000c8e0: 696f 6e61 6c5b 7374 725d 203d 204e 6f6e  ional[str] = Non
-0000c8f0: 652c 0a20 2020 2020 2020 2061 6c6c 6f77  e,.        allow
-0000c900: 6564 5f73 7461 7475 7365 733a 204f 7074  ed_statuses: Opt
-0000c910: 696f 6e61 6c5b 4c69 7374 5b73 7472 5d5d  ional[List[str]]
-0000c920: 203d 204e 6f6e 652c 0a20 2020 2020 2020   = None,.       
-0000c930: 2072 6571 7569 7265 5f73 6e61 7073 686f   require_snapsho
-0000c940: 743a 2062 6f6f 6c20 3d20 4661 6c73 652c  t: bool = False,
-0000c950: 0a20 2020 2020 2020 202a 2c0a 2020 2020  .        *,.    
-0000c960: 2020 2020 6462 3a20 4462 2c0a 2020 2020      db: Db,.    
-0000c970: 2020 2020 6375 723d 4e6f 6e65 2c0a 2020      cur=None,.  
-0000c980: 2020 2920 2d3e 204f 7074 696f 6e61 6c5b    ) -> Optional[
-0000c990: 4f72 6967 696e 5669 7369 745d 3a0a 2020  OriginVisit]:.  
-0000c9a0: 2020 2020 2020 6966 2061 6c6c 6f77 6564        if allowed
-0000c9b0: 5f73 7461 7475 7365 7320 616e 6420 6e6f  _statuses and no
-0000c9c0: 7420 7365 7428 616c 6c6f 7765 645f 7374  t set(allowed_st
-0000c9d0: 6174 7573 6573 292e 696e 7465 7273 6563  atuses).intersec
-0000c9e0: 7469 6f6e 2856 4953 4954 5f53 5441 5455  tion(VISIT_STATU
-0000c9f0: 5345 5329 3a0a 2020 2020 2020 2020 2020  SES):.          
-0000ca00: 2020 7261 6973 6520 5374 6f72 6167 6541    raise StorageA
-0000ca10: 7267 756d 656e 7445 7863 6570 7469 6f6e  rgumentException
-0000ca20: 280a 2020 2020 2020 2020 2020 2020 2020  (.              
-0000ca30: 2020 6622 556e 6b6e 6f77 6e20 616c 6c6f    f"Unknown allo
-0000ca40: 7765 6420 7374 6174 7573 6573 207b 272c  wed statuses {',
-0000ca50: 272e 6a6f 696e 2861 6c6c 6f77 6564 5f73  '.join(allowed_s
-0000ca60: 7461 7475 7365 7329 7d2c 206f 6e6c 7920  tatuses)}, only 
-0000ca70: 220a 2020 2020 2020 2020 2020 2020 2020  ".              
-0000ca80: 2020 6622 7b27 2c27 2e6a 6f69 6e28 5649    f"{','.join(VI
-0000ca90: 5349 545f 5354 4154 5553 4553 297d 2061  SIT_STATUSES)} a
-0000caa0: 7574 686f 7269 7a65 6422 0a20 2020 2020  uthorized".     
-0000cab0: 2020 2020 2020 2029 0a0a 2020 2020 2020         )..      
-0000cac0: 2020 726f 7720 3d20 6462 2e6f 7269 6769    row = db.origi
-0000cad0: 6e5f 7669 7369 745f 6765 745f 6c61 7465  n_visit_get_late
-0000cae0: 7374 280a 2020 2020 2020 2020 2020 2020  st(.            
-0000caf0: 6f72 6967 696e 2c0a 2020 2020 2020 2020  origin,.        
-0000cb00: 2020 2020 7479 7065 3d74 7970 652c 0a20      type=type,. 
-0000cb10: 2020 2020 2020 2020 2020 2061 6c6c 6f77             allow
-0000cb20: 6564 5f73 7461 7475 7365 733d 616c 6c6f  ed_statuses=allo
-0000cb30: 7765 645f 7374 6174 7573 6573 2c0a 2020  wed_statuses,.  
-0000cb40: 2020 2020 2020 2020 2020 7265 7175 6972            requir
-0000cb50: 655f 736e 6170 7368 6f74 3d72 6571 7569  e_snapshot=requi
-0000cb60: 7265 5f73 6e61 7073 686f 742c 0a20 2020  re_snapshot,.   
-0000cb70: 2020 2020 2020 2020 2063 7572 3d63 7572           cur=cur
-0000cb80: 2c0a 2020 2020 2020 2020 290a 2020 2020  ,.        ).    
-0000cb90: 2020 2020 6966 2072 6f77 3a0a 2020 2020      if row:.    
-0000cba0: 2020 2020 2020 2020 726f 775f 6420 3d20          row_d = 
-0000cbb0: 6469 6374 287a 6970 2864 622e 6f72 6967  dict(zip(db.orig
-0000cbc0: 696e 5f76 6973 6974 5f67 6574 5f63 6f6c  in_visit_get_col
-0000cbd0: 732c 2072 6f77 2929 0a20 2020 2020 2020  s, row)).       
-0000cbe0: 2020 2020 2061 7373 6572 7420 280a 2020       assert (.  
-0000cbf0: 2020 2020 2020 2020 2020 2020 2020 726f                ro
-0000cc00: 775f 645b 2276 6973 6974 225d 2069 7320  w_d["visit"] is 
-0000cc10: 6e6f 7420 4e6f 6e65 0a20 2020 2020 2020  not None.       
-0000cc20: 2020 2020 2029 2c20 226f 7269 6769 6e5f       ), "origin_
-0000cc30: 7669 7369 745f 7374 6174 7573 204c 4546  visit_status LEF
-0000cc40: 5420 4a4f 494e 206f 7269 6769 6e5f 7669  T JOIN origin_vi
-0000cc50: 7369 7420 7265 7475 726e 6564 204e 554c  sit returned NUL
-0000cc60: 4c22 0a20 2020 2020 2020 2020 2020 2076  L".            v
-0000cc70: 6973 6974 203d 204f 7269 6769 6e56 6973  isit = OriginVis
-0000cc80: 6974 280a 2020 2020 2020 2020 2020 2020  it(.            
-0000cc90: 2020 2020 6f72 6967 696e 3d72 6f77 5f64      origin=row_d
-0000cca0: 5b22 6f72 6967 696e 225d 2c0a 2020 2020  ["origin"],.    
-0000ccb0: 2020 2020 2020 2020 2020 2020 7669 7369              visi
-0000ccc0: 743d 726f 775f 645b 2276 6973 6974 225d  t=row_d["visit"]
-0000ccd0: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-0000cce0: 2020 6461 7465 3d72 6f77 5f64 5b22 6461    date=row_d["da
-0000ccf0: 7465 225d 2c0a 2020 2020 2020 2020 2020  te"],.          
-0000cd00: 2020 2020 2020 7479 7065 3d72 6f77 5f64        type=row_d
-0000cd10: 5b22 7479 7065 225d 2c0a 2020 2020 2020  ["type"],.      
-0000cd20: 2020 2020 2020 290a 2020 2020 2020 2020        ).        
-0000cd30: 2020 2020 7265 7475 726e 2076 6973 6974      return visit
-0000cd40: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
-0000cd50: 4e6f 6e65 0a0a 2020 2020 4064 625f 7472  None..    @db_tr
-0000cd60: 616e 7361 6374 696f 6e28 7374 6174 656d  ansaction(statem
-0000cd70: 656e 745f 7469 6d65 6f75 743d 3530 3029  ent_timeout=500)
-0000cd80: 0a20 2020 2064 6566 206f 7269 6769 6e5f  .    def origin_
-0000cd90: 7669 7369 745f 7374 6174 7573 5f67 6574  visit_status_get
-0000cda0: 280a 2020 2020 2020 2020 7365 6c66 2c0a  (.        self,.
-0000cdb0: 2020 2020 2020 2020 6f72 6967 696e 3a20          origin: 
-0000cdc0: 7374 722c 0a20 2020 2020 2020 2076 6973  str,.        vis
-0000cdd0: 6974 3a20 696e 742c 0a20 2020 2020 2020  it: int,.       
-0000cde0: 2070 6167 655f 746f 6b65 6e3a 204f 7074   page_token: Opt
-0000cdf0: 696f 6e61 6c5b 7374 725d 203d 204e 6f6e  ional[str] = Non
-0000ce00: 652c 0a20 2020 2020 2020 206f 7264 6572  e,.        order
-0000ce10: 3a20 4c69 7374 4f72 6465 7220 3d20 4c69  : ListOrder = Li
-0000ce20: 7374 4f72 6465 722e 4153 432c 0a20 2020  stOrder.ASC,.   
-0000ce30: 2020 2020 206c 696d 6974 3a20 696e 7420       limit: int 
-0000ce40: 3d20 3130 2c0a 2020 2020 2020 2020 2a2c  = 10,.        *,
-0000ce50: 0a20 2020 2020 2020 2064 623a 2044 622c  .        db: Db,
-0000ce60: 0a20 2020 2020 2020 2063 7572 3d4e 6f6e  .        cur=Non
-0000ce70: 652c 0a20 2020 2029 202d 3e20 5061 6765  e,.    ) -> Page
-0000ce80: 6452 6573 756c 745b 4f72 6967 696e 5669  dResult[OriginVi
-0000ce90: 7369 7453 7461 7475 735d 3a0a 2020 2020  sitStatus]:.    
-0000cea0: 2020 2020 6e65 7874 5f70 6167 655f 746f      next_page_to
-0000ceb0: 6b65 6e20 3d20 4e6f 6e65 0a20 2020 2020  ken = None.     
-0000cec0: 2020 2064 6174 655f 6672 6f6d 203d 204e     date_from = N
-0000ced0: 6f6e 650a 2020 2020 2020 2020 6966 2070  one.        if p
-0000cee0: 6167 655f 746f 6b65 6e20 6973 206e 6f74  age_token is not
-0000cef0: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
-0000cf00: 2020 2074 7279 3a0a 2020 2020 2020 2020     try:.        
-0000cf10: 2020 2020 2020 2020 6461 7465 5f66 726f          date_fro
-0000cf20: 6d20 3d20 6461 7465 7469 6d65 2e64 6174  m = datetime.dat
-0000cf30: 6574 696d 652e 6672 6f6d 6973 6f66 6f72  etime.fromisofor
-0000cf40: 6d61 7428 7061 6765 5f74 6f6b 656e 290a  mat(page_token).
-0000cf50: 2020 2020 2020 2020 2020 2020 6578 6365              exce
-0000cf60: 7074 2056 616c 7565 4572 726f 723a 0a20  pt ValueError:. 
-0000cf70: 2020 2020 2020 2020 2020 2020 2020 2072                 r
-0000cf80: 6169 7365 2053 746f 7261 6765 4172 6775  aise StorageArgu
-0000cf90: 6d65 6e74 4578 6365 7074 696f 6e28 0a20  mentException(. 
-0000cfa0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000cfb0: 2020 2022 496e 7661 6c69 6420 7061 6765     "Invalid page
-0000cfc0: 5f74 6f6b 656e 2061 7267 756d 656e 7420  _token argument 
-0000cfd0: 746f 206f 7269 6769 6e5f 7669 7369 745f  to origin_visit_
-0000cfe0: 7374 6174 7573 5f67 6574 2e22 0a20 2020  status_get.".   
-0000cff0: 2020 2020 2020 2020 2020 2020 2029 2066               ) f
-0000d000: 726f 6d20 4e6f 6e65 0a0a 2020 2020 2020  rom None..      
-0000d010: 2020 7669 7369 745f 7374 6174 7573 6573    visit_statuses
-0000d020: 3a20 4c69 7374 5b4f 7269 6769 6e56 6973  : List[OriginVis
-0000d030: 6974 5374 6174 7573 5d20 3d20 5b5d 0a20  itStatus] = []. 
-0000d040: 2020 2020 2020 2023 2054 616b 6520 6f6e         # Take on
-0000d050: 6520 6d6f 7265 2076 6973 6974 2073 7461  e more visit sta
-0000d060: 7475 7320 736f 2077 6520 6361 6e20 7265  tus so we can re
-0000d070: 7573 6520 6974 2061 7320 7468 6520 6e65  use it as the ne
-0000d080: 7874 2070 6167 6520 746f 6b65 6e20 6966  xt page token if
-0000d090: 2061 6e79 0a20 2020 2020 2020 2066 6f72   any.        for
-0000d0a0: 2072 6f77 2069 6e20 6462 2e6f 7269 6769   row in db.origi
-0000d0b0: 6e5f 7669 7369 745f 7374 6174 7573 5f67  n_visit_status_g
-0000d0c0: 6574 5f72 616e 6765 280a 2020 2020 2020  et_range(.      
-0000d0d0: 2020 2020 2020 6f72 6967 696e 2c0a 2020        origin,.  
-0000d0e0: 2020 2020 2020 2020 2020 7669 7369 742c            visit,
-0000d0f0: 0a20 2020 2020 2020 2020 2020 2064 6174  .            dat
-0000d100: 655f 6672 6f6d 3d64 6174 655f 6672 6f6d  e_from=date_from
-0000d110: 2c0a 2020 2020 2020 2020 2020 2020 6f72  ,.            or
-0000d120: 6465 723d 6f72 6465 722c 0a20 2020 2020  der=order,.     
-0000d130: 2020 2020 2020 206c 696d 6974 3d6c 696d         limit=lim
-0000d140: 6974 202b 2031 2c0a 2020 2020 2020 2020  it + 1,.        
-0000d150: 2020 2020 6375 723d 6375 722c 0a20 2020      cur=cur,.   
-0000d160: 2020 2020 2029 3a0a 2020 2020 2020 2020       ):.        
-0000d170: 2020 2020 726f 775f 6420 3d20 6469 6374      row_d = dict
-0000d180: 287a 6970 2864 622e 6f72 6967 696e 5f76  (zip(db.origin_v
-0000d190: 6973 6974 5f73 7461 7475 735f 636f 6c73  isit_status_cols
-0000d1a0: 2c20 726f 7729 290a 2020 2020 2020 2020  , row)).        
-0000d1b0: 2020 2020 7669 7369 745f 7374 6174 7573      visit_status
-0000d1c0: 6573 2e61 7070 656e 6428 4f72 6967 696e  es.append(Origin
-0000d1d0: 5669 7369 7453 7461 7475 7328 2a2a 726f  VisitStatus(**ro
-0000d1e0: 775f 6429 290a 0a20 2020 2020 2020 2069  w_d))..        i
-0000d1f0: 6620 6c65 6e28 7669 7369 745f 7374 6174  f len(visit_stat
-0000d200: 7573 6573 2920 3e20 6c69 6d69 743a 0a20  uses) > limit:. 
-0000d210: 2020 2020 2020 2020 2020 2023 206c 6173             # las
-0000d220: 7420 7669 7369 7420 7374 6174 7573 2064  t visit status d
-0000d230: 6174 6520 6973 2074 6865 206e 6578 7420  ate is the next 
-0000d240: 7061 6765 2074 6f6b 656e 0a20 2020 2020  page token.     
-0000d250: 2020 2020 2020 206e 6578 745f 7061 6765         next_page
-0000d260: 5f74 6f6b 656e 203d 2073 7472 2876 6973  _token = str(vis
-0000d270: 6974 5f73 7461 7475 7365 735b 2d31 5d2e  it_statuses[-1].
-0000d280: 6461 7465 290a 2020 2020 2020 2020 2020  date).          
-0000d290: 2020 2320 6578 636c 7564 696e 6720 7468    # excluding th
-0000d2a0: 6174 2076 6973 6974 2073 7461 7475 7320  at visit status 
-0000d2b0: 6672 6f6d 2074 6865 2072 6573 756c 7420  from the result 
-0000d2c0: 746f 2072 6573 7065 6374 2074 6865 206c  to respect the l
-0000d2d0: 696d 6974 2073 697a 650a 2020 2020 2020  imit size.      
-0000d2e0: 2020 2020 2020 7669 7369 745f 7374 6174        visit_stat
-0000d2f0: 7573 6573 203d 2076 6973 6974 5f73 7461  uses = visit_sta
-0000d300: 7475 7365 735b 3a6c 696d 6974 5d0a 0a20  tuses[:limit].. 
-0000d310: 2020 2020 2020 2072 6574 7572 6e20 5061         return Pa
-0000d320: 6765 6452 6573 756c 7428 7265 7375 6c74  gedResult(result
-0000d330: 733d 7669 7369 745f 7374 6174 7573 6573  s=visit_statuses
-0000d340: 2c20 6e65 7874 5f70 6167 655f 746f 6b65  , next_page_toke
-0000d350: 6e3d 6e65 7874 5f70 6167 655f 746f 6b65  n=next_page_toke
-0000d360: 6e29 0a0a 2020 2020 4064 625f 7472 616e  n)..    @db_tran
-0000d370: 7361 6374 696f 6e28 290a 2020 2020 6465  saction().    de
-0000d380: 6620 6f72 6967 696e 5f76 6973 6974 5f73  f origin_visit_s
-0000d390: 7461 7475 735f 6765 745f 7261 6e64 6f6d  tatus_get_random
-0000d3a0: 280a 2020 2020 2020 2020 7365 6c66 2c20  (.        self, 
-0000d3b0: 7479 7065 3a20 7374 722c 202a 2c20 6462  type: str, *, db
-0000d3c0: 3a20 4462 2c20 6375 723d 4e6f 6e65 0a20  : Db, cur=None. 
-0000d3d0: 2020 2029 202d 3e20 4f70 7469 6f6e 616c     ) -> Optional
-0000d3e0: 5b4f 7269 6769 6e56 6973 6974 5374 6174  [OriginVisitStat
-0000d3f0: 7573 5d3a 0a20 2020 2020 2020 2072 6f77  us]:.        row
-0000d400: 203d 2064 622e 6f72 6967 696e 5f76 6973   = db.origin_vis
-0000d410: 6974 5f67 6574 5f72 616e 646f 6d28 7479  it_get_random(ty
-0000d420: 7065 2c20 6375 7229 0a20 2020 2020 2020  pe, cur).       
-0000d430: 2069 6620 726f 7720 6973 206e 6f74 204e   if row is not N
-0000d440: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
-0000d450: 2072 6f77 5f64 203d 2064 6963 7428 7a69   row_d = dict(zi
-0000d460: 7028 6462 2e6f 7269 6769 6e5f 7669 7369  p(db.origin_visi
-0000d470: 745f 7374 6174 7573 5f63 6f6c 732c 2072  t_status_cols, r
-0000d480: 6f77 2929 0a20 2020 2020 2020 2020 2020  ow)).           
-0000d490: 2072 6574 7572 6e20 4f72 6967 696e 5669   return OriginVi
-0000d4a0: 7369 7453 7461 7475 7328 2a2a 726f 775f  sitStatus(**row_
-0000d4b0: 6429 0a20 2020 2020 2020 2072 6574 7572  d).        retur
-0000d4c0: 6e20 4e6f 6e65 0a0a 2020 2020 2323 2323  n None..    ####
-0000d4d0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-0000d4e0: 2323 2323 2323 0a20 2020 2023 204f 7269  ######.    # Ori
-0000d4f0: 6769 6e0a 2020 2020 2323 2323 2323 2323  gin.    ########
-0000d500: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-0000d510: 2323 0a0a 2020 2020 4064 625f 7472 616e  ##..    @db_tran
-0000d520: 7361 6374 696f 6e28 7374 6174 656d 656e  saction(statemen
-0000d530: 745f 7469 6d65 6f75 743d 3130 3030 290a  t_timeout=1000).
-0000d540: 2020 2020 6465 6620 6f72 6967 696e 5f67      def origin_g
-0000d550: 6574 280a 2020 2020 2020 2020 7365 6c66  et(.        self
-0000d560: 2c20 6f72 6967 696e 733a 204c 6973 745b  , origins: List[
-0000d570: 7374 725d 2c20 2a2c 2064 623a 2044 622c  str], *, db: Db,
-0000d580: 2063 7572 3d4e 6f6e 650a 2020 2020 2920   cur=None.    ) 
-0000d590: 2d3e 2049 7465 7261 626c 655b 4f70 7469  -> Iterable[Opti
-0000d5a0: 6f6e 616c 5b4f 7269 6769 6e5d 5d3a 0a20  onal[Origin]]:. 
-0000d5b0: 2020 2020 2020 2072 6f77 7320 3d20 6462         rows = db
-0000d5c0: 2e6f 7269 6769 6e5f 6765 745f 6279 5f75  .origin_get_by_u
-0000d5d0: 726c 286f 7269 6769 6e73 2c20 6375 7229  rl(origins, cur)
-0000d5e0: 0a20 2020 2020 2020 2072 6573 756c 743a  .        result:
-0000d5f0: 204c 6973 745b 4f70 7469 6f6e 616c 5b4f   List[Optional[O
-0000d600: 7269 6769 6e5d 5d20 3d20 5b5d 0a20 2020  rigin]] = [].   
-0000d610: 2020 2020 2066 6f72 2072 6f77 2069 6e20       for row in 
-0000d620: 726f 7773 3a0a 2020 2020 2020 2020 2020  rows:.          
-0000d630: 2020 6f72 6967 696e 5f64 203d 2064 6963    origin_d = dic
-0000d640: 7428 7a69 7028 6462 2e6f 7269 6769 6e5f  t(zip(db.origin_
-0000d650: 636f 6c73 2c20 726f 7729 290a 2020 2020  cols, row)).    
-0000d660: 2020 2020 2020 2020 7572 6c20 3d20 6f72          url = or
-0000d670: 6967 696e 5f64 5b22 7572 6c22 5d0a 2020  igin_d["url"].  
-0000d680: 2020 2020 2020 2020 2020 7265 7375 6c74            result
-0000d690: 2e61 7070 656e 6428 4e6f 6e65 2069 6620  .append(None if 
-0000d6a0: 7572 6c20 6973 204e 6f6e 6520 656c 7365  url is None else
-0000d6b0: 204f 7269 6769 6e28 7572 6c3d 7572 6c29   Origin(url=url)
-0000d6c0: 290a 2020 2020 2020 2020 7265 7475 726e  ).        return
-0000d6d0: 2072 6573 756c 740a 0a20 2020 2040 6462   result..    @db
-0000d6e0: 5f74 7261 6e73 6163 7469 6f6e 2873 7461  _transaction(sta
-0000d6f0: 7465 6d65 6e74 5f74 696d 656f 7574 3d31  tement_timeout=1
-0000d700: 3030 3029 0a20 2020 2064 6566 206f 7269  000).    def ori
-0000d710: 6769 6e5f 6765 745f 6279 5f73 6861 3128  gin_get_by_sha1(
-0000d720: 0a20 2020 2020 2020 2073 656c 662c 2073  .        self, s
-0000d730: 6861 3173 3a20 4c69 7374 5b62 7974 6573  ha1s: List[bytes
-0000d740: 5d2c 202a 2c20 6462 3a20 4462 2c20 6375  ], *, db: Db, cu
-0000d750: 723d 4e6f 6e65 0a20 2020 2029 202d 3e20  r=None.    ) -> 
-0000d760: 4c69 7374 5b4f 7074 696f 6e61 6c5b 4469  List[Optional[Di
-0000d770: 6374 5b73 7472 2c20 416e 795d 5d5d 3a0a  ct[str, Any]]]:.
-0000d780: 2020 2020 2020 2020 7265 7475 726e 205b          return [
-0000d790: 0a20 2020 2020 2020 2020 2020 2064 6963  .            dic
-0000d7a0: 7428 7a69 7028 6462 2e6f 7269 6769 6e5f  t(zip(db.origin_
-0000d7b0: 636f 6c73 2c20 726f 7729 2920 6966 2072  cols, row)) if r
-0000d7c0: 6f77 5b30 5d20 656c 7365 204e 6f6e 650a  ow[0] else None.
-0000d7d0: 2020 2020 2020 2020 2020 2020 666f 7220              for 
-0000d7e0: 726f 7720 696e 2064 622e 6f72 6967 696e  row in db.origin
-0000d7f0: 5f67 6574 5f62 795f 7368 6131 2873 6861  _get_by_sha1(sha
-0000d800: 3173 2c20 6375 7229 0a20 2020 2020 2020  1s, cur).       
-0000d810: 205d 0a0a 2020 2020 4064 625f 7472 616e   ]..    @db_tran
-0000d820: 7361 6374 696f 6e5f 6765 6e65 7261 746f  saction_generato
-0000d830: 7228 290a 2020 2020 6465 6620 6f72 6967  r().    def orig
-0000d840: 696e 5f67 6574 5f72 616e 6765 2873 656c  in_get_range(sel
-0000d850: 662c 206f 7269 6769 6e5f 6672 6f6d 3d31  f, origin_from=1
-0000d860: 2c20 6f72 6967 696e 5f63 6f75 6e74 3d31  , origin_count=1
-0000d870: 3030 2c20 2a2c 2064 623a 2044 622c 2063  00, *, db: Db, c
-0000d880: 7572 3d4e 6f6e 6529 3a0a 2020 2020 2020  ur=None):.      
-0000d890: 2020 666f 7220 6f72 6967 696e 2069 6e20    for origin in 
-0000d8a0: 6462 2e6f 7269 6769 6e5f 6765 745f 7261  db.origin_get_ra
-0000d8b0: 6e67 6528 6f72 6967 696e 5f66 726f 6d2c  nge(origin_from,
-0000d8c0: 206f 7269 6769 6e5f 636f 756e 742c 2063   origin_count, c
-0000d8d0: 7572 293a 0a20 2020 2020 2020 2020 2020  ur):.           
-0000d8e0: 2079 6965 6c64 2064 6963 7428 7a69 7028   yield dict(zip(
-0000d8f0: 6462 2e6f 7269 6769 6e5f 6765 745f 7261  db.origin_get_ra
-0000d900: 6e67 655f 636f 6c73 2c20 6f72 6967 696e  nge_cols, origin
-0000d910: 2929 0a0a 2020 2020 4064 625f 7472 616e  ))..    @db_tran
-0000d920: 7361 6374 696f 6e28 290a 2020 2020 6465  saction().    de
-0000d930: 6620 6f72 6967 696e 5f6c 6973 7428 0a20  f origin_list(. 
-0000d940: 2020 2020 2020 2073 656c 662c 2070 6167         self, pag
-0000d950: 655f 746f 6b65 6e3a 204f 7074 696f 6e61  e_token: Optiona
-0000d960: 6c5b 7374 725d 203d 204e 6f6e 652c 206c  l[str] = None, l
-0000d970: 696d 6974 3a20 696e 7420 3d20 3130 302c  imit: int = 100,
-0000d980: 202a 2c20 6462 3a20 4462 2c20 6375 723d   *, db: Db, cur=
-0000d990: 4e6f 6e65 0a20 2020 2029 202d 3e20 5061  None.    ) -> Pa
-0000d9a0: 6765 6452 6573 756c 745b 4f72 6967 696e  gedResult[Origin
-0000d9b0: 5d3a 0a20 2020 2020 2020 2070 6167 655f  ]:.        page_
-0000d9c0: 746f 6b65 6e20 3d20 7061 6765 5f74 6f6b  token = page_tok
-0000d9d0: 656e 206f 7220 2230 220a 2020 2020 2020  en or "0".      
-0000d9e0: 2020 6966 206e 6f74 2069 7369 6e73 7461    if not isinsta
-0000d9f0: 6e63 6528 7061 6765 5f74 6f6b 656e 2c20  nce(page_token, 
-0000da00: 7374 7229 3a0a 2020 2020 2020 2020 2020  str):.          
-0000da10: 2020 7261 6973 6520 5374 6f72 6167 6541    raise StorageA
-0000da20: 7267 756d 656e 7445 7863 6570 7469 6f6e  rgumentException
-0000da30: 2822 7061 6765 5f74 6f6b 656e 206d 7573  ("page_token mus
-0000da40: 7420 6265 2061 2073 7472 696e 672e 2229  t be a string.")
-0000da50: 0a20 2020 2020 2020 206f 7269 6769 6e5f  .        origin_
-0000da60: 6672 6f6d 203d 2069 6e74 2870 6167 655f  from = int(page_
-0000da70: 746f 6b65 6e29 0a20 2020 2020 2020 206e  token).        n
-0000da80: 6578 745f 7061 6765 5f74 6f6b 656e 203d  ext_page_token =
-0000da90: 204e 6f6e 650a 0a20 2020 2020 2020 206f   None..        o
-0000daa0: 7269 6769 6e73 3a20 4c69 7374 5b4f 7269  rigins: List[Ori
-0000dab0: 6769 6e5d 203d 205b 5d0a 2020 2020 2020  gin] = [].      
-0000dac0: 2020 2320 5461 6b65 206f 6e65 206d 6f72    # Take one mor
-0000dad0: 6520 6f72 6967 696e 2073 6f20 7765 2063  e origin so we c
-0000dae0: 616e 2072 6575 7365 2069 7420 6173 2074  an reuse it as t
-0000daf0: 6865 206e 6578 7420 7061 6765 2074 6f6b  he next page tok
-0000db00: 656e 2069 6620 616e 790a 2020 2020 2020  en if any.      
-0000db10: 2020 666f 7220 726f 775f 6420 696e 2073    for row_d in s
-0000db20: 656c 662e 6f72 6967 696e 5f67 6574 5f72  elf.origin_get_r
-0000db30: 616e 6765 286f 7269 6769 6e5f 6672 6f6d  ange(origin_from
-0000db40: 2c20 6c69 6d69 7420 2b20 312c 2064 623d  , limit + 1, db=
-0000db50: 6462 2c20 6375 723d 6375 7229 3a0a 2020  db, cur=cur):.  
-0000db60: 2020 2020 2020 2020 2020 6f72 6967 696e            origin
-0000db70: 732e 6170 7065 6e64 284f 7269 6769 6e28  s.append(Origin(
-0000db80: 7572 6c3d 726f 775f 645b 2275 726c 225d  url=row_d["url"]
-0000db90: 2929 0a20 2020 2020 2020 2020 2020 2023  )).            #
-0000dba0: 206b 6565 7020 7468 6520 6c61 7374 5f69   keep the last_i
-0000dbb0: 6420 666f 7220 7468 6520 7061 6769 6e61  d for the pagina
-0000dbc0: 7469 6f6e 2069 6620 6e65 6564 6564 0a20  tion if needed. 
-0000dbd0: 2020 2020 2020 2020 2020 206c 6173 745f             last_
-0000dbe0: 6964 203d 2072 6f77 5f64 5b22 6964 225d  id = row_d["id"]
-0000dbf0: 0a0a 2020 2020 2020 2020 6966 206c 656e  ..        if len
-0000dc00: 286f 7269 6769 6e73 2920 3e20 6c69 6d69  (origins) > limi
-0000dc10: 743a 2020 2320 6461 7461 206c 6566 7420  t:  # data left 
-0000dc20: 666f 7220 7375 6273 6571 7565 6e74 2063  for subsequent c
-0000dc30: 616c 6c0a 2020 2020 2020 2020 2020 2020  all.            
-0000dc40: 2320 6c61 7374 206f 7269 6769 6e20 6964  # last origin id
-0000dc50: 2069 7320 7468 6520 6e65 7874 2070 6167   is the next pag
-0000dc60: 6520 746f 6b65 6e0a 2020 2020 2020 2020  e token.        
-0000dc70: 2020 2020 6e65 7874 5f70 6167 655f 746f      next_page_to
-0000dc80: 6b65 6e20 3d20 7374 7228 6c61 7374 5f69  ken = str(last_i
-0000dc90: 6429 0a20 2020 2020 2020 2020 2020 2023  d).            #
-0000dca0: 2065 7863 6c75 6469 6e67 2074 6861 7420   excluding that 
-0000dcb0: 6f72 6967 696e 2066 726f 6d20 7468 6520  origin from the 
-0000dcc0: 7265 7375 6c74 2074 6f20 7265 7370 6563  result to respec
-0000dcd0: 7420 7468 6520 6c69 6d69 7420 7369 7a65  t the limit size
-0000dce0: 0a20 2020 2020 2020 2020 2020 206f 7269  .            ori
-0000dcf0: 6769 6e73 203d 206f 7269 6769 6e73 5b3a  gins = origins[:
-0000dd00: 6c69 6d69 745d 0a0a 2020 2020 2020 2020  limit]..        
-0000dd10: 6173 7365 7274 206c 656e 286f 7269 6769  assert len(origi
-0000dd20: 6e73 2920 3c3d 206c 696d 6974 0a20 2020  ns) <= limit.   
-0000dd30: 2020 2020 2072 6574 7572 6e20 5061 6765       return Page
-0000dd40: 6452 6573 756c 7428 7265 7375 6c74 733d  dResult(results=
-0000dd50: 6f72 6967 696e 732c 206e 6578 745f 7061  origins, next_pa
-0000dd60: 6765 5f74 6f6b 656e 3d6e 6578 745f 7061  ge_token=next_pa
-0000dd70: 6765 5f74 6f6b 656e 290a 0a20 2020 2040  ge_token)..    @
-0000dd80: 6462 5f74 7261 6e73 6163 7469 6f6e 2829  db_transaction()
-0000dd90: 0a20 2020 2064 6566 206f 7269 6769 6e5f  .    def origin_
-0000dda0: 7365 6172 6368 280a 2020 2020 2020 2020  search(.        
-0000ddb0: 7365 6c66 2c0a 2020 2020 2020 2020 7572  self,.        ur
-0000ddc0: 6c5f 7061 7474 6572 6e3a 2073 7472 2c0a  l_pattern: str,.
-0000ddd0: 2020 2020 2020 2020 7061 6765 5f74 6f6b          page_tok
-0000dde0: 656e 3a20 4f70 7469 6f6e 616c 5b73 7472  en: Optional[str
-0000ddf0: 5d20 3d20 4e6f 6e65 2c0a 2020 2020 2020  ] = None,.      
-0000de00: 2020 6c69 6d69 743a 2069 6e74 203d 2035    limit: int = 5
-0000de10: 302c 0a20 2020 2020 2020 2072 6567 6578  0,.        regex
-0000de20: 703a 2062 6f6f 6c20 3d20 4661 6c73 652c  p: bool = False,
-0000de30: 0a20 2020 2020 2020 2077 6974 685f 7669  .        with_vi
-0000de40: 7369 743a 2062 6f6f 6c20 3d20 4661 6c73  sit: bool = Fals
-0000de50: 652c 0a20 2020 2020 2020 2076 6973 6974  e,.        visit
-0000de60: 5f74 7970 6573 3a20 4f70 7469 6f6e 616c  _types: Optional
-0000de70: 5b4c 6973 745b 7374 725d 5d20 3d20 4e6f  [List[str]] = No
-0000de80: 6e65 2c0a 2020 2020 2020 2020 2a2c 0a20  ne,.        *,. 
-0000de90: 2020 2020 2020 2064 623a 2044 622c 0a20         db: Db,. 
-0000dea0: 2020 2020 2020 2063 7572 3d4e 6f6e 652c         cur=None,
-0000deb0: 0a20 2020 2029 202d 3e20 5061 6765 6452  .    ) -> PagedR
-0000dec0: 6573 756c 745b 4f72 6967 696e 5d3a 0a20  esult[Origin]:. 
-0000ded0: 2020 2020 2020 206e 6578 745f 7061 6765         next_page
-0000dee0: 5f74 6f6b 656e 203d 204e 6f6e 650a 2020  _token = None.  
-0000def0: 2020 2020 2020 6f66 6673 6574 203d 2069        offset = i
-0000df00: 6e74 2870 6167 655f 746f 6b65 6e29 2069  nt(page_token) i
-0000df10: 6620 7061 6765 5f74 6f6b 656e 2065 6c73  f page_token els
-0000df20: 6520 300a 0a20 2020 2020 2020 206f 7269  e 0..        ori
-0000df30: 6769 6e73 203d 205b 5d0a 2020 2020 2020  gins = [].      
-0000df40: 2020 2320 5461 6b65 206f 6e65 206d 6f72    # Take one mor
-0000df50: 6520 6f72 6967 696e 2073 6f20 7765 2063  e origin so we c
-0000df60: 616e 2072 6575 7365 2069 7420 6173 2074  an reuse it as t
-0000df70: 6865 206e 6578 7420 7061 6765 2074 6f6b  he next page tok
-0000df80: 656e 2069 6620 616e 790a 2020 2020 2020  en if any.      
-0000df90: 2020 666f 7220 6f72 6967 696e 2069 6e20    for origin in 
-0000dfa0: 6462 2e6f 7269 6769 6e5f 7365 6172 6368  db.origin_search
-0000dfb0: 280a 2020 2020 2020 2020 2020 2020 7572  (.            ur
-0000dfc0: 6c5f 7061 7474 6572 6e2c 206f 6666 7365  l_pattern, offse
-0000dfd0: 742c 206c 696d 6974 202b 2031 2c20 7265  t, limit + 1, re
-0000dfe0: 6765 7870 2c20 7769 7468 5f76 6973 6974  gexp, with_visit
-0000dff0: 2c20 7669 7369 745f 7479 7065 732c 2063  , visit_types, c
-0000e000: 7572 0a20 2020 2020 2020 2029 3a0a 2020  ur.        ):.  
-0000e010: 2020 2020 2020 2020 2020 726f 775f 6420            row_d 
-0000e020: 3d20 6469 6374 287a 6970 2864 622e 6f72  = dict(zip(db.or
-0000e030: 6967 696e 5f63 6f6c 732c 206f 7269 6769  igin_cols, origi
-0000e040: 6e29 290a 2020 2020 2020 2020 2020 2020  n)).            
-0000e050: 6f72 6967 696e 732e 6170 7065 6e64 284f  origins.append(O
-0000e060: 7269 6769 6e28 7572 6c3d 726f 775f 645b  rigin(url=row_d[
-0000e070: 2275 726c 225d 2929 0a0a 2020 2020 2020  "url"]))..      
-0000e080: 2020 6966 206c 656e 286f 7269 6769 6e73    if len(origins
-0000e090: 2920 3e20 6c69 6d69 743a 0a20 2020 2020  ) > limit:.     
-0000e0a0: 2020 2020 2020 2023 206e 6578 7420 6f66         # next of
-0000e0b0: 6673 6574 0a20 2020 2020 2020 2020 2020  fset.           
-0000e0c0: 206e 6578 745f 7061 6765 5f74 6f6b 656e   next_page_token
-0000e0d0: 203d 2073 7472 286f 6666 7365 7420 2b20   = str(offset + 
-0000e0e0: 6c69 6d69 7429 0a20 2020 2020 2020 2020  limit).         
-0000e0f0: 2020 2023 2065 7863 6c75 6469 6e67 2074     # excluding t
-0000e100: 6861 7420 6f72 6967 696e 2066 726f 6d20  hat origin from 
-0000e110: 7468 6520 7265 7375 6c74 2074 6f20 7265  the result to re
-0000e120: 7370 6563 7420 7468 6520 6c69 6d69 7420  spect the limit 
-0000e130: 7369 7a65 0a20 2020 2020 2020 2020 2020  size.           
-0000e140: 206f 7269 6769 6e73 203d 206f 7269 6769   origins = origi
-0000e150: 6e73 5b3a 6c69 6d69 745d 0a0a 2020 2020  ns[:limit]..    
-0000e160: 2020 2020 6173 7365 7274 206c 656e 286f      assert len(o
-0000e170: 7269 6769 6e73 2920 3c3d 206c 696d 6974  rigins) <= limit
-0000e180: 0a0a 2020 2020 2020 2020 7265 7475 726e  ..        return
-0000e190: 2050 6167 6564 5265 7375 6c74 2872 6573   PagedResult(res
-0000e1a0: 756c 7473 3d6f 7269 6769 6e73 2c20 6e65  ults=origins, ne
-0000e1b0: 7874 5f70 6167 655f 746f 6b65 6e3d 6e65  xt_page_token=ne
-0000e1c0: 7874 5f70 6167 655f 746f 6b65 6e29 0a0a  xt_page_token)..
-0000e1d0: 2020 2020 4064 625f 7472 616e 7361 6374      @db_transact
-0000e1e0: 696f 6e28 290a 2020 2020 6465 6620 6f72  ion().    def or
-0000e1f0: 6967 696e 5f63 6f75 6e74 280a 2020 2020  igin_count(.    
-0000e200: 2020 2020 7365 6c66 2c0a 2020 2020 2020      self,.      
-0000e210: 2020 7572 6c5f 7061 7474 6572 6e3a 2073    url_pattern: s
-0000e220: 7472 2c0a 2020 2020 2020 2020 7265 6765  tr,.        rege
-0000e230: 7870 3a20 626f 6f6c 203d 2046 616c 7365  xp: bool = False
-0000e240: 2c0a 2020 2020 2020 2020 7769 7468 5f76  ,.        with_v
-0000e250: 6973 6974 3a20 626f 6f6c 203d 2046 616c  isit: bool = Fal
-0000e260: 7365 2c0a 2020 2020 2020 2020 2a2c 0a20  se,.        *,. 
-0000e270: 2020 2020 2020 2064 623a 2044 622c 0a20         db: Db,. 
-0000e280: 2020 2020 2020 2063 7572 3d4e 6f6e 652c         cur=None,
-0000e290: 0a20 2020 2029 202d 3e20 696e 743a 0a20  .    ) -> int:. 
-0000e2a0: 2020 2020 2020 2072 6574 7572 6e20 6462         return db
-0000e2b0: 2e6f 7269 6769 6e5f 636f 756e 7428 7572  .origin_count(ur
-0000e2c0: 6c5f 7061 7474 6572 6e2c 2072 6567 6578  l_pattern, regex
-0000e2d0: 702c 2077 6974 685f 7669 7369 742c 2063  p, with_visit, c
-0000e2e0: 7572 290a 0a20 2020 2040 6462 5f74 7261  ur)..    @db_tra
-0000e2f0: 6e73 6163 7469 6f6e 2829 0a20 2020 2064  nsaction().    d
-0000e300: 6566 206f 7269 6769 6e5f 736e 6170 7368  ef origin_snapsh
-0000e310: 6f74 5f67 6574 5f61 6c6c 280a 2020 2020  ot_get_all(.    
-0000e320: 2020 2020 7365 6c66 2c20 6f72 6967 696e      self, origin
-0000e330: 5f75 726c 3a20 7374 722c 202a 2c20 6462  _url: str, *, db
-0000e340: 3a20 4462 2c20 6375 723d 4e6f 6e65 0a20  : Db, cur=None. 
-0000e350: 2020 2029 202d 3e20 4c69 7374 5b53 6861     ) -> List[Sha
-0000e360: 3147 6974 5d3a 0a20 2020 2020 2020 2072  1Git]:.        r
-0000e370: 6574 7572 6e20 6c69 7374 2864 622e 6f72  eturn list(db.or
-0000e380: 6967 696e 5f73 6e61 7073 686f 745f 6765  igin_snapshot_ge
-0000e390: 745f 616c 6c28 6f72 6967 696e 5f75 726c  t_all(origin_url
-0000e3a0: 2c20 6375 7229 290a 0a20 2020 2040 6462  , cur))..    @db
-0000e3b0: 5f74 7261 6e73 6163 7469 6f6e 2829 0a20  _transaction(). 
-0000e3c0: 2020 2064 6566 206f 7269 6769 6e5f 6164     def origin_ad
-0000e3d0: 6428 7365 6c66 2c20 6f72 6967 696e 733a  d(self, origins:
-0000e3e0: 204c 6973 745b 4f72 6967 696e 5d2c 202a   List[Origin], *
-0000e3f0: 2c20 6462 3a20 4462 2c20 6375 723d 4e6f  , db: Db, cur=No
-0000e400: 6e65 2920 2d3e 2044 6963 745b 7374 722c  ne) -> Dict[str,
-0000e410: 2069 6e74 5d3a 0a20 2020 2020 2020 2075   int]:.        u
-0000e420: 726c 7320 3d20 5b6f 2e75 726c 2066 6f72  rls = [o.url for
-0000e430: 206f 2069 6e20 6f72 6967 696e 735d 0a20   o in origins]. 
-0000e440: 2020 2020 2020 206b 6e6f 776e 5f6f 7269         known_ori
-0000e450: 6769 6e73 203d 2073 6574 2875 726c 2066  gins = set(url f
-0000e460: 6f72 2028 7572 6c2c 2920 696e 2064 622e  or (url,) in db.
-0000e470: 6f72 6967 696e 5f67 6574 5f62 795f 7572  origin_get_by_ur
-0000e480: 6c28 7572 6c73 2c20 6375 7229 290a 2020  l(urls, cur)).  
-0000e490: 2020 2020 2020 2320 6b65 6570 206f 6e6c        # keep onl
-0000e4a0: 7920 6f6e 6520 6f63 6375 7272 656e 6365  y one occurrence
-0000e4b0: 206f 6620 6561 6368 2067 6976 656e 206f   of each given o
-0000e4c0: 7269 6769 6e20 7768 696c 6520 6b65 6570  rigin while keep
-0000e4d0: 696e 6720 7468 6520 6c69 7374 0a20 2020  ing the list.   
-0000e4e0: 2020 2020 2023 2073 6f72 7465 6420 6173       # sorted as
-0000e4f0: 206f 7269 6769 6e61 6c6c 7920 6769 7665   originally give
-0000e500: 6e0a 2020 2020 2020 2020 746f 5f61 6464  n.        to_add
-0000e510: 203d 2073 6f72 7465 6428 7365 7428 7572   = sorted(set(ur
-0000e520: 6c73 2920 2d20 6b6e 6f77 6e5f 6f72 6967  ls) - known_orig
-0000e530: 696e 732c 206b 6579 3d75 726c 732e 696e  ins, key=urls.in
-0000e540: 6465 7829 0a0a 2020 2020 2020 2020 7365  dex)..        se
-0000e550: 6c66 2e6a 6f75 726e 616c 5f77 7269 7465  lf.journal_write
-0000e560: 722e 6f72 6967 696e 5f61 6464 285b 4f72  r.origin_add([Or
-0000e570: 6967 696e 2875 726c 3d75 726c 2920 666f  igin(url=url) fo
-0000e580: 7220 7572 6c20 696e 2074 6f5f 6164 645d  r url in to_add]
-0000e590: 290a 2020 2020 2020 2020 6164 6465 6420  ).        added 
-0000e5a0: 3d20 300a 2020 2020 2020 2020 666f 7220  = 0.        for 
-0000e5b0: 7572 6c20 696e 2074 6f5f 6164 643a 0a20  url in to_add:. 
-0000e5c0: 2020 2020 2020 2020 2020 2069 6620 6462             if db
-0000e5d0: 2e6f 7269 6769 6e5f 6164 6428 7572 6c2c  .origin_add(url,
-0000e5e0: 2063 7572 293a 0a20 2020 2020 2020 2020   cur):.         
-0000e5f0: 2020 2020 2020 2061 6464 6564 202b 3d20         added += 
-0000e600: 310a 2020 2020 2020 2020 7265 7475 726e  1.        return
-0000e610: 207b 226f 7269 6769 6e3a 6164 6422 3a20   {"origin:add": 
-0000e620: 6164 6465 647d 0a0a 2020 2020 2323 2323  added}..    ####
-0000e630: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-0000e640: 2323 2323 2323 0a20 2020 2023 206d 6973  ######.    # mis
-0000e650: 632e 0a20 2020 2023 2323 2323 2323 2323  c..    #########
-0000e660: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-0000e670: 230a 0a20 2020 2040 6462 5f74 7261 6e73  #..    @db_trans
-0000e680: 6163 7469 6f6e 2873 7461 7465 6d65 6e74  action(statement
-0000e690: 5f74 696d 656f 7574 3d32 3030 3029 0a20  _timeout=2000). 
-0000e6a0: 2020 2064 6566 206f 626a 6563 745f 6669     def object_fi
-0000e6b0: 6e64 5f62 795f 7368 6131 5f67 6974 280a  nd_by_sha1_git(.
-0000e6c0: 2020 2020 2020 2020 7365 6c66 2c20 6964          self, id
-0000e6d0: 733a 204c 6973 745b 5368 6131 4769 745d  s: List[Sha1Git]
-0000e6e0: 2c20 2a2c 2064 623a 2044 622c 2063 7572  , *, db: Db, cur
-0000e6f0: 3d4e 6f6e 650a 2020 2020 2920 2d3e 2044  =None.    ) -> D
-0000e700: 6963 745b 5368 6131 4769 742c 204c 6973  ict[Sha1Git, Lis
-0000e710: 745b 4469 6374 5d5d 3a0a 2020 2020 2020  t[Dict]]:.      
-0000e720: 2020 7265 743a 2044 6963 745b 5368 6131    ret: Dict[Sha1
-0000e730: 4769 742c 204c 6973 745b 4469 6374 5d5d  Git, List[Dict]]
-0000e740: 203d 207b 6964 3a20 5b5d 2066 6f72 2069   = {id: [] for i
-0000e750: 6420 696e 2069 6473 7d0a 0a20 2020 2020  d in ids}..     
-0000e760: 2020 2066 6f72 2072 6574 7661 6c20 696e     for retval in
-0000e770: 2064 622e 6f62 6a65 6374 5f66 696e 645f   db.object_find_
-0000e780: 6279 5f73 6861 315f 6769 7428 6964 732c  by_sha1_git(ids,
-0000e790: 2063 7572 3d63 7572 293a 0a20 2020 2020   cur=cur):.     
-0000e7a0: 2020 2020 2020 2069 6620 7265 7476 616c         if retval
-0000e7b0: 5b31 5d3a 0a20 2020 2020 2020 2020 2020  [1]:.           
-0000e7c0: 2020 2020 2072 6574 5b72 6574 7661 6c5b       ret[retval[
-0000e7d0: 305d 5d2e 6170 7065 6e64 280a 2020 2020  0]].append(.    
-0000e7e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e7f0: 6469 6374 287a 6970 2864 622e 6f62 6a65  dict(zip(db.obje
-0000e800: 6374 5f66 696e 645f 6279 5f73 6861 315f  ct_find_by_sha1_
-0000e810: 6769 745f 636f 6c73 2c20 7265 7476 616c  git_cols, retval
-0000e820: 2929 0a20 2020 2020 2020 2020 2020 2020  )).             
-0000e830: 2020 2029 0a0a 2020 2020 2020 2020 7265     )..        re
-0000e840: 7475 726e 2072 6574 0a0a 2020 2020 4064  turn ret..    @d
-0000e850: 625f 7472 616e 7361 6374 696f 6e28 7374  b_transaction(st
-0000e860: 6174 656d 656e 745f 7469 6d65 6f75 743d  atement_timeout=
-0000e870: 3530 3029 0a20 2020 2064 6566 2073 7461  500).    def sta
-0000e880: 745f 636f 756e 7465 7273 2873 656c 662c  t_counters(self,
-0000e890: 202a 2c20 6462 3a20 4462 2c20 6375 723d   *, db: Db, cur=
-0000e8a0: 4e6f 6e65 293a 0a20 2020 2020 2020 2072  None):.        r
-0000e8b0: 6574 7572 6e20 7b6b 3a20 7620 666f 7220  eturn {k: v for 
-0000e8c0: 286b 2c20 7629 2069 6e20 6462 2e73 7461  (k, v) in db.sta
-0000e8d0: 745f 636f 756e 7465 7273 2829 7d0a 0a20  t_counters()}.. 
-0000e8e0: 2020 2040 6462 5f74 7261 6e73 6163 7469     @db_transacti
-0000e8f0: 6f6e 2829 0a20 2020 2064 6566 2072 6566  on().    def ref
-0000e900: 7265 7368 5f73 7461 745f 636f 756e 7465  resh_stat_counte
-0000e910: 7273 2873 656c 662c 202a 2c20 6462 3a20  rs(self, *, db: 
-0000e920: 4462 2c20 6375 723d 4e6f 6e65 293a 0a20  Db, cur=None):. 
-0000e930: 2020 2020 2020 206b 6579 7320 3d20 5b0a         keys = [.
-0000e940: 2020 2020 2020 2020 2020 2020 2263 6f6e              "con
-0000e950: 7465 6e74 222c 0a20 2020 2020 2020 2020  tent",.         
-0000e960: 2020 2022 6469 7265 6374 6f72 7922 2c0a     "directory",.
-0000e970: 2020 2020 2020 2020 2020 2020 2264 6972              "dir
-0000e980: 6563 746f 7279 5f65 6e74 7279 5f64 6972  ectory_entry_dir
-0000e990: 222c 0a20 2020 2020 2020 2020 2020 2022  ",.            "
-0000e9a0: 6469 7265 6374 6f72 795f 656e 7472 795f  directory_entry_
-0000e9b0: 6669 6c65 222c 0a20 2020 2020 2020 2020  file",.         
-0000e9c0: 2020 2022 6469 7265 6374 6f72 795f 656e     "directory_en
-0000e9d0: 7472 795f 7265 7622 2c0a 2020 2020 2020  try_rev",.      
-0000e9e0: 2020 2020 2020 226f 7269 6769 6e22 2c0a        "origin",.
-0000e9f0: 2020 2020 2020 2020 2020 2020 226f 7269              "ori
-0000ea00: 6769 6e5f 7669 7369 7422 2c0a 2020 2020  gin_visit",.    
-0000ea10: 2020 2020 2020 2020 2270 6572 736f 6e22          "person"
-0000ea20: 2c0a 2020 2020 2020 2020 2020 2020 2272  ,.            "r
-0000ea30: 656c 6561 7365 222c 0a20 2020 2020 2020  elease",.       
-0000ea40: 2020 2020 2022 7265 7669 7369 6f6e 222c       "revision",
-0000ea50: 0a20 2020 2020 2020 2020 2020 2022 7265  .            "re
-0000ea60: 7669 7369 6f6e 5f68 6973 746f 7279 222c  vision_history",
-0000ea70: 0a20 2020 2020 2020 2020 2020 2022 736b  .            "sk
-0000ea80: 6970 7065 645f 636f 6e74 656e 7422 2c0a  ipped_content",.
-0000ea90: 2020 2020 2020 2020 2020 2020 2273 6e61              "sna
-0000eaa0: 7073 686f 7422 2c0a 2020 2020 2020 2020  pshot",.        
-0000eab0: 5d0a 0a20 2020 2020 2020 2066 6f72 206b  ]..        for k
-0000eac0: 6579 2069 6e20 6b65 7973 3a0a 2020 2020  ey in keys:.    
-0000ead0: 2020 2020 2020 2020 6375 722e 6578 6563          cur.exec
-0000eae0: 7574 6528 2273 656c 6563 7420 2a20 6672  ute("select * fr
-0000eaf0: 6f6d 2073 7768 5f75 7064 6174 655f 636f  om swh_update_co
-0000eb00: 756e 7465 7228 2573 2922 2c20 286b 6579  unter(%s)", (key
-0000eb10: 2c29 290a 0a20 2020 2023 2323 2323 2323  ,))..    #######
-0000eb20: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-0000eb30: 2323 230a 2020 2020 2320 5261 7745 7874  ###.    # RawExt
-0000eb40: 7269 6e73 6963 4d65 7461 6461 7461 0a20  rinsicMetadata. 
-0000eb50: 2020 2023 2323 2323 2323 2323 2323 2323     #############
-0000eb60: 2323 2323 2323 2323 2323 2323 230a 0a20  #############.. 
-0000eb70: 2020 2040 6462 5f74 7261 6e73 6163 7469     @db_transacti
-0000eb80: 6f6e 2829 0a20 2020 2064 6566 2072 6177  on().    def raw
-0000eb90: 5f65 7874 7269 6e73 6963 5f6d 6574 6164  _extrinsic_metad
-0000eba0: 6174 615f 6164 6428 0a20 2020 2020 2020  ata_add(.       
-0000ebb0: 2073 656c 662c 0a20 2020 2020 2020 206d   self,.        m
-0000ebc0: 6574 6164 6174 613a 204c 6973 745b 5261  etadata: List[Ra
-0000ebd0: 7745 7874 7269 6e73 6963 4d65 7461 6461  wExtrinsicMetada
-0000ebe0: 7461 5d2c 0a20 2020 2020 2020 2064 622c  ta],.        db,
-0000ebf0: 0a20 2020 2020 2020 2063 7572 2c0a 2020  .        cur,.  
-0000ec00: 2020 2920 2d3e 2044 6963 745b 7374 722c    ) -> Dict[str,
-0000ec10: 2069 6e74 5d3a 0a20 2020 2020 2020 206d   int]:.        m
-0000ec20: 6574 6164 6174 6120 3d20 6c69 7374 286d  etadata = list(m
-0000ec30: 6574 6164 6174 6129 0a20 2020 2020 2020  etadata).       
-0000ec40: 2073 656c 662e 6a6f 7572 6e61 6c5f 7772   self.journal_wr
-0000ec50: 6974 6572 2e72 6177 5f65 7874 7269 6e73  iter.raw_extrins
-0000ec60: 6963 5f6d 6574 6164 6174 615f 6164 6428  ic_metadata_add(
-0000ec70: 6d65 7461 6461 7461 290a 2020 2020 2020  metadata).      
-0000ec80: 2020 636f 756e 7465 7220 3d20 436f 756e    counter = Coun
-0000ec90: 7465 725b 4578 7465 6e64 6564 4f62 6a65  ter[ExtendedObje
-0000eca0: 6374 5479 7065 5d28 290a 2020 2020 2020  ctType]().      
-0000ecb0: 2020 666f 7220 6d65 7461 6461 7461 5f65    for metadata_e
-0000ecc0: 6e74 7279 2069 6e20 6d65 7461 6461 7461  ntry in metadata
-0000ecd0: 3a0a 2020 2020 2020 2020 2020 2020 6175  :.            au
-0000ece0: 7468 6f72 6974 795f 6964 203d 2073 656c  thority_id = sel
-0000ecf0: 662e 5f67 6574 5f61 7574 686f 7269 7479  f._get_authority
-0000ed00: 5f69 6428 6d65 7461 6461 7461 5f65 6e74  _id(metadata_ent
-0000ed10: 7279 2e61 7574 686f 7269 7479 2c20 6462  ry.authority, db
-0000ed20: 2c20 6375 7229 0a20 2020 2020 2020 2020  , cur).         
-0000ed30: 2020 2066 6574 6368 6572 5f69 6420 3d20     fetcher_id = 
-0000ed40: 7365 6c66 2e5f 6765 745f 6665 7463 6865  self._get_fetche
-0000ed50: 725f 6964 286d 6574 6164 6174 615f 656e  r_id(metadata_en
-0000ed60: 7472 792e 6665 7463 6865 722c 2064 622c  try.fetcher, db,
-0000ed70: 2063 7572 290a 0a20 2020 2020 2020 2020   cur)..         
-0000ed80: 2020 2064 622e 7261 775f 6578 7472 696e     db.raw_extrin
-0000ed90: 7369 635f 6d65 7461 6461 7461 5f61 6464  sic_metadata_add
-0000eda0: 280a 2020 2020 2020 2020 2020 2020 2020  (.              
-0000edb0: 2020 6964 3d6d 6574 6164 6174 615f 656e    id=metadata_en
-0000edc0: 7472 792e 6964 2c0a 2020 2020 2020 2020  try.id,.        
-0000edd0: 2020 2020 2020 2020 7479 7065 3d6d 6574          type=met
-0000ede0: 6164 6174 615f 656e 7472 792e 7461 7267  adata_entry.targ
-0000edf0: 6574 2e6f 626a 6563 745f 7479 7065 2e6e  et.object_type.n
-0000ee00: 616d 652e 6c6f 7765 7228 292c 0a20 2020  ame.lower(),.   
-0000ee10: 2020 2020 2020 2020 2020 2020 2074 6172               tar
-0000ee20: 6765 743d 7374 7228 6d65 7461 6461 7461  get=str(metadata
-0000ee30: 5f65 6e74 7279 2e74 6172 6765 7429 2c0a  _entry.target),.
-0000ee40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ee50: 6469 7363 6f76 6572 795f 6461 7465 3d6d  discovery_date=m
-0000ee60: 6574 6164 6174 615f 656e 7472 792e 6469  etadata_entry.di
-0000ee70: 7363 6f76 6572 795f 6461 7465 2c0a 2020  scovery_date,.  
-0000ee80: 2020 2020 2020 2020 2020 2020 2020 6175                au
-0000ee90: 7468 6f72 6974 795f 6964 3d61 7574 686f  thority_id=autho
-0000eea0: 7269 7479 5f69 642c 0a20 2020 2020 2020  rity_id,.       
-0000eeb0: 2020 2020 2020 2020 2066 6574 6368 6572           fetcher
-0000eec0: 5f69 643d 6665 7463 6865 725f 6964 2c0a  _id=fetcher_id,.
-0000eed0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000eee0: 666f 726d 6174 3d6d 6574 6164 6174 615f  format=metadata_
-0000eef0: 656e 7472 792e 666f 726d 6174 2c0a 2020  entry.format,.  
-0000ef00: 2020 2020 2020 2020 2020 2020 2020 6d65                me
-0000ef10: 7461 6461 7461 3d6d 6574 6164 6174 615f  tadata=metadata_
-0000ef20: 656e 7472 792e 6d65 7461 6461 7461 2c0a  entry.metadata,.
-0000ef30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ef40: 6f72 6967 696e 3d6d 6574 6164 6174 615f  origin=metadata_
-0000ef50: 656e 7472 792e 6f72 6967 696e 2c0a 2020  entry.origin,.  
-0000ef60: 2020 2020 2020 2020 2020 2020 2020 7669                vi
-0000ef70: 7369 743d 6d65 7461 6461 7461 5f65 6e74  sit=metadata_ent
-0000ef80: 7279 2e76 6973 6974 2c0a 2020 2020 2020  ry.visit,.      
-0000ef90: 2020 2020 2020 2020 2020 736e 6170 7368            snapsh
-0000efa0: 6f74 3d6d 6170 5f6f 7074 696f 6e61 6c28  ot=map_optional(
-0000efb0: 7374 722c 206d 6574 6164 6174 615f 656e  str, metadata_en
-0000efc0: 7472 792e 736e 6170 7368 6f74 292c 0a20  try.snapshot),. 
-0000efd0: 2020 2020 2020 2020 2020 2020 2020 2072                 r
-0000efe0: 656c 6561 7365 3d6d 6170 5f6f 7074 696f  elease=map_optio
-0000eff0: 6e61 6c28 7374 722c 206d 6574 6164 6174  nal(str, metadat
-0000f000: 615f 656e 7472 792e 7265 6c65 6173 6529  a_entry.release)
-0000f010: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-0000f020: 2020 7265 7669 7369 6f6e 3d6d 6170 5f6f    revision=map_o
-0000f030: 7074 696f 6e61 6c28 7374 722c 206d 6574  ptional(str, met
-0000f040: 6164 6174 615f 656e 7472 792e 7265 7669  adata_entry.revi
-0000f050: 7369 6f6e 292c 0a20 2020 2020 2020 2020  sion),.         
-0000f060: 2020 2020 2020 2070 6174 683d 6d65 7461         path=meta
-0000f070: 6461 7461 5f65 6e74 7279 2e70 6174 682c  data_entry.path,
-0000f080: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000f090: 2064 6972 6563 746f 7279 3d6d 6170 5f6f   directory=map_o
-0000f0a0: 7074 696f 6e61 6c28 7374 722c 206d 6574  ptional(str, met
-0000f0b0: 6164 6174 615f 656e 7472 792e 6469 7265  adata_entry.dire
-0000f0c0: 6374 6f72 7929 2c0a 2020 2020 2020 2020  ctory),.        
-0000f0d0: 2020 2020 2020 2020 6375 723d 6375 722c          cur=cur,
-0000f0e0: 0a20 2020 2020 2020 2020 2020 2029 0a20  .            ). 
-0000f0f0: 2020 2020 2020 2020 2020 2063 6f75 6e74             count
-0000f100: 6572 5b6d 6574 6164 6174 615f 656e 7472  er[metadata_entr
-0000f110: 792e 7461 7267 6574 2e6f 626a 6563 745f  y.target.object_
-0000f120: 7479 7065 5d20 2b3d 2031 0a0a 2020 2020  type] += 1..    
-0000f130: 2020 2020 7265 7475 726e 207b 0a20 2020      return {.   
-0000f140: 2020 2020 2020 2020 2066 227b 7479 7065           f"{type
-0000f150: 2e76 616c 7565 7d5f 6d65 7461 6461 7461  .value}_metadata
-0000f160: 3a61 6464 223a 2063 6f75 6e74 2066 6f72  :add": count for
-0000f170: 2028 7479 7065 2c20 636f 756e 7429 2069   (type, count) i
-0000f180: 6e20 636f 756e 7465 722e 6974 656d 7328  n counter.items(
-0000f190: 290a 2020 2020 2020 2020 7d0a 0a20 2020  ).        }..   
-0000f1a0: 2040 6462 5f74 7261 6e73 6163 7469 6f6e   @db_transaction
-0000f1b0: 2829 0a20 2020 2064 6566 2072 6177 5f65  ().    def raw_e
-0000f1c0: 7874 7269 6e73 6963 5f6d 6574 6164 6174  xtrinsic_metadat
-0000f1d0: 615f 6765 7428 0a20 2020 2020 2020 2073  a_get(.        s
-0000f1e0: 656c 662c 0a20 2020 2020 2020 2074 6172  elf,.        tar
-0000f1f0: 6765 743a 2045 7874 656e 6465 6453 5748  get: ExtendedSWH
-0000f200: 4944 2c0a 2020 2020 2020 2020 6175 7468  ID,.        auth
-0000f210: 6f72 6974 793a 204d 6574 6164 6174 6141  ority: MetadataA
-0000f220: 7574 686f 7269 7479 2c0a 2020 2020 2020  uthority,.      
-0000f230: 2020 6166 7465 723a 204f 7074 696f 6e61    after: Optiona
-0000f240: 6c5b 6461 7465 7469 6d65 2e64 6174 6574  l[datetime.datet
-0000f250: 696d 655d 203d 204e 6f6e 652c 0a20 2020  ime] = None,.   
-0000f260: 2020 2020 2070 6167 655f 746f 6b65 6e3a       page_token:
-0000f270: 204f 7074 696f 6e61 6c5b 6279 7465 735d   Optional[bytes]
-0000f280: 203d 204e 6f6e 652c 0a20 2020 2020 2020   = None,.       
-0000f290: 206c 696d 6974 3a20 696e 7420 3d20 3130   limit: int = 10
-0000f2a0: 3030 2c0a 2020 2020 2020 2020 2a2c 0a20  00,.        *,. 
-0000f2b0: 2020 2020 2020 2064 623a 2044 622c 0a20         db: Db,. 
-0000f2c0: 2020 2020 2020 2063 7572 3d4e 6f6e 652c         cur=None,
-0000f2d0: 0a20 2020 2029 202d 3e20 5061 6765 6452  .    ) -> PagedR
-0000f2e0: 6573 756c 745b 5261 7745 7874 7269 6e73  esult[RawExtrins
-0000f2f0: 6963 4d65 7461 6461 7461 5d3a 0a20 2020  icMetadata]:.   
-0000f300: 2020 2020 2069 6620 7061 6765 5f74 6f6b       if page_tok
-0000f310: 656e 3a0a 2020 2020 2020 2020 2020 2020  en:.            
-0000f320: 2861 6674 6572 5f74 696d 652c 2061 6674  (after_time, aft
-0000f330: 6572 5f66 6574 6368 6572 2920 3d20 6d73  er_fetcher) = ms
-0000f340: 6770 6163 6b5f 6c6f 6164 7328 6261 7365  gpack_loads(base
-0000f350: 3634 2e62 3634 6465 636f 6465 2870 6167  64.b64decode(pag
-0000f360: 655f 746f 6b65 6e29 290a 2020 2020 2020  e_token)).      
-0000f370: 2020 2020 2020 6966 2061 6674 6572 2061        if after a
-0000f380: 6e64 2061 6674 6572 5f74 696d 6520 3c20  nd after_time < 
-0000f390: 6166 7465 723a 0a20 2020 2020 2020 2020  after:.         
-0000f3a0: 2020 2020 2020 2072 6169 7365 2053 746f         raise Sto
-0000f3b0: 7261 6765 4172 6775 6d65 6e74 4578 6365  rageArgumentExce
-0000f3c0: 7074 696f 6e28 0a20 2020 2020 2020 2020  ption(.         
-0000f3d0: 2020 2020 2020 2020 2020 2022 7061 6765             "page
-0000f3e0: 5f74 6f6b 656e 2069 7320 696e 636f 6e73  _token is incons
-0000f3f0: 6973 7465 6e74 2077 6974 6820 7468 6520  istent with the 
-0000f400: 7661 6c75 6520 6f66 2027 6166 7465 7227  value of 'after'
-0000f410: 2e22 0a20 2020 2020 2020 2020 2020 2020  .".             
-0000f420: 2020 2029 0a20 2020 2020 2020 2065 6c73     ).        els
-0000f430: 653a 0a20 2020 2020 2020 2020 2020 2061  e:.            a
-0000f440: 6674 6572 5f74 696d 6520 3d20 6166 7465  fter_time = afte
-0000f450: 720a 2020 2020 2020 2020 2020 2020 6166  r.            af
-0000f460: 7465 725f 6665 7463 6865 7220 3d20 4e6f  ter_fetcher = No
-0000f470: 6e65 0a0a 2020 2020 2020 2020 7472 793a  ne..        try:
-0000f480: 0a20 2020 2020 2020 2020 2020 2061 7574  .            aut
-0000f490: 686f 7269 7479 5f69 6420 3d20 7365 6c66  hority_id = self
-0000f4a0: 2e5f 6765 745f 6175 7468 6f72 6974 795f  ._get_authority_
-0000f4b0: 6964 2861 7574 686f 7269 7479 2c20 6462  id(authority, db
-0000f4c0: 2c20 6375 7229 0a20 2020 2020 2020 2065  , cur).        e
-0000f4d0: 7863 6570 7420 556e 6b6e 6f77 6e4d 6574  xcept UnknownMet
-0000f4e0: 6164 6174 6141 7574 686f 7269 7479 3a0a  adataAuthority:.
-0000f4f0: 2020 2020 2020 2020 2020 2020 7265 7475              retu
-0000f500: 726e 2050 6167 6564 5265 7375 6c74 280a  rn PagedResult(.
-0000f510: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f520: 6e65 7874 5f70 6167 655f 746f 6b65 6e3d  next_page_token=
-0000f530: 4e6f 6e65 2c0a 2020 2020 2020 2020 2020  None,.          
-0000f540: 2020 2020 2020 7265 7375 6c74 733d 5b5d        results=[]
-0000f550: 2c0a 2020 2020 2020 2020 2020 2020 290a  ,.            ).
-0000f560: 0a20 2020 2020 2020 2072 6f77 7320 3d20  .        rows = 
-0000f570: 6462 2e72 6177 5f65 7874 7269 6e73 6963  db.raw_extrinsic
-0000f580: 5f6d 6574 6164 6174 615f 6765 7428 0a20  _metadata_get(. 
-0000f590: 2020 2020 2020 2020 2020 2073 7472 2874             str(t
-0000f5a0: 6172 6765 7429 2c0a 2020 2020 2020 2020  arget),.        
-0000f5b0: 2020 2020 6175 7468 6f72 6974 795f 6964      authority_id
-0000f5c0: 2c0a 2020 2020 2020 2020 2020 2020 6166  ,.            af
-0000f5d0: 7465 725f 7469 6d65 2c0a 2020 2020 2020  ter_time,.      
-0000f5e0: 2020 2020 2020 6166 7465 725f 6665 7463        after_fetc
-0000f5f0: 6865 722c 0a20 2020 2020 2020 2020 2020  her,.           
-0000f600: 206c 696d 6974 202b 2031 2c0a 2020 2020   limit + 1,.    
-0000f610: 2020 2020 2020 2020 6375 722c 0a20 2020          cur,.   
-0000f620: 2020 2020 2029 0a20 2020 2020 2020 2072       ).        r
-0000f630: 6f77 7320 3d20 5b64 6963 7428 7a69 7028  ows = [dict(zip(
-0000f640: 6462 2e72 6177 5f65 7874 7269 6e73 6963  db.raw_extrinsic
-0000f650: 5f6d 6574 6164 6174 615f 6765 745f 636f  _metadata_get_co
-0000f660: 6c73 2c20 726f 7729 2920 666f 7220 726f  ls, row)) for ro
-0000f670: 7720 696e 2072 6f77 735d 0a20 2020 2020  w in rows].     
-0000f680: 2020 2072 6573 756c 7473 203d 205b 5d0a     results = [].
-0000f690: 2020 2020 2020 2020 666f 7220 726f 7720          for row 
-0000f6a0: 696e 2072 6f77 733a 0a20 2020 2020 2020  in rows:.       
-0000f6b0: 2020 2020 2061 7373 6572 7420 7374 7228       assert str(
-0000f6c0: 7461 7267 6574 2920 3d3d 2072 6f77 5b22  target) == row["
-0000f6d0: 7261 775f 6578 7472 696e 7369 635f 6d65  raw_extrinsic_me
-0000f6e0: 7461 6461 7461 2e74 6172 6765 7422 5d0a  tadata.target"].
-0000f6f0: 2020 2020 2020 2020 2020 2020 7265 7375              resu
-0000f700: 6c74 732e 6170 7065 6e64 2863 6f6e 7665  lts.append(conve
-0000f710: 7274 6572 732e 6462 5f74 6f5f 7261 775f  rters.db_to_raw_
-0000f720: 6578 7472 696e 7369 635f 6d65 7461 6461  extrinsic_metada
-0000f730: 7461 2872 6f77 2929 0a0a 2020 2020 2020  ta(row))..      
-0000f740: 2020 6966 206c 656e 2872 6573 756c 7473    if len(results
-0000f750: 2920 3e20 6c69 6d69 743a 0a20 2020 2020  ) > limit:.     
-0000f760: 2020 2020 2020 2072 6573 756c 7473 2e70         results.p
-0000f770: 6f70 2829 0a20 2020 2020 2020 2020 2020  op().           
-0000f780: 2061 7373 6572 7420 6c65 6e28 7265 7375   assert len(resu
-0000f790: 6c74 7329 203d 3d20 6c69 6d69 740a 2020  lts) == limit.  
-0000f7a0: 2020 2020 2020 2020 2020 6c61 7374 5f72            last_r
-0000f7b0: 6574 7572 6e65 645f 726f 7720 3d20 726f  eturned_row = ro
-0000f7c0: 7773 5b2d 325d 2020 2320 726f 7773 5b2d  ws[-2]  # rows[-
-0000f7d0: 315d 2063 6f72 7265 7370 6f6e 6473 2074  1] corresponds t
-0000f7e0: 6f20 7468 6520 706f 7070 6564 2072 6573  o the popped res
-0000f7f0: 756c 740a 2020 2020 2020 2020 2020 2020  ult.            
-0000f800: 6e65 7874 5f70 6167 655f 746f 6b65 6e3a  next_page_token:
-0000f810: 204f 7074 696f 6e61 6c5b 7374 725d 203d   Optional[str] =
-0000f820: 2062 6173 6536 342e 6236 3465 6e63 6f64   base64.b64encod
-0000f830: 6528 0a20 2020 2020 2020 2020 2020 2020  e(.             
-0000f840: 2020 206d 7367 7061 636b 5f64 756d 7073     msgpack_dumps
-0000f850: 280a 2020 2020 2020 2020 2020 2020 2020  (.              
-0000f860: 2020 2020 2020 280a 2020 2020 2020 2020        (.        
-0000f870: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f880: 6c61 7374 5f72 6574 7572 6e65 645f 726f  last_returned_ro
-0000f890: 775b 2264 6973 636f 7665 7279 5f64 6174  w["discovery_dat
-0000f8a0: 6522 5d2c 0a20 2020 2020 2020 2020 2020  e"],.           
-0000f8b0: 2020 2020 2020 2020 2020 2020 206c 6173               las
-0000f8c0: 745f 7265 7475 726e 6564 5f72 6f77 5b22  t_returned_row["
-0000f8d0: 6d65 7461 6461 7461 5f66 6574 6368 6572  metadata_fetcher
-0000f8e0: 2e69 6422 5d2c 0a20 2020 2020 2020 2020  .id"],.         
-0000f8f0: 2020 2020 2020 2020 2020 2029 0a20 2020             ).   
-0000f900: 2020 2020 2020 2020 2020 2020 2029 0a20               ). 
-0000f910: 2020 2020 2020 2020 2020 2029 2e64 6563             ).dec
-0000f920: 6f64 6528 290a 2020 2020 2020 2020 656c  ode().        el
-0000f930: 7365 3a0a 2020 2020 2020 2020 2020 2020  se:.            
-0000f940: 6e65 7874 5f70 6167 655f 746f 6b65 6e20  next_page_token 
-0000f950: 3d20 4e6f 6e65 0a0a 2020 2020 2020 2020  = None..        
-0000f960: 7265 7475 726e 2050 6167 6564 5265 7375  return PagedResu
-0000f970: 6c74 280a 2020 2020 2020 2020 2020 2020  lt(.            
-0000f980: 6e65 7874 5f70 6167 655f 746f 6b65 6e3d  next_page_token=
-0000f990: 6e65 7874 5f70 6167 655f 746f 6b65 6e2c  next_page_token,
-0000f9a0: 0a20 2020 2020 2020 2020 2020 2072 6573  .            res
-0000f9b0: 756c 7473 3d72 6573 756c 7473 2c0a 2020  ults=results,.  
-0000f9c0: 2020 2020 2020 290a 0a20 2020 2040 6462        )..    @db
-0000f9d0: 5f74 7261 6e73 6163 7469 6f6e 2829 0a20  _transaction(). 
-0000f9e0: 2020 2064 6566 2072 6177 5f65 7874 7269     def raw_extri
-0000f9f0: 6e73 6963 5f6d 6574 6164 6174 615f 6765  nsic_metadata_ge
-0000fa00: 745f 6279 5f69 6473 280a 2020 2020 2020  t_by_ids(.      
-0000fa10: 2020 7365 6c66 2c0a 2020 2020 2020 2020    self,.        
-0000fa20: 6964 733a 204c 6973 745b 5368 6131 4769  ids: List[Sha1Gi
-0000fa30: 745d 2c0a 2020 2020 2020 2020 2a2c 0a20  t],.        *,. 
-0000fa40: 2020 2020 2020 2064 623a 2044 622c 0a20         db: Db,. 
-0000fa50: 2020 2020 2020 2063 7572 3d4e 6f6e 652c         cur=None,
-0000fa60: 0a20 2020 2029 202d 3e20 4c69 7374 5b52  .    ) -> List[R
-0000fa70: 6177 4578 7472 696e 7369 634d 6574 6164  awExtrinsicMetad
-0000fa80: 6174 615d 3a0a 2020 2020 2020 2020 7265  ata]:.        re
-0000fa90: 7475 726e 205b 0a20 2020 2020 2020 2020  turn [.         
-0000faa0: 2020 2063 6f6e 7665 7274 6572 732e 6462     converters.db
-0000fab0: 5f74 6f5f 7261 775f 6578 7472 696e 7369  _to_raw_extrinsi
-0000fac0: 635f 6d65 7461 6461 7461 280a 2020 2020  c_metadata(.    
-0000fad0: 2020 2020 2020 2020 2020 2020 6469 6374              dict
-0000fae0: 287a 6970 2864 622e 7261 775f 6578 7472  (zip(db.raw_extr
-0000faf0: 696e 7369 635f 6d65 7461 6461 7461 5f67  insic_metadata_g
-0000fb00: 6574 5f63 6f6c 732c 2072 6f77 2929 0a20  et_cols, row)). 
-0000fb10: 2020 2020 2020 2020 2020 2029 0a20 2020             ).   
-0000fb20: 2020 2020 2020 2020 2066 6f72 2072 6f77           for row
-0000fb30: 2069 6e20 6462 2e72 6177 5f65 7874 7269   in db.raw_extri
-0000fb40: 6e73 6963 5f6d 6574 6164 6174 615f 6765  nsic_metadata_ge
-0000fb50: 745f 6279 5f69 6473 2869 6473 290a 2020  t_by_ids(ids).  
-0000fb60: 2020 2020 2020 5d0a 0a20 2020 2023 2323        ]..    ###
-0000fb70: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-0000fb80: 2323 2323 2323 230a 2020 2020 2320 4d65  #######.    # Me
-0000fb90: 7461 6461 7461 4665 7463 6865 7220 616e  tadataFetcher an
-0000fba0: 6420 4d65 7461 6461 7461 4175 7468 6f72  d MetadataAuthor
-0000fbb0: 6974 790a 2020 2020 2323 2323 2323 2323  ity.    ########
-0000fbc0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-0000fbd0: 2323 0a0a 2020 2020 4064 625f 7472 616e  ##..    @db_tran
-0000fbe0: 7361 6374 696f 6e28 290a 2020 2020 6465  saction().    de
-0000fbf0: 6620 6d65 7461 6461 7461 5f66 6574 6368  f metadata_fetch
-0000fc00: 6572 5f61 6464 280a 2020 2020 2020 2020  er_add(.        
-0000fc10: 7365 6c66 2c20 6665 7463 6865 7273 3a20  self, fetchers: 
-0000fc20: 4c69 7374 5b4d 6574 6164 6174 6146 6574  List[MetadataFet
-0000fc30: 6368 6572 5d2c 202a 2c20 6462 3a20 4462  cher], *, db: Db
-0000fc40: 2c20 6375 723d 4e6f 6e65 0a20 2020 2029  , cur=None.    )
-0000fc50: 202d 3e20 4469 6374 5b73 7472 2c20 696e   -> Dict[str, in
-0000fc60: 745d 3a0a 2020 2020 2020 2020 6665 7463  t]:.        fetc
-0000fc70: 6865 7273 203d 206c 6973 7428 6665 7463  hers = list(fetc
-0000fc80: 6865 7273 290a 2020 2020 2020 2020 7365  hers).        se
-0000fc90: 6c66 2e6a 6f75 726e 616c 5f77 7269 7465  lf.journal_write
-0000fca0: 722e 6d65 7461 6461 7461 5f66 6574 6368  r.metadata_fetch
-0000fcb0: 6572 5f61 6464 2866 6574 6368 6572 7329  er_add(fetchers)
-0000fcc0: 0a20 2020 2020 2020 2063 6f75 6e74 203d  .        count =
-0000fcd0: 2030 0a20 2020 2020 2020 2066 6f72 2066   0.        for f
-0000fce0: 6574 6368 6572 2069 6e20 6665 7463 6865  etcher in fetche
-0000fcf0: 7273 3a0a 2020 2020 2020 2020 2020 2020  rs:.            
-0000fd00: 6462 2e6d 6574 6164 6174 615f 6665 7463  db.metadata_fetc
-0000fd10: 6865 725f 6164 6428 6665 7463 6865 722e  her_add(fetcher.
-0000fd20: 6e61 6d65 2c20 6665 7463 6865 722e 7665  name, fetcher.ve
-0000fd30: 7273 696f 6e2c 2063 7572 3d63 7572 290a  rsion, cur=cur).
-0000fd40: 2020 2020 2020 2020 2020 2020 636f 756e              coun
-0000fd50: 7420 2b3d 2031 0a20 2020 2020 2020 2072  t += 1.        r
-0000fd60: 6574 7572 6e20 7b22 6d65 7461 6461 7461  eturn {"metadata
-0000fd70: 5f66 6574 6368 6572 3a61 6464 223a 2063  _fetcher:add": c
-0000fd80: 6f75 6e74 7d0a 0a20 2020 2040 6462 5f74  ount}..    @db_t
-0000fd90: 7261 6e73 6163 7469 6f6e 2873 7461 7465  ransaction(state
-0000fda0: 6d65 6e74 5f74 696d 656f 7574 3d35 3030  ment_timeout=500
-0000fdb0: 290a 2020 2020 6465 6620 6d65 7461 6461  ).    def metada
-0000fdc0: 7461 5f66 6574 6368 6572 5f67 6574 280a  ta_fetcher_get(.
-0000fdd0: 2020 2020 2020 2020 7365 6c66 2c20 6e61          self, na
-0000fde0: 6d65 3a20 7374 722c 2076 6572 7369 6f6e  me: str, version
-0000fdf0: 3a20 7374 722c 202a 2c20 6462 3a20 4462  : str, *, db: Db
-0000fe00: 2c20 6375 723d 4e6f 6e65 0a20 2020 2029  , cur=None.    )
-0000fe10: 202d 3e20 4f70 7469 6f6e 616c 5b4d 6574   -> Optional[Met
-0000fe20: 6164 6174 6146 6574 6368 6572 5d3a 0a20  adataFetcher]:. 
-0000fe30: 2020 2020 2020 2072 6f77 203d 2064 622e         row = db.
-0000fe40: 6d65 7461 6461 7461 5f66 6574 6368 6572  metadata_fetcher
-0000fe50: 5f67 6574 286e 616d 652c 2076 6572 7369  _get(name, versi
-0000fe60: 6f6e 2c20 6375 723d 6375 7229 0a20 2020  on, cur=cur).   
-0000fe70: 2020 2020 2069 6620 6e6f 7420 726f 773a       if not row:
-0000fe80: 0a20 2020 2020 2020 2020 2020 2072 6574  .            ret
-0000fe90: 7572 6e20 4e6f 6e65 0a20 2020 2020 2020  urn None.       
-0000fea0: 2072 6574 7572 6e20 4d65 7461 6461 7461   return Metadata
-0000feb0: 4665 7463 6865 722e 6672 6f6d 5f64 6963  Fetcher.from_dic
-0000fec0: 7428 6469 6374 287a 6970 2864 622e 6d65  t(dict(zip(db.me
-0000fed0: 7461 6461 7461 5f66 6574 6368 6572 5f63  tadata_fetcher_c
-0000fee0: 6f6c 732c 2072 6f77 2929 290a 0a20 2020  ols, row)))..   
-0000fef0: 2040 6462 5f74 7261 6e73 6163 7469 6f6e   @db_transaction
-0000ff00: 2829 0a20 2020 2064 6566 2072 6177 5f65  ().    def raw_e
-0000ff10: 7874 7269 6e73 6963 5f6d 6574 6164 6174  xtrinsic_metadat
-0000ff20: 615f 6765 745f 6175 7468 6f72 6974 6965  a_get_authoritie
-0000ff30: 7328 0a20 2020 2020 2020 2073 656c 662c  s(.        self,
-0000ff40: 0a20 2020 2020 2020 2074 6172 6765 743a  .        target:
-0000ff50: 2045 7874 656e 6465 6453 5748 4944 2c0a   ExtendedSWHID,.
-0000ff60: 2020 2020 2020 2020 2a2c 0a20 2020 2020          *,.     
-0000ff70: 2020 2064 623a 2044 622c 0a20 2020 2020     db: Db,.     
-0000ff80: 2020 2063 7572 3d4e 6f6e 652c 0a20 2020     cur=None,.   
-0000ff90: 2029 202d 3e20 4c69 7374 5b4d 6574 6164   ) -> List[Metad
-0000ffa0: 6174 6141 7574 686f 7269 7479 5d3a 0a20  ataAuthority]:. 
-0000ffb0: 2020 2020 2020 2072 6574 7572 6e20 5b0a         return [.
-0000ffc0: 2020 2020 2020 2020 2020 2020 4d65 7461              Meta
-0000ffd0: 6461 7461 4175 7468 6f72 6974 7928 0a20  dataAuthority(. 
-0000ffe0: 2020 2020 2020 2020 2020 2020 2020 2074                 t
-0000fff0: 7970 653d 4d65 7461 6461 7461 4175 7468  ype=MetadataAuth
-00010000: 6f72 6974 7954 7970 6528 6175 7468 6f72  orityType(author
-00010010: 6974 795f 7479 7065 292c 2075 726c 3d61  ity_type), url=a
-00010020: 7574 686f 7269 7479 5f75 726c 0a20 2020  uthority_url.   
-00010030: 2020 2020 2020 2020 2029 0a20 2020 2020           ).     
-00010040: 2020 2020 2020 2066 6f72 2028 0a20 2020         for (.   
-00010050: 2020 2020 2020 2020 2020 2020 2061 7574               aut
-00010060: 686f 7269 7479 5f74 7970 652c 0a20 2020  hority_type,.   
-00010070: 2020 2020 2020 2020 2020 2020 2061 7574               aut
-00010080: 686f 7269 7479 5f75 726c 2c0a 2020 2020  hority_url,.    
-00010090: 2020 2020 2020 2020 2920 696e 2064 622e          ) in db.
-000100a0: 7261 775f 6578 7472 696e 7369 635f 6d65  raw_extrinsic_me
-000100b0: 7461 6461 7461 5f67 6574 5f61 7574 686f  tadata_get_autho
-000100c0: 7269 7469 6573 2873 7472 2874 6172 6765  rities(str(targe
-000100d0: 7429 2c20 6375 7229 0a20 2020 2020 2020  t), cur).       
-000100e0: 205d 0a0a 2020 2020 4064 625f 7472 616e   ]..    @db_tran
-000100f0: 7361 6374 696f 6e28 290a 2020 2020 6465  saction().    de
-00010100: 6620 6d65 7461 6461 7461 5f61 7574 686f  f metadata_autho
-00010110: 7269 7479 5f61 6464 280a 2020 2020 2020  rity_add(.      
-00010120: 2020 7365 6c66 2c20 6175 7468 6f72 6974    self, authorit
-00010130: 6965 733a 204c 6973 745b 4d65 7461 6461  ies: List[Metada
-00010140: 7461 4175 7468 6f72 6974 795d 2c20 2a2c  taAuthority], *,
-00010150: 2064 623a 2044 622c 2063 7572 3d4e 6f6e   db: Db, cur=Non
-00010160: 650a 2020 2020 2920 2d3e 2044 6963 745b  e.    ) -> Dict[
-00010170: 7374 722c 2069 6e74 5d3a 0a20 2020 2020  str, int]:.     
-00010180: 2020 2061 7574 686f 7269 7469 6573 203d     authorities =
-00010190: 206c 6973 7428 6175 7468 6f72 6974 6965   list(authoritie
-000101a0: 7329 0a20 2020 2020 2020 2073 656c 662e  s).        self.
-000101b0: 6a6f 7572 6e61 6c5f 7772 6974 6572 2e6d  journal_writer.m
-000101c0: 6574 6164 6174 615f 6175 7468 6f72 6974  etadata_authorit
-000101d0: 795f 6164 6428 6175 7468 6f72 6974 6965  y_add(authoritie
-000101e0: 7329 0a20 2020 2020 2020 2063 6f75 6e74  s).        count
-000101f0: 203d 2030 0a20 2020 2020 2020 2066 6f72   = 0.        for
-00010200: 2061 7574 686f 7269 7479 2069 6e20 6175   authority in au
-00010210: 7468 6f72 6974 6965 733a 0a20 2020 2020  thorities:.     
-00010220: 2020 2020 2020 2064 622e 6d65 7461 6461         db.metada
-00010230: 7461 5f61 7574 686f 7269 7479 5f61 6464  ta_authority_add
-00010240: 2861 7574 686f 7269 7479 2e74 7970 652e  (authority.type.
-00010250: 7661 6c75 652c 2061 7574 686f 7269 7479  value, authority
-00010260: 2e75 726c 2c20 6375 723d 6375 7229 0a20  .url, cur=cur). 
-00010270: 2020 2020 2020 2020 2020 2063 6f75 6e74             count
-00010280: 202b 3d20 310a 2020 2020 2020 2020 7265   += 1.        re
-00010290: 7475 726e 207b 226d 6574 6164 6174 615f  turn {"metadata_
-000102a0: 6175 7468 6f72 6974 793a 6164 6422 3a20  authority:add": 
-000102b0: 636f 756e 747d 0a0a 2020 2020 4064 625f  count}..    @db_
-000102c0: 7472 616e 7361 6374 696f 6e28 290a 2020  transaction().  
-000102d0: 2020 6465 6620 6d65 7461 6461 7461 5f61    def metadata_a
-000102e0: 7574 686f 7269 7479 5f67 6574 280a 2020  uthority_get(.  
-000102f0: 2020 2020 2020 7365 6c66 2c20 7479 7065        self, type
-00010300: 3a20 4d65 7461 6461 7461 4175 7468 6f72  : MetadataAuthor
-00010310: 6974 7954 7970 652c 2075 726c 3a20 7374  ityType, url: st
-00010320: 722c 202a 2c20 6462 3a20 4462 2c20 6375  r, *, db: Db, cu
-00010330: 723d 4e6f 6e65 0a20 2020 2029 202d 3e20  r=None.    ) -> 
-00010340: 4f70 7469 6f6e 616c 5b4d 6574 6164 6174  Optional[Metadat
-00010350: 6141 7574 686f 7269 7479 5d3a 0a20 2020  aAuthority]:.   
-00010360: 2020 2020 2072 6f77 203d 2064 622e 6d65       row = db.me
-00010370: 7461 6461 7461 5f61 7574 686f 7269 7479  tadata_authority
-00010380: 5f67 6574 2874 7970 652e 7661 6c75 652c  _get(type.value,
-00010390: 2075 726c 2c20 6375 723d 6375 7229 0a20   url, cur=cur). 
-000103a0: 2020 2020 2020 2069 6620 6e6f 7420 726f         if not ro
-000103b0: 773a 0a20 2020 2020 2020 2020 2020 2072  w:.            r
-000103c0: 6574 7572 6e20 4e6f 6e65 0a20 2020 2020  eturn None.     
-000103d0: 2020 2072 6574 7572 6e20 4d65 7461 6461     return Metada
-000103e0: 7461 4175 7468 6f72 6974 792e 6672 6f6d  taAuthority.from
-000103f0: 5f64 6963 7428 6469 6374 287a 6970 2864  _dict(dict(zip(d
-00010400: 622e 6d65 7461 6461 7461 5f61 7574 686f  b.metadata_autho
-00010410: 7269 7479 5f63 6f6c 732c 2072 6f77 2929  rity_cols, row))
-00010420: 290a 0a20 2020 2023 2323 2323 2323 2323  )..    #########
-00010430: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00010440: 0a20 2020 2023 2027 6f62 6a65 6374 5f72  .    # 'object_r
-00010450: 6566 6572 656e 6365 7327 2074 6162 6c65  eferences' table
-00010460: 0a20 2020 2023 2323 2323 2323 2323 2323  .    ###########
-00010470: 2323 2323 2323 2323 2323 2323 2323 0a0a  ##############..
-00010480: 2020 2020 4064 625f 7472 616e 7361 6374      @db_transact
-00010490: 696f 6e28 290a 2020 2020 6465 6620 6f62  ion().    def ob
-000104a0: 6a65 6374 5f66 696e 645f 7265 6365 6e74  ject_find_recent
-000104b0: 5f72 6566 6572 656e 6365 7328 0a20 2020  _references(.   
-000104c0: 2020 2020 2073 656c 662c 2074 6172 6765       self, targe
-000104d0: 745f 7377 6869 643a 2045 7874 656e 6465  t_swhid: Extende
-000104e0: 6453 5748 4944 2c20 6c69 6d69 743a 2069  dSWHID, limit: i
-000104f0: 6e74 2c20 2a2c 2064 623a 2044 622c 2063  nt, *, db: Db, c
-00010500: 7572 3d4e 6f6e 650a 2020 2020 2920 2d3e  ur=None.    ) ->
-00010510: 204c 6973 745b 4578 7465 6e64 6564 5357   List[ExtendedSW
-00010520: 4849 445d 3a0a 2020 2020 2020 2020 7265  HID]:.        re
-00010530: 7475 726e 205b 0a20 2020 2020 2020 2020  turn [.         
-00010540: 2020 2063 6f6e 7665 7274 6572 732e 6462     converters.db
-00010550: 5f74 6f5f 6f62 6a65 6374 5f72 6566 6572  _to_object_refer
-00010560: 656e 6365 5f73 6f75 7263 6528 726f 7729  ence_source(row)
-00010570: 0a20 2020 2020 2020 2020 2020 2066 6f72  .            for
-00010580: 2072 6f77 2069 6e20 6462 2e6f 626a 6563   row in db.objec
-00010590: 745f 7265 6665 7265 6e63 6573 5f67 6574  t_references_get
-000105a0: 280a 2020 2020 2020 2020 2020 2020 2020  (.              
-000105b0: 2020 7461 7267 6574 5f74 7970 653d 7461    target_type=ta
-000105c0: 7267 6574 5f73 7768 6964 2e6f 626a 6563  rget_swhid.objec
-000105d0: 745f 7479 7065 2e6e 616d 652e 6c6f 7765  t_type.name.lowe
-000105e0: 7228 292c 0a20 2020 2020 2020 2020 2020  r(),.           
-000105f0: 2020 2020 2074 6172 6765 743d 7461 7267       target=targ
-00010600: 6574 5f73 7768 6964 2e6f 626a 6563 745f  et_swhid.object_
-00010610: 6964 2c0a 2020 2020 2020 2020 2020 2020  id,.            
-00010620: 2020 2020 6c69 6d69 743d 6c69 6d69 742c      limit=limit,
-00010630: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00010640: 2063 7572 3d63 7572 2c0a 2020 2020 2020   cur=cur,.      
-00010650: 2020 2020 2020 290a 2020 2020 2020 2020        ).        
-00010660: 5d0a 0a20 2020 2040 6462 5f74 7261 6e73  ]..    @db_trans
-00010670: 6163 7469 6f6e 2829 0a20 2020 2064 6566  action().    def
-00010680: 206f 626a 6563 745f 7265 6665 7265 6e63   object_referenc
-00010690: 6573 5f61 6464 280a 2020 2020 2020 2020  es_add(.        
-000106a0: 7365 6c66 2c20 7265 6665 7265 6e63 6573  self, references
-000106b0: 3a20 4c69 7374 5b4f 626a 6563 7452 6566  : List[ObjectRef
-000106c0: 6572 656e 6365 5d2c 202a 2c20 6462 3a20  erence], *, db: 
-000106d0: 4462 2c20 6375 723d 4e6f 6e65 0a20 2020  Db, cur=None.   
-000106e0: 2029 202d 3e20 4469 6374 5b73 7472 2c20   ) -> Dict[str, 
-000106f0: 696e 745d 3a0a 2020 2020 2020 2020 746f  int]:.        to
-00010700: 5f61 6464 203d 206c 6973 7428 7b63 6f6e  _add = list({con
-00010710: 7665 7274 6572 732e 6f62 6a65 6374 5f72  verters.object_r
-00010720: 6566 6572 656e 6365 5f74 6f5f 6462 2872  eference_to_db(r
-00010730: 6566 2920 666f 7220 7265 6620 696e 2072  ef) for ref in r
-00010740: 6566 6572 656e 6365 737d 290a 2020 2020  eferences}).    
-00010750: 2020 2020 6462 2e6f 626a 6563 745f 7265      db.object_re
-00010760: 6665 7265 6e63 6573 5f61 6464 280a 2020  ferences_add(.  
-00010770: 2020 2020 2020 2020 2020 746f 5f61 6464            to_add
-00010780: 2c0a 2020 2020 2020 2020 2020 2020 6375  ,.            cu
-00010790: 723d 6375 722c 0a20 2020 2020 2020 2029  r=cur,.        )
-000107a0: 0a0a 2020 2020 2020 2020 7265 7475 726e  ..        return
-000107b0: 207b 226f 626a 6563 745f 7265 6665 7265   {"object_refere
-000107c0: 6e63 653a 6164 6422 3a20 6c65 6e28 746f  nce:add": len(to
-000107d0: 5f61 6464 297d 0a0a 2020 2020 6465 6620  _add)}..    def 
-000107e0: 636c 6561 725f 6275 6666 6572 7328 7365  clear_buffers(se
-000107f0: 6c66 2c20 6f62 6a65 6374 5f74 7970 6573  lf, object_types
-00010800: 3a20 5365 7175 656e 6365 5b73 7472 5d20  : Sequence[str] 
-00010810: 3d20 2829 2920 2d3e 204e 6f6e 653a 0a20  = ()) -> None:. 
-00010820: 2020 2020 2020 2022 2222 446f 206e 6f74         """Do not
-00010830: 6869 6e67 2222 220a 2020 2020 2020 2020  hing""".        
-00010840: 7265 7475 726e 204e 6f6e 650a 0a20 2020  return None..   
-00010850: 2064 6566 2066 6c75 7368 2873 656c 662c   def flush(self,
-00010860: 206f 626a 6563 745f 7479 7065 733a 2053   object_types: S
-00010870: 6571 7565 6e63 655b 7374 725d 203d 2028  equence[str] = (
-00010880: 2929 202d 3e20 4469 6374 5b73 7472 2c20  )) -> Dict[str, 
-00010890: 696e 745d 3a0a 2020 2020 2020 2020 7265  int]:.        re
-000108a0: 7475 726e 207b 7d0a 0a20 2020 2064 6566  turn {}..    def
-000108b0: 205f 6765 745f 6175 7468 6f72 6974 795f   _get_authority_
-000108c0: 6964 2873 656c 662c 2061 7574 686f 7269  id(self, authori
-000108d0: 7479 3a20 4d65 7461 6461 7461 4175 7468  ty: MetadataAuth
-000108e0: 6f72 6974 792c 2064 622c 2063 7572 293a  ority, db, cur):
-000108f0: 0a20 2020 2020 2020 2061 7574 686f 7269  .        authori
-00010900: 7479 5f69 6420 3d20 6462 2e6d 6574 6164  ty_id = db.metad
-00010910: 6174 615f 6175 7468 6f72 6974 795f 6765  ata_authority_ge
-00010920: 745f 6964 280a 2020 2020 2020 2020 2020  t_id(.          
-00010930: 2020 6175 7468 6f72 6974 792e 7479 7065    authority.type
-00010940: 2e76 616c 7565 2c20 6175 7468 6f72 6974  .value, authorit
-00010950: 792e 7572 6c2c 2063 7572 0a20 2020 2020  y.url, cur.     
-00010960: 2020 2029 0a20 2020 2020 2020 2069 6620     ).        if 
-00010970: 6e6f 7420 6175 7468 6f72 6974 795f 6964  not authority_id
-00010980: 3a0a 2020 2020 2020 2020 2020 2020 7261  :.            ra
-00010990: 6973 6520 556e 6b6e 6f77 6e4d 6574 6164  ise UnknownMetad
-000109a0: 6174 6141 7574 686f 7269 7479 2873 7472  ataAuthority(str
-000109b0: 2861 7574 686f 7269 7479 2929 0a20 2020  (authority)).   
-000109c0: 2020 2020 2072 6574 7572 6e20 6175 7468       return auth
-000109d0: 6f72 6974 795f 6964 0a0a 2020 2020 6465  ority_id..    de
-000109e0: 6620 5f67 6574 5f66 6574 6368 6572 5f69  f _get_fetcher_i
-000109f0: 6428 7365 6c66 2c20 6665 7463 6865 723a  d(self, fetcher:
-00010a00: 204d 6574 6164 6174 6146 6574 6368 6572   MetadataFetcher
-00010a10: 2c20 6462 2c20 6375 7229 3a0a 2020 2020  , db, cur):.    
-00010a20: 2020 2020 6665 7463 6865 725f 6964 203d      fetcher_id =
-00010a30: 2064 622e 6d65 7461 6461 7461 5f66 6574   db.metadata_fet
-00010a40: 6368 6572 5f67 6574 5f69 6428 6665 7463  cher_get_id(fetc
-00010a50: 6865 722e 6e61 6d65 2c20 6665 7463 6865  her.name, fetche
-00010a60: 722e 7665 7273 696f 6e2c 2063 7572 290a  r.version, cur).
-00010a70: 2020 2020 2020 2020 6966 206e 6f74 2066          if not f
-00010a80: 6574 6368 6572 5f69 643a 0a20 2020 2020  etcher_id:.     
-00010a90: 2020 2020 2020 2072 6169 7365 2055 6e6b         raise Unk
-00010aa0: 6e6f 776e 4d65 7461 6461 7461 4665 7463  nownMetadataFetc
-00010ab0: 6865 7228 7374 7228 6665 7463 6865 7229  her(str(fetcher)
-00010ac0: 290a 2020 2020 2020 2020 7265 7475 726e  ).        return
-00010ad0: 2066 6574 6368 6572 5f69 640a 0a20 2020   fetcher_id..   
-00010ae0: 2023 2323 2323 2323 2323 2323 2323 2323   ###############
-00010af0: 2323 2323 2323 2323 2323 0a20 2020 2023  ##########.    #
-00010b00: 204f 626a 6563 7444 656c 6574 696f 6e49   ObjectDeletionI
-00010b10: 6e74 6572 6661 6365 0a20 2020 2023 2323  nterface.    ###
-00010b20: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00010b30: 2323 2323 2323 0a0a 2020 2020 4064 625f  ######..    @db_
-00010b40: 7472 616e 7361 6374 696f 6e28 290a 2020  transaction().  
-00010b50: 2020 6465 6620 6f62 6a65 6374 5f64 656c    def object_del
-00010b60: 6574 6528 0a20 2020 2020 2020 2073 656c  ete(.        sel
-00010b70: 662c 2073 7768 6964 733a 204c 6973 745b  f, swhids: List[
-00010b80: 4578 7465 6e64 6564 5357 4849 445d 2c20  ExtendedSWHID], 
-00010b90: 2a2c 2064 623a 2044 622c 2063 7572 3d4e  *, db: Db, cur=N
-00010ba0: 6f6e 650a 2020 2020 2920 2d3e 2044 6963  one.    ) -> Dic
-00010bb0: 745b 7374 722c 2069 6e74 5d3a 0a20 2020  t[str, int]:.   
-00010bc0: 2020 2020 2022 2222 4465 6c65 7465 206f       """Delete o
-00010bd0: 626a 6563 7473 2066 726f 6d20 7468 6520  bjects from the 
-00010be0: 7374 6f72 6167 650a 0a20 2020 2020 2020  storage..       
-00010bf0: 2041 6c6c 2073 6b69 7070 6564 2063 6f6e   All skipped con
-00010c00: 7465 6e74 206f 626a 6563 7473 206d 6174  tent objects mat
-00010c10: 6368 696e 6720 7468 6520 6769 7665 6e20  ching the given 
-00010c20: 5357 4849 4420 7769 6c6c 2062 6520 7265  SWHID will be re
-00010c30: 6d6f 7665 642c 0a20 2020 2020 2020 2069  moved,.        i
-00010c40: 6e63 6c75 6469 6e67 2074 686f 7365 2077  ncluding those w
-00010c50: 686f 2068 6176 6520 7468 6520 7361 6d65  ho have the same
-00010c60: 2053 5748 4944 2064 7565 2074 6f20 6861   SWHID due to ha
-00010c70: 7368 2063 6f6c 6c69 7369 6f6e 732e 0a0a  sh collisions...
-00010c80: 2020 2020 2020 2020 4f72 6967 696e 206f          Origin o
-00010c90: 626a 6563 7473 2061 7265 2072 656d 6f76  bjects are remov
-00010ca0: 6564 2061 6c6f 6e67 7369 6465 2074 6865  ed alongside the
-00010cb0: 6972 2061 7373 6f63 6961 7465 6420 6f72  ir associated or
-00010cc0: 6967 696e 2076 6973 6974 2061 6e64 0a20  igin visit and. 
-00010cd0: 2020 2020 2020 206f 7269 6769 6e20 7669         origin vi
-00010ce0: 7369 7420 7374 6174 7573 206f 626a 6563  sit status objec
-00010cf0: 7473 2e0a 0a20 2020 2020 2020 2041 7267  ts...        Arg
-00010d00: 733a 0a20 2020 2020 2020 2020 2020 2073  s:.            s
-00010d10: 7768 6964 733a 206c 6973 7420 6f66 2053  whids: list of S
-00010d20: 5748 4944 206f 6620 7468 6520 6f62 6a65  WHID of the obje
-00010d30: 6374 7320 746f 2072 656d 6f76 650a 0a20  cts to remove.. 
-00010d40: 2020 2020 2020 2052 6574 7572 6e73 3a0a         Returns:.
-00010d50: 2020 2020 2020 2020 2020 2020 5375 6d6d              Summ
-00010d60: 6172 7920 6469 6374 2077 6974 6820 7468  ary dict with th
-00010d70: 6520 666f 6c6c 6f77 696e 6720 6b65 7973  e following keys
-00010d80: 2061 6e64 2061 7373 6f63 6961 7465 6420   and associated 
-00010d90: 7661 6c75 6573 3a0a 0a20 2020 2020 2020  values:..       
-00010da0: 2020 2020 2020 2020 2063 6f6e 7465 6e74           content
-00010db0: 3a64 656c 6574 653a 204e 756d 6265 7220  :delete: Number 
-00010dc0: 6f66 2063 6f6e 7465 6e74 206f 626a 6563  of content objec
-00010dd0: 7473 2072 656d 6f76 6564 0a20 2020 2020  ts removed.     
-00010de0: 2020 2020 2020 2020 2020 2063 6f6e 7465             conte
-00010df0: 6e74 3a64 656c 6574 653a 6279 7465 733a  nt:delete:bytes:
-00010e00: 2053 756d 206f 6620 7468 6520 7265 6d6f   Sum of the remo
-00010e10: 7665 6420 636f 6e74 656e 7473 e280 9920  ved contents... 
-00010e20: 6461 7461 206c 656e 6774 680a 2020 2020  data length.    
-00010e30: 2020 2020 2020 2020 2020 2020 736b 6970              skip
-00010e40: 7065 645f 636f 6e74 656e 743a 6465 6c65  ped_content:dele
-00010e50: 7465 3a20 4e75 6d62 6572 206f 6620 736b  te: Number of sk
-00010e60: 6970 7065 6420 636f 6e74 656e 7420 6f62  ipped content ob
-00010e70: 6a65 6374 7320 7265 6d6f 7665 640a 2020  jects removed.  
-00010e80: 2020 2020 2020 2020 2020 2020 2020 6469                di
-00010e90: 7265 6374 6f72 793a 6465 6c65 7465 3a20  rectory:delete: 
-00010ea0: 4e75 6d62 6572 206f 6620 6469 7265 6374  Number of direct
-00010eb0: 6f72 7920 6f62 6a65 6374 7320 7265 6d6f  ory objects remo
-00010ec0: 7665 640a 2020 2020 2020 2020 2020 2020  ved.            
-00010ed0: 2020 2020 7265 7669 7369 6f6e 3a64 656c      revision:del
-00010ee0: 6574 653a 204e 756d 6265 7220 6f66 2072  ete: Number of r
-00010ef0: 6576 6973 696f 6e20 6f62 6a65 6374 7320  evision objects 
-00010f00: 7265 6d6f 7665 640a 2020 2020 2020 2020  removed.        
-00010f10: 2020 2020 2020 2020 7265 6c65 6173 653a          release:
-00010f20: 6465 6c65 7465 3a20 4e75 6d62 6572 206f  delete: Number o
-00010f30: 6620 7265 6c65 6173 6520 6f62 6a65 6374  f release object
-00010f40: 7320 7265 6d6f 7665 640a 2020 2020 2020  s removed.      
-00010f50: 2020 2020 2020 2020 2020 736e 6170 7368            snapsh
-00010f60: 6f74 3a64 656c 6574 653a 204e 756d 6265  ot:delete: Numbe
-00010f70: 7220 6f66 2073 6e61 7073 686f 7420 6f62  r of snapshot ob
-00010f80: 6a65 6374 7320 7265 6d6f 7665 640a 2020  jects removed.  
-00010f90: 2020 2020 2020 2020 2020 2020 2020 6f72                or
-00010fa0: 6967 696e 3a64 656c 6574 653a 204e 756d  igin:delete: Num
-00010fb0: 6265 7220 6f66 206f 7269 6769 6e20 6f62  ber of origin ob
-00010fc0: 6a65 6374 7320 7265 6d6f 7665 640a 2020  jects removed.  
-00010fd0: 2020 2020 2020 2020 2020 2020 2020 6f72                or
-00010fe0: 6967 696e 5f76 6973 6974 3a64 656c 6574  igin_visit:delet
-00010ff0: 653a 204e 756d 6265 7220 6f66 206f 7269  e: Number of ori
-00011000: 6769 6e20 7669 7369 7420 6f62 6a65 6374  gin visit object
-00011010: 7320 7265 6d6f 7665 640a 2020 2020 2020  s removed.      
-00011020: 2020 2020 2020 2020 2020 6f72 6967 696e            origin
-00011030: 5f76 6973 6974 5f73 7461 7475 733a 6465  _visit_status:de
-00011040: 6c65 7465 3a20 4e75 6d62 6572 206f 6620  lete: Number of 
-00011050: 6f72 6967 696e 2076 6973 6974 2073 7461  origin visit sta
-00011060: 7475 7320 6f62 6a65 6374 7320 7265 6d6f  tus objects remo
-00011070: 7665 640a 2020 2020 2020 2020 2222 220a  ved.        """.
-00011080: 2020 2020 2020 2020 6f62 6a65 6374 5f72          object_r
-00011090: 6f77 7320 3d20 5b0a 2020 2020 2020 2020  ows = [.        
-000110a0: 2020 2020 2873 7768 6964 2e6f 626a 6563      (swhid.objec
-000110b0: 745f 7479 7065 2e6e 616d 652e 6c6f 7765  t_type.name.lowe
-000110c0: 7228 292c 2073 7768 6964 2e6f 626a 6563  r(), swhid.objec
-000110d0: 745f 6964 2920 666f 7220 7377 6869 6420  t_id) for swhid 
-000110e0: 696e 2073 7768 6964 730a 2020 2020 2020  in swhids.      
-000110f0: 2020 5d0a 2020 2020 2020 2020 7265 7475    ].        retu
-00011100: 726e 2064 622e 6f62 6a65 6374 5f64 656c  rn db.object_del
-00011110: 6574 6528 6f62 6a65 6374 5f72 6f77 7329  ete(object_rows)
-00011120: 0a                                       .
+00008b00: 2020 2020 2020 2066 6f72 206e 616d 652c         for name,
+00008b10: 2069 6e66 6f20 696e 2073 6e61 7073 686f   info in snapsho
+00008b20: 742e 6272 616e 6368 6573 2e69 7465 6d73  t.branches.items
+00008b30: 2829 0a20 2020 2020 2020 2020 2020 2020  ().             
+00008b40: 2020 2020 2020 2020 2020 2029 2c0a 2020             ),.  
+00008b50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008b60: 2020 2020 2020 2274 6d70 5f73 6e61 7073        "tmp_snaps
+00008b70: 686f 745f 6272 616e 6368 222c 0a20 2020  hot_branch",.   
+00008b80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008b90: 2020 2020 205b 226e 616d 6522 2c20 2274       ["name", "t
+00008ba0: 6172 6765 7422 2c20 2274 6172 6765 745f  arget", "target_
+00008bb0: 7479 7065 225d 2c0a 2020 2020 2020 2020  type"],.        
+00008bc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008bd0: 6375 722c 0a20 2020 2020 2020 2020 2020  cur,.           
+00008be0: 2020 2020 2020 2020 2029 0a0a 2020 2020           )..    
+00008bf0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+00008c00: 2e6a 6f75 726e 616c 5f77 7269 7465 722e  .journal_writer.
+00008c10: 736e 6170 7368 6f74 5f61 6464 285b 736e  snapshot_add([sn
+00008c20: 6170 7368 6f74 5d29 0a0a 2020 2020 2020  apshot])..      
+00008c30: 2020 2020 2020 2020 2020 6462 2e73 6e61            db.sna
+00008c40: 7073 686f 745f 6164 6428 736e 6170 7368  pshot_add(snapsh
+00008c50: 6f74 2e69 642c 2063 7572 290a 2020 2020  ot.id, cur).    
+00008c60: 2020 2020 2020 2020 2020 2020 636f 756e              coun
+00008c70: 7420 2b3d 2031 0a0a 2020 2020 2020 2020  t += 1..        
+00008c80: 7265 7475 726e 207b 2273 6e61 7073 686f  return {"snapsho
+00008c90: 743a 6164 6422 3a20 636f 756e 747d 0a0a  t:add": count}..
+00008ca0: 2020 2020 4064 625f 7472 616e 7361 6374      @db_transact
+00008cb0: 696f 6e5f 6765 6e65 7261 746f 7228 290a  ion_generator().
+00008cc0: 2020 2020 6465 6620 736e 6170 7368 6f74      def snapshot
+00008cd0: 5f6d 6973 7369 6e67 280a 2020 2020 2020  _missing(.      
+00008ce0: 2020 7365 6c66 2c20 736e 6170 7368 6f74    self, snapshot
+00008cf0: 733a 204c 6973 745b 5368 6131 4769 745d  s: List[Sha1Git]
+00008d00: 2c20 2a2c 2064 623a 2044 622c 2063 7572  , *, db: Db, cur
+00008d10: 3d4e 6f6e 650a 2020 2020 2920 2d3e 2049  =None.    ) -> I
+00008d20: 7465 7261 626c 655b 5368 6131 4769 745d  terable[Sha1Git]
+00008d30: 3a0a 2020 2020 2020 2020 666f 7220 6f62  :.        for ob
+00008d40: 6a20 696e 2064 622e 736e 6170 7368 6f74  j in db.snapshot
+00008d50: 5f6d 6973 7369 6e67 5f66 726f 6d5f 6c69  _missing_from_li
+00008d60: 7374 2873 6e61 7073 686f 7473 2c20 6375  st(snapshots, cu
+00008d70: 7229 3a0a 2020 2020 2020 2020 2020 2020  r):.            
+00008d80: 7969 656c 6420 6f62 6a5b 305d 0a0a 2020  yield obj[0]..  
+00008d90: 2020 4064 625f 7472 616e 7361 6374 696f    @db_transactio
+00008da0: 6e28 7374 6174 656d 656e 745f 7469 6d65  n(statement_time
+00008db0: 6f75 743d 3230 3030 290a 2020 2020 6465  out=2000).    de
+00008dc0: 6620 736e 6170 7368 6f74 5f67 6574 280a  f snapshot_get(.
+00008dd0: 2020 2020 2020 2020 7365 6c66 2c20 736e          self, sn
+00008de0: 6170 7368 6f74 5f69 643a 2053 6861 3147  apshot_id: Sha1G
+00008df0: 6974 2c20 2a2c 2064 623a 2044 622c 2063  it, *, db: Db, c
+00008e00: 7572 3d4e 6f6e 650a 2020 2020 2920 2d3e  ur=None.    ) ->
+00008e10: 204f 7074 696f 6e61 6c5b 4469 6374 5b73   Optional[Dict[s
+00008e20: 7472 2c20 416e 795d 5d3a 0a20 2020 2020  tr, Any]]:.     
+00008e30: 2020 2064 203d 2073 656c 662e 736e 6170     d = self.snap
+00008e40: 7368 6f74 5f67 6574 5f62 7261 6e63 6865  shot_get_branche
+00008e50: 7328 736e 6170 7368 6f74 5f69 6429 0a20  s(snapshot_id). 
+00008e60: 2020 2020 2020 2069 6620 6420 6973 204e         if d is N
+00008e70: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
+00008e80: 2072 6574 7572 6e20 640a 2020 2020 2020   return d.      
+00008e90: 2020 7265 7475 726e 207b 0a20 2020 2020    return {.     
+00008ea0: 2020 2020 2020 2022 6964 223a 2064 5b22         "id": d["
+00008eb0: 6964 225d 2c0a 2020 2020 2020 2020 2020  id"],.          
+00008ec0: 2020 2262 7261 6e63 6865 7322 3a20 7b0a    "branches": {.
+00008ed0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008ee0: 6e61 6d65 3a20 6272 616e 6368 2e74 6f5f  name: branch.to_
+00008ef0: 6469 6374 2829 2069 6620 6272 616e 6368  dict() if branch
+00008f00: 2065 6c73 6520 4e6f 6e65 0a20 2020 2020   else None.     
+00008f10: 2020 2020 2020 2020 2020 2066 6f72 2028             for (
+00008f20: 6e61 6d65 2c20 6272 616e 6368 2920 696e  name, branch) in
+00008f30: 2064 5b22 6272 616e 6368 6573 225d 2e69   d["branches"].i
+00008f40: 7465 6d73 2829 0a20 2020 2020 2020 2020  tems().         
+00008f50: 2020 207d 2c0a 2020 2020 2020 2020 2020     },.          
+00008f60: 2020 226e 6578 745f 6272 616e 6368 223a    "next_branch":
+00008f70: 2064 5b22 6e65 7874 5f62 7261 6e63 6822   d["next_branch"
+00008f80: 5d2c 0a20 2020 2020 2020 207d 0a0a 2020  ],.        }..  
+00008f90: 2020 4064 625f 7472 616e 7361 6374 696f    @db_transactio
+00008fa0: 6e28 290a 2020 2020 6465 6620 736e 6170  n().    def snap
+00008fb0: 7368 6f74 5f67 6574 5f69 645f 7061 7274  shot_get_id_part
+00008fc0: 6974 696f 6e28 0a20 2020 2020 2020 2073  ition(.        s
+00008fd0: 656c 662c 0a20 2020 2020 2020 2070 6172  elf,.        par
+00008fe0: 7469 7469 6f6e 5f69 643a 2069 6e74 2c0a  tition_id: int,.
+00008ff0: 2020 2020 2020 2020 6e62 5f70 6172 7469          nb_parti
+00009000: 7469 6f6e 733a 2069 6e74 2c0a 2020 2020  tions: int,.    
+00009010: 2020 2020 7061 6765 5f74 6f6b 656e 3a20      page_token: 
+00009020: 4f70 7469 6f6e 616c 5b73 7472 5d20 3d20  Optional[str] = 
+00009030: 4e6f 6e65 2c0a 2020 2020 2020 2020 6c69  None,.        li
+00009040: 6d69 743a 2069 6e74 203d 2031 3030 302c  mit: int = 1000,
+00009050: 0a20 2020 2020 2020 202a 2c0a 2020 2020  .        *,.    
+00009060: 2020 2020 6462 3a20 4462 2c0a 2020 2020      db: Db,.    
+00009070: 2020 2020 6375 723d 4e6f 6e65 2c0a 2020      cur=None,.  
+00009080: 2020 2920 2d3e 2050 6167 6564 5265 7375    ) -> PagedResu
+00009090: 6c74 5b53 6861 3147 6974 5d3a 0a20 2020  lt[Sha1Git]:.   
+000090a0: 2020 2020 2072 6574 7572 6e20 5f67 6574       return _get
+000090b0: 5f70 6167 696e 6174 6564 5f73 6861 315f  _paginated_sha1_
+000090c0: 7061 7274 6974 696f 6e28 0a20 2020 2020  partition(.     
+000090d0: 2020 2020 2020 2063 7572 2c0a 2020 2020         cur,.    
+000090e0: 2020 2020 2020 2020 7061 7274 6974 696f          partitio
+000090f0: 6e5f 6964 2c0a 2020 2020 2020 2020 2020  n_id,.          
+00009100: 2020 6e62 5f70 6172 7469 7469 6f6e 732c    nb_partitions,
+00009110: 0a20 2020 2020 2020 2020 2020 2070 6167  .            pag
+00009120: 655f 746f 6b65 6e2c 0a20 2020 2020 2020  e_token,.       
+00009130: 2020 2020 206c 696d 6974 2c0a 2020 2020       limit,.    
+00009140: 2020 2020 2020 2020 6462 2e73 6e61 7073          db.snaps
+00009150: 686f 745f 6765 745f 6964 5f72 616e 6765  hot_get_id_range
+00009160: 2c0a 2020 2020 2020 2020 2020 2020 6f70  ,.            op
+00009170: 6572 6174 6f72 2e69 7465 6d67 6574 7465  erator.itemgette
+00009180: 7228 3029 2c0a 2020 2020 2020 2020 2020  r(0),.          
+00009190: 2020 6c61 6d62 6461 2069 645f 3a20 6964    lambda id_: id
+000091a0: 5f2c 0a20 2020 2020 2020 2029 0a0a 2020  _,.        )..  
+000091b0: 2020 4064 625f 7472 616e 7361 6374 696f    @db_transactio
+000091c0: 6e28 7374 6174 656d 656e 745f 7469 6d65  n(statement_time
+000091d0: 6f75 743d 3230 3030 290a 2020 2020 6465  out=2000).    de
+000091e0: 6620 736e 6170 7368 6f74 5f63 6f75 6e74  f snapshot_count
+000091f0: 5f62 7261 6e63 6865 7328 0a20 2020 2020  _branches(.     
+00009200: 2020 2073 656c 662c 0a20 2020 2020 2020     self,.       
+00009210: 2073 6e61 7073 686f 745f 6964 3a20 5368   snapshot_id: Sh
+00009220: 6131 4769 742c 0a20 2020 2020 2020 2062  a1Git,.        b
+00009230: 7261 6e63 685f 6e61 6d65 5f65 7863 6c75  ranch_name_exclu
+00009240: 6465 5f70 7265 6669 783a 204f 7074 696f  de_prefix: Optio
+00009250: 6e61 6c5b 6279 7465 735d 203d 204e 6f6e  nal[bytes] = Non
+00009260: 652c 0a20 2020 2020 2020 202a 2c0a 2020  e,.        *,.  
+00009270: 2020 2020 2020 6462 3a20 4462 2c0a 2020        db: Db,.  
+00009280: 2020 2020 2020 6375 723d 4e6f 6e65 2c0a        cur=None,.
+00009290: 2020 2020 2920 2d3e 204f 7074 696f 6e61      ) -> Optiona
+000092a0: 6c5b 4469 6374 5b4f 7074 696f 6e61 6c5b  l[Dict[Optional[
+000092b0: 7374 725d 2c20 696e 745d 5d3a 0a20 2020  str], int]]:.   
+000092c0: 2020 2020 2072 6574 7572 6e20 6469 6374       return dict
+000092d0: 280a 2020 2020 2020 2020 2020 2020 5b0a  (.            [.
+000092e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000092f0: 6263 0a20 2020 2020 2020 2020 2020 2020  bc.             
+00009300: 2020 2066 6f72 2062 6320 696e 2064 622e     for bc in db.
+00009310: 736e 6170 7368 6f74 5f63 6f75 6e74 5f62  snapshot_count_b
+00009320: 7261 6e63 6865 7328 0a20 2020 2020 2020  ranches(.       
+00009330: 2020 2020 2020 2020 2020 2020 2073 6e61               sna
+00009340: 7073 686f 745f 6964 2c0a 2020 2020 2020  pshot_id,.      
+00009350: 2020 2020 2020 2020 2020 2020 2020 6272                br
+00009360: 616e 6368 5f6e 616d 655f 6578 636c 7564  anch_name_exclud
+00009370: 655f 7072 6566 6978 2c0a 2020 2020 2020  e_prefix,.      
+00009380: 2020 2020 2020 2020 2020 2020 2020 6375                cu
+00009390: 722c 0a20 2020 2020 2020 2020 2020 2020  r,.             
+000093a0: 2020 2029 0a20 2020 2020 2020 2020 2020     ).           
+000093b0: 205d 0a20 2020 2020 2020 2029 0a0a 2020   ].        )..  
+000093c0: 2020 4064 625f 7472 616e 7361 6374 696f    @db_transactio
+000093d0: 6e28 7374 6174 656d 656e 745f 7469 6d65  n(statement_time
+000093e0: 6f75 743d 3230 3030 290a 2020 2020 6465  out=2000).    de
+000093f0: 6620 736e 6170 7368 6f74 5f67 6574 5f62  f snapshot_get_b
+00009400: 7261 6e63 6865 7328 0a20 2020 2020 2020  ranches(.       
+00009410: 2073 656c 662c 0a20 2020 2020 2020 2073   self,.        s
+00009420: 6e61 7073 686f 745f 6964 3a20 5368 6131  napshot_id: Sha1
+00009430: 4769 742c 0a20 2020 2020 2020 2062 7261  Git,.        bra
+00009440: 6e63 6865 735f 6672 6f6d 3a20 6279 7465  nches_from: byte
+00009450: 7320 3d20 6222 222c 0a20 2020 2020 2020  s = b"",.       
+00009460: 2062 7261 6e63 6865 735f 636f 756e 743a   branches_count:
+00009470: 2069 6e74 203d 2031 3030 302c 0a20 2020   int = 1000,.   
+00009480: 2020 2020 2074 6172 6765 745f 7479 7065       target_type
+00009490: 733a 204f 7074 696f 6e61 6c5b 4c69 7374  s: Optional[List
+000094a0: 5b73 7472 5d5d 203d 204e 6f6e 652c 0a20  [str]] = None,. 
+000094b0: 2020 2020 2020 2062 7261 6e63 685f 6e61         branch_na
+000094c0: 6d65 5f69 6e63 6c75 6465 5f73 7562 7374  me_include_subst
+000094d0: 7269 6e67 3a20 4f70 7469 6f6e 616c 5b62  ring: Optional[b
+000094e0: 7974 6573 5d20 3d20 4e6f 6e65 2c0a 2020  ytes] = None,.  
+000094f0: 2020 2020 2020 6272 616e 6368 5f6e 616d        branch_nam
+00009500: 655f 6578 636c 7564 655f 7072 6566 6978  e_exclude_prefix
+00009510: 3a20 4f70 7469 6f6e 616c 5b62 7974 6573  : Optional[bytes
+00009520: 5d20 3d20 4e6f 6e65 2c0a 2020 2020 2020  ] = None,.      
+00009530: 2020 2a2c 0a20 2020 2020 2020 2064 623a    *,.        db:
+00009540: 2044 622c 0a20 2020 2020 2020 2063 7572   Db,.        cur
+00009550: 3d4e 6f6e 652c 0a20 2020 2029 202d 3e20  =None,.    ) -> 
+00009560: 4f70 7469 6f6e 616c 5b50 6172 7469 616c  Optional[Partial
+00009570: 4272 616e 6368 6573 5d3a 0a20 2020 2020  Branches]:.     
+00009580: 2020 2069 6620 736e 6170 7368 6f74 5f69     if snapshot_i
+00009590: 6420 3d3d 2045 4d50 5459 5f53 4e41 5053  d == EMPTY_SNAPS
+000095a0: 484f 545f 4944 3a0a 2020 2020 2020 2020  HOT_ID:.        
+000095b0: 2020 2020 7265 7475 726e 2050 6172 7469      return Parti
+000095c0: 616c 4272 616e 6368 6573 280a 2020 2020  alBranches(.    
+000095d0: 2020 2020 2020 2020 2020 2020 6964 3d73              id=s
+000095e0: 6e61 7073 686f 745f 6964 2c0a 2020 2020  napshot_id,.    
+000095f0: 2020 2020 2020 2020 2020 2020 6272 616e              bran
+00009600: 6368 6573 3d7b 7d2c 0a20 2020 2020 2020  ches={},.       
+00009610: 2020 2020 2020 2020 206e 6578 745f 6272           next_br
+00009620: 616e 6368 3d4e 6f6e 652c 0a20 2020 2020  anch=None,.     
+00009630: 2020 2020 2020 2029 0a0a 2020 2020 2020         )..      
+00009640: 2020 6966 206c 6973 7428 7365 6c66 2e73    if list(self.s
+00009650: 6e61 7073 686f 745f 6d69 7373 696e 6728  napshot_missing(
+00009660: 5b73 6e61 7073 686f 745f 6964 5d29 293a  [snapshot_id])):
+00009670: 0a20 2020 2020 2020 2020 2020 2072 6574  .            ret
+00009680: 7572 6e20 4e6f 6e65 0a0a 2020 2020 2020  urn None..      
+00009690: 2020 6272 616e 6368 6573 203d 207b 7d0a    branches = {}.
+000096a0: 2020 2020 2020 2020 6e65 7874 5f62 7261          next_bra
+000096b0: 6e63 6820 3d20 4e6f 6e65 0a0a 2020 2020  nch = None..    
+000096c0: 2020 2020 6665 7463 6865 645f 6272 616e      fetched_bran
+000096d0: 6368 6573 203d 206c 6973 7428 0a20 2020  ches = list(.   
+000096e0: 2020 2020 2020 2020 2064 622e 736e 6170           db.snap
+000096f0: 7368 6f74 5f67 6574 5f62 795f 6964 280a  shot_get_by_id(.
+00009700: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009710: 736e 6170 7368 6f74 5f69 642c 0a20 2020  snapshot_id,.   
+00009720: 2020 2020 2020 2020 2020 2020 2062 7261               bra
+00009730: 6e63 6865 735f 6672 6f6d 3d62 7261 6e63  nches_from=branc
+00009740: 6865 735f 6672 6f6d 2c0a 2020 2020 2020  hes_from,.      
+00009750: 2020 2020 2020 2020 2020 2320 7468 6520            # the 
+00009760: 756e 6465 726c 7969 6e67 2053 514c 2071  underlying SQL q
+00009770: 7565 7279 2063 616e 2062 6520 7175 6974  uery can be quit
+00009780: 6520 6578 7065 6e73 6976 6520 746f 2065  e expensive to e
+00009790: 7865 6375 7465 2066 6f72 2073 6d61 6c6c  xecute for small
+000097a0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000097b0: 2023 2062 7261 6e63 6865 735f 636f 756e   # branches_coun
+000097c0: 7420 7661 6c75 652c 2073 6f20 7765 2065  t value, so we e
+000097d0: 6e73 7572 6520 6120 6d69 6e69 6d75 6d20  nsure a minimum 
+000097e0: 6272 616e 6368 6573 206c 696d 6974 206f  branches limit o
+000097f0: 6620 3130 2066 6f72 0a20 2020 2020 2020  f 10 for.       
+00009800: 2020 2020 2020 2020 2023 206f 7074 696d           # optim
+00009810: 616c 2070 6572 666f 726d 616e 6365 730a  al performances.
+00009820: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009830: 6272 616e 6368 6573 5f63 6f75 6e74 3d6d  branches_count=m
+00009840: 6178 2862 7261 6e63 6865 735f 636f 756e  ax(branches_coun
+00009850: 7420 2b20 312c 2031 3029 2c0a 2020 2020  t + 1, 10),.    
+00009860: 2020 2020 2020 2020 2020 2020 7461 7267              targ
+00009870: 6574 5f74 7970 6573 3d74 6172 6765 745f  et_types=target_
+00009880: 7479 7065 732c 0a20 2020 2020 2020 2020  types,.         
+00009890: 2020 2020 2020 2062 7261 6e63 685f 6e61         branch_na
+000098a0: 6d65 5f69 6e63 6c75 6465 5f73 7562 7374  me_include_subst
+000098b0: 7269 6e67 3d62 7261 6e63 685f 6e61 6d65  ring=branch_name
+000098c0: 5f69 6e63 6c75 6465 5f73 7562 7374 7269  _include_substri
+000098d0: 6e67 2c0a 2020 2020 2020 2020 2020 2020  ng,.            
+000098e0: 2020 2020 6272 616e 6368 5f6e 616d 655f      branch_name_
+000098f0: 6578 636c 7564 655f 7072 6566 6978 3d62  exclude_prefix=b
+00009900: 7261 6e63 685f 6e61 6d65 5f65 7863 6c75  ranch_name_exclu
+00009910: 6465 5f70 7265 6669 782c 0a20 2020 2020  de_prefix,.     
+00009920: 2020 2020 2020 2020 2020 2063 7572 3d63             cur=c
+00009930: 7572 2c0a 2020 2020 2020 2020 2020 2020  ur,.            
+00009940: 290a 2020 2020 2020 2020 290a 2020 2020  ).        ).    
+00009950: 2020 2020 666f 7220 726f 7720 696e 2066      for row in f
+00009960: 6574 6368 6564 5f62 7261 6e63 6865 735b  etched_branches[
+00009970: 3a62 7261 6e63 6865 735f 636f 756e 745d  :branches_count]
+00009980: 3a0a 2020 2020 2020 2020 2020 2020 6272  :.            br
+00009990: 616e 6368 5f64 203d 2064 6963 7428 7a69  anch_d = dict(zi
+000099a0: 7028 6462 2e73 6e61 7073 686f 745f 6765  p(db.snapshot_ge
+000099b0: 745f 636f 6c73 2c20 726f 7729 290a 2020  t_cols, row)).  
+000099c0: 2020 2020 2020 2020 2020 6465 6c20 6272            del br
+000099d0: 616e 6368 5f64 5b22 736e 6170 7368 6f74  anch_d["snapshot
+000099e0: 5f69 6422 5d0a 2020 2020 2020 2020 2020  _id"].          
+000099f0: 2020 6e61 6d65 203d 2062 7261 6e63 685f    name = branch_
+00009a00: 642e 706f 7028 226e 616d 6522 290a 2020  d.pop("name").  
+00009a10: 2020 2020 2020 2020 2020 6966 2062 7261            if bra
+00009a20: 6e63 685f 645b 2274 6172 6765 7422 5d20  nch_d["target"] 
+00009a30: 6973 204e 6f6e 6520 616e 6420 6272 616e  is None and bran
+00009a40: 6368 5f64 5b22 7461 7267 6574 5f74 7970  ch_d["target_typ
+00009a50: 6522 5d20 6973 204e 6f6e 653a 0a20 2020  e"] is None:.   
+00009a60: 2020 2020 2020 2020 2020 2020 2062 7261               bra
+00009a70: 6e63 6820 3d20 4e6f 6e65 0a20 2020 2020  nch = None.     
+00009a80: 2020 2020 2020 2065 6c73 653a 0a20 2020         else:.   
+00009a90: 2020 2020 2020 2020 2020 2020 2061 7373               ass
+00009aa0: 6572 7420 6272 616e 6368 5f64 5b22 7461  ert branch_d["ta
+00009ab0: 7267 6574 5f74 7970 6522 5d20 6973 206e  rget_type"] is n
+00009ac0: 6f74 204e 6f6e 650a 2020 2020 2020 2020  ot None.        
+00009ad0: 2020 2020 2020 2020 6272 616e 6368 203d          branch =
+00009ae0: 2053 6e61 7073 686f 7442 7261 6e63 6828   SnapshotBranch(
+00009af0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00009b00: 2020 2020 2074 6172 6765 743d 6272 616e       target=bran
+00009b10: 6368 5f64 5b22 7461 7267 6574 225d 2c0a  ch_d["target"],.
+00009b20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009b30: 2020 2020 7461 7267 6574 5f74 7970 653d      target_type=
+00009b40: 536e 6170 7368 6f74 5461 7267 6574 5479  SnapshotTargetTy
+00009b50: 7065 2862 7261 6e63 685f 645b 2274 6172  pe(branch_d["tar
+00009b60: 6765 745f 7479 7065 225d 292c 0a20 2020  get_type"]),.   
+00009b70: 2020 2020 2020 2020 2020 2020 2029 0a20               ). 
+00009b80: 2020 2020 2020 2020 2020 2062 7261 6e63             branc
+00009b90: 6865 735b 6e61 6d65 5d20 3d20 6272 616e  hes[name] = bran
+00009ba0: 6368 0a0a 2020 2020 2020 2020 6966 206c  ch..        if l
+00009bb0: 656e 2866 6574 6368 6564 5f62 7261 6e63  en(fetched_branc
+00009bc0: 6865 7329 203e 2062 7261 6e63 6865 735f  hes) > branches_
+00009bd0: 636f 756e 743a 0a20 2020 2020 2020 2020  count:.         
+00009be0: 2020 206e 6578 745f 6272 616e 6368 203d     next_branch =
+00009bf0: 2064 6963 7428 0a20 2020 2020 2020 2020   dict(.         
+00009c00: 2020 2020 2020 207a 6970 2864 622e 736e         zip(db.sn
+00009c10: 6170 7368 6f74 5f67 6574 5f63 6f6c 732c  apshot_get_cols,
+00009c20: 2066 6574 6368 6564 5f62 7261 6e63 6865   fetched_branche
+00009c30: 735b 6272 616e 6368 6573 5f63 6f75 6e74  s[branches_count
+00009c40: 5d29 0a20 2020 2020 2020 2020 2020 2029  ]).            )
+00009c50: 5b22 6e61 6d65 225d 0a0a 2020 2020 2020  ["name"]..      
+00009c60: 2020 7265 7475 726e 2050 6172 7469 616c    return Partial
+00009c70: 4272 616e 6368 6573 280a 2020 2020 2020  Branches(.      
+00009c80: 2020 2020 2020 6964 3d73 6e61 7073 686f        id=snapsho
+00009c90: 745f 6964 2c0a 2020 2020 2020 2020 2020  t_id,.          
+00009ca0: 2020 6272 616e 6368 6573 3d62 7261 6e63    branches=branc
+00009cb0: 6865 732c 0a20 2020 2020 2020 2020 2020  hes,.           
+00009cc0: 206e 6578 745f 6272 616e 6368 3d6e 6578   next_branch=nex
+00009cd0: 745f 6272 616e 6368 2c0a 2020 2020 2020  t_branch,.      
+00009ce0: 2020 290a 0a20 2020 2040 6462 5f74 7261    )..    @db_tra
+00009cf0: 6e73 6163 7469 6f6e 2829 0a20 2020 2064  nsaction().    d
+00009d00: 6566 2073 6e61 7073 686f 745f 6765 745f  ef snapshot_get_
+00009d10: 7261 6e64 6f6d 2873 656c 662c 202a 2c20  random(self, *, 
+00009d20: 6462 3a20 4462 2c20 6375 723d 4e6f 6e65  db: Db, cur=None
+00009d30: 2920 2d3e 2053 6861 3147 6974 3a0a 2020  ) -> Sha1Git:.  
+00009d40: 2020 2020 2020 7265 7475 726e 2064 622e        return db.
+00009d50: 736e 6170 7368 6f74 5f67 6574 5f72 616e  snapshot_get_ran
+00009d60: 646f 6d28 6375 7229 0a0a 2020 2020 4064  dom(cur)..    @d
+00009d70: 625f 7472 616e 7361 6374 696f 6e28 7374  b_transaction(st
+00009d80: 6174 656d 656e 745f 7469 6d65 6f75 743d  atement_timeout=
+00009d90: 3230 3030 290a 2020 2020 6465 6620 736e  2000).    def sn
+00009da0: 6170 7368 6f74 5f62 7261 6e63 685f 6765  apshot_branch_ge
+00009db0: 745f 6279 5f6e 616d 6528 0a20 2020 2020  t_by_name(.     
+00009dc0: 2020 2073 656c 662c 0a20 2020 2020 2020     self,.       
+00009dd0: 2073 6e61 7073 686f 745f 6964 3a20 5368   snapshot_id: Sh
+00009de0: 6131 4769 742c 0a20 2020 2020 2020 2062  a1Git,.        b
+00009df0: 7261 6e63 685f 6e61 6d65 3a20 6279 7465  ranch_name: byte
+00009e00: 732c 0a20 2020 2020 2020 2064 623a 2044  s,.        db: D
+00009e10: 622c 0a20 2020 2020 2020 2063 7572 3d4e  b,.        cur=N
+00009e20: 6f6e 652c 0a20 2020 2020 2020 2066 6f6c  one,.        fol
+00009e30: 6c6f 775f 616c 6961 735f 6368 6169 6e3a  low_alias_chain:
+00009e40: 2062 6f6f 6c20 3d20 5472 7565 2c0a 2020   bool = True,.  
+00009e50: 2020 2020 2020 6d61 785f 616c 6961 735f        max_alias_
+00009e60: 6368 6169 6e5f 6c65 6e67 7468 3a20 696e  chain_length: in
+00009e70: 7420 3d20 3130 302c 0a20 2020 2029 202d  t = 100,.    ) -
+00009e80: 3e20 4f70 7469 6f6e 616c 5b53 6e61 7073  > Optional[Snaps
+00009e90: 686f 7442 7261 6e63 6842 794e 616d 6552  hotBranchByNameR
+00009ea0: 6573 706f 6e73 655d 3a0a 2020 2020 2020  esponse]:.      
+00009eb0: 2020 6966 206c 6973 7428 7365 6c66 2e73    if list(self.s
+00009ec0: 6e61 7073 686f 745f 6d69 7373 696e 6728  napshot_missing(
+00009ed0: 5b73 6e61 7073 686f 745f 6964 5d29 293a  [snapshot_id])):
+00009ee0: 0a20 2020 2020 2020 2020 2020 2072 6574  .            ret
+00009ef0: 7572 6e20 4e6f 6e65 0a0a 2020 2020 2020  urn None..      
+00009f00: 2020 6966 2073 6e61 7073 686f 745f 6964    if snapshot_id
+00009f10: 203d 3d20 454d 5054 595f 534e 4150 5348   == EMPTY_SNAPSH
+00009f20: 4f54 5f49 443a 0a20 2020 2020 2020 2020  OT_ID:.         
+00009f30: 2020 2072 6574 7572 6e20 536e 6170 7368     return Snapsh
+00009f40: 6f74 4272 616e 6368 4279 4e61 6d65 5265  otBranchByNameRe
+00009f50: 7370 6f6e 7365 280a 2020 2020 2020 2020  sponse(.        
+00009f60: 2020 2020 2020 2020 6272 616e 6368 5f66          branch_f
+00009f70: 6f75 6e64 3d46 616c 7365 2c0a 2020 2020  ound=False,.    
+00009f80: 2020 2020 2020 2020 2020 2020 7461 7267              targ
+00009f90: 6574 3d4e 6f6e 652c 0a20 2020 2020 2020  et=None,.       
+00009fa0: 2020 2020 2020 2020 2061 6c69 6173 6573           aliases
+00009fb0: 5f66 6f6c 6c6f 7765 643d 5b5d 2c0a 2020  _followed=[],.  
+00009fc0: 2020 2020 2020 2020 2020 290a 0a20 2020            )..   
+00009fd0: 2020 2020 2063 6f6c 735f 746f 5f66 6574       cols_to_fet
+00009fe0: 6368 203d 205b 2274 6172 6765 7422 2c20  ch = ["target", 
+00009ff0: 2274 6172 6765 745f 7479 7065 225d 0a20  "target_type"]. 
+0000a000: 2020 2020 2020 2072 6573 6f6c 7665 5f63         resolve_c
+0000a010: 6861 696e 3a20 4c69 7374 5b62 7974 6573  hain: List[bytes
+0000a020: 5d20 3d20 5b5d 0a20 2020 2020 2020 2077  ] = [].        w
+0000a030: 6869 6c65 2054 7275 653a 0a20 2020 2020  hile True:.     
+0000a040: 2020 2020 2020 2062 7261 6e63 6820 3d20         branch = 
+0000a050: 6462 2e73 6e61 7073 686f 745f 6272 616e  db.snapshot_bran
+0000a060: 6368 5f67 6574 5f62 795f 6e61 6d65 280a  ch_get_by_name(.
+0000a070: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a080: 636f 6c73 5f74 6f5f 6665 7463 683d 636f  cols_to_fetch=co
+0000a090: 6c73 5f74 6f5f 6665 7463 682c 0a20 2020  ls_to_fetch,.   
+0000a0a0: 2020 2020 2020 2020 2020 2020 2073 6e61               sna
+0000a0b0: 7073 686f 745f 6964 3d73 6e61 7073 686f  pshot_id=snapsho
+0000a0c0: 745f 6964 2c0a 2020 2020 2020 2020 2020  t_id,.          
+0000a0d0: 2020 2020 2020 6272 616e 6368 5f6e 616d        branch_nam
+0000a0e0: 653d 6272 616e 6368 5f6e 616d 652c 0a20  e=branch_name,. 
+0000a0f0: 2020 2020 2020 2020 2020 2020 2020 2063                 c
+0000a100: 7572 3d63 7572 2c0a 2020 2020 2020 2020  ur=cur,.        
+0000a110: 2020 2020 290a 2020 2020 2020 2020 2020      ).          
+0000a120: 2020 6966 2062 7261 6e63 6820 6973 204e    if branch is N
+0000a130: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
+0000a140: 2020 2020 2023 2074 6172 6765 7420 6272       # target br
+0000a150: 616e 6368 2069 7320 4e6f 6e65 2c20 7468  anch is None, th
+0000a160: 6572 6520 636f 756c 6420 6265 2069 7465  ere could be ite
+0000a170: 6d73 2069 6e20 616c 6961 7365 735f 666f  ms in aliases_fo
+0000a180: 6c6c 6f77 6564 0a20 2020 2020 2020 2020  llowed.         
+0000a190: 2020 2020 2020 2074 6172 6765 7420 3d20         target = 
+0000a1a0: 4e6f 6e65 0a20 2020 2020 2020 2020 2020  None.           
+0000a1b0: 2020 2020 2062 7265 616b 0a20 2020 2020       break.     
+0000a1c0: 2020 2020 2020 2062 7261 6e63 685f 6420         branch_d 
+0000a1d0: 3d20 6469 6374 287a 6970 2863 6f6c 735f  = dict(zip(cols_
+0000a1e0: 746f 5f66 6574 6368 2c20 6272 616e 6368  to_fetch, branch
+0000a1f0: 2929 0a20 2020 2020 2020 2020 2020 2072  )).            r
+0000a200: 6573 6f6c 7665 5f63 6861 696e 2e61 7070  esolve_chain.app
+0000a210: 656e 6428 6272 616e 6368 5f6e 616d 6529  end(branch_name)
+0000a220: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
+0000a230: 280a 2020 2020 2020 2020 2020 2020 2020  (.              
+0000a240: 2020 6272 616e 6368 5f64 5b22 7461 7267    branch_d["targ
+0000a250: 6574 5f74 7970 6522 5d20 213d 2053 6e61  et_type"] != Sna
+0000a260: 7073 686f 7454 6172 6765 7454 7970 652e  pshotTargetType.
+0000a270: 414c 4941 532e 7661 6c75 650a 2020 2020  ALIAS.value.    
+0000a280: 2020 2020 2020 2020 2020 2020 6f72 206e              or n
+0000a290: 6f74 2066 6f6c 6c6f 775f 616c 6961 735f  ot follow_alias_
+0000a2a0: 6368 6169 6e0a 2020 2020 2020 2020 2020  chain.          
+0000a2b0: 2020 293a 0a20 2020 2020 2020 2020 2020    ):.           
+0000a2c0: 2020 2020 2023 2066 6972 7374 206e 6f6e       # first non
+0000a2d0: 2061 6c69 6173 2062 7261 6e63 6820 6f72   alias branch or
+0000a2e0: 2074 6865 2066 6972 7374 2062 7261 6e63   the first branc
+0000a2f0: 6820 7768 656e 2066 6f6c 6c6f 775f 616c  h when follow_al
+0000a300: 6961 735f 6368 6169 6e20 6973 2046 616c  ias_chain is Fal
+0000a310: 7365 0a20 2020 2020 2020 2020 2020 2020  se.             
+0000a320: 2020 2074 6172 6765 7420 3d20 280a 2020     target = (.  
+0000a330: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a340: 2020 536e 6170 7368 6f74 4272 616e 6368    SnapshotBranch
+0000a350: 280a 2020 2020 2020 2020 2020 2020 2020  (.              
+0000a360: 2020 2020 2020 2020 2020 7461 7267 6574            target
+0000a370: 3d62 7261 6e63 685f 645b 2274 6172 6765  =branch_d["targe
+0000a380: 7422 5d2c 0a20 2020 2020 2020 2020 2020  t"],.           
+0000a390: 2020 2020 2020 2020 2020 2020 2074 6172               tar
+0000a3a0: 6765 745f 7479 7065 3d53 6e61 7073 686f  get_type=Snapsho
+0000a3b0: 7454 6172 6765 7454 7970 6528 6272 616e  tTargetType(bran
+0000a3c0: 6368 5f64 5b22 7461 7267 6574 5f74 7970  ch_d["target_typ
+0000a3d0: 6522 5d29 2c0a 2020 2020 2020 2020 2020  e"]),.          
+0000a3e0: 2020 2020 2020 2020 2020 290a 2020 2020            ).    
+0000a3f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a400: 6966 2062 7261 6e63 685f 645b 2274 6172  if branch_d["tar
+0000a410: 6765 7422 5d0a 2020 2020 2020 2020 2020  get"].          
+0000a420: 2020 2020 2020 2020 2020 656c 7365 204e            else N
+0000a430: 6f6e 650a 2020 2020 2020 2020 2020 2020  one.            
+0000a440: 2020 2020 290a 2020 2020 2020 2020 2020      ).          
+0000a450: 2020 2020 2020 6272 6561 6b0a 2020 2020        break.    
+0000a460: 2020 2020 2020 2020 656c 6966 2028 0a20          elif (. 
+0000a470: 2020 2020 2020 2020 2020 2020 2020 2023                 #
+0000a480: 2043 6972 6375 6c61 7220 7265 6665 7265   Circular refere
+0000a490: 6e63 650a 2020 2020 2020 2020 2020 2020  nce.            
+0000a4a0: 2020 2020 7265 736f 6c76 655f 6368 6169      resolve_chai
+0000a4b0: 6e2e 636f 756e 7428 6272 616e 6368 5f6e  n.count(branch_n
+0000a4c0: 616d 6529 203e 2031 0a20 2020 2020 2020  ame) > 1.       
+0000a4d0: 2020 2020 2020 2020 2023 2054 6f6f 206d           # Too m
+0000a4e0: 616e 7920 7265 2d64 6972 6563 7473 0a20  any re-directs. 
+0000a4f0: 2020 2020 2020 2020 2020 2020 2020 206f                 o
+0000a500: 7220 6c65 6e28 7265 736f 6c76 655f 6368  r len(resolve_ch
+0000a510: 6169 6e29 203e 3d20 6d61 785f 616c 6961  ain) >= max_alia
+0000a520: 735f 6368 6169 6e5f 6c65 6e67 7468 0a20  s_chain_length. 
+0000a530: 2020 2020 2020 2020 2020 2029 3a0a 2020             ):.  
+0000a540: 2020 2020 2020 2020 2020 2020 2020 7461                ta
+0000a550: 7267 6574 203d 204e 6f6e 650a 2020 2020  rget = None.    
+0000a560: 2020 2020 2020 2020 2020 2020 6272 6561              brea
+0000a570: 6b0a 2020 2020 2020 2020 2020 2020 2320  k.            # 
+0000a580: 4272 616e 6368 2068 6173 2061 206e 6f6e  Branch has a non
+0000a590: 2d4e 6f6e 6520 7461 7267 6574 2077 6974  -None target wit
+0000a5a0: 6820 7479 7065 2061 6c69 6173 0a20 2020  h type alias.   
+0000a5b0: 2020 2020 2020 2020 2062 7261 6e63 685f           branch_
+0000a5c0: 6e61 6d65 203d 2062 7261 6e63 685f 645b  name = branch_d[
+0000a5d0: 2274 6172 6765 7422 5d0a 0a20 2020 2020  "target"]..     
+0000a5e0: 2020 2072 6574 7572 6e20 536e 6170 7368     return Snapsh
+0000a5f0: 6f74 4272 616e 6368 4279 4e61 6d65 5265  otBranchByNameRe
+0000a600: 7370 6f6e 7365 280a 2020 2020 2020 2020  sponse(.        
+0000a610: 2020 2020 2320 7265 736f 6c76 655f 6368      # resolve_ch
+0000a620: 6961 6e20 6861 7320 6974 656d 732c 2062  ian has items, b
+0000a630: 7261 6368 5f66 6f75 6e64 206d 7573 7420  rach_found must 
+0000a640: 6265 2054 7275 650a 2020 2020 2020 2020  be True.        
+0000a650: 2020 2020 6272 616e 6368 5f66 6f75 6e64      branch_found
+0000a660: 3d62 6f6f 6c28 7265 736f 6c76 655f 6368  =bool(resolve_ch
+0000a670: 6169 6e29 2c0a 2020 2020 2020 2020 2020  ain),.          
+0000a680: 2020 7461 7267 6574 3d74 6172 6765 742c    target=target,
+0000a690: 0a20 2020 2020 2020 2020 2020 2061 6c69  .            ali
+0000a6a0: 6173 6573 5f66 6f6c 6c6f 7765 643d 7265  ases_followed=re
+0000a6b0: 736f 6c76 655f 6368 6169 6e2c 0a20 2020  solve_chain,.   
+0000a6c0: 2020 2020 2029 0a0a 2020 2020 2323 2323       )..    ####
+0000a6d0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+0000a6e0: 2323 2323 2323 0a20 2020 2023 204f 7269  ######.    # Ori
+0000a6f0: 6769 6e56 6973 6974 2061 6e64 204f 7269  ginVisit and Ori
+0000a700: 6769 6e56 6973 6974 5374 6174 7573 0a20  ginVisitStatus. 
+0000a710: 2020 2023 2323 2323 2323 2323 2323 2323     #############
+0000a720: 2323 2323 2323 2323 2323 2323 230a 0a20  #############.. 
+0000a730: 2020 2040 6462 5f74 7261 6e73 6163 7469     @db_transacti
+0000a740: 6f6e 2829 0a20 2020 2064 6566 206f 7269  on().    def ori
+0000a750: 6769 6e5f 7669 7369 745f 6164 6428 0a20  gin_visit_add(. 
+0000a760: 2020 2020 2020 2073 656c 662c 2076 6973         self, vis
+0000a770: 6974 733a 204c 6973 745b 4f72 6967 696e  its: List[Origin
+0000a780: 5669 7369 745d 2c20 2a2c 2064 623a 2044  Visit], *, db: D
+0000a790: 622c 2063 7572 3d4e 6f6e 650a 2020 2020  b, cur=None.    
+0000a7a0: 2920 2d3e 2049 7465 7261 626c 655b 4f72  ) -> Iterable[Or
+0000a7b0: 6967 696e 5669 7369 745d 3a0a 2020 2020  iginVisit]:.    
+0000a7c0: 2020 2020 666f 7220 7669 7369 7420 696e      for visit in
+0000a7d0: 2076 6973 6974 733a 0a20 2020 2020 2020   visits:.       
+0000a7e0: 2020 2020 206f 7269 6769 6e20 3d20 7365       origin = se
+0000a7f0: 6c66 2e6f 7269 6769 6e5f 6765 7428 5b76  lf.origin_get([v
+0000a800: 6973 6974 2e6f 7269 6769 6e5d 2c20 6462  isit.origin], db
+0000a810: 3d64 622c 2063 7572 3d63 7572 295b 305d  =db, cur=cur)[0]
+0000a820: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
+0000a830: 6e6f 7420 6f72 6967 696e 3a20 2023 2043  not origin:  # C
+0000a840: 616e 6e6f 7420 6164 6420 6120 7669 7369  annot add a visi
+0000a850: 7420 7769 7468 6f75 7420 616e 206f 7269  t without an ori
+0000a860: 6769 6e0a 2020 2020 2020 2020 2020 2020  gin.            
+0000a870: 2020 2020 7261 6973 6520 5374 6f72 6167      raise Storag
+0000a880: 6541 7267 756d 656e 7445 7863 6570 7469  eArgumentExcepti
+0000a890: 6f6e 2822 556e 6b6e 6f77 6e20 6f72 6967  on("Unknown orig
+0000a8a0: 696e 2025 7322 2c20 7669 7369 742e 6f72  in %s", visit.or
+0000a8b0: 6967 696e 290a 0a20 2020 2020 2020 2061  igin)..        a
+0000a8c0: 6c6c 5f76 6973 6974 7320 3d20 5b5d 0a20  ll_visits = []. 
+0000a8d0: 2020 2020 2020 2066 6f72 2076 6973 6974         for visit
+0000a8e0: 2069 6e20 7669 7369 7473 3a0a 2020 2020   in visits:.    
+0000a8f0: 2020 2020 2020 2020 6966 2076 6973 6974          if visit
+0000a900: 2e76 6973 6974 3a0a 2020 2020 2020 2020  .visit:.        
+0000a910: 2020 2020 2020 2020 7365 6c66 2e6a 6f75          self.jou
+0000a920: 726e 616c 5f77 7269 7465 722e 6f72 6967  rnal_writer.orig
+0000a930: 696e 5f76 6973 6974 5f61 6464 285b 7669  in_visit_add([vi
+0000a940: 7369 745d 290a 2020 2020 2020 2020 2020  sit]).          
+0000a950: 2020 2020 2020 6462 2e6f 7269 6769 6e5f        db.origin_
+0000a960: 7669 7369 745f 6164 645f 7769 7468 5f69  visit_add_with_i
+0000a970: 6428 7669 7369 742c 2063 7572 3d63 7572  d(visit, cur=cur
+0000a980: 290a 2020 2020 2020 2020 2020 2020 656c  ).            el
+0000a990: 7365 3a0a 2020 2020 2020 2020 2020 2020  se:.            
+0000a9a0: 2020 2020 2320 7669 7369 745f 6964 2069      # visit_id i
+0000a9b0: 7320 6e6f 7420 6769 7665 6e2c 2069 7420  s not given, it 
+0000a9c0: 6e65 6564 7320 746f 2062 6520 7365 7420  needs to be set 
+0000a9d0: 6279 2074 6865 2064 620a 2020 2020 2020  by the db.      
+0000a9e0: 2020 2020 2020 2020 2020 7769 7468 2063            with c
+0000a9f0: 6f6e 7665 7274 5f76 616c 6964 6174 696f  onvert_validatio
+0000aa00: 6e5f 6578 6365 7074 696f 6e73 2829 3a0a  n_exceptions():.
+0000aa10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000aa20: 2020 2020 7669 7369 745f 6964 203d 2064      visit_id = d
+0000aa30: 622e 6f72 6967 696e 5f76 6973 6974 5f61  b.origin_visit_a
+0000aa40: 6464 280a 2020 2020 2020 2020 2020 2020  dd(.            
+0000aa50: 2020 2020 2020 2020 2020 2020 7669 7369              visi
+0000aa60: 742e 6f72 6967 696e 2c20 7669 7369 742e  t.origin, visit.
+0000aa70: 6461 7465 2c20 7669 7369 742e 7479 7065  date, visit.type
+0000aa80: 2c20 6375 723d 6375 720a 2020 2020 2020  , cur=cur.      
+0000aa90: 2020 2020 2020 2020 2020 2020 2020 290a                ).
+0000aaa0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000aab0: 7669 7369 7420 3d20 6174 7472 2e65 766f  visit = attr.evo
+0000aac0: 6c76 6528 7669 7369 742c 2076 6973 6974  lve(visit, visit
+0000aad0: 3d76 6973 6974 5f69 6429 0a20 2020 2020  =visit_id).     
+0000aae0: 2020 2020 2020 2020 2020 2023 2046 6f72             # For
+0000aaf0: 6365 6420 746f 2077 7269 7465 2069 6e20  ced to write in 
+0000ab00: 7468 6520 6a6f 7572 6e61 6c20 6166 7465  the journal afte
+0000ab10: 7220 7468 6520 6462 2028 7369 6e63 6520  r the db (since 
+0000ab20: 6974 7320 7468 6520 6462 0a20 2020 2020  its the db.     
+0000ab30: 2020 2020 2020 2020 2020 2023 2063 616c             # cal
+0000ab40: 6c20 7468 6174 2073 6574 2074 6865 2076  l that set the v
+0000ab50: 6973 6974 2069 6429 0a20 2020 2020 2020  isit id).       
+0000ab60: 2020 2020 2020 2020 2073 656c 662e 6a6f           self.jo
+0000ab70: 7572 6e61 6c5f 7772 6974 6572 2e6f 7269  urnal_writer.ori
+0000ab80: 6769 6e5f 7669 7369 745f 6164 6428 5b76  gin_visit_add([v
+0000ab90: 6973 6974 5d29 0a20 2020 2020 2020 2020  isit]).         
+0000aba0: 2020 2020 2020 2023 2049 6e20 7468 6973         # In this
+0000abb0: 2063 6173 652c 2077 6520 616c 736f 2077   case, we also w
+0000abc0: 616e 7420 746f 2063 7265 6174 6520 7468  ant to create th
+0000abd0: 6520 696e 6974 6961 6c20 4f56 5320 6f62  e initial OVS ob
+0000abe0: 6a65 6374 0a20 2020 2020 2020 2020 2020  ject.           
+0000abf0: 2020 2020 2076 6973 6974 5f73 7461 7475       visit_statu
+0000ac00: 7320 3d20 4f72 6967 696e 5669 7369 7453  s = OriginVisitS
+0000ac10: 7461 7475 7328 0a20 2020 2020 2020 2020  tatus(.         
+0000ac20: 2020 2020 2020 2020 2020 206f 7269 6769             origi
+0000ac30: 6e3d 7669 7369 742e 6f72 6967 696e 2c0a  n=visit.origin,.
+0000ac40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ac50: 2020 2020 7669 7369 743d 7669 7369 745f      visit=visit_
+0000ac60: 6964 2c0a 2020 2020 2020 2020 2020 2020  id,.            
+0000ac70: 2020 2020 2020 2020 6461 7465 3d76 6973          date=vis
+0000ac80: 6974 2e64 6174 652c 0a20 2020 2020 2020  it.date,.       
+0000ac90: 2020 2020 2020 2020 2020 2020 2074 7970               typ
+0000aca0: 653d 7669 7369 742e 7479 7065 2c0a 2020  e=visit.type,.  
+0000acb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000acc0: 2020 7374 6174 7573 3d22 6372 6561 7465    status="create
+0000acd0: 6422 2c0a 2020 2020 2020 2020 2020 2020  d",.            
+0000ace0: 2020 2020 2020 2020 736e 6170 7368 6f74          snapshot
+0000acf0: 3d4e 6f6e 652c 0a20 2020 2020 2020 2020  =None,.         
+0000ad00: 2020 2020 2020 2029 0a20 2020 2020 2020         ).       
+0000ad10: 2020 2020 2020 2020 2073 656c 662e 5f6f           self._o
+0000ad20: 7269 6769 6e5f 7669 7369 745f 7374 6174  rigin_visit_stat
+0000ad30: 7573 5f61 6464 2876 6973 6974 5f73 7461  us_add(visit_sta
+0000ad40: 7475 732c 2064 623d 6462 2c20 6375 723d  tus, db=db, cur=
+0000ad50: 6375 7229 0a20 2020 2020 2020 2020 2020  cur).           
+0000ad60: 2061 7373 6572 7420 7669 7369 742e 7669   assert visit.vi
+0000ad70: 7369 7420 6973 206e 6f74 204e 6f6e 650a  sit is not None.
+0000ad80: 2020 2020 2020 2020 2020 2020 616c 6c5f              all_
+0000ad90: 7669 7369 7473 2e61 7070 656e 6428 7669  visits.append(vi
+0000ada0: 7369 7429 0a0a 2020 2020 2020 2020 7265  sit)..        re
+0000adb0: 7475 726e 2061 6c6c 5f76 6973 6974 730a  turn all_visits.
+0000adc0: 0a20 2020 2064 6566 205f 6f72 6967 696e  .    def _origin
+0000add0: 5f76 6973 6974 5f73 7461 7475 735f 6164  _visit_status_ad
+0000ade0: 6428 0a20 2020 2020 2020 2073 656c 662c  d(.        self,
+0000adf0: 2076 6973 6974 5f73 7461 7475 733a 204f   visit_status: O
+0000ae00: 7269 6769 6e56 6973 6974 5374 6174 7573  riginVisitStatus
+0000ae10: 2c20 6462 2c20 6375 720a 2020 2020 2920  , db, cur.    ) 
+0000ae20: 2d3e 204e 6f6e 653a 0a20 2020 2020 2020  -> None:.       
+0000ae30: 2022 2222 4164 6420 616e 206f 7269 6769   """Add an origi
+0000ae40: 6e20 7669 7369 7420 7374 6174 7573 2222  n visit status""
+0000ae50: 220a 2020 2020 2020 2020 7365 6c66 2e6a  ".        self.j
+0000ae60: 6f75 726e 616c 5f77 7269 7465 722e 6f72  ournal_writer.or
+0000ae70: 6967 696e 5f76 6973 6974 5f73 7461 7475  igin_visit_statu
+0000ae80: 735f 6164 6428 5b76 6973 6974 5f73 7461  s_add([visit_sta
+0000ae90: 7475 735d 290a 2020 2020 2020 2020 6462  tus]).        db
+0000aea0: 2e6f 7269 6769 6e5f 7669 7369 745f 7374  .origin_visit_st
+0000aeb0: 6174 7573 5f61 6464 2876 6973 6974 5f73  atus_add(visit_s
+0000aec0: 7461 7475 732c 2063 7572 3d63 7572 290a  tatus, cur=cur).
+0000aed0: 0a20 2020 2040 6462 5f74 7261 6e73 6163  .    @db_transac
+0000aee0: 7469 6f6e 2829 0a20 2020 2064 6566 206f  tion().    def o
+0000aef0: 7269 6769 6e5f 7669 7369 745f 7374 6174  rigin_visit_stat
+0000af00: 7573 5f61 6464 280a 2020 2020 2020 2020  us_add(.        
+0000af10: 7365 6c66 2c0a 2020 2020 2020 2020 7669  self,.        vi
+0000af20: 7369 745f 7374 6174 7573 6573 3a20 4c69  sit_statuses: Li
+0000af30: 7374 5b4f 7269 6769 6e56 6973 6974 5374  st[OriginVisitSt
+0000af40: 6174 7573 5d2c 0a20 2020 2020 2020 202a  atus],.        *
+0000af50: 2c0a 2020 2020 2020 2020 6462 3a20 4462  ,.        db: Db
+0000af60: 2c0a 2020 2020 2020 2020 6375 723d 4e6f  ,.        cur=No
+0000af70: 6e65 2c0a 2020 2020 2920 2d3e 2044 6963  ne,.    ) -> Dic
+0000af80: 745b 7374 722c 2069 6e74 5d3a 0a20 2020  t[str, int]:.   
+0000af90: 2020 2020 2076 6973 6974 5f73 7461 7475       visit_statu
+0000afa0: 7365 735f 203d 205b 5d0a 0a20 2020 2020  ses_ = []..     
+0000afb0: 2020 2023 2046 6972 7374 2072 6f75 6e64     # First round
+0000afc0: 2074 6f20 6368 6563 6b20 6578 6973 7465   to check existe
+0000afd0: 6e63 6520 2866 6169 6c20 6561 726c 7920  nce (fail early 
+0000afe0: 6966 2061 6e79 2069 7320 6b6f 290a 2020  if any is ko).  
+0000aff0: 2020 2020 2020 666f 7220 7669 7369 745f        for visit_
+0000b000: 7374 6174 7573 2069 6e20 7669 7369 745f  status in visit_
+0000b010: 7374 6174 7573 6573 3a0a 2020 2020 2020  statuses:.      
+0000b020: 2020 2020 2020 6f72 6967 696e 5f75 726c        origin_url
+0000b030: 203d 2073 656c 662e 6f72 6967 696e 5f67   = self.origin_g
+0000b040: 6574 285b 7669 7369 745f 7374 6174 7573  et([visit_status
+0000b050: 2e6f 7269 6769 6e5d 2c20 6462 3d64 622c  .origin], db=db,
+0000b060: 2063 7572 3d63 7572 295b 305d 0a20 2020   cur=cur)[0].   
+0000b070: 2020 2020 2020 2020 2069 6620 6e6f 7420           if not 
+0000b080: 6f72 6967 696e 5f75 726c 3a0a 2020 2020  origin_url:.    
+0000b090: 2020 2020 2020 2020 2020 2020 7261 6973              rais
+0000b0a0: 6520 5374 6f72 6167 6541 7267 756d 656e  e StorageArgumen
+0000b0b0: 7445 7863 6570 7469 6f6e 2866 2255 6e6b  tException(f"Unk
+0000b0c0: 6e6f 776e 206f 7269 6769 6e20 7b76 6973  nown origin {vis
+0000b0d0: 6974 5f73 7461 7475 732e 6f72 6967 696e  it_status.origin
+0000b0e0: 7d22 290a 0a20 2020 2020 2020 2020 2020  }")..           
+0000b0f0: 2069 6620 7669 7369 745f 7374 6174 7573   if visit_status
+0000b100: 2e74 7970 6520 6973 204e 6f6e 653a 0a20  .type is None:. 
+0000b110: 2020 2020 2020 2020 2020 2020 2020 206f                 o
+0000b120: 7269 6769 6e5f 7669 7369 7420 3d20 7365  rigin_visit = se
+0000b130: 6c66 2e6f 7269 6769 6e5f 7669 7369 745f  lf.origin_visit_
+0000b140: 6765 745f 6279 280a 2020 2020 2020 2020  get_by(.        
+0000b150: 2020 2020 2020 2020 2020 2020 7669 7369              visi
+0000b160: 745f 7374 6174 7573 2e6f 7269 6769 6e2c  t_status.origin,
+0000b170: 2076 6973 6974 5f73 7461 7475 732e 7669   visit_status.vi
+0000b180: 7369 742c 2064 623d 6462 2c20 6375 723d  sit, db=db, cur=
+0000b190: 6375 720a 2020 2020 2020 2020 2020 2020  cur.            
+0000b1a0: 2020 2020 290a 2020 2020 2020 2020 2020      ).          
+0000b1b0: 2020 2020 2020 6966 206f 7269 6769 6e5f        if origin_
+0000b1c0: 7669 7369 7420 6973 204e 6f6e 653a 0a20  visit is None:. 
+0000b1d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b1e0: 2020 2072 6169 7365 2053 746f 7261 6765     raise Storage
+0000b1f0: 4172 6775 6d65 6e74 4578 6365 7074 696f  ArgumentExceptio
+0000b200: 6e28 0a20 2020 2020 2020 2020 2020 2020  n(.             
+0000b210: 2020 2020 2020 2020 2020 2066 2255 6e6b             f"Unk
+0000b220: 6e6f 776e 206f 7269 6769 6e20 7669 7369  nown origin visi
+0000b230: 7420 7b76 6973 6974 5f73 7461 7475 732e  t {visit_status.
+0000b240: 7669 7369 747d 2022 0a20 2020 2020 2020  visit} ".       
+0000b250: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b260: 2066 226f 6620 6f72 6967 696e 207b 7669   f"of origin {vi
+0000b270: 7369 745f 7374 6174 7573 2e6f 7269 6769  sit_status.origi
+0000b280: 6e7d 220a 2020 2020 2020 2020 2020 2020  n}".            
+0000b290: 2020 2020 2020 2020 290a 0a20 2020 2020          )..     
+0000b2a0: 2020 2020 2020 2020 2020 206f 7269 6769             origi
+0000b2b0: 6e5f 7669 7369 745f 7374 6174 7573 203d  n_visit_status =
+0000b2c0: 2061 7474 722e 6576 6f6c 7665 2876 6973   attr.evolve(vis
+0000b2d0: 6974 5f73 7461 7475 732c 2074 7970 653d  it_status, type=
+0000b2e0: 6f72 6967 696e 5f76 6973 6974 2e74 7970  origin_visit.typ
+0000b2f0: 6529 0a20 2020 2020 2020 2020 2020 2065  e).            e
+0000b300: 6c73 653a 0a20 2020 2020 2020 2020 2020  lse:.           
+0000b310: 2020 2020 206f 7269 6769 6e5f 7669 7369       origin_visi
+0000b320: 745f 7374 6174 7573 203d 2076 6973 6974  t_status = visit
+0000b330: 5f73 7461 7475 730a 0a20 2020 2020 2020  _status..       
+0000b340: 2020 2020 2076 6973 6974 5f73 7461 7475       visit_statu
+0000b350: 7365 735f 2e61 7070 656e 6428 6f72 6967  ses_.append(orig
+0000b360: 696e 5f76 6973 6974 5f73 7461 7475 7329  in_visit_status)
+0000b370: 0a0a 2020 2020 2020 2020 666f 7220 7669  ..        for vi
+0000b380: 7369 745f 7374 6174 7573 2069 6e20 7669  sit_status in vi
+0000b390: 7369 745f 7374 6174 7573 6573 5f3a 0a20  sit_statuses_:. 
+0000b3a0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+0000b3b0: 5f6f 7269 6769 6e5f 7669 7369 745f 7374  _origin_visit_st
+0000b3c0: 6174 7573 5f61 6464 2876 6973 6974 5f73  atus_add(visit_s
+0000b3d0: 7461 7475 732c 2064 622c 2063 7572 290a  tatus, db, cur).
+0000b3e0: 2020 2020 2020 2020 7265 7475 726e 207b          return {
+0000b3f0: 226f 7269 6769 6e5f 7669 7369 745f 7374  "origin_visit_st
+0000b400: 6174 7573 3a61 6464 223a 206c 656e 2876  atus:add": len(v
+0000b410: 6973 6974 5f73 7461 7475 7365 735f 297d  isit_statuses_)}
+0000b420: 0a0a 2020 2020 4064 625f 7472 616e 7361  ..    @db_transa
+0000b430: 6374 696f 6e28 290a 2020 2020 6465 6620  ction().    def 
+0000b440: 6f72 6967 696e 5f76 6973 6974 5f73 7461  origin_visit_sta
+0000b450: 7475 735f 6765 745f 6c61 7465 7374 280a  tus_get_latest(.
+0000b460: 2020 2020 2020 2020 7365 6c66 2c0a 2020          self,.  
+0000b470: 2020 2020 2020 6f72 6967 696e 5f75 726c        origin_url
+0000b480: 3a20 7374 722c 0a20 2020 2020 2020 2076  : str,.        v
+0000b490: 6973 6974 3a20 696e 742c 0a20 2020 2020  isit: int,.     
+0000b4a0: 2020 2061 6c6c 6f77 6564 5f73 7461 7475     allowed_statu
+0000b4b0: 7365 733a 204f 7074 696f 6e61 6c5b 4c69  ses: Optional[Li
+0000b4c0: 7374 5b73 7472 5d5d 203d 204e 6f6e 652c  st[str]] = None,
+0000b4d0: 0a20 2020 2020 2020 2072 6571 7569 7265  .        require
+0000b4e0: 5f73 6e61 7073 686f 743a 2062 6f6f 6c20  _snapshot: bool 
+0000b4f0: 3d20 4661 6c73 652c 0a20 2020 2020 2020  = False,.       
+0000b500: 202a 2c0a 2020 2020 2020 2020 6462 3a20   *,.        db: 
+0000b510: 4462 2c0a 2020 2020 2020 2020 6375 723d  Db,.        cur=
+0000b520: 4e6f 6e65 2c0a 2020 2020 2920 2d3e 204f  None,.    ) -> O
+0000b530: 7074 696f 6e61 6c5b 4f72 6967 696e 5669  ptional[OriginVi
+0000b540: 7369 7453 7461 7475 735d 3a0a 2020 2020  sitStatus]:.    
+0000b550: 2020 2020 6966 2061 6c6c 6f77 6564 5f73      if allowed_s
+0000b560: 7461 7475 7365 7320 616e 6420 6e6f 7420  tatuses and not 
+0000b570: 7365 7428 616c 6c6f 7765 645f 7374 6174  set(allowed_stat
+0000b580: 7573 6573 292e 696e 7465 7273 6563 7469  uses).intersecti
+0000b590: 6f6e 2856 4953 4954 5f53 5441 5455 5345  on(VISIT_STATUSE
+0000b5a0: 5329 3a0a 2020 2020 2020 2020 2020 2020  S):.            
+0000b5b0: 7261 6973 6520 5374 6f72 6167 6541 7267  raise StorageArg
+0000b5c0: 756d 656e 7445 7863 6570 7469 6f6e 280a  umentException(.
+0000b5d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b5e0: 6622 556e 6b6e 6f77 6e20 616c 6c6f 7765  f"Unknown allowe
+0000b5f0: 6420 7374 6174 7573 6573 207b 272c 272e  d statuses {','.
+0000b600: 6a6f 696e 2861 6c6c 6f77 6564 5f73 7461  join(allowed_sta
+0000b610: 7475 7365 7329 7d2c 206f 6e6c 7920 220a  tuses)}, only ".
+0000b620: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b630: 6622 7b27 2c27 2e6a 6f69 6e28 5649 5349  f"{','.join(VISI
+0000b640: 545f 5354 4154 5553 4553 297d 2061 7574  T_STATUSES)} aut
+0000b650: 686f 7269 7a65 6422 0a20 2020 2020 2020  horized".       
+0000b660: 2020 2020 2029 0a0a 2020 2020 2020 2020       )..        
+0000b670: 726f 775f 6420 3d20 6462 2e6f 7269 6769  row_d = db.origi
+0000b680: 6e5f 7669 7369 745f 7374 6174 7573 5f67  n_visit_status_g
+0000b690: 6574 5f6c 6174 6573 7428 0a20 2020 2020  et_latest(.     
+0000b6a0: 2020 2020 2020 206f 7269 6769 6e5f 7572         origin_ur
+0000b6b0: 6c2c 2076 6973 6974 2c20 616c 6c6f 7765  l, visit, allowe
+0000b6c0: 645f 7374 6174 7573 6573 2c20 7265 7175  d_statuses, requ
+0000b6d0: 6972 655f 736e 6170 7368 6f74 2c20 6375  ire_snapshot, cu
+0000b6e0: 723d 6375 720a 2020 2020 2020 2020 290a  r=cur.        ).
+0000b6f0: 2020 2020 2020 2020 6966 206e 6f74 2072          if not r
+0000b700: 6f77 5f64 3a0a 2020 2020 2020 2020 2020  ow_d:.          
+0000b710: 2020 7265 7475 726e 204e 6f6e 650a 2020    return None.  
+0000b720: 2020 2020 2020 7265 7475 726e 204f 7269        return Ori
+0000b730: 6769 6e56 6973 6974 5374 6174 7573 282a  ginVisitStatus(*
+0000b740: 2a72 6f77 5f64 290a 0a20 2020 2040 6462  *row_d)..    @db
+0000b750: 5f74 7261 6e73 6163 7469 6f6e 2873 7461  _transaction(sta
+0000b760: 7465 6d65 6e74 5f74 696d 656f 7574 3d35  tement_timeout=5
+0000b770: 3030 290a 2020 2020 6465 6620 6f72 6967  00).    def orig
+0000b780: 696e 5f76 6973 6974 5f67 6574 280a 2020  in_visit_get(.  
+0000b790: 2020 2020 2020 7365 6c66 2c0a 2020 2020        self,.    
+0000b7a0: 2020 2020 6f72 6967 696e 3a20 7374 722c      origin: str,
+0000b7b0: 0a20 2020 2020 2020 2070 6167 655f 746f  .        page_to
+0000b7c0: 6b65 6e3a 204f 7074 696f 6e61 6c5b 7374  ken: Optional[st
+0000b7d0: 725d 203d 204e 6f6e 652c 0a20 2020 2020  r] = None,.     
+0000b7e0: 2020 206f 7264 6572 3a20 4c69 7374 4f72     order: ListOr
+0000b7f0: 6465 7220 3d20 4c69 7374 4f72 6465 722e  der = ListOrder.
+0000b800: 4153 432c 0a20 2020 2020 2020 206c 696d  ASC,.        lim
+0000b810: 6974 3a20 696e 7420 3d20 3130 2c0a 2020  it: int = 10,.  
+0000b820: 2020 2020 2020 2a2c 0a20 2020 2020 2020        *,.       
+0000b830: 2064 623a 2044 622c 0a20 2020 2020 2020   db: Db,.       
+0000b840: 2063 7572 3d4e 6f6e 652c 0a20 2020 2029   cur=None,.    )
+0000b850: 202d 3e20 5061 6765 6452 6573 756c 745b   -> PagedResult[
+0000b860: 4f72 6967 696e 5669 7369 745d 3a0a 2020  OriginVisit]:.  
+0000b870: 2020 2020 2020 7061 6765 5f74 6f6b 656e        page_token
+0000b880: 203d 2070 6167 655f 746f 6b65 6e20 6f72   = page_token or
+0000b890: 2022 3022 0a20 2020 2020 2020 2069 6620   "0".        if 
+0000b8a0: 6e6f 7420 6973 696e 7374 616e 6365 286f  not isinstance(o
+0000b8b0: 7264 6572 2c20 4c69 7374 4f72 6465 7229  rder, ListOrder)
+0000b8c0: 3a0a 2020 2020 2020 2020 2020 2020 7261  :.            ra
+0000b8d0: 6973 6520 5374 6f72 6167 6541 7267 756d  ise StorageArgum
+0000b8e0: 656e 7445 7863 6570 7469 6f6e 2822 6f72  entException("or
+0000b8f0: 6465 7220 6d75 7374 2062 6520 6120 4c69  der must be a Li
+0000b900: 7374 4f72 6465 7220 7661 6c75 6522 290a  stOrder value").
+0000b910: 2020 2020 2020 2020 6966 206e 6f74 2069          if not i
+0000b920: 7369 6e73 7461 6e63 6528 7061 6765 5f74  sinstance(page_t
+0000b930: 6f6b 656e 2c20 7374 7229 3a0a 2020 2020  oken, str):.    
+0000b940: 2020 2020 2020 2020 7261 6973 6520 5374          raise St
+0000b950: 6f72 6167 6541 7267 756d 656e 7445 7863  orageArgumentExc
+0000b960: 6570 7469 6f6e 2822 7061 6765 5f74 6f6b  eption("page_tok
+0000b970: 656e 206d 7573 7420 6265 2061 2073 7472  en must be a str
+0000b980: 696e 672e 2229 0a0a 2020 2020 2020 2020  ing.")..        
+0000b990: 6e65 7874 5f70 6167 655f 746f 6b65 6e20  next_page_token 
+0000b9a0: 3d20 4e6f 6e65 0a20 2020 2020 2020 2076  = None.        v
+0000b9b0: 6973 6974 5f66 726f 6d20 3d20 696e 7428  isit_from = int(
+0000b9c0: 7061 6765 5f74 6f6b 656e 290a 2020 2020  page_token).    
+0000b9d0: 2020 2020 7669 7369 7473 3a20 4c69 7374      visits: List
+0000b9e0: 5b4f 7269 6769 6e56 6973 6974 5d20 3d20  [OriginVisit] = 
+0000b9f0: 5b5d 0a20 2020 2020 2020 2065 7874 7261  [].        extra
+0000ba00: 5f6c 696d 6974 203d 206c 696d 6974 202b  _limit = limit +
+0000ba10: 2031 0a20 2020 2020 2020 2066 6f72 2072   1.        for r
+0000ba20: 6f77 2069 6e20 6462 2e6f 7269 6769 6e5f  ow in db.origin_
+0000ba30: 7669 7369 745f 6765 745f 7261 6e67 6528  visit_get_range(
+0000ba40: 0a20 2020 2020 2020 2020 2020 206f 7269  .            ori
+0000ba50: 6769 6e2c 2076 6973 6974 5f66 726f 6d3d  gin, visit_from=
+0000ba60: 7669 7369 745f 6672 6f6d 2c20 6f72 6465  visit_from, orde
+0000ba70: 723d 6f72 6465 722c 206c 696d 6974 3d65  r=order, limit=e
+0000ba80: 7874 7261 5f6c 696d 6974 2c20 6375 723d  xtra_limit, cur=
+0000ba90: 6375 720a 2020 2020 2020 2020 293a 0a20  cur.        ):. 
+0000baa0: 2020 2020 2020 2020 2020 2072 6f77 5f64             row_d
+0000bab0: 203d 2064 6963 7428 7a69 7028 6462 2e6f   = dict(zip(db.o
+0000bac0: 7269 6769 6e5f 7669 7369 745f 636f 6c73  rigin_visit_cols
+0000bad0: 2c20 726f 7729 290a 2020 2020 2020 2020  , row)).        
+0000bae0: 2020 2020 7669 7369 7473 2e61 7070 656e      visits.appen
+0000baf0: 6428 0a20 2020 2020 2020 2020 2020 2020  d(.             
+0000bb00: 2020 204f 7269 6769 6e56 6973 6974 280a     OriginVisit(.
+0000bb10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000bb20: 2020 2020 6f72 6967 696e 3d72 6f77 5f64      origin=row_d
+0000bb30: 5b22 6f72 6967 696e 225d 2c0a 2020 2020  ["origin"],.    
+0000bb40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000bb50: 7669 7369 743d 726f 775f 645b 2276 6973  visit=row_d["vis
+0000bb60: 6974 225d 2c0a 2020 2020 2020 2020 2020  it"],.          
+0000bb70: 2020 2020 2020 2020 2020 6461 7465 3d72            date=r
+0000bb80: 6f77 5f64 5b22 6461 7465 225d 2c0a 2020  ow_d["date"],.  
+0000bb90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000bba0: 2020 7479 7065 3d72 6f77 5f64 5b22 7479    type=row_d["ty
+0000bbb0: 7065 225d 2c0a 2020 2020 2020 2020 2020  pe"],.          
+0000bbc0: 2020 2020 2020 290a 2020 2020 2020 2020        ).        
+0000bbd0: 2020 2020 290a 0a20 2020 2020 2020 2061      )..        a
+0000bbe0: 7373 6572 7420 6c65 6e28 7669 7369 7473  ssert len(visits
+0000bbf0: 2920 3c3d 2065 7874 7261 5f6c 696d 6974  ) <= extra_limit
+0000bc00: 0a0a 2020 2020 2020 2020 6966 206c 656e  ..        if len
+0000bc10: 2876 6973 6974 7329 203d 3d20 6578 7472  (visits) == extr
+0000bc20: 615f 6c69 6d69 743a 0a20 2020 2020 2020  a_limit:.       
+0000bc30: 2020 2020 2076 6973 6974 7320 3d20 7669       visits = vi
+0000bc40: 7369 7473 5b3a 6c69 6d69 745d 0a20 2020  sits[:limit].   
+0000bc50: 2020 2020 2020 2020 206e 6578 745f 7061           next_pa
+0000bc60: 6765 5f74 6f6b 656e 203d 2073 7472 2876  ge_token = str(v
+0000bc70: 6973 6974 735b 2d31 5d2e 7669 7369 7429  isits[-1].visit)
+0000bc80: 0a0a 2020 2020 2020 2020 7265 7475 726e  ..        return
+0000bc90: 2050 6167 6564 5265 7375 6c74 2872 6573   PagedResult(res
+0000bca0: 756c 7473 3d76 6973 6974 732c 206e 6578  ults=visits, nex
+0000bcb0: 745f 7061 6765 5f74 6f6b 656e 3d6e 6578  t_page_token=nex
+0000bcc0: 745f 7061 6765 5f74 6f6b 656e 290a 0a20  t_page_token).. 
+0000bcd0: 2020 2040 6462 5f74 7261 6e73 6163 7469     @db_transacti
+0000bce0: 6f6e 2873 7461 7465 6d65 6e74 5f74 696d  on(statement_tim
+0000bcf0: 656f 7574 3d32 3030 3029 0a20 2020 2064  eout=2000).    d
+0000bd00: 6566 206f 7269 6769 6e5f 7669 7369 745f  ef origin_visit_
+0000bd10: 6765 745f 7769 7468 5f73 7461 7475 7365  get_with_statuse
+0000bd20: 7328 0a20 2020 2020 2020 2073 656c 662c  s(.        self,
+0000bd30: 0a20 2020 2020 2020 206f 7269 6769 6e3a  .        origin:
+0000bd40: 2073 7472 2c0a 2020 2020 2020 2020 616c   str,.        al
+0000bd50: 6c6f 7765 645f 7374 6174 7573 6573 3a20  lowed_statuses: 
+0000bd60: 4f70 7469 6f6e 616c 5b4c 6973 745b 7374  Optional[List[st
+0000bd70: 725d 5d20 3d20 4e6f 6e65 2c0a 2020 2020  r]] = None,.    
+0000bd80: 2020 2020 7265 7175 6972 655f 736e 6170      require_snap
+0000bd90: 7368 6f74 3a20 626f 6f6c 203d 2046 616c  shot: bool = Fal
+0000bda0: 7365 2c0a 2020 2020 2020 2020 7061 6765  se,.        page
+0000bdb0: 5f74 6f6b 656e 3a20 4f70 7469 6f6e 616c  _token: Optional
+0000bdc0: 5b73 7472 5d20 3d20 4e6f 6e65 2c0a 2020  [str] = None,.  
+0000bdd0: 2020 2020 2020 6f72 6465 723a 204c 6973        order: Lis
+0000bde0: 744f 7264 6572 203d 204c 6973 744f 7264  tOrder = ListOrd
+0000bdf0: 6572 2e41 5343 2c0a 2020 2020 2020 2020  er.ASC,.        
+0000be00: 6c69 6d69 743a 2069 6e74 203d 2031 302c  limit: int = 10,
+0000be10: 0a20 2020 2020 2020 202a 2c0a 2020 2020  .        *,.    
+0000be20: 2020 2020 6462 3a20 4462 2c0a 2020 2020      db: Db,.    
+0000be30: 2020 2020 6375 723d 4e6f 6e65 2c0a 2020      cur=None,.  
+0000be40: 2020 2920 2d3e 2050 6167 6564 5265 7375    ) -> PagedResu
+0000be50: 6c74 5b4f 7269 6769 6e56 6973 6974 5769  lt[OriginVisitWi
+0000be60: 7468 5374 6174 7573 6573 5d3a 0a20 2020  thStatuses]:.   
+0000be70: 2020 2020 2070 6167 655f 746f 6b65 6e20       page_token 
+0000be80: 3d20 7061 6765 5f74 6f6b 656e 206f 7220  = page_token or 
+0000be90: 2230 220a 2020 2020 2020 2020 6966 206e  "0".        if n
+0000bea0: 6f74 2069 7369 6e73 7461 6e63 6528 6f72  ot isinstance(or
+0000beb0: 6465 722c 204c 6973 744f 7264 6572 293a  der, ListOrder):
+0000bec0: 0a20 2020 2020 2020 2020 2020 2072 6169  .            rai
+0000bed0: 7365 2053 746f 7261 6765 4172 6775 6d65  se StorageArgume
+0000bee0: 6e74 4578 6365 7074 696f 6e28 226f 7264  ntException("ord
+0000bef0: 6572 206d 7573 7420 6265 2061 204c 6973  er must be a Lis
+0000bf00: 744f 7264 6572 2076 616c 7565 2229 0a20  tOrder value"). 
+0000bf10: 2020 2020 2020 2069 6620 6e6f 7420 6973         if not is
+0000bf20: 696e 7374 616e 6365 2870 6167 655f 746f  instance(page_to
+0000bf30: 6b65 6e2c 2073 7472 293a 0a20 2020 2020  ken, str):.     
+0000bf40: 2020 2020 2020 2072 6169 7365 2053 746f         raise Sto
+0000bf50: 7261 6765 4172 6775 6d65 6e74 4578 6365  rageArgumentExce
+0000bf60: 7074 696f 6e28 2270 6167 655f 746f 6b65  ption("page_toke
+0000bf70: 6e20 6d75 7374 2062 6520 6120 7374 7269  n must be a stri
+0000bf80: 6e67 2e22 290a 0a20 2020 2020 2020 2023  ng.")..        #
+0000bf90: 2046 6972 7374 2067 6574 2076 6973 6974   First get visit
+0000bfa0: 7320 2870 6c75 7320 6f6e 6520 736f 2077  s (plus one so w
+0000bfb0: 6520 6361 6e20 7573 6520 6974 2061 7320  e can use it as 
+0000bfc0: 7468 6520 6e65 7874 2070 6167 6520 746f  the next page to
+0000bfd0: 6b65 6e20 6966 2061 6e79 290a 2020 2020  ken if any).    
+0000bfe0: 2020 2020 7669 7369 7473 5f70 6167 6520      visits_page 
+0000bff0: 3d20 7365 6c66 2e6f 7269 6769 6e5f 7669  = self.origin_vi
+0000c000: 7369 745f 6765 7428 0a20 2020 2020 2020  sit_get(.       
+0000c010: 2020 2020 206f 7269 6769 6e3d 6f72 6967       origin=orig
+0000c020: 696e 2c0a 2020 2020 2020 2020 2020 2020  in,.            
+0000c030: 7061 6765 5f74 6f6b 656e 3d70 6167 655f  page_token=page_
+0000c040: 746f 6b65 6e2c 0a20 2020 2020 2020 2020  token,.         
+0000c050: 2020 206f 7264 6572 3d6f 7264 6572 2c0a     order=order,.
+0000c060: 2020 2020 2020 2020 2020 2020 6c69 6d69              limi
+0000c070: 743d 6c69 6d69 742c 0a20 2020 2020 2020  t=limit,.       
+0000c080: 2020 2020 2064 623d 6462 2c0a 2020 2020       db=db,.    
+0000c090: 2020 2020 2020 2020 6375 723d 6375 722c          cur=cur,
+0000c0a0: 0a20 2020 2020 2020 2029 0a0a 2020 2020  .        )..    
+0000c0b0: 2020 2020 7669 7369 7473 203d 2076 6973      visits = vis
+0000c0c0: 6974 735f 7061 6765 2e72 6573 756c 7473  its_page.results
+0000c0d0: 0a20 2020 2020 2020 206e 6578 745f 7061  .        next_pa
+0000c0e0: 6765 5f74 6f6b 656e 203d 2076 6973 6974  ge_token = visit
+0000c0f0: 735f 7061 6765 2e6e 6578 745f 7061 6765  s_page.next_page
+0000c100: 5f74 6f6b 656e 0a0a 2020 2020 2020 2020  _token..        
+0000c110: 6966 2076 6973 6974 733a 0a20 2020 2020  if visits:.     
+0000c120: 2020 2020 2020 2076 6973 6974 5f66 726f         visit_fro
+0000c130: 6d20 3d20 6d69 6e28 7669 7369 7473 5b30  m = min(visits[0
+0000c140: 5d2e 7669 7369 742c 2076 6973 6974 735b  ].visit, visits[
+0000c150: 2d31 5d2e 7669 7369 7429 0a20 2020 2020  -1].visit).     
+0000c160: 2020 2020 2020 2076 6973 6974 5f74 6f20         visit_to 
+0000c170: 3d20 6d61 7828 7669 7369 7473 5b30 5d2e  = max(visits[0].
+0000c180: 7669 7369 742c 2076 6973 6974 735b 2d31  visit, visits[-1
+0000c190: 5d2e 7669 7369 7429 0a0a 2020 2020 2020  ].visit)..      
+0000c1a0: 2020 2020 2020 2320 5468 656e 2c20 6665        # Then, fe
+0000c1b0: 7463 6820 616c 6c20 7374 6174 7573 6573  tch all statuses
+0000c1c0: 2061 7373 6f63 6961 7465 6420 746f 2074   associated to t
+0000c1d0: 6865 7365 2076 6973 6974 730a 2020 2020  hese visits.    
+0000c1e0: 2020 2020 2020 2020 7669 7369 745f 7374          visit_st
+0000c1f0: 6174 7573 6573 3a20 4469 6374 5b69 6e74  atuses: Dict[int
+0000c200: 2c20 4c69 7374 5b4f 7269 6769 6e56 6973  , List[OriginVis
+0000c210: 6974 5374 6174 7573 5d5d 203d 2064 6566  itStatus]] = def
+0000c220: 6175 6c74 6469 6374 286c 6973 7429 0a20  aultdict(list). 
+0000c230: 2020 2020 2020 2020 2020 2066 6f72 2072             for r
+0000c240: 6f77 2069 6e20 6462 2e6f 7269 6769 6e5f  ow in db.origin_
+0000c250: 7669 7369 745f 7374 6174 7573 5f67 6574  visit_status_get
+0000c260: 5f61 6c6c 5f69 6e5f 7261 6e67 6528 0a20  _all_in_range(. 
+0000c270: 2020 2020 2020 2020 2020 2020 2020 206f                 o
+0000c280: 7269 6769 6e2c 0a20 2020 2020 2020 2020  rigin,.         
+0000c290: 2020 2020 2020 2061 6c6c 6f77 6564 5f73         allowed_s
+0000c2a0: 7461 7475 7365 732c 0a20 2020 2020 2020  tatuses,.       
+0000c2b0: 2020 2020 2020 2020 2072 6571 7569 7265           require
+0000c2c0: 5f73 6e61 7073 686f 742c 0a20 2020 2020  _snapshot,.     
+0000c2d0: 2020 2020 2020 2020 2020 2076 6973 6974             visit
+0000c2e0: 5f66 726f 6d3d 7669 7369 745f 6672 6f6d  _from=visit_from
+0000c2f0: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+0000c300: 2020 7669 7369 745f 746f 3d76 6973 6974    visit_to=visit
+0000c310: 5f74 6f2c 0a20 2020 2020 2020 2020 2020  _to,.           
+0000c320: 2020 2020 2063 7572 3d63 7572 2c0a 2020       cur=cur,.  
+0000c330: 2020 2020 2020 2020 2020 293a 0a20 2020            ):.   
+0000c340: 2020 2020 2020 2020 2020 2020 2072 6f77               row
+0000c350: 5f64 203d 2064 6963 7428 7a69 7028 6462  _d = dict(zip(db
+0000c360: 2e6f 7269 6769 6e5f 7669 7369 745f 7374  .origin_visit_st
+0000c370: 6174 7573 5f63 6f6c 732c 2072 6f77 2929  atus_cols, row))
+0000c380: 0a0a 2020 2020 2020 2020 2020 2020 2020  ..              
+0000c390: 2020 7669 7369 745f 7374 6174 7573 6573    visit_statuses
+0000c3a0: 5b72 6f77 5f64 5b22 7669 7369 7422 5d5d  [row_d["visit"]]
+0000c3b0: 2e61 7070 656e 6428 4f72 6967 696e 5669  .append(OriginVi
+0000c3c0: 7369 7453 7461 7475 7328 2a2a 726f 775f  sitStatus(**row_
+0000c3d0: 6429 290a 0a20 2020 2020 2020 2072 6573  d))..        res
+0000c3e0: 756c 7473 203d 205b 0a20 2020 2020 2020  ults = [.       
+0000c3f0: 2020 2020 204f 7269 6769 6e56 6973 6974       OriginVisit
+0000c400: 5769 7468 5374 6174 7573 6573 2876 6973  WithStatuses(vis
+0000c410: 6974 3d76 6973 6974 2c20 7374 6174 7573  it=visit, status
+0000c420: 6573 3d76 6973 6974 5f73 7461 7475 7365  es=visit_statuse
+0000c430: 735b 7669 7369 742e 7669 7369 745d 290a  s[visit.visit]).
+0000c440: 2020 2020 2020 2020 2020 2020 666f 7220              for 
+0000c450: 7669 7369 7420 696e 2076 6973 6974 730a  visit in visits.
+0000c460: 2020 2020 2020 2020 5d0a 0a20 2020 2020          ]..     
+0000c470: 2020 2072 6574 7572 6e20 5061 6765 6452     return PagedR
+0000c480: 6573 756c 7428 7265 7375 6c74 733d 7265  esult(results=re
+0000c490: 7375 6c74 732c 206e 6578 745f 7061 6765  sults, next_page
+0000c4a0: 5f74 6f6b 656e 3d6e 6578 745f 7061 6765  _token=next_page
+0000c4b0: 5f74 6f6b 656e 290a 0a20 2020 2040 6462  _token)..    @db
+0000c4c0: 5f74 7261 6e73 6163 7469 6f6e 2873 7461  _transaction(sta
+0000c4d0: 7465 6d65 6e74 5f74 696d 656f 7574 3d32  tement_timeout=2
+0000c4e0: 3030 3029 0a20 2020 2064 6566 206f 7269  000).    def ori
+0000c4f0: 6769 6e5f 7669 7369 745f 6669 6e64 5f62  gin_visit_find_b
+0000c500: 795f 6461 7465 280a 2020 2020 2020 2020  y_date(.        
+0000c510: 7365 6c66 2c0a 2020 2020 2020 2020 6f72  self,.        or
+0000c520: 6967 696e 3a20 7374 722c 0a20 2020 2020  igin: str,.     
+0000c530: 2020 2076 6973 6974 5f64 6174 653a 2064     visit_date: d
+0000c540: 6174 6574 696d 652e 6461 7465 7469 6d65  atetime.datetime
+0000c550: 2c0a 2020 2020 2020 2020 7479 7065 3a20  ,.        type: 
+0000c560: 4f70 7469 6f6e 616c 5b73 7472 5d20 3d20  Optional[str] = 
+0000c570: 4e6f 6e65 2c0a 2020 2020 2020 2020 2a2c  None,.        *,
+0000c580: 0a20 2020 2020 2020 2064 623a 2044 622c  .        db: Db,
+0000c590: 0a20 2020 2020 2020 2063 7572 3d4e 6f6e  .        cur=Non
+0000c5a0: 652c 0a20 2020 2029 202d 3e20 4f70 7469  e,.    ) -> Opti
+0000c5b0: 6f6e 616c 5b4f 7269 6769 6e56 6973 6974  onal[OriginVisit
+0000c5c0: 5d3a 0a20 2020 2020 2020 2072 6f77 5f64  ]:.        row_d
+0000c5d0: 203d 2064 622e 6f72 6967 696e 5f76 6973   = db.origin_vis
+0000c5e0: 6974 5f66 696e 645f 6279 5f64 6174 6528  it_find_by_date(
+0000c5f0: 6f72 6967 696e 2c20 7669 7369 745f 6461  origin, visit_da
+0000c600: 7465 2c20 7479 7065 3d74 7970 652c 2063  te, type=type, c
+0000c610: 7572 3d63 7572 290a 2020 2020 2020 2020  ur=cur).        
+0000c620: 6966 206e 6f74 2072 6f77 5f64 3a0a 2020  if not row_d:.  
+0000c630: 2020 2020 2020 2020 2020 7265 7475 726e            return
+0000c640: 204e 6f6e 650a 2020 2020 2020 2020 7265   None.        re
+0000c650: 7475 726e 204f 7269 6769 6e56 6973 6974  turn OriginVisit
+0000c660: 280a 2020 2020 2020 2020 2020 2020 6f72  (.            or
+0000c670: 6967 696e 3d72 6f77 5f64 5b22 6f72 6967  igin=row_d["orig
+0000c680: 696e 225d 2c0a 2020 2020 2020 2020 2020  in"],.          
+0000c690: 2020 7669 7369 743d 726f 775f 645b 2276    visit=row_d["v
+0000c6a0: 6973 6974 225d 2c0a 2020 2020 2020 2020  isit"],.        
+0000c6b0: 2020 2020 6461 7465 3d72 6f77 5f64 5b22      date=row_d["
+0000c6c0: 6461 7465 225d 2c0a 2020 2020 2020 2020  date"],.        
+0000c6d0: 2020 2020 7479 7065 3d72 6f77 5f64 5b22      type=row_d["
+0000c6e0: 7479 7065 225d 2c0a 2020 2020 2020 2020  type"],.        
+0000c6f0: 290a 0a20 2020 2040 6462 5f74 7261 6e73  )..    @db_trans
+0000c700: 6163 7469 6f6e 2873 7461 7465 6d65 6e74  action(statement
+0000c710: 5f74 696d 656f 7574 3d35 3030 290a 2020  _timeout=500).  
+0000c720: 2020 6465 6620 6f72 6967 696e 5f76 6973    def origin_vis
+0000c730: 6974 5f67 6574 5f62 7928 0a20 2020 2020  it_get_by(.     
+0000c740: 2020 2073 656c 662c 206f 7269 6769 6e3a     self, origin:
+0000c750: 2073 7472 2c20 7669 7369 743a 2069 6e74   str, visit: int
+0000c760: 2c20 2a2c 2064 623a 2044 622c 2063 7572  , *, db: Db, cur
+0000c770: 3d4e 6f6e 650a 2020 2020 2920 2d3e 204f  =None.    ) -> O
+0000c780: 7074 696f 6e61 6c5b 4f72 6967 696e 5669  ptional[OriginVi
+0000c790: 7369 745d 3a0a 2020 2020 2020 2020 726f  sit]:.        ro
+0000c7a0: 7720 3d20 6462 2e6f 7269 6769 6e5f 7669  w = db.origin_vi
+0000c7b0: 7369 745f 6765 7428 6f72 6967 696e 2c20  sit_get(origin, 
+0000c7c0: 7669 7369 742c 2063 7572 290a 2020 2020  visit, cur).    
+0000c7d0: 2020 2020 6966 2072 6f77 3a0a 2020 2020      if row:.    
+0000c7e0: 2020 2020 2020 2020 726f 775f 6420 3d20          row_d = 
+0000c7f0: 6469 6374 287a 6970 2864 622e 6f72 6967  dict(zip(db.orig
+0000c800: 696e 5f76 6973 6974 5f67 6574 5f63 6f6c  in_visit_get_col
+0000c810: 732c 2072 6f77 2929 0a20 2020 2020 2020  s, row)).       
+0000c820: 2020 2020 2072 6574 7572 6e20 4f72 6967       return Orig
+0000c830: 696e 5669 7369 7428 0a20 2020 2020 2020  inVisit(.       
+0000c840: 2020 2020 2020 2020 206f 7269 6769 6e3d           origin=
+0000c850: 726f 775f 645b 226f 7269 6769 6e22 5d2c  row_d["origin"],
+0000c860: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000c870: 2076 6973 6974 3d72 6f77 5f64 5b22 7669   visit=row_d["vi
+0000c880: 7369 7422 5d2c 0a20 2020 2020 2020 2020  sit"],.         
+0000c890: 2020 2020 2020 2064 6174 653d 726f 775f         date=row_
+0000c8a0: 645b 2264 6174 6522 5d2c 0a20 2020 2020  d["date"],.     
+0000c8b0: 2020 2020 2020 2020 2020 2074 7970 653d             type=
+0000c8c0: 726f 775f 645b 2274 7970 6522 5d2c 0a20  row_d["type"],. 
+0000c8d0: 2020 2020 2020 2020 2020 2029 0a20 2020             ).   
+0000c8e0: 2020 2020 2072 6574 7572 6e20 4e6f 6e65       return None
+0000c8f0: 0a0a 2020 2020 4064 625f 7472 616e 7361  ..    @db_transa
+0000c900: 6374 696f 6e28 7374 6174 656d 656e 745f  ction(statement_
+0000c910: 7469 6d65 6f75 743d 3430 3030 290a 2020  timeout=4000).  
+0000c920: 2020 6465 6620 6f72 6967 696e 5f76 6973    def origin_vis
+0000c930: 6974 5f67 6574 5f6c 6174 6573 7428 0a20  it_get_latest(. 
+0000c940: 2020 2020 2020 2073 656c 662c 0a20 2020         self,.   
+0000c950: 2020 2020 206f 7269 6769 6e3a 2073 7472       origin: str
+0000c960: 2c0a 2020 2020 2020 2020 7479 7065 3a20  ,.        type: 
+0000c970: 4f70 7469 6f6e 616c 5b73 7472 5d20 3d20  Optional[str] = 
+0000c980: 4e6f 6e65 2c0a 2020 2020 2020 2020 616c  None,.        al
+0000c990: 6c6f 7765 645f 7374 6174 7573 6573 3a20  lowed_statuses: 
+0000c9a0: 4f70 7469 6f6e 616c 5b4c 6973 745b 7374  Optional[List[st
+0000c9b0: 725d 5d20 3d20 4e6f 6e65 2c0a 2020 2020  r]] = None,.    
+0000c9c0: 2020 2020 7265 7175 6972 655f 736e 6170      require_snap
+0000c9d0: 7368 6f74 3a20 626f 6f6c 203d 2046 616c  shot: bool = Fal
+0000c9e0: 7365 2c0a 2020 2020 2020 2020 2a2c 0a20  se,.        *,. 
+0000c9f0: 2020 2020 2020 2064 623a 2044 622c 0a20         db: Db,. 
+0000ca00: 2020 2020 2020 2063 7572 3d4e 6f6e 652c         cur=None,
+0000ca10: 0a20 2020 2029 202d 3e20 4f70 7469 6f6e  .    ) -> Option
+0000ca20: 616c 5b4f 7269 6769 6e56 6973 6974 5d3a  al[OriginVisit]:
+0000ca30: 0a20 2020 2020 2020 2069 6620 616c 6c6f  .        if allo
+0000ca40: 7765 645f 7374 6174 7573 6573 2061 6e64  wed_statuses and
+0000ca50: 206e 6f74 2073 6574 2861 6c6c 6f77 6564   not set(allowed
+0000ca60: 5f73 7461 7475 7365 7329 2e69 6e74 6572  _statuses).inter
+0000ca70: 7365 6374 696f 6e28 5649 5349 545f 5354  section(VISIT_ST
+0000ca80: 4154 5553 4553 293a 0a20 2020 2020 2020  ATUSES):.       
+0000ca90: 2020 2020 2072 6169 7365 2053 746f 7261       raise Stora
+0000caa0: 6765 4172 6775 6d65 6e74 4578 6365 7074  geArgumentExcept
+0000cab0: 696f 6e28 0a20 2020 2020 2020 2020 2020  ion(.           
+0000cac0: 2020 2020 2066 2255 6e6b 6e6f 776e 2061       f"Unknown a
+0000cad0: 6c6c 6f77 6564 2073 7461 7475 7365 7320  llowed statuses 
+0000cae0: 7b27 2c27 2e6a 6f69 6e28 616c 6c6f 7765  {','.join(allowe
+0000caf0: 645f 7374 6174 7573 6573 297d 2c20 6f6e  d_statuses)}, on
+0000cb00: 6c79 2022 0a20 2020 2020 2020 2020 2020  ly ".           
+0000cb10: 2020 2020 2066 227b 272c 272e 6a6f 696e       f"{','.join
+0000cb20: 2856 4953 4954 5f53 5441 5455 5345 5329  (VISIT_STATUSES)
+0000cb30: 7d20 6175 7468 6f72 697a 6564 220a 2020  } authorized".  
+0000cb40: 2020 2020 2020 2020 2020 290a 0a20 2020            )..   
+0000cb50: 2020 2020 2072 6f77 203d 2064 622e 6f72       row = db.or
+0000cb60: 6967 696e 5f76 6973 6974 5f67 6574 5f6c  igin_visit_get_l
+0000cb70: 6174 6573 7428 0a20 2020 2020 2020 2020  atest(.         
+0000cb80: 2020 206f 7269 6769 6e2c 0a20 2020 2020     origin,.     
+0000cb90: 2020 2020 2020 2074 7970 653d 7479 7065         type=type
+0000cba0: 2c0a 2020 2020 2020 2020 2020 2020 616c  ,.            al
+0000cbb0: 6c6f 7765 645f 7374 6174 7573 6573 3d61  lowed_statuses=a
+0000cbc0: 6c6c 6f77 6564 5f73 7461 7475 7365 732c  llowed_statuses,
+0000cbd0: 0a20 2020 2020 2020 2020 2020 2072 6571  .            req
+0000cbe0: 7569 7265 5f73 6e61 7073 686f 743d 7265  uire_snapshot=re
+0000cbf0: 7175 6972 655f 736e 6170 7368 6f74 2c0a  quire_snapshot,.
+0000cc00: 2020 2020 2020 2020 2020 2020 6375 723d              cur=
+0000cc10: 6375 722c 0a20 2020 2020 2020 2029 0a20  cur,.        ). 
+0000cc20: 2020 2020 2020 2069 6620 726f 773a 0a20         if row:. 
+0000cc30: 2020 2020 2020 2020 2020 2072 6f77 5f64             row_d
+0000cc40: 203d 2064 6963 7428 7a69 7028 6462 2e6f   = dict(zip(db.o
+0000cc50: 7269 6769 6e5f 7669 7369 745f 6765 745f  rigin_visit_get_
+0000cc60: 636f 6c73 2c20 726f 7729 290a 2020 2020  cols, row)).    
+0000cc70: 2020 2020 2020 2020 6173 7365 7274 2028          assert (
+0000cc80: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000cc90: 2072 6f77 5f64 5b22 7669 7369 7422 5d20   row_d["visit"] 
+0000cca0: 6973 206e 6f74 204e 6f6e 650a 2020 2020  is not None.    
+0000ccb0: 2020 2020 2020 2020 292c 2022 6f72 6967          ), "orig
+0000ccc0: 696e 5f76 6973 6974 5f73 7461 7475 7320  in_visit_status 
+0000ccd0: 4c45 4654 204a 4f49 4e20 6f72 6967 696e  LEFT JOIN origin
+0000cce0: 5f76 6973 6974 2072 6574 7572 6e65 6420  _visit returned 
+0000ccf0: 4e55 4c4c 220a 2020 2020 2020 2020 2020  NULL".          
+0000cd00: 2020 7669 7369 7420 3d20 4f72 6967 696e    visit = Origin
+0000cd10: 5669 7369 7428 0a20 2020 2020 2020 2020  Visit(.         
+0000cd20: 2020 2020 2020 206f 7269 6769 6e3d 726f         origin=ro
+0000cd30: 775f 645b 226f 7269 6769 6e22 5d2c 0a20  w_d["origin"],. 
+0000cd40: 2020 2020 2020 2020 2020 2020 2020 2076                 v
+0000cd50: 6973 6974 3d72 6f77 5f64 5b22 7669 7369  isit=row_d["visi
+0000cd60: 7422 5d2c 0a20 2020 2020 2020 2020 2020  t"],.           
+0000cd70: 2020 2020 2064 6174 653d 726f 775f 645b       date=row_d[
+0000cd80: 2264 6174 6522 5d2c 0a20 2020 2020 2020  "date"],.       
+0000cd90: 2020 2020 2020 2020 2074 7970 653d 726f           type=ro
+0000cda0: 775f 645b 2274 7970 6522 5d2c 0a20 2020  w_d["type"],.   
+0000cdb0: 2020 2020 2020 2020 2029 0a20 2020 2020           ).     
+0000cdc0: 2020 2020 2020 2072 6574 7572 6e20 7669         return vi
+0000cdd0: 7369 740a 2020 2020 2020 2020 7265 7475  sit.        retu
+0000cde0: 726e 204e 6f6e 650a 0a20 2020 2040 6462  rn None..    @db
+0000cdf0: 5f74 7261 6e73 6163 7469 6f6e 2873 7461  _transaction(sta
+0000ce00: 7465 6d65 6e74 5f74 696d 656f 7574 3d35  tement_timeout=5
+0000ce10: 3030 290a 2020 2020 6465 6620 6f72 6967  00).    def orig
+0000ce20: 696e 5f76 6973 6974 5f73 7461 7475 735f  in_visit_status_
+0000ce30: 6765 7428 0a20 2020 2020 2020 2073 656c  get(.        sel
+0000ce40: 662c 0a20 2020 2020 2020 206f 7269 6769  f,.        origi
+0000ce50: 6e3a 2073 7472 2c0a 2020 2020 2020 2020  n: str,.        
+0000ce60: 7669 7369 743a 2069 6e74 2c0a 2020 2020  visit: int,.    
+0000ce70: 2020 2020 7061 6765 5f74 6f6b 656e 3a20      page_token: 
+0000ce80: 4f70 7469 6f6e 616c 5b73 7472 5d20 3d20  Optional[str] = 
+0000ce90: 4e6f 6e65 2c0a 2020 2020 2020 2020 6f72  None,.        or
+0000cea0: 6465 723a 204c 6973 744f 7264 6572 203d  der: ListOrder =
+0000ceb0: 204c 6973 744f 7264 6572 2e41 5343 2c0a   ListOrder.ASC,.
+0000cec0: 2020 2020 2020 2020 6c69 6d69 743a 2069          limit: i
+0000ced0: 6e74 203d 2031 302c 0a20 2020 2020 2020  nt = 10,.       
+0000cee0: 202a 2c0a 2020 2020 2020 2020 6462 3a20   *,.        db: 
+0000cef0: 4462 2c0a 2020 2020 2020 2020 6375 723d  Db,.        cur=
+0000cf00: 4e6f 6e65 2c0a 2020 2020 2920 2d3e 2050  None,.    ) -> P
+0000cf10: 6167 6564 5265 7375 6c74 5b4f 7269 6769  agedResult[Origi
+0000cf20: 6e56 6973 6974 5374 6174 7573 5d3a 0a20  nVisitStatus]:. 
+0000cf30: 2020 2020 2020 206e 6578 745f 7061 6765         next_page
+0000cf40: 5f74 6f6b 656e 203d 204e 6f6e 650a 2020  _token = None.  
+0000cf50: 2020 2020 2020 6461 7465 5f66 726f 6d20        date_from 
+0000cf60: 3d20 4e6f 6e65 0a20 2020 2020 2020 2069  = None.        i
+0000cf70: 6620 7061 6765 5f74 6f6b 656e 2069 7320  f page_token is 
+0000cf80: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
+0000cf90: 2020 2020 2020 7472 793a 0a20 2020 2020        try:.     
+0000cfa0: 2020 2020 2020 2020 2020 2064 6174 655f             date_
+0000cfb0: 6672 6f6d 203d 2064 6174 6574 696d 652e  from = datetime.
+0000cfc0: 6461 7465 7469 6d65 2e66 726f 6d69 736f  datetime.fromiso
+0000cfd0: 666f 726d 6174 2870 6167 655f 746f 6b65  format(page_toke
+0000cfe0: 6e29 0a20 2020 2020 2020 2020 2020 2065  n).            e
+0000cff0: 7863 6570 7420 5661 6c75 6545 7272 6f72  xcept ValueError
+0000d000: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+0000d010: 2020 7261 6973 6520 5374 6f72 6167 6541    raise StorageA
+0000d020: 7267 756d 656e 7445 7863 6570 7469 6f6e  rgumentException
+0000d030: 280a 2020 2020 2020 2020 2020 2020 2020  (.              
+0000d040: 2020 2020 2020 2249 6e76 616c 6964 2070        "Invalid p
+0000d050: 6167 655f 746f 6b65 6e20 6172 6775 6d65  age_token argume
+0000d060: 6e74 2074 6f20 6f72 6967 696e 5f76 6973  nt to origin_vis
+0000d070: 6974 5f73 7461 7475 735f 6765 742e 220a  it_status_get.".
+0000d080: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d090: 2920 6672 6f6d 204e 6f6e 650a 0a20 2020  ) from None..   
+0000d0a0: 2020 2020 2076 6973 6974 5f73 7461 7475       visit_statu
+0000d0b0: 7365 733a 204c 6973 745b 4f72 6967 696e  ses: List[Origin
+0000d0c0: 5669 7369 7453 7461 7475 735d 203d 205b  VisitStatus] = [
+0000d0d0: 5d0a 2020 2020 2020 2020 2320 5461 6b65  ].        # Take
+0000d0e0: 206f 6e65 206d 6f72 6520 7669 7369 7420   one more visit 
+0000d0f0: 7374 6174 7573 2073 6f20 7765 2063 616e  status so we can
+0000d100: 2072 6575 7365 2069 7420 6173 2074 6865   reuse it as the
+0000d110: 206e 6578 7420 7061 6765 2074 6f6b 656e   next page token
+0000d120: 2069 6620 616e 790a 2020 2020 2020 2020   if any.        
+0000d130: 666f 7220 726f 7720 696e 2064 622e 6f72  for row in db.or
+0000d140: 6967 696e 5f76 6973 6974 5f73 7461 7475  igin_visit_statu
+0000d150: 735f 6765 745f 7261 6e67 6528 0a20 2020  s_get_range(.   
+0000d160: 2020 2020 2020 2020 206f 7269 6769 6e2c           origin,
+0000d170: 0a20 2020 2020 2020 2020 2020 2076 6973  .            vis
+0000d180: 6974 2c0a 2020 2020 2020 2020 2020 2020  it,.            
+0000d190: 6461 7465 5f66 726f 6d3d 6461 7465 5f66  date_from=date_f
+0000d1a0: 726f 6d2c 0a20 2020 2020 2020 2020 2020  rom,.           
+0000d1b0: 206f 7264 6572 3d6f 7264 6572 2c0a 2020   order=order,.  
+0000d1c0: 2020 2020 2020 2020 2020 6c69 6d69 743d            limit=
+0000d1d0: 6c69 6d69 7420 2b20 312c 0a20 2020 2020  limit + 1,.     
+0000d1e0: 2020 2020 2020 2063 7572 3d63 7572 2c0a         cur=cur,.
+0000d1f0: 2020 2020 2020 2020 293a 0a20 2020 2020          ):.     
+0000d200: 2020 2020 2020 2072 6f77 5f64 203d 2064         row_d = d
+0000d210: 6963 7428 7a69 7028 6462 2e6f 7269 6769  ict(zip(db.origi
+0000d220: 6e5f 7669 7369 745f 7374 6174 7573 5f63  n_visit_status_c
+0000d230: 6f6c 732c 2072 6f77 2929 0a20 2020 2020  ols, row)).     
+0000d240: 2020 2020 2020 2076 6973 6974 5f73 7461         visit_sta
+0000d250: 7475 7365 732e 6170 7065 6e64 284f 7269  tuses.append(Ori
+0000d260: 6769 6e56 6973 6974 5374 6174 7573 282a  ginVisitStatus(*
+0000d270: 2a72 6f77 5f64 2929 0a0a 2020 2020 2020  *row_d))..      
+0000d280: 2020 6966 206c 656e 2876 6973 6974 5f73    if len(visit_s
+0000d290: 7461 7475 7365 7329 203e 206c 696d 6974  tatuses) > limit
+0000d2a0: 3a0a 2020 2020 2020 2020 2020 2020 2320  :.            # 
+0000d2b0: 6c61 7374 2076 6973 6974 2073 7461 7475  last visit statu
+0000d2c0: 7320 6461 7465 2069 7320 7468 6520 6e65  s date is the ne
+0000d2d0: 7874 2070 6167 6520 746f 6b65 6e0a 2020  xt page token.  
+0000d2e0: 2020 2020 2020 2020 2020 6e65 7874 5f70            next_p
+0000d2f0: 6167 655f 746f 6b65 6e20 3d20 7374 7228  age_token = str(
+0000d300: 7669 7369 745f 7374 6174 7573 6573 5b2d  visit_statuses[-
+0000d310: 315d 2e64 6174 6529 0a20 2020 2020 2020  1].date).       
+0000d320: 2020 2020 2023 2065 7863 6c75 6469 6e67       # excluding
+0000d330: 2074 6861 7420 7669 7369 7420 7374 6174   that visit stat
+0000d340: 7573 2066 726f 6d20 7468 6520 7265 7375  us from the resu
+0000d350: 6c74 2074 6f20 7265 7370 6563 7420 7468  lt to respect th
+0000d360: 6520 6c69 6d69 7420 7369 7a65 0a20 2020  e limit size.   
+0000d370: 2020 2020 2020 2020 2076 6973 6974 5f73           visit_s
+0000d380: 7461 7475 7365 7320 3d20 7669 7369 745f  tatuses = visit_
+0000d390: 7374 6174 7573 6573 5b3a 6c69 6d69 745d  statuses[:limit]
+0000d3a0: 0a0a 2020 2020 2020 2020 7265 7475 726e  ..        return
+0000d3b0: 2050 6167 6564 5265 7375 6c74 2872 6573   PagedResult(res
+0000d3c0: 756c 7473 3d76 6973 6974 5f73 7461 7475  ults=visit_statu
+0000d3d0: 7365 732c 206e 6578 745f 7061 6765 5f74  ses, next_page_t
+0000d3e0: 6f6b 656e 3d6e 6578 745f 7061 6765 5f74  oken=next_page_t
+0000d3f0: 6f6b 656e 290a 0a20 2020 2040 6462 5f74  oken)..    @db_t
+0000d400: 7261 6e73 6163 7469 6f6e 2829 0a20 2020  ransaction().   
+0000d410: 2064 6566 206f 7269 6769 6e5f 7669 7369   def origin_visi
+0000d420: 745f 7374 6174 7573 5f67 6574 5f72 616e  t_status_get_ran
+0000d430: 646f 6d28 0a20 2020 2020 2020 2073 656c  dom(.        sel
+0000d440: 662c 2074 7970 653a 2073 7472 2c20 2a2c  f, type: str, *,
+0000d450: 2064 623a 2044 622c 2063 7572 3d4e 6f6e   db: Db, cur=Non
+0000d460: 650a 2020 2020 2920 2d3e 204f 7074 696f  e.    ) -> Optio
+0000d470: 6e61 6c5b 4f72 6967 696e 5669 7369 7453  nal[OriginVisitS
+0000d480: 7461 7475 735d 3a0a 2020 2020 2020 2020  tatus]:.        
+0000d490: 726f 7720 3d20 6462 2e6f 7269 6769 6e5f  row = db.origin_
+0000d4a0: 7669 7369 745f 6765 745f 7261 6e64 6f6d  visit_get_random
+0000d4b0: 2874 7970 652c 2063 7572 290a 2020 2020  (type, cur).    
+0000d4c0: 2020 2020 6966 2072 6f77 2069 7320 6e6f      if row is no
+0000d4d0: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
+0000d4e0: 2020 2020 726f 775f 6420 3d20 6469 6374      row_d = dict
+0000d4f0: 287a 6970 2864 622e 6f72 6967 696e 5f76  (zip(db.origin_v
+0000d500: 6973 6974 5f73 7461 7475 735f 636f 6c73  isit_status_cols
+0000d510: 2c20 726f 7729 290a 2020 2020 2020 2020  , row)).        
+0000d520: 2020 2020 7265 7475 726e 204f 7269 6769      return Origi
+0000d530: 6e56 6973 6974 5374 6174 7573 282a 2a72  nVisitStatus(**r
+0000d540: 6f77 5f64 290a 2020 2020 2020 2020 7265  ow_d).        re
+0000d550: 7475 726e 204e 6f6e 650a 0a20 2020 2023  turn None..    #
+0000d560: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+0000d570: 2323 2323 2323 2323 230a 2020 2020 2320  #########.    # 
+0000d580: 4f72 6967 696e 0a20 2020 2023 2323 2323  Origin.    #####
+0000d590: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+0000d5a0: 2323 2323 230a 0a20 2020 2040 6462 5f74  #####..    @db_t
+0000d5b0: 7261 6e73 6163 7469 6f6e 2873 7461 7465  ransaction(state
+0000d5c0: 6d65 6e74 5f74 696d 656f 7574 3d31 3030  ment_timeout=100
+0000d5d0: 3029 0a20 2020 2064 6566 206f 7269 6769  0).    def origi
+0000d5e0: 6e5f 6765 7428 0a20 2020 2020 2020 2073  n_get(.        s
+0000d5f0: 656c 662c 206f 7269 6769 6e73 3a20 4c69  elf, origins: Li
+0000d600: 7374 5b73 7472 5d2c 202a 2c20 6462 3a20  st[str], *, db: 
+0000d610: 4462 2c20 6375 723d 4e6f 6e65 0a20 2020  Db, cur=None.   
+0000d620: 2029 202d 3e20 4974 6572 6162 6c65 5b4f   ) -> Iterable[O
+0000d630: 7074 696f 6e61 6c5b 4f72 6967 696e 5d5d  ptional[Origin]]
+0000d640: 3a0a 2020 2020 2020 2020 726f 7773 203d  :.        rows =
+0000d650: 2064 622e 6f72 6967 696e 5f67 6574 5f62   db.origin_get_b
+0000d660: 795f 7572 6c28 6f72 6967 696e 732c 2063  y_url(origins, c
+0000d670: 7572 290a 2020 2020 2020 2020 7265 7375  ur).        resu
+0000d680: 6c74 3a20 4c69 7374 5b4f 7074 696f 6e61  lt: List[Optiona
+0000d690: 6c5b 4f72 6967 696e 5d5d 203d 205b 5d0a  l[Origin]] = [].
+0000d6a0: 2020 2020 2020 2020 666f 7220 726f 7720          for row 
+0000d6b0: 696e 2072 6f77 733a 0a20 2020 2020 2020  in rows:.       
+0000d6c0: 2020 2020 206f 7269 6769 6e5f 6420 3d20       origin_d = 
+0000d6d0: 6469 6374 287a 6970 2864 622e 6f72 6967  dict(zip(db.orig
+0000d6e0: 696e 5f63 6f6c 732c 2072 6f77 2929 0a20  in_cols, row)). 
+0000d6f0: 2020 2020 2020 2020 2020 2075 726c 203d             url =
+0000d700: 206f 7269 6769 6e5f 645b 2275 726c 225d   origin_d["url"]
+0000d710: 0a20 2020 2020 2020 2020 2020 2072 6573  .            res
+0000d720: 756c 742e 6170 7065 6e64 284e 6f6e 6520  ult.append(None 
+0000d730: 6966 2075 726c 2069 7320 4e6f 6e65 2065  if url is None e
+0000d740: 6c73 6520 4f72 6967 696e 2875 726c 3d75  lse Origin(url=u
+0000d750: 726c 2929 0a20 2020 2020 2020 2072 6574  rl)).        ret
+0000d760: 7572 6e20 7265 7375 6c74 0a0a 2020 2020  urn result..    
+0000d770: 4064 625f 7472 616e 7361 6374 696f 6e28  @db_transaction(
+0000d780: 7374 6174 656d 656e 745f 7469 6d65 6f75  statement_timeou
+0000d790: 743d 3130 3030 290a 2020 2020 6465 6620  t=1000).    def 
+0000d7a0: 6f72 6967 696e 5f67 6574 5f62 795f 7368  origin_get_by_sh
+0000d7b0: 6131 280a 2020 2020 2020 2020 7365 6c66  a1(.        self
+0000d7c0: 2c20 7368 6131 733a 204c 6973 745b 6279  , sha1s: List[by
+0000d7d0: 7465 735d 2c20 2a2c 2064 623a 2044 622c  tes], *, db: Db,
+0000d7e0: 2063 7572 3d4e 6f6e 650a 2020 2020 2920   cur=None.    ) 
+0000d7f0: 2d3e 204c 6973 745b 4f70 7469 6f6e 616c  -> List[Optional
+0000d800: 5b44 6963 745b 7374 722c 2041 6e79 5d5d  [Dict[str, Any]]
+0000d810: 5d3a 0a20 2020 2020 2020 2072 6574 7572  ]:.        retur
+0000d820: 6e20 5b0a 2020 2020 2020 2020 2020 2020  n [.            
+0000d830: 6469 6374 287a 6970 2864 622e 6f72 6967  dict(zip(db.orig
+0000d840: 696e 5f63 6f6c 732c 2072 6f77 2929 2069  in_cols, row)) i
+0000d850: 6620 726f 775b 305d 2065 6c73 6520 4e6f  f row[0] else No
+0000d860: 6e65 0a20 2020 2020 2020 2020 2020 2066  ne.            f
+0000d870: 6f72 2072 6f77 2069 6e20 6462 2e6f 7269  or row in db.ori
+0000d880: 6769 6e5f 6765 745f 6279 5f73 6861 3128  gin_get_by_sha1(
+0000d890: 7368 6131 732c 2063 7572 290a 2020 2020  sha1s, cur).    
+0000d8a0: 2020 2020 5d0a 0a20 2020 2040 6462 5f74      ]..    @db_t
+0000d8b0: 7261 6e73 6163 7469 6f6e 5f67 656e 6572  ransaction_gener
+0000d8c0: 6174 6f72 2829 0a20 2020 2064 6566 206f  ator().    def o
+0000d8d0: 7269 6769 6e5f 6765 745f 7261 6e67 6528  rigin_get_range(
+0000d8e0: 7365 6c66 2c20 6f72 6967 696e 5f66 726f  self, origin_fro
+0000d8f0: 6d3d 312c 206f 7269 6769 6e5f 636f 756e  m=1, origin_coun
+0000d900: 743d 3130 302c 202a 2c20 6462 3a20 4462  t=100, *, db: Db
+0000d910: 2c20 6375 723d 4e6f 6e65 293a 0a20 2020  , cur=None):.   
+0000d920: 2020 2020 2066 6f72 206f 7269 6769 6e20       for origin 
+0000d930: 696e 2064 622e 6f72 6967 696e 5f67 6574  in db.origin_get
+0000d940: 5f72 616e 6765 286f 7269 6769 6e5f 6672  _range(origin_fr
+0000d950: 6f6d 2c20 6f72 6967 696e 5f63 6f75 6e74  om, origin_count
+0000d960: 2c20 6375 7229 3a0a 2020 2020 2020 2020  , cur):.        
+0000d970: 2020 2020 7969 656c 6420 6469 6374 287a      yield dict(z
+0000d980: 6970 2864 622e 6f72 6967 696e 5f67 6574  ip(db.origin_get
+0000d990: 5f72 616e 6765 5f63 6f6c 732c 206f 7269  _range_cols, ori
+0000d9a0: 6769 6e29 290a 0a20 2020 2040 6462 5f74  gin))..    @db_t
+0000d9b0: 7261 6e73 6163 7469 6f6e 2829 0a20 2020  ransaction().   
+0000d9c0: 2064 6566 206f 7269 6769 6e5f 6c69 7374   def origin_list
+0000d9d0: 280a 2020 2020 2020 2020 7365 6c66 2c20  (.        self, 
+0000d9e0: 7061 6765 5f74 6f6b 656e 3a20 4f70 7469  page_token: Opti
+0000d9f0: 6f6e 616c 5b73 7472 5d20 3d20 4e6f 6e65  onal[str] = None
+0000da00: 2c20 6c69 6d69 743a 2069 6e74 203d 2031  , limit: int = 1
+0000da10: 3030 2c20 2a2c 2064 623a 2044 622c 2063  00, *, db: Db, c
+0000da20: 7572 3d4e 6f6e 650a 2020 2020 2920 2d3e  ur=None.    ) ->
+0000da30: 2050 6167 6564 5265 7375 6c74 5b4f 7269   PagedResult[Ori
+0000da40: 6769 6e5d 3a0a 2020 2020 2020 2020 7061  gin]:.        pa
+0000da50: 6765 5f74 6f6b 656e 203d 2070 6167 655f  ge_token = page_
+0000da60: 746f 6b65 6e20 6f72 2022 3022 0a20 2020  token or "0".   
+0000da70: 2020 2020 2069 6620 6e6f 7420 6973 696e       if not isin
+0000da80: 7374 616e 6365 2870 6167 655f 746f 6b65  stance(page_toke
+0000da90: 6e2c 2073 7472 293a 0a20 2020 2020 2020  n, str):.       
+0000daa0: 2020 2020 2072 6169 7365 2053 746f 7261       raise Stora
+0000dab0: 6765 4172 6775 6d65 6e74 4578 6365 7074  geArgumentExcept
+0000dac0: 696f 6e28 2270 6167 655f 746f 6b65 6e20  ion("page_token 
+0000dad0: 6d75 7374 2062 6520 6120 7374 7269 6e67  must be a string
+0000dae0: 2e22 290a 2020 2020 2020 2020 6f72 6967  .").        orig
+0000daf0: 696e 5f66 726f 6d20 3d20 696e 7428 7061  in_from = int(pa
+0000db00: 6765 5f74 6f6b 656e 290a 2020 2020 2020  ge_token).      
+0000db10: 2020 6e65 7874 5f70 6167 655f 746f 6b65    next_page_toke
+0000db20: 6e20 3d20 4e6f 6e65 0a0a 2020 2020 2020  n = None..      
+0000db30: 2020 6f72 6967 696e 733a 204c 6973 745b    origins: List[
+0000db40: 4f72 6967 696e 5d20 3d20 5b5d 0a20 2020  Origin] = [].   
+0000db50: 2020 2020 2023 2054 616b 6520 6f6e 6520       # Take one 
+0000db60: 6d6f 7265 206f 7269 6769 6e20 736f 2077  more origin so w
+0000db70: 6520 6361 6e20 7265 7573 6520 6974 2061  e can reuse it a
+0000db80: 7320 7468 6520 6e65 7874 2070 6167 6520  s the next page 
+0000db90: 746f 6b65 6e20 6966 2061 6e79 0a20 2020  token if any.   
+0000dba0: 2020 2020 2066 6f72 2072 6f77 5f64 2069       for row_d i
+0000dbb0: 6e20 7365 6c66 2e6f 7269 6769 6e5f 6765  n self.origin_ge
+0000dbc0: 745f 7261 6e67 6528 6f72 6967 696e 5f66  t_range(origin_f
+0000dbd0: 726f 6d2c 206c 696d 6974 202b 2031 2c20  rom, limit + 1, 
+0000dbe0: 6462 3d64 622c 2063 7572 3d63 7572 293a  db=db, cur=cur):
+0000dbf0: 0a20 2020 2020 2020 2020 2020 206f 7269  .            ori
+0000dc00: 6769 6e73 2e61 7070 656e 6428 4f72 6967  gins.append(Orig
+0000dc10: 696e 2875 726c 3d72 6f77 5f64 5b22 7572  in(url=row_d["ur
+0000dc20: 6c22 5d29 290a 2020 2020 2020 2020 2020  l"])).          
+0000dc30: 2020 2320 6b65 6570 2074 6865 206c 6173    # keep the las
+0000dc40: 745f 6964 2066 6f72 2074 6865 2070 6167  t_id for the pag
+0000dc50: 696e 6174 696f 6e20 6966 206e 6565 6465  ination if neede
+0000dc60: 640a 2020 2020 2020 2020 2020 2020 6c61  d.            la
+0000dc70: 7374 5f69 6420 3d20 726f 775f 645b 2269  st_id = row_d["i
+0000dc80: 6422 5d0a 0a20 2020 2020 2020 2069 6620  d"]..        if 
+0000dc90: 6c65 6e28 6f72 6967 696e 7329 203e 206c  len(origins) > l
+0000dca0: 696d 6974 3a20 2023 2064 6174 6120 6c65  imit:  # data le
+0000dcb0: 6674 2066 6f72 2073 7562 7365 7175 656e  ft for subsequen
+0000dcc0: 7420 6361 6c6c 0a20 2020 2020 2020 2020  t call.         
+0000dcd0: 2020 2023 206c 6173 7420 6f72 6967 696e     # last origin
+0000dce0: 2069 6420 6973 2074 6865 206e 6578 7420   id is the next 
+0000dcf0: 7061 6765 2074 6f6b 656e 0a20 2020 2020  page token.     
+0000dd00: 2020 2020 2020 206e 6578 745f 7061 6765         next_page
+0000dd10: 5f74 6f6b 656e 203d 2073 7472 286c 6173  _token = str(las
+0000dd20: 745f 6964 290a 2020 2020 2020 2020 2020  t_id).          
+0000dd30: 2020 2320 6578 636c 7564 696e 6720 7468    # excluding th
+0000dd40: 6174 206f 7269 6769 6e20 6672 6f6d 2074  at origin from t
+0000dd50: 6865 2072 6573 756c 7420 746f 2072 6573  he result to res
+0000dd60: 7065 6374 2074 6865 206c 696d 6974 2073  pect the limit s
+0000dd70: 697a 650a 2020 2020 2020 2020 2020 2020  ize.            
+0000dd80: 6f72 6967 696e 7320 3d20 6f72 6967 696e  origins = origin
+0000dd90: 735b 3a6c 696d 6974 5d0a 0a20 2020 2020  s[:limit]..     
+0000dda0: 2020 2061 7373 6572 7420 6c65 6e28 6f72     assert len(or
+0000ddb0: 6967 696e 7329 203c 3d20 6c69 6d69 740a  igins) <= limit.
+0000ddc0: 2020 2020 2020 2020 7265 7475 726e 2050          return P
+0000ddd0: 6167 6564 5265 7375 6c74 2872 6573 756c  agedResult(resul
+0000dde0: 7473 3d6f 7269 6769 6e73 2c20 6e65 7874  ts=origins, next
+0000ddf0: 5f70 6167 655f 746f 6b65 6e3d 6e65 7874  _page_token=next
+0000de00: 5f70 6167 655f 746f 6b65 6e29 0a0a 2020  _page_token)..  
+0000de10: 2020 4064 625f 7472 616e 7361 6374 696f    @db_transactio
+0000de20: 6e28 290a 2020 2020 6465 6620 6f72 6967  n().    def orig
+0000de30: 696e 5f73 6561 7263 6828 0a20 2020 2020  in_search(.     
+0000de40: 2020 2073 656c 662c 0a20 2020 2020 2020     self,.       
+0000de50: 2075 726c 5f70 6174 7465 726e 3a20 7374   url_pattern: st
+0000de60: 722c 0a20 2020 2020 2020 2070 6167 655f  r,.        page_
+0000de70: 746f 6b65 6e3a 204f 7074 696f 6e61 6c5b  token: Optional[
+0000de80: 7374 725d 203d 204e 6f6e 652c 0a20 2020  str] = None,.   
+0000de90: 2020 2020 206c 696d 6974 3a20 696e 7420       limit: int 
+0000dea0: 3d20 3530 2c0a 2020 2020 2020 2020 7265  = 50,.        re
+0000deb0: 6765 7870 3a20 626f 6f6c 203d 2046 616c  gexp: bool = Fal
+0000dec0: 7365 2c0a 2020 2020 2020 2020 7769 7468  se,.        with
+0000ded0: 5f76 6973 6974 3a20 626f 6f6c 203d 2046  _visit: bool = F
+0000dee0: 616c 7365 2c0a 2020 2020 2020 2020 7669  alse,.        vi
+0000def0: 7369 745f 7479 7065 733a 204f 7074 696f  sit_types: Optio
+0000df00: 6e61 6c5b 4c69 7374 5b73 7472 5d5d 203d  nal[List[str]] =
+0000df10: 204e 6f6e 652c 0a20 2020 2020 2020 202a   None,.        *
+0000df20: 2c0a 2020 2020 2020 2020 6462 3a20 4462  ,.        db: Db
+0000df30: 2c0a 2020 2020 2020 2020 6375 723d 4e6f  ,.        cur=No
+0000df40: 6e65 2c0a 2020 2020 2920 2d3e 2050 6167  ne,.    ) -> Pag
+0000df50: 6564 5265 7375 6c74 5b4f 7269 6769 6e5d  edResult[Origin]
+0000df60: 3a0a 2020 2020 2020 2020 6e65 7874 5f70  :.        next_p
+0000df70: 6167 655f 746f 6b65 6e20 3d20 4e6f 6e65  age_token = None
+0000df80: 0a20 2020 2020 2020 206f 6666 7365 7420  .        offset 
+0000df90: 3d20 696e 7428 7061 6765 5f74 6f6b 656e  = int(page_token
+0000dfa0: 2920 6966 2070 6167 655f 746f 6b65 6e20  ) if page_token 
+0000dfb0: 656c 7365 2030 0a0a 2020 2020 2020 2020  else 0..        
+0000dfc0: 6f72 6967 696e 7320 3d20 5b5d 0a20 2020  origins = [].   
+0000dfd0: 2020 2020 2023 2054 616b 6520 6f6e 6520       # Take one 
+0000dfe0: 6d6f 7265 206f 7269 6769 6e20 736f 2077  more origin so w
+0000dff0: 6520 6361 6e20 7265 7573 6520 6974 2061  e can reuse it a
+0000e000: 7320 7468 6520 6e65 7874 2070 6167 6520  s the next page 
+0000e010: 746f 6b65 6e20 6966 2061 6e79 0a20 2020  token if any.   
+0000e020: 2020 2020 2066 6f72 206f 7269 6769 6e20       for origin 
+0000e030: 696e 2064 622e 6f72 6967 696e 5f73 6561  in db.origin_sea
+0000e040: 7263 6828 0a20 2020 2020 2020 2020 2020  rch(.           
+0000e050: 2075 726c 5f70 6174 7465 726e 2c20 6f66   url_pattern, of
+0000e060: 6673 6574 2c20 6c69 6d69 7420 2b20 312c  fset, limit + 1,
+0000e070: 2072 6567 6578 702c 2077 6974 685f 7669   regexp, with_vi
+0000e080: 7369 742c 2076 6973 6974 5f74 7970 6573  sit, visit_types
+0000e090: 2c20 6375 720a 2020 2020 2020 2020 293a  , cur.        ):
+0000e0a0: 0a20 2020 2020 2020 2020 2020 2072 6f77  .            row
+0000e0b0: 5f64 203d 2064 6963 7428 7a69 7028 6462  _d = dict(zip(db
+0000e0c0: 2e6f 7269 6769 6e5f 636f 6c73 2c20 6f72  .origin_cols, or
+0000e0d0: 6967 696e 2929 0a20 2020 2020 2020 2020  igin)).         
+0000e0e0: 2020 206f 7269 6769 6e73 2e61 7070 656e     origins.appen
+0000e0f0: 6428 4f72 6967 696e 2875 726c 3d72 6f77  d(Origin(url=row
+0000e100: 5f64 5b22 7572 6c22 5d29 290a 0a20 2020  _d["url"]))..   
+0000e110: 2020 2020 2069 6620 6c65 6e28 6f72 6967       if len(orig
+0000e120: 696e 7329 203e 206c 696d 6974 3a0a 2020  ins) > limit:.  
+0000e130: 2020 2020 2020 2020 2020 2320 6e65 7874            # next
+0000e140: 206f 6666 7365 740a 2020 2020 2020 2020   offset.        
+0000e150: 2020 2020 6e65 7874 5f70 6167 655f 746f      next_page_to
+0000e160: 6b65 6e20 3d20 7374 7228 6f66 6673 6574  ken = str(offset
+0000e170: 202b 206c 696d 6974 290a 2020 2020 2020   + limit).      
+0000e180: 2020 2020 2020 2320 6578 636c 7564 696e        # excludin
+0000e190: 6720 7468 6174 206f 7269 6769 6e20 6672  g that origin fr
+0000e1a0: 6f6d 2074 6865 2072 6573 756c 7420 746f  om the result to
+0000e1b0: 2072 6573 7065 6374 2074 6865 206c 696d   respect the lim
+0000e1c0: 6974 2073 697a 650a 2020 2020 2020 2020  it size.        
+0000e1d0: 2020 2020 6f72 6967 696e 7320 3d20 6f72      origins = or
+0000e1e0: 6967 696e 735b 3a6c 696d 6974 5d0a 0a20  igins[:limit].. 
+0000e1f0: 2020 2020 2020 2061 7373 6572 7420 6c65         assert le
+0000e200: 6e28 6f72 6967 696e 7329 203c 3d20 6c69  n(origins) <= li
+0000e210: 6d69 740a 0a20 2020 2020 2020 2072 6574  mit..        ret
+0000e220: 7572 6e20 5061 6765 6452 6573 756c 7428  urn PagedResult(
+0000e230: 7265 7375 6c74 733d 6f72 6967 696e 732c  results=origins,
+0000e240: 206e 6578 745f 7061 6765 5f74 6f6b 656e   next_page_token
+0000e250: 3d6e 6578 745f 7061 6765 5f74 6f6b 656e  =next_page_token
+0000e260: 290a 0a20 2020 2040 6462 5f74 7261 6e73  )..    @db_trans
+0000e270: 6163 7469 6f6e 2829 0a20 2020 2064 6566  action().    def
+0000e280: 206f 7269 6769 6e5f 636f 756e 7428 0a20   origin_count(. 
+0000e290: 2020 2020 2020 2073 656c 662c 0a20 2020         self,.   
+0000e2a0: 2020 2020 2075 726c 5f70 6174 7465 726e       url_pattern
+0000e2b0: 3a20 7374 722c 0a20 2020 2020 2020 2072  : str,.        r
+0000e2c0: 6567 6578 703a 2062 6f6f 6c20 3d20 4661  egexp: bool = Fa
+0000e2d0: 6c73 652c 0a20 2020 2020 2020 2077 6974  lse,.        wit
+0000e2e0: 685f 7669 7369 743a 2062 6f6f 6c20 3d20  h_visit: bool = 
+0000e2f0: 4661 6c73 652c 0a20 2020 2020 2020 202a  False,.        *
+0000e300: 2c0a 2020 2020 2020 2020 6462 3a20 4462  ,.        db: Db
+0000e310: 2c0a 2020 2020 2020 2020 6375 723d 4e6f  ,.        cur=No
+0000e320: 6e65 2c0a 2020 2020 2920 2d3e 2069 6e74  ne,.    ) -> int
+0000e330: 3a0a 2020 2020 2020 2020 7265 7475 726e  :.        return
+0000e340: 2064 622e 6f72 6967 696e 5f63 6f75 6e74   db.origin_count
+0000e350: 2875 726c 5f70 6174 7465 726e 2c20 7265  (url_pattern, re
+0000e360: 6765 7870 2c20 7769 7468 5f76 6973 6974  gexp, with_visit
+0000e370: 2c20 6375 7229 0a0a 2020 2020 4064 625f  , cur)..    @db_
+0000e380: 7472 616e 7361 6374 696f 6e28 290a 2020  transaction().  
+0000e390: 2020 6465 6620 6f72 6967 696e 5f73 6e61    def origin_sna
+0000e3a0: 7073 686f 745f 6765 745f 616c 6c28 0a20  pshot_get_all(. 
+0000e3b0: 2020 2020 2020 2073 656c 662c 206f 7269         self, ori
+0000e3c0: 6769 6e5f 7572 6c3a 2073 7472 2c20 2a2c  gin_url: str, *,
+0000e3d0: 2064 623a 2044 622c 2063 7572 3d4e 6f6e   db: Db, cur=Non
+0000e3e0: 650a 2020 2020 2920 2d3e 204c 6973 745b  e.    ) -> List[
+0000e3f0: 5368 6131 4769 745d 3a0a 2020 2020 2020  Sha1Git]:.      
+0000e400: 2020 7265 7475 726e 206c 6973 7428 6462    return list(db
+0000e410: 2e6f 7269 6769 6e5f 736e 6170 7368 6f74  .origin_snapshot
+0000e420: 5f67 6574 5f61 6c6c 286f 7269 6769 6e5f  _get_all(origin_
+0000e430: 7572 6c2c 2063 7572 2929 0a0a 2020 2020  url, cur))..    
+0000e440: 4064 625f 7472 616e 7361 6374 696f 6e28  @db_transaction(
+0000e450: 290a 2020 2020 6465 6620 6f72 6967 696e  ).    def origin
+0000e460: 5f61 6464 2873 656c 662c 206f 7269 6769  _add(self, origi
+0000e470: 6e73 3a20 4c69 7374 5b4f 7269 6769 6e5d  ns: List[Origin]
+0000e480: 2c20 2a2c 2064 623a 2044 622c 2063 7572  , *, db: Db, cur
+0000e490: 3d4e 6f6e 6529 202d 3e20 4469 6374 5b73  =None) -> Dict[s
+0000e4a0: 7472 2c20 696e 745d 3a0a 2020 2020 2020  tr, int]:.      
+0000e4b0: 2020 7572 6c73 203d 205b 6f2e 7572 6c20    urls = [o.url 
+0000e4c0: 666f 7220 6f20 696e 206f 7269 6769 6e73  for o in origins
+0000e4d0: 5d0a 2020 2020 2020 2020 6b6e 6f77 6e5f  ].        known_
+0000e4e0: 6f72 6967 696e 7320 3d20 7365 7428 7572  origins = set(ur
+0000e4f0: 6c20 666f 7220 2875 726c 2c29 2069 6e20  l for (url,) in 
+0000e500: 6462 2e6f 7269 6769 6e5f 6765 745f 6279  db.origin_get_by
+0000e510: 5f75 726c 2875 726c 732c 2063 7572 2929  _url(urls, cur))
+0000e520: 0a20 2020 2020 2020 2023 206b 6565 7020  .        # keep 
+0000e530: 6f6e 6c79 206f 6e65 206f 6363 7572 7265  only one occurre
+0000e540: 6e63 6520 6f66 2065 6163 6820 6769 7665  nce of each give
+0000e550: 6e20 6f72 6967 696e 2077 6869 6c65 206b  n origin while k
+0000e560: 6565 7069 6e67 2074 6865 206c 6973 740a  eeping the list.
+0000e570: 2020 2020 2020 2020 2320 736f 7274 6564          # sorted
+0000e580: 2061 7320 6f72 6967 696e 616c 6c79 2067   as originally g
+0000e590: 6976 656e 0a20 2020 2020 2020 2074 6f5f  iven.        to_
+0000e5a0: 6164 6420 3d20 736f 7274 6564 2873 6574  add = sorted(set
+0000e5b0: 2875 726c 7329 202d 206b 6e6f 776e 5f6f  (urls) - known_o
+0000e5c0: 7269 6769 6e73 2c20 6b65 793d 7572 6c73  rigins, key=urls
+0000e5d0: 2e69 6e64 6578 290a 0a20 2020 2020 2020  .index)..       
+0000e5e0: 2073 656c 662e 6a6f 7572 6e61 6c5f 7772   self.journal_wr
+0000e5f0: 6974 6572 2e6f 7269 6769 6e5f 6164 6428  iter.origin_add(
+0000e600: 5b4f 7269 6769 6e28 7572 6c3d 7572 6c29  [Origin(url=url)
+0000e610: 2066 6f72 2075 726c 2069 6e20 746f 5f61   for url in to_a
+0000e620: 6464 5d29 0a20 2020 2020 2020 2061 6464  dd]).        add
+0000e630: 6564 203d 2030 0a20 2020 2020 2020 2066  ed = 0.        f
+0000e640: 6f72 2075 726c 2069 6e20 746f 5f61 6464  or url in to_add
+0000e650: 3a0a 2020 2020 2020 2020 2020 2020 6966  :.            if
+0000e660: 2064 622e 6f72 6967 696e 5f61 6464 2875   db.origin_add(u
+0000e670: 726c 2c20 6375 7229 3a0a 2020 2020 2020  rl, cur):.      
+0000e680: 2020 2020 2020 2020 2020 6164 6465 6420            added 
+0000e690: 2b3d 2031 0a20 2020 2020 2020 2072 6574  += 1.        ret
+0000e6a0: 7572 6e20 7b22 6f72 6967 696e 3a61 6464  urn {"origin:add
+0000e6b0: 223a 2061 6464 6564 7d0a 0a20 2020 2023  ": added}..    #
+0000e6c0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+0000e6d0: 2323 2323 2323 2323 230a 2020 2020 2320  #########.    # 
+0000e6e0: 6d69 7363 2e0a 2020 2020 2323 2323 2323  misc..    ######
+0000e6f0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+0000e700: 2323 2323 0a0a 2020 2020 4064 625f 7472  ####..    @db_tr
+0000e710: 616e 7361 6374 696f 6e28 7374 6174 656d  ansaction(statem
+0000e720: 656e 745f 7469 6d65 6f75 743d 3230 3030  ent_timeout=2000
+0000e730: 290a 2020 2020 6465 6620 6f62 6a65 6374  ).    def object
+0000e740: 5f66 696e 645f 6279 5f73 6861 315f 6769  _find_by_sha1_gi
+0000e750: 7428 0a20 2020 2020 2020 2073 656c 662c  t(.        self,
+0000e760: 2069 6473 3a20 4c69 7374 5b53 6861 3147   ids: List[Sha1G
+0000e770: 6974 5d2c 202a 2c20 6462 3a20 4462 2c20  it], *, db: Db, 
+0000e780: 6375 723d 4e6f 6e65 0a20 2020 2029 202d  cur=None.    ) -
+0000e790: 3e20 4469 6374 5b53 6861 3147 6974 2c20  > Dict[Sha1Git, 
+0000e7a0: 4c69 7374 5b44 6963 745d 5d3a 0a20 2020  List[Dict]]:.   
+0000e7b0: 2020 2020 2072 6574 3a20 4469 6374 5b53       ret: Dict[S
+0000e7c0: 6861 3147 6974 2c20 4c69 7374 5b44 6963  ha1Git, List[Dic
+0000e7d0: 745d 5d20 3d20 7b69 643a 205b 5d20 666f  t]] = {id: [] fo
+0000e7e0: 7220 6964 2069 6e20 6964 737d 0a0a 2020  r id in ids}..  
+0000e7f0: 2020 2020 2020 666f 7220 7265 7476 616c        for retval
+0000e800: 2069 6e20 6462 2e6f 626a 6563 745f 6669   in db.object_fi
+0000e810: 6e64 5f62 795f 7368 6131 5f67 6974 2869  nd_by_sha1_git(i
+0000e820: 6473 2c20 6375 723d 6375 7229 3a0a 2020  ds, cur=cur):.  
+0000e830: 2020 2020 2020 2020 2020 6966 2072 6574            if ret
+0000e840: 7661 6c5b 315d 3a0a 2020 2020 2020 2020  val[1]:.        
+0000e850: 2020 2020 2020 2020 7265 745b 7265 7476          ret[retv
+0000e860: 616c 5b30 5d5d 2e61 7070 656e 6428 0a20  al[0]].append(. 
+0000e870: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e880: 2020 2064 6963 7428 7a69 7028 6462 2e6f     dict(zip(db.o
+0000e890: 626a 6563 745f 6669 6e64 5f62 795f 7368  bject_find_by_sh
+0000e8a0: 6131 5f67 6974 5f63 6f6c 732c 2072 6574  a1_git_cols, ret
+0000e8b0: 7661 6c29 290a 2020 2020 2020 2020 2020  val)).          
+0000e8c0: 2020 2020 2020 290a 0a20 2020 2020 2020        )..       
+0000e8d0: 2072 6574 7572 6e20 7265 740a 0a20 2020   return ret..   
+0000e8e0: 2040 6462 5f74 7261 6e73 6163 7469 6f6e   @db_transaction
+0000e8f0: 2873 7461 7465 6d65 6e74 5f74 696d 656f  (statement_timeo
+0000e900: 7574 3d35 3030 290a 2020 2020 6465 6620  ut=500).    def 
+0000e910: 7374 6174 5f63 6f75 6e74 6572 7328 7365  stat_counters(se
+0000e920: 6c66 2c20 2a2c 2064 623a 2044 622c 2063  lf, *, db: Db, c
+0000e930: 7572 3d4e 6f6e 6529 3a0a 2020 2020 2020  ur=None):.      
+0000e940: 2020 7265 7475 726e 207b 6b3a 2076 2066    return {k: v f
+0000e950: 6f72 2028 6b2c 2076 2920 696e 2064 622e  or (k, v) in db.
+0000e960: 7374 6174 5f63 6f75 6e74 6572 7328 297d  stat_counters()}
+0000e970: 0a0a 2020 2020 4064 625f 7472 616e 7361  ..    @db_transa
+0000e980: 6374 696f 6e28 290a 2020 2020 6465 6620  ction().    def 
+0000e990: 7265 6672 6573 685f 7374 6174 5f63 6f75  refresh_stat_cou
+0000e9a0: 6e74 6572 7328 7365 6c66 2c20 2a2c 2064  nters(self, *, d
+0000e9b0: 623a 2044 622c 2063 7572 3d4e 6f6e 6529  b: Db, cur=None)
+0000e9c0: 3a0a 2020 2020 2020 2020 6b65 7973 203d  :.        keys =
+0000e9d0: 205b 0a20 2020 2020 2020 2020 2020 2022   [.            "
+0000e9e0: 636f 6e74 656e 7422 2c0a 2020 2020 2020  content",.      
+0000e9f0: 2020 2020 2020 2264 6972 6563 746f 7279        "directory
+0000ea00: 222c 0a20 2020 2020 2020 2020 2020 2022  ",.            "
+0000ea10: 6469 7265 6374 6f72 795f 656e 7472 795f  directory_entry_
+0000ea20: 6469 7222 2c0a 2020 2020 2020 2020 2020  dir",.          
+0000ea30: 2020 2264 6972 6563 746f 7279 5f65 6e74    "directory_ent
+0000ea40: 7279 5f66 696c 6522 2c0a 2020 2020 2020  ry_file",.      
+0000ea50: 2020 2020 2020 2264 6972 6563 746f 7279        "directory
+0000ea60: 5f65 6e74 7279 5f72 6576 222c 0a20 2020  _entry_rev",.   
+0000ea70: 2020 2020 2020 2020 2022 6f72 6967 696e           "origin
+0000ea80: 222c 0a20 2020 2020 2020 2020 2020 2022  ",.            "
+0000ea90: 6f72 6967 696e 5f76 6973 6974 222c 0a20  origin_visit",. 
+0000eaa0: 2020 2020 2020 2020 2020 2022 7065 7273             "pers
+0000eab0: 6f6e 222c 0a20 2020 2020 2020 2020 2020  on",.           
+0000eac0: 2022 7265 6c65 6173 6522 2c0a 2020 2020   "release",.    
+0000ead0: 2020 2020 2020 2020 2272 6576 6973 696f          "revisio
+0000eae0: 6e22 2c0a 2020 2020 2020 2020 2020 2020  n",.            
+0000eaf0: 2272 6576 6973 696f 6e5f 6869 7374 6f72  "revision_histor
+0000eb00: 7922 2c0a 2020 2020 2020 2020 2020 2020  y",.            
+0000eb10: 2273 6b69 7070 6564 5f63 6f6e 7465 6e74  "skipped_content
+0000eb20: 222c 0a20 2020 2020 2020 2020 2020 2022  ",.            "
+0000eb30: 736e 6170 7368 6f74 222c 0a20 2020 2020  snapshot",.     
+0000eb40: 2020 205d 0a0a 2020 2020 2020 2020 666f     ]..        fo
+0000eb50: 7220 6b65 7920 696e 206b 6579 733a 0a20  r key in keys:. 
+0000eb60: 2020 2020 2020 2020 2020 2063 7572 2e65             cur.e
+0000eb70: 7865 6375 7465 2822 7365 6c65 6374 202a  xecute("select *
+0000eb80: 2066 726f 6d20 7377 685f 7570 6461 7465   from swh_update
+0000eb90: 5f63 6f75 6e74 6572 2825 7329 222c 2028  _counter(%s)", (
+0000eba0: 6b65 792c 2929 0a0a 2020 2020 2323 2323  key,))..    ####
+0000ebb0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+0000ebc0: 2323 2323 2323 0a20 2020 2023 2052 6177  ######.    # Raw
+0000ebd0: 4578 7472 696e 7369 634d 6574 6164 6174  ExtrinsicMetadat
+0000ebe0: 610a 2020 2020 2323 2323 2323 2323 2323  a.    ##########
+0000ebf0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+0000ec00: 0a0a 2020 2020 4064 625f 7472 616e 7361  ..    @db_transa
+0000ec10: 6374 696f 6e28 290a 2020 2020 6465 6620  ction().    def 
+0000ec20: 7261 775f 6578 7472 696e 7369 635f 6d65  raw_extrinsic_me
+0000ec30: 7461 6461 7461 5f61 6464 280a 2020 2020  tadata_add(.    
+0000ec40: 2020 2020 7365 6c66 2c0a 2020 2020 2020      self,.      
+0000ec50: 2020 6d65 7461 6461 7461 3a20 4c69 7374    metadata: List
+0000ec60: 5b52 6177 4578 7472 696e 7369 634d 6574  [RawExtrinsicMet
+0000ec70: 6164 6174 615d 2c0a 2020 2020 2020 2020  adata],.        
+0000ec80: 6462 2c0a 2020 2020 2020 2020 6375 722c  db,.        cur,
+0000ec90: 0a20 2020 2029 202d 3e20 4469 6374 5b73  .    ) -> Dict[s
+0000eca0: 7472 2c20 696e 745d 3a0a 2020 2020 2020  tr, int]:.      
+0000ecb0: 2020 6d65 7461 6461 7461 203d 206c 6973    metadata = lis
+0000ecc0: 7428 6d65 7461 6461 7461 290a 2020 2020  t(metadata).    
+0000ecd0: 2020 2020 7365 6c66 2e6a 6f75 726e 616c      self.journal
+0000ece0: 5f77 7269 7465 722e 7261 775f 6578 7472  _writer.raw_extr
+0000ecf0: 696e 7369 635f 6d65 7461 6461 7461 5f61  insic_metadata_a
+0000ed00: 6464 286d 6574 6164 6174 6129 0a20 2020  dd(metadata).   
+0000ed10: 2020 2020 2063 6f75 6e74 6572 203d 2043       counter = C
+0000ed20: 6f75 6e74 6572 5b45 7874 656e 6465 644f  ounter[ExtendedO
+0000ed30: 626a 6563 7454 7970 655d 2829 0a20 2020  bjectType]().   
+0000ed40: 2020 2020 2066 6f72 206d 6574 6164 6174       for metadat
+0000ed50: 615f 656e 7472 7920 696e 206d 6574 6164  a_entry in metad
+0000ed60: 6174 613a 0a20 2020 2020 2020 2020 2020  ata:.           
+0000ed70: 2061 7574 686f 7269 7479 5f69 6420 3d20   authority_id = 
+0000ed80: 7365 6c66 2e5f 6765 745f 6175 7468 6f72  self._get_author
+0000ed90: 6974 795f 6964 286d 6574 6164 6174 615f  ity_id(metadata_
+0000eda0: 656e 7472 792e 6175 7468 6f72 6974 792c  entry.authority,
+0000edb0: 2064 622c 2063 7572 290a 2020 2020 2020   db, cur).      
+0000edc0: 2020 2020 2020 6665 7463 6865 725f 6964        fetcher_id
+0000edd0: 203d 2073 656c 662e 5f67 6574 5f66 6574   = self._get_fet
+0000ede0: 6368 6572 5f69 6428 6d65 7461 6461 7461  cher_id(metadata
+0000edf0: 5f65 6e74 7279 2e66 6574 6368 6572 2c20  _entry.fetcher, 
+0000ee00: 6462 2c20 6375 7229 0a0a 2020 2020 2020  db, cur)..      
+0000ee10: 2020 2020 2020 6462 2e72 6177 5f65 7874        db.raw_ext
+0000ee20: 7269 6e73 6963 5f6d 6574 6164 6174 615f  rinsic_metadata_
+0000ee30: 6164 6428 0a20 2020 2020 2020 2020 2020  add(.           
+0000ee40: 2020 2020 2069 643d 6d65 7461 6461 7461       id=metadata
+0000ee50: 5f65 6e74 7279 2e69 642c 0a20 2020 2020  _entry.id,.     
+0000ee60: 2020 2020 2020 2020 2020 2074 7970 653d             type=
+0000ee70: 6d65 7461 6461 7461 5f65 6e74 7279 2e74  metadata_entry.t
+0000ee80: 6172 6765 742e 6f62 6a65 6374 5f74 7970  arget.object_typ
+0000ee90: 652e 6e61 6d65 2e6c 6f77 6572 2829 2c0a  e.name.lower(),.
+0000eea0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000eeb0: 7461 7267 6574 3d73 7472 286d 6574 6164  target=str(metad
+0000eec0: 6174 615f 656e 7472 792e 7461 7267 6574  ata_entry.target
+0000eed0: 292c 0a20 2020 2020 2020 2020 2020 2020  ),.             
+0000eee0: 2020 2064 6973 636f 7665 7279 5f64 6174     discovery_dat
+0000eef0: 653d 6d65 7461 6461 7461 5f65 6e74 7279  e=metadata_entry
+0000ef00: 2e64 6973 636f 7665 7279 5f64 6174 652c  .discovery_date,
+0000ef10: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000ef20: 2061 7574 686f 7269 7479 5f69 643d 6175   authority_id=au
+0000ef30: 7468 6f72 6974 795f 6964 2c0a 2020 2020  thority_id,.    
+0000ef40: 2020 2020 2020 2020 2020 2020 6665 7463              fetc
+0000ef50: 6865 725f 6964 3d66 6574 6368 6572 5f69  her_id=fetcher_i
+0000ef60: 642c 0a20 2020 2020 2020 2020 2020 2020  d,.             
+0000ef70: 2020 2066 6f72 6d61 743d 6d65 7461 6461     format=metada
+0000ef80: 7461 5f65 6e74 7279 2e66 6f72 6d61 742c  ta_entry.format,
+0000ef90: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000efa0: 206d 6574 6164 6174 613d 6d65 7461 6461   metadata=metada
+0000efb0: 7461 5f65 6e74 7279 2e6d 6574 6164 6174  ta_entry.metadat
+0000efc0: 612c 0a20 2020 2020 2020 2020 2020 2020  a,.             
+0000efd0: 2020 206f 7269 6769 6e3d 6d65 7461 6461     origin=metada
+0000efe0: 7461 5f65 6e74 7279 2e6f 7269 6769 6e2c  ta_entry.origin,
+0000eff0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000f000: 2076 6973 6974 3d6d 6574 6164 6174 615f   visit=metadata_
+0000f010: 656e 7472 792e 7669 7369 742c 0a20 2020  entry.visit,.   
+0000f020: 2020 2020 2020 2020 2020 2020 2073 6e61               sna
+0000f030: 7073 686f 743d 6d61 705f 6f70 7469 6f6e  pshot=map_option
+0000f040: 616c 2873 7472 2c20 6d65 7461 6461 7461  al(str, metadata
+0000f050: 5f65 6e74 7279 2e73 6e61 7073 686f 7429  _entry.snapshot)
+0000f060: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+0000f070: 2020 7265 6c65 6173 653d 6d61 705f 6f70    release=map_op
+0000f080: 7469 6f6e 616c 2873 7472 2c20 6d65 7461  tional(str, meta
+0000f090: 6461 7461 5f65 6e74 7279 2e72 656c 6561  data_entry.relea
+0000f0a0: 7365 292c 0a20 2020 2020 2020 2020 2020  se),.           
+0000f0b0: 2020 2020 2072 6576 6973 696f 6e3d 6d61       revision=ma
+0000f0c0: 705f 6f70 7469 6f6e 616c 2873 7472 2c20  p_optional(str, 
+0000f0d0: 6d65 7461 6461 7461 5f65 6e74 7279 2e72  metadata_entry.r
+0000f0e0: 6576 6973 696f 6e29 2c0a 2020 2020 2020  evision),.      
+0000f0f0: 2020 2020 2020 2020 2020 7061 7468 3d6d            path=m
+0000f100: 6574 6164 6174 615f 656e 7472 792e 7061  etadata_entry.pa
+0000f110: 7468 2c0a 2020 2020 2020 2020 2020 2020  th,.            
+0000f120: 2020 2020 6469 7265 6374 6f72 793d 6d61      directory=ma
+0000f130: 705f 6f70 7469 6f6e 616c 2873 7472 2c20  p_optional(str, 
+0000f140: 6d65 7461 6461 7461 5f65 6e74 7279 2e64  metadata_entry.d
+0000f150: 6972 6563 746f 7279 292c 0a20 2020 2020  irectory),.     
+0000f160: 2020 2020 2020 2020 2020 2063 7572 3d63             cur=c
+0000f170: 7572 2c0a 2020 2020 2020 2020 2020 2020  ur,.            
+0000f180: 290a 2020 2020 2020 2020 2020 2020 636f  ).            co
+0000f190: 756e 7465 725b 6d65 7461 6461 7461 5f65  unter[metadata_e
+0000f1a0: 6e74 7279 2e74 6172 6765 742e 6f62 6a65  ntry.target.obje
+0000f1b0: 6374 5f74 7970 655d 202b 3d20 310a 0a20  ct_type] += 1.. 
+0000f1c0: 2020 2020 2020 2072 6574 7572 6e20 7b0a         return {.
+0000f1d0: 2020 2020 2020 2020 2020 2020 6622 7b74              f"{t
+0000f1e0: 7970 652e 7661 6c75 657d 5f6d 6574 6164  ype.value}_metad
+0000f1f0: 6174 613a 6164 6422 3a20 636f 756e 7420  ata:add": count 
+0000f200: 666f 7220 2874 7970 652c 2063 6f75 6e74  for (type, count
+0000f210: 2920 696e 2063 6f75 6e74 6572 2e69 7465  ) in counter.ite
+0000f220: 6d73 2829 0a20 2020 2020 2020 207d 0a0a  ms().        }..
+0000f230: 2020 2020 4064 625f 7472 616e 7361 6374      @db_transact
+0000f240: 696f 6e28 290a 2020 2020 6465 6620 7261  ion().    def ra
+0000f250: 775f 6578 7472 696e 7369 635f 6d65 7461  w_extrinsic_meta
+0000f260: 6461 7461 5f67 6574 280a 2020 2020 2020  data_get(.      
+0000f270: 2020 7365 6c66 2c0a 2020 2020 2020 2020    self,.        
+0000f280: 7461 7267 6574 3a20 4578 7465 6e64 6564  target: Extended
+0000f290: 5357 4849 442c 0a20 2020 2020 2020 2061  SWHID,.        a
+0000f2a0: 7574 686f 7269 7479 3a20 4d65 7461 6461  uthority: Metada
+0000f2b0: 7461 4175 7468 6f72 6974 792c 0a20 2020  taAuthority,.   
+0000f2c0: 2020 2020 2061 6674 6572 3a20 4f70 7469       after: Opti
+0000f2d0: 6f6e 616c 5b64 6174 6574 696d 652e 6461  onal[datetime.da
+0000f2e0: 7465 7469 6d65 5d20 3d20 4e6f 6e65 2c0a  tetime] = None,.
+0000f2f0: 2020 2020 2020 2020 7061 6765 5f74 6f6b          page_tok
+0000f300: 656e 3a20 4f70 7469 6f6e 616c 5b62 7974  en: Optional[byt
+0000f310: 6573 5d20 3d20 4e6f 6e65 2c0a 2020 2020  es] = None,.    
+0000f320: 2020 2020 6c69 6d69 743a 2069 6e74 203d      limit: int =
+0000f330: 2031 3030 302c 0a20 2020 2020 2020 202a   1000,.        *
+0000f340: 2c0a 2020 2020 2020 2020 6462 3a20 4462  ,.        db: Db
+0000f350: 2c0a 2020 2020 2020 2020 6375 723d 4e6f  ,.        cur=No
+0000f360: 6e65 2c0a 2020 2020 2920 2d3e 2050 6167  ne,.    ) -> Pag
+0000f370: 6564 5265 7375 6c74 5b52 6177 4578 7472  edResult[RawExtr
+0000f380: 696e 7369 634d 6574 6164 6174 615d 3a0a  insicMetadata]:.
+0000f390: 2020 2020 2020 2020 6966 2070 6167 655f          if page_
+0000f3a0: 746f 6b65 6e3a 0a20 2020 2020 2020 2020  token:.         
+0000f3b0: 2020 2028 6166 7465 725f 7469 6d65 2c20     (after_time, 
+0000f3c0: 6166 7465 725f 6665 7463 6865 7229 203d  after_fetcher) =
+0000f3d0: 206d 7367 7061 636b 5f6c 6f61 6473 2862   msgpack_loads(b
+0000f3e0: 6173 6536 342e 6236 3464 6563 6f64 6528  ase64.b64decode(
+0000f3f0: 7061 6765 5f74 6f6b 656e 2929 0a20 2020  page_token)).   
+0000f400: 2020 2020 2020 2020 2069 6620 6166 7465           if afte
+0000f410: 7220 616e 6420 6166 7465 725f 7469 6d65  r and after_time
+0000f420: 203c 2061 6674 6572 3a0a 2020 2020 2020   < after:.      
+0000f430: 2020 2020 2020 2020 2020 7261 6973 6520            raise 
+0000f440: 5374 6f72 6167 6541 7267 756d 656e 7445  StorageArgumentE
+0000f450: 7863 6570 7469 6f6e 280a 2020 2020 2020  xception(.      
+0000f460: 2020 2020 2020 2020 2020 2020 2020 2270                "p
+0000f470: 6167 655f 746f 6b65 6e20 6973 2069 6e63  age_token is inc
+0000f480: 6f6e 7369 7374 656e 7420 7769 7468 2074  onsistent with t
+0000f490: 6865 2076 616c 7565 206f 6620 2761 6674  he value of 'aft
+0000f4a0: 6572 272e 220a 2020 2020 2020 2020 2020  er'.".          
+0000f4b0: 2020 2020 2020 290a 2020 2020 2020 2020        ).        
+0000f4c0: 656c 7365 3a0a 2020 2020 2020 2020 2020  else:.          
+0000f4d0: 2020 6166 7465 725f 7469 6d65 203d 2061    after_time = a
+0000f4e0: 6674 6572 0a20 2020 2020 2020 2020 2020  fter.           
+0000f4f0: 2061 6674 6572 5f66 6574 6368 6572 203d   after_fetcher =
+0000f500: 204e 6f6e 650a 0a20 2020 2020 2020 2074   None..        t
+0000f510: 7279 3a0a 2020 2020 2020 2020 2020 2020  ry:.            
+0000f520: 6175 7468 6f72 6974 795f 6964 203d 2073  authority_id = s
+0000f530: 656c 662e 5f67 6574 5f61 7574 686f 7269  elf._get_authori
+0000f540: 7479 5f69 6428 6175 7468 6f72 6974 792c  ty_id(authority,
+0000f550: 2064 622c 2063 7572 290a 2020 2020 2020   db, cur).      
+0000f560: 2020 6578 6365 7074 2055 6e6b 6e6f 776e    except Unknown
+0000f570: 4d65 7461 6461 7461 4175 7468 6f72 6974  MetadataAuthorit
+0000f580: 793a 0a20 2020 2020 2020 2020 2020 2072  y:.            r
+0000f590: 6574 7572 6e20 5061 6765 6452 6573 756c  eturn PagedResul
+0000f5a0: 7428 0a20 2020 2020 2020 2020 2020 2020  t(.             
+0000f5b0: 2020 206e 6578 745f 7061 6765 5f74 6f6b     next_page_tok
+0000f5c0: 656e 3d4e 6f6e 652c 0a20 2020 2020 2020  en=None,.       
+0000f5d0: 2020 2020 2020 2020 2072 6573 756c 7473           results
+0000f5e0: 3d5b 5d2c 0a20 2020 2020 2020 2020 2020  =[],.           
+0000f5f0: 2029 0a0a 2020 2020 2020 2020 726f 7773   )..        rows
+0000f600: 203d 2064 622e 7261 775f 6578 7472 696e   = db.raw_extrin
+0000f610: 7369 635f 6d65 7461 6461 7461 5f67 6574  sic_metadata_get
+0000f620: 280a 2020 2020 2020 2020 2020 2020 7374  (.            st
+0000f630: 7228 7461 7267 6574 292c 0a20 2020 2020  r(target),.     
+0000f640: 2020 2020 2020 2061 7574 686f 7269 7479         authority
+0000f650: 5f69 642c 0a20 2020 2020 2020 2020 2020  _id,.           
+0000f660: 2061 6674 6572 5f74 696d 652c 0a20 2020   after_time,.   
+0000f670: 2020 2020 2020 2020 2061 6674 6572 5f66           after_f
+0000f680: 6574 6368 6572 2c0a 2020 2020 2020 2020  etcher,.        
+0000f690: 2020 2020 6c69 6d69 7420 2b20 312c 0a20      limit + 1,. 
+0000f6a0: 2020 2020 2020 2020 2020 2063 7572 2c0a             cur,.
+0000f6b0: 2020 2020 2020 2020 290a 2020 2020 2020          ).      
+0000f6c0: 2020 726f 7773 203d 205b 6469 6374 287a    rows = [dict(z
+0000f6d0: 6970 2864 622e 7261 775f 6578 7472 696e  ip(db.raw_extrin
+0000f6e0: 7369 635f 6d65 7461 6461 7461 5f67 6574  sic_metadata_get
+0000f6f0: 5f63 6f6c 732c 2072 6f77 2929 2066 6f72  _cols, row)) for
+0000f700: 2072 6f77 2069 6e20 726f 7773 5d0a 2020   row in rows].  
+0000f710: 2020 2020 2020 7265 7375 6c74 7320 3d20        results = 
+0000f720: 5b5d 0a20 2020 2020 2020 2066 6f72 2072  [].        for r
+0000f730: 6f77 2069 6e20 726f 7773 3a0a 2020 2020  ow in rows:.    
+0000f740: 2020 2020 2020 2020 6173 7365 7274 2073          assert s
+0000f750: 7472 2874 6172 6765 7429 203d 3d20 726f  tr(target) == ro
+0000f760: 775b 2272 6177 5f65 7874 7269 6e73 6963  w["raw_extrinsic
+0000f770: 5f6d 6574 6164 6174 612e 7461 7267 6574  _metadata.target
+0000f780: 225d 0a20 2020 2020 2020 2020 2020 2072  "].            r
+0000f790: 6573 756c 7473 2e61 7070 656e 6428 636f  esults.append(co
+0000f7a0: 6e76 6572 7465 7273 2e64 625f 746f 5f72  nverters.db_to_r
+0000f7b0: 6177 5f65 7874 7269 6e73 6963 5f6d 6574  aw_extrinsic_met
+0000f7c0: 6164 6174 6128 726f 7729 290a 0a20 2020  adata(row))..   
+0000f7d0: 2020 2020 2069 6620 6c65 6e28 7265 7375       if len(resu
+0000f7e0: 6c74 7329 203e 206c 696d 6974 3a0a 2020  lts) > limit:.  
+0000f7f0: 2020 2020 2020 2020 2020 7265 7375 6c74            result
+0000f800: 732e 706f 7028 290a 2020 2020 2020 2020  s.pop().        
+0000f810: 2020 2020 6173 7365 7274 206c 656e 2872      assert len(r
+0000f820: 6573 756c 7473 2920 3d3d 206c 696d 6974  esults) == limit
+0000f830: 0a20 2020 2020 2020 2020 2020 206c 6173  .            las
+0000f840: 745f 7265 7475 726e 6564 5f72 6f77 203d  t_returned_row =
+0000f850: 2072 6f77 735b 2d32 5d20 2023 2072 6f77   rows[-2]  # row
+0000f860: 735b 2d31 5d20 636f 7272 6573 706f 6e64  s[-1] correspond
+0000f870: 7320 746f 2074 6865 2070 6f70 7065 6420  s to the popped 
+0000f880: 7265 7375 6c74 0a20 2020 2020 2020 2020  result.         
+0000f890: 2020 206e 6578 745f 7061 6765 5f74 6f6b     next_page_tok
+0000f8a0: 656e 3a20 4f70 7469 6f6e 616c 5b73 7472  en: Optional[str
+0000f8b0: 5d20 3d20 6261 7365 3634 2e62 3634 656e  ] = base64.b64en
+0000f8c0: 636f 6465 280a 2020 2020 2020 2020 2020  code(.          
+0000f8d0: 2020 2020 2020 6d73 6770 6163 6b5f 6475        msgpack_du
+0000f8e0: 6d70 7328 0a20 2020 2020 2020 2020 2020  mps(.           
+0000f8f0: 2020 2020 2020 2020 2028 0a20 2020 2020           (.     
+0000f900: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f910: 2020 206c 6173 745f 7265 7475 726e 6564     last_returned
+0000f920: 5f72 6f77 5b22 6469 7363 6f76 6572 795f  _row["discovery_
+0000f930: 6461 7465 225d 2c0a 2020 2020 2020 2020  date"],.        
+0000f940: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f950: 6c61 7374 5f72 6574 7572 6e65 645f 726f  last_returned_ro
+0000f960: 775b 226d 6574 6164 6174 615f 6665 7463  w["metadata_fetc
+0000f970: 6865 722e 6964 225d 2c0a 2020 2020 2020  her.id"],.      
+0000f980: 2020 2020 2020 2020 2020 2020 2020 290a                ).
+0000f990: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f9a0: 290a 2020 2020 2020 2020 2020 2020 292e  ).            ).
+0000f9b0: 6465 636f 6465 2829 0a20 2020 2020 2020  decode().       
+0000f9c0: 2065 6c73 653a 0a20 2020 2020 2020 2020   else:.         
+0000f9d0: 2020 206e 6578 745f 7061 6765 5f74 6f6b     next_page_tok
+0000f9e0: 656e 203d 204e 6f6e 650a 0a20 2020 2020  en = None..     
+0000f9f0: 2020 2072 6574 7572 6e20 5061 6765 6452     return PagedR
+0000fa00: 6573 756c 7428 0a20 2020 2020 2020 2020  esult(.         
+0000fa10: 2020 206e 6578 745f 7061 6765 5f74 6f6b     next_page_tok
+0000fa20: 656e 3d6e 6578 745f 7061 6765 5f74 6f6b  en=next_page_tok
+0000fa30: 656e 2c0a 2020 2020 2020 2020 2020 2020  en,.            
+0000fa40: 7265 7375 6c74 733d 7265 7375 6c74 732c  results=results,
+0000fa50: 0a20 2020 2020 2020 2029 0a0a 2020 2020  .        )..    
+0000fa60: 4064 625f 7472 616e 7361 6374 696f 6e28  @db_transaction(
+0000fa70: 290a 2020 2020 6465 6620 7261 775f 6578  ).    def raw_ex
+0000fa80: 7472 696e 7369 635f 6d65 7461 6461 7461  trinsic_metadata
+0000fa90: 5f67 6574 5f62 795f 6964 7328 0a20 2020  _get_by_ids(.   
+0000faa0: 2020 2020 2073 656c 662c 0a20 2020 2020       self,.     
+0000fab0: 2020 2069 6473 3a20 4c69 7374 5b53 6861     ids: List[Sha
+0000fac0: 3147 6974 5d2c 0a20 2020 2020 2020 202a  1Git],.        *
+0000fad0: 2c0a 2020 2020 2020 2020 6462 3a20 4462  ,.        db: Db
+0000fae0: 2c0a 2020 2020 2020 2020 6375 723d 4e6f  ,.        cur=No
+0000faf0: 6e65 2c0a 2020 2020 2920 2d3e 204c 6973  ne,.    ) -> Lis
+0000fb00: 745b 5261 7745 7874 7269 6e73 6963 4d65  t[RawExtrinsicMe
+0000fb10: 7461 6461 7461 5d3a 0a20 2020 2020 2020  tadata]:.       
+0000fb20: 2072 6574 7572 6e20 5b0a 2020 2020 2020   return [.      
+0000fb30: 2020 2020 2020 636f 6e76 6572 7465 7273        converters
+0000fb40: 2e64 625f 746f 5f72 6177 5f65 7874 7269  .db_to_raw_extri
+0000fb50: 6e73 6963 5f6d 6574 6164 6174 6128 0a20  nsic_metadata(. 
+0000fb60: 2020 2020 2020 2020 2020 2020 2020 2064                 d
+0000fb70: 6963 7428 7a69 7028 6462 2e72 6177 5f65  ict(zip(db.raw_e
+0000fb80: 7874 7269 6e73 6963 5f6d 6574 6164 6174  xtrinsic_metadat
+0000fb90: 615f 6765 745f 636f 6c73 2c20 726f 7729  a_get_cols, row)
+0000fba0: 290a 2020 2020 2020 2020 2020 2020 290a  ).            ).
+0000fbb0: 2020 2020 2020 2020 2020 2020 666f 7220              for 
+0000fbc0: 726f 7720 696e 2064 622e 7261 775f 6578  row in db.raw_ex
+0000fbd0: 7472 696e 7369 635f 6d65 7461 6461 7461  trinsic_metadata
+0000fbe0: 5f67 6574 5f62 795f 6964 7328 6964 7329  _get_by_ids(ids)
+0000fbf0: 0a20 2020 2020 2020 205d 0a0a 2020 2020  .        ]..    
+0000fc00: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+0000fc10: 2323 2323 2323 2323 2323 0a20 2020 2023  ##########.    #
+0000fc20: 204d 6574 6164 6174 6146 6574 6368 6572   MetadataFetcher
+0000fc30: 2061 6e64 204d 6574 6164 6174 6141 7574   and MetadataAut
+0000fc40: 686f 7269 7479 0a20 2020 2023 2323 2323  hority.    #####
+0000fc50: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+0000fc60: 2323 2323 230a 0a20 2020 2040 6462 5f74  #####..    @db_t
+0000fc70: 7261 6e73 6163 7469 6f6e 2829 0a20 2020  ransaction().   
+0000fc80: 2064 6566 206d 6574 6164 6174 615f 6665   def metadata_fe
+0000fc90: 7463 6865 725f 6164 6428 0a20 2020 2020  tcher_add(.     
+0000fca0: 2020 2073 656c 662c 2066 6574 6368 6572     self, fetcher
+0000fcb0: 733a 204c 6973 745b 4d65 7461 6461 7461  s: List[Metadata
+0000fcc0: 4665 7463 6865 725d 2c20 2a2c 2064 623a  Fetcher], *, db:
+0000fcd0: 2044 622c 2063 7572 3d4e 6f6e 650a 2020   Db, cur=None.  
+0000fce0: 2020 2920 2d3e 2044 6963 745b 7374 722c    ) -> Dict[str,
+0000fcf0: 2069 6e74 5d3a 0a20 2020 2020 2020 2066   int]:.        f
+0000fd00: 6574 6368 6572 7320 3d20 6c69 7374 2866  etchers = list(f
+0000fd10: 6574 6368 6572 7329 0a20 2020 2020 2020  etchers).       
+0000fd20: 2073 656c 662e 6a6f 7572 6e61 6c5f 7772   self.journal_wr
+0000fd30: 6974 6572 2e6d 6574 6164 6174 615f 6665  iter.metadata_fe
+0000fd40: 7463 6865 725f 6164 6428 6665 7463 6865  tcher_add(fetche
+0000fd50: 7273 290a 2020 2020 2020 2020 636f 756e  rs).        coun
+0000fd60: 7420 3d20 300a 2020 2020 2020 2020 666f  t = 0.        fo
+0000fd70: 7220 6665 7463 6865 7220 696e 2066 6574  r fetcher in fet
+0000fd80: 6368 6572 733a 0a20 2020 2020 2020 2020  chers:.         
+0000fd90: 2020 2064 622e 6d65 7461 6461 7461 5f66     db.metadata_f
+0000fda0: 6574 6368 6572 5f61 6464 2866 6574 6368  etcher_add(fetch
+0000fdb0: 6572 2e6e 616d 652c 2066 6574 6368 6572  er.name, fetcher
+0000fdc0: 2e76 6572 7369 6f6e 2c20 6375 723d 6375  .version, cur=cu
+0000fdd0: 7229 0a20 2020 2020 2020 2020 2020 2063  r).            c
+0000fde0: 6f75 6e74 202b 3d20 310a 2020 2020 2020  ount += 1.      
+0000fdf0: 2020 7265 7475 726e 207b 226d 6574 6164    return {"metad
+0000fe00: 6174 615f 6665 7463 6865 723a 6164 6422  ata_fetcher:add"
+0000fe10: 3a20 636f 756e 747d 0a0a 2020 2020 4064  : count}..    @d
+0000fe20: 625f 7472 616e 7361 6374 696f 6e28 7374  b_transaction(st
+0000fe30: 6174 656d 656e 745f 7469 6d65 6f75 743d  atement_timeout=
+0000fe40: 3530 3029 0a20 2020 2064 6566 206d 6574  500).    def met
+0000fe50: 6164 6174 615f 6665 7463 6865 725f 6765  adata_fetcher_ge
+0000fe60: 7428 0a20 2020 2020 2020 2073 656c 662c  t(.        self,
+0000fe70: 206e 616d 653a 2073 7472 2c20 7665 7273   name: str, vers
+0000fe80: 696f 6e3a 2073 7472 2c20 2a2c 2064 623a  ion: str, *, db:
+0000fe90: 2044 622c 2063 7572 3d4e 6f6e 650a 2020   Db, cur=None.  
+0000fea0: 2020 2920 2d3e 204f 7074 696f 6e61 6c5b    ) -> Optional[
+0000feb0: 4d65 7461 6461 7461 4665 7463 6865 725d  MetadataFetcher]
+0000fec0: 3a0a 2020 2020 2020 2020 726f 7720 3d20  :.        row = 
+0000fed0: 6462 2e6d 6574 6164 6174 615f 6665 7463  db.metadata_fetc
+0000fee0: 6865 725f 6765 7428 6e61 6d65 2c20 7665  her_get(name, ve
+0000fef0: 7273 696f 6e2c 2063 7572 3d63 7572 290a  rsion, cur=cur).
+0000ff00: 2020 2020 2020 2020 6966 206e 6f74 2072          if not r
+0000ff10: 6f77 3a0a 2020 2020 2020 2020 2020 2020  ow:.            
+0000ff20: 7265 7475 726e 204e 6f6e 650a 2020 2020  return None.    
+0000ff30: 2020 2020 7265 7475 726e 204d 6574 6164      return Metad
+0000ff40: 6174 6146 6574 6368 6572 2e66 726f 6d5f  ataFetcher.from_
+0000ff50: 6469 6374 2864 6963 7428 7a69 7028 6462  dict(dict(zip(db
+0000ff60: 2e6d 6574 6164 6174 615f 6665 7463 6865  .metadata_fetche
+0000ff70: 725f 636f 6c73 2c20 726f 7729 2929 0a0a  r_cols, row)))..
+0000ff80: 2020 2020 4064 625f 7472 616e 7361 6374      @db_transact
+0000ff90: 696f 6e28 290a 2020 2020 6465 6620 7261  ion().    def ra
+0000ffa0: 775f 6578 7472 696e 7369 635f 6d65 7461  w_extrinsic_meta
+0000ffb0: 6461 7461 5f67 6574 5f61 7574 686f 7269  data_get_authori
+0000ffc0: 7469 6573 280a 2020 2020 2020 2020 7365  ties(.        se
+0000ffd0: 6c66 2c0a 2020 2020 2020 2020 7461 7267  lf,.        targ
+0000ffe0: 6574 3a20 4578 7465 6e64 6564 5357 4849  et: ExtendedSWHI
+0000fff0: 442c 0a20 2020 2020 2020 202a 2c0a 2020  D,.        *,.  
+00010000: 2020 2020 2020 6462 3a20 4462 2c0a 2020        db: Db,.  
+00010010: 2020 2020 2020 6375 723d 4e6f 6e65 2c0a        cur=None,.
+00010020: 2020 2020 2920 2d3e 204c 6973 745b 4d65      ) -> List[Me
+00010030: 7461 6461 7461 4175 7468 6f72 6974 795d  tadataAuthority]
+00010040: 3a0a 2020 2020 2020 2020 7265 7475 726e  :.        return
+00010050: 205b 0a20 2020 2020 2020 2020 2020 204d   [.            M
+00010060: 6574 6164 6174 6141 7574 686f 7269 7479  etadataAuthority
+00010070: 280a 2020 2020 2020 2020 2020 2020 2020  (.              
+00010080: 2020 7479 7065 3d4d 6574 6164 6174 6141    type=MetadataA
+00010090: 7574 686f 7269 7479 5479 7065 2861 7574  uthorityType(aut
+000100a0: 686f 7269 7479 5f74 7970 6529 2c20 7572  hority_type), ur
+000100b0: 6c3d 6175 7468 6f72 6974 795f 7572 6c0a  l=authority_url.
+000100c0: 2020 2020 2020 2020 2020 2020 290a 2020              ).  
+000100d0: 2020 2020 2020 2020 2020 666f 7220 280a            for (.
+000100e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000100f0: 6175 7468 6f72 6974 795f 7479 7065 2c0a  authority_type,.
+00010100: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010110: 6175 7468 6f72 6974 795f 7572 6c2c 0a20  authority_url,. 
+00010120: 2020 2020 2020 2020 2020 2029 2069 6e20             ) in 
+00010130: 6462 2e72 6177 5f65 7874 7269 6e73 6963  db.raw_extrinsic
+00010140: 5f6d 6574 6164 6174 615f 6765 745f 6175  _metadata_get_au
+00010150: 7468 6f72 6974 6965 7328 7374 7228 7461  thorities(str(ta
+00010160: 7267 6574 292c 2063 7572 290a 2020 2020  rget), cur).    
+00010170: 2020 2020 5d0a 0a20 2020 2040 6462 5f74      ]..    @db_t
+00010180: 7261 6e73 6163 7469 6f6e 2829 0a20 2020  ransaction().   
+00010190: 2064 6566 206d 6574 6164 6174 615f 6175   def metadata_au
+000101a0: 7468 6f72 6974 795f 6164 6428 0a20 2020  thority_add(.   
+000101b0: 2020 2020 2073 656c 662c 2061 7574 686f       self, autho
+000101c0: 7269 7469 6573 3a20 4c69 7374 5b4d 6574  rities: List[Met
+000101d0: 6164 6174 6141 7574 686f 7269 7479 5d2c  adataAuthority],
+000101e0: 202a 2c20 6462 3a20 4462 2c20 6375 723d   *, db: Db, cur=
+000101f0: 4e6f 6e65 0a20 2020 2029 202d 3e20 4469  None.    ) -> Di
+00010200: 6374 5b73 7472 2c20 696e 745d 3a0a 2020  ct[str, int]:.  
+00010210: 2020 2020 2020 6175 7468 6f72 6974 6965        authoritie
+00010220: 7320 3d20 6c69 7374 2861 7574 686f 7269  s = list(authori
+00010230: 7469 6573 290a 2020 2020 2020 2020 7365  ties).        se
+00010240: 6c66 2e6a 6f75 726e 616c 5f77 7269 7465  lf.journal_write
+00010250: 722e 6d65 7461 6461 7461 5f61 7574 686f  r.metadata_autho
+00010260: 7269 7479 5f61 6464 2861 7574 686f 7269  rity_add(authori
+00010270: 7469 6573 290a 2020 2020 2020 2020 636f  ties).        co
+00010280: 756e 7420 3d20 300a 2020 2020 2020 2020  unt = 0.        
+00010290: 666f 7220 6175 7468 6f72 6974 7920 696e  for authority in
+000102a0: 2061 7574 686f 7269 7469 6573 3a0a 2020   authorities:.  
+000102b0: 2020 2020 2020 2020 2020 6462 2e6d 6574            db.met
+000102c0: 6164 6174 615f 6175 7468 6f72 6974 795f  adata_authority_
+000102d0: 6164 6428 6175 7468 6f72 6974 792e 7479  add(authority.ty
+000102e0: 7065 2e76 616c 7565 2c20 6175 7468 6f72  pe.value, author
+000102f0: 6974 792e 7572 6c2c 2063 7572 3d63 7572  ity.url, cur=cur
+00010300: 290a 2020 2020 2020 2020 2020 2020 636f  ).            co
+00010310: 756e 7420 2b3d 2031 0a20 2020 2020 2020  unt += 1.       
+00010320: 2072 6574 7572 6e20 7b22 6d65 7461 6461   return {"metada
+00010330: 7461 5f61 7574 686f 7269 7479 3a61 6464  ta_authority:add
+00010340: 223a 2063 6f75 6e74 7d0a 0a20 2020 2040  ": count}..    @
+00010350: 6462 5f74 7261 6e73 6163 7469 6f6e 2829  db_transaction()
+00010360: 0a20 2020 2064 6566 206d 6574 6164 6174  .    def metadat
+00010370: 615f 6175 7468 6f72 6974 795f 6765 7428  a_authority_get(
+00010380: 0a20 2020 2020 2020 2073 656c 662c 2074  .        self, t
+00010390: 7970 653a 204d 6574 6164 6174 6141 7574  ype: MetadataAut
+000103a0: 686f 7269 7479 5479 7065 2c20 7572 6c3a  horityType, url:
+000103b0: 2073 7472 2c20 2a2c 2064 623a 2044 622c   str, *, db: Db,
+000103c0: 2063 7572 3d4e 6f6e 650a 2020 2020 2920   cur=None.    ) 
+000103d0: 2d3e 204f 7074 696f 6e61 6c5b 4d65 7461  -> Optional[Meta
+000103e0: 6461 7461 4175 7468 6f72 6974 795d 3a0a  dataAuthority]:.
+000103f0: 2020 2020 2020 2020 726f 7720 3d20 6462          row = db
+00010400: 2e6d 6574 6164 6174 615f 6175 7468 6f72  .metadata_author
+00010410: 6974 795f 6765 7428 7479 7065 2e76 616c  ity_get(type.val
+00010420: 7565 2c20 7572 6c2c 2063 7572 3d63 7572  ue, url, cur=cur
+00010430: 290a 2020 2020 2020 2020 6966 206e 6f74  ).        if not
+00010440: 2072 6f77 3a0a 2020 2020 2020 2020 2020   row:.          
+00010450: 2020 7265 7475 726e 204e 6f6e 650a 2020    return None.  
+00010460: 2020 2020 2020 7265 7475 726e 204d 6574        return Met
+00010470: 6164 6174 6141 7574 686f 7269 7479 2e66  adataAuthority.f
+00010480: 726f 6d5f 6469 6374 2864 6963 7428 7a69  rom_dict(dict(zi
+00010490: 7028 6462 2e6d 6574 6164 6174 615f 6175  p(db.metadata_au
+000104a0: 7468 6f72 6974 795f 636f 6c73 2c20 726f  thority_cols, ro
+000104b0: 7729 2929 0a0a 2020 2020 2323 2323 2323  w)))..    ######
+000104c0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+000104d0: 2323 230a 2020 2020 2320 276f 626a 6563  ###.    # 'objec
+000104e0: 745f 7265 6665 7265 6e63 6573 2720 7461  t_references' ta
+000104f0: 626c 650a 2020 2020 2323 2323 2323 2323  ble.    ########
+00010500: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00010510: 230a 0a20 2020 2040 6462 5f74 7261 6e73  #..    @db_trans
+00010520: 6163 7469 6f6e 2829 0a20 2020 2064 6566  action().    def
+00010530: 206f 626a 6563 745f 6669 6e64 5f72 6563   object_find_rec
+00010540: 656e 745f 7265 6665 7265 6e63 6573 280a  ent_references(.
+00010550: 2020 2020 2020 2020 7365 6c66 2c20 7461          self, ta
+00010560: 7267 6574 5f73 7768 6964 3a20 4578 7465  rget_swhid: Exte
+00010570: 6e64 6564 5357 4849 442c 206c 696d 6974  ndedSWHID, limit
+00010580: 3a20 696e 742c 202a 2c20 6462 3a20 4462  : int, *, db: Db
+00010590: 2c20 6375 723d 4e6f 6e65 0a20 2020 2029  , cur=None.    )
+000105a0: 202d 3e20 4c69 7374 5b45 7874 656e 6465   -> List[Extende
+000105b0: 6453 5748 4944 5d3a 0a20 2020 2020 2020  dSWHID]:.       
+000105c0: 2072 6574 7572 6e20 5b0a 2020 2020 2020   return [.      
+000105d0: 2020 2020 2020 636f 6e76 6572 7465 7273        converters
+000105e0: 2e64 625f 746f 5f6f 626a 6563 745f 7265  .db_to_object_re
+000105f0: 6665 7265 6e63 655f 736f 7572 6365 2872  ference_source(r
+00010600: 6f77 290a 2020 2020 2020 2020 2020 2020  ow).            
+00010610: 666f 7220 726f 7720 696e 2064 622e 6f62  for row in db.ob
+00010620: 6a65 6374 5f72 6566 6572 656e 6365 735f  ject_references_
+00010630: 6765 7428 0a20 2020 2020 2020 2020 2020  get(.           
+00010640: 2020 2020 2074 6172 6765 745f 7479 7065       target_type
+00010650: 3d74 6172 6765 745f 7377 6869 642e 6f62  =target_swhid.ob
+00010660: 6a65 6374 5f74 7970 652e 6e61 6d65 2e6c  ject_type.name.l
+00010670: 6f77 6572 2829 2c0a 2020 2020 2020 2020  ower(),.        
+00010680: 2020 2020 2020 2020 7461 7267 6574 3d74          target=t
+00010690: 6172 6765 745f 7377 6869 642e 6f62 6a65  arget_swhid.obje
+000106a0: 6374 5f69 642c 0a20 2020 2020 2020 2020  ct_id,.         
+000106b0: 2020 2020 2020 206c 696d 6974 3d6c 696d         limit=lim
+000106c0: 6974 2c0a 2020 2020 2020 2020 2020 2020  it,.            
+000106d0: 2020 2020 6375 723d 6375 722c 0a20 2020      cur=cur,.   
+000106e0: 2020 2020 2020 2020 2029 0a20 2020 2020           ).     
+000106f0: 2020 205d 0a0a 2020 2020 4064 625f 7472     ]..    @db_tr
+00010700: 616e 7361 6374 696f 6e28 290a 2020 2020  ansaction().    
+00010710: 6465 6620 6f62 6a65 6374 5f72 6566 6572  def object_refer
+00010720: 656e 6365 735f 6164 6428 0a20 2020 2020  ences_add(.     
+00010730: 2020 2073 656c 662c 2072 6566 6572 656e     self, referen
+00010740: 6365 733a 204c 6973 745b 4f62 6a65 6374  ces: List[Object
+00010750: 5265 6665 7265 6e63 655d 2c20 2a2c 2064  Reference], *, d
+00010760: 623a 2044 622c 2063 7572 3d4e 6f6e 650a  b: Db, cur=None.
+00010770: 2020 2020 2920 2d3e 2044 6963 745b 7374      ) -> Dict[st
+00010780: 722c 2069 6e74 5d3a 0a20 2020 2020 2020  r, int]:.       
+00010790: 2074 6f5f 6164 6420 3d20 6c69 7374 287b   to_add = list({
+000107a0: 636f 6e76 6572 7465 7273 2e6f 626a 6563  converters.objec
+000107b0: 745f 7265 6665 7265 6e63 655f 746f 5f64  t_reference_to_d
+000107c0: 6228 7265 6629 2066 6f72 2072 6566 2069  b(ref) for ref i
+000107d0: 6e20 7265 6665 7265 6e63 6573 7d29 0a20  n references}). 
+000107e0: 2020 2020 2020 2064 622e 6f62 6a65 6374         db.object
+000107f0: 5f72 6566 6572 656e 6365 735f 6164 6428  _references_add(
+00010800: 0a20 2020 2020 2020 2020 2020 2074 6f5f  .            to_
+00010810: 6164 642c 0a20 2020 2020 2020 2020 2020  add,.           
+00010820: 2063 7572 3d63 7572 2c0a 2020 2020 2020   cur=cur,.      
+00010830: 2020 290a 0a20 2020 2020 2020 2072 6574    )..        ret
+00010840: 7572 6e20 7b22 6f62 6a65 6374 5f72 6566  urn {"object_ref
+00010850: 6572 656e 6365 3a61 6464 223a 206c 656e  erence:add": len
+00010860: 2874 6f5f 6164 6429 7d0a 0a20 2020 2064  (to_add)}..    d
+00010870: 6566 2063 6c65 6172 5f62 7566 6665 7273  ef clear_buffers
+00010880: 2873 656c 662c 206f 626a 6563 745f 7479  (self, object_ty
+00010890: 7065 733a 2053 6571 7565 6e63 655b 7374  pes: Sequence[st
+000108a0: 725d 203d 2028 2929 202d 3e20 4e6f 6e65  r] = ()) -> None
+000108b0: 3a0a 2020 2020 2020 2020 2222 2244 6f20  :.        """Do 
+000108c0: 6e6f 7468 696e 6722 2222 0a20 2020 2020  nothing""".     
+000108d0: 2020 2072 6574 7572 6e20 4e6f 6e65 0a0a     return None..
+000108e0: 2020 2020 6465 6620 666c 7573 6828 7365      def flush(se
+000108f0: 6c66 2c20 6f62 6a65 6374 5f74 7970 6573  lf, object_types
+00010900: 3a20 5365 7175 656e 6365 5b73 7472 5d20  : Sequence[str] 
+00010910: 3d20 2829 2920 2d3e 2044 6963 745b 7374  = ()) -> Dict[st
+00010920: 722c 2069 6e74 5d3a 0a20 2020 2020 2020  r, int]:.       
+00010930: 2072 6574 7572 6e20 7b7d 0a0a 2020 2020   return {}..    
+00010940: 6465 6620 5f67 6574 5f61 7574 686f 7269  def _get_authori
+00010950: 7479 5f69 6428 7365 6c66 2c20 6175 7468  ty_id(self, auth
+00010960: 6f72 6974 793a 204d 6574 6164 6174 6141  ority: MetadataA
+00010970: 7574 686f 7269 7479 2c20 6462 2c20 6375  uthority, db, cu
+00010980: 7229 3a0a 2020 2020 2020 2020 6175 7468  r):.        auth
+00010990: 6f72 6974 795f 6964 203d 2064 622e 6d65  ority_id = db.me
+000109a0: 7461 6461 7461 5f61 7574 686f 7269 7479  tadata_authority
+000109b0: 5f67 6574 5f69 6428 0a20 2020 2020 2020  _get_id(.       
+000109c0: 2020 2020 2061 7574 686f 7269 7479 2e74       authority.t
+000109d0: 7970 652e 7661 6c75 652c 2061 7574 686f  ype.value, autho
+000109e0: 7269 7479 2e75 726c 2c20 6375 720a 2020  rity.url, cur.  
+000109f0: 2020 2020 2020 290a 2020 2020 2020 2020        ).        
+00010a00: 6966 206e 6f74 2061 7574 686f 7269 7479  if not authority
+00010a10: 5f69 643a 0a20 2020 2020 2020 2020 2020  _id:.           
+00010a20: 2072 6169 7365 2055 6e6b 6e6f 776e 4d65   raise UnknownMe
+00010a30: 7461 6461 7461 4175 7468 6f72 6974 7928  tadataAuthority(
+00010a40: 7374 7228 6175 7468 6f72 6974 7929 290a  str(authority)).
+00010a50: 2020 2020 2020 2020 7265 7475 726e 2061          return a
+00010a60: 7574 686f 7269 7479 5f69 640a 0a20 2020  uthority_id..   
+00010a70: 2064 6566 205f 6765 745f 6665 7463 6865   def _get_fetche
+00010a80: 725f 6964 2873 656c 662c 2066 6574 6368  r_id(self, fetch
+00010a90: 6572 3a20 4d65 7461 6461 7461 4665 7463  er: MetadataFetc
+00010aa0: 6865 722c 2064 622c 2063 7572 293a 0a20  her, db, cur):. 
+00010ab0: 2020 2020 2020 2066 6574 6368 6572 5f69         fetcher_i
+00010ac0: 6420 3d20 6462 2e6d 6574 6164 6174 615f  d = db.metadata_
+00010ad0: 6665 7463 6865 725f 6765 745f 6964 2866  fetcher_get_id(f
+00010ae0: 6574 6368 6572 2e6e 616d 652c 2066 6574  etcher.name, fet
+00010af0: 6368 6572 2e76 6572 7369 6f6e 2c20 6375  cher.version, cu
+00010b00: 7229 0a20 2020 2020 2020 2069 6620 6e6f  r).        if no
+00010b10: 7420 6665 7463 6865 725f 6964 3a0a 2020  t fetcher_id:.  
+00010b20: 2020 2020 2020 2020 2020 7261 6973 6520            raise 
+00010b30: 556e 6b6e 6f77 6e4d 6574 6164 6174 6146  UnknownMetadataF
+00010b40: 6574 6368 6572 2873 7472 2866 6574 6368  etcher(str(fetch
+00010b50: 6572 2929 0a20 2020 2020 2020 2072 6574  er)).        ret
+00010b60: 7572 6e20 6665 7463 6865 725f 6964 0a0a  urn fetcher_id..
+00010b70: 2020 2020 2323 2323 2323 2323 2323 2323      ############
+00010b80: 2323 2323 2323 2323 2323 2323 230a 2020  #############.  
+00010b90: 2020 2320 4f62 6a65 6374 4465 6c65 7469    # ObjectDeleti
+00010ba0: 6f6e 496e 7465 7266 6163 650a 2020 2020  onInterface.    
+00010bb0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00010bc0: 2323 2323 2323 2323 230a 0a20 2020 2040  #########..    @
+00010bd0: 6462 5f74 7261 6e73 6163 7469 6f6e 2829  db_transaction()
+00010be0: 0a20 2020 2064 6566 206f 626a 6563 745f  .    def object_
+00010bf0: 6465 6c65 7465 280a 2020 2020 2020 2020  delete(.        
+00010c00: 7365 6c66 2c20 7377 6869 6473 3a20 4c69  self, swhids: Li
+00010c10: 7374 5b45 7874 656e 6465 6453 5748 4944  st[ExtendedSWHID
+00010c20: 5d2c 202a 2c20 6462 3a20 4462 2c20 6375  ], *, db: Db, cu
+00010c30: 723d 4e6f 6e65 0a20 2020 2029 202d 3e20  r=None.    ) -> 
+00010c40: 4469 6374 5b73 7472 2c20 696e 745d 3a0a  Dict[str, int]:.
+00010c50: 2020 2020 2020 2020 2222 2244 656c 6574          """Delet
+00010c60: 6520 6f62 6a65 6374 7320 6672 6f6d 2074  e objects from t
+00010c70: 6865 2073 746f 7261 6765 0a0a 2020 2020  he storage..    
+00010c80: 2020 2020 416c 6c20 736b 6970 7065 6420      All skipped 
+00010c90: 636f 6e74 656e 7420 6f62 6a65 6374 7320  content objects 
+00010ca0: 6d61 7463 6869 6e67 2074 6865 2067 6976  matching the giv
+00010cb0: 656e 2053 5748 4944 2077 696c 6c20 6265  en SWHID will be
+00010cc0: 2072 656d 6f76 6564 2c0a 2020 2020 2020   removed,.      
+00010cd0: 2020 696e 636c 7564 696e 6720 7468 6f73    including thos
+00010ce0: 6520 7768 6f20 6861 7665 2074 6865 2073  e who have the s
+00010cf0: 616d 6520 5357 4849 4420 6475 6520 746f  ame SWHID due to
+00010d00: 2068 6173 6820 636f 6c6c 6973 696f 6e73   hash collisions
+00010d10: 2e0a 0a20 2020 2020 2020 204f 7269 6769  ...        Origi
+00010d20: 6e20 6f62 6a65 6374 7320 6172 6520 7265  n objects are re
+00010d30: 6d6f 7665 6420 616c 6f6e 6773 6964 6520  moved alongside 
+00010d40: 7468 6569 7220 6173 736f 6369 6174 6564  their associated
+00010d50: 206f 7269 6769 6e20 7669 7369 7420 616e   origin visit an
+00010d60: 640a 2020 2020 2020 2020 6f72 6967 696e  d.        origin
+00010d70: 2076 6973 6974 2073 7461 7475 7320 6f62   visit status ob
+00010d80: 6a65 6374 732e 0a0a 2020 2020 2020 2020  jects...        
+00010d90: 4172 6773 3a0a 2020 2020 2020 2020 2020  Args:.          
+00010da0: 2020 7377 6869 6473 3a20 6c69 7374 206f    swhids: list o
+00010db0: 6620 5357 4849 4420 6f66 2074 6865 206f  f SWHID of the o
+00010dc0: 626a 6563 7473 2074 6f20 7265 6d6f 7665  bjects to remove
+00010dd0: 0a0a 2020 2020 2020 2020 5265 7475 726e  ..        Return
+00010de0: 733a 0a20 2020 2020 2020 2020 2020 2053  s:.            S
+00010df0: 756d 6d61 7279 2064 6963 7420 7769 7468  ummary dict with
+00010e00: 2074 6865 2066 6f6c 6c6f 7769 6e67 206b   the following k
+00010e10: 6579 7320 616e 6420 6173 736f 6369 6174  eys and associat
+00010e20: 6564 2076 616c 7565 733a 0a0a 2020 2020  ed values:..    
+00010e30: 2020 2020 2020 2020 2020 2020 636f 6e74              cont
+00010e40: 656e 743a 6465 6c65 7465 3a20 4e75 6d62  ent:delete: Numb
+00010e50: 6572 206f 6620 636f 6e74 656e 7420 6f62  er of content ob
+00010e60: 6a65 6374 7320 7265 6d6f 7665 640a 2020  jects removed.  
+00010e70: 2020 2020 2020 2020 2020 2020 2020 636f                co
+00010e80: 6e74 656e 743a 6465 6c65 7465 3a62 7974  ntent:delete:byt
+00010e90: 6573 3a20 5375 6d20 6f66 2074 6865 2072  es: Sum of the r
+00010ea0: 656d 6f76 6564 2063 6f6e 7465 6e74 73e2  emoved contents.
+00010eb0: 8099 2064 6174 6120 6c65 6e67 7468 0a20  .. data length. 
+00010ec0: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+00010ed0: 6b69 7070 6564 5f63 6f6e 7465 6e74 3a64  kipped_content:d
+00010ee0: 656c 6574 653a 204e 756d 6265 7220 6f66  elete: Number of
+00010ef0: 2073 6b69 7070 6564 2063 6f6e 7465 6e74   skipped content
+00010f00: 206f 626a 6563 7473 2072 656d 6f76 6564   objects removed
+00010f10: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00010f20: 2064 6972 6563 746f 7279 3a64 656c 6574   directory:delet
+00010f30: 653a 204e 756d 6265 7220 6f66 2064 6972  e: Number of dir
+00010f40: 6563 746f 7279 206f 626a 6563 7473 2072  ectory objects r
+00010f50: 656d 6f76 6564 0a20 2020 2020 2020 2020  emoved.         
+00010f60: 2020 2020 2020 2072 6576 6973 696f 6e3a         revision:
+00010f70: 6465 6c65 7465 3a20 4e75 6d62 6572 206f  delete: Number o
+00010f80: 6620 7265 7669 7369 6f6e 206f 626a 6563  f revision objec
+00010f90: 7473 2072 656d 6f76 6564 0a20 2020 2020  ts removed.     
+00010fa0: 2020 2020 2020 2020 2020 2072 656c 6561             relea
+00010fb0: 7365 3a64 656c 6574 653a 204e 756d 6265  se:delete: Numbe
+00010fc0: 7220 6f66 2072 656c 6561 7365 206f 626a  r of release obj
+00010fd0: 6563 7473 2072 656d 6f76 6564 0a20 2020  ects removed.   
+00010fe0: 2020 2020 2020 2020 2020 2020 2073 6e61               sna
+00010ff0: 7073 686f 743a 6465 6c65 7465 3a20 4e75  pshot:delete: Nu
+00011000: 6d62 6572 206f 6620 736e 6170 7368 6f74  mber of snapshot
+00011010: 206f 626a 6563 7473 2072 656d 6f76 6564   objects removed
+00011020: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00011030: 206f 7269 6769 6e3a 6465 6c65 7465 3a20   origin:delete: 
+00011040: 4e75 6d62 6572 206f 6620 6f72 6967 696e  Number of origin
+00011050: 206f 626a 6563 7473 2072 656d 6f76 6564   objects removed
+00011060: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00011070: 206f 7269 6769 6e5f 7669 7369 743a 6465   origin_visit:de
+00011080: 6c65 7465 3a20 4e75 6d62 6572 206f 6620  lete: Number of 
+00011090: 6f72 6967 696e 2076 6973 6974 206f 626a  origin visit obj
+000110a0: 6563 7473 2072 656d 6f76 6564 0a20 2020  ects removed.   
+000110b0: 2020 2020 2020 2020 2020 2020 206f 7269               ori
+000110c0: 6769 6e5f 7669 7369 745f 7374 6174 7573  gin_visit_status
+000110d0: 3a64 656c 6574 653a 204e 756d 6265 7220  :delete: Number 
+000110e0: 6f66 206f 7269 6769 6e20 7669 7369 7420  of origin visit 
+000110f0: 7374 6174 7573 206f 626a 6563 7473 2072  status objects r
+00011100: 656d 6f76 6564 0a20 2020 2020 2020 2022  emoved.        "
+00011110: 2222 0a20 2020 2020 2020 206f 626a 6563  "".        objec
+00011120: 745f 726f 7773 203d 205b 0a20 2020 2020  t_rows = [.     
+00011130: 2020 2020 2020 2028 7377 6869 642e 6f62         (swhid.ob
+00011140: 6a65 6374 5f74 7970 652e 6e61 6d65 2e6c  ject_type.name.l
+00011150: 6f77 6572 2829 2c20 7377 6869 642e 6f62  ower(), swhid.ob
+00011160: 6a65 6374 5f69 6429 2066 6f72 2073 7768  ject_id) for swh
+00011170: 6964 2069 6e20 7377 6869 6473 0a20 2020  id in swhids.   
+00011180: 2020 2020 205d 0a20 2020 2020 2020 2072       ].        r
+00011190: 6574 7572 6e20 6462 2e6f 626a 6563 745f  eturn db.object_
+000111a0: 6465 6c65 7465 286f 626a 6563 745f 726f  delete(object_ro
+000111b0: 7773 290a                                ws).
```

### Comparing `swh_storage-2.4.0/swh/storage/proxies/blocking/__init__.py` & `swh_storage-2.4.1/swh/storage/proxies/blocking/__init__.py`

 * *Files identical despite different names*

### Comparing `swh_storage-2.4.0/swh/storage/proxies/blocking/cli.py` & `swh_storage-2.4.1/swh/storage/proxies/blocking/cli.py`

 * *Files 4% similar despite different names*

```diff
@@ -155,20 +155,36 @@
 
 
 def format_blocked_state(state: "BlockingState") -> str:
     return state.name.lower().replace("_", "-")
 
 
 def read_origins(file: TextIO) -> List[str]:
+    import logging
     import re
 
-    filter_re = re.compile(r"^(#|$)")
-    return [
-        line.strip() for line in file.read().split("\n") if not filter_re.match(line)
-    ]
+    filter_re = re.compile(r"^#")
+    urls = []
+
+    for line in file.readlines():
+        line = line.strip()
+
+        if not line:
+            continue
+
+        if filter_re.match(line):
+            continue
+
+        if line.endswith("/"):
+            logging.getLogger(__name__).warning(
+                "URL pattern ends with /, will only be used for exact matching"
+            )
+
+        urls.append(line)
+    return urls
 
 
 @blocking_cli_group.command(name="update-objects")
 @click.option("-m", "--message", help="an explanation for this change")
 @click.option("-f", "--file", type=click.File(), help="a file with one Origin per line")
 @click.argument("request", metavar="SLUG", type=RequestType())
 @click.argument("new-state", metavar="NEW_STATE", type=BlockedStateType())
```

### Comparing `swh_storage-2.4.0/swh/storage/proxies/blocking/db.py` & `swh_storage-2.4.1/swh/storage/proxies/blocking/db.py`

 * *Files 14% similar despite different names*

```diff
@@ -95,14 +95,58 @@
 
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
 
         self.conn.autocommit = True
 
 
+def get_urls_to_check(url: str) -> Tuple[List[str], List[str]]:
+    """Get the entries to check in the database for the given `url`, in order.
+
+    Exact matching is done on the following strings, in order:
+     - the url with any trailing slashes removed (the so-called "trimmed url");
+     - the url passed exactly;
+     - if the trimmed url ends with a dot and one of the
+       :const:`KNOWN_SUFFIXES`, the url with this suffix stripped.
+
+    The prefix matching is done by splitting the path part of the URL on
+    slashes, and successively removing the last elements.
+
+    Returns:
+      A tuple with a list of exact matches, and a list of prefix matches
+
+    """
+
+    # Generate exact strings to match against
+    exact_matches = [url]
+
+    if url.endswith("/"):
+        trimmed_url = url.rstrip("/")
+        exact_matches.insert(0, trimmed_url)
+    else:
+        trimmed_url = url
+
+    if "." in trimmed_url:
+        stripped_url, suffix = trimmed_url.rsplit(".", 1)
+        if suffix in KNOWN_SUFFIXES:
+            exact_matches.append(stripped_url)
+
+    # Generate prefixes to match against
+    parsed_url = urlparse(trimmed_url)
+    base_url = f"{parsed_url.scheme}://{parsed_url.netloc}"
+
+    prefix_matches = []
+
+    split_path = parsed_url.path.lstrip("/").split("/")
+    for i in range(1, len(split_path) + 1):
+        prefix_matches.append("/".join([base_url] + split_path[: len(split_path) - i]))
+
+    return exact_matches, prefix_matches
+
+
 class BlockingAdmin(BlockingDb):
     def create_request(self, slug: str, reason: str) -> BlockingRequest:
         """Record a new blocking request
 
         Arguments:
           slug: human-readable unique identifier for the request
           reason: free-form text recording why the request was made
@@ -407,73 +451,31 @@
 
         If the given url matches a set of registered blocking rules, return the
         most appropriate one. Otherwise, return None.
 
         Log the blocking event in the database (log only a matching events).
         """
         logging.debug("url: %s", url)
-        cur = self.cursor()
         statsd.increment(METRIC_QUERY_TOTAL, 1)
 
-        # first look for an exact match on
-        # 1. the given URL
-        # 2. the trimmed URL (if trailing /)
-        # 3. the extension-less URL (if any)
-        checked_urls = [url]
-        if url.endswith("/"):
-            trimmed_url = url.rstrip("/")
-            checked_urls.insert(0, trimmed_url)
-        else:
-            trimmed_url = url
-        if trimmed_url.rsplit(".", 1)[-1] in KNOWN_SUFFIXES:
-            checked_urls.append(trimmed_url.rsplit(".", 1)[0])
-        logger.debug("Checked urls for exact match: %s", checked_urls)
+        exact_matches, prefix_matches = get_urls_to_check(url)
 
+        cur = self.cursor()
         psycopg2.extras.execute_values(
             cur,
             """
             SELECT url_match, request, state
             FROM blocked_origin
             INNER JOIN (VALUES %s) v(url_match)
             USING (url_match)
             ORDER BY char_length(url_match) DESC LIMIT 1
             """,
-            ((_url,) for _url in checked_urls),
+            ((_url,) for _url in exact_matches + prefix_matches),
         )
         row = cur.fetchone()
-        if not row:
-            # no exact match found, check for prefix matches on sub-path urls
-            checked_urls = []
-            parsed_url = urlparse(trimmed_url)
-            path = parsed_url.path
-            baseurl = f"{parsed_url.scheme}://{parsed_url.netloc}"
-            checked_urls.append(baseurl)
-            for path_element in path.split("/"):
-                if path_element:
-                    checked_urls.append(f"{checked_urls[-1]}/{path_element}")
-
-            logger.debug("Checked urls for prefix match: %s", checked_urls)
-            # the request below is a bit tricky; joining on something like
-            #    ON v.url LIKE blocked_origin.url_match || '/%%'
-            # works but prevent pg from using the btree index.
-            # This below should allow pg to use index. This trick (suggested by
-            # vlorentz) is to know that '0' is the next character after '/'.
-            psycopg2.extras.execute_values(
-                cur,
-                """
-                SELECT url_match, request, state
-                FROM blocked_origin
-                INNER JOIN (VALUES %s) v(url)
-                ON   v.url > blocked_origin.url_match || '/'
-                 AND v.url < blocked_origin.url_match || '0'
-                ORDER BY char_length(url_match) DESC LIMIT 1
-                """,
-                ((_url,) for _url in checked_urls),
-            )
-            row = cur.fetchone()
 
         if row:
             url_match, request_id, state = row
             status = BlockingStatus(
                 state=BlockingState[state.upper()], request=request_id
             )
             logger.debug("Matching status for %s: %s", url_match, status)
```

### Comparing `swh_storage-2.4.0/swh/storage/proxies/blocking/sql/30-schema.sql` & `swh_storage-2.4.1/swh/storage/proxies/blocking/sql/30-schema.sql`

 * *Files identical despite different names*

### Comparing `swh_storage-2.4.0/swh/storage/proxies/buffer.py` & `swh_storage-2.4.1/swh/storage/proxies/buffer.py`

 * *Files identical despite different names*

### Comparing `swh_storage-2.4.0/swh/storage/proxies/counter.py` & `swh_storage-2.4.1/swh/storage/proxies/counter.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 # See top-level LICENSE file for more information
 
 
 from typing import Callable
 
 from swh.counters import get_counters
 from swh.counters.interface import CountersInterface
-from swh.storage import get_storage
+from swh.storage import StorageSpec, get_storage
 from swh.storage.interface import StorageInterface
 
 OBJECT_TYPES = [
     "content",
     "directory",
     "snapshot",
     "origin_visit_status",
@@ -43,15 +43,15 @@
             url: http://counters.internal.staging.swh.network:5011/
           storage:
             cls: remote
             url: http://storage.internal.staging.swh.network:5002/
 
     """
 
-    def __init__(self, counters, storage):
+    def __init__(self, counters, storage: StorageSpec) -> None:
         self.counters: CountersInterface = get_counters(**counters)
         self.storage: StorageInterface = get_storage(**storage)
 
     def __getattr__(self, key):
         if key == "storage":
             raise AttributeError(key)
         if key.endswith("_add"):
```

### Comparing `swh_storage-2.4.0/swh/storage/proxies/filter.py` & `swh_storage-2.4.1/swh/storage/proxies/filter.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     Content,
     Directory,
     Release,
     Revision,
     Sha1Git,
     SkippedContent,
 )
-from swh.storage import get_storage
+from swh.storage import StorageSpec, get_storage
 from swh.storage.interface import HashDict, StorageInterface
 
 
 class FilteringProxyStorage:
     """Filtering Storage implementation. This is in charge of transparently
        filtering out known objects prior to adding them to storage.
 
@@ -32,15 +32,15 @@
             cls: remote
             url: http://storage.internal.staging.swh.network:5002/
 
     """
 
     object_types = ["content", "skipped_content", "directory", "revision", "release"]
 
-    def __init__(self, storage):
+    def __init__(self, storage: StorageSpec) -> None:
         self.storage: StorageInterface = get_storage(**storage)
 
     def __getattr__(self, key):
         if key == "storage":
             raise AttributeError(key)
         return getattr(self.storage, key)
```

### Comparing `swh_storage-2.4.0/swh/storage/proxies/masking/__init__.py` & `swh_storage-2.4.1/swh/storage/proxies/masking/__init__.py`

 * *Files 19% similar despite different names*

```diff
@@ -2,30 +2,43 @@
 # See the AUTHORS file at the top-level directory of this distribution
 # License: GNU General Public License version 3, or any later version
 # See top-level LICENSE file for more information
 
 from contextlib import contextmanager
 import functools
 import inspect
-from typing import Any, Callable, Dict, Iterable, Iterator, List, Optional, Union
+import itertools
+from typing import (
+    Any,
+    Callable,
+    Dict,
+    Iterable,
+    Iterator,
+    List,
+    Optional,
+    TypeVar,
+    Union,
+)
 
+import attr
 import psycopg2.pool
 
-from swh.core.api.classes import PagedResult
+from swh.core.utils import grouper
 from swh.model.hashutil import MultiHash
-from swh.model.model import Origin
+from swh.model.model import Origin, Person, Release, Revision, Sha1Git
 from swh.model.swhids import ExtendedObjectType, ExtendedSWHID
 from swh.storage import get_storage
 from swh.storage.exc import MaskedObjectException
-from swh.storage.interface import HashDict, Sha1, StorageInterface
+from swh.storage.interface import HashDict, PagedResult, Sha1, StorageInterface, TResult
 from swh.storage.metrics import DifferentialTimer
 from swh.storage.proxies.masking.db import MaskedStatus
 
 from .db import MaskingQuery
 
+BATCH_SIZE = 1024
 MASKING_OVERHEAD_METRIC = "swh_storage_masking_overhead_seconds"
 
 
 def get_datastore(cls, db):
     assert cls == "postgresql"
     from .db import MaskingAdmin
 
@@ -188,15 +201,14 @@
             masked = q.swhids_are_masked(swhids)
 
         if masked:
             raise MaskedObjectException(masked)
 
     def __getattr__(self, key):
         method = None
-
         if key in self._methods_by_name:
             method = self._methods_by_name[key](key)
         else:
             suffix = key.rsplit("_", 1)[-1]
 
             if suffix in self._methods_by_suffix:
                 method = self._methods_by_suffix[suffix](key)
@@ -229,15 +241,14 @@
             "raw_extrinsic_metadata_get": self._getter_pagedresult,
             "origin_visit_get_with_statuses": self._getter_pagedresult,
             "origin_visit_status_get": self._getter_pagedresult,
             # Returns a list of (optional) objects
             "origin_get_by_sha1": self._getter_list,
             "content_find": self._getter_list,
             "skipped_content_find": self._getter_list,
-            "revision_log": self._getter_list,
             "revision_shortlog": self._getter_list,
             "extid_get_from_target": self._getter_list,
             "raw_extrinsic_metadata_get_by_ids": self._getter_list,
             # Filter arguments
             "directory_entry_get_by_path": self._getter_filtering_arguments,
             "directory_get_entries": self._getter_filtering_arguments,
             "directory_get_raw_manifest": self._getter_filtering_arguments,
@@ -427,25 +438,27 @@
                 self._raise_if_masked_result(method_name, result)
 
                 return result
 
         return newf
 
     def _raise_if_masked_result_in_list(
-        self, method_name: str, results: Iterable[Any]
-    ) -> None:
+        self, method_name: str, results: Iterable[TResult]
+    ) -> List[TResult]:
         """Raise a :exc:`MaskedObjectException` if any non-:const:`None` object
         in ``results`` is masked."""
         result_swhids = set()
+        results = list(results)
         for result in results:
             if result is not None:
                 result_swhids.update(self._get_swhids_in_result(method_name, result))
 
         if result_swhids:
             self._raise_if_masked_swhids(list(result_swhids))
+        return results
 
     def _getter_list(
         self,
         method_name: str,
     ):
         """Handle methods returning a list (or a generator) of optional objects,
         raising :exc:`MaskedObjectException` for all the masked objects in the
@@ -477,7 +490,166 @@
                     results = method(*args, **kwargs)
 
                 self._raise_if_masked_result_in_list(method_name, results.results)
 
                 return results
 
         return newf
+
+    # Patching proxy feature set
+
+    TRevision = TypeVar("TRevision", Revision, Optional[Revision])
+
+    def _apply_revision_display_names(
+        self, revisions: List[TRevision]
+    ) -> List[TRevision]:
+        emails = set()
+        for rev in revisions:
+            if (
+                rev is not None
+                and rev.author is not None
+                and rev.author.email  # ignore None or empty email addresses
+            ):
+                emails.add(rev.author.email)
+            if (
+                rev is not None
+                and rev.committer is not None
+                and rev.committer.email  # ignore None or empty email addresses
+            ):
+                emails.add(rev.committer.email)
+
+        with self._masking_query() as q:
+            display_names = q.display_name(list(emails))
+
+        # Short path for the common case
+        if not display_names:
+            return revisions
+
+        persons: Dict[Optional[bytes], Person] = {
+            email: Person.from_fullname(display_name)
+            for (email, display_name) in display_names.items()
+        }
+
+        return [
+            None
+            if revision is None
+            else attr.evolve(
+                revision,
+                author=revision.author
+                if revision.author is None
+                else persons.get(revision.author.email, revision.author),
+                committer=revision.committer
+                if revision.committer is None
+                else persons.get(revision.committer.email, revision.committer),
+            )
+            for revision in revisions
+        ]
+
+    TRelease = TypeVar("TRelease", Release, Optional[Release])
+
+    def _apply_release_display_names(self, releases: List[TRelease]) -> List[TRelease]:
+        emails = set()
+        for rel in releases:
+            if (
+                rel is not None
+                and rel.author is not None
+                and rel.author.email  # ignore None or empty email addresses
+            ):
+                emails.add(rel.author.email)
+
+        with self._masking_query() as q:
+            display_names = q.display_name(list(emails))
+        # Short path for the common case
+        if not display_names:
+            return releases
+
+        persons: Dict[Optional[bytes], Person] = {
+            email: Person.from_fullname(display_name)
+            for (email, display_name) in display_names.items()
+        }
+
+        return [
+            None
+            if release is None
+            else attr.evolve(
+                release,
+                author=release.author
+                if release.author is None
+                else persons.get(release.author.email, release.author),
+            )
+            for release in releases
+        ]
+
+    def revision_get(
+        self, revision_ids: List[Sha1Git], ignore_displayname: bool = False
+    ) -> List[Optional[Revision]]:
+        revisions = self.storage.revision_get(revision_ids)
+        self._raise_if_masked_result_in_list("revision_get", revisions)
+        return self._apply_revision_display_names(revisions)
+
+    def revision_log(
+        self,
+        revisions: List[Sha1Git],
+        ignore_displayname: bool = False,
+        limit: Optional[int] = None,
+    ) -> Iterable[Optional[Dict[str, Any]]]:
+        revision_batches = grouper(
+            self.storage.revision_log(revisions, limit=limit), BATCH_SIZE
+        )
+        yield from map(
+            Revision.to_dict,
+            itertools.chain.from_iterable(
+                self._apply_revision_display_names(
+                    self._raise_if_masked_result_in_list(
+                        "revision_log", list(map(Revision.from_dict, revision_batch))
+                    )
+                )
+                for revision_batch in revision_batches
+            ),
+        )
+
+    def revision_get_partition(
+        self,
+        partition_id: int,
+        nb_partitions: int,
+        page_token: Optional[str] = None,
+        limit: int = 1000,
+    ) -> PagedResult[Revision]:
+        page: PagedResult[Revision] = self.storage.revision_get_partition(
+            partition_id, nb_partitions, page_token, limit
+        )
+        return PagedResult(
+            results=self._apply_revision_display_names(
+                self._raise_if_masked_result_in_list(
+                    "revision_get_parition", page.results
+                )
+            ),
+            next_page_token=page.next_page_token,
+        )
+
+    def release_get(
+        self, releases: List[Sha1Git], ignore_displayname: bool = False
+    ) -> List[Optional[Release]]:
+        return self._apply_release_display_names(
+            self._raise_if_masked_result_in_list(
+                "release_get", self.storage.release_get(releases)
+            )
+        )
+
+    def release_get_partition(
+        self,
+        partition_id: int,
+        nb_partitions: int,
+        page_token: Optional[str] = None,
+        limit: int = 1000,
+    ) -> PagedResult[Release]:
+        page = self.storage.release_get_partition(
+            partition_id, nb_partitions, page_token, limit
+        )
+        return PagedResult(
+            results=self._apply_release_display_names(
+                self._raise_if_masked_result_in_list(
+                    "release_get_partition", page.results
+                )
+            ),
+            next_page_token=page.next_page_token,
+        )
```

### Comparing `swh_storage-2.4.0/swh/storage/proxies/masking/cli.py` & `swh_storage-2.4.1/swh/storage/proxies/masking/cli.py`

 * *Files identical despite different names*

### Comparing `swh_storage-2.4.0/swh/storage/proxies/masking/db.py` & `swh_storage-2.4.1/swh/storage/proxies/masking/db.py`

 * *Files 8% similar despite different names*

```diff
@@ -84,17 +84,28 @@
 @attr.s
 class MaskedObject:
     request_slug = attr.ib(type=str)
     swhid = attr.ib(type=ExtendedSWHID)
     state = attr.ib(type=MaskedState)
 
 
+@attr.s
+class DisplayName:
+    """A request for masking a set of objects"""
+
+    original_email = attr.ib(type=bytes)
+    """Email on revision/release objects to match before applying the display name"""
+
+    display_name = attr.ib(type=bytes)
+    """Full name, usually of the form ``Name <email>``, used for display queries"""
+
+
 class MaskingDb(BaseDb):
     # we started with 192, because this used to be part of the main storage db
-    current_version = 193
+    current_version = 194
 
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
 
         self.conn.autocommit = True
 
 
@@ -325,14 +336,28 @@
             raise RequestNotFound(request_id)
 
         res = cur.fetchone()
         assert res is not None, "PostgreSQL returned an inconsistent result"
 
         return MaskingRequestHistory(request=request_id, date=res[0], message=message)
 
+    def set_display_name(self, original_email: bytes, display_name: bytes) -> None:
+        """Updates the display name of the person identified by the email address."""
+        cur = self.cursor()
+
+        cur.execute(
+            """
+            INSERT INTO display_name (original_email, display_name)
+            VALUES (%s, %s)
+            ON CONFLICT (original_email) DO UPDATE
+            SET display_name=EXCLUDED.display_name
+            """,
+            (original_email, display_name),
+        )
+
     def get_history(self, request_id: UUID) -> List[MaskingRequestHistory]:
         """Get the history of a given request.
 
         Raises: :exc:`RequestNotFound` if the request if not found.
         """
         cur = self.cursor()
 
@@ -402,14 +427,37 @@
                 MaskedStatus(request=request_id, state=MaskedState[state.upper()])
             )
 
         if ret:
             statsd.increment(METRIC_MASKED_TOTAL, len(ret))
         return ret
 
+    def display_name(self, original_emails: List[bytes]) -> Dict[bytes, bytes]:
+        """Returns the display name of the person identified by each ``original_email``,
+        if any.
+        """
+        cur = self.cursor()
+
+        ret: Dict[bytes, bytes] = {}
+
+        for original_email, display_name in psycopg2.extras.execute_values(
+            cur,
+            """
+            SELECT original_email, display_name
+            FROM display_name
+            INNER JOIN (VALUES %s) v(original_email)
+            USING (original_email)
+            """,
+            [(email,) for email in original_emails],
+            fetch=True,
+        ):
+            ret[original_email] = display_name
+
+        return ret
+
     def iter_masked_swhids(self) -> Iterator[Tuple[ExtendedSWHID, List[MaskedStatus]]]:
         """Returns the complete list of masked SWHIDs.
 
         SWHIDs are guaranteed to be unique in the iterator.
 
         Yields:
             For each masked object, its SWHID and a list of :class:`MaskedStatus`
```

### Comparing `swh_storage-2.4.0/swh/storage/proxies/masking/sql/30-schema.sql` & `swh_storage-2.4.1/swh/storage/proxies/masking/sql/30-schema.sql`

 * *Files 22% similar despite different names*

```diff
@@ -37,7 +37,20 @@
 );
 
 comment on table masked_object is 'All the objects known to be affected by a specific request';
 comment on column masked_object.object_id is 'The object_id part of the object''s SWHID';
 comment on column masked_object.object_type is 'The object_type part of the object''s SWHID';
 comment on column masked_object.request is 'Reference to the affecting request';
 comment on column masked_object.state is 'The degree to which the object is masked as a result of the request';
+
+
+
+-- Used only by the patching proxy, not the masking proxy
+
+create table if not exists display_name (
+  original_email bytea not null primary key,
+  display_name bytea not null
+);
+
+comment on table display_name is 'Map from revision/release email to current full name';
+comment on column display_name.original_email is 'Email on revision/release objects to match before applying the display name';
+comment on column display_name.display_name is 'Full name, usually of the form `Name <email>, used for display queries';
```

### Comparing `swh_storage-2.4.0/swh/storage/proxies/record_references.py` & `swh_storage-2.4.1/swh/storage/proxies/record_references.py`

 * *Files identical despite different names*

### Comparing `swh_storage-2.4.0/swh/storage/proxies/retry.py` & `swh_storage-2.4.1/swh/storage/proxies/retry.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 import logging
 import traceback
 
 from tenacity import RetryCallState, retry, stop_after_attempt, wait_random_exponential
 from tenacity.wait import wait_base
 
 from swh.core.api import TransientRemoteException
-from swh.storage import get_storage
+from swh.storage import StorageSpec, get_storage
 from swh.storage.exc import NonRetryableException
 from swh.storage.interface import StorageInterface
 
 logger = logging.getLogger(__name__)
 
 
 def should_retry_adding(retry_state: RetryCallState) -> bool:
@@ -85,15 +85,15 @@
 
 class RetryingProxyStorage:
     """Storage implementation which retries adding objects when it specifically
     fails (hash collision, integrity error).
 
     """
 
-    def __init__(self, storage):
+    def __init__(self, storage: StorageSpec):
         self.storage: StorageInterface = get_storage(**storage)
         for attribute_name in dir(StorageInterface):
             if attribute_name.startswith("_"):
                 continue
             attribute = getattr(self.storage, attribute_name)
             if hasattr(attribute, "__call__"):
                 setattr(
```

### Comparing `swh_storage-2.4.0/swh/storage/proxies/tenacious.py` & `swh_storage-2.4.1/swh/storage/proxies/tenacious.py`

 * *Files identical despite different names*

### Comparing `swh_storage-2.4.0/swh/storage/proxies/validate.py` & `swh_storage-2.4.1/swh/storage/proxies/validate.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 # See top-level LICENSE file for more information
 
 
 from typing import Dict, Iterable, List
 
 from swh.model.hashutil import MultiHash, hash_to_bytes, hash_to_hex
 from swh.model.model import Content, Directory, Release, Revision, Snapshot
-from swh.storage import get_storage
+from swh.storage import StorageSpec, get_storage
 from swh.storage.exc import StorageArgumentException
 from swh.storage.interface import StorageInterface
 
 
 class ValidatingProxyStorage:
     """Proxy for storage classes, which checks inserted objects have a correct hash.
 
@@ -24,15 +24,15 @@
           cls: validate
           storage:
             cls: remote
             url: http://storage.internal.staging.swh.network:5002/
 
     """
 
-    def __init__(self, storage):
+    def __init__(self, storage: StorageSpec) -> None:
         self.storage: StorageInterface = get_storage(**storage)
 
     def __getattr__(self, key):
         if key == "storage":
             raise AttributeError(key)
         return getattr(self.storage, key)
```

### Comparing `swh_storage-2.4.0/swh/storage/pytest_plugin.py` & `swh_storage-2.4.1/swh/storage/pytest_plugin.py`

 * *Files identical despite different names*

### Comparing `swh_storage-2.4.0/swh/storage/replay.py` & `swh_storage-2.4.1/swh/storage/replay.py`

 * *Files identical despite different names*

### Comparing `swh_storage-2.4.0/swh/storage/sql/10-superuser-init.sql` & `swh_storage-2.4.1/swh/storage/sql/10-superuser-init.sql`

 * *Files identical despite different names*

### Comparing `swh_storage-2.4.0/swh/storage/sql/15-flavor.sql` & `swh_storage-2.4.1/swh/storage/sql/15-flavor.sql`

 * *Files identical despite different names*

### Comparing `swh_storage-2.4.0/swh/storage/sql/20-enums.sql` & `swh_storage-2.4.1/swh/storage/sql/20-enums.sql`

 * *Files identical despite different names*

### Comparing `swh_storage-2.4.0/swh/storage/sql/30-schema.sql` & `swh_storage-2.4.1/swh/storage/sql/30-schema.sql`

 * *Files identical despite different names*

### Comparing `swh_storage-2.4.0/swh/storage/sql/40-funcs.sql` & `swh_storage-2.4.1/swh/storage/sql/40-funcs.sql`

 * *Files identical despite different names*

### Comparing `swh_storage-2.4.0/swh/storage/sql/60-indexes.sql` & `swh_storage-2.4.1/swh/storage/sql/60-indexes.sql`

 * *Files identical despite different names*

### Comparing `swh_storage-2.4.0/swh/storage/sql/logical_replication/replication_source.sql` & `swh_storage-2.4.1/swh/storage/sql/logical_replication/replication_source.sql`

 * *Files identical despite different names*

### Comparing `swh_storage-2.4.0/swh/storage/sql/upgrades/015.sql` & `swh_storage-2.4.1/swh/storage/sql/upgrades/015.sql`

 * *Files identical despite different names*

### Comparing `swh_storage-2.4.0/swh/storage/sql/upgrades/016.sql` & `swh_storage-2.4.1/swh/storage/sql/upgrades/016.sql`

 * *Files identical despite different names*

### Comparing `swh_storage-2.4.0/swh/storage/sql/upgrades/017.sql` & `swh_storage-2.4.1/swh/storage/sql/upgrades/017.sql`

 * *Files identical despite different names*

### Comparing `swh_storage-2.4.0/swh/storage/sql/upgrades/018.sql` & `swh_storage-2.4.1/swh/storage/sql/upgrades/018.sql`

 * *Files identical despite different names*

### Comparing `swh_storage-2.4.0/swh/storage/sql/upgrades/019.sql` & `swh_storage-2.4.1/swh/storage/sql/upgrades/019.sql`

 * *Files identical despite different names*

### Comparing `swh_storage-2.4.0/swh/storage/sql/upgrades/020.sql` & `swh_storage-2.4.1/swh/storage/sql/upgrades/020.sql`

 * *Files identical despite different names*

### Comparing `swh_storage-2.4.0/swh/storage/sql/upgrades/021.sql` & `swh_storage-2.4.1/swh/storage/sql/upgrades/021.sql`

 * *Files identical despite different names*

### Comparing `swh_storage-2.4.0/swh/storage/sql/upgrades/022.sql` & `swh_storage-2.4.1/swh/storage/sql/upgrades/022.sql`

 * *Files identical despite different names*

### Comparing `swh_storage-2.4.0/swh/storage/sql/upgrades/023.sql` & `swh_storage-2.4.1/swh/storage/sql/upgrades/023.sql`

 * *Files identical despite different names*

### Comparing `swh_storage-2.4.0/swh/storage/sql/upgrades/024.sql` & `swh_storage-2.4.1/swh/storage/sql/upgrades/024.sql`

 * *Files identical despite different names*

### Comparing `swh_storage-2.4.0/swh/storage/sql/upgrades/025.sql` & `swh_storage-2.4.1/swh/storage/sql/upgrades/025.sql`

 * *Files identical despite different names*

### Comparing `swh_storage-2.4.0/swh/storage/sql/upgrades/026.sql` & `swh_storage-2.4.1/swh/storage/sql/upgrades/026.sql`

 * *Files identical despite different names*

### Comparing `swh_storage-2.4.0/swh/storage/sql/upgrades/027.sql` & `swh_storage-2.4.1/swh/storage/sql/upgrades/027.sql`

 * *Files identical despite different names*

### Comparing `swh_storage-2.4.0/swh/storage/sql/upgrades/028.sql` & `swh_storage-2.4.1/swh/storage/sql/upgrades/028.sql`

 * *Files identical despite different names*

### Comparing `swh_storage-2.4.0/swh/storage/sql/upgrades/029.sql` & `swh_storage-2.4.1/swh/storage/sql/upgrades/029.sql`

 * *Files identical despite different names*

### Comparing `swh_storage-2.4.0/swh/storage/sql/upgrades/030.sql` & `swh_storage-2.4.1/swh/storage/sql/upgrades/030.sql`

 * *Files identical despite different names*

### Comparing `swh_storage-2.4.0/swh/storage/sql/upgrades/032.sql` & `swh_storage-2.4.1/swh/storage/sql/upgrades/032.sql`

 * *Files identical despite different names*

### Comparing `swh_storage-2.4.0/swh/storage/sql/upgrades/033.sql` & `swh_storage-2.4.1/swh/storage/sql/upgrades/033.sql`

 * *Files identical despite different names*

### Comparing `swh_storage-2.4.0/swh/storage/sql/upgrades/034.sql` & `swh_storage-2.4.1/swh/storage/sql/upgrades/034.sql`

 * *Files identical despite different names*

### Comparing `swh_storage-2.4.0/swh/storage/sql/upgrades/035.sql` & `swh_storage-2.4.1/swh/storage/sql/upgrades/035.sql`

 * *Files identical despite different names*

### Comparing `swh_storage-2.4.0/swh/storage/sql/upgrades/036.sql` & `swh_storage-2.4.1/swh/storage/sql/upgrades/036.sql`

 * *Files identical despite different names*

### Comparing `swh_storage-2.4.0/swh/storage/sql/upgrades/037.sql` & `swh_storage-2.4.1/swh/storage/sql/upgrades/037.sql`

 * *Files identical despite different names*

### Comparing `swh_storage-2.4.0/swh/storage/sql/upgrades/038.sql` & `swh_storage-2.4.1/swh/storage/sql/upgrades/038.sql`

 * *Files identical despite different names*

### Comparing `swh_storage-2.4.0/swh/storage/sql/upgrades/039.sql` & `swh_storage-2.4.1/swh/storage/sql/upgrades/039.sql`

 * *Files identical despite different names*

### Comparing `swh_storage-2.4.0/swh/storage/sql/upgrades/040.sql` & `swh_storage-2.4.1/swh/storage/sql/upgrades/040.sql`

 * *Files identical despite different names*

### Comparing `swh_storage-2.4.0/swh/storage/sql/upgrades/041.sql` & `swh_storage-2.4.1/swh/storage/sql/upgrades/041.sql`

 * *Files identical despite different names*

### Comparing `swh_storage-2.4.0/swh/storage/sql/upgrades/042.sql` & `swh_storage-2.4.1/swh/storage/sql/upgrades/042.sql`

 * *Files identical despite different names*

### Comparing `swh_storage-2.4.0/swh/storage/sql/upgrades/043.sql` & `swh_storage-2.4.1/swh/storage/sql/upgrades/043.sql`

 * *Files identical despite different names*

### Comparing `swh_storage-2.4.0/swh/storage/sql/upgrades/044.sql` & `swh_storage-2.4.1/swh/storage/sql/upgrades/044.sql`

 * *Files identical despite different names*

### Comparing `swh_storage-2.4.0/swh/storage/sql/upgrades/046.sql` & `swh_storage-2.4.1/swh/storage/sql/upgrades/046.sql`

 * *Files identical despite different names*

### Comparing `swh_storage-2.4.0/swh/storage/sql/upgrades/047.sql` & `swh_storage-2.4.1/swh/storage/sql/upgrades/047.sql`

 * *Files identical despite different names*

### Comparing `swh_storage-2.4.0/swh/storage/sql/upgrades/048.sql` & `swh_storage-2.4.1/swh/storage/sql/upgrades/048.sql`

 * *Files identical despite different names*

### Comparing `swh_storage-2.4.0/swh/storage/sql/upgrades/049.sql` & `swh_storage-2.4.1/swh/storage/sql/upgrades/049.sql`

 * *Files identical despite different names*

### Comparing `swh_storage-2.4.0/swh/storage/sql/upgrades/050.sql` & `swh_storage-2.4.1/swh/storage/sql/upgrades/050.sql`

 * *Files identical despite different names*

### Comparing `swh_storage-2.4.0/swh/storage/sql/upgrades/051.sql` & `swh_storage-2.4.1/swh/storage/sql/upgrades/051.sql`

 * *Files identical despite different names*

### Comparing `swh_storage-2.4.0/swh/storage/sql/upgrades/052.sql` & `swh_storage-2.4.1/swh/storage/sql/upgrades/052.sql`

 * *Files identical despite different names*

### Comparing `swh_storage-2.4.0/swh/storage/sql/upgrades/053.sql` & `swh_storage-2.4.1/swh/storage/sql/upgrades/053.sql`

 * *Files identical despite different names*

### Comparing `swh_storage-2.4.0/swh/storage/sql/upgrades/054.sql` & `swh_storage-2.4.1/swh/storage/sql/upgrades/054.sql`

 * *Files identical despite different names*

### Comparing `swh_storage-2.4.0/swh/storage/sql/upgrades/055.sql` & `swh_storage-2.4.1/swh/storage/sql/upgrades/055.sql`

 * *Files identical despite different names*

### Comparing `swh_storage-2.4.0/swh/storage/sql/upgrades/056.sql` & `swh_storage-2.4.1/swh/storage/sql/upgrades/056.sql`

 * *Files identical despite different names*

### Comparing `swh_storage-2.4.0/swh/storage/sql/upgrades/057.sql` & `swh_storage-2.4.1/swh/storage/sql/upgrades/057.sql`

 * *Files identical despite different names*

### Comparing `swh_storage-2.4.0/swh/storage/sql/upgrades/058.sql` & `swh_storage-2.4.1/swh/storage/sql/upgrades/058.sql`

 * *Files identical despite different names*

### Comparing `swh_storage-2.4.0/swh/storage/sql/upgrades/059.sql` & `swh_storage-2.4.1/swh/storage/sql/upgrades/059.sql`

 * *Files identical despite different names*

### Comparing `swh_storage-2.4.0/swh/storage/sql/upgrades/060.sql` & `swh_storage-2.4.1/swh/storage/sql/upgrades/060.sql`

 * *Files identical despite different names*

### Comparing `swh_storage-2.4.0/swh/storage/sql/upgrades/061.sql` & `swh_storage-2.4.1/swh/storage/sql/upgrades/061.sql`

 * *Files identical despite different names*

### Comparing `swh_storage-2.4.0/swh/storage/sql/upgrades/062.sql` & `swh_storage-2.4.1/swh/storage/sql/upgrades/062.sql`

 * *Files identical despite different names*

### Comparing `swh_storage-2.4.0/swh/storage/sql/upgrades/063.sql` & `swh_storage-2.4.1/swh/storage/sql/upgrades/063.sql`

 * *Files identical despite different names*

### Comparing `swh_storage-2.4.0/swh/storage/sql/upgrades/064.sql` & `swh_storage-2.4.1/swh/storage/sql/upgrades/064.sql`

 * *Files identical despite different names*

### Comparing `swh_storage-2.4.0/swh/storage/sql/upgrades/065.sql` & `swh_storage-2.4.1/swh/storage/sql/upgrades/065.sql`

 * *Files identical despite different names*

### Comparing `swh_storage-2.4.0/swh/storage/sql/upgrades/067.sql` & `swh_storage-2.4.1/swh/storage/sql/upgrades/067.sql`

 * *Files identical despite different names*

### Comparing `swh_storage-2.4.0/swh/storage/sql/upgrades/068.sql` & `swh_storage-2.4.1/swh/storage/sql/upgrades/068.sql`

 * *Files identical despite different names*

### Comparing `swh_storage-2.4.0/swh/storage/sql/upgrades/069.sql` & `swh_storage-2.4.1/swh/storage/sql/upgrades/069.sql`

 * *Files identical despite different names*

### Comparing `swh_storage-2.4.0/swh/storage/sql/upgrades/071.sql` & `swh_storage-2.4.1/swh/storage/sql/upgrades/071.sql`

 * *Files identical despite different names*

### Comparing `swh_storage-2.4.0/swh/storage/sql/upgrades/072.sql` & `swh_storage-2.4.1/swh/storage/sql/upgrades/072.sql`

 * *Files identical despite different names*

### Comparing `swh_storage-2.4.0/swh/storage/sql/upgrades/073.sql` & `swh_storage-2.4.1/swh/storage/sql/upgrades/073.sql`

 * *Files identical despite different names*

### Comparing `swh_storage-2.4.0/swh/storage/sql/upgrades/074.sql` & `swh_storage-2.4.1/swh/storage/sql/upgrades/074.sql`

 * *Files identical despite different names*

### Comparing `swh_storage-2.4.0/swh/storage/sql/upgrades/075.sql` & `swh_storage-2.4.1/swh/storage/sql/upgrades/075.sql`

 * *Files identical despite different names*

### Comparing `swh_storage-2.4.0/swh/storage/sql/upgrades/076.sql` & `swh_storage-2.4.1/swh/storage/sql/upgrades/076.sql`

 * *Files identical despite different names*

### Comparing `swh_storage-2.4.0/swh/storage/sql/upgrades/077.sql` & `swh_storage-2.4.1/swh/storage/sql/upgrades/077.sql`

 * *Files identical despite different names*

### Comparing `swh_storage-2.4.0/swh/storage/sql/upgrades/078.sql` & `swh_storage-2.4.1/swh/storage/sql/upgrades/078.sql`

 * *Files identical despite different names*

### Comparing `swh_storage-2.4.0/swh/storage/sql/upgrades/079.sql` & `swh_storage-2.4.1/swh/storage/sql/upgrades/079.sql`

 * *Files identical despite different names*

### Comparing `swh_storage-2.4.0/swh/storage/sql/upgrades/080.sql` & `swh_storage-2.4.1/swh/storage/sql/upgrades/080.sql`

 * *Files identical despite different names*

### Comparing `swh_storage-2.4.0/swh/storage/sql/upgrades/081.sql` & `swh_storage-2.4.1/swh/storage/sql/upgrades/081.sql`

 * *Files identical despite different names*

### Comparing `swh_storage-2.4.0/swh/storage/sql/upgrades/082.sql` & `swh_storage-2.4.1/swh/storage/sql/upgrades/082.sql`

 * *Files identical despite different names*

### Comparing `swh_storage-2.4.0/swh/storage/sql/upgrades/083.sql` & `swh_storage-2.4.1/swh/storage/sql/upgrades/083.sql`

 * *Files identical despite different names*

### Comparing `swh_storage-2.4.0/swh/storage/sql/upgrades/084.sql` & `swh_storage-2.4.1/swh/storage/sql/upgrades/084.sql`

 * *Files identical despite different names*

### Comparing `swh_storage-2.4.0/swh/storage/sql/upgrades/085.sql` & `swh_storage-2.4.1/swh/storage/sql/upgrades/085.sql`

 * *Files identical despite different names*

### Comparing `swh_storage-2.4.0/swh/storage/sql/upgrades/086.sql` & `swh_storage-2.4.1/swh/storage/sql/upgrades/086.sql`

 * *Files identical despite different names*

### Comparing `swh_storage-2.4.0/swh/storage/sql/upgrades/087.sql` & `swh_storage-2.4.1/swh/storage/sql/upgrades/087.sql`

 * *Files identical despite different names*

### Comparing `swh_storage-2.4.0/swh/storage/sql/upgrades/088.sql` & `swh_storage-2.4.1/swh/storage/sql/upgrades/088.sql`

 * *Files identical despite different names*

### Comparing `swh_storage-2.4.0/swh/storage/sql/upgrades/089.sql` & `swh_storage-2.4.1/swh/storage/sql/upgrades/089.sql`

 * *Files identical despite different names*

### Comparing `swh_storage-2.4.0/swh/storage/sql/upgrades/090.sql` & `swh_storage-2.4.1/swh/storage/sql/upgrades/090.sql`

 * *Files identical despite different names*

### Comparing `swh_storage-2.4.0/swh/storage/sql/upgrades/091.sql` & `swh_storage-2.4.1/swh/storage/sql/upgrades/091.sql`

 * *Files identical despite different names*

### Comparing `swh_storage-2.4.0/swh/storage/sql/upgrades/092.sql` & `swh_storage-2.4.1/swh/storage/sql/upgrades/092.sql`

 * *Files identical despite different names*

### Comparing `swh_storage-2.4.0/swh/storage/sql/upgrades/093.sql` & `swh_storage-2.4.1/swh/storage/sql/upgrades/093.sql`

 * *Files identical despite different names*

### Comparing `swh_storage-2.4.0/swh/storage/sql/upgrades/094.sql` & `swh_storage-2.4.1/swh/storage/sql/upgrades/094.sql`

 * *Files identical despite different names*

### Comparing `swh_storage-2.4.0/swh/storage/sql/upgrades/095.sql` & `swh_storage-2.4.1/swh/storage/sql/upgrades/095.sql`

 * *Files identical despite different names*

### Comparing `swh_storage-2.4.0/swh/storage/sql/upgrades/096.sql` & `swh_storage-2.4.1/swh/storage/sql/upgrades/096.sql`

 * *Files identical despite different names*

### Comparing `swh_storage-2.4.0/swh/storage/sql/upgrades/097.sql` & `swh_storage-2.4.1/swh/storage/sql/upgrades/097.sql`

 * *Files identical despite different names*

### Comparing `swh_storage-2.4.0/swh/storage/sql/upgrades/099.sql` & `swh_storage-2.4.1/swh/storage/sql/upgrades/099.sql`

 * *Files identical despite different names*

### Comparing `swh_storage-2.4.0/swh/storage/sql/upgrades/100.sql` & `swh_storage-2.4.1/swh/storage/sql/upgrades/100.sql`

 * *Files identical despite different names*

### Comparing `swh_storage-2.4.0/swh/storage/sql/upgrades/101.sql` & `swh_storage-2.4.1/swh/storage/sql/upgrades/101.sql`

 * *Files identical despite different names*

### Comparing `swh_storage-2.4.0/swh/storage/sql/upgrades/102.sql` & `swh_storage-2.4.1/swh/storage/sql/upgrades/102.sql`

 * *Files identical despite different names*

### Comparing `swh_storage-2.4.0/swh/storage/sql/upgrades/103.sql` & `swh_storage-2.4.1/swh/storage/sql/upgrades/103.sql`

 * *Files identical despite different names*

### Comparing `swh_storage-2.4.0/swh/storage/sql/upgrades/104.sql` & `swh_storage-2.4.1/swh/storage/sql/upgrades/104.sql`

 * *Files identical despite different names*

### Comparing `swh_storage-2.4.0/swh/storage/sql/upgrades/105.sql` & `swh_storage-2.4.1/swh/storage/sql/upgrades/105.sql`

 * *Files identical despite different names*

### Comparing `swh_storage-2.4.0/swh/storage/sql/upgrades/106.sql` & `swh_storage-2.4.1/swh/storage/sql/upgrades/106.sql`

 * *Files identical despite different names*

### Comparing `swh_storage-2.4.0/swh/storage/sql/upgrades/107.sql` & `swh_storage-2.4.1/swh/storage/sql/upgrades/107.sql`

 * *Files identical despite different names*

### Comparing `swh_storage-2.4.0/swh/storage/sql/upgrades/108.sql` & `swh_storage-2.4.1/swh/storage/sql/upgrades/108.sql`

 * *Files identical despite different names*

### Comparing `swh_storage-2.4.0/swh/storage/sql/upgrades/109.sql` & `swh_storage-2.4.1/swh/storage/sql/upgrades/109.sql`

 * *Files identical despite different names*

### Comparing `swh_storage-2.4.0/swh/storage/sql/upgrades/110.sql` & `swh_storage-2.4.1/swh/storage/sql/upgrades/110.sql`

 * *Files identical despite different names*

### Comparing `swh_storage-2.4.0/swh/storage/sql/upgrades/111.sql` & `swh_storage-2.4.1/swh/storage/sql/upgrades/111.sql`

 * *Files identical despite different names*

### Comparing `swh_storage-2.4.0/swh/storage/sql/upgrades/112.sql` & `swh_storage-2.4.1/swh/storage/sql/upgrades/112.sql`

 * *Files identical despite different names*

### Comparing `swh_storage-2.4.0/swh/storage/sql/upgrades/113.sql` & `swh_storage-2.4.1/swh/storage/sql/upgrades/113.sql`

 * *Files identical despite different names*

### Comparing `swh_storage-2.4.0/swh/storage/sql/upgrades/114.sql` & `swh_storage-2.4.1/swh/storage/sql/upgrades/114.sql`

 * *Files identical despite different names*

### Comparing `swh_storage-2.4.0/swh/storage/sql/upgrades/115.sql` & `swh_storage-2.4.1/swh/storage/sql/upgrades/115.sql`

 * *Files identical despite different names*

### Comparing `swh_storage-2.4.0/swh/storage/sql/upgrades/117.sql` & `swh_storage-2.4.1/swh/storage/sql/upgrades/117.sql`

 * *Files identical despite different names*

### Comparing `swh_storage-2.4.0/swh/storage/sql/upgrades/118.sql` & `swh_storage-2.4.1/swh/storage/sql/upgrades/118.sql`

 * *Files identical despite different names*

### Comparing `swh_storage-2.4.0/swh/storage/sql/upgrades/119.sql` & `swh_storage-2.4.1/swh/storage/sql/upgrades/119.sql`

 * *Files identical despite different names*

### Comparing `swh_storage-2.4.0/swh/storage/sql/upgrades/120.sql` & `swh_storage-2.4.1/swh/storage/sql/upgrades/120.sql`

 * *Files identical despite different names*

### Comparing `swh_storage-2.4.0/swh/storage/sql/upgrades/123.sql` & `swh_storage-2.4.1/swh/storage/sql/upgrades/123.sql`

 * *Files identical despite different names*

### Comparing `swh_storage-2.4.0/swh/storage/sql/upgrades/124.sql` & `swh_storage-2.4.1/swh/storage/sql/upgrades/124.sql`

 * *Files identical despite different names*

### Comparing `swh_storage-2.4.0/swh/storage/sql/upgrades/125.sql` & `swh_storage-2.4.1/swh/storage/sql/upgrades/125.sql`

 * *Files identical despite different names*

### Comparing `swh_storage-2.4.0/swh/storage/sql/upgrades/127.sql` & `swh_storage-2.4.1/swh/storage/sql/upgrades/127.sql`

 * *Files identical despite different names*

### Comparing `swh_storage-2.4.0/swh/storage/sql/upgrades/128.sql` & `swh_storage-2.4.1/swh/storage/sql/upgrades/128.sql`

 * *Files identical despite different names*

### Comparing `swh_storage-2.4.0/swh/storage/sql/upgrades/129.sql` & `swh_storage-2.4.1/swh/storage/sql/upgrades/129.sql`

 * *Files identical despite different names*

### Comparing `swh_storage-2.4.0/swh/storage/sql/upgrades/130.sql` & `swh_storage-2.4.1/swh/storage/sql/upgrades/130.sql`

 * *Files identical despite different names*

### Comparing `swh_storage-2.4.0/swh/storage/sql/upgrades/134.sql` & `swh_storage-2.4.1/swh/storage/sql/upgrades/134.sql`

 * *Files identical despite different names*

### Comparing `swh_storage-2.4.0/swh/storage/sql/upgrades/136.sql` & `swh_storage-2.4.1/swh/storage/sql/upgrades/136.sql`

 * *Files identical despite different names*

### Comparing `swh_storage-2.4.0/swh/storage/sql/upgrades/137.sql` & `swh_storage-2.4.1/swh/storage/sql/upgrades/137.sql`

 * *Files identical despite different names*

### Comparing `swh_storage-2.4.0/swh/storage/sql/upgrades/138.sql` & `swh_storage-2.4.1/swh/storage/sql/upgrades/138.sql`

 * *Files identical despite different names*

### Comparing `swh_storage-2.4.0/swh/storage/sql/upgrades/139.sql` & `swh_storage-2.4.1/swh/storage/sql/upgrades/139.sql`

 * *Files identical despite different names*

### Comparing `swh_storage-2.4.0/swh/storage/sql/upgrades/143.sql` & `swh_storage-2.4.1/swh/storage/sql/upgrades/143.sql`

 * *Files identical despite different names*

### Comparing `swh_storage-2.4.0/swh/storage/sql/upgrades/146.sql` & `swh_storage-2.4.1/swh/storage/sql/upgrades/146.sql`

 * *Files identical despite different names*

### Comparing `swh_storage-2.4.0/swh/storage/sql/upgrades/147.sql` & `swh_storage-2.4.1/swh/storage/sql/upgrades/147.sql`

 * *Files identical despite different names*

### Comparing `swh_storage-2.4.0/swh/storage/sql/upgrades/148.sql` & `swh_storage-2.4.1/swh/storage/sql/upgrades/148.sql`

 * *Files identical despite different names*

### Comparing `swh_storage-2.4.0/swh/storage/sql/upgrades/149.sql` & `swh_storage-2.4.1/swh/storage/sql/upgrades/149.sql`

 * *Files identical despite different names*

### Comparing `swh_storage-2.4.0/swh/storage/sql/upgrades/150.sql` & `swh_storage-2.4.1/swh/storage/sql/upgrades/150.sql`

 * *Files identical despite different names*

### Comparing `swh_storage-2.4.0/swh/storage/sql/upgrades/154.sql` & `swh_storage-2.4.1/swh/storage/sql/upgrades/154.sql`

 * *Files identical despite different names*

### Comparing `swh_storage-2.4.0/swh/storage/sql/upgrades/155.sql` & `swh_storage-2.4.1/swh/storage/sql/upgrades/155.sql`

 * *Files identical despite different names*

### Comparing `swh_storage-2.4.0/swh/storage/sql/upgrades/156.sql` & `swh_storage-2.4.1/swh/storage/sql/upgrades/156.sql`

 * *Files identical despite different names*

### Comparing `swh_storage-2.4.0/swh/storage/sql/upgrades/157.sql` & `swh_storage-2.4.1/swh/storage/sql/upgrades/157.sql`

 * *Files identical despite different names*

### Comparing `swh_storage-2.4.0/swh/storage/sql/upgrades/158.sql` & `swh_storage-2.4.1/swh/storage/sql/upgrades/158.sql`

 * *Files identical despite different names*

### Comparing `swh_storage-2.4.0/swh/storage/sql/upgrades/159.sql` & `swh_storage-2.4.1/swh/storage/sql/upgrades/159.sql`

 * *Files identical despite different names*

### Comparing `swh_storage-2.4.0/swh/storage/sql/upgrades/160.sql` & `swh_storage-2.4.1/swh/storage/sql/upgrades/160.sql`

 * *Files identical despite different names*

### Comparing `swh_storage-2.4.0/swh/storage/sql/upgrades/161.sql` & `swh_storage-2.4.1/swh/storage/sql/upgrades/161.sql`

 * *Files identical despite different names*

### Comparing `swh_storage-2.4.0/swh/storage/sql/upgrades/162.sql` & `swh_storage-2.4.1/swh/storage/sql/upgrades/162.sql`

 * *Files identical despite different names*

### Comparing `swh_storage-2.4.0/swh/storage/sql/upgrades/163.sql` & `swh_storage-2.4.1/swh/storage/sql/upgrades/163.sql`

 * *Files identical despite different names*

### Comparing `swh_storage-2.4.0/swh/storage/sql/upgrades/167.sql` & `swh_storage-2.4.1/swh/storage/sql/upgrades/167.sql`

 * *Files identical despite different names*

### Comparing `swh_storage-2.4.0/swh/storage/sql/upgrades/168.sql` & `swh_storage-2.4.1/swh/storage/sql/upgrades/168.sql`

 * *Files identical despite different names*

### Comparing `swh_storage-2.4.0/swh/storage/sql/upgrades/169.sql` & `swh_storage-2.4.1/swh/storage/sql/upgrades/169.sql`

 * *Files identical despite different names*

### Comparing `swh_storage-2.4.0/swh/storage/sql/upgrades/170.sql` & `swh_storage-2.4.1/swh/storage/sql/upgrades/170.sql`

 * *Files identical despite different names*

### Comparing `swh_storage-2.4.0/swh/storage/sql/upgrades/171.sql` & `swh_storage-2.4.1/swh/storage/sql/upgrades/171.sql`

 * *Files identical despite different names*

### Comparing `swh_storage-2.4.0/swh/storage/sql/upgrades/172.sql` & `swh_storage-2.4.1/swh/storage/sql/upgrades/172.sql`

 * *Files identical despite different names*

### Comparing `swh_storage-2.4.0/swh/storage/sql/upgrades/173.sql` & `swh_storage-2.4.1/swh/storage/sql/upgrades/173.sql`

 * *Files identical despite different names*

### Comparing `swh_storage-2.4.0/swh/storage/sql/upgrades/175.sql` & `swh_storage-2.4.1/swh/storage/sql/upgrades/175.sql`

 * *Files identical despite different names*

### Comparing `swh_storage-2.4.0/swh/storage/sql/upgrades/176.sql` & `swh_storage-2.4.1/swh/storage/sql/upgrades/176.sql`

 * *Files identical despite different names*

### Comparing `swh_storage-2.4.0/swh/storage/sql/upgrades/179.sql` & `swh_storage-2.4.1/swh/storage/sql/upgrades/179.sql`

 * *Files identical despite different names*

### Comparing `swh_storage-2.4.0/swh/storage/sql/upgrades/180.sql` & `swh_storage-2.4.1/swh/storage/sql/upgrades/180.sql`

 * *Files identical despite different names*

### Comparing `swh_storage-2.4.0/swh/storage/sql/upgrades/181.sql` & `swh_storage-2.4.1/swh/storage/sql/upgrades/181.sql`

 * *Files identical despite different names*

### Comparing `swh_storage-2.4.0/swh/storage/sql/upgrades/182.sql` & `swh_storage-2.4.1/swh/storage/sql/upgrades/182.sql`

 * *Files identical despite different names*

### Comparing `swh_storage-2.4.0/swh/storage/sql/upgrades/183.sql` & `swh_storage-2.4.1/swh/storage/sql/upgrades/183.sql`

 * *Files identical despite different names*

### Comparing `swh_storage-2.4.0/swh/storage/sql/upgrades/184.sql` & `swh_storage-2.4.1/swh/storage/sql/upgrades/184.sql`

 * *Files identical despite different names*

### Comparing `swh_storage-2.4.0/swh/storage/sql/upgrades/185.sql` & `swh_storage-2.4.1/swh/storage/sql/upgrades/185.sql`

 * *Files identical despite different names*

### Comparing `swh_storage-2.4.0/swh/storage/sql/upgrades/187.sql` & `swh_storage-2.4.1/swh/storage/sql/upgrades/187.sql`

 * *Files identical despite different names*

### Comparing `swh_storage-2.4.0/swh/storage/sql/upgrades/188.sql` & `swh_storage-2.4.1/swh/storage/sql/upgrades/188.sql`

 * *Files identical despite different names*

### Comparing `swh_storage-2.4.0/swh/storage/sql/upgrades/189.sql` & `swh_storage-2.4.1/swh/storage/sql/upgrades/189.sql`

 * *Files identical despite different names*

### Comparing `swh_storage-2.4.0/swh/storage/sql/upgrades/190.sql` & `swh_storage-2.4.1/swh/storage/sql/upgrades/190.sql`

 * *Files identical despite different names*

### Comparing `swh_storage-2.4.0/swh/storage/sql/upgrades/191.sql` & `swh_storage-2.4.1/swh/storage/sql/upgrades/191.sql`

 * *Files identical despite different names*

### Comparing `swh_storage-2.4.0/swh/storage/sql/upgrades/193.sql` & `swh_storage-2.4.1/swh/storage/sql/upgrades/193.sql`

 * *Files identical despite different names*

### Comparing `swh_storage-2.4.0/swh/storage/tests/algos/test_diff.py` & `swh_storage-2.4.1/swh/storage/tests/algos/test_diff.py`

 * *Files identical despite different names*

### Comparing `swh_storage-2.4.0/swh/storage/tests/algos/test_dir_iterator.py` & `swh_storage-2.4.1/swh/storage/tests/algos/test_dir_iterator.py`

 * *Files identical despite different names*

### Comparing `swh_storage-2.4.0/swh/storage/tests/algos/test_directory.py` & `swh_storage-2.4.1/swh/storage/tests/algos/test_directory.py`

 * *Files identical despite different names*

### Comparing `swh_storage-2.4.0/swh/storage/tests/algos/test_discovery.py` & `swh_storage-2.4.1/swh/storage/tests/algos/test_discovery.py`

 * *Files identical despite different names*

### Comparing `swh_storage-2.4.0/swh/storage/tests/algos/test_origin.py` & `swh_storage-2.4.1/swh/storage/tests/algos/test_origin.py`

 * *Files identical despite different names*

### Comparing `swh_storage-2.4.0/swh/storage/tests/algos/test_revisions_walker.py` & `swh_storage-2.4.1/swh/storage/tests/algos/test_revisions_walker.py`

 * *Files identical despite different names*

### Comparing `swh_storage-2.4.0/swh/storage/tests/algos/test_snapshot.py` & `swh_storage-2.4.1/swh/storage/tests/algos/test_snapshot.py`

 * *Files 5% similar despite different names*

```diff
@@ -174,14 +174,68 @@
     assert actual_snapshot.id == complete_snapshot.id
     assert len(actual_snapshot.branches.values()) == 1
 
     with pytest.raises(ValueError, match="branches_count must be a positive integer"):
         snapshot_get_latest(swh_storage, origin.url, branches_count="something-wrong")
 
 
+def test_snapshot_get_latest_for_visit_type(swh_storage, sample_data):
+    origin = sample_data.origin
+    swh_storage.origin_add(sample_data.origins)
+
+    visit1, visit2 = sample_data.origin_visits[:2]
+    visit1 = visit1.evolve(type="git")
+    visit2 = visit2.evolve(type="git-checkout")
+    assert visit1.origin == visit2.origin == origin.url
+
+    ov1, ov2 = swh_storage.origin_visit_add([visit1, visit2])
+
+    simple_snapshot = sample_data.snapshots[0]
+    complete_snapshot = sample_data.snapshots[2]
+    swh_storage.snapshot_add([simple_snapshot, complete_snapshot])
+
+    swh_storage.origin_visit_status_add(
+        [
+            OriginVisitStatus(
+                origin=origin.url,
+                visit=ov1.visit,
+                date=visit1.date,
+                status="full",
+                snapshot=complete_snapshot.id,
+            )
+        ]
+    )
+
+    swh_storage.origin_visit_status_add(
+        [
+            OriginVisitStatus(
+                origin=origin.url,
+                visit=ov2.visit,
+                date=visit2.date,
+                status="full",
+                snapshot=simple_snapshot.id,
+            )
+        ]
+    )
+
+    git_snapshot = snapshot_get_latest(
+        swh_storage,
+        origin.url,
+        visit_type="git",
+    )
+    assert git_snapshot == complete_snapshot
+
+    git_checkout_snapshot = snapshot_get_latest(
+        swh_storage,
+        origin.url,
+        visit_type="git-checkout",
+    )
+    assert git_checkout_snapshot == simple_snapshot
+
+
 def test_snapshot_id_get_from_revision(swh_storage, sample_data):
     origin = sample_data.origin
     swh_storage.origin_add([origin])
 
     date_visit2 = now()
     visit1, visit2 = sample_data.origin_visits[:2]
     assert visit1.origin == origin.url
```

### Comparing `swh_storage-2.4.0/swh/storage/tests/blocking/conftest.py` & `swh_storage-2.4.1/swh/storage/tests/blocking/conftest.py`

 * *Files identical despite different names*

### Comparing `swh_storage-2.4.0/swh/storage/tests/blocking/test_cli.py` & `swh_storage-2.4.1/swh/storage/tests/blocking/test_cli.py`

 * *Files identical despite different names*

### Comparing `swh_storage-2.4.0/swh/storage/tests/blocking/test_db.py` & `swh_storage-2.4.1/swh/storage/tests/blocking/test_db.py`

 * *Files 24% similar despite different names*

```diff
@@ -12,18 +12,87 @@
 from swh.storage.proxies.blocking.db import (
     BlockingAdmin,
     BlockingQuery,
     BlockingState,
     BlockingStatus,
     DuplicateRequest,
     RequestNotFound,
+    get_urls_to_check,
 )
 from swh.storage.tests.storage_data import StorageData
 
 
+@pytest.mark.parametrize(
+    "url,exact,prefix",
+    [
+        pytest.param(
+            "https://github.com/user1/test1.git",
+            [
+                "https://github.com/user1/test1.git",
+                "https://github.com/user1/test1",
+            ],
+            ["https://github.com/user1", "https://github.com"],
+            id="known-suffix-git",
+        ),
+        pytest.param(
+            "https://foss.heptapod.net/user1/test1.hg",
+            [
+                "https://foss.heptapod.net/user1/test1.hg",
+                "https://foss.heptapod.net/user1/test1",
+            ],
+            ["https://foss.heptapod.net/user1", "https://foss.heptapod.net"],
+            id="known-suffix-hg",
+        ),
+        pytest.param(
+            "svn+ssh://example.com/svnroot/users/user1/test1.svn",
+            [
+                "svn+ssh://example.com/svnroot/users/user1/test1.svn",
+                "svn+ssh://example.com/svnroot/users/user1/test1",
+            ],
+            [
+                "svn+ssh://example.com/svnroot/users/user1",
+                "svn+ssh://example.com/svnroot/users",
+                "svn+ssh://example.com/svnroot",
+                "svn+ssh://example.com",
+            ],
+            id="known-suffix-svn",
+        ),
+        pytest.param(
+            "https://github.com/user1/test1",
+            [
+                "https://github.com/user1/test1",
+            ],
+            ["https://github.com/user1", "https://github.com"],
+            id="bare",
+        ),
+        pytest.param(
+            "https://github.com/user1/test1/",
+            [
+                "https://github.com/user1/test1",
+                "https://github.com/user1/test1/",
+            ],
+            ["https://github.com/user1", "https://github.com"],
+            id="slash",
+        ),
+        pytest.param(
+            "https://github.com/user1/test1.git/",
+            [
+                "https://github.com/user1/test1.git",
+                "https://github.com/user1/test1.git/",
+                "https://github.com/user1/test1",
+            ],
+            ["https://github.com/user1", "https://github.com"],
+            id="slash-suffix",
+        ),
+    ],
+)
+def test_get_urls_to_check(url, exact, prefix):
+    assert get_urls_to_check(url) == (exact, prefix)
+
+
 def test_db_version(blocking_admin: BlockingAdmin):
     dbmodule, dbversion, dbflavor = get_database_info(blocking_admin.conn.dsn)
     assert dbmodule == "storage.proxies.blocking"
     assert dbversion == BlockingAdmin.current_version
     assert dbflavor is None
```

### Comparing `swh_storage-2.4.0/swh/storage/tests/blocking/test_proxy.py` & `swh_storage-2.4.1/swh/storage/tests/blocking/test_proxy.py`

 * *Files identical despite different names*

### Comparing `swh_storage-2.4.0/swh/storage/tests/blocking/test_proxy_blocking.py` & `swh_storage-2.4.1/swh/storage/tests/blocking/test_proxy_blocking.py`

 * *Files identical despite different names*

### Comparing `swh_storage-2.4.0/swh/storage/tests/blocking/test_proxy_no_blocking.py` & `swh_storage-2.4.1/swh/storage/tests/blocking/test_proxy_no_blocking.py`

 * *Files identical despite different names*

### Comparing `swh_storage-2.4.0/swh/storage/tests/conftest.py` & `swh_storage-2.4.1/swh/storage/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `swh_storage-2.4.0/swh/storage/tests/masking/test_cli.py` & `swh_storage-2.4.1/swh/storage/tests/masking/test_cli.py`

 * *Files identical despite different names*

### Comparing `swh_storage-2.4.0/swh/storage/tests/masking/test_db.py` & `swh_storage-2.4.1/swh/storage/tests/masking/test_db.py`

 * *Files 6% similar despite different names*

```diff
@@ -251,14 +251,28 @@
     for swhid in visible:
         del expected[swhid]
 
     assert masking_query.swhids_are_masked(all_swhids) == expected
     assert dict(masking_query.iter_masked_swhids()) == expected
 
 
+def test_set_display_name(masking_admin: MaskingAdmin, masking_query: MaskingQuery):
+    assert masking_query.display_name([b"author1@example.com"]) == {}
+    assert masking_query.display_name([b"author2@example.com"]) == {}
+
+    masking_admin.set_display_name(
+        b"author1@example.com", b"author2 <author2@example.com>"
+    )
+
+    assert masking_query.display_name([b"author1@example.com"]) == {
+        b"author1@example.com": b"author2 <author2@example.com>"
+    }
+    assert masking_query.display_name([b"author2@example.com"]) == {}
+
+
 def test_query_metrics(
     masking_admin: MaskingAdmin, masking_query: MaskingQuery, mocker
 ):
     increment = mocker.patch("swh.core.statsd.statsd.increment")
 
     # Create a request
     request = masking_admin.create_request(slug="foo", reason="bar")
```

### Comparing `swh_storage-2.4.0/swh/storage/tests/masking/test_proxy.py` & `swh_storage-2.4.1/swh/storage/tests/masking/test_proxy.py`

 * *Files 2% similar despite different names*

```diff
@@ -33,31 +33,14 @@
 
 
 def now() -> datetime.datetime:
     return datetime.datetime.now(tz=datetime.timezone.utc)
 
 
 @pytest.fixture
-def swh_storage_backend_config():
-    return {
-        "cls": "memory",
-        "journal_writer": {
-            "cls": "memory",
-        },
-    }
-
-
-@pytest.fixture
-def swh_storage(masking_db_postgresql, swh_storage_backend):
-    return MaskingProxyStorage(
-        masking_db=masking_db_postgresql.info.dsn, storage=swh_storage_backend
-    )
-
-
-@pytest.fixture
 def set_object_visibility(masking_admin):
     # Create a request
     request = masking_admin.create_request(slug="foo", reason="bar")
 
     def set_visibility(objects: Iterable[ExtendedSWHID], new_state: MaskedState):
         masking_admin.set_object_state(
             request_id=request.id,
@@ -400,15 +383,15 @@
     )
 
     # Getting one entry in the log still works
     assert list(swh_storage.revision_log([StorageData.revision2.id], limit=1))
 
     # But the parent is properly masked
     assert_masked_objects_raise(
-        lambda: swh_storage.revision_log([StorageData.revision2.id], limit=2),
+        lambda: list(swh_storage.revision_log([StorageData.revision2.id], limit=2)),
         [StorageData.revision.swhid().to_extended()],
         set_object_visibility,
     )
 
 
 def test_revision_shortlog(swh_storage, set_object_visibility):
     # revision2 has one parent, revision
@@ -422,15 +405,17 @@
     )
 
     # Getting one entry in the log still works
     assert list(swh_storage.revision_shortlog([StorageData.revision2.id], limit=1))
 
     # But the parent is properly masked
     assert_masked_objects_raise(
-        lambda: swh_storage.revision_shortlog([StorageData.revision2.id], limit=2),
+        lambda: list(
+            swh_storage.revision_shortlog([StorageData.revision2.id], limit=2)
+        ),
         [StorageData.revision.swhid().to_extended()],
         set_object_visibility,
     )
 
 
 def test_revision_get_partition(swh_storage, set_object_visibility):
     revisions = [
```

### Comparing `swh_storage-2.4.0/swh/storage/tests/masking/test_proxy_masking.py` & `swh_storage-2.4.1/swh/storage/tests/masking/test_proxy_masking.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,25 +9,14 @@
 
 from swh.storage.exc import MaskedObjectException
 from swh.storage.proxies.masking import MaskingProxyStorage
 from swh.storage.proxies.masking.db import MaskedState
 from swh.storage.tests.storage_data import StorageData
 from swh.storage.tests.test_in_memory import TestInMemoryStorage as _TestStorage
 
-
-@pytest.fixture
-def swh_storage_backend_config():
-    yield {
-        "cls": "memory",
-        "journal_writer": {
-            "cls": "memory",
-        },
-    }
-
-
 MASKED_SWHIDS = {
     StorageData.content.swhid().to_extended(),
     StorageData.directory.swhid().to_extended(),
     StorageData.revision.swhid().to_extended(),
     StorageData.release.swhid().to_extended(),
     StorageData.snapshot.swhid().to_extended(),
     StorageData.origin.swhid(),
```

### Comparing `swh_storage-2.4.0/swh/storage/tests/masking/test_proxy_no_masking.py` & `swh_storage-2.4.1/swh/storage/tests/masking/test_proxy_passthrough.py`

 * *Files 17% similar despite different names*

```diff
@@ -6,28 +6,14 @@
 
 import pytest
 
 from swh.storage.proxies.masking import MaskingProxyStorage
 from swh.storage.tests.test_in_memory import TestInMemoryStorage as _TestStorage
 
 
-@pytest.fixture
-def swh_storage_backend_config():
-    yield {
-        "cls": "memory",
-        "journal_writer": {
-            "cls": "memory",
-        },
-    }
-
-
-@pytest.fixture
-def swh_storage(masking_db_postgresql, swh_storage_backend):
-    return MaskingProxyStorage(
-        masking_db=masking_db_postgresql.info.dsn, storage=swh_storage_backend
-    )
-
-
 class TestStorage(_TestStorage):
     @pytest.mark.xfail(reason="typing.Protocol instance check is annoying")
     def test_types(self, *args, **kwargs):
         super().test_types(*args, **kwargs)
+
+    def test_storage_type(self, swh_storage):
+        assert isinstance(swh_storage, MaskingProxyStorage)
```

### Comparing `swh_storage-2.4.0/swh/storage/tests/migrate_extrinsic_metadata/test_cran.py` & `swh_storage-2.4.1/swh/storage/tests/migrate_extrinsic_metadata/test_cran.py`

 * *Files identical despite different names*

### Comparing `swh_storage-2.4.0/swh/storage/tests/migrate_extrinsic_metadata/test_debian.py` & `swh_storage-2.4.1/swh/storage/tests/migrate_extrinsic_metadata/test_debian.py`

 * *Files identical despite different names*

### Comparing `swh_storage-2.4.0/swh/storage/tests/migrate_extrinsic_metadata/test_deposit.py` & `swh_storage-2.4.1/swh/storage/tests/migrate_extrinsic_metadata/test_deposit.py`

 * *Files identical despite different names*

### Comparing `swh_storage-2.4.0/swh/storage/tests/migrate_extrinsic_metadata/test_gnu.py` & `swh_storage-2.4.1/swh/storage/tests/migrate_extrinsic_metadata/test_gnu.py`

 * *Files identical despite different names*

### Comparing `swh_storage-2.4.0/swh/storage/tests/migrate_extrinsic_metadata/test_nixguix.py` & `swh_storage-2.4.1/swh/storage/tests/migrate_extrinsic_metadata/test_nixguix.py`

 * *Files identical despite different names*

### Comparing `swh_storage-2.4.0/swh/storage/tests/migrate_extrinsic_metadata/test_npm.py` & `swh_storage-2.4.1/swh/storage/tests/migrate_extrinsic_metadata/test_npm.py`

 * *Files identical despite different names*

### Comparing `swh_storage-2.4.0/swh/storage/tests/migrate_extrinsic_metadata/test_pypi.py` & `swh_storage-2.4.1/swh/storage/tests/migrate_extrinsic_metadata/test_pypi.py`

 * *Files identical despite different names*

### Comparing `swh_storage-2.4.0/swh/storage/tests/storage_data.py` & `swh_storage-2.4.1/swh/storage/tests/storage_data.py`

 * *Files identical despite different names*

### Comparing `swh_storage-2.4.0/swh/storage/tests/storage_tests.py` & `swh_storage-2.4.1/swh/storage/tests/storage_tests.py`

 * *Files identical despite different names*

### Comparing `swh_storage-2.4.0/swh/storage/tests/test_api_client.py` & `swh_storage-2.4.1/swh/storage/tests/test_api_client.py`

 * *Files identical despite different names*

### Comparing `swh_storage-2.4.0/swh/storage/tests/test_backfill.py` & `swh_storage-2.4.1/swh/storage/tests/test_backfill.py`

 * *Files identical despite different names*

### Comparing `swh_storage-2.4.0/swh/storage/tests/test_buffer.py` & `swh_storage-2.4.1/swh/storage/tests/test_buffer.py`

 * *Files identical despite different names*

### Comparing `swh_storage-2.4.0/swh/storage/tests/test_cassandra.py` & `swh_storage-2.4.1/swh/storage/tests/test_cassandra.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,15 +24,18 @@
     TimestampWithTimezone,
 )
 from swh.storage import get_storage
 from swh.storage.cassandra.cql import BATCH_INSERT_MAX_SIZE
 import swh.storage.cassandra.model
 from swh.storage.cassandra.model import BaseRow, ContentRow, ExtIDRow
 from swh.storage.cassandra.schema import CREATE_TABLES_QUERIES, HASH_ALGORITHMS, TABLES
-from swh.storage.cassandra.storage import DIRECTORY_ENTRIES_INSERT_ALGOS
+from swh.storage.cassandra.storage import (
+    DIRECTORY_ENTRIES_INSERT_ALGOS,
+    CassandraStorage,
+)
 from swh.storage.tests.storage_data import StorageData
 from swh.storage.tests.storage_tests import (
     TestStorageGeneratedData as _TestStorageGeneratedData,
 )
 from swh.storage.tests.storage_tests import TestStorage as _TestStorage
 from swh.storage.utils import now, remove_keys
 
@@ -339,15 +342,18 @@
 
         assert called == 2
 
         # but cont2 should be filtered out
         assert actual_result == [expected_content]
 
     def test_content_get_partition_murmur3_collision(
-        self, swh_storage, mocker, sample_data
+        self,
+        swh_storage: CassandraStorage,
+        mocker,
+        sample_data,
     ):
         """The Murmur3 token is used as link from index tables to the main table; and
         non-matching contents with colliding murmur3-hash are filtered-out when reading
         the main table.
 
         This test checks the content_get_partition endpoints return all contents, even
         the collisions.
```

### Comparing `swh_storage-2.4.0/swh/storage/tests/test_cassandra_converters.py` & `swh_storage-2.4.1/swh/storage/tests/test_cassandra_converters.py`

 * *Files identical despite different names*

### Comparing `swh_storage-2.4.0/swh/storage/tests/test_cassandra_migration.py` & `swh_storage-2.4.1/swh/storage/tests/test_cassandra_migration.py`

 * *Files identical despite different names*

### Comparing `swh_storage-2.4.0/swh/storage/tests/test_cli.py` & `swh_storage-2.4.1/swh/storage/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `swh_storage-2.4.0/swh/storage/tests/test_counter.py` & `swh_storage-2.4.1/swh/storage/tests/test_counter.py`

 * *Files identical despite different names*

### Comparing `swh_storage-2.4.0/swh/storage/tests/test_exception.py` & `swh_storage-2.4.1/swh/storage/tests/test_exception.py`

 * *Files identical despite different names*

### Comparing `swh_storage-2.4.0/swh/storage/tests/test_filter.py` & `swh_storage-2.4.1/swh/storage/tests/test_filter.py`

 * *Files identical despite different names*

### Comparing `swh_storage-2.4.0/swh/storage/tests/test_in_memory.py` & `swh_storage-2.4.1/swh/storage/tests/test_in_memory.py`

 * *Files identical despite different names*

### Comparing `swh_storage-2.4.0/swh/storage/tests/test_init.py` & `swh_storage-2.4.1/swh/storage/tests/test_init.py`

 * *Files identical despite different names*

### Comparing `swh_storage-2.4.0/swh/storage/tests/test_kafka_writer.py` & `swh_storage-2.4.1/swh/storage/tests/test_kafka_writer.py`

 * *Files identical despite different names*

### Comparing `swh_storage-2.4.0/swh/storage/tests/test_metrics.py` & `swh_storage-2.4.1/swh/storage/tests/test_metrics.py`

 * *Files identical despite different names*

### Comparing `swh_storage-2.4.0/swh/storage/tests/test_postgresql.py` & `swh_storage-2.4.1/swh/storage/tests/test_postgresql.py`

 * *Files identical despite different names*

### Comparing `swh_storage-2.4.0/swh/storage/tests/test_postgresql_converters.py` & `swh_storage-2.4.1/swh/storage/tests/test_postgresql_converters.py`

 * *Files identical despite different names*

### Comparing `swh_storage-2.4.0/swh/storage/tests/test_postgresql_flavor_mirror.py` & `swh_storage-2.4.1/swh/storage/tests/test_postgresql_flavor_mirror.py`

 * *Files identical despite different names*

### Comparing `swh_storage-2.4.0/swh/storage/tests/test_postgresql_flavor_readreplica.py` & `swh_storage-2.4.1/swh/storage/tests/test_postgresql_flavor_readreplica.py`

 * *Files identical despite different names*

### Comparing `swh_storage-2.4.0/swh/storage/tests/test_pytest_plugin.py` & `swh_storage-2.4.1/swh/storage/tests/test_pytest_plugin.py`

 * *Files identical despite different names*

### Comparing `swh_storage-2.4.0/swh/storage/tests/test_record_references.py` & `swh_storage-2.4.1/swh/storage/tests/test_record_references.py`

 * *Files identical despite different names*

### Comparing `swh_storage-2.4.0/swh/storage/tests/test_replay.py` & `swh_storage-2.4.1/swh/storage/tests/test_replay.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,34 +4,36 @@
 # See top-level LICENSE file for more information
 
 import dataclasses
 import datetime
 import functools
 import logging
 import re
-from typing import Any, Container, Dict, Optional, cast
+from typing import Any, Container, Dict, Optional, Tuple, cast
 
 import attr
 import pytest
 
 from swh.journal.client import JournalClient
 from swh.journal.serializers import kafka_to_value, key_to_kafka, value_to_kafka
+from swh.journal.writer import JournalWriterInterface
 from swh.model.hashutil import MultiHash, hash_to_bytes, hash_to_hex
 from swh.model.model import Revision, RevisionType
 from swh.model.tests.swh_model_data import (
     COMMITTERS,
     DATES,
     DUPLICATE_CONTENTS,
     REVISIONS,
 )
 from swh.model.tests.swh_model_data import TEST_OBJECTS as _TEST_OBJECTS
 from swh.storage import get_storage
 from swh.storage.cassandra.model import ContentRow, SkippedContentRow
 from swh.storage.exc import StorageArgumentException
 from swh.storage.in_memory import InMemoryStorage
+from swh.storage.interface import StorageInterface
 from swh.storage.replay import ModelObjectDeserializer, process_replay_objects
 
 UTC = datetime.timezone.utc
 
 TEST_OBJECTS = _TEST_OBJECTS.copy()
 # add a revision with metadata to check this later is dropped while being replayed
 TEST_OBJECTS["revision"] = list(_TEST_OBJECTS["revision"]) + [
@@ -50,15 +52,15 @@
     ),
 ]
 WRONG_ID_REG = re.compile(
     "Object has id [0-9a-f]{40}, but it should be [0-9a-f]{40}: .*"
 )
 
 
-def nullify_ctime(obj):
+def nullify_ctime(obj: Any) -> Any:
     if isinstance(obj, (ContentRow, SkippedContentRow)):
         return dataclasses.replace(obj, ctime=None)
     else:
         return obj
 
 
 @pytest.fixture()
@@ -135,37 +137,41 @@
         logtext = record.getMessage()
         if "Colliding contents:" in logtext:
             collision += 1
 
     assert collision == 0, "No collision should be detected"
 
 
-def test_storage_replay_with_collision(replayer_storage_and_client, caplog):
+def test_storage_replay_with_collision(
+    replayer_storage_and_client: Tuple[StorageInterface, JournalClient], caplog
+):
     """Another replayer scenario with collisions.
 
     This:
     - writes objects to the topic, including colliding contents
     - replayer consumes objects from the topic and replay them
     - This drops the colliding contents from the replay when detected
 
     """
     src, replayer = replayer_storage_and_client
+    journal: JournalWriterInterface = src.journal_writer.journal  # type: ignore
+    assert journal is not None
 
     # Fill Kafka using a source storage
     nb_sent = 0
     for object_type, objects in TEST_OBJECTS.items():
         method = getattr(src, object_type + "_add")
         method(objects)
         nb_sent += len(objects)
-    src.journal_writer.journal.flush()
+    journal.flush()
 
     # Create collision in input data
     # These should not be written in the destination
-    producer = src.journal_writer.journal.producer
-    prefix = src.journal_writer.journal._prefix
+    producer = journal.producer  # type: ignore
+    prefix = journal._prefix  # type: ignore
     for content in DUPLICATE_CONTENTS:
         topic = f"{prefix}.content"
         key = content.sha1
         now = datetime.datetime.now(tz=UTC)
         content = attr.evolve(content, ctime=now)
         producer.produce(
             topic=topic,
@@ -364,15 +370,16 @@
     for obj_type, objs in TEST_OBJECTS.items():
         if obj_type in ("origin_visit", "origin_visit_status"):
             # these are unrelated with what we want to test here
             continue
         method = getattr(storage, obj_type + "_add")
         method(objs)
         nb_sent += len(objs)
-    storage.journal_writer.journal.flush()  # type: ignore[attr-defined]
+    journal: JournalWriterInterface = storage.journal_writer.journal  # type:ignore
+    journal.flush()
 
     # Fill a destination storage from Kafka, potentially using privileged topics
     dst_storage = get_storage(cls="memory")
     deserializer = ModelObjectDeserializer(
         validate=False
     )  # we cannot validate an anonymized replay
     replayer = JournalClient(
```

### Comparing `swh_storage-2.4.0/swh/storage/tests/test_retry.py` & `swh_storage-2.4.1/swh/storage/tests/test_retry.py`

 * *Files identical despite different names*

### Comparing `swh_storage-2.4.0/swh/storage/tests/test_revision_bw_compat.py` & `swh_storage-2.4.1/swh/storage/tests/test_revision_bw_compat.py`

 * *Files identical despite different names*

### Comparing `swh_storage-2.4.0/swh/storage/tests/test_serializers.py` & `swh_storage-2.4.1/swh/storage/tests/test_serializers.py`

 * *Files identical despite different names*

### Comparing `swh_storage-2.4.0/swh/storage/tests/test_server.py` & `swh_storage-2.4.1/swh/storage/tests/test_server.py`

 * *Files identical despite different names*

### Comparing `swh_storage-2.4.0/swh/storage/tests/test_storage_data.py` & `swh_storage-2.4.1/swh/storage/tests/test_storage_data.py`

 * *Files identical despite different names*

### Comparing `swh_storage-2.4.0/swh/storage/tests/test_tenacious.py` & `swh_storage-2.4.1/swh/storage/tests/test_tenacious.py`

 * *Files identical despite different names*

### Comparing `swh_storage-2.4.0/swh/storage/tests/test_utils.py` & `swh_storage-2.4.1/swh/storage/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `swh_storage-2.4.0/swh/storage/tests/test_validate.py` & `swh_storage-2.4.1/swh/storage/tests/test_validate.py`

 * *Files identical despite different names*

### Comparing `swh_storage-2.4.0/swh/storage/utils.py` & `swh_storage-2.4.1/swh/storage/utils.py`

 * *Files identical despite different names*

### Comparing `swh_storage-2.4.0/swh/storage/writer.py` & `swh_storage-2.4.1/swh/storage/writer.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # Copyright (C) 2020 The Software Heritage developers
 # See the AUTHORS file at the top-level directory of this distribution
 # License: GNU General Public License version 3, or any later version
 # See top-level LICENSE file for more information
 
-from typing import Any, Dict, Iterable
+from typing import Any, Dict, Iterable, Optional
 
 from swh.model.model import (
     Content,
     Directory,
     ExtID,
     MetadataAuthority,
     MetadataFetcher,
@@ -18,15 +18,16 @@
     Release,
     Revision,
     SkippedContent,
     Snapshot,
 )
 
 try:
-    from swh.journal.writer import get_journal_writer
+    from swh.journal.writer import JournalWriterInterface, get_journal_writer
+    from swh.journal.writer.interface import ValueProtocol
 except ImportError:
     get_journal_writer = None  # type: ignore
     # mypy limitation, see https://github.com/python/mypy/issues/1153
 
 
 def model_object_dict_sanitizer(
     object_type: str, object_dict: Dict[str, Any]
@@ -39,34 +40,35 @@
 
 class JournalWriter:
     """Journal writer storage collaborator. It's in charge of adding objects to
     the journal.
 
     """
 
-    def __init__(self, journal_writer):
+    def __init__(self, journal_writer: Optional[Dict[str, Any]]):
+        self.journal: Optional[JournalWriterInterface] = None
         if journal_writer:
             if get_journal_writer is None:
                 raise EnvironmentError(
                     "You need the swh.journal package to use the "
                     "journal_writer feature"
                 )
             self.journal = get_journal_writer(
                 value_sanitizer=model_object_dict_sanitizer, **journal_writer
             )
-        else:
-            self.journal = None
 
-    def write_addition(self, object_type, value) -> None:
+    def write_addition(self, object_type: str, object_: ValueProtocol) -> None:
         if self.journal:
-            self.journal.write_addition(object_type, value)
+            self.journal.write_addition(object_type, object_)
 
-    def write_additions(self, object_type, values) -> None:
+    def write_additions(
+        self, object_type: str, objects: Iterable[ValueProtocol]
+    ) -> None:
         if self.journal:
-            self.journal.write_additions(object_type, values)
+            self.journal.write_additions(object_type, objects)
 
     def content_add(self, contents: Iterable[Content]) -> None:
         """Add contents to the journal. Drop the data field if provided."""
         contents = [item.evolve(data=None, get_data=None) for item in contents]
         self.write_additions("content", contents)
 
     def content_update(self, contents: Iterable[Dict[str, Any]]) -> None:
```

### Comparing `swh_storage-2.4.0/swh.storage.egg-info/PKG-INFO` & `swh_storage-2.4.1/swh.storage.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: swh.storage
-Version: 2.4.0
+Version: 2.4.1
 Summary: Software Heritage storage manager
 Author-email: Software Heritage developers <swh-devel@inria.fr>
 Project-URL: Homepage, https://gitlab.softwareheritage.org/swh/devel/swh-storage
 Project-URL: Bug Reports, https://gitlab.softwareheritage.org/swh/devel/swh-storage/-/issues
 Project-URL: Funding, https://www.softwareheritage.org/donate
 Project-URL: Documentation, https://docs.softwareheritage.org/devel/swh-storage/
 Project-URL: Source, https://gitlab.softwareheritage.org/swh/devel/swh-storage.git
@@ -34,14 +34,15 @@
 Provides-Extra: testing
 Requires-Dist: hypothesis>=3.11.0; extra == "testing"
 Requires-Dist: pytest>=8.1; extra == "testing"
 Requires-Dist: pytest-mock; extra == "testing"
 Requires-Dist: swh.core[testing]>=3.0.0; extra == "testing"
 Requires-Dist: swh.model[testing]>=6.13.0; extra == "testing"
 Requires-Dist: pytz; extra == "testing"
+Requires-Dist: pytest-postgresql; extra == "testing"
 Requires-Dist: pytest-redis; extra == "testing"
 Requires-Dist: pytest-xdist; extra == "testing"
 Requires-Dist: types-python-dateutil; extra == "testing"
 Requires-Dist: types-pytz; extra == "testing"
 Requires-Dist: types-pyyaml; extra == "testing"
 Requires-Dist: types-redis; extra == "testing"
 Requires-Dist: types-requests; extra == "testing"
```

### Comparing `swh_storage-2.4.0/swh.storage.egg-info/SOURCES.txt` & `swh_storage-2.4.1/swh.storage.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -116,14 +116,15 @@
 swh/storage/proxies/masking/cli.py
 swh/storage/proxies/masking/db.py
 swh/storage/proxies/masking/sql/10-superuser-init.sql
 swh/storage/proxies/masking/sql/20-types.sql
 swh/storage/proxies/masking/sql/30-schema.sql
 swh/storage/proxies/masking/sql/60-indexes.sql
 swh/storage/proxies/masking/sql/upgrades/193.sql
+swh/storage/proxies/masking/sql/upgrades/194.sql
 swh/storage/sql/10-superuser-init.sql
 swh/storage/sql/15-flavor.sql
 swh/storage/sql/20-enums.sql
 swh/storage/sql/30-schema.sql
 swh/storage/sql/40-funcs.sql
 swh/storage/sql/60-indexes.sql
 swh/storage/sql/logical_replication/replication_source.sql
@@ -356,15 +357,16 @@
 swh/storage/tests/data/storage.yml
 swh/storage/tests/masking/__init__.py
 swh/storage/tests/masking/conftest.py
 swh/storage/tests/masking/test_cli.py
 swh/storage/tests/masking/test_db.py
 swh/storage/tests/masking/test_proxy.py
 swh/storage/tests/masking/test_proxy_masking.py
-swh/storage/tests/masking/test_proxy_no_masking.py
+swh/storage/tests/masking/test_proxy_passthrough.py
+swh/storage/tests/masking/test_proxy_patching.py
 swh/storage/tests/migrate_extrinsic_metadata/test_cran.py
 swh/storage/tests/migrate_extrinsic_metadata/test_debian.py
 swh/storage/tests/migrate_extrinsic_metadata/test_deposit.py
 swh/storage/tests/migrate_extrinsic_metadata/test_gnu.py
 swh/storage/tests/migrate_extrinsic_metadata/test_nixguix.py
 swh/storage/tests/migrate_extrinsic_metadata/test_npm.py
 swh/storage/tests/migrate_extrinsic_metadata/test_pypi.py
```

### Comparing `swh_storage-2.4.0/swh.storage.egg-info/entry_points.txt` & `swh_storage-2.4.1/swh.storage.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `swh_storage-2.4.0/tox.ini` & `swh_storage-2.4.1/tox.ini`

 * *Files identical despite different names*

