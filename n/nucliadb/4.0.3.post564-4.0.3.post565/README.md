# Comparing `tmp/nucliadb-4.0.3.post564-py3-none-any.whl.zip` & `tmp/nucliadb-4.0.3.post565-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,477 +1,477 @@
-Zip file size: 777489 bytes, number of entries: 475
--rw-r--r--  2.0 unx     1135 b- defN 24-Jun-03 12:08 migrations/0001_bootstrap.py
--rw-r--r--  2.0 unx     1177 b- defN 24-Jun-03 12:08 migrations/0002_rollover_shards.py
--rw-r--r--  2.0 unx     2436 b- defN 24-Jun-03 12:08 migrations/0003_allfields_key.py
--rw-r--r--  2.0 unx     1177 b- defN 24-Jun-03 12:08 migrations/0004_rollover_shards.py
--rw-r--r--  2.0 unx     1177 b- defN 24-Jun-03 12:08 migrations/0005_rollover_shards.py
--rw-r--r--  2.0 unx     1024 b- defN 24-Jun-03 12:08 migrations/0006_rollover_shards.py
--rw-r--r--  2.0 unx     1301 b- defN 24-Jun-03 12:08 migrations/0008_cleanup_leftover_rollover_metadata.py
--rw-r--r--  2.0 unx     1378 b- defN 24-Jun-03 12:08 migrations/0009_upgrade_relations_and_texts_to_v2.py
--rw-r--r--  2.0 unx     1610 b- defN 24-Jun-03 12:08 migrations/0010_fix_corrupt_indexes.py
--rw-r--r--  2.0 unx     1843 b- defN 24-Jun-03 12:08 migrations/0011_materialize_labelset_ids.py
--rw-r--r--  2.0 unx     1443 b- defN 24-Jun-03 12:08 migrations/0012_rollover_shards.py
--rw-r--r--  2.0 unx     1024 b- defN 24-Jun-03 12:08 migrations/0013_rollover_shards.py
--rw-r--r--  2.0 unx     1382 b- defN 24-Jun-03 12:08 migrations/0014_rollover_shards.py
--rw-r--r--  2.0 unx     1462 b- defN 24-Jun-03 12:08 migrations/0015_targeted_rollover.py
--rw-r--r--  2.0 unx     2506 b- defN 24-Jun-03 12:08 migrations/0016_upgrade_to_paragraphs_v2.py
--rw-r--r--  2.0 unx     2100 b- defN 24-Jun-03 12:08 migrations/0017_multiple_writable_shards.py
--rw-r--r--  2.0 unx     2264 b- defN 24-Jun-03 12:08 migrations/0018_purge_orphan_kbslugs.py
--rw-r--r--  2.0 unx     2506 b- defN 24-Jun-03 12:08 migrations/0019_upgrade_to_paragraphs_v3.py
--rw-r--r--  2.0 unx     3271 b- defN 24-Jun-03 12:08 migrations/0020_drain_nodes_from_cluster.py
--rw-r--r--  2.0 unx     1734 b- defN 24-Jun-03 12:08 migrations/0021_overwrite_vectorsets_key.py
--rw-r--r--  2.0 unx      835 b- defN 24-Jun-03 12:08 migrations/__init__.py
--rw-r--r--  2.0 unx      891 b- defN 24-Jun-03 12:08 nucliadb/__init__.py
--rw-r--r--  2.0 unx     3733 b- defN 24-Jun-03 12:08 nucliadb/health.py
--rw-r--r--  2.0 unx    11793 b- defN 24-Jun-03 12:08 nucliadb/learning_proxy.py
--rw-r--r--  2.0 unx     4820 b- defN 24-Jun-03 12:08 nucliadb/metrics_exporter.py
--rw-r--r--  2.0 unx     2272 b- defN 24-Jun-03 12:08 nucliadb/openapi.py
--rw-r--r--  2.0 unx        0 b- defN 24-Jun-03 12:08 nucliadb/py.typed
--rw-r--r--  2.0 unx      835 b- defN 24-Jun-03 12:08 nucliadb/common/__init__.py
--rw-r--r--  2.0 unx     1912 b- defN 24-Jun-03 12:08 nucliadb/common/ids.py
--rw-r--r--  2.0 unx     5175 b- defN 24-Jun-03 12:08 nucliadb/common/locking.py
--rw-r--r--  2.0 unx      835 b- defN 24-Jun-03 12:08 nucliadb/common/cluster/__init__.py
--rw-r--r--  2.0 unx     5134 b- defN 24-Jun-03 12:08 nucliadb/common/cluster/base.py
--rw-r--r--  2.0 unx     1495 b- defN 24-Jun-03 12:08 nucliadb/common/cluster/exceptions.py
--rw-r--r--  2.0 unx     3793 b- defN 24-Jun-03 12:08 nucliadb/common/cluster/grpc_node_dummy.py
--rw-r--r--  2.0 unx     3429 b- defN 24-Jun-03 12:08 nucliadb/common/cluster/index_node.py
--rw-r--r--  2.0 unx    24804 b- defN 24-Jun-03 12:08 nucliadb/common/cluster/manager.py
--rw-r--r--  2.0 unx     8831 b- defN 24-Jun-03 12:08 nucliadb/common/cluster/rebalance.py
--rw-r--r--  2.0 unx    20532 b- defN 24-Jun-03 12:08 nucliadb/common/cluster/rollover.py
--rw-r--r--  2.0 unx     3016 b- defN 24-Jun-03 12:08 nucliadb/common/cluster/settings.py
--rw-r--r--  2.0 unx     5715 b- defN 24-Jun-03 12:08 nucliadb/common/cluster/utils.py
--rw-r--r--  2.0 unx      835 b- defN 24-Jun-03 12:08 nucliadb/common/cluster/discovery/__init__.py
--rw-r--r--  2.0 unx     6553 b- defN 24-Jun-03 12:08 nucliadb/common/cluster/discovery/base.py
--rw-r--r--  2.0 unx    12512 b- defN 24-Jun-03 12:08 nucliadb/common/cluster/discovery/k8s.py
--rw-r--r--  2.0 unx     1957 b- defN 24-Jun-03 12:08 nucliadb/common/cluster/discovery/manual.py
--rw-r--r--  2.0 unx     1737 b- defN 24-Jun-03 12:08 nucliadb/common/cluster/discovery/single.py
--rw-r--r--  2.0 unx     1139 b- defN 24-Jun-03 12:08 nucliadb/common/cluster/discovery/types.py
--rw-r--r--  2.0 unx     2548 b- defN 24-Jun-03 12:08 nucliadb/common/cluster/discovery/utils.py
--rw-r--r--  2.0 unx      833 b- defN 24-Jun-03 12:08 nucliadb/common/cluster/standalone/__init__.py
--rw-r--r--  2.0 unx    13712 b- defN 24-Jun-03 12:08 nucliadb/common/cluster/standalone/grpc_node_binding.py
--rw-r--r--  2.0 unx     4683 b- defN 24-Jun-03 12:08 nucliadb/common/cluster/standalone/index_node.py
--rw-r--r--  2.0 unx     3444 b- defN 24-Jun-03 12:08 nucliadb/common/cluster/standalone/service.py
--rw-r--r--  2.0 unx     3545 b- defN 24-Jun-03 12:08 nucliadb/common/cluster/standalone/utils.py
--rw-r--r--  2.0 unx     3440 b- defN 24-Jun-03 12:08 nucliadb/common/context/__init__.py
--rw-r--r--  2.0 unx     1628 b- defN 24-Jun-03 12:08 nucliadb/common/context/fastapi.py
--rw-r--r--  2.0 unx     2062 b- defN 24-Jun-03 12:08 nucliadb/common/datamanagers/__init__.py
--rw-r--r--  2.0 unx     3095 b- defN 24-Jun-03 12:08 nucliadb/common/datamanagers/atomic.py
--rw-r--r--  2.0 unx     1451 b- defN 24-Jun-03 12:08 nucliadb/common/datamanagers/cluster.py
--rw-r--r--  2.0 unx     5383 b- defN 24-Jun-03 12:08 nucliadb/common/datamanagers/entities.py
--rw-r--r--  2.0 unx      883 b- defN 24-Jun-03 12:08 nucliadb/common/datamanagers/exceptions.py
--rw-r--r--  2.0 unx     2764 b- defN 24-Jun-03 12:08 nucliadb/common/datamanagers/fields.py
--rw-r--r--  2.0 unx     3994 b- defN 24-Jun-03 12:08 nucliadb/common/datamanagers/kb.py
--rw-r--r--  2.0 unx     5389 b- defN 24-Jun-03 12:08 nucliadb/common/datamanagers/labels.py
--rw-r--r--  2.0 unx     1599 b- defN 24-Jun-03 12:08 nucliadb/common/datamanagers/processing.py
--rw-r--r--  2.0 unx    11931 b- defN 24-Jun-03 12:08 nucliadb/common/datamanagers/resources.py
--rw-r--r--  2.0 unx     5643 b- defN 24-Jun-03 12:08 nucliadb/common/datamanagers/rollover.py
--rw-r--r--  2.0 unx     1548 b- defN 24-Jun-03 12:08 nucliadb/common/datamanagers/synonyms.py
--rw-r--r--  2.0 unx     1923 b- defN 24-Jun-03 12:08 nucliadb/common/datamanagers/utils.py
--rw-r--r--  2.0 unx     3780 b- defN 24-Jun-03 12:08 nucliadb/common/datamanagers/vectorsets.py
--rw-r--r--  2.0 unx      835 b- defN 24-Jun-03 12:08 nucliadb/common/http_clients/__init__.py
--rw-r--r--  2.0 unx     2146 b- defN 24-Jun-03 12:08 nucliadb/common/http_clients/auth.py
--rw-r--r--  2.0 unx     1100 b- defN 24-Jun-03 12:08 nucliadb/common/http_clients/exceptions.py
--rw-r--r--  2.0 unx     7155 b- defN 24-Jun-03 12:08 nucliadb/common/http_clients/processing.py
--rw-r--r--  2.0 unx     1540 b- defN 24-Jun-03 12:08 nucliadb/common/http_clients/pypi.py
--rw-r--r--  2.0 unx     1551 b- defN 24-Jun-03 12:08 nucliadb/common/http_clients/utils.py
--rw-r--r--  2.0 unx      835 b- defN 24-Jun-03 12:08 nucliadb/common/maindb/__init__.py
--rw-r--r--  2.0 unx     3449 b- defN 24-Jun-03 12:08 nucliadb/common/maindb/driver.py
--rw-r--r--  2.0 unx      988 b- defN 24-Jun-03 12:08 nucliadb/common/maindb/exceptions.py
--rw-r--r--  2.0 unx     6769 b- defN 24-Jun-03 12:08 nucliadb/common/maindb/local.py
--rw-r--r--  2.0 unx     8673 b- defN 24-Jun-03 12:08 nucliadb/common/maindb/pg.py
--rw-r--r--  2.0 unx     6053 b- defN 24-Jun-03 12:08 nucliadb/common/maindb/redis.py
--rw-r--r--  2.0 unx    15314 b- defN 24-Jun-03 12:08 nucliadb/common/maindb/tikv.py
--rw-r--r--  2.0 unx     4167 b- defN 24-Jun-03 12:08 nucliadb/common/maindb/utils.py
--rw-r--r--  2.0 unx      932 b- defN 24-Jun-03 12:08 nucliadb/export_import/__init__.py
--rw-r--r--  2.0 unx     6185 b- defN 24-Jun-03 12:08 nucliadb/export_import/datamanager.py
--rw-r--r--  2.0 unx     1949 b- defN 24-Jun-03 12:08 nucliadb/export_import/exceptions.py
--rw-r--r--  2.0 unx     7116 b- defN 24-Jun-03 12:08 nucliadb/export_import/exporter.py
--rw-r--r--  2.0 unx     4258 b- defN 24-Jun-03 12:08 nucliadb/export_import/importer.py
--rw-r--r--  2.0 unx     2063 b- defN 24-Jun-03 12:08 nucliadb/export_import/models.py
--rw-r--r--  2.0 unx     2571 b- defN 24-Jun-03 12:08 nucliadb/export_import/tasks.py
--rw-r--r--  2.0 unx    19655 b- defN 24-Jun-03 12:08 nucliadb/export_import/utils.py
--rw-r--r--  2.0 unx     1011 b- defN 24-Jun-03 12:08 nucliadb/ingest/__init__.py
--rw-r--r--  2.0 unx     7277 b- defN 24-Jun-03 12:08 nucliadb/ingest/app.py
--rw-r--r--  2.0 unx     1005 b- defN 24-Jun-03 12:08 nucliadb/ingest/cache.py
--rw-r--r--  2.0 unx     2484 b- defN 24-Jun-03 12:08 nucliadb/ingest/partitions.py
--rw-r--r--  2.0 unx    19904 b- defN 24-Jun-03 12:08 nucliadb/ingest/processing.py
--rw-r--r--  2.0 unx        0 b- defN 24-Jun-03 12:08 nucliadb/ingest/py.typed
--rw-r--r--  2.0 unx    20291 b- defN 24-Jun-03 12:08 nucliadb/ingest/serialize.py
--rw-r--r--  2.0 unx     3207 b- defN 24-Jun-03 12:08 nucliadb/ingest/settings.py
--rw-r--r--  2.0 unx     2314 b- defN 24-Jun-03 12:08 nucliadb/ingest/utils.py
--rw-r--r--  2.0 unx      835 b- defN 24-Jun-03 12:08 nucliadb/ingest/consumer/__init__.py
--rw-r--r--  2.0 unx     6918 b- defN 24-Jun-03 12:08 nucliadb/ingest/consumer/auditing.py
--rw-r--r--  2.0 unx    12174 b- defN 24-Jun-03 12:08 nucliadb/ingest/consumer/consumer.py
--rw-r--r--  2.0 unx     3934 b- defN 24-Jun-03 12:08 nucliadb/ingest/consumer/materializer.py
--rw-r--r--  2.0 unx     1075 b- defN 24-Jun-03 12:08 nucliadb/ingest/consumer/metrics.py
--rw-r--r--  2.0 unx     9546 b- defN 24-Jun-03 12:08 nucliadb/ingest/consumer/pull.py
--rw-r--r--  2.0 unx     6871 b- defN 24-Jun-03 12:08 nucliadb/ingest/consumer/service.py
--rw-r--r--  2.0 unx     4331 b- defN 24-Jun-03 12:08 nucliadb/ingest/consumer/shard_creator.py
--rw-r--r--  2.0 unx     2656 b- defN 24-Jun-03 12:08 nucliadb/ingest/consumer/utils.py
--rw-r--r--  2.0 unx      835 b- defN 24-Jun-03 12:08 nucliadb/ingest/fields/__init__.py
--rw-r--r--  2.0 unx    17797 b- defN 24-Jun-03 12:08 nucliadb/ingest/fields/base.py
--rw-r--r--  2.0 unx     7047 b- defN 24-Jun-03 12:08 nucliadb/ingest/fields/conversation.py
--rw-r--r--  2.0 unx     1223 b- defN 24-Jun-03 12:08 nucliadb/ingest/fields/date.py
--rw-r--r--  2.0 unx     1205 b- defN 24-Jun-03 12:08 nucliadb/ingest/fields/exceptions.py
--rw-r--r--  2.0 unx     4840 b- defN 24-Jun-03 12:08 nucliadb/ingest/fields/file.py
--rw-r--r--  2.0 unx     1547 b- defN 24-Jun-03 12:08 nucliadb/ingest/fields/generic.py
--rw-r--r--  2.0 unx     1235 b- defN 24-Jun-03 12:08 nucliadb/ingest/fields/keywordset.py
--rw-r--r--  2.0 unx     2250 b- defN 24-Jun-03 12:08 nucliadb/ingest/fields/layout.py
--rw-r--r--  2.0 unx     4212 b- defN 24-Jun-03 12:08 nucliadb/ingest/fields/link.py
--rw-r--r--  2.0 unx     1319 b- defN 24-Jun-03 12:08 nucliadb/ingest/fields/text.py
--rw-r--r--  2.0 unx      835 b- defN 24-Jun-03 12:08 nucliadb/ingest/orm/__init__.py
--rw-r--r--  2.0 unx    28721 b- defN 24-Jun-03 12:08 nucliadb/ingest/orm/brain.py
--rw-r--r--  2.0 unx     6954 b- defN 24-Jun-03 12:08 nucliadb/ingest/orm/broker_message.py
--rw-r--r--  2.0 unx    15758 b- defN 24-Jun-03 12:08 nucliadb/ingest/orm/entities.py
--rw-r--r--  2.0 unx     1326 b- defN 24-Jun-03 12:08 nucliadb/ingest/orm/exceptions.py
--rw-r--r--  2.0 unx    16068 b- defN 24-Jun-03 12:08 nucliadb/ingest/orm/knowledgebox.py
--rw-r--r--  2.0 unx     1096 b- defN 24-Jun-03 12:08 nucliadb/ingest/orm/metrics.py
--rw-r--r--  2.0 unx    54798 b- defN 24-Jun-03 12:08 nucliadb/ingest/orm/resource.py
--rw-r--r--  2.0 unx     2685 b- defN 24-Jun-03 12:08 nucliadb/ingest/orm/utils.py
--rw-r--r--  2.0 unx    27092 b- defN 24-Jun-03 12:08 nucliadb/ingest/orm/processor/__init__.py
--rw-r--r--  2.0 unx     5104 b- defN 24-Jun-03 12:08 nucliadb/ingest/orm/processor/auditing.py
--rw-r--r--  2.0 unx     1704 b- defN 24-Jun-03 12:08 nucliadb/ingest/orm/processor/sequence_manager.py
--rw-r--r--  2.0 unx     2057 b- defN 24-Jun-03 12:08 nucliadb/ingest/service/__init__.py
--rw-r--r--  2.0 unx      835 b- defN 24-Jun-03 12:08 nucliadb/ingest/service/exceptions.py
--rw-r--r--  2.0 unx    29886 b- defN 24-Jun-03 12:08 nucliadb/ingest/service/writer.py
--rw-r--r--  2.0 unx      835 b- defN 24-Jun-03 12:08 nucliadb/ingest/tests/__init__.py
--rw-r--r--  2.0 unx     1157 b- defN 24-Jun-03 12:08 nucliadb/ingest/tests/conftest.py
--rw-r--r--  2.0 unx    24111 b- defN 24-Jun-03 12:08 nucliadb/ingest/tests/fixtures.py
--rw-r--r--  2.0 unx    62843 b- defN 24-Jun-03 12:08 nucliadb/ingest/tests/vectors.py
--rw-r--r--  2.0 unx      835 b- defN 24-Jun-03 12:08 nucliadb/ingest/tests/integration/__init__.py
--rw-r--r--  2.0 unx      833 b- defN 24-Jun-03 12:08 nucliadb/ingest/tests/integration/consumer/__init__.py
--rw-r--r--  2.0 unx     2500 b- defN 24-Jun-03 12:08 nucliadb/ingest/tests/integration/consumer/test_auditing.py
--rw-r--r--  2.0 unx     3836 b- defN 24-Jun-03 12:08 nucliadb/ingest/tests/integration/consumer/test_materializer.py
--rw-r--r--  2.0 unx     4470 b- defN 24-Jun-03 12:08 nucliadb/ingest/tests/integration/consumer/test_pull.py
--rw-r--r--  2.0 unx     2763 b- defN 24-Jun-03 12:08 nucliadb/ingest/tests/integration/consumer/test_service.py
--rw-r--r--  2.0 unx     2019 b- defN 24-Jun-03 12:08 nucliadb/ingest/tests/integration/consumer/test_shard_creator.py
--rw-r--r--  2.0 unx      835 b- defN 24-Jun-03 12:08 nucliadb/ingest/tests/integration/ingest/__init__.py
--rw-r--r--  2.0 unx    27247 b- defN 24-Jun-03 12:08 nucliadb/ingest/tests/integration/ingest/test_ingest.py
--rw-r--r--  2.0 unx     3040 b- defN 24-Jun-03 12:08 nucliadb/ingest/tests/integration/ingest/test_processing_engine.py
--rw-r--r--  2.0 unx     8586 b- defN 24-Jun-03 12:08 nucliadb/ingest/tests/integration/ingest/test_relations.py
--rw-r--r--  2.0 unx     5637 b- defN 24-Jun-03 12:08 nucliadb/ingest/tests/integration/ingest/test_vectorsets.py
--rw-r--r--  2.0 unx      835 b- defN 24-Jun-03 12:08 nucliadb/ingest/tests/unit/__init__.py
--rw-r--r--  2.0 unx     1189 b- defN 24-Jun-03 12:08 nucliadb/ingest/tests/unit/test_cache.py
--rw-r--r--  2.0 unx     1432 b- defN 24-Jun-03 12:08 nucliadb/ingest/tests/unit/test_partitions.py
--rw-r--r--  2.0 unx     5807 b- defN 24-Jun-03 12:08 nucliadb/ingest/tests/unit/test_processing.py
--rw-r--r--  2.0 unx      978 b- defN 24-Jun-03 12:08 nucliadb/ingest/tests/unit/test_settings.py
--rw-r--r--  2.0 unx      833 b- defN 24-Jun-03 12:08 nucliadb/ingest/tests/unit/consumer/__init__.py
--rw-r--r--  2.0 unx     3885 b- defN 24-Jun-03 12:08 nucliadb/ingest/tests/unit/consumer/test_auditing.py
--rw-r--r--  2.0 unx     2472 b- defN 24-Jun-03 12:08 nucliadb/ingest/tests/unit/consumer/test_consumer.py
--rw-r--r--  2.0 unx     2063 b- defN 24-Jun-03 12:08 nucliadb/ingest/tests/unit/consumer/test_pull.py
--rw-r--r--  2.0 unx     4140 b- defN 24-Jun-03 12:08 nucliadb/ingest/tests/unit/consumer/test_shard_creator.py
--rw-r--r--  2.0 unx     1934 b- defN 24-Jun-03 12:08 nucliadb/ingest/tests/unit/consumer/test_utils.py
--rw-r--r--  2.0 unx      835 b- defN 24-Jun-03 12:08 nucliadb/ingest/tests/unit/orm/__init__.py
--rw-r--r--  2.0 unx     9876 b- defN 24-Jun-03 12:08 nucliadb/ingest/tests/unit/orm/test_brain.py
--rw-r--r--  2.0 unx     2572 b- defN 24-Jun-03 12:08 nucliadb/ingest/tests/unit/orm/test_brain_vectors.py
--rw-r--r--  2.0 unx     1174 b- defN 24-Jun-03 12:08 nucliadb/ingest/tests/unit/orm/test_orm_utils.py
--rw-r--r--  2.0 unx     4045 b- defN 24-Jun-03 12:08 nucliadb/ingest/tests/unit/orm/test_processor.py
--rw-r--r--  2.0 unx    11033 b- defN 24-Jun-03 12:08 nucliadb/ingest/tests/unit/orm/test_resource.py
--rw-r--r--  2.0 unx     2216 b- defN 24-Jun-03 12:08 nucliadb/middleware/__init__.py
--rw-r--r--  2.0 unx     3912 b- defN 24-Jun-03 12:08 nucliadb/middleware/transaction.py
--rw-r--r--  2.0 unx      835 b- defN 24-Jun-03 12:08 nucliadb/migrator/__init__.py
--rw-r--r--  2.0 unx     2119 b- defN 24-Jun-03 12:08 nucliadb/migrator/command.py
--rw-r--r--  2.0 unx     1334 b- defN 24-Jun-03 12:08 nucliadb/migrator/context.py
--rw-r--r--  2.0 unx     5104 b- defN 24-Jun-03 12:08 nucliadb/migrator/datamanager.py
--rw-r--r--  2.0 unx      889 b- defN 24-Jun-03 12:08 nucliadb/migrator/exceptions.py
--rw-r--r--  2.0 unx     9370 b- defN 24-Jun-03 12:08 nucliadb/migrator/migrator.py
--rw-r--r--  2.0 unx     1145 b- defN 24-Jun-03 12:08 nucliadb/migrator/models.py
--rw-r--r--  2.0 unx     1144 b- defN 24-Jun-03 12:08 nucliadb/migrator/settings.py
--rw-r--r--  2.0 unx     2346 b- defN 24-Jun-03 12:08 nucliadb/migrator/utils.py
--rw-r--r--  2.0 unx      835 b- defN 24-Jun-03 12:08 nucliadb/models/__init__.py
--rw-r--r--  2.0 unx     1599 b- defN 24-Jun-03 12:08 nucliadb/models/responses.py
--rw-r--r--  2.0 unx     6041 b- defN 24-Jun-03 12:08 nucliadb/purge/__init__.py
--rw-r--r--  2.0 unx     9367 b- defN 24-Jun-03 12:08 nucliadb/purge/orphan_shards.py
--rw-r--r--  2.0 unx     1328 b- defN 24-Jun-03 12:08 nucliadb/reader/__init__.py
--rw-r--r--  2.0 unx     3709 b- defN 24-Jun-03 12:08 nucliadb/reader/app.py
--rw-r--r--  2.0 unx     1366 b- defN 24-Jun-03 12:08 nucliadb/reader/lifecycle.py
--rw-r--r--  2.0 unx     1031 b- defN 24-Jun-03 12:08 nucliadb/reader/openapi.py
--rw-r--r--  2.0 unx        0 b- defN 24-Jun-03 12:08 nucliadb/reader/py.typed
--rw-r--r--  2.0 unx     1447 b- defN 24-Jun-03 12:08 nucliadb/reader/run.py
--rw-r--r--  2.0 unx      872 b- defN 24-Jun-03 12:08 nucliadb/reader/api/__init__.py
--rw-r--r--  2.0 unx     2458 b- defN 24-Jun-03 12:08 nucliadb/reader/api/models.py
--rw-r--r--  2.0 unx     1110 b- defN 24-Jun-03 12:08 nucliadb/reader/api/v1/__init__.py
--rw-r--r--  2.0 unx    12457 b- defN 24-Jun-03 12:08 nucliadb/reader/api/v1/download.py
--rw-r--r--  2.0 unx     6448 b- defN 24-Jun-03 12:08 nucliadb/reader/api/v1/export_import.py
--rw-r--r--  2.0 unx     3641 b- defN 24-Jun-03 12:08 nucliadb/reader/api/v1/knowledgebox.py
--rw-r--r--  2.0 unx     2099 b- defN 24-Jun-03 12:08 nucliadb/reader/api/v1/learning_collector.py
--rw-r--r--  2.0 unx     4472 b- defN 24-Jun-03 12:08 nucliadb/reader/api/v1/learning_config.py
--rw-r--r--  2.0 unx    13961 b- defN 24-Jun-03 12:08 nucliadb/reader/api/v1/resource.py
--rw-r--r--  2.0 unx     1011 b- defN 24-Jun-03 12:08 nucliadb/reader/api/v1/router.py
--rw-r--r--  2.0 unx    11902 b- defN 24-Jun-03 12:08 nucliadb/reader/api/v1/services.py
--rw-r--r--  2.0 unx      835 b- defN 24-Jun-03 12:08 nucliadb/reader/reader/__init__.py
--rw-r--r--  2.0 unx     7979 b- defN 24-Jun-03 12:08 nucliadb/reader/reader/notifications.py
--rw-r--r--  2.0 unx      835 b- defN 24-Jun-03 12:08 nucliadb/reader/tests/__init__.py
--rw-r--r--  2.0 unx     1224 b- defN 24-Jun-03 12:08 nucliadb/reader/tests/conftest.py
--rw-r--r--  2.0 unx     4355 b- defN 24-Jun-03 12:08 nucliadb/reader/tests/fixtures.py
--rw-r--r--  2.0 unx     2748 b- defN 24-Jun-03 12:08 nucliadb/reader/tests/test_list_resources.py
--rw-r--r--  2.0 unx    10199 b- defN 24-Jun-03 12:08 nucliadb/reader/tests/test_reader_file_download.py
--rw-r--r--  2.0 unx    10586 b- defN 24-Jun-03 12:08 nucliadb/reader/tests/test_reader_resource.py
--rw-r--r--  2.0 unx     6535 b- defN 24-Jun-03 12:08 nucliadb/reader/tests/test_reader_resource_field.py
--rw-r--r--  2.0 unx     1535 b- defN 24-Jun-03 12:08 nucliadb/search/__init__.py
--rw-r--r--  2.0 unx     4905 b- defN 24-Jun-03 12:08 nucliadb/search/app.py
--rw-r--r--  2.0 unx     1956 b- defN 24-Jun-03 12:08 nucliadb/search/lifecycle.py
--rw-r--r--  2.0 unx     1016 b- defN 24-Jun-03 12:08 nucliadb/search/openapi.py
--rw-r--r--  2.0 unx    20665 b- defN 24-Jun-03 12:08 nucliadb/search/predict.py
--rw-r--r--  2.0 unx        0 b- defN 24-Jun-03 12:08 nucliadb/search/py.typed
--rw-r--r--  2.0 unx     1402 b- defN 24-Jun-03 12:08 nucliadb/search/run.py
--rw-r--r--  2.0 unx     1193 b- defN 24-Jun-03 12:08 nucliadb/search/settings.py
--rw-r--r--  2.0 unx     1037 b- defN 24-Jun-03 12:08 nucliadb/search/utilities.py
--rw-r--r--  2.0 unx      835 b- defN 24-Jun-03 12:08 nucliadb/search/api/__init__.py
--rw-r--r--  2.0 unx     1298 b- defN 24-Jun-03 12:08 nucliadb/search/api/v1/__init__.py
--rw-r--r--  2.0 unx     3435 b- defN 24-Jun-03 12:08 nucliadb/search/api/v1/ask.py
--rw-r--r--  2.0 unx     9514 b- defN 24-Jun-03 12:08 nucliadb/search/api/v1/chat.py
--rw-r--r--  2.0 unx     2668 b- defN 24-Jun-03 12:08 nucliadb/search/api/v1/feedback.py
--rw-r--r--  2.0 unx     8795 b- defN 24-Jun-03 12:08 nucliadb/search/api/v1/find.py
--rw-r--r--  2.0 unx     6941 b- defN 24-Jun-03 12:08 nucliadb/search/api/v1/knowledgebox.py
--rw-r--r--  2.0 unx     3047 b- defN 24-Jun-03 12:08 nucliadb/search/api/v1/predict_proxy.py
--rw-r--r--  2.0 unx      988 b- defN 24-Jun-03 12:08 nucliadb/search/api/v1/router.py
--rw-r--r--  2.0 unx    19262 b- defN 24-Jun-03 12:08 nucliadb/search/api/v1/search.py
--rw-r--r--  2.0 unx     5970 b- defN 24-Jun-03 12:08 nucliadb/search/api/v1/suggest.py
--rw-r--r--  2.0 unx     2499 b- defN 24-Jun-03 12:08 nucliadb/search/api/v1/summarize.py
--rw-r--r--  2.0 unx     1434 b- defN 24-Jun-03 12:08 nucliadb/search/api/v1/utils.py
--rw-r--r--  2.0 unx      835 b- defN 24-Jun-03 12:08 nucliadb/search/api/v1/resource/__init__.py
--rw-r--r--  2.0 unx     3869 b- defN 24-Jun-03 12:08 nucliadb/search/api/v1/resource/ask.py
--rw-r--r--  2.0 unx     5866 b- defN 24-Jun-03 12:08 nucliadb/search/api/v1/resource/chat.py
--rw-r--r--  2.0 unx     5303 b- defN 24-Jun-03 12:08 nucliadb/search/api/v1/resource/search.py
--rw-r--r--  2.0 unx      833 b- defN 24-Jun-03 12:08 nucliadb/search/requesters/__init__.py
--rw-r--r--  2.0 unx     9111 b- defN 24-Jun-03 12:08 nucliadb/search/requesters/utils.py
--rw-r--r--  2.0 unx      835 b- defN 24-Jun-03 12:08 nucliadb/search/search/__init__.py
--rw-r--r--  2.0 unx     2746 b- defN 24-Jun-03 12:08 nucliadb/search/search/cache.py
--rw-r--r--  2.0 unx     1154 b- defN 24-Jun-03 12:08 nucliadb/search/search/exceptions.py
--rw-r--r--  2.0 unx     5465 b- defN 24-Jun-03 12:08 nucliadb/search/search/fetch.py
--rw-r--r--  2.0 unx     6513 b- defN 24-Jun-03 12:08 nucliadb/search/search/filters.py
--rw-r--r--  2.0 unx     4612 b- defN 24-Jun-03 12:08 nucliadb/search/search/find.py
--rw-r--r--  2.0 unx    17152 b- defN 24-Jun-03 12:08 nucliadb/search/search/find_merge.py
--rw-r--r--  2.0 unx    21282 b- defN 24-Jun-03 12:08 nucliadb/search/search/merge.py
--rw-r--r--  2.0 unx     1130 b- defN 24-Jun-03 12:08 nucliadb/search/search/metrics.py
--rw-r--r--  2.0 unx     8698 b- defN 24-Jun-03 12:08 nucliadb/search/search/paragraphs.py
--rw-r--r--  2.0 unx     3015 b- defN 24-Jun-03 12:08 nucliadb/search/search/predict_proxy.py
--rw-r--r--  2.0 unx    31093 b- defN 24-Jun-03 12:08 nucliadb/search/search/query.py
--rw-r--r--  2.0 unx     3018 b- defN 24-Jun-03 12:08 nucliadb/search/search/shards.py
--rw-r--r--  2.0 unx     5101 b- defN 24-Jun-03 12:08 nucliadb/search/search/summarize.py
--rw-r--r--  2.0 unx     2438 b- defN 24-Jun-03 12:08 nucliadb/search/search/utils.py
--rw-r--r--  2.0 unx      835 b- defN 24-Jun-03 12:08 nucliadb/search/search/chat/__init__.py
--rw-r--r--  2.0 unx    16676 b- defN 24-Jun-03 12:08 nucliadb/search/search/chat/ask.py
--rw-r--r--  2.0 unx     2058 b- defN 24-Jun-03 12:08 nucliadb/search/search/chat/images.py
--rw-r--r--  2.0 unx    20793 b- defN 24-Jun-03 12:08 nucliadb/search/search/chat/prompt.py
--rw-r--r--  2.0 unx    17543 b- defN 24-Jun-03 12:08 nucliadb/search/search/chat/query.py
--rw-r--r--  2.0 unx      835 b- defN 24-Jun-03 12:08 nucliadb/search/tests/__init__.py
--rw-r--r--  2.0 unx     1295 b- defN 24-Jun-03 12:08 nucliadb/search/tests/conftest.py
--rw-r--r--  2.0 unx     6578 b- defN 24-Jun-03 12:08 nucliadb/search/tests/fixtures.py
--rw-r--r--  2.0 unx    15480 b- defN 24-Jun-03 12:08 nucliadb/search/tests/node.py
--rw-r--r--  2.0 unx      833 b- defN 24-Jun-03 12:08 nucliadb/search/tests/unit/__init__.py
--rw-r--r--  2.0 unx     2649 b- defN 24-Jun-03 12:08 nucliadb/search/tests/unit/test_app.py
--rw-r--r--  2.0 unx     3374 b- defN 24-Jun-03 12:08 nucliadb/search/tests/unit/test_find_merge.py
--rw-r--r--  2.0 unx     1400 b- defN 24-Jun-03 12:08 nucliadb/search/tests/unit/test_merge.py
--rw-r--r--  2.0 unx    15721 b- defN 24-Jun-03 12:08 nucliadb/search/tests/unit/test_predict.py
--rw-r--r--  2.0 unx     1328 b- defN 24-Jun-03 12:08 nucliadb/search/tests/unit/test_run.py
--rw-r--r--  2.0 unx      835 b- defN 24-Jun-03 12:08 nucliadb/search/tests/unit/api/__init__.py
--rw-r--r--  2.0 unx      835 b- defN 24-Jun-03 12:08 nucliadb/search/tests/unit/api/v1/__init__.py
--rw-r--r--  2.0 unx     3759 b- defN 24-Jun-03 12:08 nucliadb/search/tests/unit/api/v1/test_ask.py
--rw-r--r--  2.0 unx     2966 b- defN 24-Jun-03 12:08 nucliadb/search/tests/unit/api/v1/test_chat.py
--rw-r--r--  2.0 unx     2865 b- defN 24-Jun-03 12:08 nucliadb/search/tests/unit/api/v1/test_predict_proxy.py
--rw-r--r--  2.0 unx     2901 b- defN 24-Jun-03 12:08 nucliadb/search/tests/unit/api/v1/test_summarize.py
--rw-r--r--  2.0 unx      835 b- defN 24-Jun-03 12:08 nucliadb/search/tests/unit/api/v1/resource/__init__.py
--rw-r--r--  2.0 unx     3040 b- defN 24-Jun-03 12:08 nucliadb/search/tests/unit/api/v1/resource/test_chat.py
--rw-r--r--  2.0 unx      833 b- defN 24-Jun-03 12:08 nucliadb/search/tests/unit/search/__init__.py
--rw-r--r--  2.0 unx     8586 b- defN 24-Jun-03 12:08 nucliadb/search/tests/unit/search/test_chat_prompt.py
--rw-r--r--  2.0 unx     3736 b- defN 24-Jun-03 12:08 nucliadb/search/tests/unit/search/test_fetch.py
--rw-r--r--  2.0 unx     4306 b- defN 24-Jun-03 12:08 nucliadb/search/tests/unit/search/test_filters.py
--rw-r--r--  2.0 unx     4492 b- defN 24-Jun-03 12:08 nucliadb/search/tests/unit/search/test_paragraphs.py
--rw-r--r--  2.0 unx     3496 b- defN 24-Jun-03 12:08 nucliadb/search/tests/unit/search/test_predict_proxy.py
--rw-r--r--  2.0 unx     5121 b- defN 24-Jun-03 12:08 nucliadb/search/tests/unit/search/test_query.py
--rw-r--r--  2.0 unx      833 b- defN 24-Jun-03 12:08 nucliadb/search/tests/unit/search/requesters/__init__.py
--rw-r--r--  2.0 unx     6455 b- defN 24-Jun-03 12:08 nucliadb/search/tests/unit/search/requesters/test_utils.py
--rw-r--r--  2.0 unx      835 b- defN 24-Jun-03 12:08 nucliadb/search/tests/unit/search/search/__init__.py
--rw-r--r--  2.0 unx     1759 b- defN 24-Jun-03 12:08 nucliadb/search/tests/unit/search/search/test_shards.py
--rw-r--r--  2.0 unx     2511 b- defN 24-Jun-03 12:08 nucliadb/search/tests/unit/search/search/test_utils.py
--rw-r--r--  2.0 unx      835 b- defN 24-Jun-03 12:08 nucliadb/standalone/__init__.py
--rw-r--r--  2.0 unx     6749 b- defN 24-Jun-03 12:08 nucliadb/standalone/api_router.py
--rw-r--r--  2.0 unx     5763 b- defN 24-Jun-03 12:08 nucliadb/standalone/app.py
--rw-r--r--  2.0 unx     7800 b- defN 24-Jun-03 12:08 nucliadb/standalone/auth.py
--rw-r--r--  2.0 unx     5313 b- defN 24-Jun-03 12:08 nucliadb/standalone/config.py
--rw-r--r--  2.0 unx     6986 b- defN 24-Jun-03 12:08 nucliadb/standalone/introspect.py
--rw-r--r--  2.0 unx     2488 b- defN 24-Jun-03 12:08 nucliadb/standalone/lifecycle.py
--rw-r--r--  2.0 unx     1980 b- defN 24-Jun-03 12:08 nucliadb/standalone/migrations.py
--rw-r--r--  2.0 unx     1322 b- defN 24-Jun-03 12:08 nucliadb/standalone/purge.py
--rw-r--r--  2.0 unx        0 b- defN 24-Jun-03 12:08 nucliadb/standalone/py.typed
--rw-r--r--  2.0 unx     5636 b- defN 24-Jun-03 12:08 nucliadb/standalone/run.py
--rw-r--r--  2.0 unx     5822 b- defN 24-Jun-03 12:08 nucliadb/standalone/settings.py
--rw-r--r--  2.0 unx     3132 b- defN 24-Jun-03 12:08 nucliadb/standalone/versions.py
--rw-r--r--  2.0 unx     2285 b- defN 24-Jun-03 12:08 nucliadb/standalone/static/favicon.ico
--rw-r--r--  2.0 unx     3833 b- defN 24-Jun-03 12:08 nucliadb/standalone/static/index.html
--rw-r--r--  2.0 unx     2639 b- defN 24-Jun-03 12:08 nucliadb/standalone/static/logo.svg
--rw-r--r--  2.0 unx      835 b- defN 24-Jun-03 12:08 nucliadb/standalone/tests/__init__.py
--rw-r--r--  2.0 unx     1294 b- defN 24-Jun-03 12:08 nucliadb/standalone/tests/conftest.py
--rw-r--r--  2.0 unx     1319 b- defN 24-Jun-03 12:08 nucliadb/standalone/tests/fixtures.py
--rw-r--r--  2.0 unx      833 b- defN 24-Jun-03 12:08 nucliadb/standalone/tests/unit/__init__.py
--rw-r--r--  2.0 unx     1722 b- defN 24-Jun-03 12:08 nucliadb/standalone/tests/unit/test_api_router.py
--rw-r--r--  2.0 unx     5509 b- defN 24-Jun-03 12:08 nucliadb/standalone/tests/unit/test_auth.py
--rw-r--r--  2.0 unx     1334 b- defN 24-Jun-03 12:08 nucliadb/standalone/tests/unit/test_introspect.py
--rw-r--r--  2.0 unx     1863 b- defN 24-Jun-03 12:08 nucliadb/standalone/tests/unit/test_migrations.py
--rw-r--r--  2.0 unx     1546 b- defN 24-Jun-03 12:08 nucliadb/standalone/tests/unit/test_run.py
--rw-r--r--  2.0 unx     1972 b- defN 24-Jun-03 12:08 nucliadb/standalone/tests/unit/test_versions.py
--rw-r--r--  2.0 unx     1037 b- defN 24-Jun-03 12:08 nucliadb/tasks/__init__.py
--rw-r--r--  2.0 unx     7655 b- defN 24-Jun-03 12:08 nucliadb/tasks/consumer.py
--rw-r--r--  2.0 unx      924 b- defN 24-Jun-03 12:08 nucliadb/tasks/logger.py
--rw-r--r--  2.0 unx     1378 b- defN 24-Jun-03 12:08 nucliadb/tasks/models.py
--rw-r--r--  2.0 unx     3457 b- defN 24-Jun-03 12:08 nucliadb/tasks/producer.py
--rw-r--r--  2.0 unx     1753 b- defN 24-Jun-03 12:08 nucliadb/tasks/registry.py
--rw-r--r--  2.0 unx     1360 b- defN 24-Jun-03 12:08 nucliadb/tasks/utils.py
--rw-r--r--  2.0 unx      835 b- defN 24-Jun-03 12:08 nucliadb/tests/__init__.py
--rw-r--r--  2.0 unx     1229 b- defN 24-Jun-03 12:08 nucliadb/tests/conftest.py
--rw-r--r--  2.0 unx    22365 b- defN 24-Jun-03 12:08 nucliadb/tests/fixtures.py
--rw-r--r--  2.0 unx     7549 b- defN 24-Jun-03 12:08 nucliadb/tests/tikv.py
--rw-r--r--  2.0 unx      835 b- defN 24-Jun-03 12:08 nucliadb/tests/benchmarks/__init__.py
--rw-r--r--  2.0 unx     3032 b- defN 24-Jun-03 12:08 nucliadb/tests/benchmarks/test_search.py
--rw-r--r--  2.0 unx      919 b- defN 24-Jun-03 12:08 nucliadb/tests/knowledgeboxes/__init__.py
--rw-r--r--  2.0 unx     7002 b- defN 24-Jun-03 12:08 nucliadb/tests/knowledgeboxes/philosophy_books.py
--rw-r--r--  2.0 unx     3037 b- defN 24-Jun-03 12:08 nucliadb/tests/knowledgeboxes/ten_dummy_resources.py
--rw-r--r--  2.0 unx     1148 b- defN 24-Jun-03 12:08 nucliadb/tests/migrations/__init__.py
--rw-r--r--  2.0 unx     2726 b- defN 24-Jun-03 12:08 nucliadb/tests/migrations/test_migration_0017.py
--rw-r--r--  2.0 unx     3662 b- defN 24-Jun-03 12:08 nucliadb/tests/migrations/test_migration_0018.py
--rw-r--r--  2.0 unx     3439 b- defN 24-Jun-03 12:08 nucliadb/tests/migrations/test_migration_0021.py
--rw-r--r--  2.0 unx      835 b- defN 24-Jun-03 12:08 nucliadb/tests/unit/__init__.py
--rw-r--r--  2.0 unx     1487 b- defN 24-Jun-03 12:08 nucliadb/tests/unit/test_field_ids.py
--rw-r--r--  2.0 unx     2780 b- defN 24-Jun-03 12:08 nucliadb/tests/unit/test_health.py
--rw-r--r--  2.0 unx     1543 b- defN 24-Jun-03 12:08 nucliadb/tests/unit/test_kb_slugs.py
--rw-r--r--  2.0 unx     7892 b- defN 24-Jun-03 12:08 nucliadb/tests/unit/test_learning_proxy.py
--rw-r--r--  2.0 unx     2642 b- defN 24-Jun-03 12:08 nucliadb/tests/unit/test_metrics_exporter.py
--rw-r--r--  2.0 unx     1341 b- defN 24-Jun-03 12:08 nucliadb/tests/unit/test_openapi.py
--rw-r--r--  2.0 unx     3649 b- defN 24-Jun-03 12:08 nucliadb/tests/unit/test_purge.py
--rw-r--r--  2.0 unx      835 b- defN 24-Jun-03 12:08 nucliadb/tests/unit/common/__init__.py
--rw-r--r--  2.0 unx     1268 b- defN 24-Jun-03 12:08 nucliadb/tests/unit/common/test_context.py
--rw-r--r--  2.0 unx      835 b- defN 24-Jun-03 12:08 nucliadb/tests/unit/common/cluster/__init__.py
--rw-r--r--  2.0 unx    12240 b- defN 24-Jun-03 12:08 nucliadb/tests/unit/common/cluster/test_cluster.py
--rw-r--r--  2.0 unx     5387 b- defN 24-Jun-03 12:08 nucliadb/tests/unit/common/cluster/test_kb_shard_manager.py
--rw-r--r--  2.0 unx     1428 b- defN 24-Jun-03 12:08 nucliadb/tests/unit/common/cluster/test_rebalance.py
--rw-r--r--  2.0 unx     9609 b- defN 24-Jun-03 12:08 nucliadb/tests/unit/common/cluster/test_rollover.py
--rw-r--r--  2.0 unx      835 b- defN 24-Jun-03 12:08 nucliadb/tests/unit/common/cluster/discovery/__init__.py
--rw-r--r--  2.0 unx     5627 b- defN 24-Jun-03 12:08 nucliadb/tests/unit/common/cluster/discovery/test_k8s.py
--rw-r--r--  2.0 unx      833 b- defN 24-Jun-03 12:08 nucliadb/tests/unit/common/cluster/standalone/__init__.py
--rw-r--r--  2.0 unx     3761 b- defN 24-Jun-03 12:08 nucliadb/tests/unit/common/cluster/standalone/test_service.py
--rw-r--r--  2.0 unx     2136 b- defN 24-Jun-03 12:08 nucliadb/tests/unit/common/cluster/standalone/test_utils.py
--rw-r--r--  2.0 unx      833 b- defN 24-Jun-03 12:08 nucliadb/tests/unit/common/maindb/__init__.py
--rw-r--r--  2.0 unx     3579 b- defN 24-Jun-03 12:08 nucliadb/tests/unit/common/maindb/test_driver.py
--rw-r--r--  2.0 unx     2119 b- defN 24-Jun-03 12:08 nucliadb/tests/unit/common/maindb/test_tikv.py
--rw-r--r--  2.0 unx     3213 b- defN 24-Jun-03 12:08 nucliadb/tests/unit/common/maindb/test_utils.py
--rw-r--r--  2.0 unx      835 b- defN 24-Jun-03 12:08 nucliadb/tests/unit/export_import/__init__.py
--rw-r--r--  2.0 unx     1435 b- defN 24-Jun-03 12:08 nucliadb/tests/unit/export_import/test_datamanager.py
--rw-r--r--  2.0 unx     9706 b- defN 24-Jun-03 12:08 nucliadb/tests/unit/export_import/test_utils.py
--rw-r--r--  2.0 unx      835 b- defN 24-Jun-03 12:08 nucliadb/tests/unit/migrator/__init__.py
--rw-r--r--  2.0 unx     3233 b- defN 24-Jun-03 12:08 nucliadb/tests/unit/migrator/test_migrator.py
--rw-r--r--  2.0 unx      835 b- defN 24-Jun-03 12:08 nucliadb/tests/unit/tasks/__init__.py
--rw-r--r--  2.0 unx     1375 b- defN 24-Jun-03 12:08 nucliadb/tests/unit/tasks/conftest.py
--rw-r--r--  2.0 unx     2714 b- defN 24-Jun-03 12:08 nucliadb/tests/unit/tasks/test_consumer.py
--rw-r--r--  2.0 unx     3189 b- defN 24-Jun-03 12:08 nucliadb/tests/unit/tasks/test_producer.py
--rw-r--r--  2.0 unx     1827 b- defN 24-Jun-03 12:08 nucliadb/tests/unit/tasks/test_tasks.py
--rw-r--r--  2.0 unx     2507 b- defN 24-Jun-03 12:08 nucliadb/tests/utils/__init__.py
--rw-r--r--  2.0 unx     1797 b- defN 24-Jun-03 12:08 nucliadb/tests/utils/aiohttp_session.py
--rw-r--r--  2.0 unx     2533 b- defN 24-Jun-03 12:08 nucliadb/tests/utils/entities.py
--rw-r--r--  2.0 unx     6327 b- defN 24-Jun-03 12:08 nucliadb/tests/utils/broker_messages/__init__.py
--rw-r--r--  2.0 unx     7557 b- defN 24-Jun-03 12:08 nucliadb/tests/utils/broker_messages/fields.py
--rw-r--r--  2.0 unx     1196 b- defN 24-Jun-03 12:08 nucliadb/tests/utils/broker_messages/helpers.py
--rw-r--r--  2.0 unx     1325 b- defN 24-Jun-03 12:08 nucliadb/train/__init__.py
--rw-r--r--  2.0 unx     3530 b- defN 24-Jun-03 12:08 nucliadb/train/app.py
--rw-r--r--  2.0 unx     3800 b- defN 24-Jun-03 12:08 nucliadb/train/generator.py
--rw-r--r--  2.0 unx     1698 b- defN 24-Jun-03 12:08 nucliadb/train/lifecycle.py
--rw-r--r--  2.0 unx     1198 b- defN 24-Jun-03 12:08 nucliadb/train/models.py
--rw-r--r--  2.0 unx     5776 b- defN 24-Jun-03 12:08 nucliadb/train/nodes.py
--rw-r--r--  2.0 unx        0 b- defN 24-Jun-03 12:08 nucliadb/train/py.typed
--rw-r--r--  2.0 unx     1400 b- defN 24-Jun-03 12:08 nucliadb/train/run.py
--rw-r--r--  2.0 unx     5750 b- defN 24-Jun-03 12:08 nucliadb/train/servicer.py
--rw-r--r--  2.0 unx     1415 b- defN 24-Jun-03 12:08 nucliadb/train/settings.py
--rw-r--r--  2.0 unx     1496 b- defN 24-Jun-03 12:08 nucliadb/train/types.py
--rw-r--r--  2.0 unx     3265 b- defN 24-Jun-03 12:08 nucliadb/train/upload.py
--rw-r--r--  2.0 unx     6395 b- defN 24-Jun-03 12:08 nucliadb/train/uploader.py
--rw-r--r--  2.0 unx     3179 b- defN 24-Jun-03 12:08 nucliadb/train/utils.py
--rw-r--r--  2.0 unx      835 b- defN 24-Jun-03 12:08 nucliadb/train/api/__init__.py
--rw-r--r--  2.0 unx     1479 b- defN 24-Jun-03 12:08 nucliadb/train/api/utils.py
--rw-r--r--  2.0 unx      928 b- defN 24-Jun-03 12:08 nucliadb/train/api/v1/__init__.py
--rw-r--r--  2.0 unx     2071 b- defN 24-Jun-03 12:08 nucliadb/train/api/v1/check.py
--rw-r--r--  2.0 unx      910 b- defN 24-Jun-03 12:08 nucliadb/train/api/v1/router.py
--rw-r--r--  2.0 unx     1908 b- defN 24-Jun-03 12:08 nucliadb/train/api/v1/shards.py
--rw-r--r--  2.0 unx     2135 b- defN 24-Jun-03 12:08 nucliadb/train/api/v1/trainset.py
--rw-r--r--  2.0 unx      835 b- defN 24-Jun-03 12:08 nucliadb/train/generators/__init__.py
--rw-r--r--  2.0 unx     3723 b- defN 24-Jun-03 12:08 nucliadb/train/generators/field_classifier.py
--rw-r--r--  2.0 unx     6712 b- defN 24-Jun-03 12:08 nucliadb/train/generators/image_classifier.py
--rw-r--r--  2.0 unx     2789 b- defN 24-Jun-03 12:08 nucliadb/train/generators/paragraph_classifier.py
--rw-r--r--  2.0 unx     3590 b- defN 24-Jun-03 12:08 nucliadb/train/generators/paragraph_streaming.py
--rw-r--r--  2.0 unx     5372 b- defN 24-Jun-03 12:08 nucliadb/train/generators/question_answer_streaming.py
--rw-r--r--  2.0 unx     5160 b- defN 24-Jun-03 12:08 nucliadb/train/generators/sentence_classifier.py
--rw-r--r--  2.0 unx    10446 b- defN 24-Jun-03 12:08 nucliadb/train/generators/token_classifier.py
--rw-r--r--  2.0 unx     3877 b- defN 24-Jun-03 12:08 nucliadb/train/generators/utils.py
--rw-r--r--  2.0 unx      835 b- defN 24-Jun-03 12:08 nucliadb/train/tests/__init__.py
--rw-r--r--  2.0 unx     1125 b- defN 24-Jun-03 12:08 nucliadb/train/tests/conftest.py
--rw-r--r--  2.0 unx    10995 b- defN 24-Jun-03 12:08 nucliadb/train/tests/fixtures.py
--rw-r--r--  2.0 unx     4571 b- defN 24-Jun-03 12:08 nucliadb/train/tests/test_field_classification.py
--rw-r--r--  2.0 unx     2729 b- defN 24-Jun-03 12:08 nucliadb/train/tests/test_get_entities.py
--rw-r--r--  2.0 unx     1660 b- defN 24-Jun-03 12:08 nucliadb/train/tests/test_get_info.py
--rw-r--r--  2.0 unx     1379 b- defN 24-Jun-03 12:08 nucliadb/train/tests/test_get_ontology.py
--rw-r--r--  2.0 unx     2201 b- defN 24-Jun-03 12:08 nucliadb/train/tests/test_get_ontology_count.py
--rw-r--r--  2.0 unx     7669 b- defN 24-Jun-03 12:08 nucliadb/train/tests/test_image_classification.py
--rw-r--r--  2.0 unx     1416 b- defN 24-Jun-03 12:08 nucliadb/train/tests/test_list_fields.py
--rw-r--r--  2.0 unx     2944 b- defN 24-Jun-03 12:08 nucliadb/train/tests/test_list_paragraphs.py
--rw-r--r--  2.0 unx     1423 b- defN 24-Jun-03 12:08 nucliadb/train/tests/test_list_resources.py
--rw-r--r--  2.0 unx     2947 b- defN 24-Jun-03 12:08 nucliadb/train/tests/test_list_sentences.py
--rw-r--r--  2.0 unx     4645 b- defN 24-Jun-03 12:08 nucliadb/train/tests/test_paragraph_classification.py
--rw-r--r--  2.0 unx     4320 b- defN 24-Jun-03 12:08 nucliadb/train/tests/test_paragraph_streaming.py
--rw-r--r--  2.0 unx     8751 b- defN 24-Jun-03 12:08 nucliadb/train/tests/test_question_answer_streaming.py
--rw-r--r--  2.0 unx     5051 b- defN 24-Jun-03 12:08 nucliadb/train/tests/test_sentence_classification.py
--rw-r--r--  2.0 unx     5583 b- defN 24-Jun-03 12:08 nucliadb/train/tests/test_token_classification.py
--rw-r--r--  2.0 unx     3324 b- defN 24-Jun-03 12:08 nucliadb/train/tests/utils.py
--rw-r--r--  2.0 unx     1328 b- defN 24-Jun-03 12:08 nucliadb/writer/__init__.py
--rw-r--r--  2.0 unx     4268 b- defN 24-Jun-03 12:08 nucliadb/writer/app.py
--rw-r--r--  2.0 unx    19472 b- defN 24-Jun-03 12:08 nucliadb/writer/back_pressure.py
--rw-r--r--  2.0 unx      929 b- defN 24-Jun-03 12:08 nucliadb/writer/exceptions.py
--rw-r--r--  2.0 unx     1953 b- defN 24-Jun-03 12:08 nucliadb/writer/lifecycle.py
--rw-r--r--  2.0 unx     1032 b- defN 24-Jun-03 12:08 nucliadb/writer/openapi.py
--rw-r--r--  2.0 unx        0 b- defN 24-Jun-03 12:08 nucliadb/writer/py.typed
--rw-r--r--  2.0 unx     1448 b- defN 24-Jun-03 12:08 nucliadb/writer/run.py
--rw-r--r--  2.0 unx     3103 b- defN 24-Jun-03 12:08 nucliadb/writer/settings.py
--rw-r--r--  2.0 unx     1036 b- defN 24-Jun-03 12:08 nucliadb/writer/utilities.py
--rw-r--r--  2.0 unx      835 b- defN 24-Jun-03 12:08 nucliadb/writer/api/__init__.py
--rw-r--r--  2.0 unx     1429 b- defN 24-Jun-03 12:08 nucliadb/writer/api/constants.py
--rw-r--r--  2.0 unx     1095 b- defN 24-Jun-03 12:08 nucliadb/writer/api/v1/__init__.py
--rw-r--r--  2.0 unx     6421 b- defN 24-Jun-03 12:08 nucliadb/writer/api/v1/export_import.py
--rw-r--r--  2.0 unx    24482 b- defN 24-Jun-03 12:08 nucliadb/writer/api/v1/field.py
--rw-r--r--  2.0 unx     5248 b- defN 24-Jun-03 12:08 nucliadb/writer/api/v1/knowledgebox.py
--rw-r--r--  2.0 unx     2058 b- defN 24-Jun-03 12:08 nucliadb/writer/api/v1/learning_config.py
--rw-r--r--  2.0 unx    18628 b- defN 24-Jun-03 12:08 nucliadb/writer/api/v1/resource.py
--rw-r--r--  2.0 unx     1034 b- defN 24-Jun-03 12:08 nucliadb/writer/api/v1/router.py
--rw-r--r--  2.0 unx    10485 b- defN 24-Jun-03 12:08 nucliadb/writer/api/v1/services.py
--rw-r--r--  2.0 unx    30985 b- defN 24-Jun-03 12:08 nucliadb/writer/api/v1/upload.py
--rw-r--r--  2.0 unx     1612 b- defN 24-Jun-03 12:08 nucliadb/writer/layouts/__init__.py
--rw-r--r--  2.0 unx     2115 b- defN 24-Jun-03 12:08 nucliadb/writer/layouts/v1.py
--rw-r--r--  2.0 unx      835 b- defN 24-Jun-03 12:08 nucliadb/writer/resource/__init__.py
--rw-r--r--  2.0 unx     1425 b- defN 24-Jun-03 12:08 nucliadb/writer/resource/audit.py
--rw-r--r--  2.0 unx    10968 b- defN 24-Jun-03 12:08 nucliadb/writer/resource/basic.py
--rw-r--r--  2.0 unx    16740 b- defN 24-Jun-03 12:08 nucliadb/writer/resource/field.py
--rw-r--r--  2.0 unx     2022 b- defN 24-Jun-03 12:08 nucliadb/writer/resource/origin.py
--rw-r--r--  2.0 unx      835 b- defN 24-Jun-03 12:08 nucliadb/writer/tests/__init__.py
--rw-r--r--  2.0 unx     1200 b- defN 24-Jun-03 12:08 nucliadb/writer/tests/conftest.py
--rw-r--r--  2.0 unx     5971 b- defN 24-Jun-03 12:08 nucliadb/writer/tests/fixtures.py
--rw-r--r--  2.0 unx    15472 b- defN 24-Jun-03 12:08 nucliadb/writer/tests/test_fields.py
--rw-r--r--  2.0 unx    25988 b- defN 24-Jun-03 12:08 nucliadb/writer/tests/test_files.py
--rw-r--r--  2.0 unx     1729 b- defN 24-Jun-03 12:08 nucliadb/writer/tests/test_knowledgebox.py
--rw-r--r--  2.0 unx     4400 b- defN 24-Jun-03 12:08 nucliadb/writer/tests/test_reprocess_file_field.py
--rw-r--r--  2.0 unx    16857 b- defN 24-Jun-03 12:08 nucliadb/writer/tests/test_resources.py
--rw-r--r--  2.0 unx     5120 b- defN 24-Jun-03 12:08 nucliadb/writer/tests/test_service.py
--rw-r--r--  2.0 unx     6054 b- defN 24-Jun-03 12:08 nucliadb/writer/tests/test_tus.py
--rw-r--r--  2.0 unx     1287 b- defN 24-Jun-03 12:08 nucliadb/writer/tests/utils.py
--rw-r--r--  2.0 unx     5226 b- defN 24-Jun-03 12:08 nucliadb/writer/tus/__init__.py
--rw-r--r--  2.0 unx     5082 b- defN 24-Jun-03 12:08 nucliadb/writer/tus/dm.py
--rw-r--r--  2.0 unx     2186 b- defN 24-Jun-03 12:08 nucliadb/writer/tus/exceptions.py
--rw-r--r--  2.0 unx    14527 b- defN 24-Jun-03 12:08 nucliadb/writer/tus/gcs.py
--rw-r--r--  2.0 unx     5849 b- defN 24-Jun-03 12:08 nucliadb/writer/tus/local.py
--rw-r--r--  2.0 unx     4367 b- defN 24-Jun-03 12:08 nucliadb/writer/tus/pg.py
--rw-r--r--  2.0 unx     9069 b- defN 24-Jun-03 12:08 nucliadb/writer/tus/s3.py
--rw-r--r--  2.0 unx     4734 b- defN 24-Jun-03 12:08 nucliadb/writer/tus/storage.py
--rw-r--r--  2.0 unx     2556 b- defN 24-Jun-03 12:08 nucliadb/writer/tus/utils.py
--rw-r--r--  2.0 unx     4474 b- defN 24-Jun-03 12:09 nucliadb-4.0.3.post564.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-Jun-03 12:09 nucliadb-4.0.3.post564.dist-info/WHEEL
--rw-r--r--  2.0 unx     1268 b- defN 24-Jun-03 12:09 nucliadb-4.0.3.post564.dist-info/entry_points.txt
--rw-r--r--  2.0 unx       20 b- defN 24-Jun-03 12:09 nucliadb-4.0.3.post564.dist-info/top_level.txt
--rw-r--r--  2.0 unx        1 b- defN 24-Jun-03 12:09 nucliadb-4.0.3.post564.dist-info/zip-safe
--rw-rw-r--  2.0 unx    44525 b- defN 24-Jun-03 12:09 nucliadb-4.0.3.post564.dist-info/RECORD
-475 files, 2290952 bytes uncompressed, 706271 bytes compressed:  69.2%
+Zip file size: 777843 bytes, number of entries: 475
+-rw-r--r--  2.0 unx     1135 b- defN 24-Jun-03 13:10 migrations/0001_bootstrap.py
+-rw-r--r--  2.0 unx     1177 b- defN 24-Jun-03 13:10 migrations/0002_rollover_shards.py
+-rw-r--r--  2.0 unx     2436 b- defN 24-Jun-03 13:10 migrations/0003_allfields_key.py
+-rw-r--r--  2.0 unx     1177 b- defN 24-Jun-03 13:10 migrations/0004_rollover_shards.py
+-rw-r--r--  2.0 unx     1177 b- defN 24-Jun-03 13:10 migrations/0005_rollover_shards.py
+-rw-r--r--  2.0 unx     1024 b- defN 24-Jun-03 13:10 migrations/0006_rollover_shards.py
+-rw-r--r--  2.0 unx     1301 b- defN 24-Jun-03 13:10 migrations/0008_cleanup_leftover_rollover_metadata.py
+-rw-r--r--  2.0 unx     1378 b- defN 24-Jun-03 13:10 migrations/0009_upgrade_relations_and_texts_to_v2.py
+-rw-r--r--  2.0 unx     1610 b- defN 24-Jun-03 13:10 migrations/0010_fix_corrupt_indexes.py
+-rw-r--r--  2.0 unx     1843 b- defN 24-Jun-03 13:10 migrations/0011_materialize_labelset_ids.py
+-rw-r--r--  2.0 unx     1443 b- defN 24-Jun-03 13:10 migrations/0012_rollover_shards.py
+-rw-r--r--  2.0 unx     1024 b- defN 24-Jun-03 13:10 migrations/0013_rollover_shards.py
+-rw-r--r--  2.0 unx     1382 b- defN 24-Jun-03 13:10 migrations/0014_rollover_shards.py
+-rw-r--r--  2.0 unx     1462 b- defN 24-Jun-03 13:10 migrations/0015_targeted_rollover.py
+-rw-r--r--  2.0 unx     2506 b- defN 24-Jun-03 13:10 migrations/0016_upgrade_to_paragraphs_v2.py
+-rw-r--r--  2.0 unx     2100 b- defN 24-Jun-03 13:10 migrations/0017_multiple_writable_shards.py
+-rw-r--r--  2.0 unx     2264 b- defN 24-Jun-03 13:10 migrations/0018_purge_orphan_kbslugs.py
+-rw-r--r--  2.0 unx     2506 b- defN 24-Jun-03 13:10 migrations/0019_upgrade_to_paragraphs_v3.py
+-rw-r--r--  2.0 unx     3271 b- defN 24-Jun-03 13:10 migrations/0020_drain_nodes_from_cluster.py
+-rw-r--r--  2.0 unx     1734 b- defN 24-Jun-03 13:10 migrations/0021_overwrite_vectorsets_key.py
+-rw-r--r--  2.0 unx      835 b- defN 24-Jun-03 13:10 migrations/__init__.py
+-rw-r--r--  2.0 unx      891 b- defN 24-Jun-03 13:10 nucliadb/__init__.py
+-rw-r--r--  2.0 unx     3733 b- defN 24-Jun-03 13:10 nucliadb/health.py
+-rw-r--r--  2.0 unx    11793 b- defN 24-Jun-03 13:10 nucliadb/learning_proxy.py
+-rw-r--r--  2.0 unx     4820 b- defN 24-Jun-03 13:10 nucliadb/metrics_exporter.py
+-rw-r--r--  2.0 unx     2272 b- defN 24-Jun-03 13:10 nucliadb/openapi.py
+-rw-r--r--  2.0 unx        0 b- defN 24-Jun-03 13:10 nucliadb/py.typed
+-rw-r--r--  2.0 unx      835 b- defN 24-Jun-03 13:10 nucliadb/common/__init__.py
+-rw-r--r--  2.0 unx     1912 b- defN 24-Jun-03 13:10 nucliadb/common/ids.py
+-rw-r--r--  2.0 unx     5175 b- defN 24-Jun-03 13:10 nucliadb/common/locking.py
+-rw-r--r--  2.0 unx      835 b- defN 24-Jun-03 13:10 nucliadb/common/cluster/__init__.py
+-rw-r--r--  2.0 unx     5134 b- defN 24-Jun-03 13:10 nucliadb/common/cluster/base.py
+-rw-r--r--  2.0 unx     1495 b- defN 24-Jun-03 13:10 nucliadb/common/cluster/exceptions.py
+-rw-r--r--  2.0 unx     3793 b- defN 24-Jun-03 13:10 nucliadb/common/cluster/grpc_node_dummy.py
+-rw-r--r--  2.0 unx     3429 b- defN 24-Jun-03 13:10 nucliadb/common/cluster/index_node.py
+-rw-r--r--  2.0 unx    24804 b- defN 24-Jun-03 13:10 nucliadb/common/cluster/manager.py
+-rw-r--r--  2.0 unx     8831 b- defN 24-Jun-03 13:10 nucliadb/common/cluster/rebalance.py
+-rw-r--r--  2.0 unx    20532 b- defN 24-Jun-03 13:10 nucliadb/common/cluster/rollover.py
+-rw-r--r--  2.0 unx     3016 b- defN 24-Jun-03 13:10 nucliadb/common/cluster/settings.py
+-rw-r--r--  2.0 unx     5715 b- defN 24-Jun-03 13:10 nucliadb/common/cluster/utils.py
+-rw-r--r--  2.0 unx      835 b- defN 24-Jun-03 13:10 nucliadb/common/cluster/discovery/__init__.py
+-rw-r--r--  2.0 unx     6553 b- defN 24-Jun-03 13:10 nucliadb/common/cluster/discovery/base.py
+-rw-r--r--  2.0 unx    12512 b- defN 24-Jun-03 13:10 nucliadb/common/cluster/discovery/k8s.py
+-rw-r--r--  2.0 unx     1957 b- defN 24-Jun-03 13:10 nucliadb/common/cluster/discovery/manual.py
+-rw-r--r--  2.0 unx     1737 b- defN 24-Jun-03 13:10 nucliadb/common/cluster/discovery/single.py
+-rw-r--r--  2.0 unx     1139 b- defN 24-Jun-03 13:10 nucliadb/common/cluster/discovery/types.py
+-rw-r--r--  2.0 unx     2548 b- defN 24-Jun-03 13:10 nucliadb/common/cluster/discovery/utils.py
+-rw-r--r--  2.0 unx      833 b- defN 24-Jun-03 13:10 nucliadb/common/cluster/standalone/__init__.py
+-rw-r--r--  2.0 unx    13712 b- defN 24-Jun-03 13:10 nucliadb/common/cluster/standalone/grpc_node_binding.py
+-rw-r--r--  2.0 unx     4683 b- defN 24-Jun-03 13:10 nucliadb/common/cluster/standalone/index_node.py
+-rw-r--r--  2.0 unx     3444 b- defN 24-Jun-03 13:10 nucliadb/common/cluster/standalone/service.py
+-rw-r--r--  2.0 unx     3545 b- defN 24-Jun-03 13:10 nucliadb/common/cluster/standalone/utils.py
+-rw-r--r--  2.0 unx     3440 b- defN 24-Jun-03 13:10 nucliadb/common/context/__init__.py
+-rw-r--r--  2.0 unx     1628 b- defN 24-Jun-03 13:10 nucliadb/common/context/fastapi.py
+-rw-r--r--  2.0 unx     2062 b- defN 24-Jun-03 13:10 nucliadb/common/datamanagers/__init__.py
+-rw-r--r--  2.0 unx     3095 b- defN 24-Jun-03 13:10 nucliadb/common/datamanagers/atomic.py
+-rw-r--r--  2.0 unx     1451 b- defN 24-Jun-03 13:10 nucliadb/common/datamanagers/cluster.py
+-rw-r--r--  2.0 unx     5383 b- defN 24-Jun-03 13:10 nucliadb/common/datamanagers/entities.py
+-rw-r--r--  2.0 unx      883 b- defN 24-Jun-03 13:10 nucliadb/common/datamanagers/exceptions.py
+-rw-r--r--  2.0 unx     2764 b- defN 24-Jun-03 13:10 nucliadb/common/datamanagers/fields.py
+-rw-r--r--  2.0 unx     3994 b- defN 24-Jun-03 13:10 nucliadb/common/datamanagers/kb.py
+-rw-r--r--  2.0 unx     5389 b- defN 24-Jun-03 13:10 nucliadb/common/datamanagers/labels.py
+-rw-r--r--  2.0 unx     1599 b- defN 24-Jun-03 13:10 nucliadb/common/datamanagers/processing.py
+-rw-r--r--  2.0 unx    11931 b- defN 24-Jun-03 13:10 nucliadb/common/datamanagers/resources.py
+-rw-r--r--  2.0 unx     5643 b- defN 24-Jun-03 13:10 nucliadb/common/datamanagers/rollover.py
+-rw-r--r--  2.0 unx     1548 b- defN 24-Jun-03 13:10 nucliadb/common/datamanagers/synonyms.py
+-rw-r--r--  2.0 unx     1923 b- defN 24-Jun-03 13:10 nucliadb/common/datamanagers/utils.py
+-rw-r--r--  2.0 unx     3780 b- defN 24-Jun-03 13:10 nucliadb/common/datamanagers/vectorsets.py
+-rw-r--r--  2.0 unx      835 b- defN 24-Jun-03 13:10 nucliadb/common/http_clients/__init__.py
+-rw-r--r--  2.0 unx     2146 b- defN 24-Jun-03 13:10 nucliadb/common/http_clients/auth.py
+-rw-r--r--  2.0 unx     1100 b- defN 24-Jun-03 13:10 nucliadb/common/http_clients/exceptions.py
+-rw-r--r--  2.0 unx     7155 b- defN 24-Jun-03 13:10 nucliadb/common/http_clients/processing.py
+-rw-r--r--  2.0 unx     1540 b- defN 24-Jun-03 13:10 nucliadb/common/http_clients/pypi.py
+-rw-r--r--  2.0 unx     1551 b- defN 24-Jun-03 13:10 nucliadb/common/http_clients/utils.py
+-rw-r--r--  2.0 unx      835 b- defN 24-Jun-03 13:10 nucliadb/common/maindb/__init__.py
+-rw-r--r--  2.0 unx     3449 b- defN 24-Jun-03 13:10 nucliadb/common/maindb/driver.py
+-rw-r--r--  2.0 unx      988 b- defN 24-Jun-03 13:10 nucliadb/common/maindb/exceptions.py
+-rw-r--r--  2.0 unx     6769 b- defN 24-Jun-03 13:10 nucliadb/common/maindb/local.py
+-rw-r--r--  2.0 unx    10484 b- defN 24-Jun-03 13:10 nucliadb/common/maindb/pg.py
+-rw-r--r--  2.0 unx     6053 b- defN 24-Jun-03 13:10 nucliadb/common/maindb/redis.py
+-rw-r--r--  2.0 unx    15209 b- defN 24-Jun-03 13:10 nucliadb/common/maindb/tikv.py
+-rw-r--r--  2.0 unx     4233 b- defN 24-Jun-03 13:10 nucliadb/common/maindb/utils.py
+-rw-r--r--  2.0 unx      932 b- defN 24-Jun-03 13:10 nucliadb/export_import/__init__.py
+-rw-r--r--  2.0 unx     6185 b- defN 24-Jun-03 13:10 nucliadb/export_import/datamanager.py
+-rw-r--r--  2.0 unx     1949 b- defN 24-Jun-03 13:10 nucliadb/export_import/exceptions.py
+-rw-r--r--  2.0 unx     7116 b- defN 24-Jun-03 13:10 nucliadb/export_import/exporter.py
+-rw-r--r--  2.0 unx     4258 b- defN 24-Jun-03 13:10 nucliadb/export_import/importer.py
+-rw-r--r--  2.0 unx     2063 b- defN 24-Jun-03 13:10 nucliadb/export_import/models.py
+-rw-r--r--  2.0 unx     2571 b- defN 24-Jun-03 13:10 nucliadb/export_import/tasks.py
+-rw-r--r--  2.0 unx    19655 b- defN 24-Jun-03 13:10 nucliadb/export_import/utils.py
+-rw-r--r--  2.0 unx     1011 b- defN 24-Jun-03 13:10 nucliadb/ingest/__init__.py
+-rw-r--r--  2.0 unx     7277 b- defN 24-Jun-03 13:10 nucliadb/ingest/app.py
+-rw-r--r--  2.0 unx     1005 b- defN 24-Jun-03 13:10 nucliadb/ingest/cache.py
+-rw-r--r--  2.0 unx     2484 b- defN 24-Jun-03 13:10 nucliadb/ingest/partitions.py
+-rw-r--r--  2.0 unx    19904 b- defN 24-Jun-03 13:10 nucliadb/ingest/processing.py
+-rw-r--r--  2.0 unx        0 b- defN 24-Jun-03 13:10 nucliadb/ingest/py.typed
+-rw-r--r--  2.0 unx    20291 b- defN 24-Jun-03 13:10 nucliadb/ingest/serialize.py
+-rw-r--r--  2.0 unx     3348 b- defN 24-Jun-03 13:10 nucliadb/ingest/settings.py
+-rw-r--r--  2.0 unx     2314 b- defN 24-Jun-03 13:10 nucliadb/ingest/utils.py
+-rw-r--r--  2.0 unx      835 b- defN 24-Jun-03 13:10 nucliadb/ingest/consumer/__init__.py
+-rw-r--r--  2.0 unx     6918 b- defN 24-Jun-03 13:10 nucliadb/ingest/consumer/auditing.py
+-rw-r--r--  2.0 unx    12174 b- defN 24-Jun-03 13:10 nucliadb/ingest/consumer/consumer.py
+-rw-r--r--  2.0 unx     3934 b- defN 24-Jun-03 13:10 nucliadb/ingest/consumer/materializer.py
+-rw-r--r--  2.0 unx     1075 b- defN 24-Jun-03 13:10 nucliadb/ingest/consumer/metrics.py
+-rw-r--r--  2.0 unx     9546 b- defN 24-Jun-03 13:10 nucliadb/ingest/consumer/pull.py
+-rw-r--r--  2.0 unx     6871 b- defN 24-Jun-03 13:10 nucliadb/ingest/consumer/service.py
+-rw-r--r--  2.0 unx     4331 b- defN 24-Jun-03 13:10 nucliadb/ingest/consumer/shard_creator.py
+-rw-r--r--  2.0 unx     2656 b- defN 24-Jun-03 13:10 nucliadb/ingest/consumer/utils.py
+-rw-r--r--  2.0 unx      835 b- defN 24-Jun-03 13:10 nucliadb/ingest/fields/__init__.py
+-rw-r--r--  2.0 unx    17797 b- defN 24-Jun-03 13:10 nucliadb/ingest/fields/base.py
+-rw-r--r--  2.0 unx     7047 b- defN 24-Jun-03 13:10 nucliadb/ingest/fields/conversation.py
+-rw-r--r--  2.0 unx     1223 b- defN 24-Jun-03 13:10 nucliadb/ingest/fields/date.py
+-rw-r--r--  2.0 unx     1205 b- defN 24-Jun-03 13:10 nucliadb/ingest/fields/exceptions.py
+-rw-r--r--  2.0 unx     4840 b- defN 24-Jun-03 13:10 nucliadb/ingest/fields/file.py
+-rw-r--r--  2.0 unx     1547 b- defN 24-Jun-03 13:10 nucliadb/ingest/fields/generic.py
+-rw-r--r--  2.0 unx     1235 b- defN 24-Jun-03 13:10 nucliadb/ingest/fields/keywordset.py
+-rw-r--r--  2.0 unx     2250 b- defN 24-Jun-03 13:10 nucliadb/ingest/fields/layout.py
+-rw-r--r--  2.0 unx     4212 b- defN 24-Jun-03 13:10 nucliadb/ingest/fields/link.py
+-rw-r--r--  2.0 unx     1319 b- defN 24-Jun-03 13:10 nucliadb/ingest/fields/text.py
+-rw-r--r--  2.0 unx      835 b- defN 24-Jun-03 13:10 nucliadb/ingest/orm/__init__.py
+-rw-r--r--  2.0 unx    28721 b- defN 24-Jun-03 13:10 nucliadb/ingest/orm/brain.py
+-rw-r--r--  2.0 unx     6954 b- defN 24-Jun-03 13:10 nucliadb/ingest/orm/broker_message.py
+-rw-r--r--  2.0 unx    15758 b- defN 24-Jun-03 13:10 nucliadb/ingest/orm/entities.py
+-rw-r--r--  2.0 unx     1326 b- defN 24-Jun-03 13:10 nucliadb/ingest/orm/exceptions.py
+-rw-r--r--  2.0 unx    16068 b- defN 24-Jun-03 13:10 nucliadb/ingest/orm/knowledgebox.py
+-rw-r--r--  2.0 unx     1096 b- defN 24-Jun-03 13:10 nucliadb/ingest/orm/metrics.py
+-rw-r--r--  2.0 unx    54798 b- defN 24-Jun-03 13:10 nucliadb/ingest/orm/resource.py
+-rw-r--r--  2.0 unx     2685 b- defN 24-Jun-03 13:10 nucliadb/ingest/orm/utils.py
+-rw-r--r--  2.0 unx    27092 b- defN 24-Jun-03 13:10 nucliadb/ingest/orm/processor/__init__.py
+-rw-r--r--  2.0 unx     5104 b- defN 24-Jun-03 13:10 nucliadb/ingest/orm/processor/auditing.py
+-rw-r--r--  2.0 unx     1704 b- defN 24-Jun-03 13:10 nucliadb/ingest/orm/processor/sequence_manager.py
+-rw-r--r--  2.0 unx     2057 b- defN 24-Jun-03 13:10 nucliadb/ingest/service/__init__.py
+-rw-r--r--  2.0 unx      835 b- defN 24-Jun-03 13:10 nucliadb/ingest/service/exceptions.py
+-rw-r--r--  2.0 unx    29886 b- defN 24-Jun-03 13:10 nucliadb/ingest/service/writer.py
+-rw-r--r--  2.0 unx      835 b- defN 24-Jun-03 13:10 nucliadb/ingest/tests/__init__.py
+-rw-r--r--  2.0 unx     1157 b- defN 24-Jun-03 13:10 nucliadb/ingest/tests/conftest.py
+-rw-r--r--  2.0 unx    24111 b- defN 24-Jun-03 13:10 nucliadb/ingest/tests/fixtures.py
+-rw-r--r--  2.0 unx    62843 b- defN 24-Jun-03 13:10 nucliadb/ingest/tests/vectors.py
+-rw-r--r--  2.0 unx      835 b- defN 24-Jun-03 13:10 nucliadb/ingest/tests/integration/__init__.py
+-rw-r--r--  2.0 unx      833 b- defN 24-Jun-03 13:10 nucliadb/ingest/tests/integration/consumer/__init__.py
+-rw-r--r--  2.0 unx     2500 b- defN 24-Jun-03 13:10 nucliadb/ingest/tests/integration/consumer/test_auditing.py
+-rw-r--r--  2.0 unx     3836 b- defN 24-Jun-03 13:10 nucliadb/ingest/tests/integration/consumer/test_materializer.py
+-rw-r--r--  2.0 unx     4470 b- defN 24-Jun-03 13:10 nucliadb/ingest/tests/integration/consumer/test_pull.py
+-rw-r--r--  2.0 unx     2763 b- defN 24-Jun-03 13:10 nucliadb/ingest/tests/integration/consumer/test_service.py
+-rw-r--r--  2.0 unx     2019 b- defN 24-Jun-03 13:10 nucliadb/ingest/tests/integration/consumer/test_shard_creator.py
+-rw-r--r--  2.0 unx      835 b- defN 24-Jun-03 13:10 nucliadb/ingest/tests/integration/ingest/__init__.py
+-rw-r--r--  2.0 unx    27247 b- defN 24-Jun-03 13:10 nucliadb/ingest/tests/integration/ingest/test_ingest.py
+-rw-r--r--  2.0 unx     3040 b- defN 24-Jun-03 13:10 nucliadb/ingest/tests/integration/ingest/test_processing_engine.py
+-rw-r--r--  2.0 unx     8586 b- defN 24-Jun-03 13:10 nucliadb/ingest/tests/integration/ingest/test_relations.py
+-rw-r--r--  2.0 unx     5637 b- defN 24-Jun-03 13:10 nucliadb/ingest/tests/integration/ingest/test_vectorsets.py
+-rw-r--r--  2.0 unx      835 b- defN 24-Jun-03 13:10 nucliadb/ingest/tests/unit/__init__.py
+-rw-r--r--  2.0 unx     1189 b- defN 24-Jun-03 13:10 nucliadb/ingest/tests/unit/test_cache.py
+-rw-r--r--  2.0 unx     1432 b- defN 24-Jun-03 13:10 nucliadb/ingest/tests/unit/test_partitions.py
+-rw-r--r--  2.0 unx     5807 b- defN 24-Jun-03 13:10 nucliadb/ingest/tests/unit/test_processing.py
+-rw-r--r--  2.0 unx      978 b- defN 24-Jun-03 13:10 nucliadb/ingest/tests/unit/test_settings.py
+-rw-r--r--  2.0 unx      833 b- defN 24-Jun-03 13:10 nucliadb/ingest/tests/unit/consumer/__init__.py
+-rw-r--r--  2.0 unx     3885 b- defN 24-Jun-03 13:10 nucliadb/ingest/tests/unit/consumer/test_auditing.py
+-rw-r--r--  2.0 unx     2472 b- defN 24-Jun-03 13:10 nucliadb/ingest/tests/unit/consumer/test_consumer.py
+-rw-r--r--  2.0 unx     2063 b- defN 24-Jun-03 13:10 nucliadb/ingest/tests/unit/consumer/test_pull.py
+-rw-r--r--  2.0 unx     4140 b- defN 24-Jun-03 13:10 nucliadb/ingest/tests/unit/consumer/test_shard_creator.py
+-rw-r--r--  2.0 unx     1934 b- defN 24-Jun-03 13:10 nucliadb/ingest/tests/unit/consumer/test_utils.py
+-rw-r--r--  2.0 unx      835 b- defN 24-Jun-03 13:10 nucliadb/ingest/tests/unit/orm/__init__.py
+-rw-r--r--  2.0 unx     9876 b- defN 24-Jun-03 13:10 nucliadb/ingest/tests/unit/orm/test_brain.py
+-rw-r--r--  2.0 unx     2572 b- defN 24-Jun-03 13:10 nucliadb/ingest/tests/unit/orm/test_brain_vectors.py
+-rw-r--r--  2.0 unx     1174 b- defN 24-Jun-03 13:10 nucliadb/ingest/tests/unit/orm/test_orm_utils.py
+-rw-r--r--  2.0 unx     4045 b- defN 24-Jun-03 13:10 nucliadb/ingest/tests/unit/orm/test_processor.py
+-rw-r--r--  2.0 unx    11033 b- defN 24-Jun-03 13:10 nucliadb/ingest/tests/unit/orm/test_resource.py
+-rw-r--r--  2.0 unx     2216 b- defN 24-Jun-03 13:10 nucliadb/middleware/__init__.py
+-rw-r--r--  2.0 unx     3912 b- defN 24-Jun-03 13:10 nucliadb/middleware/transaction.py
+-rw-r--r--  2.0 unx      835 b- defN 24-Jun-03 13:10 nucliadb/migrator/__init__.py
+-rw-r--r--  2.0 unx     2119 b- defN 24-Jun-03 13:10 nucliadb/migrator/command.py
+-rw-r--r--  2.0 unx     1334 b- defN 24-Jun-03 13:10 nucliadb/migrator/context.py
+-rw-r--r--  2.0 unx     5104 b- defN 24-Jun-03 13:10 nucliadb/migrator/datamanager.py
+-rw-r--r--  2.0 unx      889 b- defN 24-Jun-03 13:10 nucliadb/migrator/exceptions.py
+-rw-r--r--  2.0 unx     9370 b- defN 24-Jun-03 13:10 nucliadb/migrator/migrator.py
+-rw-r--r--  2.0 unx     1145 b- defN 24-Jun-03 13:10 nucliadb/migrator/models.py
+-rw-r--r--  2.0 unx     1144 b- defN 24-Jun-03 13:10 nucliadb/migrator/settings.py
+-rw-r--r--  2.0 unx     2346 b- defN 24-Jun-03 13:10 nucliadb/migrator/utils.py
+-rw-r--r--  2.0 unx      835 b- defN 24-Jun-03 13:10 nucliadb/models/__init__.py
+-rw-r--r--  2.0 unx     1599 b- defN 24-Jun-03 13:10 nucliadb/models/responses.py
+-rw-r--r--  2.0 unx     6041 b- defN 24-Jun-03 13:10 nucliadb/purge/__init__.py
+-rw-r--r--  2.0 unx     9367 b- defN 24-Jun-03 13:10 nucliadb/purge/orphan_shards.py
+-rw-r--r--  2.0 unx     1328 b- defN 24-Jun-03 13:10 nucliadb/reader/__init__.py
+-rw-r--r--  2.0 unx     3709 b- defN 24-Jun-03 13:10 nucliadb/reader/app.py
+-rw-r--r--  2.0 unx     1366 b- defN 24-Jun-03 13:10 nucliadb/reader/lifecycle.py
+-rw-r--r--  2.0 unx     1031 b- defN 24-Jun-03 13:10 nucliadb/reader/openapi.py
+-rw-r--r--  2.0 unx        0 b- defN 24-Jun-03 13:10 nucliadb/reader/py.typed
+-rw-r--r--  2.0 unx     1447 b- defN 24-Jun-03 13:10 nucliadb/reader/run.py
+-rw-r--r--  2.0 unx      872 b- defN 24-Jun-03 13:10 nucliadb/reader/api/__init__.py
+-rw-r--r--  2.0 unx     2458 b- defN 24-Jun-03 13:10 nucliadb/reader/api/models.py
+-rw-r--r--  2.0 unx     1110 b- defN 24-Jun-03 13:10 nucliadb/reader/api/v1/__init__.py
+-rw-r--r--  2.0 unx    12457 b- defN 24-Jun-03 13:10 nucliadb/reader/api/v1/download.py
+-rw-r--r--  2.0 unx     6448 b- defN 24-Jun-03 13:10 nucliadb/reader/api/v1/export_import.py
+-rw-r--r--  2.0 unx     3641 b- defN 24-Jun-03 13:10 nucliadb/reader/api/v1/knowledgebox.py
+-rw-r--r--  2.0 unx     2099 b- defN 24-Jun-03 13:10 nucliadb/reader/api/v1/learning_collector.py
+-rw-r--r--  2.0 unx     4472 b- defN 24-Jun-03 13:10 nucliadb/reader/api/v1/learning_config.py
+-rw-r--r--  2.0 unx    13961 b- defN 24-Jun-03 13:10 nucliadb/reader/api/v1/resource.py
+-rw-r--r--  2.0 unx     1011 b- defN 24-Jun-03 13:10 nucliadb/reader/api/v1/router.py
+-rw-r--r--  2.0 unx    11902 b- defN 24-Jun-03 13:10 nucliadb/reader/api/v1/services.py
+-rw-r--r--  2.0 unx      835 b- defN 24-Jun-03 13:10 nucliadb/reader/reader/__init__.py
+-rw-r--r--  2.0 unx     7979 b- defN 24-Jun-03 13:10 nucliadb/reader/reader/notifications.py
+-rw-r--r--  2.0 unx      835 b- defN 24-Jun-03 13:10 nucliadb/reader/tests/__init__.py
+-rw-r--r--  2.0 unx     1224 b- defN 24-Jun-03 13:10 nucliadb/reader/tests/conftest.py
+-rw-r--r--  2.0 unx     4355 b- defN 24-Jun-03 13:10 nucliadb/reader/tests/fixtures.py
+-rw-r--r--  2.0 unx     2748 b- defN 24-Jun-03 13:10 nucliadb/reader/tests/test_list_resources.py
+-rw-r--r--  2.0 unx    10199 b- defN 24-Jun-03 13:10 nucliadb/reader/tests/test_reader_file_download.py
+-rw-r--r--  2.0 unx    10586 b- defN 24-Jun-03 13:10 nucliadb/reader/tests/test_reader_resource.py
+-rw-r--r--  2.0 unx     6535 b- defN 24-Jun-03 13:10 nucliadb/reader/tests/test_reader_resource_field.py
+-rw-r--r--  2.0 unx     1535 b- defN 24-Jun-03 13:10 nucliadb/search/__init__.py
+-rw-r--r--  2.0 unx     4905 b- defN 24-Jun-03 13:10 nucliadb/search/app.py
+-rw-r--r--  2.0 unx     1956 b- defN 24-Jun-03 13:10 nucliadb/search/lifecycle.py
+-rw-r--r--  2.0 unx     1016 b- defN 24-Jun-03 13:10 nucliadb/search/openapi.py
+-rw-r--r--  2.0 unx    20665 b- defN 24-Jun-03 13:10 nucliadb/search/predict.py
+-rw-r--r--  2.0 unx        0 b- defN 24-Jun-03 13:10 nucliadb/search/py.typed
+-rw-r--r--  2.0 unx     1402 b- defN 24-Jun-03 13:10 nucliadb/search/run.py
+-rw-r--r--  2.0 unx     1193 b- defN 24-Jun-03 13:10 nucliadb/search/settings.py
+-rw-r--r--  2.0 unx     1037 b- defN 24-Jun-03 13:10 nucliadb/search/utilities.py
+-rw-r--r--  2.0 unx      835 b- defN 24-Jun-03 13:10 nucliadb/search/api/__init__.py
+-rw-r--r--  2.0 unx     1298 b- defN 24-Jun-03 13:10 nucliadb/search/api/v1/__init__.py
+-rw-r--r--  2.0 unx     3435 b- defN 24-Jun-03 13:10 nucliadb/search/api/v1/ask.py
+-rw-r--r--  2.0 unx     9514 b- defN 24-Jun-03 13:10 nucliadb/search/api/v1/chat.py
+-rw-r--r--  2.0 unx     2668 b- defN 24-Jun-03 13:10 nucliadb/search/api/v1/feedback.py
+-rw-r--r--  2.0 unx     8795 b- defN 24-Jun-03 13:10 nucliadb/search/api/v1/find.py
+-rw-r--r--  2.0 unx     6941 b- defN 24-Jun-03 13:10 nucliadb/search/api/v1/knowledgebox.py
+-rw-r--r--  2.0 unx     3047 b- defN 24-Jun-03 13:10 nucliadb/search/api/v1/predict_proxy.py
+-rw-r--r--  2.0 unx      988 b- defN 24-Jun-03 13:10 nucliadb/search/api/v1/router.py
+-rw-r--r--  2.0 unx    19262 b- defN 24-Jun-03 13:10 nucliadb/search/api/v1/search.py
+-rw-r--r--  2.0 unx     5970 b- defN 24-Jun-03 13:10 nucliadb/search/api/v1/suggest.py
+-rw-r--r--  2.0 unx     2499 b- defN 24-Jun-03 13:10 nucliadb/search/api/v1/summarize.py
+-rw-r--r--  2.0 unx     1434 b- defN 24-Jun-03 13:10 nucliadb/search/api/v1/utils.py
+-rw-r--r--  2.0 unx      835 b- defN 24-Jun-03 13:10 nucliadb/search/api/v1/resource/__init__.py
+-rw-r--r--  2.0 unx     3869 b- defN 24-Jun-03 13:10 nucliadb/search/api/v1/resource/ask.py
+-rw-r--r--  2.0 unx     5866 b- defN 24-Jun-03 13:10 nucliadb/search/api/v1/resource/chat.py
+-rw-r--r--  2.0 unx     5303 b- defN 24-Jun-03 13:10 nucliadb/search/api/v1/resource/search.py
+-rw-r--r--  2.0 unx      833 b- defN 24-Jun-03 13:10 nucliadb/search/requesters/__init__.py
+-rw-r--r--  2.0 unx     9111 b- defN 24-Jun-03 13:10 nucliadb/search/requesters/utils.py
+-rw-r--r--  2.0 unx      835 b- defN 24-Jun-03 13:10 nucliadb/search/search/__init__.py
+-rw-r--r--  2.0 unx     2746 b- defN 24-Jun-03 13:10 nucliadb/search/search/cache.py
+-rw-r--r--  2.0 unx     1154 b- defN 24-Jun-03 13:10 nucliadb/search/search/exceptions.py
+-rw-r--r--  2.0 unx     5465 b- defN 24-Jun-03 13:10 nucliadb/search/search/fetch.py
+-rw-r--r--  2.0 unx     6513 b- defN 24-Jun-03 13:10 nucliadb/search/search/filters.py
+-rw-r--r--  2.0 unx     4612 b- defN 24-Jun-03 13:10 nucliadb/search/search/find.py
+-rw-r--r--  2.0 unx    17152 b- defN 24-Jun-03 13:10 nucliadb/search/search/find_merge.py
+-rw-r--r--  2.0 unx    21282 b- defN 24-Jun-03 13:10 nucliadb/search/search/merge.py
+-rw-r--r--  2.0 unx     1130 b- defN 24-Jun-03 13:10 nucliadb/search/search/metrics.py
+-rw-r--r--  2.0 unx     8698 b- defN 24-Jun-03 13:10 nucliadb/search/search/paragraphs.py
+-rw-r--r--  2.0 unx     3015 b- defN 24-Jun-03 13:10 nucliadb/search/search/predict_proxy.py
+-rw-r--r--  2.0 unx    31093 b- defN 24-Jun-03 13:10 nucliadb/search/search/query.py
+-rw-r--r--  2.0 unx     3018 b- defN 24-Jun-03 13:10 nucliadb/search/search/shards.py
+-rw-r--r--  2.0 unx     5101 b- defN 24-Jun-03 13:10 nucliadb/search/search/summarize.py
+-rw-r--r--  2.0 unx     2438 b- defN 24-Jun-03 13:10 nucliadb/search/search/utils.py
+-rw-r--r--  2.0 unx      835 b- defN 24-Jun-03 13:10 nucliadb/search/search/chat/__init__.py
+-rw-r--r--  2.0 unx    16676 b- defN 24-Jun-03 13:10 nucliadb/search/search/chat/ask.py
+-rw-r--r--  2.0 unx     2058 b- defN 24-Jun-03 13:10 nucliadb/search/search/chat/images.py
+-rw-r--r--  2.0 unx    20793 b- defN 24-Jun-03 13:10 nucliadb/search/search/chat/prompt.py
+-rw-r--r--  2.0 unx    17543 b- defN 24-Jun-03 13:10 nucliadb/search/search/chat/query.py
+-rw-r--r--  2.0 unx      835 b- defN 24-Jun-03 13:10 nucliadb/search/tests/__init__.py
+-rw-r--r--  2.0 unx     1295 b- defN 24-Jun-03 13:10 nucliadb/search/tests/conftest.py
+-rw-r--r--  2.0 unx     6578 b- defN 24-Jun-03 13:10 nucliadb/search/tests/fixtures.py
+-rw-r--r--  2.0 unx    15480 b- defN 24-Jun-03 13:10 nucliadb/search/tests/node.py
+-rw-r--r--  2.0 unx      833 b- defN 24-Jun-03 13:10 nucliadb/search/tests/unit/__init__.py
+-rw-r--r--  2.0 unx     2649 b- defN 24-Jun-03 13:10 nucliadb/search/tests/unit/test_app.py
+-rw-r--r--  2.0 unx     3374 b- defN 24-Jun-03 13:10 nucliadb/search/tests/unit/test_find_merge.py
+-rw-r--r--  2.0 unx     1400 b- defN 24-Jun-03 13:10 nucliadb/search/tests/unit/test_merge.py
+-rw-r--r--  2.0 unx    15721 b- defN 24-Jun-03 13:10 nucliadb/search/tests/unit/test_predict.py
+-rw-r--r--  2.0 unx     1328 b- defN 24-Jun-03 13:10 nucliadb/search/tests/unit/test_run.py
+-rw-r--r--  2.0 unx      835 b- defN 24-Jun-03 13:10 nucliadb/search/tests/unit/api/__init__.py
+-rw-r--r--  2.0 unx      835 b- defN 24-Jun-03 13:10 nucliadb/search/tests/unit/api/v1/__init__.py
+-rw-r--r--  2.0 unx     3759 b- defN 24-Jun-03 13:10 nucliadb/search/tests/unit/api/v1/test_ask.py
+-rw-r--r--  2.0 unx     2966 b- defN 24-Jun-03 13:10 nucliadb/search/tests/unit/api/v1/test_chat.py
+-rw-r--r--  2.0 unx     2865 b- defN 24-Jun-03 13:10 nucliadb/search/tests/unit/api/v1/test_predict_proxy.py
+-rw-r--r--  2.0 unx     2901 b- defN 24-Jun-03 13:10 nucliadb/search/tests/unit/api/v1/test_summarize.py
+-rw-r--r--  2.0 unx      835 b- defN 24-Jun-03 13:10 nucliadb/search/tests/unit/api/v1/resource/__init__.py
+-rw-r--r--  2.0 unx     3040 b- defN 24-Jun-03 13:10 nucliadb/search/tests/unit/api/v1/resource/test_chat.py
+-rw-r--r--  2.0 unx      833 b- defN 24-Jun-03 13:10 nucliadb/search/tests/unit/search/__init__.py
+-rw-r--r--  2.0 unx     8586 b- defN 24-Jun-03 13:10 nucliadb/search/tests/unit/search/test_chat_prompt.py
+-rw-r--r--  2.0 unx     3736 b- defN 24-Jun-03 13:10 nucliadb/search/tests/unit/search/test_fetch.py
+-rw-r--r--  2.0 unx     4306 b- defN 24-Jun-03 13:10 nucliadb/search/tests/unit/search/test_filters.py
+-rw-r--r--  2.0 unx     4492 b- defN 24-Jun-03 13:10 nucliadb/search/tests/unit/search/test_paragraphs.py
+-rw-r--r--  2.0 unx     3496 b- defN 24-Jun-03 13:10 nucliadb/search/tests/unit/search/test_predict_proxy.py
+-rw-r--r--  2.0 unx     5121 b- defN 24-Jun-03 13:10 nucliadb/search/tests/unit/search/test_query.py
+-rw-r--r--  2.0 unx      833 b- defN 24-Jun-03 13:10 nucliadb/search/tests/unit/search/requesters/__init__.py
+-rw-r--r--  2.0 unx     6455 b- defN 24-Jun-03 13:10 nucliadb/search/tests/unit/search/requesters/test_utils.py
+-rw-r--r--  2.0 unx      835 b- defN 24-Jun-03 13:10 nucliadb/search/tests/unit/search/search/__init__.py
+-rw-r--r--  2.0 unx     1759 b- defN 24-Jun-03 13:10 nucliadb/search/tests/unit/search/search/test_shards.py
+-rw-r--r--  2.0 unx     2511 b- defN 24-Jun-03 13:10 nucliadb/search/tests/unit/search/search/test_utils.py
+-rw-r--r--  2.0 unx      835 b- defN 24-Jun-03 13:10 nucliadb/standalone/__init__.py
+-rw-r--r--  2.0 unx     6749 b- defN 24-Jun-03 13:10 nucliadb/standalone/api_router.py
+-rw-r--r--  2.0 unx     5763 b- defN 24-Jun-03 13:10 nucliadb/standalone/app.py
+-rw-r--r--  2.0 unx     7800 b- defN 24-Jun-03 13:10 nucliadb/standalone/auth.py
+-rw-r--r--  2.0 unx     5313 b- defN 24-Jun-03 13:10 nucliadb/standalone/config.py
+-rw-r--r--  2.0 unx     6986 b- defN 24-Jun-03 13:10 nucliadb/standalone/introspect.py
+-rw-r--r--  2.0 unx     2488 b- defN 24-Jun-03 13:10 nucliadb/standalone/lifecycle.py
+-rw-r--r--  2.0 unx     1980 b- defN 24-Jun-03 13:10 nucliadb/standalone/migrations.py
+-rw-r--r--  2.0 unx     1322 b- defN 24-Jun-03 13:10 nucliadb/standalone/purge.py
+-rw-r--r--  2.0 unx        0 b- defN 24-Jun-03 13:10 nucliadb/standalone/py.typed
+-rw-r--r--  2.0 unx     5636 b- defN 24-Jun-03 13:10 nucliadb/standalone/run.py
+-rw-r--r--  2.0 unx     5822 b- defN 24-Jun-03 13:10 nucliadb/standalone/settings.py
+-rw-r--r--  2.0 unx     3132 b- defN 24-Jun-03 13:10 nucliadb/standalone/versions.py
+-rw-r--r--  2.0 unx     2285 b- defN 24-Jun-03 13:10 nucliadb/standalone/static/favicon.ico
+-rw-r--r--  2.0 unx     3833 b- defN 24-Jun-03 13:10 nucliadb/standalone/static/index.html
+-rw-r--r--  2.0 unx     2639 b- defN 24-Jun-03 13:10 nucliadb/standalone/static/logo.svg
+-rw-r--r--  2.0 unx      835 b- defN 24-Jun-03 13:10 nucliadb/standalone/tests/__init__.py
+-rw-r--r--  2.0 unx     1294 b- defN 24-Jun-03 13:10 nucliadb/standalone/tests/conftest.py
+-rw-r--r--  2.0 unx     1319 b- defN 24-Jun-03 13:10 nucliadb/standalone/tests/fixtures.py
+-rw-r--r--  2.0 unx      833 b- defN 24-Jun-03 13:10 nucliadb/standalone/tests/unit/__init__.py
+-rw-r--r--  2.0 unx     1722 b- defN 24-Jun-03 13:10 nucliadb/standalone/tests/unit/test_api_router.py
+-rw-r--r--  2.0 unx     5509 b- defN 24-Jun-03 13:10 nucliadb/standalone/tests/unit/test_auth.py
+-rw-r--r--  2.0 unx     1334 b- defN 24-Jun-03 13:10 nucliadb/standalone/tests/unit/test_introspect.py
+-rw-r--r--  2.0 unx     1863 b- defN 24-Jun-03 13:10 nucliadb/standalone/tests/unit/test_migrations.py
+-rw-r--r--  2.0 unx     1546 b- defN 24-Jun-03 13:10 nucliadb/standalone/tests/unit/test_run.py
+-rw-r--r--  2.0 unx     1972 b- defN 24-Jun-03 13:10 nucliadb/standalone/tests/unit/test_versions.py
+-rw-r--r--  2.0 unx     1037 b- defN 24-Jun-03 13:10 nucliadb/tasks/__init__.py
+-rw-r--r--  2.0 unx     7655 b- defN 24-Jun-03 13:10 nucliadb/tasks/consumer.py
+-rw-r--r--  2.0 unx      924 b- defN 24-Jun-03 13:10 nucliadb/tasks/logger.py
+-rw-r--r--  2.0 unx     1378 b- defN 24-Jun-03 13:10 nucliadb/tasks/models.py
+-rw-r--r--  2.0 unx     3457 b- defN 24-Jun-03 13:10 nucliadb/tasks/producer.py
+-rw-r--r--  2.0 unx     1753 b- defN 24-Jun-03 13:10 nucliadb/tasks/registry.py
+-rw-r--r--  2.0 unx     1360 b- defN 24-Jun-03 13:10 nucliadb/tasks/utils.py
+-rw-r--r--  2.0 unx      835 b- defN 24-Jun-03 13:10 nucliadb/tests/__init__.py
+-rw-r--r--  2.0 unx     1229 b- defN 24-Jun-03 13:10 nucliadb/tests/conftest.py
+-rw-r--r--  2.0 unx    22365 b- defN 24-Jun-03 13:10 nucliadb/tests/fixtures.py
+-rw-r--r--  2.0 unx     7549 b- defN 24-Jun-03 13:10 nucliadb/tests/tikv.py
+-rw-r--r--  2.0 unx      835 b- defN 24-Jun-03 13:10 nucliadb/tests/benchmarks/__init__.py
+-rw-r--r--  2.0 unx     3032 b- defN 24-Jun-03 13:10 nucliadb/tests/benchmarks/test_search.py
+-rw-r--r--  2.0 unx      919 b- defN 24-Jun-03 13:10 nucliadb/tests/knowledgeboxes/__init__.py
+-rw-r--r--  2.0 unx     7002 b- defN 24-Jun-03 13:10 nucliadb/tests/knowledgeboxes/philosophy_books.py
+-rw-r--r--  2.0 unx     3037 b- defN 24-Jun-03 13:10 nucliadb/tests/knowledgeboxes/ten_dummy_resources.py
+-rw-r--r--  2.0 unx     1148 b- defN 24-Jun-03 13:10 nucliadb/tests/migrations/__init__.py
+-rw-r--r--  2.0 unx     2726 b- defN 24-Jun-03 13:10 nucliadb/tests/migrations/test_migration_0017.py
+-rw-r--r--  2.0 unx     3662 b- defN 24-Jun-03 13:10 nucliadb/tests/migrations/test_migration_0018.py
+-rw-r--r--  2.0 unx     3439 b- defN 24-Jun-03 13:10 nucliadb/tests/migrations/test_migration_0021.py
+-rw-r--r--  2.0 unx      835 b- defN 24-Jun-03 13:10 nucliadb/tests/unit/__init__.py
+-rw-r--r--  2.0 unx     1487 b- defN 24-Jun-03 13:10 nucliadb/tests/unit/test_field_ids.py
+-rw-r--r--  2.0 unx     2780 b- defN 24-Jun-03 13:10 nucliadb/tests/unit/test_health.py
+-rw-r--r--  2.0 unx     1543 b- defN 24-Jun-03 13:10 nucliadb/tests/unit/test_kb_slugs.py
+-rw-r--r--  2.0 unx     7892 b- defN 24-Jun-03 13:10 nucliadb/tests/unit/test_learning_proxy.py
+-rw-r--r--  2.0 unx     2642 b- defN 24-Jun-03 13:10 nucliadb/tests/unit/test_metrics_exporter.py
+-rw-r--r--  2.0 unx     1341 b- defN 24-Jun-03 13:10 nucliadb/tests/unit/test_openapi.py
+-rw-r--r--  2.0 unx     3649 b- defN 24-Jun-03 13:10 nucliadb/tests/unit/test_purge.py
+-rw-r--r--  2.0 unx      835 b- defN 24-Jun-03 13:10 nucliadb/tests/unit/common/__init__.py
+-rw-r--r--  2.0 unx     1268 b- defN 24-Jun-03 13:10 nucliadb/tests/unit/common/test_context.py
+-rw-r--r--  2.0 unx      835 b- defN 24-Jun-03 13:10 nucliadb/tests/unit/common/cluster/__init__.py
+-rw-r--r--  2.0 unx    12240 b- defN 24-Jun-03 13:10 nucliadb/tests/unit/common/cluster/test_cluster.py
+-rw-r--r--  2.0 unx     5387 b- defN 24-Jun-03 13:10 nucliadb/tests/unit/common/cluster/test_kb_shard_manager.py
+-rw-r--r--  2.0 unx     1428 b- defN 24-Jun-03 13:10 nucliadb/tests/unit/common/cluster/test_rebalance.py
+-rw-r--r--  2.0 unx     9609 b- defN 24-Jun-03 13:10 nucliadb/tests/unit/common/cluster/test_rollover.py
+-rw-r--r--  2.0 unx      835 b- defN 24-Jun-03 13:10 nucliadb/tests/unit/common/cluster/discovery/__init__.py
+-rw-r--r--  2.0 unx     5627 b- defN 24-Jun-03 13:10 nucliadb/tests/unit/common/cluster/discovery/test_k8s.py
+-rw-r--r--  2.0 unx      833 b- defN 24-Jun-03 13:10 nucliadb/tests/unit/common/cluster/standalone/__init__.py
+-rw-r--r--  2.0 unx     3761 b- defN 24-Jun-03 13:10 nucliadb/tests/unit/common/cluster/standalone/test_service.py
+-rw-r--r--  2.0 unx     2136 b- defN 24-Jun-03 13:10 nucliadb/tests/unit/common/cluster/standalone/test_utils.py
+-rw-r--r--  2.0 unx      833 b- defN 24-Jun-03 13:10 nucliadb/tests/unit/common/maindb/__init__.py
+-rw-r--r--  2.0 unx     3579 b- defN 24-Jun-03 13:10 nucliadb/tests/unit/common/maindb/test_driver.py
+-rw-r--r--  2.0 unx     2119 b- defN 24-Jun-03 13:10 nucliadb/tests/unit/common/maindb/test_tikv.py
+-rw-r--r--  2.0 unx     3213 b- defN 24-Jun-03 13:10 nucliadb/tests/unit/common/maindb/test_utils.py
+-rw-r--r--  2.0 unx      835 b- defN 24-Jun-03 13:10 nucliadb/tests/unit/export_import/__init__.py
+-rw-r--r--  2.0 unx     1435 b- defN 24-Jun-03 13:10 nucliadb/tests/unit/export_import/test_datamanager.py
+-rw-r--r--  2.0 unx     9706 b- defN 24-Jun-03 13:10 nucliadb/tests/unit/export_import/test_utils.py
+-rw-r--r--  2.0 unx      835 b- defN 24-Jun-03 13:10 nucliadb/tests/unit/migrator/__init__.py
+-rw-r--r--  2.0 unx     3233 b- defN 24-Jun-03 13:10 nucliadb/tests/unit/migrator/test_migrator.py
+-rw-r--r--  2.0 unx      835 b- defN 24-Jun-03 13:10 nucliadb/tests/unit/tasks/__init__.py
+-rw-r--r--  2.0 unx     1375 b- defN 24-Jun-03 13:10 nucliadb/tests/unit/tasks/conftest.py
+-rw-r--r--  2.0 unx     2714 b- defN 24-Jun-03 13:10 nucliadb/tests/unit/tasks/test_consumer.py
+-rw-r--r--  2.0 unx     3189 b- defN 24-Jun-03 13:10 nucliadb/tests/unit/tasks/test_producer.py
+-rw-r--r--  2.0 unx     1827 b- defN 24-Jun-03 13:10 nucliadb/tests/unit/tasks/test_tasks.py
+-rw-r--r--  2.0 unx     2507 b- defN 24-Jun-03 13:10 nucliadb/tests/utils/__init__.py
+-rw-r--r--  2.0 unx     1797 b- defN 24-Jun-03 13:10 nucliadb/tests/utils/aiohttp_session.py
+-rw-r--r--  2.0 unx     2533 b- defN 24-Jun-03 13:10 nucliadb/tests/utils/entities.py
+-rw-r--r--  2.0 unx     6327 b- defN 24-Jun-03 13:10 nucliadb/tests/utils/broker_messages/__init__.py
+-rw-r--r--  2.0 unx     7557 b- defN 24-Jun-03 13:10 nucliadb/tests/utils/broker_messages/fields.py
+-rw-r--r--  2.0 unx     1196 b- defN 24-Jun-03 13:10 nucliadb/tests/utils/broker_messages/helpers.py
+-rw-r--r--  2.0 unx     1325 b- defN 24-Jun-03 13:10 nucliadb/train/__init__.py
+-rw-r--r--  2.0 unx     3530 b- defN 24-Jun-03 13:10 nucliadb/train/app.py
+-rw-r--r--  2.0 unx     3800 b- defN 24-Jun-03 13:10 nucliadb/train/generator.py
+-rw-r--r--  2.0 unx     1698 b- defN 24-Jun-03 13:10 nucliadb/train/lifecycle.py
+-rw-r--r--  2.0 unx     1198 b- defN 24-Jun-03 13:10 nucliadb/train/models.py
+-rw-r--r--  2.0 unx     5776 b- defN 24-Jun-03 13:10 nucliadb/train/nodes.py
+-rw-r--r--  2.0 unx        0 b- defN 24-Jun-03 13:10 nucliadb/train/py.typed
+-rw-r--r--  2.0 unx     1400 b- defN 24-Jun-03 13:10 nucliadb/train/run.py
+-rw-r--r--  2.0 unx     5750 b- defN 24-Jun-03 13:10 nucliadb/train/servicer.py
+-rw-r--r--  2.0 unx     1415 b- defN 24-Jun-03 13:10 nucliadb/train/settings.py
+-rw-r--r--  2.0 unx     1496 b- defN 24-Jun-03 13:10 nucliadb/train/types.py
+-rw-r--r--  2.0 unx     3265 b- defN 24-Jun-03 13:10 nucliadb/train/upload.py
+-rw-r--r--  2.0 unx     6395 b- defN 24-Jun-03 13:10 nucliadb/train/uploader.py
+-rw-r--r--  2.0 unx     3179 b- defN 24-Jun-03 13:10 nucliadb/train/utils.py
+-rw-r--r--  2.0 unx      835 b- defN 24-Jun-03 13:10 nucliadb/train/api/__init__.py
+-rw-r--r--  2.0 unx     1479 b- defN 24-Jun-03 13:10 nucliadb/train/api/utils.py
+-rw-r--r--  2.0 unx      928 b- defN 24-Jun-03 13:10 nucliadb/train/api/v1/__init__.py
+-rw-r--r--  2.0 unx     2071 b- defN 24-Jun-03 13:10 nucliadb/train/api/v1/check.py
+-rw-r--r--  2.0 unx      910 b- defN 24-Jun-03 13:10 nucliadb/train/api/v1/router.py
+-rw-r--r--  2.0 unx     1908 b- defN 24-Jun-03 13:10 nucliadb/train/api/v1/shards.py
+-rw-r--r--  2.0 unx     2135 b- defN 24-Jun-03 13:10 nucliadb/train/api/v1/trainset.py
+-rw-r--r--  2.0 unx      835 b- defN 24-Jun-03 13:10 nucliadb/train/generators/__init__.py
+-rw-r--r--  2.0 unx     3723 b- defN 24-Jun-03 13:10 nucliadb/train/generators/field_classifier.py
+-rw-r--r--  2.0 unx     6712 b- defN 24-Jun-03 13:10 nucliadb/train/generators/image_classifier.py
+-rw-r--r--  2.0 unx     2789 b- defN 24-Jun-03 13:10 nucliadb/train/generators/paragraph_classifier.py
+-rw-r--r--  2.0 unx     3590 b- defN 24-Jun-03 13:10 nucliadb/train/generators/paragraph_streaming.py
+-rw-r--r--  2.0 unx     5372 b- defN 24-Jun-03 13:10 nucliadb/train/generators/question_answer_streaming.py
+-rw-r--r--  2.0 unx     5160 b- defN 24-Jun-03 13:10 nucliadb/train/generators/sentence_classifier.py
+-rw-r--r--  2.0 unx    10446 b- defN 24-Jun-03 13:10 nucliadb/train/generators/token_classifier.py
+-rw-r--r--  2.0 unx     3877 b- defN 24-Jun-03 13:10 nucliadb/train/generators/utils.py
+-rw-r--r--  2.0 unx      835 b- defN 24-Jun-03 13:10 nucliadb/train/tests/__init__.py
+-rw-r--r--  2.0 unx     1125 b- defN 24-Jun-03 13:10 nucliadb/train/tests/conftest.py
+-rw-r--r--  2.0 unx    10995 b- defN 24-Jun-03 13:10 nucliadb/train/tests/fixtures.py
+-rw-r--r--  2.0 unx     4571 b- defN 24-Jun-03 13:10 nucliadb/train/tests/test_field_classification.py
+-rw-r--r--  2.0 unx     2729 b- defN 24-Jun-03 13:10 nucliadb/train/tests/test_get_entities.py
+-rw-r--r--  2.0 unx     1660 b- defN 24-Jun-03 13:10 nucliadb/train/tests/test_get_info.py
+-rw-r--r--  2.0 unx     1379 b- defN 24-Jun-03 13:10 nucliadb/train/tests/test_get_ontology.py
+-rw-r--r--  2.0 unx     2201 b- defN 24-Jun-03 13:10 nucliadb/train/tests/test_get_ontology_count.py
+-rw-r--r--  2.0 unx     7669 b- defN 24-Jun-03 13:10 nucliadb/train/tests/test_image_classification.py
+-rw-r--r--  2.0 unx     1416 b- defN 24-Jun-03 13:10 nucliadb/train/tests/test_list_fields.py
+-rw-r--r--  2.0 unx     2944 b- defN 24-Jun-03 13:10 nucliadb/train/tests/test_list_paragraphs.py
+-rw-r--r--  2.0 unx     1423 b- defN 24-Jun-03 13:10 nucliadb/train/tests/test_list_resources.py
+-rw-r--r--  2.0 unx     2947 b- defN 24-Jun-03 13:10 nucliadb/train/tests/test_list_sentences.py
+-rw-r--r--  2.0 unx     4645 b- defN 24-Jun-03 13:10 nucliadb/train/tests/test_paragraph_classification.py
+-rw-r--r--  2.0 unx     4320 b- defN 24-Jun-03 13:10 nucliadb/train/tests/test_paragraph_streaming.py
+-rw-r--r--  2.0 unx     8751 b- defN 24-Jun-03 13:10 nucliadb/train/tests/test_question_answer_streaming.py
+-rw-r--r--  2.0 unx     5051 b- defN 24-Jun-03 13:10 nucliadb/train/tests/test_sentence_classification.py
+-rw-r--r--  2.0 unx     5583 b- defN 24-Jun-03 13:10 nucliadb/train/tests/test_token_classification.py
+-rw-r--r--  2.0 unx     3324 b- defN 24-Jun-03 13:10 nucliadb/train/tests/utils.py
+-rw-r--r--  2.0 unx     1328 b- defN 24-Jun-03 13:10 nucliadb/writer/__init__.py
+-rw-r--r--  2.0 unx     4268 b- defN 24-Jun-03 13:10 nucliadb/writer/app.py
+-rw-r--r--  2.0 unx    19472 b- defN 24-Jun-03 13:10 nucliadb/writer/back_pressure.py
+-rw-r--r--  2.0 unx      929 b- defN 24-Jun-03 13:10 nucliadb/writer/exceptions.py
+-rw-r--r--  2.0 unx     1953 b- defN 24-Jun-03 13:10 nucliadb/writer/lifecycle.py
+-rw-r--r--  2.0 unx     1032 b- defN 24-Jun-03 13:10 nucliadb/writer/openapi.py
+-rw-r--r--  2.0 unx        0 b- defN 24-Jun-03 13:10 nucliadb/writer/py.typed
+-rw-r--r--  2.0 unx     1448 b- defN 24-Jun-03 13:10 nucliadb/writer/run.py
+-rw-r--r--  2.0 unx     3103 b- defN 24-Jun-03 13:10 nucliadb/writer/settings.py
+-rw-r--r--  2.0 unx     1036 b- defN 24-Jun-03 13:10 nucliadb/writer/utilities.py
+-rw-r--r--  2.0 unx      835 b- defN 24-Jun-03 13:10 nucliadb/writer/api/__init__.py
+-rw-r--r--  2.0 unx     1429 b- defN 24-Jun-03 13:10 nucliadb/writer/api/constants.py
+-rw-r--r--  2.0 unx     1095 b- defN 24-Jun-03 13:10 nucliadb/writer/api/v1/__init__.py
+-rw-r--r--  2.0 unx     6421 b- defN 24-Jun-03 13:10 nucliadb/writer/api/v1/export_import.py
+-rw-r--r--  2.0 unx    24482 b- defN 24-Jun-03 13:10 nucliadb/writer/api/v1/field.py
+-rw-r--r--  2.0 unx     5248 b- defN 24-Jun-03 13:10 nucliadb/writer/api/v1/knowledgebox.py
+-rw-r--r--  2.0 unx     2058 b- defN 24-Jun-03 13:10 nucliadb/writer/api/v1/learning_config.py
+-rw-r--r--  2.0 unx    18628 b- defN 24-Jun-03 13:10 nucliadb/writer/api/v1/resource.py
+-rw-r--r--  2.0 unx     1034 b- defN 24-Jun-03 13:10 nucliadb/writer/api/v1/router.py
+-rw-r--r--  2.0 unx    10485 b- defN 24-Jun-03 13:10 nucliadb/writer/api/v1/services.py
+-rw-r--r--  2.0 unx    30985 b- defN 24-Jun-03 13:10 nucliadb/writer/api/v1/upload.py
+-rw-r--r--  2.0 unx     1612 b- defN 24-Jun-03 13:10 nucliadb/writer/layouts/__init__.py
+-rw-r--r--  2.0 unx     2115 b- defN 24-Jun-03 13:10 nucliadb/writer/layouts/v1.py
+-rw-r--r--  2.0 unx      835 b- defN 24-Jun-03 13:10 nucliadb/writer/resource/__init__.py
+-rw-r--r--  2.0 unx     1425 b- defN 24-Jun-03 13:10 nucliadb/writer/resource/audit.py
+-rw-r--r--  2.0 unx    10968 b- defN 24-Jun-03 13:10 nucliadb/writer/resource/basic.py
+-rw-r--r--  2.0 unx    16740 b- defN 24-Jun-03 13:10 nucliadb/writer/resource/field.py
+-rw-r--r--  2.0 unx     2022 b- defN 24-Jun-03 13:10 nucliadb/writer/resource/origin.py
+-rw-r--r--  2.0 unx      835 b- defN 24-Jun-03 13:10 nucliadb/writer/tests/__init__.py
+-rw-r--r--  2.0 unx     1200 b- defN 24-Jun-03 13:10 nucliadb/writer/tests/conftest.py
+-rw-r--r--  2.0 unx     5971 b- defN 24-Jun-03 13:10 nucliadb/writer/tests/fixtures.py
+-rw-r--r--  2.0 unx    15472 b- defN 24-Jun-03 13:10 nucliadb/writer/tests/test_fields.py
+-rw-r--r--  2.0 unx    25988 b- defN 24-Jun-03 13:10 nucliadb/writer/tests/test_files.py
+-rw-r--r--  2.0 unx     1729 b- defN 24-Jun-03 13:10 nucliadb/writer/tests/test_knowledgebox.py
+-rw-r--r--  2.0 unx     4400 b- defN 24-Jun-03 13:10 nucliadb/writer/tests/test_reprocess_file_field.py
+-rw-r--r--  2.0 unx    16857 b- defN 24-Jun-03 13:10 nucliadb/writer/tests/test_resources.py
+-rw-r--r--  2.0 unx     5120 b- defN 24-Jun-03 13:10 nucliadb/writer/tests/test_service.py
+-rw-r--r--  2.0 unx     6054 b- defN 24-Jun-03 13:10 nucliadb/writer/tests/test_tus.py
+-rw-r--r--  2.0 unx     1287 b- defN 24-Jun-03 13:10 nucliadb/writer/tests/utils.py
+-rw-r--r--  2.0 unx     5226 b- defN 24-Jun-03 13:10 nucliadb/writer/tus/__init__.py
+-rw-r--r--  2.0 unx     5082 b- defN 24-Jun-03 13:10 nucliadb/writer/tus/dm.py
+-rw-r--r--  2.0 unx     2186 b- defN 24-Jun-03 13:10 nucliadb/writer/tus/exceptions.py
+-rw-r--r--  2.0 unx    14527 b- defN 24-Jun-03 13:10 nucliadb/writer/tus/gcs.py
+-rw-r--r--  2.0 unx     5849 b- defN 24-Jun-03 13:10 nucliadb/writer/tus/local.py
+-rw-r--r--  2.0 unx     4367 b- defN 24-Jun-03 13:10 nucliadb/writer/tus/pg.py
+-rw-r--r--  2.0 unx     9069 b- defN 24-Jun-03 13:10 nucliadb/writer/tus/s3.py
+-rw-r--r--  2.0 unx     4734 b- defN 24-Jun-03 13:10 nucliadb/writer/tus/storage.py
+-rw-r--r--  2.0 unx     2556 b- defN 24-Jun-03 13:10 nucliadb/writer/tus/utils.py
+-rw-r--r--  2.0 unx     4474 b- defN 24-Jun-03 13:12 nucliadb-4.0.3.post565.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-Jun-03 13:12 nucliadb-4.0.3.post565.dist-info/WHEEL
+-rw-r--r--  2.0 unx     1268 b- defN 24-Jun-03 13:12 nucliadb-4.0.3.post565.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx       20 b- defN 24-Jun-03 13:12 nucliadb-4.0.3.post565.dist-info/top_level.txt
+-rw-r--r--  2.0 unx        1 b- defN 24-Jun-03 13:12 nucliadb-4.0.3.post565.dist-info/zip-safe
+-rw-rw-r--  2.0 unx    44526 b- defN 24-Jun-03 13:12 nucliadb-4.0.3.post565.dist-info/RECORD
+475 files, 2292866 bytes uncompressed, 706625 bytes compressed:  69.2%
```

## zipnote {}

```diff
@@ -1401,26 +1401,26 @@
 
 Filename: nucliadb/writer/tus/storage.py
 Comment: 
 
 Filename: nucliadb/writer/tus/utils.py
 Comment: 
 
-Filename: nucliadb-4.0.3.post564.dist-info/METADATA
+Filename: nucliadb-4.0.3.post565.dist-info/METADATA
 Comment: 
 
-Filename: nucliadb-4.0.3.post564.dist-info/WHEEL
+Filename: nucliadb-4.0.3.post565.dist-info/WHEEL
 Comment: 
 
-Filename: nucliadb-4.0.3.post564.dist-info/entry_points.txt
+Filename: nucliadb-4.0.3.post565.dist-info/entry_points.txt
 Comment: 
 
-Filename: nucliadb-4.0.3.post564.dist-info/top_level.txt
+Filename: nucliadb-4.0.3.post565.dist-info/top_level.txt
 Comment: 
 
-Filename: nucliadb-4.0.3.post564.dist-info/zip-safe
+Filename: nucliadb-4.0.3.post565.dist-info/zip-safe
 Comment: 
 
-Filename: nucliadb-4.0.3.post564.dist-info/RECORD
+Filename: nucliadb-4.0.3.post565.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## nucliadb/common/maindb/pg.py

```diff
@@ -16,15 +16,15 @@
 #
 # You should have received a copy of the GNU Affero General Public License
 # along with this program. If not, see <http://www.gnu.org/licenses/>.
 #
 from __future__ import annotations
 
 import asyncio
-from typing import Any, AsyncGenerator, Optional, Union
+from typing import Any, AsyncGenerator, List, Optional, Union
 
 import asyncpg
 import backoff
 
 from nucliadb.common.maindb.driver import DEFAULT_SCAN_LIMIT, Driver, Transaction
 
 RETRIABLE_EXCEPTIONS = (
@@ -36,14 +36,27 @@
 CREATE_TABLE = """
 CREATE TABLE IF NOT EXISTS resources (
     key TEXT PRIMARY KEY,
     value BYTEA
 );
 """
 
+CREATE_REPLICATION_TABLE = """
+CREATE TABLE IF NOT EXISTS replication (
+    id BIGSERIAL PRIMARY KEY,
+    delete bool NOT NULL,
+    key TEXT NOT NULL,
+    value BYTEA
+);
+CREATE TABLE IF NOT EXISTS replication_commit (
+    commit_id BIGSERIAL PRIMARY KEY,
+    operations BIGINT[]
+);
+"""
+
 
 class DataLayer:
     def __init__(self, connection: Union[asyncpg.Connection, asyncpg.Pool]):
         self.connection = connection
         self.lock = asyncio.Lock()
 
     async def get(self, key: str, select_for_update: bool = False) -> Optional[bytes]:
@@ -62,18 +75,44 @@
 ON CONFLICT (key)
 DO UPDATE SET value = EXCLUDED.value
 """,
                 key,
                 value,
             )
 
+    async def set_replication(self, key: str, value: bytes) -> int:
+        async with self.lock:
+            return (
+                await self.connection.fetchrow(
+                    "INSERT INTO replication (delete, key, value) VALUES (false, $1, $2) RETURNING ID",
+                    key,
+                    value,
+                )
+            )["id"]
+
+    async def create_replication_commit(self, replication_ops: List[int]):
+        async with self.lock:
+            await self.connection.execute(
+                "INSERT INTO replication_commit (operations) VALUES ($1)",
+                replication_ops,
+            )
+
     async def delete(self, key: str) -> None:
         async with self.lock:
             await self.connection.execute("DELETE FROM resources WHERE key = $1", key)
 
+    async def delete_replication(self, key: str) -> int:
+        async with self.lock:
+            return (
+                await self.connection.fetchrow(
+                    "INSERT INTO replication (delete, key) VALUES (true, $1) RETURNING id",
+                    key,
+                )
+            )["id"]
+
     async def batch_get(
         self, keys: list[str], select_for_update: bool = False
     ) -> list[Optional[bytes]]:
         async with self.lock:
             statement = "SELECT key, value FROM resources WHERE key = ANY($1)"
             if select_for_update:
                 statement += " FOR UPDATE"
@@ -146,26 +185,35 @@
             except Exception:
                 await self.txn.rollback()
                 raise
             finally:
                 self.open = False
                 await self.connection.close()
 
+    async def create_replication_commit(self, replication_ops: List[int]):
+        return await self.data_layer.create_replication_commit(replication_ops)
+
     async def batch_get(self, keys: list[str]):
         return await self.data_layer.batch_get(keys, select_for_update=True)
 
     async def get(self, key: str) -> Optional[bytes]:
         return await self.data_layer.get(key, select_for_update=True)
 
     async def set(self, key: str, value: bytes):
         await self.data_layer.set(key, value)
 
+    async def set_replication(self, key: str, value: bytes) -> int:
+        return await self.data_layer.set_replication(key, value)
+
     async def delete(self, key: str):
         await self.data_layer.delete(key)
 
+    async def delete_replication(self, key: str) -> int:
+        return await self.data_layer.delete_replication(key)
+
     @backoff.on_exception(
         backoff.expo, RETRIABLE_EXCEPTIONS, jitter=backoff.random_jitter, max_tries=2
     )
     async def keys(
         self,
         match: str,
         count: int = DEFAULT_SCAN_LIMIT,
@@ -228,26 +276,29 @@
     pool: asyncpg.Pool
 
     def __init__(self, url: str, connection_pool_max_size: int = 10):
         self.url = url
         self.connection_pool_max_size = connection_pool_max_size
         self._lock = asyncio.Lock()
 
-    async def initialize(self):
+    async def initialize(self, for_replication: bool = False):
         async with self._lock:
             if self.initialized is False:
                 self.pool = await asyncpg.create_pool(
                     self.url,
                     max_size=self.connection_pool_max_size,
                 )
 
                 # check if table exists
+                create_table = (
+                    CREATE_REPLICATION_TABLE if for_replication else CREATE_TABLE
+                )
                 try:
                     async with self.pool.acquire() as conn:
-                        await conn.execute(CREATE_TABLE)
+                        await conn.execute(create_table)
                 except asyncpg.exceptions.UniqueViolationError:  # pragma: no cover
                     pass
 
             self.initialized = True
 
     async def finalize(self):
         async with self._lock:
```

## nucliadb/common/maindb/tikv.py

```diff
@@ -32,14 +32,16 @@
     DEFAULT_SCAN_LIMIT,
     Driver,
     Transaction,
 )
 from nucliadb.common.maindb.exceptions import ConflictError, MaindbServerError
 from nucliadb_telemetry import metrics
 
+from .pg import PGDriver, PGTransaction
+
 try:
     from tikv_client import asynchronous  # type: ignore
 
     TiKV = True
 except ImportError:  # pragma: no cover
     TiKV = False
 
@@ -258,29 +260,42 @@
                 break
         return value
 
 
 class TiKVTransaction(Transaction):
     driver: TiKVDriver
 
-    def __init__(self, txn: Any, driver: TiKVDriver):
+    def __init__(
+        self,
+        txn: Any,
+        driver: TiKVDriver,
+        replication_tx: Optional[PGTransaction] = None,
+    ):
         self.txn = txn
         self.driver = driver
         self.data_layer = TiKVDataLayer(txn)
         self.open = True
+        self.replication_tx = replication_tx
+        self.replication_ops: List[int] = []
 
     async def abort(self):
         if not self.open:
             return
         await self.data_layer.abort()
+        if self.replication_tx:
+            self.replication_ops.clear()
+            await self.replication_tx.abort()
         self.open = False
 
     async def commit(self):
         assert self.open
         await self.data_layer.commit()
+        if self.replication_tx and self.replication_ops:
+            await self.replication_tx.create_replication_commit(self.replication_ops)
+            await self.replication_tx.commit()
         self.open = False
 
     async def batch_get(self, keys: list[str]) -> list[Optional[bytes]]:
         assert self.open
         return await self.data_layer.batch_get(keys)
 
     @backoff.on_exception(
@@ -291,18 +306,26 @@
     )
     async def get(self, key: str) -> Optional[bytes]:
         assert self.open
         return await self.data_layer.get(key)
 
     async def set(self, key: str, value: bytes) -> None:
         assert self.open
+        if self.replication_tx:
+            self.replication_ops.append(
+                await self.replication_tx.set_replication(key, value)
+            )
         return await self.data_layer.set(key, value)
 
     async def delete(self, key: str) -> None:
         assert self.open
+        if self.replication_tx:
+            self.replication_ops.append(
+                await self.replication_tx.delete_replication(key)
+            )
         return await self.data_layer.delete(key)
 
     async def keys(
         self, match: str, count: int = DEFAULT_SCAN_LIMIT, include_start: bool = True
     ):
         assert self.open
         # XXX must have connection outside of current txn
@@ -314,57 +337,14 @@
             yield key
 
     async def count(self, match: str) -> int:
         assert self.open
         return await self.data_layer.count(match)
 
 
-class ReadOnlyTiKVTransaction(Transaction):
-    driver: TiKVDriver
-
-    def __init__(self, connection: asynchronous.Snapshot, driver: TiKVDriver):
-        self.connection = connection
-        self.data_layer = TiKVDataLayer(connection)
-        self.driver = driver
-        self.open = True
-
-    async def abort(self):
-        self.open = False
-        # Read only transactions are implemented as snapshots, which
-        # are read only and isolated, and they don't need to be aborted.
-
-    async def commit(self):
-        raise Exception("Cannot commit transaction in read only mode")
-
-    async def batch_get(self, keys: list[str]) -> list[Optional[bytes]]:
-        assert self.open
-        return await self.data_layer.batch_get(keys)
-
-    async def get(self, key: str) -> Optional[bytes]:
-        assert self.open
-        return await self.data_layer.get(key)
-
-    async def set(self, key: str, value: bytes) -> None:
-        raise Exception("Cannot set in read only transaction")
-
-    async def delete(self, key: str) -> None:
-        raise Exception("Cannot delete in read only transaction")
-
-    async def keys(
-        self, match: str, count: int = DEFAULT_SCAN_LIMIT, include_start: bool = True
-    ):
-        assert self.open
-        async for key in self.data_layer.keys(match, count, include_start):
-            yield key
-
-    async def count(self, match: str) -> int:
-        assert self.open
-        return await self.data_layer.count(match)
-
-
 class ConnectionHolder:
     _txn_connection: asynchronous.TransactionClient
 
     def __init__(self, url: list[str]):
         self.url = url
         self.connect_lock = asyncio.Lock()
 
@@ -430,33 +410,42 @@
         else:
             async with self.connect_lock:
                 logger.warning("Reconnecting to TiKV")
                 await self.initialize()
 
 
 class TiKVDriver(Driver):
-    def __init__(self, url: List[str], pool_size: int = 3):
+    def __init__(
+        self, url: List[str], pool_size: int = 3, replication_url: Optional[str] = None
+    ):
         if TiKV is False:
             raise ImportError("TiKV is not installed")
         self.url = url
         self.pool: list[ConnectionHolder] = []
         self.pool_size = pool_size
+        if replication_url:
+            self.replication_driver: Optional[PGDriver] = PGDriver(replication_url)
+        else:
+            self.replication_driver = None
 
     async def initialize(self):
         self.pool = [ConnectionHolder(self.url) for _ in range(self.pool_size)]
         for holder in self.pool:
             await holder.reinitialize()
+        if self.replication_driver:
+            await self.replication_driver.initialize(for_replication=True)
 
     async def finalize(self):
         self.pool.clear()
+        if self.replication_driver:
+            await self.replication_driver.finalize()
 
     def get_connection_holder(self) -> ConnectionHolder:
         return random.choice(self.pool)
 
-    async def begin(
-        self, read_only: bool = False
-    ) -> Union[TiKVTransaction, ReadOnlyTiKVTransaction]:
+    async def begin(self, read_only: bool = False) -> TiKVTransaction:
         conn = self.get_connection_holder()
-        # if read_only:
-        #     return ReadOnlyTiKVTransaction(await conn.get_snapshot(), self)
-        # else:
-        return TiKVTransaction(await conn.begin_transaction(), self)
+        if self.replication_driver and not read_only:
+            replication_tx: PGTransaction = await self.replication_driver.begin()  # type: ignore
+            return TiKVTransaction(await conn.begin_transaction(), self, replication_tx)
+        else:
+            return TiKVTransaction(await conn.begin_transaction(), self)
```

## nucliadb/common/maindb/utils.py

```diff
@@ -75,15 +75,17 @@
     elif settings.driver == DriverConfig.TIKV:
         if not TIKV:
             raise ConfigurationError("`tikv_client` python package not installed.")
         if settings.driver_tikv_url is None:
             raise ConfigurationError("No DRIVER_TIKV_URL env var defined.")
 
         tikv_driver = TiKVDriver(
-            settings.driver_tikv_url, settings.driver_tikv_connection_pool_size
+            settings.driver_tikv_url,
+            settings.driver_tikv_connection_pool_size,
+            settings.driver_tikv_replication_pg_url,
         )
         set_utility(Utility.MAINDB_DRIVER, tikv_driver)
     elif settings.driver == DriverConfig.PG:
         if not PG:
             raise ConfigurationError("`asyncpg` python package not installed.")
         if settings.driver_pg_url is None:
             raise ConfigurationError("No DRIVER_PG_URL env var defined.")
```

## nucliadb/ingest/settings.py

```diff
@@ -67,14 +67,18 @@
         default=20,
         description="PostgreSQL max pool size. The maximum number of connections to the PostgreSQL server.",
     )
     driver_tikv_connection_pool_size: int = Field(
         default=3,
         description="TiKV max pool size. The maximum number of connections to the TiKV server.",
     )
+    driver_tikv_replication_pg_url: Optional[str] = Field(
+        default=None,
+        description="PostgreSQL DSN for replication",
+    )
 
 
 class Settings(DriverSettings):
     grpc_port: int = 8030
 
     partitions: list[str] = ["1"]
```

## Comparing `nucliadb-4.0.3.post564.dist-info/METADATA` & `nucliadb-4.0.3.post565.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nucliadb
-Version: 4.0.3.post564
+Version: 4.0.3.post565
 Home-page: https://docs.nuclia.dev/docs/guides/nucliadb/intro
 Author: NucliaDB Community
 Author-email: nucliadb@nuclia.com
 License: BSD
 Project-URL: Nuclia, https://nuclia.com
 Project-URL: Github, https://github.com/nuclia/nucliadb
 Project-URL: Discord, https://discord.gg/8EvQwmsbzf
@@ -18,18 +18,18 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: 3 :: Only
 Requires-Python: >=3.9, <4
 Description-Content-Type: text/markdown
-Requires-Dist: nucliadb-telemetry[all] >=4.0.3.post564
-Requires-Dist: nucliadb-utils[cache,fastapi,storages] >=4.0.3.post564
-Requires-Dist: nucliadb-protos >=4.0.3.post564
-Requires-Dist: nucliadb-models >=4.0.3.post564
+Requires-Dist: nucliadb-telemetry[all] >=4.0.3.post565
+Requires-Dist: nucliadb-utils[cache,fastapi,storages] >=4.0.3.post565
+Requires-Dist: nucliadb-protos >=4.0.3.post565
+Requires-Dist: nucliadb-models >=4.0.3.post565
 Requires-Dist: nucliadb-admin-assets >=1.0.0.post1224
 Requires-Dist: nucliadb-node-binding >=2.26.0
 Requires-Dist: uvicorn <0.19.0
 Requires-Dist: argdantic
 Requires-Dist: aiohttp >=3.9.4
 Requires-Dist: lru-dict >=1.1.7
 Requires-Dist: backoff
```

## Comparing `nucliadb-4.0.3.post564.dist-info/entry_points.txt` & `nucliadb-4.0.3.post565.dist-info/entry_points.txt`

 * *Files identical despite different names*

## Comparing `nucliadb-4.0.3.post564.dist-info/RECORD` & `nucliadb-4.0.3.post565.dist-info/RECORD`

 * *Files 1% similar despite different names*

```diff
@@ -72,18 +72,18 @@
 nucliadb/common/http_clients/processing.py,sha256=-J5Lxmlk4coboOWvYQ4gc88AIrvHzSV9bzVsedmslCQ,7155
 nucliadb/common/http_clients/pypi.py,sha256=VHIUjwJEJVntVUo_FRoXIo8sLmluy7sa9-iXSITcrMY,1540
 nucliadb/common/http_clients/utils.py,sha256=b7FCaOSf21UVE9OqDhBpWetxP2nguV_gKwBBb9dYifI,1551
 nucliadb/common/maindb/__init__.py,sha256=cp15ZcFnHvpcu_5-aK2A4uUyvuZVV_MJn4bIXMa20ks,835
 nucliadb/common/maindb/driver.py,sha256=ldk1vxo-fx9vmAr8nzqQ0v8Z1fc6K_xzhsYa0QTcdlA,3449
 nucliadb/common/maindb/exceptions.py,sha256=u6ZSQW6jk5QM_IL5XmQ_dF-vZ-JkuWEqZbNJ-S6FG_g,988
 nucliadb/common/maindb/local.py,sha256=E6rWm9QOXOdkk6is6Ut6AiUaW9pRr2UgS_eHyMp2e-s,6769
-nucliadb/common/maindb/pg.py,sha256=ouQkD8o53LcFvjQr2KSBmZPHFi4dx0r29wOdSizlOfs,8673
+nucliadb/common/maindb/pg.py,sha256=EUUiHmoUxQ7SA1PZIY2uKH4c_Xxlx4q1rTp0PA-1iBc,10484
 nucliadb/common/maindb/redis.py,sha256=fPvLuDDlxXUiGPsO936SaaopFhdvzD_HGXgSV8TneY4,6053
-nucliadb/common/maindb/tikv.py,sha256=7Jp3YLwmb-ZDb0v6TQupo8xtSeAPLde3th45QH424pc,15314
-nucliadb/common/maindb/utils.py,sha256=LmZL3pbGcUuCK8DFtOuVbM7K_kjhea0ofnuy95sXfzE,4167
+nucliadb/common/maindb/tikv.py,sha256=ZIuDGHYtFEhqp0clCqD241YcxN62bRJucf1ty3cdi3A,15209
+nucliadb/common/maindb/utils.py,sha256=47yMvohguOc84cDib-q7JbMYtZudJO7pzLVAnYBjtUk,4233
 nucliadb/export_import/__init__.py,sha256=y-Is0Bxa8TMV6UiOW0deC_D3U465P65CQ5RjBjIWnow,932
 nucliadb/export_import/datamanager.py,sha256=sNq01FYRsanPbwO0UmPeAdMdb5J914wWo-_YPkCqW_8,6185
 nucliadb/export_import/exceptions.py,sha256=Dw8WqfG4r6MPJc5TPfbjMvCgXXWTcTOecGHRVU1h3kM,1949
 nucliadb/export_import/exporter.py,sha256=boXHZrH6UhnIPttHBjF0lHN0UT0OyQhPC1IEV6wAnwk,7116
 nucliadb/export_import/importer.py,sha256=kiZxziPo8ynQuO41mPmeUhVbV5w7iaFNzxlcNaKPcwA,4258
 nucliadb/export_import/models.py,sha256=VHetyHlofHH5yzcV5q6hN15zGKJTRAu7GOTNveN-tGA,2063
 nucliadb/export_import/tasks.py,sha256=HptUd322AmFDrlXqXcHLD3UYzaeHA54PevbvWxhqZjo,2571
@@ -91,15 +91,15 @@
 nucliadb/ingest/__init__.py,sha256=fsw3C38VP50km3R-nHL775LNGPpJ4JxqXJ2Ib1f5SqE,1011
 nucliadb/ingest/app.py,sha256=g51GuMZ9oLuIn8YZ7EKglVlLmu114VSmWzqMCbKtXRE,7277
 nucliadb/ingest/cache.py,sha256=w7jMMzamOmQ7gwXna6Dqm6isRNBVv6l5BTBlTxaYWjE,1005
 nucliadb/ingest/partitions.py,sha256=xhonCO-gqNO-8TlitjcmchVrxCLi-99SyOWvX4va1lE,2484
 nucliadb/ingest/processing.py,sha256=5UWQ8H_rBgDEmRYsiAI5CC9JPA_StMxhzRU8QKSs4bs,19904
 nucliadb/ingest/py.typed,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 nucliadb/ingest/serialize.py,sha256=ROCJZX0rtPx8skltubzN48es3mPSuxrI5mu_CfkdJOw,20291
-nucliadb/ingest/settings.py,sha256=VrOfSSwadDb2LRl0rwlJl5DSiDILj03KSD-n0Jh4yaE,3207
+nucliadb/ingest/settings.py,sha256=xm9Je4wJl8m-CTwuINavzSC_BExoP40IK2qyDTAlXUk,3348
 nucliadb/ingest/utils.py,sha256=dyFEv9V38OlkrQdM8_Xgii3YmbsRqNUoZeYApe39kx0,2314
 nucliadb/ingest/consumer/__init__.py,sha256=cp15ZcFnHvpcu_5-aK2A4uUyvuZVV_MJn4bIXMa20ks,835
 nucliadb/ingest/consumer/auditing.py,sha256=P6a7HgEJVE5WBJuyL7Q2avuqLqQ5QE3VaxoifS3YT3k,6918
 nucliadb/ingest/consumer/consumer.py,sha256=bJgVt1G7RchZrHX-5ykG2uHfGNY_HEjsLE2ZsgAv8HA,12174
 nucliadb/ingest/consumer/materializer.py,sha256=yN37qqXLwa4s2PuSNdgJTRKH7mFNhbexj2j7239iNg4,3934
 nucliadb/ingest/consumer/metrics.py,sha256=ji1l_4cKiHJthQd8YNem1ft4iMbw9KThmVvJmLcv3Xg,1075
 nucliadb/ingest/consumer/pull.py,sha256=pvD4Wn73wItyImmnoHADDISKYzI5K0XyUVtVmFJ0GvM,9546
@@ -463,13 +463,13 @@
 nucliadb/writer/tus/exceptions.py,sha256=CmxYKnHXpXug25DYV4SpVAU47SGD-NVBd7pNTRbWHyk,2186
 nucliadb/writer/tus/gcs.py,sha256=WykJZicWKRYkVB5_Fkb_1cVLovAk86IVkEn1VgEDufc,14527
 nucliadb/writer/tus/local.py,sha256=lIOoGaylnsxPBYGskcmKSHv7MsvwIYFS4soDLey_KSs,5849
 nucliadb/writer/tus/pg.py,sha256=JUK_xKsyNcKAvWOch8gUMTc_e1evI_3aC6-Y5gMk2jw,4367
 nucliadb/writer/tus/s3.py,sha256=a9mfPtjBW3QaTYY2r6P7u_Y13V6mBefZjWgV4juZzgE,9069
 nucliadb/writer/tus/storage.py,sha256=8iBOjWIcY6PawQq_rmSiBKi0Gl6J6Q5ad6L-9nLCcJ4,4734
 nucliadb/writer/tus/utils.py,sha256=MSdVbRsRSZVdkaum69_0wku7X3p5wlZf4nr6E0GMKbw,2556
-nucliadb-4.0.3.post564.dist-info/METADATA,sha256=fpc_ECsXuaJzFtTA_HAW9VBICapU7krcx2y5KsokzVI,4474
-nucliadb-4.0.3.post564.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
-nucliadb-4.0.3.post564.dist-info/entry_points.txt,sha256=XqGfgFDuY3zXQc8ewXM2TRVjTModIq851zOsgrmaXx4,1268
-nucliadb-4.0.3.post564.dist-info/top_level.txt,sha256=hwYhTVnX7jkQ9gJCkVrbqEG1M4lT2F_iPQND1fCzF80,20
-nucliadb-4.0.3.post564.dist-info/zip-safe,sha256=AbpHGcgLb-kRsJGnwFEktk7uzpZOCcBY74-YBdrKVGs,1
-nucliadb-4.0.3.post564.dist-info/RECORD,,
+nucliadb-4.0.3.post565.dist-info/METADATA,sha256=WLZf5pmXjqFM2M_0Hs65EIKZRY_rfmyYjI54J1OOb9Q,4474
+nucliadb-4.0.3.post565.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
+nucliadb-4.0.3.post565.dist-info/entry_points.txt,sha256=XqGfgFDuY3zXQc8ewXM2TRVjTModIq851zOsgrmaXx4,1268
+nucliadb-4.0.3.post565.dist-info/top_level.txt,sha256=hwYhTVnX7jkQ9gJCkVrbqEG1M4lT2F_iPQND1fCzF80,20
+nucliadb-4.0.3.post565.dist-info/zip-safe,sha256=AbpHGcgLb-kRsJGnwFEktk7uzpZOCcBY74-YBdrKVGs,1
+nucliadb-4.0.3.post565.dist-info/RECORD,,
```

