# Comparing `tmp/nucliadb-4.0.3.post562-py3-none-any.whl.zip` & `tmp/nucliadb-4.0.3.post563-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,477 +1,477 @@
-Zip file size: 777407 bytes, number of entries: 475
--rw-r--r--  2.0 unx     1135 b- defN 24-May-31 09:48 migrations/0001_bootstrap.py
--rw-r--r--  2.0 unx     1177 b- defN 24-May-31 09:48 migrations/0002_rollover_shards.py
--rw-r--r--  2.0 unx     2436 b- defN 24-May-31 09:48 migrations/0003_allfields_key.py
--rw-r--r--  2.0 unx     1177 b- defN 24-May-31 09:48 migrations/0004_rollover_shards.py
--rw-r--r--  2.0 unx     1177 b- defN 24-May-31 09:48 migrations/0005_rollover_shards.py
--rw-r--r--  2.0 unx     1024 b- defN 24-May-31 09:48 migrations/0006_rollover_shards.py
--rw-r--r--  2.0 unx     1301 b- defN 24-May-31 09:48 migrations/0008_cleanup_leftover_rollover_metadata.py
--rw-r--r--  2.0 unx     1378 b- defN 24-May-31 09:48 migrations/0009_upgrade_relations_and_texts_to_v2.py
--rw-r--r--  2.0 unx     1610 b- defN 24-May-31 09:48 migrations/0010_fix_corrupt_indexes.py
--rw-r--r--  2.0 unx     1843 b- defN 24-May-31 09:48 migrations/0011_materialize_labelset_ids.py
--rw-r--r--  2.0 unx     1443 b- defN 24-May-31 09:48 migrations/0012_rollover_shards.py
--rw-r--r--  2.0 unx     1024 b- defN 24-May-31 09:48 migrations/0013_rollover_shards.py
--rw-r--r--  2.0 unx     1382 b- defN 24-May-31 09:48 migrations/0014_rollover_shards.py
--rw-r--r--  2.0 unx     1462 b- defN 24-May-31 09:48 migrations/0015_targeted_rollover.py
--rw-r--r--  2.0 unx     2506 b- defN 24-May-31 09:48 migrations/0016_upgrade_to_paragraphs_v2.py
--rw-r--r--  2.0 unx     2100 b- defN 24-May-31 09:48 migrations/0017_multiple_writable_shards.py
--rw-r--r--  2.0 unx     2264 b- defN 24-May-31 09:48 migrations/0018_purge_orphan_kbslugs.py
--rw-r--r--  2.0 unx     2506 b- defN 24-May-31 09:48 migrations/0019_upgrade_to_paragraphs_v3.py
--rw-r--r--  2.0 unx     3282 b- defN 24-May-31 09:48 migrations/0020_drain_nodes_from_cluster.py
--rw-r--r--  2.0 unx     1734 b- defN 24-May-31 09:48 migrations/0021_overwrite_vectorsets_key.py
--rw-r--r--  2.0 unx      835 b- defN 24-May-31 09:48 migrations/__init__.py
--rw-r--r--  2.0 unx      891 b- defN 24-May-31 09:48 nucliadb/__init__.py
--rw-r--r--  2.0 unx     3733 b- defN 24-May-31 09:48 nucliadb/health.py
--rw-r--r--  2.0 unx    11793 b- defN 24-May-31 09:48 nucliadb/learning_proxy.py
--rw-r--r--  2.0 unx     4806 b- defN 24-May-31 09:48 nucliadb/metrics_exporter.py
--rw-r--r--  2.0 unx     2272 b- defN 24-May-31 09:48 nucliadb/openapi.py
--rw-r--r--  2.0 unx        0 b- defN 24-May-31 09:48 nucliadb/py.typed
--rw-r--r--  2.0 unx      835 b- defN 24-May-31 09:48 nucliadb/common/__init__.py
--rw-r--r--  2.0 unx     1912 b- defN 24-May-31 09:48 nucliadb/common/ids.py
--rw-r--r--  2.0 unx     5175 b- defN 24-May-31 09:48 nucliadb/common/locking.py
--rw-r--r--  2.0 unx      835 b- defN 24-May-31 09:48 nucliadb/common/cluster/__init__.py
--rw-r--r--  2.0 unx     5134 b- defN 24-May-31 09:48 nucliadb/common/cluster/base.py
--rw-r--r--  2.0 unx     1495 b- defN 24-May-31 09:48 nucliadb/common/cluster/exceptions.py
--rw-r--r--  2.0 unx     3793 b- defN 24-May-31 09:48 nucliadb/common/cluster/grpc_node_dummy.py
--rw-r--r--  2.0 unx     3429 b- defN 24-May-31 09:48 nucliadb/common/cluster/index_node.py
--rw-r--r--  2.0 unx    24815 b- defN 24-May-31 09:48 nucliadb/common/cluster/manager.py
--rw-r--r--  2.0 unx     8853 b- defN 24-May-31 09:48 nucliadb/common/cluster/rebalance.py
--rw-r--r--  2.0 unx    20532 b- defN 24-May-31 09:48 nucliadb/common/cluster/rollover.py
--rw-r--r--  2.0 unx     3016 b- defN 24-May-31 09:48 nucliadb/common/cluster/settings.py
--rw-r--r--  2.0 unx     5713 b- defN 24-May-31 09:48 nucliadb/common/cluster/utils.py
--rw-r--r--  2.0 unx      835 b- defN 24-May-31 09:48 nucliadb/common/cluster/discovery/__init__.py
--rw-r--r--  2.0 unx     6553 b- defN 24-May-31 09:48 nucliadb/common/cluster/discovery/base.py
--rw-r--r--  2.0 unx    12512 b- defN 24-May-31 09:48 nucliadb/common/cluster/discovery/k8s.py
--rw-r--r--  2.0 unx     1957 b- defN 24-May-31 09:48 nucliadb/common/cluster/discovery/manual.py
--rw-r--r--  2.0 unx     1737 b- defN 24-May-31 09:48 nucliadb/common/cluster/discovery/single.py
--rw-r--r--  2.0 unx     1139 b- defN 24-May-31 09:48 nucliadb/common/cluster/discovery/types.py
--rw-r--r--  2.0 unx     2548 b- defN 24-May-31 09:48 nucliadb/common/cluster/discovery/utils.py
--rw-r--r--  2.0 unx      833 b- defN 24-May-31 09:48 nucliadb/common/cluster/standalone/__init__.py
--rw-r--r--  2.0 unx    13712 b- defN 24-May-31 09:48 nucliadb/common/cluster/standalone/grpc_node_binding.py
--rw-r--r--  2.0 unx     4683 b- defN 24-May-31 09:48 nucliadb/common/cluster/standalone/index_node.py
--rw-r--r--  2.0 unx     3444 b- defN 24-May-31 09:48 nucliadb/common/cluster/standalone/service.py
--rw-r--r--  2.0 unx     3545 b- defN 24-May-31 09:48 nucliadb/common/cluster/standalone/utils.py
--rw-r--r--  2.0 unx     3440 b- defN 24-May-31 09:48 nucliadb/common/context/__init__.py
--rw-r--r--  2.0 unx     1628 b- defN 24-May-31 09:48 nucliadb/common/context/fastapi.py
--rw-r--r--  2.0 unx     1966 b- defN 24-May-31 09:48 nucliadb/common/datamanagers/__init__.py
--rw-r--r--  2.0 unx     2648 b- defN 24-May-31 09:48 nucliadb/common/datamanagers/atomic.py
--rw-r--r--  2.0 unx     1451 b- defN 24-May-31 09:48 nucliadb/common/datamanagers/cluster.py
--rw-r--r--  2.0 unx     5383 b- defN 24-May-31 09:48 nucliadb/common/datamanagers/entities.py
--rw-r--r--  2.0 unx      883 b- defN 24-May-31 09:48 nucliadb/common/datamanagers/exceptions.py
--rw-r--r--  2.0 unx     2764 b- defN 24-May-31 09:48 nucliadb/common/datamanagers/fields.py
--rw-r--r--  2.0 unx     3994 b- defN 24-May-31 09:48 nucliadb/common/datamanagers/kb.py
--rw-r--r--  2.0 unx     5389 b- defN 24-May-31 09:48 nucliadb/common/datamanagers/labels.py
--rw-r--r--  2.0 unx     1599 b- defN 24-May-31 09:48 nucliadb/common/datamanagers/processing.py
--rw-r--r--  2.0 unx    11922 b- defN 24-May-31 09:48 nucliadb/common/datamanagers/resources.py
--rw-r--r--  2.0 unx     5634 b- defN 24-May-31 09:48 nucliadb/common/datamanagers/rollover.py
--rw-r--r--  2.0 unx     1548 b- defN 24-May-31 09:48 nucliadb/common/datamanagers/synonyms.py
--rw-r--r--  2.0 unx     1631 b- defN 24-May-31 09:48 nucliadb/common/datamanagers/utils.py
--rw-r--r--  2.0 unx     3780 b- defN 24-May-31 09:48 nucliadb/common/datamanagers/vectorsets.py
--rw-r--r--  2.0 unx      835 b- defN 24-May-31 09:48 nucliadb/common/http_clients/__init__.py
--rw-r--r--  2.0 unx     2146 b- defN 24-May-31 09:48 nucliadb/common/http_clients/auth.py
--rw-r--r--  2.0 unx     1100 b- defN 24-May-31 09:48 nucliadb/common/http_clients/exceptions.py
--rw-r--r--  2.0 unx     7155 b- defN 24-May-31 09:48 nucliadb/common/http_clients/processing.py
--rw-r--r--  2.0 unx     1540 b- defN 24-May-31 09:48 nucliadb/common/http_clients/pypi.py
--rw-r--r--  2.0 unx     1551 b- defN 24-May-31 09:48 nucliadb/common/http_clients/utils.py
--rw-r--r--  2.0 unx      835 b- defN 24-May-31 09:48 nucliadb/common/maindb/__init__.py
--rw-r--r--  2.0 unx     3449 b- defN 24-May-31 09:48 nucliadb/common/maindb/driver.py
--rw-r--r--  2.0 unx      988 b- defN 24-May-31 09:48 nucliadb/common/maindb/exceptions.py
--rw-r--r--  2.0 unx     6769 b- defN 24-May-31 09:48 nucliadb/common/maindb/local.py
--rw-r--r--  2.0 unx     8391 b- defN 24-May-31 09:48 nucliadb/common/maindb/pg.py
--rw-r--r--  2.0 unx     6053 b- defN 24-May-31 09:48 nucliadb/common/maindb/redis.py
--rw-r--r--  2.0 unx    15314 b- defN 24-May-31 09:48 nucliadb/common/maindb/tikv.py
--rw-r--r--  2.0 unx     4167 b- defN 24-May-31 09:48 nucliadb/common/maindb/utils.py
--rw-r--r--  2.0 unx      932 b- defN 24-May-31 09:48 nucliadb/export_import/__init__.py
--rw-r--r--  2.0 unx     6171 b- defN 24-May-31 09:48 nucliadb/export_import/datamanager.py
--rw-r--r--  2.0 unx     1949 b- defN 24-May-31 09:48 nucliadb/export_import/exceptions.py
--rw-r--r--  2.0 unx     7116 b- defN 24-May-31 09:48 nucliadb/export_import/exporter.py
--rw-r--r--  2.0 unx     4258 b- defN 24-May-31 09:48 nucliadb/export_import/importer.py
--rw-r--r--  2.0 unx     2063 b- defN 24-May-31 09:48 nucliadb/export_import/models.py
--rw-r--r--  2.0 unx     2571 b- defN 24-May-31 09:48 nucliadb/export_import/tasks.py
--rw-r--r--  2.0 unx    19646 b- defN 24-May-31 09:48 nucliadb/export_import/utils.py
--rw-r--r--  2.0 unx     1011 b- defN 24-May-31 09:48 nucliadb/ingest/__init__.py
--rw-r--r--  2.0 unx     7277 b- defN 24-May-31 09:48 nucliadb/ingest/app.py
--rw-r--r--  2.0 unx     1005 b- defN 24-May-31 09:48 nucliadb/ingest/cache.py
--rw-r--r--  2.0 unx     2484 b- defN 24-May-31 09:48 nucliadb/ingest/partitions.py
--rw-r--r--  2.0 unx    19904 b- defN 24-May-31 09:48 nucliadb/ingest/processing.py
--rw-r--r--  2.0 unx        0 b- defN 24-May-31 09:48 nucliadb/ingest/py.typed
--rw-r--r--  2.0 unx    20277 b- defN 24-May-31 09:48 nucliadb/ingest/serialize.py
--rw-r--r--  2.0 unx     3207 b- defN 24-May-31 09:48 nucliadb/ingest/settings.py
--rw-r--r--  2.0 unx     2314 b- defN 24-May-31 09:48 nucliadb/ingest/utils.py
--rw-r--r--  2.0 unx      835 b- defN 24-May-31 09:48 nucliadb/ingest/consumer/__init__.py
--rw-r--r--  2.0 unx     6918 b- defN 24-May-31 09:48 nucliadb/ingest/consumer/auditing.py
--rw-r--r--  2.0 unx    12174 b- defN 24-May-31 09:48 nucliadb/ingest/consumer/consumer.py
--rw-r--r--  2.0 unx     3945 b- defN 24-May-31 09:48 nucliadb/ingest/consumer/materializer.py
--rw-r--r--  2.0 unx     1075 b- defN 24-May-31 09:48 nucliadb/ingest/consumer/metrics.py
--rw-r--r--  2.0 unx     9543 b- defN 24-May-31 09:48 nucliadb/ingest/consumer/pull.py
--rw-r--r--  2.0 unx     6871 b- defN 24-May-31 09:48 nucliadb/ingest/consumer/service.py
--rw-r--r--  2.0 unx     4331 b- defN 24-May-31 09:48 nucliadb/ingest/consumer/shard_creator.py
--rw-r--r--  2.0 unx     2656 b- defN 24-May-31 09:48 nucliadb/ingest/consumer/utils.py
--rw-r--r--  2.0 unx      835 b- defN 24-May-31 09:48 nucliadb/ingest/fields/__init__.py
--rw-r--r--  2.0 unx    17797 b- defN 24-May-31 09:48 nucliadb/ingest/fields/base.py
--rw-r--r--  2.0 unx     7047 b- defN 24-May-31 09:48 nucliadb/ingest/fields/conversation.py
--rw-r--r--  2.0 unx     1223 b- defN 24-May-31 09:48 nucliadb/ingest/fields/date.py
--rw-r--r--  2.0 unx     1205 b- defN 24-May-31 09:48 nucliadb/ingest/fields/exceptions.py
--rw-r--r--  2.0 unx     4840 b- defN 24-May-31 09:48 nucliadb/ingest/fields/file.py
--rw-r--r--  2.0 unx     1547 b- defN 24-May-31 09:48 nucliadb/ingest/fields/generic.py
--rw-r--r--  2.0 unx     1235 b- defN 24-May-31 09:48 nucliadb/ingest/fields/keywordset.py
--rw-r--r--  2.0 unx     2250 b- defN 24-May-31 09:48 nucliadb/ingest/fields/layout.py
--rw-r--r--  2.0 unx     4212 b- defN 24-May-31 09:48 nucliadb/ingest/fields/link.py
--rw-r--r--  2.0 unx     1319 b- defN 24-May-31 09:48 nucliadb/ingest/fields/text.py
--rw-r--r--  2.0 unx      835 b- defN 24-May-31 09:48 nucliadb/ingest/orm/__init__.py
--rw-r--r--  2.0 unx    28721 b- defN 24-May-31 09:48 nucliadb/ingest/orm/brain.py
--rw-r--r--  2.0 unx     6954 b- defN 24-May-31 09:48 nucliadb/ingest/orm/broker_message.py
--rw-r--r--  2.0 unx    15758 b- defN 24-May-31 09:48 nucliadb/ingest/orm/entities.py
--rw-r--r--  2.0 unx     1326 b- defN 24-May-31 09:48 nucliadb/ingest/orm/exceptions.py
--rw-r--r--  2.0 unx    16914 b- defN 24-May-31 09:48 nucliadb/ingest/orm/knowledgebox.py
--rw-r--r--  2.0 unx     1096 b- defN 24-May-31 09:48 nucliadb/ingest/orm/metrics.py
--rw-r--r--  2.0 unx    54798 b- defN 24-May-31 09:48 nucliadb/ingest/orm/resource.py
--rw-r--r--  2.0 unx     2685 b- defN 24-May-31 09:48 nucliadb/ingest/orm/utils.py
--rw-r--r--  2.0 unx    27092 b- defN 24-May-31 09:48 nucliadb/ingest/orm/processor/__init__.py
--rw-r--r--  2.0 unx     5090 b- defN 24-May-31 09:48 nucliadb/ingest/orm/processor/auditing.py
--rw-r--r--  2.0 unx     1690 b- defN 24-May-31 09:48 nucliadb/ingest/orm/processor/sequence_manager.py
--rw-r--r--  2.0 unx     2057 b- defN 24-May-31 09:48 nucliadb/ingest/service/__init__.py
--rw-r--r--  2.0 unx      835 b- defN 24-May-31 09:48 nucliadb/ingest/service/exceptions.py
--rw-r--r--  2.0 unx    32883 b- defN 24-May-31 09:48 nucliadb/ingest/service/writer.py
--rw-r--r--  2.0 unx      835 b- defN 24-May-31 09:48 nucliadb/ingest/tests/__init__.py
--rw-r--r--  2.0 unx     1157 b- defN 24-May-31 09:48 nucliadb/ingest/tests/conftest.py
--rw-r--r--  2.0 unx    24111 b- defN 24-May-31 09:48 nucliadb/ingest/tests/fixtures.py
--rw-r--r--  2.0 unx    62843 b- defN 24-May-31 09:48 nucliadb/ingest/tests/vectors.py
--rw-r--r--  2.0 unx      835 b- defN 24-May-31 09:48 nucliadb/ingest/tests/integration/__init__.py
--rw-r--r--  2.0 unx      833 b- defN 24-May-31 09:48 nucliadb/ingest/tests/integration/consumer/__init__.py
--rw-r--r--  2.0 unx     2500 b- defN 24-May-31 09:48 nucliadb/ingest/tests/integration/consumer/test_auditing.py
--rw-r--r--  2.0 unx     3836 b- defN 24-May-31 09:48 nucliadb/ingest/tests/integration/consumer/test_materializer.py
--rw-r--r--  2.0 unx     4470 b- defN 24-May-31 09:48 nucliadb/ingest/tests/integration/consumer/test_pull.py
--rw-r--r--  2.0 unx     2763 b- defN 24-May-31 09:48 nucliadb/ingest/tests/integration/consumer/test_service.py
--rw-r--r--  2.0 unx     2019 b- defN 24-May-31 09:48 nucliadb/ingest/tests/integration/consumer/test_shard_creator.py
--rw-r--r--  2.0 unx      835 b- defN 24-May-31 09:48 nucliadb/ingest/tests/integration/ingest/__init__.py
--rw-r--r--  2.0 unx    27247 b- defN 24-May-31 09:48 nucliadb/ingest/tests/integration/ingest/test_ingest.py
--rw-r--r--  2.0 unx     3040 b- defN 24-May-31 09:48 nucliadb/ingest/tests/integration/ingest/test_processing_engine.py
--rw-r--r--  2.0 unx     8586 b- defN 24-May-31 09:48 nucliadb/ingest/tests/integration/ingest/test_relations.py
--rw-r--r--  2.0 unx     5637 b- defN 24-May-31 09:48 nucliadb/ingest/tests/integration/ingest/test_vectorsets.py
--rw-r--r--  2.0 unx      835 b- defN 24-May-31 09:48 nucliadb/ingest/tests/unit/__init__.py
--rw-r--r--  2.0 unx     1189 b- defN 24-May-31 09:48 nucliadb/ingest/tests/unit/test_cache.py
--rw-r--r--  2.0 unx     1432 b- defN 24-May-31 09:48 nucliadb/ingest/tests/unit/test_partitions.py
--rw-r--r--  2.0 unx     5807 b- defN 24-May-31 09:48 nucliadb/ingest/tests/unit/test_processing.py
--rw-r--r--  2.0 unx      978 b- defN 24-May-31 09:48 nucliadb/ingest/tests/unit/test_settings.py
--rw-r--r--  2.0 unx      833 b- defN 24-May-31 09:48 nucliadb/ingest/tests/unit/consumer/__init__.py
--rw-r--r--  2.0 unx     3885 b- defN 24-May-31 09:48 nucliadb/ingest/tests/unit/consumer/test_auditing.py
--rw-r--r--  2.0 unx     2472 b- defN 24-May-31 09:48 nucliadb/ingest/tests/unit/consumer/test_consumer.py
--rw-r--r--  2.0 unx     2063 b- defN 24-May-31 09:48 nucliadb/ingest/tests/unit/consumer/test_pull.py
--rw-r--r--  2.0 unx     4140 b- defN 24-May-31 09:48 nucliadb/ingest/tests/unit/consumer/test_shard_creator.py
--rw-r--r--  2.0 unx     1934 b- defN 24-May-31 09:48 nucliadb/ingest/tests/unit/consumer/test_utils.py
--rw-r--r--  2.0 unx      835 b- defN 24-May-31 09:48 nucliadb/ingest/tests/unit/orm/__init__.py
--rw-r--r--  2.0 unx     9876 b- defN 24-May-31 09:48 nucliadb/ingest/tests/unit/orm/test_brain.py
--rw-r--r--  2.0 unx     2572 b- defN 24-May-31 09:48 nucliadb/ingest/tests/unit/orm/test_brain_vectors.py
--rw-r--r--  2.0 unx     1174 b- defN 24-May-31 09:48 nucliadb/ingest/tests/unit/orm/test_orm_utils.py
--rw-r--r--  2.0 unx     4045 b- defN 24-May-31 09:48 nucliadb/ingest/tests/unit/orm/test_processor.py
--rw-r--r--  2.0 unx    11033 b- defN 24-May-31 09:48 nucliadb/ingest/tests/unit/orm/test_resource.py
--rw-r--r--  2.0 unx     2216 b- defN 24-May-31 09:48 nucliadb/middleware/__init__.py
--rw-r--r--  2.0 unx     3912 b- defN 24-May-31 09:48 nucliadb/middleware/transaction.py
--rw-r--r--  2.0 unx      835 b- defN 24-May-31 09:48 nucliadb/migrator/__init__.py
--rw-r--r--  2.0 unx     2119 b- defN 24-May-31 09:48 nucliadb/migrator/command.py
--rw-r--r--  2.0 unx     1334 b- defN 24-May-31 09:48 nucliadb/migrator/context.py
--rw-r--r--  2.0 unx     5104 b- defN 24-May-31 09:48 nucliadb/migrator/datamanager.py
--rw-r--r--  2.0 unx      889 b- defN 24-May-31 09:48 nucliadb/migrator/exceptions.py
--rw-r--r--  2.0 unx     9370 b- defN 24-May-31 09:48 nucliadb/migrator/migrator.py
--rw-r--r--  2.0 unx     1145 b- defN 24-May-31 09:48 nucliadb/migrator/models.py
--rw-r--r--  2.0 unx     1144 b- defN 24-May-31 09:48 nucliadb/migrator/settings.py
--rw-r--r--  2.0 unx     2346 b- defN 24-May-31 09:48 nucliadb/migrator/utils.py
--rw-r--r--  2.0 unx      835 b- defN 24-May-31 09:48 nucliadb/models/__init__.py
--rw-r--r--  2.0 unx     1599 b- defN 24-May-31 09:48 nucliadb/models/responses.py
--rw-r--r--  2.0 unx     6041 b- defN 24-May-31 09:48 nucliadb/purge/__init__.py
--rw-r--r--  2.0 unx     9364 b- defN 24-May-31 09:48 nucliadb/purge/orphan_shards.py
--rw-r--r--  2.0 unx     1328 b- defN 24-May-31 09:48 nucliadb/reader/__init__.py
--rw-r--r--  2.0 unx     3709 b- defN 24-May-31 09:48 nucliadb/reader/app.py
--rw-r--r--  2.0 unx     1366 b- defN 24-May-31 09:48 nucliadb/reader/lifecycle.py
--rw-r--r--  2.0 unx     1031 b- defN 24-May-31 09:48 nucliadb/reader/openapi.py
--rw-r--r--  2.0 unx        0 b- defN 24-May-31 09:48 nucliadb/reader/py.typed
--rw-r--r--  2.0 unx     1447 b- defN 24-May-31 09:48 nucliadb/reader/run.py
--rw-r--r--  2.0 unx      872 b- defN 24-May-31 09:48 nucliadb/reader/api/__init__.py
--rw-r--r--  2.0 unx     2458 b- defN 24-May-31 09:48 nucliadb/reader/api/models.py
--rw-r--r--  2.0 unx     1110 b- defN 24-May-31 09:48 nucliadb/reader/api/v1/__init__.py
--rw-r--r--  2.0 unx    12457 b- defN 24-May-31 09:48 nucliadb/reader/api/v1/download.py
--rw-r--r--  2.0 unx     6459 b- defN 24-May-31 09:48 nucliadb/reader/api/v1/export_import.py
--rw-r--r--  2.0 unx     3641 b- defN 24-May-31 09:48 nucliadb/reader/api/v1/knowledgebox.py
--rw-r--r--  2.0 unx     2099 b- defN 24-May-31 09:48 nucliadb/reader/api/v1/learning_collector.py
--rw-r--r--  2.0 unx     4472 b- defN 24-May-31 09:48 nucliadb/reader/api/v1/learning_config.py
--rw-r--r--  2.0 unx    13961 b- defN 24-May-31 09:48 nucliadb/reader/api/v1/resource.py
--rw-r--r--  2.0 unx     1011 b- defN 24-May-31 09:48 nucliadb/reader/api/v1/router.py
--rw-r--r--  2.0 unx    12115 b- defN 24-May-31 09:48 nucliadb/reader/api/v1/services.py
--rw-r--r--  2.0 unx      835 b- defN 24-May-31 09:48 nucliadb/reader/reader/__init__.py
--rw-r--r--  2.0 unx     7979 b- defN 24-May-31 09:48 nucliadb/reader/reader/notifications.py
--rw-r--r--  2.0 unx      835 b- defN 24-May-31 09:48 nucliadb/reader/tests/__init__.py
--rw-r--r--  2.0 unx     1224 b- defN 24-May-31 09:48 nucliadb/reader/tests/conftest.py
--rw-r--r--  2.0 unx     4355 b- defN 24-May-31 09:48 nucliadb/reader/tests/fixtures.py
--rw-r--r--  2.0 unx     2748 b- defN 24-May-31 09:48 nucliadb/reader/tests/test_list_resources.py
--rw-r--r--  2.0 unx    10199 b- defN 24-May-31 09:48 nucliadb/reader/tests/test_reader_file_download.py
--rw-r--r--  2.0 unx    10586 b- defN 24-May-31 09:48 nucliadb/reader/tests/test_reader_resource.py
--rw-r--r--  2.0 unx     6535 b- defN 24-May-31 09:48 nucliadb/reader/tests/test_reader_resource_field.py
--rw-r--r--  2.0 unx     1535 b- defN 24-May-31 09:48 nucliadb/search/__init__.py
--rw-r--r--  2.0 unx     4905 b- defN 24-May-31 09:48 nucliadb/search/app.py
--rw-r--r--  2.0 unx     1956 b- defN 24-May-31 09:48 nucliadb/search/lifecycle.py
--rw-r--r--  2.0 unx     1016 b- defN 24-May-31 09:48 nucliadb/search/openapi.py
--rw-r--r--  2.0 unx    20665 b- defN 24-May-31 09:48 nucliadb/search/predict.py
--rw-r--r--  2.0 unx        0 b- defN 24-May-31 09:48 nucliadb/search/py.typed
--rw-r--r--  2.0 unx     1402 b- defN 24-May-31 09:48 nucliadb/search/run.py
--rw-r--r--  2.0 unx     1193 b- defN 24-May-31 09:48 nucliadb/search/settings.py
--rw-r--r--  2.0 unx     1037 b- defN 24-May-31 09:48 nucliadb/search/utilities.py
--rw-r--r--  2.0 unx      835 b- defN 24-May-31 09:48 nucliadb/search/api/__init__.py
--rw-r--r--  2.0 unx     1298 b- defN 24-May-31 09:48 nucliadb/search/api/v1/__init__.py
--rw-r--r--  2.0 unx     3435 b- defN 24-May-31 09:48 nucliadb/search/api/v1/ask.py
--rw-r--r--  2.0 unx     9514 b- defN 24-May-31 09:48 nucliadb/search/api/v1/chat.py
--rw-r--r--  2.0 unx     2668 b- defN 24-May-31 09:48 nucliadb/search/api/v1/feedback.py
--rw-r--r--  2.0 unx     8795 b- defN 24-May-31 09:48 nucliadb/search/api/v1/find.py
--rw-r--r--  2.0 unx     6938 b- defN 24-May-31 09:48 nucliadb/search/api/v1/knowledgebox.py
--rw-r--r--  2.0 unx     3047 b- defN 24-May-31 09:48 nucliadb/search/api/v1/predict_proxy.py
--rw-r--r--  2.0 unx      988 b- defN 24-May-31 09:48 nucliadb/search/api/v1/router.py
--rw-r--r--  2.0 unx    19262 b- defN 24-May-31 09:48 nucliadb/search/api/v1/search.py
--rw-r--r--  2.0 unx     5970 b- defN 24-May-31 09:48 nucliadb/search/api/v1/suggest.py
--rw-r--r--  2.0 unx     2499 b- defN 24-May-31 09:48 nucliadb/search/api/v1/summarize.py
--rw-r--r--  2.0 unx     1434 b- defN 24-May-31 09:48 nucliadb/search/api/v1/utils.py
--rw-r--r--  2.0 unx      835 b- defN 24-May-31 09:48 nucliadb/search/api/v1/resource/__init__.py
--rw-r--r--  2.0 unx     3866 b- defN 24-May-31 09:48 nucliadb/search/api/v1/resource/ask.py
--rw-r--r--  2.0 unx     5863 b- defN 24-May-31 09:48 nucliadb/search/api/v1/resource/chat.py
--rw-r--r--  2.0 unx     5303 b- defN 24-May-31 09:48 nucliadb/search/api/v1/resource/search.py
--rw-r--r--  2.0 unx      833 b- defN 24-May-31 09:48 nucliadb/search/requesters/__init__.py
--rw-r--r--  2.0 unx     9111 b- defN 24-May-31 09:48 nucliadb/search/requesters/utils.py
--rw-r--r--  2.0 unx      835 b- defN 24-May-31 09:48 nucliadb/search/search/__init__.py
--rw-r--r--  2.0 unx     2746 b- defN 24-May-31 09:48 nucliadb/search/search/cache.py
--rw-r--r--  2.0 unx     1154 b- defN 24-May-31 09:48 nucliadb/search/search/exceptions.py
--rw-r--r--  2.0 unx     5465 b- defN 24-May-31 09:48 nucliadb/search/search/fetch.py
--rw-r--r--  2.0 unx     6513 b- defN 24-May-31 09:48 nucliadb/search/search/filters.py
--rw-r--r--  2.0 unx     4612 b- defN 24-May-31 09:48 nucliadb/search/search/find.py
--rw-r--r--  2.0 unx    17152 b- defN 24-May-31 09:48 nucliadb/search/search/find_merge.py
--rw-r--r--  2.0 unx    21282 b- defN 24-May-31 09:48 nucliadb/search/search/merge.py
--rw-r--r--  2.0 unx     1130 b- defN 24-May-31 09:48 nucliadb/search/search/metrics.py
--rw-r--r--  2.0 unx     8698 b- defN 24-May-31 09:48 nucliadb/search/search/paragraphs.py
--rw-r--r--  2.0 unx     3026 b- defN 24-May-31 09:48 nucliadb/search/search/predict_proxy.py
--rw-r--r--  2.0 unx    31093 b- defN 24-May-31 09:48 nucliadb/search/search/query.py
--rw-r--r--  2.0 unx     3018 b- defN 24-May-31 09:48 nucliadb/search/search/shards.py
--rw-r--r--  2.0 unx     5101 b- defN 24-May-31 09:48 nucliadb/search/search/summarize.py
--rw-r--r--  2.0 unx     2438 b- defN 24-May-31 09:48 nucliadb/search/search/utils.py
--rw-r--r--  2.0 unx      835 b- defN 24-May-31 09:48 nucliadb/search/search/chat/__init__.py
--rw-r--r--  2.0 unx    16676 b- defN 24-May-31 09:48 nucliadb/search/search/chat/ask.py
--rw-r--r--  2.0 unx     2058 b- defN 24-May-31 09:48 nucliadb/search/search/chat/images.py
--rw-r--r--  2.0 unx    20793 b- defN 24-May-31 09:48 nucliadb/search/search/chat/prompt.py
--rw-r--r--  2.0 unx    17543 b- defN 24-May-31 09:48 nucliadb/search/search/chat/query.py
--rw-r--r--  2.0 unx      835 b- defN 24-May-31 09:48 nucliadb/search/tests/__init__.py
--rw-r--r--  2.0 unx     1295 b- defN 24-May-31 09:48 nucliadb/search/tests/conftest.py
--rw-r--r--  2.0 unx     6578 b- defN 24-May-31 09:48 nucliadb/search/tests/fixtures.py
--rw-r--r--  2.0 unx    15480 b- defN 24-May-31 09:48 nucliadb/search/tests/node.py
--rw-r--r--  2.0 unx      833 b- defN 24-May-31 09:48 nucliadb/search/tests/unit/__init__.py
--rw-r--r--  2.0 unx     2649 b- defN 24-May-31 09:48 nucliadb/search/tests/unit/test_app.py
--rw-r--r--  2.0 unx     3374 b- defN 24-May-31 09:48 nucliadb/search/tests/unit/test_find_merge.py
--rw-r--r--  2.0 unx     1400 b- defN 24-May-31 09:48 nucliadb/search/tests/unit/test_merge.py
--rw-r--r--  2.0 unx    15721 b- defN 24-May-31 09:48 nucliadb/search/tests/unit/test_predict.py
--rw-r--r--  2.0 unx     1328 b- defN 24-May-31 09:48 nucliadb/search/tests/unit/test_run.py
--rw-r--r--  2.0 unx      835 b- defN 24-May-31 09:48 nucliadb/search/tests/unit/api/__init__.py
--rw-r--r--  2.0 unx      835 b- defN 24-May-31 09:48 nucliadb/search/tests/unit/api/v1/__init__.py
--rw-r--r--  2.0 unx     3759 b- defN 24-May-31 09:48 nucliadb/search/tests/unit/api/v1/test_ask.py
--rw-r--r--  2.0 unx     2966 b- defN 24-May-31 09:48 nucliadb/search/tests/unit/api/v1/test_chat.py
--rw-r--r--  2.0 unx     2865 b- defN 24-May-31 09:48 nucliadb/search/tests/unit/api/v1/test_predict_proxy.py
--rw-r--r--  2.0 unx     2901 b- defN 24-May-31 09:48 nucliadb/search/tests/unit/api/v1/test_summarize.py
--rw-r--r--  2.0 unx      835 b- defN 24-May-31 09:48 nucliadb/search/tests/unit/api/v1/resource/__init__.py
--rw-r--r--  2.0 unx     3040 b- defN 24-May-31 09:48 nucliadb/search/tests/unit/api/v1/resource/test_chat.py
--rw-r--r--  2.0 unx      833 b- defN 24-May-31 09:48 nucliadb/search/tests/unit/search/__init__.py
--rw-r--r--  2.0 unx     8586 b- defN 24-May-31 09:48 nucliadb/search/tests/unit/search/test_chat_prompt.py
--rw-r--r--  2.0 unx     3736 b- defN 24-May-31 09:48 nucliadb/search/tests/unit/search/test_fetch.py
--rw-r--r--  2.0 unx     4306 b- defN 24-May-31 09:48 nucliadb/search/tests/unit/search/test_filters.py
--rw-r--r--  2.0 unx     4492 b- defN 24-May-31 09:48 nucliadb/search/tests/unit/search/test_paragraphs.py
--rw-r--r--  2.0 unx     3496 b- defN 24-May-31 09:48 nucliadb/search/tests/unit/search/test_predict_proxy.py
--rw-r--r--  2.0 unx     5121 b- defN 24-May-31 09:48 nucliadb/search/tests/unit/search/test_query.py
--rw-r--r--  2.0 unx      833 b- defN 24-May-31 09:48 nucliadb/search/tests/unit/search/requesters/__init__.py
--rw-r--r--  2.0 unx     6455 b- defN 24-May-31 09:48 nucliadb/search/tests/unit/search/requesters/test_utils.py
--rw-r--r--  2.0 unx      835 b- defN 24-May-31 09:48 nucliadb/search/tests/unit/search/search/__init__.py
--rw-r--r--  2.0 unx     1759 b- defN 24-May-31 09:48 nucliadb/search/tests/unit/search/search/test_shards.py
--rw-r--r--  2.0 unx     2511 b- defN 24-May-31 09:48 nucliadb/search/tests/unit/search/search/test_utils.py
--rw-r--r--  2.0 unx      835 b- defN 24-May-31 09:48 nucliadb/standalone/__init__.py
--rw-r--r--  2.0 unx     6746 b- defN 24-May-31 09:48 nucliadb/standalone/api_router.py
--rw-r--r--  2.0 unx     5763 b- defN 24-May-31 09:48 nucliadb/standalone/app.py
--rw-r--r--  2.0 unx     7800 b- defN 24-May-31 09:48 nucliadb/standalone/auth.py
--rw-r--r--  2.0 unx     5313 b- defN 24-May-31 09:48 nucliadb/standalone/config.py
--rw-r--r--  2.0 unx     6986 b- defN 24-May-31 09:48 nucliadb/standalone/introspect.py
--rw-r--r--  2.0 unx     2488 b- defN 24-May-31 09:48 nucliadb/standalone/lifecycle.py
--rw-r--r--  2.0 unx     1980 b- defN 24-May-31 09:48 nucliadb/standalone/migrations.py
--rw-r--r--  2.0 unx     1322 b- defN 24-May-31 09:48 nucliadb/standalone/purge.py
--rw-r--r--  2.0 unx        0 b- defN 24-May-31 09:48 nucliadb/standalone/py.typed
--rw-r--r--  2.0 unx     5636 b- defN 24-May-31 09:48 nucliadb/standalone/run.py
--rw-r--r--  2.0 unx     5822 b- defN 24-May-31 09:48 nucliadb/standalone/settings.py
--rw-r--r--  2.0 unx     3132 b- defN 24-May-31 09:48 nucliadb/standalone/versions.py
--rw-r--r--  2.0 unx     2285 b- defN 24-May-31 09:48 nucliadb/standalone/static/favicon.ico
--rw-r--r--  2.0 unx     3833 b- defN 24-May-31 09:48 nucliadb/standalone/static/index.html
--rw-r--r--  2.0 unx     2639 b- defN 24-May-31 09:48 nucliadb/standalone/static/logo.svg
--rw-r--r--  2.0 unx      835 b- defN 24-May-31 09:48 nucliadb/standalone/tests/__init__.py
--rw-r--r--  2.0 unx     1294 b- defN 24-May-31 09:48 nucliadb/standalone/tests/conftest.py
--rw-r--r--  2.0 unx     1319 b- defN 24-May-31 09:48 nucliadb/standalone/tests/fixtures.py
--rw-r--r--  2.0 unx      833 b- defN 24-May-31 09:48 nucliadb/standalone/tests/unit/__init__.py
--rw-r--r--  2.0 unx     1722 b- defN 24-May-31 09:48 nucliadb/standalone/tests/unit/test_api_router.py
--rw-r--r--  2.0 unx     5509 b- defN 24-May-31 09:48 nucliadb/standalone/tests/unit/test_auth.py
--rw-r--r--  2.0 unx     1334 b- defN 24-May-31 09:48 nucliadb/standalone/tests/unit/test_introspect.py
--rw-r--r--  2.0 unx     1863 b- defN 24-May-31 09:48 nucliadb/standalone/tests/unit/test_migrations.py
--rw-r--r--  2.0 unx     1546 b- defN 24-May-31 09:48 nucliadb/standalone/tests/unit/test_run.py
--rw-r--r--  2.0 unx     1972 b- defN 24-May-31 09:48 nucliadb/standalone/tests/unit/test_versions.py
--rw-r--r--  2.0 unx     1037 b- defN 24-May-31 09:48 nucliadb/tasks/__init__.py
--rw-r--r--  2.0 unx     7655 b- defN 24-May-31 09:48 nucliadb/tasks/consumer.py
--rw-r--r--  2.0 unx      924 b- defN 24-May-31 09:48 nucliadb/tasks/logger.py
--rw-r--r--  2.0 unx     1378 b- defN 24-May-31 09:48 nucliadb/tasks/models.py
--rw-r--r--  2.0 unx     3457 b- defN 24-May-31 09:48 nucliadb/tasks/producer.py
--rw-r--r--  2.0 unx     1753 b- defN 24-May-31 09:48 nucliadb/tasks/registry.py
--rw-r--r--  2.0 unx     1360 b- defN 24-May-31 09:48 nucliadb/tasks/utils.py
--rw-r--r--  2.0 unx      835 b- defN 24-May-31 09:48 nucliadb/tests/__init__.py
--rw-r--r--  2.0 unx     1229 b- defN 24-May-31 09:48 nucliadb/tests/conftest.py
--rw-r--r--  2.0 unx    22365 b- defN 24-May-31 09:48 nucliadb/tests/fixtures.py
--rw-r--r--  2.0 unx     7549 b- defN 24-May-31 09:48 nucliadb/tests/tikv.py
--rw-r--r--  2.0 unx      835 b- defN 24-May-31 09:48 nucliadb/tests/benchmarks/__init__.py
--rw-r--r--  2.0 unx     3032 b- defN 24-May-31 09:48 nucliadb/tests/benchmarks/test_search.py
--rw-r--r--  2.0 unx      919 b- defN 24-May-31 09:48 nucliadb/tests/knowledgeboxes/__init__.py
--rw-r--r--  2.0 unx     7002 b- defN 24-May-31 09:48 nucliadb/tests/knowledgeboxes/philosophy_books.py
--rw-r--r--  2.0 unx     3037 b- defN 24-May-31 09:48 nucliadb/tests/knowledgeboxes/ten_dummy_resources.py
--rw-r--r--  2.0 unx     1148 b- defN 24-May-31 09:48 nucliadb/tests/migrations/__init__.py
--rw-r--r--  2.0 unx     2726 b- defN 24-May-31 09:48 nucliadb/tests/migrations/test_migration_0017.py
--rw-r--r--  2.0 unx     3662 b- defN 24-May-31 09:48 nucliadb/tests/migrations/test_migration_0018.py
--rw-r--r--  2.0 unx     3439 b- defN 24-May-31 09:48 nucliadb/tests/migrations/test_migration_0021.py
--rw-r--r--  2.0 unx      835 b- defN 24-May-31 09:48 nucliadb/tests/unit/__init__.py
--rw-r--r--  2.0 unx     1487 b- defN 24-May-31 09:48 nucliadb/tests/unit/test_field_ids.py
--rw-r--r--  2.0 unx     2780 b- defN 24-May-31 09:48 nucliadb/tests/unit/test_health.py
--rw-r--r--  2.0 unx     1543 b- defN 24-May-31 09:48 nucliadb/tests/unit/test_kb_slugs.py
--rw-r--r--  2.0 unx     7892 b- defN 24-May-31 09:48 nucliadb/tests/unit/test_learning_proxy.py
--rw-r--r--  2.0 unx     2642 b- defN 24-May-31 09:48 nucliadb/tests/unit/test_metrics_exporter.py
--rw-r--r--  2.0 unx     1341 b- defN 24-May-31 09:48 nucliadb/tests/unit/test_openapi.py
--rw-r--r--  2.0 unx     3649 b- defN 24-May-31 09:48 nucliadb/tests/unit/test_purge.py
--rw-r--r--  2.0 unx      835 b- defN 24-May-31 09:48 nucliadb/tests/unit/common/__init__.py
--rw-r--r--  2.0 unx     1268 b- defN 24-May-31 09:48 nucliadb/tests/unit/common/test_context.py
--rw-r--r--  2.0 unx      835 b- defN 24-May-31 09:48 nucliadb/tests/unit/common/cluster/__init__.py
--rw-r--r--  2.0 unx    12240 b- defN 24-May-31 09:48 nucliadb/tests/unit/common/cluster/test_cluster.py
--rw-r--r--  2.0 unx     5387 b- defN 24-May-31 09:48 nucliadb/tests/unit/common/cluster/test_kb_shard_manager.py
--rw-r--r--  2.0 unx     1428 b- defN 24-May-31 09:48 nucliadb/tests/unit/common/cluster/test_rebalance.py
--rw-r--r--  2.0 unx     9465 b- defN 24-May-31 09:48 nucliadb/tests/unit/common/cluster/test_rollover.py
--rw-r--r--  2.0 unx      835 b- defN 24-May-31 09:48 nucliadb/tests/unit/common/cluster/discovery/__init__.py
--rw-r--r--  2.0 unx     5627 b- defN 24-May-31 09:48 nucliadb/tests/unit/common/cluster/discovery/test_k8s.py
--rw-r--r--  2.0 unx      833 b- defN 24-May-31 09:48 nucliadb/tests/unit/common/cluster/standalone/__init__.py
--rw-r--r--  2.0 unx     3761 b- defN 24-May-31 09:48 nucliadb/tests/unit/common/cluster/standalone/test_service.py
--rw-r--r--  2.0 unx     2136 b- defN 24-May-31 09:48 nucliadb/tests/unit/common/cluster/standalone/test_utils.py
--rw-r--r--  2.0 unx      833 b- defN 24-May-31 09:48 nucliadb/tests/unit/common/maindb/__init__.py
--rw-r--r--  2.0 unx     3579 b- defN 24-May-31 09:48 nucliadb/tests/unit/common/maindb/test_driver.py
--rw-r--r--  2.0 unx     2119 b- defN 24-May-31 09:48 nucliadb/tests/unit/common/maindb/test_tikv.py
--rw-r--r--  2.0 unx     3213 b- defN 24-May-31 09:48 nucliadb/tests/unit/common/maindb/test_utils.py
--rw-r--r--  2.0 unx      835 b- defN 24-May-31 09:48 nucliadb/tests/unit/export_import/__init__.py
--rw-r--r--  2.0 unx     1435 b- defN 24-May-31 09:48 nucliadb/tests/unit/export_import/test_datamanager.py
--rw-r--r--  2.0 unx     9706 b- defN 24-May-31 09:48 nucliadb/tests/unit/export_import/test_utils.py
--rw-r--r--  2.0 unx      835 b- defN 24-May-31 09:48 nucliadb/tests/unit/migrator/__init__.py
--rw-r--r--  2.0 unx     3233 b- defN 24-May-31 09:48 nucliadb/tests/unit/migrator/test_migrator.py
--rw-r--r--  2.0 unx      835 b- defN 24-May-31 09:48 nucliadb/tests/unit/tasks/__init__.py
--rw-r--r--  2.0 unx     1375 b- defN 24-May-31 09:48 nucliadb/tests/unit/tasks/conftest.py
--rw-r--r--  2.0 unx     2714 b- defN 24-May-31 09:48 nucliadb/tests/unit/tasks/test_consumer.py
--rw-r--r--  2.0 unx     3189 b- defN 24-May-31 09:48 nucliadb/tests/unit/tasks/test_producer.py
--rw-r--r--  2.0 unx     1827 b- defN 24-May-31 09:48 nucliadb/tests/unit/tasks/test_tasks.py
--rw-r--r--  2.0 unx     2507 b- defN 24-May-31 09:48 nucliadb/tests/utils/__init__.py
--rw-r--r--  2.0 unx     1797 b- defN 24-May-31 09:48 nucliadb/tests/utils/aiohttp_session.py
--rw-r--r--  2.0 unx     2533 b- defN 24-May-31 09:48 nucliadb/tests/utils/entities.py
--rw-r--r--  2.0 unx     6327 b- defN 24-May-31 09:48 nucliadb/tests/utils/broker_messages/__init__.py
--rw-r--r--  2.0 unx     7557 b- defN 24-May-31 09:48 nucliadb/tests/utils/broker_messages/fields.py
--rw-r--r--  2.0 unx     1196 b- defN 24-May-31 09:48 nucliadb/tests/utils/broker_messages/helpers.py
--rw-r--r--  2.0 unx     1325 b- defN 24-May-31 09:48 nucliadb/train/__init__.py
--rw-r--r--  2.0 unx     3530 b- defN 24-May-31 09:48 nucliadb/train/app.py
--rw-r--r--  2.0 unx     3800 b- defN 24-May-31 09:48 nucliadb/train/generator.py
--rw-r--r--  2.0 unx     1698 b- defN 24-May-31 09:48 nucliadb/train/lifecycle.py
--rw-r--r--  2.0 unx     1198 b- defN 24-May-31 09:48 nucliadb/train/models.py
--rw-r--r--  2.0 unx     5776 b- defN 24-May-31 09:48 nucliadb/train/nodes.py
--rw-r--r--  2.0 unx        0 b- defN 24-May-31 09:48 nucliadb/train/py.typed
--rw-r--r--  2.0 unx     1400 b- defN 24-May-31 09:48 nucliadb/train/run.py
--rw-r--r--  2.0 unx     5926 b- defN 24-May-31 09:48 nucliadb/train/servicer.py
--rw-r--r--  2.0 unx     1415 b- defN 24-May-31 09:48 nucliadb/train/settings.py
--rw-r--r--  2.0 unx     1496 b- defN 24-May-31 09:48 nucliadb/train/types.py
--rw-r--r--  2.0 unx     3265 b- defN 24-May-31 09:48 nucliadb/train/upload.py
--rw-r--r--  2.0 unx     6420 b- defN 24-May-31 09:48 nucliadb/train/uploader.py
--rw-r--r--  2.0 unx     3179 b- defN 24-May-31 09:48 nucliadb/train/utils.py
--rw-r--r--  2.0 unx      835 b- defN 24-May-31 09:48 nucliadb/train/api/__init__.py
--rw-r--r--  2.0 unx     1479 b- defN 24-May-31 09:48 nucliadb/train/api/utils.py
--rw-r--r--  2.0 unx      928 b- defN 24-May-31 09:48 nucliadb/train/api/v1/__init__.py
--rw-r--r--  2.0 unx     2071 b- defN 24-May-31 09:48 nucliadb/train/api/v1/check.py
--rw-r--r--  2.0 unx      910 b- defN 24-May-31 09:48 nucliadb/train/api/v1/router.py
--rw-r--r--  2.0 unx     1908 b- defN 24-May-31 09:48 nucliadb/train/api/v1/shards.py
--rw-r--r--  2.0 unx     2135 b- defN 24-May-31 09:48 nucliadb/train/api/v1/trainset.py
--rw-r--r--  2.0 unx      835 b- defN 24-May-31 09:48 nucliadb/train/generators/__init__.py
--rw-r--r--  2.0 unx     3723 b- defN 24-May-31 09:48 nucliadb/train/generators/field_classifier.py
--rw-r--r--  2.0 unx     6712 b- defN 24-May-31 09:48 nucliadb/train/generators/image_classifier.py
--rw-r--r--  2.0 unx     2789 b- defN 24-May-31 09:48 nucliadb/train/generators/paragraph_classifier.py
--rw-r--r--  2.0 unx     3590 b- defN 24-May-31 09:48 nucliadb/train/generators/paragraph_streaming.py
--rw-r--r--  2.0 unx     5372 b- defN 24-May-31 09:48 nucliadb/train/generators/question_answer_streaming.py
--rw-r--r--  2.0 unx     5160 b- defN 24-May-31 09:48 nucliadb/train/generators/sentence_classifier.py
--rw-r--r--  2.0 unx    10446 b- defN 24-May-31 09:48 nucliadb/train/generators/token_classifier.py
--rw-r--r--  2.0 unx     3877 b- defN 24-May-31 09:48 nucliadb/train/generators/utils.py
--rw-r--r--  2.0 unx      835 b- defN 24-May-31 09:48 nucliadb/train/tests/__init__.py
--rw-r--r--  2.0 unx     1125 b- defN 24-May-31 09:48 nucliadb/train/tests/conftest.py
--rw-r--r--  2.0 unx    11063 b- defN 24-May-31 09:48 nucliadb/train/tests/fixtures.py
--rw-r--r--  2.0 unx     4598 b- defN 24-May-31 09:48 nucliadb/train/tests/test_field_classification.py
--rw-r--r--  2.0 unx     2729 b- defN 24-May-31 09:48 nucliadb/train/tests/test_get_entities.py
--rw-r--r--  2.0 unx     1660 b- defN 24-May-31 09:48 nucliadb/train/tests/test_get_info.py
--rw-r--r--  2.0 unx     1382 b- defN 24-May-31 09:48 nucliadb/train/tests/test_get_ontology.py
--rw-r--r--  2.0 unx     2201 b- defN 24-May-31 09:48 nucliadb/train/tests/test_get_ontology_count.py
--rw-r--r--  2.0 unx     7669 b- defN 24-May-31 09:48 nucliadb/train/tests/test_image_classification.py
--rw-r--r--  2.0 unx     1416 b- defN 24-May-31 09:48 nucliadb/train/tests/test_list_fields.py
--rw-r--r--  2.0 unx     2944 b- defN 24-May-31 09:48 nucliadb/train/tests/test_list_paragraphs.py
--rw-r--r--  2.0 unx     1423 b- defN 24-May-31 09:48 nucliadb/train/tests/test_list_resources.py
--rw-r--r--  2.0 unx     2947 b- defN 24-May-31 09:48 nucliadb/train/tests/test_list_sentences.py
--rw-r--r--  2.0 unx     4645 b- defN 24-May-31 09:48 nucliadb/train/tests/test_paragraph_classification.py
--rw-r--r--  2.0 unx     4320 b- defN 24-May-31 09:48 nucliadb/train/tests/test_paragraph_streaming.py
--rw-r--r--  2.0 unx     8751 b- defN 24-May-31 09:48 nucliadb/train/tests/test_question_answer_streaming.py
--rw-r--r--  2.0 unx     5051 b- defN 24-May-31 09:48 nucliadb/train/tests/test_sentence_classification.py
--rw-r--r--  2.0 unx     5583 b- defN 24-May-31 09:48 nucliadb/train/tests/test_token_classification.py
--rw-r--r--  2.0 unx     3324 b- defN 24-May-31 09:48 nucliadb/train/tests/utils.py
--rw-r--r--  2.0 unx     1328 b- defN 24-May-31 09:48 nucliadb/writer/__init__.py
--rw-r--r--  2.0 unx     4268 b- defN 24-May-31 09:48 nucliadb/writer/app.py
--rw-r--r--  2.0 unx    19483 b- defN 24-May-31 09:48 nucliadb/writer/back_pressure.py
--rw-r--r--  2.0 unx      972 b- defN 24-May-31 09:48 nucliadb/writer/exceptions.py
--rw-r--r--  2.0 unx     1953 b- defN 24-May-31 09:48 nucliadb/writer/lifecycle.py
--rw-r--r--  2.0 unx     1032 b- defN 24-May-31 09:48 nucliadb/writer/openapi.py
--rw-r--r--  2.0 unx        0 b- defN 24-May-31 09:48 nucliadb/writer/py.typed
--rw-r--r--  2.0 unx     1448 b- defN 24-May-31 09:48 nucliadb/writer/run.py
--rw-r--r--  2.0 unx     3103 b- defN 24-May-31 09:48 nucliadb/writer/settings.py
--rw-r--r--  2.0 unx     1036 b- defN 24-May-31 09:48 nucliadb/writer/utilities.py
--rw-r--r--  2.0 unx      835 b- defN 24-May-31 09:48 nucliadb/writer/api/__init__.py
--rw-r--r--  2.0 unx     1429 b- defN 24-May-31 09:48 nucliadb/writer/api/constants.py
--rw-r--r--  2.0 unx     1095 b- defN 24-May-31 09:48 nucliadb/writer/api/v1/__init__.py
--rw-r--r--  2.0 unx     6421 b- defN 24-May-31 09:48 nucliadb/writer/api/v1/export_import.py
--rw-r--r--  2.0 unx    24482 b- defN 24-May-31 09:48 nucliadb/writer/api/v1/field.py
--rw-r--r--  2.0 unx     5248 b- defN 24-May-31 09:48 nucliadb/writer/api/v1/knowledgebox.py
--rw-r--r--  2.0 unx     2058 b- defN 24-May-31 09:48 nucliadb/writer/api/v1/learning_config.py
--rw-r--r--  2.0 unx    18628 b- defN 24-May-31 09:48 nucliadb/writer/api/v1/resource.py
--rw-r--r--  2.0 unx     1034 b- defN 24-May-31 09:48 nucliadb/writer/api/v1/router.py
--rw-r--r--  2.0 unx    10216 b- defN 24-May-31 09:48 nucliadb/writer/api/v1/services.py
--rw-r--r--  2.0 unx    30985 b- defN 24-May-31 09:48 nucliadb/writer/api/v1/upload.py
--rw-r--r--  2.0 unx     1612 b- defN 24-May-31 09:48 nucliadb/writer/layouts/__init__.py
--rw-r--r--  2.0 unx     2115 b- defN 24-May-31 09:48 nucliadb/writer/layouts/v1.py
--rw-r--r--  2.0 unx      835 b- defN 24-May-31 09:48 nucliadb/writer/resource/__init__.py
--rw-r--r--  2.0 unx     1425 b- defN 24-May-31 09:48 nucliadb/writer/resource/audit.py
--rw-r--r--  2.0 unx    10968 b- defN 24-May-31 09:48 nucliadb/writer/resource/basic.py
--rw-r--r--  2.0 unx    16740 b- defN 24-May-31 09:48 nucliadb/writer/resource/field.py
--rw-r--r--  2.0 unx     2022 b- defN 24-May-31 09:48 nucliadb/writer/resource/origin.py
--rw-r--r--  2.0 unx      835 b- defN 24-May-31 09:48 nucliadb/writer/tests/__init__.py
--rw-r--r--  2.0 unx     1200 b- defN 24-May-31 09:48 nucliadb/writer/tests/conftest.py
--rw-r--r--  2.0 unx     5971 b- defN 24-May-31 09:48 nucliadb/writer/tests/fixtures.py
--rw-r--r--  2.0 unx    15472 b- defN 24-May-31 09:48 nucliadb/writer/tests/test_fields.py
--rw-r--r--  2.0 unx    25999 b- defN 24-May-31 09:48 nucliadb/writer/tests/test_files.py
--rw-r--r--  2.0 unx     1729 b- defN 24-May-31 09:48 nucliadb/writer/tests/test_knowledgebox.py
--rw-r--r--  2.0 unx     4400 b- defN 24-May-31 09:48 nucliadb/writer/tests/test_reprocess_file_field.py
--rw-r--r--  2.0 unx    16857 b- defN 24-May-31 09:48 nucliadb/writer/tests/test_resources.py
--rw-r--r--  2.0 unx     5120 b- defN 24-May-31 09:48 nucliadb/writer/tests/test_service.py
--rw-r--r--  2.0 unx     6054 b- defN 24-May-31 09:48 nucliadb/writer/tests/test_tus.py
--rw-r--r--  2.0 unx     1287 b- defN 24-May-31 09:48 nucliadb/writer/tests/utils.py
--rw-r--r--  2.0 unx     5226 b- defN 24-May-31 09:48 nucliadb/writer/tus/__init__.py
--rw-r--r--  2.0 unx     5082 b- defN 24-May-31 09:48 nucliadb/writer/tus/dm.py
--rw-r--r--  2.0 unx     2186 b- defN 24-May-31 09:48 nucliadb/writer/tus/exceptions.py
--rw-r--r--  2.0 unx    14527 b- defN 24-May-31 09:48 nucliadb/writer/tus/gcs.py
--rw-r--r--  2.0 unx     5849 b- defN 24-May-31 09:48 nucliadb/writer/tus/local.py
--rw-r--r--  2.0 unx     4367 b- defN 24-May-31 09:48 nucliadb/writer/tus/pg.py
--rw-r--r--  2.0 unx     9069 b- defN 24-May-31 09:48 nucliadb/writer/tus/s3.py
--rw-r--r--  2.0 unx     4734 b- defN 24-May-31 09:48 nucliadb/writer/tus/storage.py
--rw-r--r--  2.0 unx     2556 b- defN 24-May-31 09:48 nucliadb/writer/tus/utils.py
--rw-r--r--  2.0 unx     4474 b- defN 24-May-31 09:50 nucliadb-4.0.3.post562.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-May-31 09:50 nucliadb-4.0.3.post562.dist-info/WHEEL
--rw-r--r--  2.0 unx     1268 b- defN 24-May-31 09:50 nucliadb-4.0.3.post562.dist-info/entry_points.txt
--rw-r--r--  2.0 unx       20 b- defN 24-May-31 09:50 nucliadb-4.0.3.post562.dist-info/top_level.txt
--rw-r--r--  2.0 unx        1 b- defN 24-May-31 09:49 nucliadb-4.0.3.post562.dist-info/zip-safe
--rw-rw-r--  2.0 unx    44525 b- defN 24-May-31 09:50 nucliadb-4.0.3.post562.dist-info/RECORD
-475 files, 2293802 bytes uncompressed, 706189 bytes compressed:  69.2%
+Zip file size: 777488 bytes, number of entries: 475
+-rw-r--r--  2.0 unx     1135 b- defN 24-Jun-03 10:23 migrations/0001_bootstrap.py
+-rw-r--r--  2.0 unx     1177 b- defN 24-Jun-03 10:23 migrations/0002_rollover_shards.py
+-rw-r--r--  2.0 unx     2436 b- defN 24-Jun-03 10:23 migrations/0003_allfields_key.py
+-rw-r--r--  2.0 unx     1177 b- defN 24-Jun-03 10:23 migrations/0004_rollover_shards.py
+-rw-r--r--  2.0 unx     1177 b- defN 24-Jun-03 10:23 migrations/0005_rollover_shards.py
+-rw-r--r--  2.0 unx     1024 b- defN 24-Jun-03 10:23 migrations/0006_rollover_shards.py
+-rw-r--r--  2.0 unx     1301 b- defN 24-Jun-03 10:23 migrations/0008_cleanup_leftover_rollover_metadata.py
+-rw-r--r--  2.0 unx     1378 b- defN 24-Jun-03 10:23 migrations/0009_upgrade_relations_and_texts_to_v2.py
+-rw-r--r--  2.0 unx     1610 b- defN 24-Jun-03 10:23 migrations/0010_fix_corrupt_indexes.py
+-rw-r--r--  2.0 unx     1843 b- defN 24-Jun-03 10:23 migrations/0011_materialize_labelset_ids.py
+-rw-r--r--  2.0 unx     1443 b- defN 24-Jun-03 10:23 migrations/0012_rollover_shards.py
+-rw-r--r--  2.0 unx     1024 b- defN 24-Jun-03 10:23 migrations/0013_rollover_shards.py
+-rw-r--r--  2.0 unx     1382 b- defN 24-Jun-03 10:23 migrations/0014_rollover_shards.py
+-rw-r--r--  2.0 unx     1462 b- defN 24-Jun-03 10:23 migrations/0015_targeted_rollover.py
+-rw-r--r--  2.0 unx     2506 b- defN 24-Jun-03 10:23 migrations/0016_upgrade_to_paragraphs_v2.py
+-rw-r--r--  2.0 unx     2100 b- defN 24-Jun-03 10:23 migrations/0017_multiple_writable_shards.py
+-rw-r--r--  2.0 unx     2264 b- defN 24-Jun-03 10:23 migrations/0018_purge_orphan_kbslugs.py
+-rw-r--r--  2.0 unx     2506 b- defN 24-Jun-03 10:23 migrations/0019_upgrade_to_paragraphs_v3.py
+-rw-r--r--  2.0 unx     3271 b- defN 24-Jun-03 10:23 migrations/0020_drain_nodes_from_cluster.py
+-rw-r--r--  2.0 unx     1734 b- defN 24-Jun-03 10:23 migrations/0021_overwrite_vectorsets_key.py
+-rw-r--r--  2.0 unx      835 b- defN 24-Jun-03 10:23 migrations/__init__.py
+-rw-r--r--  2.0 unx      891 b- defN 24-Jun-03 10:23 nucliadb/__init__.py
+-rw-r--r--  2.0 unx     3733 b- defN 24-Jun-03 10:23 nucliadb/health.py
+-rw-r--r--  2.0 unx    11793 b- defN 24-Jun-03 10:23 nucliadb/learning_proxy.py
+-rw-r--r--  2.0 unx     4820 b- defN 24-Jun-03 10:23 nucliadb/metrics_exporter.py
+-rw-r--r--  2.0 unx     2272 b- defN 24-Jun-03 10:23 nucliadb/openapi.py
+-rw-r--r--  2.0 unx        0 b- defN 24-Jun-03 10:23 nucliadb/py.typed
+-rw-r--r--  2.0 unx      835 b- defN 24-Jun-03 10:23 nucliadb/common/__init__.py
+-rw-r--r--  2.0 unx     1912 b- defN 24-Jun-03 10:23 nucliadb/common/ids.py
+-rw-r--r--  2.0 unx     5175 b- defN 24-Jun-03 10:23 nucliadb/common/locking.py
+-rw-r--r--  2.0 unx      835 b- defN 24-Jun-03 10:23 nucliadb/common/cluster/__init__.py
+-rw-r--r--  2.0 unx     5134 b- defN 24-Jun-03 10:23 nucliadb/common/cluster/base.py
+-rw-r--r--  2.0 unx     1495 b- defN 24-Jun-03 10:23 nucliadb/common/cluster/exceptions.py
+-rw-r--r--  2.0 unx     3793 b- defN 24-Jun-03 10:23 nucliadb/common/cluster/grpc_node_dummy.py
+-rw-r--r--  2.0 unx     3429 b- defN 24-Jun-03 10:23 nucliadb/common/cluster/index_node.py
+-rw-r--r--  2.0 unx    24804 b- defN 24-Jun-03 10:23 nucliadb/common/cluster/manager.py
+-rw-r--r--  2.0 unx     8831 b- defN 24-Jun-03 10:23 nucliadb/common/cluster/rebalance.py
+-rw-r--r--  2.0 unx    20532 b- defN 24-Jun-03 10:23 nucliadb/common/cluster/rollover.py
+-rw-r--r--  2.0 unx     3016 b- defN 24-Jun-03 10:23 nucliadb/common/cluster/settings.py
+-rw-r--r--  2.0 unx     5715 b- defN 24-Jun-03 10:23 nucliadb/common/cluster/utils.py
+-rw-r--r--  2.0 unx      835 b- defN 24-Jun-03 10:23 nucliadb/common/cluster/discovery/__init__.py
+-rw-r--r--  2.0 unx     6553 b- defN 24-Jun-03 10:23 nucliadb/common/cluster/discovery/base.py
+-rw-r--r--  2.0 unx    12512 b- defN 24-Jun-03 10:23 nucliadb/common/cluster/discovery/k8s.py
+-rw-r--r--  2.0 unx     1957 b- defN 24-Jun-03 10:23 nucliadb/common/cluster/discovery/manual.py
+-rw-r--r--  2.0 unx     1737 b- defN 24-Jun-03 10:23 nucliadb/common/cluster/discovery/single.py
+-rw-r--r--  2.0 unx     1139 b- defN 24-Jun-03 10:23 nucliadb/common/cluster/discovery/types.py
+-rw-r--r--  2.0 unx     2548 b- defN 24-Jun-03 10:23 nucliadb/common/cluster/discovery/utils.py
+-rw-r--r--  2.0 unx      833 b- defN 24-Jun-03 10:23 nucliadb/common/cluster/standalone/__init__.py
+-rw-r--r--  2.0 unx    13712 b- defN 24-Jun-03 10:23 nucliadb/common/cluster/standalone/grpc_node_binding.py
+-rw-r--r--  2.0 unx     4683 b- defN 24-Jun-03 10:23 nucliadb/common/cluster/standalone/index_node.py
+-rw-r--r--  2.0 unx     3444 b- defN 24-Jun-03 10:23 nucliadb/common/cluster/standalone/service.py
+-rw-r--r--  2.0 unx     3545 b- defN 24-Jun-03 10:23 nucliadb/common/cluster/standalone/utils.py
+-rw-r--r--  2.0 unx     3440 b- defN 24-Jun-03 10:23 nucliadb/common/context/__init__.py
+-rw-r--r--  2.0 unx     1628 b- defN 24-Jun-03 10:23 nucliadb/common/context/fastapi.py
+-rw-r--r--  2.0 unx     2062 b- defN 24-Jun-03 10:23 nucliadb/common/datamanagers/__init__.py
+-rw-r--r--  2.0 unx     3095 b- defN 24-Jun-03 10:23 nucliadb/common/datamanagers/atomic.py
+-rw-r--r--  2.0 unx     1451 b- defN 24-Jun-03 10:23 nucliadb/common/datamanagers/cluster.py
+-rw-r--r--  2.0 unx     5383 b- defN 24-Jun-03 10:23 nucliadb/common/datamanagers/entities.py
+-rw-r--r--  2.0 unx      883 b- defN 24-Jun-03 10:23 nucliadb/common/datamanagers/exceptions.py
+-rw-r--r--  2.0 unx     2764 b- defN 24-Jun-03 10:23 nucliadb/common/datamanagers/fields.py
+-rw-r--r--  2.0 unx     3994 b- defN 24-Jun-03 10:23 nucliadb/common/datamanagers/kb.py
+-rw-r--r--  2.0 unx     5389 b- defN 24-Jun-03 10:23 nucliadb/common/datamanagers/labels.py
+-rw-r--r--  2.0 unx     1599 b- defN 24-Jun-03 10:23 nucliadb/common/datamanagers/processing.py
+-rw-r--r--  2.0 unx    11931 b- defN 24-Jun-03 10:23 nucliadb/common/datamanagers/resources.py
+-rw-r--r--  2.0 unx     5643 b- defN 24-Jun-03 10:23 nucliadb/common/datamanagers/rollover.py
+-rw-r--r--  2.0 unx     1548 b- defN 24-Jun-03 10:23 nucliadb/common/datamanagers/synonyms.py
+-rw-r--r--  2.0 unx     1923 b- defN 24-Jun-03 10:23 nucliadb/common/datamanagers/utils.py
+-rw-r--r--  2.0 unx     3780 b- defN 24-Jun-03 10:23 nucliadb/common/datamanagers/vectorsets.py
+-rw-r--r--  2.0 unx      835 b- defN 24-Jun-03 10:23 nucliadb/common/http_clients/__init__.py
+-rw-r--r--  2.0 unx     2146 b- defN 24-Jun-03 10:23 nucliadb/common/http_clients/auth.py
+-rw-r--r--  2.0 unx     1100 b- defN 24-Jun-03 10:23 nucliadb/common/http_clients/exceptions.py
+-rw-r--r--  2.0 unx     7155 b- defN 24-Jun-03 10:23 nucliadb/common/http_clients/processing.py
+-rw-r--r--  2.0 unx     1540 b- defN 24-Jun-03 10:23 nucliadb/common/http_clients/pypi.py
+-rw-r--r--  2.0 unx     1551 b- defN 24-Jun-03 10:23 nucliadb/common/http_clients/utils.py
+-rw-r--r--  2.0 unx      835 b- defN 24-Jun-03 10:23 nucliadb/common/maindb/__init__.py
+-rw-r--r--  2.0 unx     3449 b- defN 24-Jun-03 10:23 nucliadb/common/maindb/driver.py
+-rw-r--r--  2.0 unx      988 b- defN 24-Jun-03 10:23 nucliadb/common/maindb/exceptions.py
+-rw-r--r--  2.0 unx     6769 b- defN 24-Jun-03 10:23 nucliadb/common/maindb/local.py
+-rw-r--r--  2.0 unx     8673 b- defN 24-Jun-03 10:23 nucliadb/common/maindb/pg.py
+-rw-r--r--  2.0 unx     6053 b- defN 24-Jun-03 10:23 nucliadb/common/maindb/redis.py
+-rw-r--r--  2.0 unx    15314 b- defN 24-Jun-03 10:23 nucliadb/common/maindb/tikv.py
+-rw-r--r--  2.0 unx     4167 b- defN 24-Jun-03 10:23 nucliadb/common/maindb/utils.py
+-rw-r--r--  2.0 unx      932 b- defN 24-Jun-03 10:23 nucliadb/export_import/__init__.py
+-rw-r--r--  2.0 unx     6185 b- defN 24-Jun-03 10:23 nucliadb/export_import/datamanager.py
+-rw-r--r--  2.0 unx     1949 b- defN 24-Jun-03 10:23 nucliadb/export_import/exceptions.py
+-rw-r--r--  2.0 unx     7116 b- defN 24-Jun-03 10:23 nucliadb/export_import/exporter.py
+-rw-r--r--  2.0 unx     4258 b- defN 24-Jun-03 10:23 nucliadb/export_import/importer.py
+-rw-r--r--  2.0 unx     2063 b- defN 24-Jun-03 10:23 nucliadb/export_import/models.py
+-rw-r--r--  2.0 unx     2571 b- defN 24-Jun-03 10:23 nucliadb/export_import/tasks.py
+-rw-r--r--  2.0 unx    19655 b- defN 24-Jun-03 10:23 nucliadb/export_import/utils.py
+-rw-r--r--  2.0 unx     1011 b- defN 24-Jun-03 10:23 nucliadb/ingest/__init__.py
+-rw-r--r--  2.0 unx     7277 b- defN 24-Jun-03 10:23 nucliadb/ingest/app.py
+-rw-r--r--  2.0 unx     1005 b- defN 24-Jun-03 10:23 nucliadb/ingest/cache.py
+-rw-r--r--  2.0 unx     2484 b- defN 24-Jun-03 10:23 nucliadb/ingest/partitions.py
+-rw-r--r--  2.0 unx    19904 b- defN 24-Jun-03 10:23 nucliadb/ingest/processing.py
+-rw-r--r--  2.0 unx        0 b- defN 24-Jun-03 10:23 nucliadb/ingest/py.typed
+-rw-r--r--  2.0 unx    20291 b- defN 24-Jun-03 10:23 nucliadb/ingest/serialize.py
+-rw-r--r--  2.0 unx     3207 b- defN 24-Jun-03 10:23 nucliadb/ingest/settings.py
+-rw-r--r--  2.0 unx     2314 b- defN 24-Jun-03 10:23 nucliadb/ingest/utils.py
+-rw-r--r--  2.0 unx      835 b- defN 24-Jun-03 10:23 nucliadb/ingest/consumer/__init__.py
+-rw-r--r--  2.0 unx     6918 b- defN 24-Jun-03 10:23 nucliadb/ingest/consumer/auditing.py
+-rw-r--r--  2.0 unx    12174 b- defN 24-Jun-03 10:23 nucliadb/ingest/consumer/consumer.py
+-rw-r--r--  2.0 unx     3934 b- defN 24-Jun-03 10:23 nucliadb/ingest/consumer/materializer.py
+-rw-r--r--  2.0 unx     1075 b- defN 24-Jun-03 10:23 nucliadb/ingest/consumer/metrics.py
+-rw-r--r--  2.0 unx     9546 b- defN 24-Jun-03 10:23 nucliadb/ingest/consumer/pull.py
+-rw-r--r--  2.0 unx     6871 b- defN 24-Jun-03 10:23 nucliadb/ingest/consumer/service.py
+-rw-r--r--  2.0 unx     4331 b- defN 24-Jun-03 10:23 nucliadb/ingest/consumer/shard_creator.py
+-rw-r--r--  2.0 unx     2656 b- defN 24-Jun-03 10:23 nucliadb/ingest/consumer/utils.py
+-rw-r--r--  2.0 unx      835 b- defN 24-Jun-03 10:23 nucliadb/ingest/fields/__init__.py
+-rw-r--r--  2.0 unx    17797 b- defN 24-Jun-03 10:23 nucliadb/ingest/fields/base.py
+-rw-r--r--  2.0 unx     7047 b- defN 24-Jun-03 10:23 nucliadb/ingest/fields/conversation.py
+-rw-r--r--  2.0 unx     1223 b- defN 24-Jun-03 10:23 nucliadb/ingest/fields/date.py
+-rw-r--r--  2.0 unx     1205 b- defN 24-Jun-03 10:23 nucliadb/ingest/fields/exceptions.py
+-rw-r--r--  2.0 unx     4840 b- defN 24-Jun-03 10:23 nucliadb/ingest/fields/file.py
+-rw-r--r--  2.0 unx     1547 b- defN 24-Jun-03 10:23 nucliadb/ingest/fields/generic.py
+-rw-r--r--  2.0 unx     1235 b- defN 24-Jun-03 10:23 nucliadb/ingest/fields/keywordset.py
+-rw-r--r--  2.0 unx     2250 b- defN 24-Jun-03 10:23 nucliadb/ingest/fields/layout.py
+-rw-r--r--  2.0 unx     4212 b- defN 24-Jun-03 10:23 nucliadb/ingest/fields/link.py
+-rw-r--r--  2.0 unx     1319 b- defN 24-Jun-03 10:23 nucliadb/ingest/fields/text.py
+-rw-r--r--  2.0 unx      835 b- defN 24-Jun-03 10:23 nucliadb/ingest/orm/__init__.py
+-rw-r--r--  2.0 unx    28721 b- defN 24-Jun-03 10:23 nucliadb/ingest/orm/brain.py
+-rw-r--r--  2.0 unx     6954 b- defN 24-Jun-03 10:23 nucliadb/ingest/orm/broker_message.py
+-rw-r--r--  2.0 unx    15758 b- defN 24-Jun-03 10:23 nucliadb/ingest/orm/entities.py
+-rw-r--r--  2.0 unx     1326 b- defN 24-Jun-03 10:23 nucliadb/ingest/orm/exceptions.py
+-rw-r--r--  2.0 unx    16068 b- defN 24-Jun-03 10:23 nucliadb/ingest/orm/knowledgebox.py
+-rw-r--r--  2.0 unx     1096 b- defN 24-Jun-03 10:23 nucliadb/ingest/orm/metrics.py
+-rw-r--r--  2.0 unx    54798 b- defN 24-Jun-03 10:23 nucliadb/ingest/orm/resource.py
+-rw-r--r--  2.0 unx     2685 b- defN 24-Jun-03 10:23 nucliadb/ingest/orm/utils.py
+-rw-r--r--  2.0 unx    27092 b- defN 24-Jun-03 10:23 nucliadb/ingest/orm/processor/__init__.py
+-rw-r--r--  2.0 unx     5104 b- defN 24-Jun-03 10:23 nucliadb/ingest/orm/processor/auditing.py
+-rw-r--r--  2.0 unx     1704 b- defN 24-Jun-03 10:23 nucliadb/ingest/orm/processor/sequence_manager.py
+-rw-r--r--  2.0 unx     2057 b- defN 24-Jun-03 10:23 nucliadb/ingest/service/__init__.py
+-rw-r--r--  2.0 unx      835 b- defN 24-Jun-03 10:23 nucliadb/ingest/service/exceptions.py
+-rw-r--r--  2.0 unx    29886 b- defN 24-Jun-03 10:23 nucliadb/ingest/service/writer.py
+-rw-r--r--  2.0 unx      835 b- defN 24-Jun-03 10:23 nucliadb/ingest/tests/__init__.py
+-rw-r--r--  2.0 unx     1157 b- defN 24-Jun-03 10:23 nucliadb/ingest/tests/conftest.py
+-rw-r--r--  2.0 unx    24111 b- defN 24-Jun-03 10:23 nucliadb/ingest/tests/fixtures.py
+-rw-r--r--  2.0 unx    62843 b- defN 24-Jun-03 10:23 nucliadb/ingest/tests/vectors.py
+-rw-r--r--  2.0 unx      835 b- defN 24-Jun-03 10:23 nucliadb/ingest/tests/integration/__init__.py
+-rw-r--r--  2.0 unx      833 b- defN 24-Jun-03 10:23 nucliadb/ingest/tests/integration/consumer/__init__.py
+-rw-r--r--  2.0 unx     2500 b- defN 24-Jun-03 10:23 nucliadb/ingest/tests/integration/consumer/test_auditing.py
+-rw-r--r--  2.0 unx     3836 b- defN 24-Jun-03 10:23 nucliadb/ingest/tests/integration/consumer/test_materializer.py
+-rw-r--r--  2.0 unx     4470 b- defN 24-Jun-03 10:23 nucliadb/ingest/tests/integration/consumer/test_pull.py
+-rw-r--r--  2.0 unx     2763 b- defN 24-Jun-03 10:23 nucliadb/ingest/tests/integration/consumer/test_service.py
+-rw-r--r--  2.0 unx     2019 b- defN 24-Jun-03 10:23 nucliadb/ingest/tests/integration/consumer/test_shard_creator.py
+-rw-r--r--  2.0 unx      835 b- defN 24-Jun-03 10:23 nucliadb/ingest/tests/integration/ingest/__init__.py
+-rw-r--r--  2.0 unx    27247 b- defN 24-Jun-03 10:23 nucliadb/ingest/tests/integration/ingest/test_ingest.py
+-rw-r--r--  2.0 unx     3040 b- defN 24-Jun-03 10:23 nucliadb/ingest/tests/integration/ingest/test_processing_engine.py
+-rw-r--r--  2.0 unx     8586 b- defN 24-Jun-03 10:23 nucliadb/ingest/tests/integration/ingest/test_relations.py
+-rw-r--r--  2.0 unx     5637 b- defN 24-Jun-03 10:23 nucliadb/ingest/tests/integration/ingest/test_vectorsets.py
+-rw-r--r--  2.0 unx      835 b- defN 24-Jun-03 10:23 nucliadb/ingest/tests/unit/__init__.py
+-rw-r--r--  2.0 unx     1189 b- defN 24-Jun-03 10:23 nucliadb/ingest/tests/unit/test_cache.py
+-rw-r--r--  2.0 unx     1432 b- defN 24-Jun-03 10:23 nucliadb/ingest/tests/unit/test_partitions.py
+-rw-r--r--  2.0 unx     5807 b- defN 24-Jun-03 10:23 nucliadb/ingest/tests/unit/test_processing.py
+-rw-r--r--  2.0 unx      978 b- defN 24-Jun-03 10:23 nucliadb/ingest/tests/unit/test_settings.py
+-rw-r--r--  2.0 unx      833 b- defN 24-Jun-03 10:23 nucliadb/ingest/tests/unit/consumer/__init__.py
+-rw-r--r--  2.0 unx     3885 b- defN 24-Jun-03 10:23 nucliadb/ingest/tests/unit/consumer/test_auditing.py
+-rw-r--r--  2.0 unx     2472 b- defN 24-Jun-03 10:23 nucliadb/ingest/tests/unit/consumer/test_consumer.py
+-rw-r--r--  2.0 unx     2063 b- defN 24-Jun-03 10:23 nucliadb/ingest/tests/unit/consumer/test_pull.py
+-rw-r--r--  2.0 unx     4140 b- defN 24-Jun-03 10:23 nucliadb/ingest/tests/unit/consumer/test_shard_creator.py
+-rw-r--r--  2.0 unx     1934 b- defN 24-Jun-03 10:23 nucliadb/ingest/tests/unit/consumer/test_utils.py
+-rw-r--r--  2.0 unx      835 b- defN 24-Jun-03 10:23 nucliadb/ingest/tests/unit/orm/__init__.py
+-rw-r--r--  2.0 unx     9876 b- defN 24-Jun-03 10:23 nucliadb/ingest/tests/unit/orm/test_brain.py
+-rw-r--r--  2.0 unx     2572 b- defN 24-Jun-03 10:23 nucliadb/ingest/tests/unit/orm/test_brain_vectors.py
+-rw-r--r--  2.0 unx     1174 b- defN 24-Jun-03 10:23 nucliadb/ingest/tests/unit/orm/test_orm_utils.py
+-rw-r--r--  2.0 unx     4045 b- defN 24-Jun-03 10:23 nucliadb/ingest/tests/unit/orm/test_processor.py
+-rw-r--r--  2.0 unx    11033 b- defN 24-Jun-03 10:23 nucliadb/ingest/tests/unit/orm/test_resource.py
+-rw-r--r--  2.0 unx     2216 b- defN 24-Jun-03 10:23 nucliadb/middleware/__init__.py
+-rw-r--r--  2.0 unx     3912 b- defN 24-Jun-03 10:23 nucliadb/middleware/transaction.py
+-rw-r--r--  2.0 unx      835 b- defN 24-Jun-03 10:23 nucliadb/migrator/__init__.py
+-rw-r--r--  2.0 unx     2119 b- defN 24-Jun-03 10:23 nucliadb/migrator/command.py
+-rw-r--r--  2.0 unx     1334 b- defN 24-Jun-03 10:23 nucliadb/migrator/context.py
+-rw-r--r--  2.0 unx     5104 b- defN 24-Jun-03 10:23 nucliadb/migrator/datamanager.py
+-rw-r--r--  2.0 unx      889 b- defN 24-Jun-03 10:23 nucliadb/migrator/exceptions.py
+-rw-r--r--  2.0 unx     9370 b- defN 24-Jun-03 10:23 nucliadb/migrator/migrator.py
+-rw-r--r--  2.0 unx     1145 b- defN 24-Jun-03 10:23 nucliadb/migrator/models.py
+-rw-r--r--  2.0 unx     1144 b- defN 24-Jun-03 10:23 nucliadb/migrator/settings.py
+-rw-r--r--  2.0 unx     2346 b- defN 24-Jun-03 10:23 nucliadb/migrator/utils.py
+-rw-r--r--  2.0 unx      835 b- defN 24-Jun-03 10:23 nucliadb/models/__init__.py
+-rw-r--r--  2.0 unx     1599 b- defN 24-Jun-03 10:23 nucliadb/models/responses.py
+-rw-r--r--  2.0 unx     6041 b- defN 24-Jun-03 10:23 nucliadb/purge/__init__.py
+-rw-r--r--  2.0 unx     9367 b- defN 24-Jun-03 10:23 nucliadb/purge/orphan_shards.py
+-rw-r--r--  2.0 unx     1328 b- defN 24-Jun-03 10:23 nucliadb/reader/__init__.py
+-rw-r--r--  2.0 unx     3709 b- defN 24-Jun-03 10:23 nucliadb/reader/app.py
+-rw-r--r--  2.0 unx     1366 b- defN 24-Jun-03 10:23 nucliadb/reader/lifecycle.py
+-rw-r--r--  2.0 unx     1031 b- defN 24-Jun-03 10:23 nucliadb/reader/openapi.py
+-rw-r--r--  2.0 unx        0 b- defN 24-Jun-03 10:23 nucliadb/reader/py.typed
+-rw-r--r--  2.0 unx     1447 b- defN 24-Jun-03 10:23 nucliadb/reader/run.py
+-rw-r--r--  2.0 unx      872 b- defN 24-Jun-03 10:23 nucliadb/reader/api/__init__.py
+-rw-r--r--  2.0 unx     2458 b- defN 24-Jun-03 10:23 nucliadb/reader/api/models.py
+-rw-r--r--  2.0 unx     1110 b- defN 24-Jun-03 10:23 nucliadb/reader/api/v1/__init__.py
+-rw-r--r--  2.0 unx    12457 b- defN 24-Jun-03 10:23 nucliadb/reader/api/v1/download.py
+-rw-r--r--  2.0 unx     6448 b- defN 24-Jun-03 10:23 nucliadb/reader/api/v1/export_import.py
+-rw-r--r--  2.0 unx     3641 b- defN 24-Jun-03 10:23 nucliadb/reader/api/v1/knowledgebox.py
+-rw-r--r--  2.0 unx     2099 b- defN 24-Jun-03 10:23 nucliadb/reader/api/v1/learning_collector.py
+-rw-r--r--  2.0 unx     4472 b- defN 24-Jun-03 10:23 nucliadb/reader/api/v1/learning_config.py
+-rw-r--r--  2.0 unx    13961 b- defN 24-Jun-03 10:23 nucliadb/reader/api/v1/resource.py
+-rw-r--r--  2.0 unx     1011 b- defN 24-Jun-03 10:23 nucliadb/reader/api/v1/router.py
+-rw-r--r--  2.0 unx    11902 b- defN 24-Jun-03 10:23 nucliadb/reader/api/v1/services.py
+-rw-r--r--  2.0 unx      835 b- defN 24-Jun-03 10:23 nucliadb/reader/reader/__init__.py
+-rw-r--r--  2.0 unx     7979 b- defN 24-Jun-03 10:23 nucliadb/reader/reader/notifications.py
+-rw-r--r--  2.0 unx      835 b- defN 24-Jun-03 10:23 nucliadb/reader/tests/__init__.py
+-rw-r--r--  2.0 unx     1224 b- defN 24-Jun-03 10:23 nucliadb/reader/tests/conftest.py
+-rw-r--r--  2.0 unx     4355 b- defN 24-Jun-03 10:23 nucliadb/reader/tests/fixtures.py
+-rw-r--r--  2.0 unx     2748 b- defN 24-Jun-03 10:23 nucliadb/reader/tests/test_list_resources.py
+-rw-r--r--  2.0 unx    10199 b- defN 24-Jun-03 10:23 nucliadb/reader/tests/test_reader_file_download.py
+-rw-r--r--  2.0 unx    10586 b- defN 24-Jun-03 10:23 nucliadb/reader/tests/test_reader_resource.py
+-rw-r--r--  2.0 unx     6535 b- defN 24-Jun-03 10:23 nucliadb/reader/tests/test_reader_resource_field.py
+-rw-r--r--  2.0 unx     1535 b- defN 24-Jun-03 10:23 nucliadb/search/__init__.py
+-rw-r--r--  2.0 unx     4905 b- defN 24-Jun-03 10:23 nucliadb/search/app.py
+-rw-r--r--  2.0 unx     1956 b- defN 24-Jun-03 10:23 nucliadb/search/lifecycle.py
+-rw-r--r--  2.0 unx     1016 b- defN 24-Jun-03 10:23 nucliadb/search/openapi.py
+-rw-r--r--  2.0 unx    20665 b- defN 24-Jun-03 10:23 nucliadb/search/predict.py
+-rw-r--r--  2.0 unx        0 b- defN 24-Jun-03 10:23 nucliadb/search/py.typed
+-rw-r--r--  2.0 unx     1402 b- defN 24-Jun-03 10:23 nucliadb/search/run.py
+-rw-r--r--  2.0 unx     1193 b- defN 24-Jun-03 10:23 nucliadb/search/settings.py
+-rw-r--r--  2.0 unx     1037 b- defN 24-Jun-03 10:23 nucliadb/search/utilities.py
+-rw-r--r--  2.0 unx      835 b- defN 24-Jun-03 10:23 nucliadb/search/api/__init__.py
+-rw-r--r--  2.0 unx     1298 b- defN 24-Jun-03 10:23 nucliadb/search/api/v1/__init__.py
+-rw-r--r--  2.0 unx     3435 b- defN 24-Jun-03 10:23 nucliadb/search/api/v1/ask.py
+-rw-r--r--  2.0 unx     9514 b- defN 24-Jun-03 10:23 nucliadb/search/api/v1/chat.py
+-rw-r--r--  2.0 unx     2668 b- defN 24-Jun-03 10:23 nucliadb/search/api/v1/feedback.py
+-rw-r--r--  2.0 unx     8795 b- defN 24-Jun-03 10:23 nucliadb/search/api/v1/find.py
+-rw-r--r--  2.0 unx     6941 b- defN 24-Jun-03 10:23 nucliadb/search/api/v1/knowledgebox.py
+-rw-r--r--  2.0 unx     3047 b- defN 24-Jun-03 10:23 nucliadb/search/api/v1/predict_proxy.py
+-rw-r--r--  2.0 unx      988 b- defN 24-Jun-03 10:23 nucliadb/search/api/v1/router.py
+-rw-r--r--  2.0 unx    19262 b- defN 24-Jun-03 10:23 nucliadb/search/api/v1/search.py
+-rw-r--r--  2.0 unx     5970 b- defN 24-Jun-03 10:23 nucliadb/search/api/v1/suggest.py
+-rw-r--r--  2.0 unx     2499 b- defN 24-Jun-03 10:23 nucliadb/search/api/v1/summarize.py
+-rw-r--r--  2.0 unx     1434 b- defN 24-Jun-03 10:23 nucliadb/search/api/v1/utils.py
+-rw-r--r--  2.0 unx      835 b- defN 24-Jun-03 10:23 nucliadb/search/api/v1/resource/__init__.py
+-rw-r--r--  2.0 unx     3869 b- defN 24-Jun-03 10:23 nucliadb/search/api/v1/resource/ask.py
+-rw-r--r--  2.0 unx     5866 b- defN 24-Jun-03 10:23 nucliadb/search/api/v1/resource/chat.py
+-rw-r--r--  2.0 unx     5303 b- defN 24-Jun-03 10:23 nucliadb/search/api/v1/resource/search.py
+-rw-r--r--  2.0 unx      833 b- defN 24-Jun-03 10:23 nucliadb/search/requesters/__init__.py
+-rw-r--r--  2.0 unx     9111 b- defN 24-Jun-03 10:23 nucliadb/search/requesters/utils.py
+-rw-r--r--  2.0 unx      835 b- defN 24-Jun-03 10:23 nucliadb/search/search/__init__.py
+-rw-r--r--  2.0 unx     2746 b- defN 24-Jun-03 10:23 nucliadb/search/search/cache.py
+-rw-r--r--  2.0 unx     1154 b- defN 24-Jun-03 10:23 nucliadb/search/search/exceptions.py
+-rw-r--r--  2.0 unx     5465 b- defN 24-Jun-03 10:23 nucliadb/search/search/fetch.py
+-rw-r--r--  2.0 unx     6513 b- defN 24-Jun-03 10:23 nucliadb/search/search/filters.py
+-rw-r--r--  2.0 unx     4612 b- defN 24-Jun-03 10:23 nucliadb/search/search/find.py
+-rw-r--r--  2.0 unx    17152 b- defN 24-Jun-03 10:23 nucliadb/search/search/find_merge.py
+-rw-r--r--  2.0 unx    21282 b- defN 24-Jun-03 10:23 nucliadb/search/search/merge.py
+-rw-r--r--  2.0 unx     1130 b- defN 24-Jun-03 10:23 nucliadb/search/search/metrics.py
+-rw-r--r--  2.0 unx     8698 b- defN 24-Jun-03 10:23 nucliadb/search/search/paragraphs.py
+-rw-r--r--  2.0 unx     3015 b- defN 24-Jun-03 10:23 nucliadb/search/search/predict_proxy.py
+-rw-r--r--  2.0 unx    31093 b- defN 24-Jun-03 10:23 nucliadb/search/search/query.py
+-rw-r--r--  2.0 unx     3018 b- defN 24-Jun-03 10:23 nucliadb/search/search/shards.py
+-rw-r--r--  2.0 unx     5101 b- defN 24-Jun-03 10:23 nucliadb/search/search/summarize.py
+-rw-r--r--  2.0 unx     2438 b- defN 24-Jun-03 10:23 nucliadb/search/search/utils.py
+-rw-r--r--  2.0 unx      835 b- defN 24-Jun-03 10:23 nucliadb/search/search/chat/__init__.py
+-rw-r--r--  2.0 unx    16676 b- defN 24-Jun-03 10:23 nucliadb/search/search/chat/ask.py
+-rw-r--r--  2.0 unx     2058 b- defN 24-Jun-03 10:23 nucliadb/search/search/chat/images.py
+-rw-r--r--  2.0 unx    20793 b- defN 24-Jun-03 10:23 nucliadb/search/search/chat/prompt.py
+-rw-r--r--  2.0 unx    17543 b- defN 24-Jun-03 10:23 nucliadb/search/search/chat/query.py
+-rw-r--r--  2.0 unx      835 b- defN 24-Jun-03 10:23 nucliadb/search/tests/__init__.py
+-rw-r--r--  2.0 unx     1295 b- defN 24-Jun-03 10:23 nucliadb/search/tests/conftest.py
+-rw-r--r--  2.0 unx     6578 b- defN 24-Jun-03 10:23 nucliadb/search/tests/fixtures.py
+-rw-r--r--  2.0 unx    15480 b- defN 24-Jun-03 10:23 nucliadb/search/tests/node.py
+-rw-r--r--  2.0 unx      833 b- defN 24-Jun-03 10:23 nucliadb/search/tests/unit/__init__.py
+-rw-r--r--  2.0 unx     2649 b- defN 24-Jun-03 10:23 nucliadb/search/tests/unit/test_app.py
+-rw-r--r--  2.0 unx     3374 b- defN 24-Jun-03 10:23 nucliadb/search/tests/unit/test_find_merge.py
+-rw-r--r--  2.0 unx     1400 b- defN 24-Jun-03 10:23 nucliadb/search/tests/unit/test_merge.py
+-rw-r--r--  2.0 unx    15721 b- defN 24-Jun-03 10:23 nucliadb/search/tests/unit/test_predict.py
+-rw-r--r--  2.0 unx     1328 b- defN 24-Jun-03 10:23 nucliadb/search/tests/unit/test_run.py
+-rw-r--r--  2.0 unx      835 b- defN 24-Jun-03 10:23 nucliadb/search/tests/unit/api/__init__.py
+-rw-r--r--  2.0 unx      835 b- defN 24-Jun-03 10:23 nucliadb/search/tests/unit/api/v1/__init__.py
+-rw-r--r--  2.0 unx     3759 b- defN 24-Jun-03 10:23 nucliadb/search/tests/unit/api/v1/test_ask.py
+-rw-r--r--  2.0 unx     2966 b- defN 24-Jun-03 10:23 nucliadb/search/tests/unit/api/v1/test_chat.py
+-rw-r--r--  2.0 unx     2865 b- defN 24-Jun-03 10:23 nucliadb/search/tests/unit/api/v1/test_predict_proxy.py
+-rw-r--r--  2.0 unx     2901 b- defN 24-Jun-03 10:23 nucliadb/search/tests/unit/api/v1/test_summarize.py
+-rw-r--r--  2.0 unx      835 b- defN 24-Jun-03 10:23 nucliadb/search/tests/unit/api/v1/resource/__init__.py
+-rw-r--r--  2.0 unx     3040 b- defN 24-Jun-03 10:23 nucliadb/search/tests/unit/api/v1/resource/test_chat.py
+-rw-r--r--  2.0 unx      833 b- defN 24-Jun-03 10:23 nucliadb/search/tests/unit/search/__init__.py
+-rw-r--r--  2.0 unx     8586 b- defN 24-Jun-03 10:23 nucliadb/search/tests/unit/search/test_chat_prompt.py
+-rw-r--r--  2.0 unx     3736 b- defN 24-Jun-03 10:23 nucliadb/search/tests/unit/search/test_fetch.py
+-rw-r--r--  2.0 unx     4306 b- defN 24-Jun-03 10:23 nucliadb/search/tests/unit/search/test_filters.py
+-rw-r--r--  2.0 unx     4492 b- defN 24-Jun-03 10:23 nucliadb/search/tests/unit/search/test_paragraphs.py
+-rw-r--r--  2.0 unx     3496 b- defN 24-Jun-03 10:23 nucliadb/search/tests/unit/search/test_predict_proxy.py
+-rw-r--r--  2.0 unx     5121 b- defN 24-Jun-03 10:23 nucliadb/search/tests/unit/search/test_query.py
+-rw-r--r--  2.0 unx      833 b- defN 24-Jun-03 10:23 nucliadb/search/tests/unit/search/requesters/__init__.py
+-rw-r--r--  2.0 unx     6455 b- defN 24-Jun-03 10:23 nucliadb/search/tests/unit/search/requesters/test_utils.py
+-rw-r--r--  2.0 unx      835 b- defN 24-Jun-03 10:23 nucliadb/search/tests/unit/search/search/__init__.py
+-rw-r--r--  2.0 unx     1759 b- defN 24-Jun-03 10:23 nucliadb/search/tests/unit/search/search/test_shards.py
+-rw-r--r--  2.0 unx     2511 b- defN 24-Jun-03 10:23 nucliadb/search/tests/unit/search/search/test_utils.py
+-rw-r--r--  2.0 unx      835 b- defN 24-Jun-03 10:23 nucliadb/standalone/__init__.py
+-rw-r--r--  2.0 unx     6749 b- defN 24-Jun-03 10:23 nucliadb/standalone/api_router.py
+-rw-r--r--  2.0 unx     5763 b- defN 24-Jun-03 10:23 nucliadb/standalone/app.py
+-rw-r--r--  2.0 unx     7800 b- defN 24-Jun-03 10:23 nucliadb/standalone/auth.py
+-rw-r--r--  2.0 unx     5313 b- defN 24-Jun-03 10:23 nucliadb/standalone/config.py
+-rw-r--r--  2.0 unx     6986 b- defN 24-Jun-03 10:23 nucliadb/standalone/introspect.py
+-rw-r--r--  2.0 unx     2488 b- defN 24-Jun-03 10:23 nucliadb/standalone/lifecycle.py
+-rw-r--r--  2.0 unx     1980 b- defN 24-Jun-03 10:23 nucliadb/standalone/migrations.py
+-rw-r--r--  2.0 unx     1322 b- defN 24-Jun-03 10:23 nucliadb/standalone/purge.py
+-rw-r--r--  2.0 unx        0 b- defN 24-Jun-03 10:23 nucliadb/standalone/py.typed
+-rw-r--r--  2.0 unx     5636 b- defN 24-Jun-03 10:23 nucliadb/standalone/run.py
+-rw-r--r--  2.0 unx     5822 b- defN 24-Jun-03 10:23 nucliadb/standalone/settings.py
+-rw-r--r--  2.0 unx     3132 b- defN 24-Jun-03 10:23 nucliadb/standalone/versions.py
+-rw-r--r--  2.0 unx     2285 b- defN 24-Jun-03 10:23 nucliadb/standalone/static/favicon.ico
+-rw-r--r--  2.0 unx     3833 b- defN 24-Jun-03 10:23 nucliadb/standalone/static/index.html
+-rw-r--r--  2.0 unx     2639 b- defN 24-Jun-03 10:23 nucliadb/standalone/static/logo.svg
+-rw-r--r--  2.0 unx      835 b- defN 24-Jun-03 10:23 nucliadb/standalone/tests/__init__.py
+-rw-r--r--  2.0 unx     1294 b- defN 24-Jun-03 10:23 nucliadb/standalone/tests/conftest.py
+-rw-r--r--  2.0 unx     1319 b- defN 24-Jun-03 10:23 nucliadb/standalone/tests/fixtures.py
+-rw-r--r--  2.0 unx      833 b- defN 24-Jun-03 10:23 nucliadb/standalone/tests/unit/__init__.py
+-rw-r--r--  2.0 unx     1722 b- defN 24-Jun-03 10:23 nucliadb/standalone/tests/unit/test_api_router.py
+-rw-r--r--  2.0 unx     5509 b- defN 24-Jun-03 10:23 nucliadb/standalone/tests/unit/test_auth.py
+-rw-r--r--  2.0 unx     1334 b- defN 24-Jun-03 10:23 nucliadb/standalone/tests/unit/test_introspect.py
+-rw-r--r--  2.0 unx     1863 b- defN 24-Jun-03 10:23 nucliadb/standalone/tests/unit/test_migrations.py
+-rw-r--r--  2.0 unx     1546 b- defN 24-Jun-03 10:23 nucliadb/standalone/tests/unit/test_run.py
+-rw-r--r--  2.0 unx     1972 b- defN 24-Jun-03 10:23 nucliadb/standalone/tests/unit/test_versions.py
+-rw-r--r--  2.0 unx     1037 b- defN 24-Jun-03 10:23 nucliadb/tasks/__init__.py
+-rw-r--r--  2.0 unx     7655 b- defN 24-Jun-03 10:23 nucliadb/tasks/consumer.py
+-rw-r--r--  2.0 unx      924 b- defN 24-Jun-03 10:23 nucliadb/tasks/logger.py
+-rw-r--r--  2.0 unx     1378 b- defN 24-Jun-03 10:23 nucliadb/tasks/models.py
+-rw-r--r--  2.0 unx     3457 b- defN 24-Jun-03 10:23 nucliadb/tasks/producer.py
+-rw-r--r--  2.0 unx     1753 b- defN 24-Jun-03 10:23 nucliadb/tasks/registry.py
+-rw-r--r--  2.0 unx     1360 b- defN 24-Jun-03 10:23 nucliadb/tasks/utils.py
+-rw-r--r--  2.0 unx      835 b- defN 24-Jun-03 10:23 nucliadb/tests/__init__.py
+-rw-r--r--  2.0 unx     1229 b- defN 24-Jun-03 10:23 nucliadb/tests/conftest.py
+-rw-r--r--  2.0 unx    22365 b- defN 24-Jun-03 10:23 nucliadb/tests/fixtures.py
+-rw-r--r--  2.0 unx     7549 b- defN 24-Jun-03 10:23 nucliadb/tests/tikv.py
+-rw-r--r--  2.0 unx      835 b- defN 24-Jun-03 10:23 nucliadb/tests/benchmarks/__init__.py
+-rw-r--r--  2.0 unx     3032 b- defN 24-Jun-03 10:23 nucliadb/tests/benchmarks/test_search.py
+-rw-r--r--  2.0 unx      919 b- defN 24-Jun-03 10:23 nucliadb/tests/knowledgeboxes/__init__.py
+-rw-r--r--  2.0 unx     7002 b- defN 24-Jun-03 10:23 nucliadb/tests/knowledgeboxes/philosophy_books.py
+-rw-r--r--  2.0 unx     3037 b- defN 24-Jun-03 10:23 nucliadb/tests/knowledgeboxes/ten_dummy_resources.py
+-rw-r--r--  2.0 unx     1148 b- defN 24-Jun-03 10:23 nucliadb/tests/migrations/__init__.py
+-rw-r--r--  2.0 unx     2726 b- defN 24-Jun-03 10:23 nucliadb/tests/migrations/test_migration_0017.py
+-rw-r--r--  2.0 unx     3662 b- defN 24-Jun-03 10:23 nucliadb/tests/migrations/test_migration_0018.py
+-rw-r--r--  2.0 unx     3439 b- defN 24-Jun-03 10:23 nucliadb/tests/migrations/test_migration_0021.py
+-rw-r--r--  2.0 unx      835 b- defN 24-Jun-03 10:23 nucliadb/tests/unit/__init__.py
+-rw-r--r--  2.0 unx     1487 b- defN 24-Jun-03 10:23 nucliadb/tests/unit/test_field_ids.py
+-rw-r--r--  2.0 unx     2780 b- defN 24-Jun-03 10:23 nucliadb/tests/unit/test_health.py
+-rw-r--r--  2.0 unx     1543 b- defN 24-Jun-03 10:23 nucliadb/tests/unit/test_kb_slugs.py
+-rw-r--r--  2.0 unx     7892 b- defN 24-Jun-03 10:23 nucliadb/tests/unit/test_learning_proxy.py
+-rw-r--r--  2.0 unx     2642 b- defN 24-Jun-03 10:23 nucliadb/tests/unit/test_metrics_exporter.py
+-rw-r--r--  2.0 unx     1341 b- defN 24-Jun-03 10:23 nucliadb/tests/unit/test_openapi.py
+-rw-r--r--  2.0 unx     3649 b- defN 24-Jun-03 10:23 nucliadb/tests/unit/test_purge.py
+-rw-r--r--  2.0 unx      835 b- defN 24-Jun-03 10:23 nucliadb/tests/unit/common/__init__.py
+-rw-r--r--  2.0 unx     1268 b- defN 24-Jun-03 10:23 nucliadb/tests/unit/common/test_context.py
+-rw-r--r--  2.0 unx      835 b- defN 24-Jun-03 10:23 nucliadb/tests/unit/common/cluster/__init__.py
+-rw-r--r--  2.0 unx    12240 b- defN 24-Jun-03 10:23 nucliadb/tests/unit/common/cluster/test_cluster.py
+-rw-r--r--  2.0 unx     5387 b- defN 24-Jun-03 10:23 nucliadb/tests/unit/common/cluster/test_kb_shard_manager.py
+-rw-r--r--  2.0 unx     1428 b- defN 24-Jun-03 10:23 nucliadb/tests/unit/common/cluster/test_rebalance.py
+-rw-r--r--  2.0 unx     9609 b- defN 24-Jun-03 10:23 nucliadb/tests/unit/common/cluster/test_rollover.py
+-rw-r--r--  2.0 unx      835 b- defN 24-Jun-03 10:23 nucliadb/tests/unit/common/cluster/discovery/__init__.py
+-rw-r--r--  2.0 unx     5627 b- defN 24-Jun-03 10:23 nucliadb/tests/unit/common/cluster/discovery/test_k8s.py
+-rw-r--r--  2.0 unx      833 b- defN 24-Jun-03 10:23 nucliadb/tests/unit/common/cluster/standalone/__init__.py
+-rw-r--r--  2.0 unx     3761 b- defN 24-Jun-03 10:23 nucliadb/tests/unit/common/cluster/standalone/test_service.py
+-rw-r--r--  2.0 unx     2136 b- defN 24-Jun-03 10:23 nucliadb/tests/unit/common/cluster/standalone/test_utils.py
+-rw-r--r--  2.0 unx      833 b- defN 24-Jun-03 10:23 nucliadb/tests/unit/common/maindb/__init__.py
+-rw-r--r--  2.0 unx     3579 b- defN 24-Jun-03 10:23 nucliadb/tests/unit/common/maindb/test_driver.py
+-rw-r--r--  2.0 unx     2119 b- defN 24-Jun-03 10:23 nucliadb/tests/unit/common/maindb/test_tikv.py
+-rw-r--r--  2.0 unx     3213 b- defN 24-Jun-03 10:23 nucliadb/tests/unit/common/maindb/test_utils.py
+-rw-r--r--  2.0 unx      835 b- defN 24-Jun-03 10:23 nucliadb/tests/unit/export_import/__init__.py
+-rw-r--r--  2.0 unx     1435 b- defN 24-Jun-03 10:23 nucliadb/tests/unit/export_import/test_datamanager.py
+-rw-r--r--  2.0 unx     9706 b- defN 24-Jun-03 10:23 nucliadb/tests/unit/export_import/test_utils.py
+-rw-r--r--  2.0 unx      835 b- defN 24-Jun-03 10:23 nucliadb/tests/unit/migrator/__init__.py
+-rw-r--r--  2.0 unx     3233 b- defN 24-Jun-03 10:23 nucliadb/tests/unit/migrator/test_migrator.py
+-rw-r--r--  2.0 unx      835 b- defN 24-Jun-03 10:23 nucliadb/tests/unit/tasks/__init__.py
+-rw-r--r--  2.0 unx     1375 b- defN 24-Jun-03 10:23 nucliadb/tests/unit/tasks/conftest.py
+-rw-r--r--  2.0 unx     2714 b- defN 24-Jun-03 10:23 nucliadb/tests/unit/tasks/test_consumer.py
+-rw-r--r--  2.0 unx     3189 b- defN 24-Jun-03 10:23 nucliadb/tests/unit/tasks/test_producer.py
+-rw-r--r--  2.0 unx     1827 b- defN 24-Jun-03 10:23 nucliadb/tests/unit/tasks/test_tasks.py
+-rw-r--r--  2.0 unx     2507 b- defN 24-Jun-03 10:23 nucliadb/tests/utils/__init__.py
+-rw-r--r--  2.0 unx     1797 b- defN 24-Jun-03 10:23 nucliadb/tests/utils/aiohttp_session.py
+-rw-r--r--  2.0 unx     2533 b- defN 24-Jun-03 10:23 nucliadb/tests/utils/entities.py
+-rw-r--r--  2.0 unx     6327 b- defN 24-Jun-03 10:23 nucliadb/tests/utils/broker_messages/__init__.py
+-rw-r--r--  2.0 unx     7557 b- defN 24-Jun-03 10:23 nucliadb/tests/utils/broker_messages/fields.py
+-rw-r--r--  2.0 unx     1196 b- defN 24-Jun-03 10:23 nucliadb/tests/utils/broker_messages/helpers.py
+-rw-r--r--  2.0 unx     1325 b- defN 24-Jun-03 10:23 nucliadb/train/__init__.py
+-rw-r--r--  2.0 unx     3530 b- defN 24-Jun-03 10:23 nucliadb/train/app.py
+-rw-r--r--  2.0 unx     3800 b- defN 24-Jun-03 10:23 nucliadb/train/generator.py
+-rw-r--r--  2.0 unx     1698 b- defN 24-Jun-03 10:23 nucliadb/train/lifecycle.py
+-rw-r--r--  2.0 unx     1198 b- defN 24-Jun-03 10:23 nucliadb/train/models.py
+-rw-r--r--  2.0 unx     5776 b- defN 24-Jun-03 10:23 nucliadb/train/nodes.py
+-rw-r--r--  2.0 unx        0 b- defN 24-Jun-03 10:23 nucliadb/train/py.typed
+-rw-r--r--  2.0 unx     1400 b- defN 24-Jun-03 10:23 nucliadb/train/run.py
+-rw-r--r--  2.0 unx     5750 b- defN 24-Jun-03 10:23 nucliadb/train/servicer.py
+-rw-r--r--  2.0 unx     1415 b- defN 24-Jun-03 10:23 nucliadb/train/settings.py
+-rw-r--r--  2.0 unx     1496 b- defN 24-Jun-03 10:23 nucliadb/train/types.py
+-rw-r--r--  2.0 unx     3265 b- defN 24-Jun-03 10:23 nucliadb/train/upload.py
+-rw-r--r--  2.0 unx     6395 b- defN 24-Jun-03 10:23 nucliadb/train/uploader.py
+-rw-r--r--  2.0 unx     3179 b- defN 24-Jun-03 10:23 nucliadb/train/utils.py
+-rw-r--r--  2.0 unx      835 b- defN 24-Jun-03 10:23 nucliadb/train/api/__init__.py
+-rw-r--r--  2.0 unx     1479 b- defN 24-Jun-03 10:23 nucliadb/train/api/utils.py
+-rw-r--r--  2.0 unx      928 b- defN 24-Jun-03 10:23 nucliadb/train/api/v1/__init__.py
+-rw-r--r--  2.0 unx     2071 b- defN 24-Jun-03 10:23 nucliadb/train/api/v1/check.py
+-rw-r--r--  2.0 unx      910 b- defN 24-Jun-03 10:23 nucliadb/train/api/v1/router.py
+-rw-r--r--  2.0 unx     1908 b- defN 24-Jun-03 10:23 nucliadb/train/api/v1/shards.py
+-rw-r--r--  2.0 unx     2135 b- defN 24-Jun-03 10:23 nucliadb/train/api/v1/trainset.py
+-rw-r--r--  2.0 unx      835 b- defN 24-Jun-03 10:23 nucliadb/train/generators/__init__.py
+-rw-r--r--  2.0 unx     3723 b- defN 24-Jun-03 10:23 nucliadb/train/generators/field_classifier.py
+-rw-r--r--  2.0 unx     6712 b- defN 24-Jun-03 10:23 nucliadb/train/generators/image_classifier.py
+-rw-r--r--  2.0 unx     2789 b- defN 24-Jun-03 10:23 nucliadb/train/generators/paragraph_classifier.py
+-rw-r--r--  2.0 unx     3590 b- defN 24-Jun-03 10:23 nucliadb/train/generators/paragraph_streaming.py
+-rw-r--r--  2.0 unx     5372 b- defN 24-Jun-03 10:23 nucliadb/train/generators/question_answer_streaming.py
+-rw-r--r--  2.0 unx     5160 b- defN 24-Jun-03 10:23 nucliadb/train/generators/sentence_classifier.py
+-rw-r--r--  2.0 unx    10446 b- defN 24-Jun-03 10:23 nucliadb/train/generators/token_classifier.py
+-rw-r--r--  2.0 unx     3877 b- defN 24-Jun-03 10:23 nucliadb/train/generators/utils.py
+-rw-r--r--  2.0 unx      835 b- defN 24-Jun-03 10:23 nucliadb/train/tests/__init__.py
+-rw-r--r--  2.0 unx     1125 b- defN 24-Jun-03 10:23 nucliadb/train/tests/conftest.py
+-rw-r--r--  2.0 unx    10995 b- defN 24-Jun-03 10:23 nucliadb/train/tests/fixtures.py
+-rw-r--r--  2.0 unx     4571 b- defN 24-Jun-03 10:23 nucliadb/train/tests/test_field_classification.py
+-rw-r--r--  2.0 unx     2729 b- defN 24-Jun-03 10:23 nucliadb/train/tests/test_get_entities.py
+-rw-r--r--  2.0 unx     1660 b- defN 24-Jun-03 10:23 nucliadb/train/tests/test_get_info.py
+-rw-r--r--  2.0 unx     1379 b- defN 24-Jun-03 10:23 nucliadb/train/tests/test_get_ontology.py
+-rw-r--r--  2.0 unx     2201 b- defN 24-Jun-03 10:23 nucliadb/train/tests/test_get_ontology_count.py
+-rw-r--r--  2.0 unx     7669 b- defN 24-Jun-03 10:23 nucliadb/train/tests/test_image_classification.py
+-rw-r--r--  2.0 unx     1416 b- defN 24-Jun-03 10:23 nucliadb/train/tests/test_list_fields.py
+-rw-r--r--  2.0 unx     2944 b- defN 24-Jun-03 10:23 nucliadb/train/tests/test_list_paragraphs.py
+-rw-r--r--  2.0 unx     1423 b- defN 24-Jun-03 10:23 nucliadb/train/tests/test_list_resources.py
+-rw-r--r--  2.0 unx     2947 b- defN 24-Jun-03 10:23 nucliadb/train/tests/test_list_sentences.py
+-rw-r--r--  2.0 unx     4645 b- defN 24-Jun-03 10:23 nucliadb/train/tests/test_paragraph_classification.py
+-rw-r--r--  2.0 unx     4320 b- defN 24-Jun-03 10:23 nucliadb/train/tests/test_paragraph_streaming.py
+-rw-r--r--  2.0 unx     8751 b- defN 24-Jun-03 10:23 nucliadb/train/tests/test_question_answer_streaming.py
+-rw-r--r--  2.0 unx     5051 b- defN 24-Jun-03 10:23 nucliadb/train/tests/test_sentence_classification.py
+-rw-r--r--  2.0 unx     5583 b- defN 24-Jun-03 10:23 nucliadb/train/tests/test_token_classification.py
+-rw-r--r--  2.0 unx     3324 b- defN 24-Jun-03 10:23 nucliadb/train/tests/utils.py
+-rw-r--r--  2.0 unx     1328 b- defN 24-Jun-03 10:23 nucliadb/writer/__init__.py
+-rw-r--r--  2.0 unx     4268 b- defN 24-Jun-03 10:23 nucliadb/writer/app.py
+-rw-r--r--  2.0 unx    19472 b- defN 24-Jun-03 10:23 nucliadb/writer/back_pressure.py
+-rw-r--r--  2.0 unx      929 b- defN 24-Jun-03 10:23 nucliadb/writer/exceptions.py
+-rw-r--r--  2.0 unx     1953 b- defN 24-Jun-03 10:23 nucliadb/writer/lifecycle.py
+-rw-r--r--  2.0 unx     1032 b- defN 24-Jun-03 10:23 nucliadb/writer/openapi.py
+-rw-r--r--  2.0 unx        0 b- defN 24-Jun-03 10:23 nucliadb/writer/py.typed
+-rw-r--r--  2.0 unx     1448 b- defN 24-Jun-03 10:23 nucliadb/writer/run.py
+-rw-r--r--  2.0 unx     3103 b- defN 24-Jun-03 10:23 nucliadb/writer/settings.py
+-rw-r--r--  2.0 unx     1036 b- defN 24-Jun-03 10:23 nucliadb/writer/utilities.py
+-rw-r--r--  2.0 unx      835 b- defN 24-Jun-03 10:23 nucliadb/writer/api/__init__.py
+-rw-r--r--  2.0 unx     1429 b- defN 24-Jun-03 10:23 nucliadb/writer/api/constants.py
+-rw-r--r--  2.0 unx     1095 b- defN 24-Jun-03 10:23 nucliadb/writer/api/v1/__init__.py
+-rw-r--r--  2.0 unx     6421 b- defN 24-Jun-03 10:23 nucliadb/writer/api/v1/export_import.py
+-rw-r--r--  2.0 unx    24482 b- defN 24-Jun-03 10:23 nucliadb/writer/api/v1/field.py
+-rw-r--r--  2.0 unx     5248 b- defN 24-Jun-03 10:23 nucliadb/writer/api/v1/knowledgebox.py
+-rw-r--r--  2.0 unx     2058 b- defN 24-Jun-03 10:23 nucliadb/writer/api/v1/learning_config.py
+-rw-r--r--  2.0 unx    18628 b- defN 24-Jun-03 10:23 nucliadb/writer/api/v1/resource.py
+-rw-r--r--  2.0 unx     1034 b- defN 24-Jun-03 10:23 nucliadb/writer/api/v1/router.py
+-rw-r--r--  2.0 unx    10485 b- defN 24-Jun-03 10:23 nucliadb/writer/api/v1/services.py
+-rw-r--r--  2.0 unx    30985 b- defN 24-Jun-03 10:23 nucliadb/writer/api/v1/upload.py
+-rw-r--r--  2.0 unx     1612 b- defN 24-Jun-03 10:23 nucliadb/writer/layouts/__init__.py
+-rw-r--r--  2.0 unx     2115 b- defN 24-Jun-03 10:23 nucliadb/writer/layouts/v1.py
+-rw-r--r--  2.0 unx      835 b- defN 24-Jun-03 10:23 nucliadb/writer/resource/__init__.py
+-rw-r--r--  2.0 unx     1425 b- defN 24-Jun-03 10:23 nucliadb/writer/resource/audit.py
+-rw-r--r--  2.0 unx    10968 b- defN 24-Jun-03 10:23 nucliadb/writer/resource/basic.py
+-rw-r--r--  2.0 unx    16740 b- defN 24-Jun-03 10:23 nucliadb/writer/resource/field.py
+-rw-r--r--  2.0 unx     2022 b- defN 24-Jun-03 10:23 nucliadb/writer/resource/origin.py
+-rw-r--r--  2.0 unx      835 b- defN 24-Jun-03 10:23 nucliadb/writer/tests/__init__.py
+-rw-r--r--  2.0 unx     1200 b- defN 24-Jun-03 10:23 nucliadb/writer/tests/conftest.py
+-rw-r--r--  2.0 unx     5971 b- defN 24-Jun-03 10:23 nucliadb/writer/tests/fixtures.py
+-rw-r--r--  2.0 unx    15472 b- defN 24-Jun-03 10:23 nucliadb/writer/tests/test_fields.py
+-rw-r--r--  2.0 unx    25988 b- defN 24-Jun-03 10:23 nucliadb/writer/tests/test_files.py
+-rw-r--r--  2.0 unx     1729 b- defN 24-Jun-03 10:23 nucliadb/writer/tests/test_knowledgebox.py
+-rw-r--r--  2.0 unx     4400 b- defN 24-Jun-03 10:23 nucliadb/writer/tests/test_reprocess_file_field.py
+-rw-r--r--  2.0 unx    16857 b- defN 24-Jun-03 10:23 nucliadb/writer/tests/test_resources.py
+-rw-r--r--  2.0 unx     5120 b- defN 24-Jun-03 10:23 nucliadb/writer/tests/test_service.py
+-rw-r--r--  2.0 unx     6054 b- defN 24-Jun-03 10:23 nucliadb/writer/tests/test_tus.py
+-rw-r--r--  2.0 unx     1287 b- defN 24-Jun-03 10:23 nucliadb/writer/tests/utils.py
+-rw-r--r--  2.0 unx     5226 b- defN 24-Jun-03 10:23 nucliadb/writer/tus/__init__.py
+-rw-r--r--  2.0 unx     5082 b- defN 24-Jun-03 10:23 nucliadb/writer/tus/dm.py
+-rw-r--r--  2.0 unx     2186 b- defN 24-Jun-03 10:23 nucliadb/writer/tus/exceptions.py
+-rw-r--r--  2.0 unx    14527 b- defN 24-Jun-03 10:23 nucliadb/writer/tus/gcs.py
+-rw-r--r--  2.0 unx     5849 b- defN 24-Jun-03 10:23 nucliadb/writer/tus/local.py
+-rw-r--r--  2.0 unx     4367 b- defN 24-Jun-03 10:23 nucliadb/writer/tus/pg.py
+-rw-r--r--  2.0 unx     9069 b- defN 24-Jun-03 10:23 nucliadb/writer/tus/s3.py
+-rw-r--r--  2.0 unx     4734 b- defN 24-Jun-03 10:23 nucliadb/writer/tus/storage.py
+-rw-r--r--  2.0 unx     2556 b- defN 24-Jun-03 10:23 nucliadb/writer/tus/utils.py
+-rw-r--r--  2.0 unx     4474 b- defN 24-Jun-03 10:24 nucliadb-4.0.3.post563.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-Jun-03 10:24 nucliadb-4.0.3.post563.dist-info/WHEEL
+-rw-r--r--  2.0 unx     1268 b- defN 24-Jun-03 10:24 nucliadb-4.0.3.post563.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx       20 b- defN 24-Jun-03 10:24 nucliadb-4.0.3.post563.dist-info/top_level.txt
+-rw-r--r--  2.0 unx        1 b- defN 24-Jun-03 10:24 nucliadb-4.0.3.post563.dist-info/zip-safe
+-rw-rw-r--  2.0 unx    44525 b- defN 24-Jun-03 10:24 nucliadb-4.0.3.post563.dist-info/RECORD
+475 files, 2290952 bytes uncompressed, 706270 bytes compressed:  69.2%
```

## zipnote {}

```diff
@@ -1401,26 +1401,26 @@
 
 Filename: nucliadb/writer/tus/storage.py
 Comment: 
 
 Filename: nucliadb/writer/tus/utils.py
 Comment: 
 
-Filename: nucliadb-4.0.3.post562.dist-info/METADATA
+Filename: nucliadb-4.0.3.post563.dist-info/METADATA
 Comment: 
 
-Filename: nucliadb-4.0.3.post562.dist-info/WHEEL
+Filename: nucliadb-4.0.3.post563.dist-info/WHEEL
 Comment: 
 
-Filename: nucliadb-4.0.3.post562.dist-info/entry_points.txt
+Filename: nucliadb-4.0.3.post563.dist-info/entry_points.txt
 Comment: 
 
-Filename: nucliadb-4.0.3.post562.dist-info/top_level.txt
+Filename: nucliadb-4.0.3.post563.dist-info/top_level.txt
 Comment: 
 
-Filename: nucliadb-4.0.3.post562.dist-info/zip-safe
+Filename: nucliadb-4.0.3.post563.dist-info/zip-safe
 Comment: 
 
-Filename: nucliadb-4.0.3.post562.dist-info/RECORD
+Filename: nucliadb-4.0.3.post563.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## migrations/0020_drain_nodes_from_cluster.py

```diff
@@ -56,15 +56,15 @@
         return
 
     logger.info("Rolling over affected KB", extra={"kbid": kbid})
     await rollover_kb_shards(context, kbid, drain_nodes=drain_node_ids)
 
 
 async def kb_has_shards_on_drain_nodes(kbid: str, drain_node_ids: list[str]) -> bool:
-    async with datamanagers.with_transaction(read_only=True) as txn:
+    async with datamanagers.with_ro_transaction() as txn:
         shards = await datamanagers.cluster.get_kb_shards(txn, kbid=kbid)
         if not shards:
             logger.warning("Shards object not found", extra={"kbid": kbid})
             return False
         shard_in_drain_nodes = False
         for shard in shards.shards:
             for replica in shard.replicas:
```

## nucliadb/metrics_exporter.py

```diff
@@ -53,15 +53,15 @@
         SHARD_COUNT.set(node.shard_count, labels=dict(node=node.id))
 
 
 async def iter_kbids(context: ApplicationContext) -> AsyncGenerator[str, None]:
     """
     Return a list of all KB ids.
     """
-    async with context.kv_driver.transaction() as txn:
+    async with context.kv_driver.transaction(read_only=True) as txn:
         async for kbid, _ in datamanagers.kb.get_kbs(txn):
             yield kbid
 
 
 async def update_migration_metrics(context: ApplicationContext):
     """
     Report the global migration version and the number of KBs per migration version.
```

## nucliadb/common/cluster/manager.py

```diff
@@ -121,15 +121,15 @@
         if node_id in READ_REPLICA_INDEX_NODES[primary_id]:
             READ_REPLICA_INDEX_NODES[primary_id].remove(node_id)
 
 
 class KBShardManager:
     # TODO: move to data manager
     async def get_shards_by_kbid_inner(self, kbid: str) -> writer_pb2.Shards:
-        async with datamanagers.with_transaction(read_only=True) as txn:
+        async with datamanagers.with_ro_transaction() as txn:
             result = await datamanagers.cluster.get_kb_shards(txn, kbid=kbid)
             if result is None:
                 # could be None because /shards doesn't exist, or beacause the
                 # whole KB does not exist. In any case, this should not happen
                 raise ShardsNotFound(kbid)
             return result
```

## nucliadb/common/cluster/rebalance.py

```diff
@@ -39,15 +39,15 @@
 REBALANCE_LOCK = "rebalance"
 
 
 async def get_shards_paragraphs(kbid: str) -> list[tuple[str, int]]:
     """
     Ordered shard -> num paragraph by number of paragraphs
     """
-    async with datamanagers.with_transaction(read_only=True) as txn:
+    async with datamanagers.with_ro_transaction() as txn:
         kb_shards = await datamanagers.cluster.get_kb_shards(txn, kbid=kbid)
     if kb_shards is None:
         return []
 
     results = {}
     for shard_meta in kb_shards.shards:
         node, shard_id = choose_node(shard_meta)
@@ -60,15 +60,15 @@
         (shard, paragraphs)
         for shard, paragraphs in sorted(results.items(), key=lambda x: x[1])
     ]
 
 
 async def maybe_add_shard(kbid: str) -> None:
     async with locking.distributed_lock(locking.NEW_SHARD_LOCK.format(kbid=kbid)):
-        async with datamanagers.with_transaction(read_only=True) as txn:
+        async with datamanagers.with_ro_transaction() as txn:
             kb_shards = await datamanagers.cluster.get_kb_shards(txn, kbid=kbid)
         if kb_shards is None:
             return
 
         shard_paragraphs = await get_shards_paragraphs(kbid)
         total_paragraphs = sum([c for _, c in shard_paragraphs])
```

## nucliadb/common/cluster/utils.py

```diff
@@ -125,19 +125,18 @@
 async def index_resource_to_shard(
     app_context: ApplicationContext,
     kbid: str,
     resource_id: str,
     shard: writer_pb2.ShardObject,
 ) -> Optional[noderesources_pb2.Resource]:
     logger.info("Indexing resource", extra={"kbid": kbid, "resource_id": resource_id})
-
     sm = app_context.shard_manager
     partitioning = app_context.partitioning
 
-    async with datamanagers.with_transaction() as txn:
+    async with datamanagers.with_ro_transaction() as txn:
         resource_index_message = (
             await datamanagers.resources.get_resource_index_message(
                 txn, kbid=kbid, rid=resource_id
             )
         )
 
     if resource_index_message is None:
```

## nucliadb/common/datamanagers/__init__.py

```diff
@@ -38,15 +38,15 @@
     labels,
     processing,
     resources,
     rollover,
     synonyms,
     vectorsets,
 )
-from .utils import with_transaction
+from .utils import with_ro_transaction, with_rw_transaction, with_transaction
 
 __all__ = (
     "atomic",
     "cluster",
     "entities",
     "exceptions",
     "fields",
@@ -54,8 +54,10 @@
     "labels",
     "processing",
     "resources",
     "rollover",
     "synonyms",
     "vectorsets",
     "with_transaction",
+    "with_rw_transaction",
+    "with_ro_transaction",
 )
```

## nucliadb/common/datamanagers/atomic.py

```diff
@@ -35,16 +35,18 @@
 
 """
 
 import sys
 from functools import wraps
 
 from . import kb as kb_dm
+from . import labels as labels_dm
 from . import resources as resources_dm
-from .utils import with_transaction
+from . import synonyms as synonyms_dm
+from .utils import with_ro_transaction, with_transaction
 
 # XXX: we are using the not exported _ParamSpec to support 3.9. Whenever we
 # upgrade to >= 3.10 we'll be able to use ParamSpecKwargs and improve the
 # typing. We are abusing of ParamSpec anywat to better support text editors, so
 # we also need to ignore some mypy complains
 
 __python_version = (sys.version_info.major, sys.version_info.minor)
@@ -55,30 +57,44 @@
 
 P = ParamSpec("P")
 
 
 def ro_txn_wrap(fun: P) -> P:  # type: ignore
     @wraps(fun)
     async def wrapper(**kwargs: P.kwargs):
-        async with with_transaction(read_only=True) as txn:
+        async with with_ro_transaction() as txn:
             return await fun(txn, **kwargs)
 
     return wrapper
 
 
 def rw_txn_wrap(fun: P) -> P:  # type: ignore
     @wraps(fun)
     async def wrapper(**kwargs: P.kwargs):
         async with with_transaction() as txn:
-            return await fun(txn, **kwargs)
+            result = await fun(txn, **kwargs)
+            await txn.commit()
+            return result
 
     return wrapper
 
 
 class kb:
     exists_kb = ro_txn_wrap(kb_dm.exists_kb)
 
 
 class resources:
     get_resource_uuid_from_slug = ro_txn_wrap(resources_dm.get_resource_uuid_from_slug)
     resource_exists = ro_txn_wrap(resources_dm.resource_exists)
     slug_exists = ro_txn_wrap(resources_dm.slug_exists)
+
+
+class labelset:
+    get = ro_txn_wrap(labels_dm.get_labelset)
+    set = rw_txn_wrap(labels_dm.set_labelset)
+    delete = rw_txn_wrap(labels_dm.delete_labelset)
+    get_all = ro_txn_wrap(labels_dm.get_labels)
+
+
+class synonyms:
+    get = ro_txn_wrap(synonyms_dm.get)
+    set = rw_txn_wrap(synonyms_dm.set)
```

## nucliadb/common/datamanagers/resources.py

```diff
@@ -26,15 +26,15 @@
 from nucliadb.common.maindb.exceptions import ConflictError, NotFoundError
 
 # These should be refactored
 from nucliadb.ingest.settings import settings as ingest_settings
 from nucliadb_protos import noderesources_pb2, resources_pb2
 from nucliadb_utils.utilities import get_storage
 
-from .utils import with_transaction
+from .utils import with_ro_transaction
 
 if TYPE_CHECKING:
     from nucliadb.ingest.orm.resource import Resource as ResourceORM
 
 
 KB_RESOURCE_BASIC = "/kbs/{kbid}/r/{uuid}"
 KB_RESOURCE_BASIC_FS = "/kbs/{kbid}/r/{uuid}/basic"  # Only used on FS driver
@@ -248,26 +248,26 @@
             yield rid
 
 
 @backoff.on_exception(
     backoff.expo, (Exception,), jitter=backoff.random_jitter, max_tries=3
 )
 async def _iter_resource_slugs(*, kbid: str) -> AsyncGenerator[str, None]:
-    async with with_transaction() as txn:
+    async with with_ro_transaction() as txn:
         async for key in txn.keys(
             match=KB_RESOURCE_SLUG_BASE.format(kbid=kbid), count=-1
         ):
             yield key.split("/")[-1]
 
 
 @backoff.on_exception(
     backoff.expo, (Exception,), jitter=backoff.random_jitter, max_tries=3
 )
 async def _get_resource_ids_from_slugs(kbid: str, slugs: list[str]) -> list[str]:
-    async with with_transaction() as txn:
+    async with with_ro_transaction() as txn:
         rids = await txn.batch_get(
             [KB_RESOURCE_SLUG.format(kbid=kbid, slug=slug) for slug in slugs]
         )
     return [rid.decode() for rid in rids if rid is not None]
 
 
 # KB resource count (materialized key)
```

## nucliadb/common/datamanagers/rollover.py

```diff
@@ -21,15 +21,15 @@
 from typing import AsyncGenerator, Optional
 
 import orjson
 
 from nucliadb.common.maindb.driver import Transaction
 from nucliadb_protos import writer_pb2
 
-from .utils import get_kv_pb, with_transaction
+from .utils import get_kv_pb, with_ro_transaction
 
 logger = logging.getLogger(__name__)
 
 KB_ROLLOVER_SHARDS = "/kbs/{kbid}/rollover/shards"
 KB_ROLLOVER_RESOURCES_TO_INDEX = "/kbs/{kbid}/rollover/to-index/{resource}"
 KB_ROLLOVER_RESOURCES_INDEXED = "/kbs/{kbid}/rollover/indexed/{resource}"
 
@@ -118,23 +118,23 @@
 
 async def iter_indexed_keys(*, kbid: str) -> AsyncGenerator[str, None]:
     """
     For TiKV internally `keys` is not part of this transaction so this is
     internally managed
     """
     start_key = KB_ROLLOVER_RESOURCES_INDEXED.format(kbid=kbid, resource="")
-    async with with_transaction() as txn:
+    async with with_ro_transaction() as txn:
         async for key in txn.keys(match=start_key, count=-1):
             yield key.split("/")[-1]
 
 
 async def _get_batch_indexed_data(
     *, kbid, batch: list[str]
 ) -> list[tuple[str, tuple[str, int]]]:
-    async with with_transaction() as txn:
+    async with with_ro_transaction() as txn:
         values = await txn.batch_get(
             [
                 KB_ROLLOVER_RESOURCES_INDEXED.format(kbid=kbid, resource=resource_id)
                 for resource_id in batch
             ]
         )
     results: list[tuple[str, tuple[str, int]]] = []
```

## nucliadb/common/datamanagers/utils.py

```diff
@@ -36,13 +36,26 @@
         return None
     pb = pb_type()
     pb.ParseFromString(serialized)
     return pb
 
 
 @contextlib.asynccontextmanager
-async def with_transaction(read_only: bool = False, wait_for_abort: bool = True):
+async def with_rw_transaction(wait_for_abort: bool = True):
     driver = get_driver()
     async with driver.transaction(
-        read_only=read_only, wait_for_abort=wait_for_abort
+        read_only=False, wait_for_abort=wait_for_abort
     ) as txn:
         yield txn
+
+
+# For backwards compatibility
+with_transaction = with_rw_transaction
+
+
+@contextlib.asynccontextmanager
+async def with_ro_transaction(wait_for_abort: bool = True):
+    driver = get_driver()
+    async with driver.transaction(
+        read_only=True, wait_for_abort=wait_for_abort
+    ) as ro_txn:
+        yield ro_txn
```

## nucliadb/common/maindb/pg.py

```diff
@@ -42,19 +42,20 @@
 
 
 class DataLayer:
     def __init__(self, connection: Union[asyncpg.Connection, asyncpg.Pool]):
         self.connection = connection
         self.lock = asyncio.Lock()
 
-    async def get(self, key: str) -> Optional[bytes]:
+    async def get(self, key: str, select_for_update: bool = False) -> Optional[bytes]:
         async with self.lock:
-            return await self.connection.fetchval(
-                "SELECT value FROM resources WHERE key = $1", key
-            )
+            statement = "SELECT value FROM resources WHERE key = $1"
+            if select_for_update:
+                statement += " FOR UPDATE"
+            return await self.connection.fetchval(statement, key)
 
     async def set(self, key: str, value: bytes) -> None:
         async with self.lock:
             await self.connection.execute(
                 """
 INSERT INTO resources (key, value)
 VALUES ($1, $2)
@@ -65,21 +66,24 @@
                 value,
             )
 
     async def delete(self, key: str) -> None:
         async with self.lock:
             await self.connection.execute("DELETE FROM resources WHERE key = $1", key)
 
-    async def batch_get(self, keys: list[str]) -> list[Optional[bytes]]:
-        async with self.lock:
+    async def batch_get(
+        self, keys: list[str], select_for_update: bool = False
+    ) -> list[Optional[bytes]]:
+        async with self.lock:
+            statement = "SELECT key, value FROM resources WHERE key = ANY($1)"
+            if select_for_update:
+                statement += " FOR UPDATE"
             records = {
                 record["key"]: record["value"]
-                for record in await self.connection.fetch(
-                    "SELECT key, value FROM resources WHERE key = ANY($1)", keys
-                )
+                for record in await self.connection.fetch(statement, keys)
             }
         # get sorted by keys
         return [records.get(key) for key in keys]
 
     async def scan_keys(
         self,
         prefix: str,
@@ -143,18 +147,18 @@
                 await self.txn.rollback()
                 raise
             finally:
                 self.open = False
                 await self.connection.close()
 
     async def batch_get(self, keys: list[str]):
-        return await self.data_layer.batch_get(keys)
+        return await self.data_layer.batch_get(keys, select_for_update=True)
 
     async def get(self, key: str) -> Optional[bytes]:
-        return await self.data_layer.get(key)
+        return await self.data_layer.get(key, select_for_update=True)
 
     async def set(self, key: str, value: bytes):
         await self.data_layer.set(key, value)
 
     async def delete(self, key: str):
         await self.data_layer.delete(key)
```

## nucliadb/export_import/datamanager.py

```diff
@@ -49,15 +49,15 @@
         if type not in ("export", "import"):
             raise ValueError(f"Invalid type: {type}")
         key = MAINDB_EXPORT_KEY if type == "export" else MAINDB_IMPORT_KY
         return key.format(kbid=kbid, id=id)
 
     async def get_metadata(self, type: str, kbid: str, id: str) -> Metadata:
         key = self._get_maindb_metadata_key(type, kbid, id)
-        async with self.driver.transaction() as txn:
+        async with self.driver.transaction(read_only=True) as txn:
             data = await txn.get(key)
         if data is None or data == b"":
             raise MetadataNotFound()
         decoded = data.decode("utf-8")
         model_type = {
             "export": ExportMetadata,
             "import": ImportMetadata,
```

## nucliadb/export_import/utils.py

```diff
@@ -172,15 +172,15 @@
     async for rid in datamanagers.resources.iterate_resource_ids(kbid=kbid):
         yield rid
 
 
 async def get_broker_message(
     context: ApplicationContext, kbid: str, rid: str
 ) -> Optional[writer_pb2.BrokerMessage]:
-    async with datamanagers.with_transaction() as txn:
+    async with datamanagers.with_ro_transaction() as txn:
         resource = await datamanagers.resources.get_resource(txn, kbid=kbid, rid=rid)
         if resource is None:
             return None
         resource.disable_vectors = False
         resource.txn = txn
         return await generate_broker_message(resource)
 
@@ -248,20 +248,20 @@
     context: ApplicationContext, cf: resources_pb2.CloudFile
 ) -> AsyncGenerator[bytes, None]:
     async for data in context.blob_storage.download(cf.bucket_name, cf.uri):
         yield data
 
 
 async def get_entities(context: ApplicationContext, kbid: str) -> kb_pb2.EntitiesGroups:
-    async with datamanagers.with_transaction() as txn:
+    async with datamanagers.with_ro_transaction() as txn:
         return await datamanagers.entities.get_entities_groups(txn, kbid=kbid)
 
 
 async def get_labels(context: ApplicationContext, kbid: str) -> kb_pb2.Labels:
-    async with datamanagers.with_transaction() as txn:
+    async with datamanagers.with_ro_transaction() as txn:
         return await datamanagers.labels.get_labels(txn, kbid=kbid)
 
 
 class EndOfStream(Exception): ...
 
 
 class ExportStream:
```

## nucliadb/ingest/serialize.py

```diff
@@ -492,10 +492,10 @@
 
 
 async def get_resource_uuid_by_slug(
     kbid: str, slug: str, service_name: Optional[str] = None
 ) -> Optional[str]:
     storage = await get_storage(service_name=service_name)
     driver = get_driver()
-    async with driver.transaction() as txn:
+    async with driver.transaction(read_only=True) as txn:
         kb = KnowledgeBox(txn, storage, kbid)
         return await kb.get_resource_uuid_by_slug(slug)
```

## nucliadb/ingest/consumer/materializer.py

```diff
@@ -92,15 +92,15 @@
 
         self.task_handler.schedule(
             notification.kbid, partial(self.process, notification.kbid)
         )
 
     async def process(self, kbid: str) -> None:
         logger.info(f"Materializing knowledgebox", extra={"kbid": kbid})
-        async with datamanagers.with_transaction(read_only=True) as txn:
+        async with datamanagers.with_ro_transaction() as txn:
             value = await datamanagers.resources.calculate_number_of_resources(
                 txn, kbid=kbid
             )
         async with datamanagers.with_transaction() as txn:
             await datamanagers.resources.set_number_of_resources(
                 txn, kbid=kbid, value=value
             )
```

## nucliadb/ingest/consumer/pull.py

```diff
@@ -148,15 +148,15 @@
         else:
             pull_type_id = "main"
 
         async with ProcessingHTTPClient() as processing_http_client:
             logger.info(f"Collecting from NucliaDB Cloud {self.partition} partition")
             while True:
                 try:
-                    async with datamanagers.with_transaction() as txn:
+                    async with datamanagers.with_ro_transaction() as txn:
                         cursor = await datamanagers.processing.get_pull_offset(
                             txn, pull_type_id=pull_type_id, partition=self.partition
                         )
 
                     data = await processing_http_client.pull(
                         self.partition,
                         cursor=cursor,
```

## nucliadb/ingest/orm/knowledgebox.py

```diff
@@ -19,20 +19,15 @@
 #
 from datetime import datetime
 from typing import AsyncGenerator, Optional, Sequence
 from uuid import uuid4
 
 from grpc import StatusCode
 from grpc.aio import AioRpcError
-from nucliadb_protos.knowledgebox_pb2 import (
-    KnowledgeBoxConfig,
-    Labels,
-    LabelSet,
-    SemanticModelMetadata,
-)
+from nucliadb_protos.knowledgebox_pb2 import KnowledgeBoxConfig, SemanticModelMetadata
 from nucliadb_protos.resources_pb2 import Basic
 from nucliadb_protos.utils_pb2 import ReleaseChannel
 
 from nucliadb.common import datamanagers
 from nucliadb.common.cluster.exceptions import ShardNotFound
 from nucliadb.common.cluster.manager import get_index_node
 from nucliadb.common.cluster.utils import get_shard_manager
@@ -72,15 +67,15 @@
         self.txn = txn
         self.storage = storage
         self.kbid = kbid
         self._config: Optional[KnowledgeBoxConfig] = None
 
     async def get_config(self) -> Optional[KnowledgeBoxConfig]:
         if self._config is None:
-            async with datamanagers.with_transaction() as txn:
+            async with datamanagers.with_ro_transaction() as txn:
                 config = await datamanagers.kb.get_config(txn, kbid=self.kbid)
             if config is not None:
                 self._config = config
                 return config
             else:
                 return None
         else:
@@ -216,39 +211,14 @@
         if config and exist != config:
             exist.MergeFrom(config)
 
         await datamanagers.kb.set_config(txn, kbid=uuid, config=exist)
 
         return uuid
 
-    # Labels
-    async def set_labelset(self, id: str, labelset: LabelSet):
-        await datamanagers.labels.set_labelset(
-            self.txn, kbid=self.kbid, labelset_id=id, labelset=labelset
-        )
-
-    async def get_labels(self) -> Labels:
-        return await datamanagers.labels.get_labels(self.txn, kbid=self.kbid)
-
-    async def get_labelset(
-        self, labelset: str, labelset_response: writer_pb2.GetLabelSetResponse
-    ):
-        ls = await datamanagers.labels.get_labelset(
-            self.txn,
-            kbid=self.kbid,
-            labelset_id=labelset,
-        )
-        if ls is not None:
-            labelset_response.labelset.CopyFrom(ls)
-
-    async def del_labelset(self, id: str):
-        await datamanagers.labels.delete_labelset(
-            self.txn, kbid=self.kbid, labelset_id=id
-        )
-
     @classmethod
     async def purge(cls, driver: Driver, kbid: str):
         """
         Deletes all kb parts
 
         It takes care of signaling the nodes related to this kb that they
         need to delete the kb shards and also deletes the related storage
@@ -305,15 +275,15 @@
 
     @classmethod
     async def delete_all_kb_keys(
         cls, driver: Driver, kbid: str, chunk_size: int = 1_000
     ):
         prefix = KB_KEYS.format(kbid=kbid)
         while True:
-            async with driver.transaction() as txn:
+            async with driver.transaction(read_only=True) as txn:
                 all_keys = [key async for key in txn.keys(match=prefix, count=-1)]
 
             if len(all_keys) == 0:
                 break
 
             # We commit deletions in chunks because otherwise
             # tikv complains if there is too much data to commit
@@ -322,15 +292,15 @@
                     for key in chunk_of_keys:
                         await txn.delete(key)
                     await txn.commit()
 
     async def get_resource_shard(
         self, shard_id: str
     ) -> Optional[writer_pb2.ShardObject]:
-        async with datamanagers.with_transaction() as txn:
+        async with datamanagers.with_ro_transaction() as txn:
             pb = await datamanagers.cluster.get_kb_shards(txn, kbid=self.kbid)
             if pb is None:
                 logger.warning("Shards not found for kbid", extra={"kbid": self.kbid})
                 return None
         for shard in pb.shards:
             if shard.shard == shard_id:
                 return shard
```

## nucliadb/ingest/orm/processor/auditing.py

```diff
@@ -31,15 +31,15 @@
 ) -> list[audit_pb2.AuditField]:
     if message.type == writer_pb2.BrokerMessage.MessageType.DELETE:
         # If we are fully deleting a resource we won't iterate the delete_fields (if any).
         # Make no sense as we already collected all resource fields as deleted
         return []
 
     audit_storage_fields: list[audit_pb2.AuditField] = []
-    async with driver.transaction() as txn:
+    async with driver.transaction(read_only=True) as txn:
         kb = KnowledgeBox(txn, storage, message.kbid)
         resource = Resource(txn, storage, kb, message.uuid)
         field_keys = await resource.get_fields_ids()
 
         for field_id, field_type in iterate_auditable_fields(field_keys, message):
             auditfield = audit_pb2.AuditField()
             auditfield.field_type = field_type
```

## nucliadb/ingest/orm/processor/sequence_manager.py

```diff
@@ -27,15 +27,15 @@
 async def get_last_seqid(driver: Driver, worker: str) -> Optional[int]:
     """
     Get last stored sequence id for a worker.
 
     This is oriented towards the ingest consumer and processor,
     which is the only one that should be writing to this key.
     """
-    async with driver.transaction() as txn:
+    async with driver.transaction(read_only=True) as txn:
         key = TXNID.format(worker=worker)
         last_seq = await txn.get(key)
         if not last_seq:
             return None
         else:
             return int(last_seq)
```

## nucliadb/ingest/service/writer.py

```diff
@@ -25,52 +25,45 @@
 from nucliadb_protos.knowledgebox_pb2 import (
     DeleteKnowledgeBoxResponse,
     GCKnowledgeBoxResponse,
     KnowledgeBoxID,
     KnowledgeBoxNew,
     KnowledgeBoxResponseStatus,
     KnowledgeBoxUpdate,
-    Labels,
     NewKnowledgeBoxResponse,
     SemanticModelMetadata,
     UpdateKnowledgeBoxResponse,
     VectorSetConfig,
 )
 from nucliadb_protos.resources_pb2 import CloudFile
 from nucliadb_protos.writer_pb2 import (
     BinaryData,
     BrokerMessage,
     DelEntitiesRequest,
-    DelLabelsRequest,
     DelVectorSetRequest,
     DelVectorSetResponse,
     ExtractedVectorsWrapper,
     FileRequest,
     FileUploaded,
     GetEntitiesGroupRequest,
     GetEntitiesGroupResponse,
     GetEntitiesRequest,
     GetEntitiesResponse,
-    GetLabelSetRequest,
-    GetLabelSetResponse,
-    GetLabelsRequest,
-    GetLabelsResponse,
     IndexResource,
     IndexStatus,
     ListEntitiesGroupsRequest,
     ListEntitiesGroupsResponse,
     ListMembersRequest,
     ListMembersResponse,
     NewEntitiesGroupRequest,
     NewEntitiesGroupResponse,
     NewVectorSetRequest,
     NewVectorSetResponse,
     OpStatusWriter,
     SetEntitiesRequest,
-    SetLabelsRequest,
     SetVectorsRequest,
     SetVectorsResponse,
     UpdateEntitiesGroupRequest,
     UpdateEntitiesGroupResponse,
     UploadBinaryData,
     WriterStatusRequest,
     WriterStatusResponse,
@@ -303,79 +296,14 @@
                 logger.exception("Error processing", stack_info=True)
                 response.status = OpStatusWriter.Status.ERROR
                 break
             response.status = OpStatusWriter.Status.OK
             logger.info(f"Processed {message.uuid}")
         return response
 
-    async def SetLabels(self, request: SetLabelsRequest, context=None) -> OpStatusWriter:  # type: ignore
-        async with self.driver.transaction() as txn:
-            kbobj = await self.proc.get_kb_obj(txn, request.kb)
-            response = OpStatusWriter()
-            if kbobj is not None:
-                try:
-                    await kbobj.set_labelset(request.id, request.labelset)
-                    await txn.commit()
-                    response.status = OpStatusWriter.Status.OK
-                except Exception as e:
-                    errors.capture_exception(e)
-                    logger.error("Error in ingest gRPC servicer", exc_info=True)
-                    response.status = OpStatusWriter.Status.ERROR
-            else:
-                response.status = OpStatusWriter.Status.NOTFOUND
-            return response
-
-    async def DelLabels(self, request: DelLabelsRequest, context=None) -> OpStatusWriter:  # type: ignore
-        async with self.driver.transaction() as txn:
-            kbobj = await self.proc.get_kb_obj(txn, request.kb)
-            response = OpStatusWriter()
-            if kbobj is not None:
-                try:
-                    await kbobj.del_labelset(request.id)
-                    await txn.commit()
-                    response.status = OpStatusWriter.Status.OK
-                except Exception as e:
-                    errors.capture_exception(e)
-                    logger.error("Error in ingest gRPC servicer", exc_info=True)
-                    response.status = OpStatusWriter.Status.ERROR
-            else:
-                response.status = OpStatusWriter.Status.NOTFOUND
-
-            return response
-
-    async def GetLabels(self, request: GetLabelsRequest, context=None) -> GetLabelsResponse:  # type: ignore
-        async with self.driver.transaction() as txn:
-            kbobj = await self.proc.get_kb_obj(txn, request.kb)
-            labels: Optional[Labels] = None
-            if kbobj is not None:
-                labels = await kbobj.get_labels()
-        response = GetLabelsResponse()
-        if kbobj is None:
-            response.status = GetLabelsResponse.Status.NOTFOUND
-        else:
-            response.kb.uuid = kbobj.kbid
-            if labels is not None:
-                response.labels.CopyFrom(labels)
-
-        return response
-
-    async def GetLabelSet(  # type: ignore
-        self, request: GetLabelSetRequest, context=None
-    ) -> GetLabelSetResponse:
-        async with self.driver.transaction() as txn:
-            kbobj = await self.proc.get_kb_obj(txn, request.kb)
-            response = GetLabelSetResponse()
-            if kbobj is not None:
-                await kbobj.get_labelset(request.labelset, response)
-                response.kb.uuid = kbobj.kbid
-                response.status = GetLabelSetResponse.Status.OK
-            else:
-                response.status = GetLabelSetResponse.Status.NOTFOUND
-            return response
-
     async def NewEntitiesGroup(  # type: ignore
         self, request: NewEntitiesGroupRequest, context=None
     ) -> NewEntitiesGroupResponse:
         response = NewEntitiesGroupResponse()
         async with self.driver.transaction() as txn:
             kbobj = await self.proc.get_kb_obj(txn, request.kb)
             if kbobj is None:
@@ -395,15 +323,15 @@
             response.status = NewEntitiesGroupResponse.Status.OK
             return response
 
     async def GetEntities(  # type: ignore
         self, request: GetEntitiesRequest, context=None
     ) -> GetEntitiesResponse:
         response = GetEntitiesResponse()
-        async with self.driver.transaction() as txn:
+        async with self.driver.transaction(read_only=True) as txn:
             kbobj = await self.proc.get_kb_obj(txn, request.kb)
 
             if kbobj is None:
                 response.status = GetEntitiesResponse.Status.NOTFOUND
                 return response
 
             entities_manager = EntitiesManager(kbobj, txn)
@@ -418,15 +346,15 @@
                 response.status = GetEntitiesResponse.Status.OK
             return response
 
     async def ListEntitiesGroups(  # type: ignore
         self, request: ListEntitiesGroupsRequest, context=None
     ) -> ListEntitiesGroupsResponse:
         response = ListEntitiesGroupsResponse()
-        async with self.driver.transaction() as txn:
+        async with self.driver.transaction(read_only=True) as txn:
             kbobj = await self.proc.get_kb_obj(txn, request.kb)
 
             if kbobj is None:
                 response.status = ListEntitiesGroupsResponse.Status.NOTFOUND
                 return response
 
             entities_manager = EntitiesManager(kbobj, txn, use_read_replica_nodes=True)
@@ -443,15 +371,15 @@
 
             return response
 
     async def GetEntitiesGroup(  # type: ignore
         self, request: GetEntitiesGroupRequest, context=None
     ) -> GetEntitiesGroupResponse:
         response = GetEntitiesGroupResponse()
-        async with self.driver.transaction() as txn:
+        async with self.driver.transaction(read_only=True) as txn:
             kbobj = await self.proc.get_kb_obj(txn, request.kb)
             if kbobj is None:
                 response.status = GetEntitiesGroupResponse.Status.KB_NOT_FOUND
                 return response
 
             entities_manager = EntitiesManager(kbobj, txn)
             try:
@@ -548,15 +476,15 @@
             return response
 
     async def Status(  # type: ignore
         self, request: WriterStatusRequest, context=None
     ) -> WriterStatusResponse:
         logger.info("Status Call")
         response = WriterStatusResponse()
-        async with self.driver.transaction() as txn:
+        async with self.driver.transaction(read_only=True) as txn:
             async for _, slug in datamanagers.kb.get_kbs(txn):
                 response.knowledgeboxes.append(slug)
 
             for partition in settings.partitions:
                 seq_id = await sequence_manager.get_last_seqid(self.driver, partition)
                 if seq_id is not None:
                     response.msgid[partition] = seq_id
@@ -689,15 +617,15 @@
             raise AttributeError("No destination file")
         await self.storage.uploaditerator(
             generate_buffer(self.storage, request), destination, cf
         )
         result = FileUploaded()
         return result
 
-    async def NewVectorSet(
+    async def NewVectorSet(  # type: ignore
         self, request: NewVectorSetRequest, context=None
     ) -> NewVectorSetResponse:
         config = VectorSetConfig(
             vectorset_id=request.vectorset_id,
             vectorset_index_config=nodewriter_pb2.VectorIndexConfig(
                 similarity=request.similarity,
                 normalize_vectors=request.normalize_vectors,
@@ -722,15 +650,15 @@
             )
             response.status = NewVectorSetResponse.Status.ERROR
             response.details = str(exc)
         else:
             response.status = NewVectorSetResponse.Status.OK
         return response
 
-    async def DelVectorSet(
+    async def DelVectorSet(  # type: ignore
         self, request: DelVectorSetRequest, context=None
     ) -> DelVectorSetResponse:
         response = DelVectorSetResponse()
         try:
             async with self.driver.transaction() as txn:
                 kbobj = KnowledgeBoxORM(txn, self.storage, request.kbid)
                 await kbobj.delete_vectorset(request.vectorset_id)
```

## nucliadb/purge/orphan_shards.py

```diff
@@ -82,15 +82,15 @@
                 "node_id": location.node_id,
             },
         )
 
     orphan_shard_ids = indexed_shards.keys() - stored_shards.keys()
     orphan_shards: dict[str, ShardLocation] = {}
     unavailable_nodes: set[str] = set()
-    async with datamanagers.with_transaction() as txn:
+    async with datamanagers.with_ro_transaction() as txn:
         for shard_id in orphan_shard_ids:
             node_id = indexed_shards[shard_id].node_id
             node = manager.get_index_node(node_id)  # type: ignore
             if node is None:
                 unavailable_nodes.add(node_id)
                 kbid = UNKNOWN_KB
             else:
```

## nucliadb/reader/api/v1/export_import.py

```diff
@@ -156,9 +156,9 @@
             retries=metadata.task.retries,
         )
     except MetadataNotFound:
         return HTTPClientError(status_code=404, detail=f"{type.capitalize()} not found")
 
 
 async def exists_kb(kbid: str) -> bool:
-    async with datamanagers.with_transaction(read_only=True) as txn:
+    async with datamanagers.with_ro_transaction() as txn:
         return await datamanagers.kb.exists_kb(txn, kbid=kbid)
```

## nucliadb/reader/api/v1/services.py

```diff
@@ -24,26 +24,23 @@
 from fastapi.responses import StreamingResponse
 from fastapi_versioning import version  # type: ignore
 from google.protobuf.json_format import MessageToDict
 from nucliadb_protos.knowledgebox_pb2 import Synonyms
 from nucliadb_protos.writer_pb2 import (
     GetEntitiesGroupRequest,
     GetEntitiesGroupResponse,
-    GetLabelSetRequest,
-    GetLabelSetResponse,
-    GetLabelsRequest,
-    GetLabelsResponse,
     ListEntitiesGroupsRequest,
     ListEntitiesGroupsResponse,
 )
 from starlette.requests import Request
 
 from nucliadb.common import datamanagers
 from nucliadb.common.cluster.settings import in_standalone_mode
 from nucliadb.common.context.fastapi import get_app_context
+from nucliadb.common.datamanagers.exceptions import KnowledgeBoxNotFound
 from nucliadb.common.http_clients import processing
 from nucliadb.common.maindb.utils import get_driver
 from nucliadb.ingest.orm.knowledgebox import KnowledgeBox
 from nucliadb.models.responses import HTTPClientError
 from nucliadb.reader import SERVICE_NAME
 from nucliadb.reader.api.v1.router import KB_PREFIX, api
 from nucliadb.reader.reader.notifications import kb_notifications_stream
@@ -51,14 +48,15 @@
     EntitiesGroup,
     EntitiesGroupSummary,
     KnowledgeBoxEntities,
 )
 from nucliadb_models.labels import KnowledgeBoxLabels, LabelSet
 from nucliadb_models.resource import NucliaDBRoles
 from nucliadb_models.synonyms import KnowledgeBoxSynonyms
+from nucliadb_protos import writer_pb2
 from nucliadb_utils.authentication import requires
 from nucliadb_utils.utilities import get_ingest, get_storage
 
 
 @api.get(
     f"/{KB_PREFIX}/{{kbid}}/entitiesgroups",
     status_code=200,
@@ -141,92 +139,89 @@
     status_code=200,
     summary="Get Knowledge Box Label Sets",
     response_model=KnowledgeBoxLabels,
     tags=["Knowledge Box Services"],
 )
 @requires(NucliaDBRoles.READER)
 @version(1)
-async def get_labelsets(request: Request, kbid: str) -> KnowledgeBoxLabels:
-    ingest = get_ingest()
-    l_request: GetLabelsRequest = GetLabelsRequest()
-    l_request.kb.uuid = kbid
+async def get_labelsets_endoint(request: Request, kbid: str) -> KnowledgeBoxLabels:
+    try:
+        return await get_labelsets(kbid)
+    except KnowledgeBoxNotFound:
+        raise HTTPException(status_code=404, detail="Knowledge Box does not exist")
+
 
-    kbobj: GetLabelsResponse = await ingest.GetLabels(l_request)  # type: ignore
-    if kbobj.status == GetLabelsResponse.Status.OK:
-        response = KnowledgeBoxLabels(uuid=kbid)
-        for labelset, labelset_data in kbobj.labels.labelset.items():
-            labelset_response = LabelSet(
-                **MessageToDict(
-                    labelset_data,
-                    preserving_proto_field_name=True,
-                    including_default_value_fields=True,
-                )
+async def get_labelsets(kbid: str) -> KnowledgeBoxLabels:
+    kb_exists = await datamanagers.atomic.kb.exists_kb(kbid=kbid)
+    if not kb_exists:
+        raise KnowledgeBoxNotFound()
+    labelsets: writer_pb2.Labels = await datamanagers.atomic.labelset.get_all(kbid=kbid)
+    response = KnowledgeBoxLabels(uuid=kbid)
+    for labelset, labelset_data in labelsets.labelset.items():
+        labelset_response = LabelSet(
+            **MessageToDict(
+                labelset_data,
+                preserving_proto_field_name=True,
+                including_default_value_fields=True,
             )
-            response.labelsets[labelset] = labelset_response
-        return response
-    elif kbobj.status == GetLabelsResponse.Status.NOTFOUND:
-        raise HTTPException(status_code=404, detail="Knowledge Box does not exist")
-    else:
-        raise HTTPException(
-            status_code=500, detail="Error on getting Knowledge box labels"
         )
+        response.labelsets[labelset] = labelset_response
+    return response
 
 
 @api.get(
     f"/{KB_PREFIX}/{{kbid}}/labelset/{{labelset}}",
     status_code=200,
     summary="Get a Knowledge Box Label Set",
     response_model=LabelSet,
     tags=["Knowledge Box Services"],
 )
 @requires(NucliaDBRoles.READER)
 @version(1)
-async def get_labelset(request: Request, kbid: str, labelset: str) -> LabelSet:
-    ingest = get_ingest()
-    l_request: GetLabelSetRequest = GetLabelSetRequest()
-    l_request.kb.uuid = kbid
-    l_request.labelset = labelset
+async def get_labelset_endpoint(request: Request, kbid: str, labelset: str) -> LabelSet:
+    try:
+        return await get_labelset(kbid, labelset)
+    except KnowledgeBoxNotFound:
+        raise HTTPException(status_code=404, detail="Knowledge Box does not exist")
+
 
-    kbobj: GetLabelSetResponse = await ingest.GetLabelSet(l_request)  # type: ignore
-    if kbobj.status == GetLabelSetResponse.Status.OK:
+async def get_labelset(kbid: str, labelset_id: str) -> LabelSet:
+    kb_exists = await datamanagers.atomic.kb.exists_kb(kbid=kbid)
+    if not kb_exists:
+        raise KnowledgeBoxNotFound()
+    labelset: Optional[writer_pb2.LabelSet] = await datamanagers.atomic.labelset.get(
+        kbid=kbid, labelset_id=labelset_id
+    )
+    if labelset is None:
+        response = LabelSet()
+    else:
         response = LabelSet(
             **MessageToDict(
-                kbobj.labelset,
+                labelset,
                 preserving_proto_field_name=True,
                 including_default_value_fields=True,
             )
         )
-        return response
-    elif kbobj.status == GetLabelSetResponse.Status.NOTFOUND:
-        raise HTTPException(status_code=404, detail="Knowledge Box does not exist")
-    else:
-        raise HTTPException(
-            status_code=500, detail="Error on getting labelset on a Knowledge box"
-        )
+    return response
 
 
 @api.get(
     f"/{KB_PREFIX}/{{kbid}}/custom-synonyms",
     status_code=200,
     summary="Get Knowledge Box Custom Synonyms",
     tags=["Knowledge Box Services"],
     response_model=KnowledgeBoxSynonyms,
     openapi_extra={"x-operation_order": 2},
 )
 @requires(NucliaDBRoles.READER)
 @version(1)
 async def get_custom_synonyms(request: Request, kbid: str):
-    async with datamanagers.with_transaction(read_only=True) as txn:
-        if not datamanagers.kb.exists_kb(txn, kbid=kbid):
-            raise HTTPException(status_code=404, detail="Knowledge Box does not exist")
-        synonyms = await datamanagers.synonyms.get(txn, kbid=kbid)
-
-    if synonyms is None:
-        synonyms = Synonyms()
-
+    if not await datamanagers.atomic.kb.exists_kb(kbid=kbid):
+        raise HTTPException(status_code=404, detail="Knowledge Box does not exist")
+    synonyms = await datamanagers.atomic.synonyms.get(kbid=kbid) or Synonyms()
     return KnowledgeBoxSynonyms.from_message(synonyms)
 
 
 @api.get(
     f"/{KB_PREFIX}/{{kbid}}/notifications",
     status_code=200,
     summary="Knowledge Box Notifications Stream",
@@ -258,15 +253,15 @@
         media_type="binary/octet-stream",
     )
 
     return response
 
 
 async def exists_kb(kbid: str) -> bool:
-    async with datamanagers.with_transaction(read_only=True) as txn:
+    async with datamanagers.with_ro_transaction() as txn:
         return await datamanagers.kb.exists_kb(txn, kbid=kbid)
 
 
 @api.get(
     f"/{KB_PREFIX}/{{kbid}}/processing-status",
     status_code=200,
     summary="Knowledge Box Processing Status",
```

## nucliadb/search/api/v1/knowledgebox.py

```diff
@@ -150,15 +150,15 @@
                 status_code=500, detail=f"Error while geting shard data"
             )
 
         field_count += shard.fields
         paragraph_count += shard.paragraphs
         sentence_count += shard.sentences
 
-    async with datamanagers.with_transaction() as txn:
+    async with datamanagers.with_ro_transaction() as txn:
         try:
             if len(shard_groups) <= 1:
                 # for smaller kbs, this is faster and more up to date
                 resource_count = (
                     await datamanagers.resources.calculate_number_of_resources(
                         txn, kbid=kbid
                     )
```

## nucliadb/search/api/v1/resource/ask.py

```diff
@@ -103,11 +103,11 @@
         x_forwarded_for,
         x_synchronous,
         resource=resource_id,
     )
 
 
 async def get_resource_uuid_by_slug(kbid: str, slug: str) -> Optional[str]:
-    async with datamanagers.with_transaction() as txn:
+    async with datamanagers.with_ro_transaction() as txn:
         return await datamanagers.resources.get_resource_uuid_from_slug(
             txn, kbid=kbid, slug=slug
         )
```

## nucliadb/search/api/v1/resource/chat.py

```diff
@@ -166,11 +166,11 @@
             detail=f"Temporary error while rephrasing the query. Please try again later. Error: {err}",
         )
     except InvalidQueryError as exc:
         return HTTPClientError(status_code=412, detail=str(exc))
 
 
 async def get_resource_uuid_by_slug(kbid: str, slug: str) -> Optional[str]:
-    async with datamanagers.with_transaction() as txn:
+    async with datamanagers.with_ro_transaction() as txn:
         return await datamanagers.resources.get_resource_uuid_from_slug(
             txn, kbid=kbid, slug=slug
         )
```

## nucliadb/search/search/predict_proxy.py

```diff
@@ -80,9 +80,9 @@
     if nuclia_learning_id:
         response.headers["NUCLIA-LEARNING-ID"] = nuclia_learning_id
         response.headers["Access-Control-Expose-Headers"] = "NUCLIA-LEARNING-ID"
     return response
 
 
 async def exists_kb(kbid: str) -> bool:
-    async with datamanagers.with_transaction(read_only=True) as txn:
+    async with datamanagers.with_ro_transaction() as txn:
         return await datamanagers.kb.exists_kb(txn, kbid=kbid)
```

## nucliadb/standalone/api_router.py

```diff
@@ -159,15 +159,15 @@
         },
         media_type="application/octet-stream",
     )
 
 
 @standalone_api_router.get("/pull/position")
 async def pull_status(request: Request) -> JSONResponse:
-    async with datamanagers.with_transaction() as txn:
+    async with datamanagers.with_ro_transaction() as txn:
         # standalone assumes 1 partition
         current_offset = await datamanagers.processing.get_pull_offset(
             txn, pull_type_id=processing.get_nua_api_id(), partition="1"
         )
 
     async with processing.ProcessingHTTPClient() as client:
         end_offset = await client.pull_position(partition="1")
```

## nucliadb/tests/unit/common/cluster/test_rollover.py

```diff
@@ -138,14 +138,18 @@
     with (
         patch("nucliadb.common.cluster.rollover.datamanagers.rollover", mock),
         patch(
             "nucliadb.common.cluster.rollover.datamanagers.with_transaction",
             return_value=AsyncMock(),
         ),
         patch(
+            "nucliadb.common.cluster.rollover.datamanagers.with_ro_transaction",
+            return_value=AsyncMock(),
+        ),
+        patch(
             "nucliadb.ingest.consumer.shard_creator.locking.distributed_lock",
             return_value=AsyncMock(),
         ),
     ):
         yield mock
 
 
@@ -189,15 +193,14 @@
     rollover_datamanager.update_kb_rollover_shards.assert_not_called()
 
 
 async def test_index_rollover_shards(
     app_context, rollover_datamanager, resources_datamanager, shards, resource_ids
 ):
     rollover_datamanager.get_kb_rollover_shards.return_value = shards
-
     await rollover.index_rollover_shards(app_context, "kbid")
     rollover_datamanager.add_indexed.assert_called_with(
         ANY, kbid="kbid", resource_id="1", shard_id="1", modification_time=1
     )
 
 
 async def test_index_rollover_shards_handles_missing_shards(
```

## nucliadb/train/servicer.py

```diff
@@ -14,18 +14,16 @@
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the
 # GNU Affero General Public License for more details.
 #
 # You should have received a copy of the GNU Affero General Public License
 # along with this program. If not, see <http://www.gnu.org/licenses/>.
 #
 import traceback
-from typing import Optional
 
 import aiohttp
-from nucliadb_protos.knowledgebox_pb2 import Labels
 from nucliadb_protos.train_pb2 import (
     GetFieldsRequest,
     GetInfoRequest,
     GetLabelsetsCountRequest,
     GetParagraphsRequest,
     GetResourcesRequest,
     GetSentencesRequest,
@@ -35,14 +33,15 @@
 from nucliadb_protos.writer_pb2 import (
     GetEntitiesRequest,
     GetEntitiesResponse,
     GetLabelsRequest,
     GetLabelsResponse,
 )
 
+from nucliadb.common import datamanagers
 from nucliadb.train.settings import settings
 from nucliadb.train.utils import get_shard_manager
 from nucliadb_protos import train_pb2_grpc
 from nucliadb_telemetry import errors
 
 
 class TrainServicer(train_pb2_grpc.TrainServicer):
@@ -107,28 +106,23 @@
                 response.kb.uuid = kbid
                 response.status = GetEntitiesResponse.Status.OK
         return response
 
     async def GetOntology(  # type: ignore
         self, request: GetLabelsRequest, context=None
     ) -> GetLabelsResponse:
-        async with self.proc.driver.transaction() as txn:
-            kbobj = await self.proc.get_kb_obj(txn, request.kb.uuid)
-            labels: Optional[Labels] = None
-            if kbobj is not None:
-                labels = await kbobj.get_labels()
-
         response = GetLabelsResponse()
-        if kbobj is None:
-            response.status = GetLabelsResponse.Status.NOTFOUND
+        kbid = request.kb.uuid
+        labels = await datamanagers.atomic.labelset.get_all(kbid=kbid)
+        if labels is not None:
+            response.kb.uuid = kbid
+            response.status = GetLabelsResponse.Status.OK
+            response.labels.CopyFrom(labels)
         else:
-            response.kb.uuid = kbobj.kbid
-            if labels is not None:
-                response.labels.CopyFrom(labels)
-
+            response.status = GetLabelsResponse.Status.NOTFOUND
         return response
 
     async def GetOntologyCount(  # type: ignore
         self, request: GetLabelsetsCountRequest, context=None
     ) -> LabelsetsCount:
         url = settings.internal_search_api.format(kbid=request.kb.uuid)
         facets = [f"faceted=/p/{labelset}" for labelset in request.paragraph_labelsets]
```

## nucliadb/train/uploader.py

```diff
@@ -31,14 +31,15 @@
 from nucliadb_protos.writer_pb2 import (
     GetEntitiesRequest,
     GetEntitiesResponse,
     GetLabelsRequest,
     GetLabelsResponse,
 )
 
+from nucliadb.common import datamanagers
 from nucliadb.common.maindb.utils import setup_driver
 from nucliadb.ingest.orm.entities import EntitiesManager
 from nucliadb.ingest.orm.processor import Processor
 from nucliadb.train import SERVICE_NAME
 from nucliadb.train.models import RequestData
 from nucliadb.train.settings import settings
 from nucliadb_utils.utilities import get_pubsub, get_storage
@@ -86,28 +87,24 @@
             response.kb.uuid = kbid
             response.status = GetEntitiesResponse.Status.OK
         return response
 
     async def GetOntology(  # type: ignore
         self, request: GetLabelsRequest, context=None
     ) -> GetLabelsResponse:
-        async with self.proc.driver.transaction() as txn:
-            kbobj = await self.proc.get_kb_obj(txn, request.kb)
-            labels: Optional[Labels] = None
-            if kbobj is not None:
-                labels = await kbobj.get_labels()
-
+        kbid = request.kb.uuid
         response = GetLabelsResponse()
-        if kbobj is None:
+        kb_exists = await datamanagers.atomic.kb.exists_kb(kbid=kbid)
+        if not kb_exists:
             response.status = GetLabelsResponse.Status.NOTFOUND
-        else:
-            response.kb.uuid = kbobj.kbid
-            if labels is not None:
-                response.labels.CopyFrom(labels)
-
+            return response
+        response.kb.uuid = kbid
+        labels: Optional[Labels] = await datamanagers.atomic.labelset.get_all(kbid=kbid)
+        if labels is not None:
+            response.labels.CopyFrom(labels)
         return response
 
 
 async def start_upload(request: str, kb: str):
     us = UploadServicer()
     await us.initialize()
```

## nucliadb/train/tests/fixtures.py

```diff
@@ -20,31 +20,29 @@
 import asyncio
 import uuid
 from datetime import datetime
 
 import aiohttp
 import pytest
 from grpc import aio
+from httpx import AsyncClient
 from nucliadb_protos.knowledgebox_pb2 import EntitiesGroup, Label, LabelSet
 from nucliadb_protos.resources_pb2 import (
     ExtractedTextWrapper,
     FieldComputedMetadataWrapper,
     FieldID,
     FieldType,
     Paragraph,
     Position,
     Sentence,
 )
-from nucliadb_protos.writer_pb2 import (
-    BrokerMessage,
-    SetEntitiesRequest,
-    SetLabelsRequest,
-)
+from nucliadb_protos.writer_pb2 import BrokerMessage, SetEntitiesRequest
 from nucliadb_protos.writer_pb2_grpc import WriterStub
 
+from nucliadb.common import datamanagers
 from nucliadb.common.datamanagers.resources import KB_RESOURCE_SLUG_BASE
 from nucliadb.ingest.orm.entities import EntitiesManager
 from nucliadb.ingest.orm.knowledgebox import KnowledgeBox
 from nucliadb.ingest.orm.processor import Processor
 from nucliadb.standalone.settings import Settings
 from nucliadb.train.utils import start_shard_manager, stop_shard_manager
 from nucliadb_utils.tests import free_port
@@ -66,34 +64,32 @@
         headers={"X-NUCLIADB-ROLES": "WRITER"},
         base_url=f"http://localhost:{nucliadb.http_port}",
     ) as client:
         yield client
 
 
 @pytest.fixture(scope="function")
-async def knowledgebox_with_labels(nucliadb_grpc: WriterStub, knowledgebox: str):
-    slr = SetLabelsRequest()
-    slr.kb.uuid = knowledgebox
-    slr.id = "labelset_paragraphs"
-    slr.labelset.kind.append(LabelSet.LabelSetKind.PARAGRAPHS)
-    l1 = Label(title="label_machine")
-    l2 = Label(title="label_user")
-    slr.labelset.labels.append(l1)
-    slr.labelset.labels.append(l2)
-    await nucliadb_grpc.SetLabels(slr)  # type: ignore
-
-    slr = SetLabelsRequest()
-    slr.kb.uuid = knowledgebox
-    slr.id = "labelset_resources"
-    slr.labelset.kind.append(LabelSet.LabelSetKind.RESOURCES)
-    l1 = Label(title="label_machine")
-    l2 = Label(title="label_user")
-    slr.labelset.labels.append(l1)
-    slr.labelset.labels.append(l2)
-    await nucliadb_grpc.SetLabels(slr)  # type: ignore
+async def knowledgebox_with_labels(nucliadb_writer: AsyncClient, knowledgebox: str):
+    resp = await nucliadb_writer.post(
+        f"kb/{knowledgebox}/labelset/labelset_paragraphs",
+        json={
+            "kind": ["PARAGRAPHS"],
+            "labels": [{"title": "label_machine"}, {"title": "label_user"}],
+        },
+    )
+    assert resp.status_code == 200
+
+    resp = await nucliadb_writer.post(
+        f"kb/{knowledgebox}/labelset/labelset_resources",
+        json={
+            "kind": ["RESOURCES"],
+            "labels": [{"title": "label_machine"}, {"title": "label_user"}],
+        },
+    )
+    assert resp.status_code == 200
 
     yield knowledgebox
 
 
 @pytest.fixture(scope="function")
 async def knowledgebox_with_entities(nucliadb_grpc: WriterStub, knowledgebox: str):
     ser = SetEntitiesRequest()
@@ -282,16 +278,17 @@
     # Add ontology
     labelset = LabelSet()
     labelset.title = "ls1"
     label = Label()
     label_title = "label1"
     label.title = label_title
     labelset.labels.append(label)
-    await kb.set_labelset(label_title, labelset)
-    await txn.commit()
+    await datamanagers.atomic.labelset.set(
+        kbid=knowledgebox_ingest, labelset_id="ls1", labelset=labelset
+    )
 
     yield knowledgebox_ingest
 
 
 @pytest.fixture(scope="function")
 def test_settings_train(cache, gcs, fake_node, maindb_driver):  # type: ignore
     from nucliadb.train.settings import settings
```

## nucliadb/train/tests/test_field_classification.py

```diff
@@ -17,24 +17,24 @@
 # You should have received a copy of the GNU Affero General Public License
 # along with this program. If not, see <http://www.gnu.org/licenses/>.
 
 import asyncio
 
 import aiohttp
 import pytest
+from httpx import AsyncClient
 from nucliadb_protos.dataset_pb2 import FieldClassificationBatch, TaskType, TrainSet
-from nucliadb_protos.knowledgebox_pb2 import Label, LabelSet
-from nucliadb_protos.writer_pb2 import SetLabelsRequest
 from nucliadb_protos.writer_pb2_grpc import WriterStub
 
 from nucliadb.tests.utils import inject_message
 from nucliadb.tests.utils.broker_messages import BrokerMessageBuilder
 from nucliadb.train import API_PREFIX
 from nucliadb.train.api.v1.router import KB_PREFIX
 from nucliadb.train.tests.utils import get_batches_from_train_response_stream
+from nucliadb_models.labels import LabelSetKind
 
 
 @pytest.mark.asyncio
 @pytest.mark.parametrize("knowledgebox", ["STABLE", "EXPERIMENTAL"], indirect=True)
 async def test_generator_field_classification(
     train_rest_api: aiohttp.ClientSession,
     knowledgebox_with_labels: str,
@@ -81,32 +81,42 @@
                 total += len(batch.data)
             assert len(batches) == expected_batches
             assert total == expected_total
 
 
 @pytest.fixture(scope="function")
 @pytest.mark.asyncio
-async def knowledgebox_with_labels(nucliadb_grpc: WriterStub, knowledgebox: str):
-    slr = SetLabelsRequest()
-    slr.kb.uuid = knowledgebox
-    slr.id = "labelset_paragraphs"
-    slr.labelset.kind.append(LabelSet.LabelSetKind.PARAGRAPHS)
-    slr.labelset.labels.append(Label(title="label_machine"))
-    slr.labelset.labels.append(Label(title="label_user"))
-    slr.labelset.labels.append(Label(title="label_alien"))
-    await nucliadb_grpc.SetLabels(slr)  # type: ignore
-
-    slr = SetLabelsRequest()
-    slr.kb.uuid = knowledgebox
-    slr.id = "labelset_resources"
-    slr.labelset.kind.append(LabelSet.LabelSetKind.RESOURCES)
-    slr.labelset.labels.append(Label(title="label_machine"))
-    slr.labelset.labels.append(Label(title="label_user"))
-    slr.labelset.labels.append(Label(title="label_alien"))
-    await nucliadb_grpc.SetLabels(slr)  # type: ignore
+async def knowledgebox_with_labels(
+    nucliadb_grpc: WriterStub, nucliadb_writer: AsyncClient, knowledgebox: str
+):
+    resp = await nucliadb_writer.post(
+        f"/kb/{knowledgebox}/labelset/labelset_paragraphs",
+        json={
+            "kind": [LabelSetKind.PARAGRAPHS],
+            "labels": [
+                {"title": "label_machine"},
+                {"title": "label_user"},
+                {"title": "label_alien"},
+            ],
+        },
+    )
+    assert resp.status_code == 200
+
+    resp = await nucliadb_writer.post(
+        f"/kb/{knowledgebox}/labelset/labelset_resources",
+        json={
+            "kind": [LabelSetKind.RESOURCES],
+            "labels": [
+                {"title": "label_machine"},
+                {"title": "label_user"},
+                {"title": "label_alien"},
+            ],
+        },
+    )
+    assert resp.status_code == 200
 
     bmb = BrokerMessageBuilder(kbid=knowledgebox)
     bmb.with_title("First resource")
     bmb.with_summary("First summary")
     bmb.with_resource_labels("labelset_resources", ["label_user"])
     bm = bmb.build()
     await inject_message(nucliadb_grpc, bm)
```

## nucliadb/train/tests/test_get_ontology.py

```diff
@@ -27,8 +27,8 @@
 async def test_get_ontology(
     train_client: TrainStub, knowledgebox_ingest: str, test_pagination_resources
 ) -> None:
     req = GetLabelsRequest()
     req.kb.uuid = knowledgebox_ingest
 
     labels: GetLabelsResponse = await train_client.GetOntology(req)  # type: ignore
-    assert labels.labels.labelset["label1"].labels[0].title == "label1"
+    assert labels.labels.labelset["ls1"].labels[0].title == "label1"
```

## nucliadb/writer/back_pressure.py

```diff
@@ -527,15 +527,15 @@
     async with context.kv_driver.transaction() as txn:
         return await context.shard_manager.get_current_active_shard(txn, kbid)
 
 
 async def get_resource_shard(
     context: ApplicationContext, kbid: str, resource_uuid: str
 ) -> Optional[ShardObject]:
-    async with datamanagers.with_transaction(read_only=True) as txn:
+    async with datamanagers.with_ro_transaction() as txn:
         shard_id = await datamanagers.resources.get_resource_shard_id(
             txn, kbid=kbid, rid=resource_uuid
         )
         if shard_id is None:
             # Resource does not exist
             logger.debug(
                 "Resource shard not found",
```

## nucliadb/writer/exceptions.py

```diff
@@ -15,17 +15,13 @@
 # GNU Affero General Public License for more details.
 #
 # You should have received a copy of the GNU Affero General Public License
 # along with this program. If not, see <http://www.gnu.org/licenses/>.
 #
 
 
-class ConflictError(Exception):
-    pass
-
-
 class ResourceNotFound(Exception):
     pass
 
 
 class IngestNotAvailable(Exception):
     pass
```

## nucliadb/writer/api/v1/services.py

```diff
@@ -19,38 +19,39 @@
 #
 from fastapi import HTTPException, Response
 from fastapi_versioning import version
 from nucliadb_protos.knowledgebox_pb2 import Label as LabelPB
 from nucliadb_protos.knowledgebox_pb2 import LabelSet as LabelSetPB
 from nucliadb_protos.writer_pb2 import (
     DelEntitiesRequest,
-    DelLabelsRequest,
     NewEntitiesGroupRequest,
     NewEntitiesGroupResponse,
     OpStatusWriter,
-    SetLabelsRequest,
     UpdateEntitiesGroupRequest,
     UpdateEntitiesGroupResponse,
 )
 from starlette.requests import Request
 
 from nucliadb.common import datamanagers
+from nucliadb.common.datamanagers.exceptions import KnowledgeBoxNotFound
+from nucliadb.common.maindb.exceptions import ConflictError
 from nucliadb.models.responses import (
     HTTPConflict,
     HTTPInternalServerError,
     HTTPNotFound,
 )
 from nucliadb.writer.api.v1.router import KB_PREFIX, api
 from nucliadb_models.entities import (
     CreateEntitiesGroupPayload,
     UpdateEntitiesGroupPayload,
 )
 from nucliadb_models.labels import LabelSet
 from nucliadb_models.resource import NucliaDBRoles
 from nucliadb_models.synonyms import KnowledgeBoxSynonyms
+from nucliadb_protos import writer_pb2
 from nucliadb_utils.authentication import requires
 from nucliadb_utils.utilities import get_ingest
 
 
 @api.post(
     f"/{KB_PREFIX}/{{kbid}}/entitiesgroups",
     status_code=200,
@@ -176,96 +177,100 @@
     status_code=200,
     summary="Set Knowledge Box Labels",
     tags=["Knowledge Box Services"],
     openapi_extra={"x-operation_order": 1},
 )
 @requires(NucliaDBRoles.WRITER)
 @version(1)
-async def set_labels(request: Request, kbid: str, labelset: str, item: LabelSet):
-    ingest = get_ingest()
-    pbrequest: SetLabelsRequest = SetLabelsRequest(id=labelset)
-    pbrequest.kb.uuid = kbid
+async def set_labelset_endpoint(
+    request: Request, kbid: str, labelset: str, item: LabelSet
+):
+    try:
+        await set_labelset(kbid, labelset, item)
+    except KnowledgeBoxNotFound:
+        raise HTTPException(status_code=404, detail="Knowledge Box does not exist")
+    except ConflictError:
+        # TODO: Remove conflict error handling once we drop tikv support
+        raise HTTPException(
+            status_code=409,
+            detail="Conflict setting labelset on a Knowledge box. Please retry.",
+        )
 
-    if item.title:
-        pbrequest.labelset.title = item.title
 
-    if item.color:
-        pbrequest.labelset.color = item.color
-
-    pbrequest.labelset.multiple = item.multiple
+async def set_labelset(kbid: str, labelset_id: str, item: LabelSet):
+    kb_exists = await datamanagers.atomic.kb.exists_kb(kbid=kbid)
+    if not kb_exists:
+        raise KnowledgeBoxNotFound()
+    labelset = writer_pb2.LabelSet()
+    if item.title is not None:
+        labelset.title = item.title
+    if item.color is not None:
+        labelset.color = item.color
+    labelset.multiple = item.multiple
     for kind in item.kind:
-        pbrequest.labelset.kind.append(LabelSetPB.LabelSetKind.Value(kind))
-
+        labelset.kind.append(LabelSetPB.LabelSetKind.Value(kind))
     for label_input in item.labels:
         lbl = LabelPB()
         if label_input.uri:
             lbl.uri = label_input.uri
         if label_input.text:
             lbl.text = label_input.text
         if label_input.related:
             lbl.related = label_input.related
         if label_input.title:
             lbl.title = label_input.title
-        pbrequest.labelset.labels.append(lbl)
-    status: OpStatusWriter = await ingest.SetLabels(pbrequest)  # type: ignore
-    if status.status == OpStatusWriter.Status.OK:
-        return None
-    elif status.status == OpStatusWriter.Status.NOTFOUND:
-        raise HTTPException(status_code=404, detail="Knowledge Box does not exist")
-    elif status.status == OpStatusWriter.Status.ERROR:
-        raise HTTPException(
-            status_code=500, detail="Error on settings labels on a Knowledge box"
-        )
+        labelset.labels.append(lbl)
+    await datamanagers.atomic.labelset.set(
+        kbid=kbid, labelset_id=labelset_id, labelset=labelset
+    )
 
 
 @api.delete(
     f"/{KB_PREFIX}/{{kbid}}/labelset/{{labelset}}",
     status_code=200,
     summary="Delete Knowledge Box Label",
     tags=["Knowledge Box Services"],
     openapi_extra={"x-operation_order": 3},
 )
 @requires(NucliaDBRoles.WRITER)
 @version(1)
-async def delete_labels(request: Request, kbid: str, labelset: str):
-    ingest = get_ingest()
-    pbrequest: DelLabelsRequest = DelLabelsRequest()
-    pbrequest.kb.uuid = kbid
-    pbrequest.id = labelset
-    status: OpStatusWriter = await ingest.DelLabels(pbrequest)  # type: ignore
-    if status.status == OpStatusWriter.Status.OK:
-        return None
-    elif status.status == OpStatusWriter.Status.NOTFOUND:
+async def delete_labelset_endpoint(request: Request, kbid: str, labelset: str):
+    try:
+        await delete_labelset(kbid, labelset)
+    except KnowledgeBoxNotFound:
         raise HTTPException(status_code=404, detail="Knowledge Box does not exist")
-    elif status.status == OpStatusWriter.Status.ERROR:
+    except ConflictError:
+        # TODO: Remove conflict error handling once we drop tikv support
         raise HTTPException(
-            status_code=500, detail="Error on deleting labels from a Knowledge box"
+            status_code=409,
+            detail="Conflict deleting labelset from a Knowledge box. Please retry.",
         )
-    return Response(status_code=204)
+
+
+async def delete_labelset(kbid: str, labelset_id: str):
+    kb_exists = await datamanagers.atomic.kb.exists_kb(kbid=kbid)
+    if not kb_exists:
+        raise KnowledgeBoxNotFound()
+    await datamanagers.atomic.labelset.delete(kbid=kbid, labelset_id=labelset_id)
 
 
 @api.put(
     f"/{KB_PREFIX}/{{kbid}}/custom-synonyms",
     status_code=204,
     summary="Set Knowledge Box Custom Synonyms",
     tags=["Knowledge Box Services"],
     openapi_extra={"x-operation_order": 1},
 )
 @requires(NucliaDBRoles.WRITER)
 @version(1)
 async def set_custom_synonyms(request: Request, kbid: str, item: KnowledgeBoxSynonyms):
+    if not await datamanagers.atomic.kb.exists_kb(kbid=kbid):
+        raise HTTPException(status_code=404, detail="Knowledge Box does not exist")
     synonyms = item.to_message()
-
-    async with datamanagers.with_transaction() as txn:
-        if not datamanagers.kb.exists_kb(txn, kbid=kbid):
-            raise HTTPException(status_code=404, detail="Knowledge Box does not exist")
-
-        await datamanagers.synonyms.set(txn, kbid=kbid, synonyms=synonyms)
-        await txn.commit()
-
+    await datamanagers.atomic.synonyms.set(kbid=kbid, synonyms=synonyms)
     return Response(status_code=204)
 
 
 @api.delete(
     f"/{KB_PREFIX}/{{kbid}}/custom-synonyms",
     status_code=204,
     summary="Delete Knowledge Box Custom Synonyms",
```

## nucliadb/writer/tests/test_files.py

```diff
@@ -428,15 +428,15 @@
                     "X-LANGUAGE": "ca",
                     "X-MD5": "7af0916dba8b70e29d99e72941923529",
                     "content-type": "image/jpg",
                 },
             )
             assert resp.status_code == 201
 
-        async with datamanagers.with_transaction(read_only=True) as txn:
+        async with datamanagers.with_ro_transaction() as txn:
             assert (
                 await datamanagers.resources.has_field(
                     txn,
                     kbid=knowledgebox_writer,
                     rid=resource,
                     field_id=FieldID(field="field1", field_type=FieldType.FILE),
                 )
```

## Comparing `nucliadb-4.0.3.post562.dist-info/METADATA` & `nucliadb-4.0.3.post563.dist-info/METADATA`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nucliadb
-Version: 4.0.3.post562
+Version: 4.0.3.post563
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
-Requires-Dist: nucliadb-telemetry[all] >=4.0.3.post562
-Requires-Dist: nucliadb-utils[cache,fastapi,storages] >=4.0.3.post562
-Requires-Dist: nucliadb-protos >=4.0.3.post562
-Requires-Dist: nucliadb-models >=4.0.3.post562
+Requires-Dist: nucliadb-telemetry[all] >=4.0.3.post563
+Requires-Dist: nucliadb-utils[cache,fastapi,storages] >=4.0.3.post563
+Requires-Dist: nucliadb-protos >=4.0.3.post563
+Requires-Dist: nucliadb-models >=4.0.3.post563
 Requires-Dist: nucliadb-admin-assets >=1.0.0.post1224
 Requires-Dist: nucliadb-node-binding >=2.26.0
 Requires-Dist: uvicorn <0.19.0
 Requires-Dist: argdantic
 Requires-Dist: aiohttp >=3.9.4
 Requires-Dist: lru-dict >=1.1.7
 Requires-Dist: backoff
```

## Comparing `nucliadb-4.0.3.post562.dist-info/entry_points.txt` & `nucliadb-4.0.3.post563.dist-info/entry_points.txt`

 * *Files identical despite different names*

## Comparing `nucliadb-4.0.3.post562.dist-info/RECORD` & `nucliadb-4.0.3.post563.dist-info/RECORD`

 * *Files 2% similar despite different names*

```diff
@@ -12,101 +12,101 @@
 migrations/0013_rollover_shards.py,sha256=c3IU8zinlWeVRN8T6o5eLpvGzkQOHX_Yz5xuFVRUy5U,1024
 migrations/0014_rollover_shards.py,sha256=24yLtXAwlVvCwtHLx9Tz-VWCzeMuy-0o3M6QNESi_Iw,1382
 migrations/0015_targeted_rollover.py,sha256=7C9XM8wg-bpkNyFh0xJuaGzOcE2WqU1BfqtInKAjTkw,1462
 migrations/0016_upgrade_to_paragraphs_v2.py,sha256=pOZUwTDfGoLjcSSKiWaN6FUvMDN95XNCBoux3u0dsmQ,2506
 migrations/0017_multiple_writable_shards.py,sha256=NY38wFVxSDXglkZE6DRnuN1DG_1kyZXr2j37C8VhyA0,2100
 migrations/0018_purge_orphan_kbslugs.py,sha256=rlNPRkp04GGf88RrKV5ZavoDwrSnxtNlyT-P3_jB1gA,2264
 migrations/0019_upgrade_to_paragraphs_v3.py,sha256=Jf1ljYQoLj1QExz9-tDIxI7QrwPhixIHxvQJvHOl6WA,2506
-migrations/0020_drain_nodes_from_cluster.py,sha256=86HCbrIF9Q4-TC-Js8d5LDJFc2_18AcntwfCtqlXwho,3282
+migrations/0020_drain_nodes_from_cluster.py,sha256=qbIoic24Tv3wnoBSHGN6soraoHd8ZavfrCxXrZQ9UBY,3271
 migrations/0021_overwrite_vectorsets_key.py,sha256=omQbVYdssyWJ_asHmwtkezqsnmEde8oXQR9LIZY-6kg,1734
 migrations/__init__.py,sha256=cp15ZcFnHvpcu_5-aK2A4uUyvuZVV_MJn4bIXMa20ks,835
 nucliadb/__init__.py,sha256=_abCmDJ_0ku483Os4UAjPX7Nywm39cQgAV_DiyjsKeQ,891
 nucliadb/health.py,sha256=zPwd3CAFJf9owhbadtyGLvHekOjX9ykvxLYWYxnD5eo,3733
 nucliadb/learning_proxy.py,sha256=LC_4iKUrJvvnfQbOT_YG-IFuBviJgOWMvT7klzJ89UE,11793
-nucliadb/metrics_exporter.py,sha256=PummIqtRLdpcONPIpRKBj_jGYnX7B9XZ2IO048bu2pM,4806
+nucliadb/metrics_exporter.py,sha256=gI5c8hippNsOcNh8O4_qcm0NqC_l29SU-q_ovk6hhkU,4820
 nucliadb/openapi.py,sha256=wDiw0dVEvTpJvbatkJ0JZLkKm9RItZT5PWRHjqRfqTA,2272
 nucliadb/py.typed,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 nucliadb/common/__init__.py,sha256=cp15ZcFnHvpcu_5-aK2A4uUyvuZVV_MJn4bIXMa20ks,835
 nucliadb/common/ids.py,sha256=2RdVb4B9hK4WCxU5F-9ruZPBXlyyKlWX3xm0OH-Myyw,1912
 nucliadb/common/locking.py,sha256=bYfDSrWDyziKVxcmfM1HmB9pwDpOx6fPkyUviHgCK9Q,5175
 nucliadb/common/cluster/__init__.py,sha256=cp15ZcFnHvpcu_5-aK2A4uUyvuZVV_MJn4bIXMa20ks,835
 nucliadb/common/cluster/base.py,sha256=13ACuaNosUVsAkF1TqNv2xOMh_CJ9jpNv_bySiH1-ZI,5134
 nucliadb/common/cluster/exceptions.py,sha256=V3c_fgH00GyJ-a5CaGLhwTuhwhUNR9YAGvS5jaRuc_Y,1495
 nucliadb/common/cluster/grpc_node_dummy.py,sha256=rqco9bKGw77ssbKCakURWm5oGD4J0huEO5c30tvcA7Q,3793
 nucliadb/common/cluster/index_node.py,sha256=WafWLzU1l7EHj1VyG0w6qi2BW_Izc8rFze6ZWbYvT9g,3429
-nucliadb/common/cluster/manager.py,sha256=1UMXyLKT56SEcsiF3R0_gbEK3TPUGbM92zSVD_mADLA,24815
-nucliadb/common/cluster/rebalance.py,sha256=9jYILsIC93N3s62XltL2HLacQbLiXTNdMlG50v1ONR4,8853
+nucliadb/common/cluster/manager.py,sha256=nrAmPY-eVhogYpky-a0VXseaVPNUzeNw8NnboqNvbok,24804
+nucliadb/common/cluster/rebalance.py,sha256=z6VNkaPfzs9XiSpX8j1lznlKcZathsZtaPvIQy8HLus,8831
 nucliadb/common/cluster/rollover.py,sha256=bXnnZjWiq2GxPPcQuyMhFBiDrPGhWTyPFsyMejYnVVw,20532
 nucliadb/common/cluster/settings.py,sha256=-H30-AVnSe3iUUyFUga78xcMPScq7ZR6aNgRuVgQdu8,3016
-nucliadb/common/cluster/utils.py,sha256=15dQBg4XKmdD5iOZsOwU7YGx01h84HRZIWv48EtaUOE,5713
+nucliadb/common/cluster/utils.py,sha256=QCyW6aPuYOYFMSKfLSXjiULtDIC0JmKyXKDm3L3oWk4,5715
 nucliadb/common/cluster/discovery/__init__.py,sha256=cp15ZcFnHvpcu_5-aK2A4uUyvuZVV_MJn4bIXMa20ks,835
 nucliadb/common/cluster/discovery/base.py,sha256=P0JwzRYqOKxOzV_K_glwPizDGFGBY-l8G7TeTId9LIA,6553
 nucliadb/common/cluster/discovery/k8s.py,sha256=7ag_lluBoXqA-6C5M9PS3RmNmBG0QT2aZGyLAd6ltwI,12512
 nucliadb/common/cluster/discovery/manual.py,sha256=7wdcyfrR8oii2hP3AzOTAaUAGwkQu7eOj9Xl7Q49IUQ,1957
 nucliadb/common/cluster/discovery/single.py,sha256=2BhcencPKQQIfVitmTPJZm3TkBHyY9ZMcr-Clh8k2tM,1737
 nucliadb/common/cluster/discovery/types.py,sha256=vs-K790rofjZ4FWYaMkgjkZZqMvIvd_0eSw3shuiLwA,1139
 nucliadb/common/cluster/discovery/utils.py,sha256=A3DhpM3ExTSxtIo0Wh8ZIFARq2GW2OM1GPX967gyRbk,2548
 nucliadb/common/cluster/standalone/__init__.py,sha256=itSI7dtTwFP55YMX4iK7JzdMHS5CQVUiB1XzQu4UBh8,833
 nucliadb/common/cluster/standalone/grpc_node_binding.py,sha256=Rgw6w8vICjieoqhvhoHZ6mUgXbJpyXHvqpFPQ96N1yA,13712
 nucliadb/common/cluster/standalone/index_node.py,sha256=aKpkAEosp9qbd-77fYgE1AAnDc-6ER05cA_HJtkeBT0,4683
 nucliadb/common/cluster/standalone/service.py,sha256=tJI5Gc-cu4uprC84bcLQr4CMW0hBS9T2YX_Ex6zeyuI,3444
 nucliadb/common/cluster/standalone/utils.py,sha256=Y6Ni9P5piE9EeacQb4L5-o_TisAk2fl4btLwAV3tt8g,3545
 nucliadb/common/context/__init__.py,sha256=BuPPLOpTTzgD4oRb6mgmjPu-gRIaq4NeZTjx8FxAIV0,3440
 nucliadb/common/context/fastapi.py,sha256=qsxQ8s5dl67uCATrwdJCXA9JDfVn3DqxgsiWf6MUJhE,1628
-nucliadb/common/datamanagers/__init__.py,sha256=kIfpQW9JnTb2FrpuTYNKgMtDKzEsT2MsEgKRL4nvIxI,1966
-nucliadb/common/datamanagers/atomic.py,sha256=eLH9OBsGBTVnkC3j4mkfd_tMuW3ptloI90cgeM2vUWo,2648
+nucliadb/common/datamanagers/__init__.py,sha256=U1cg-KvqbfzN5AnL_tFFrERmPb81w_0MNiTmxObmla4,2062
+nucliadb/common/datamanagers/atomic.py,sha256=e_qyJr6KhTPLOuAGsSbY7AHm5LT9IqER4QULnxLeLyE,3095
 nucliadb/common/datamanagers/cluster.py,sha256=Rc_gWufL-Fx3zQ7WlgCFYBPQD9fPjUvHkyW0QK6hBSg,1451
 nucliadb/common/datamanagers/entities.py,sha256=vQe_xdyqqsII0wmqKWp1yxVTFmB67Tc6bnVxezRUVK0,5383
 nucliadb/common/datamanagers/exceptions.py,sha256=Atz_PP_GGq4jgJaWcAkcRbHBoBaGcC9yJvFteylKtTE,883
 nucliadb/common/datamanagers/fields.py,sha256=nwrPUCA5rXQH8xqf23FIKqyIYb7XRBnCTZxbx9R3riA,2764
 nucliadb/common/datamanagers/kb.py,sha256=zkG3lVbGFFLtjcTlJvJDtTY6S55xdty1nSlwI4xDEQ4,3994
 nucliadb/common/datamanagers/labels.py,sha256=2pN8RrFNTXLitDo44CS3AApjCjbv-2ALkqjwHVR_Mb0,5389
 nucliadb/common/datamanagers/processing.py,sha256=gdCHGzF2LiHOapsg4oaYFYNxACwaCbN1z3kw7iHTuNc,1599
-nucliadb/common/datamanagers/resources.py,sha256=fQ6AjyngQXGVwD6ID-OozD-orYDx06cztWe_yTZCyDg,11922
-nucliadb/common/datamanagers/rollover.py,sha256=oxrvnCWM69MG7liMekwQx8TXuNzwixEKJT_--f5Uf-0,5634
+nucliadb/common/datamanagers/resources.py,sha256=JRHy8PBwDU6TNDpqdmtoAM_Avho4Xj6FGqOHi7RvIaY,11931
+nucliadb/common/datamanagers/rollover.py,sha256=rJk3qWhLRzRYh6wx2Mr8zBX-_Wr1VzL3niLXAoAv15Y,5643
 nucliadb/common/datamanagers/synonyms.py,sha256=f7m3N7SXoYSDWvrNDcAeWoWVAHKI8ByZhnBrZ8rVdec,1548
-nucliadb/common/datamanagers/utils.py,sha256=Ll17Pbn1AunTUcGjrk7F2d1SJ0RBOejdmAAlE1BaNmM,1631
+nucliadb/common/datamanagers/utils.py,sha256=GHm3DcC0ZYzIIZW_T7GnVSCJA3gZ9pCC-xyZwuTyy2M,1923
 nucliadb/common/datamanagers/vectorsets.py,sha256=uEn7FPTkn2UCNZRAmZaqdwoUHjkLW3xQMIjPK9dodqc,3780
 nucliadb/common/http_clients/__init__.py,sha256=cp15ZcFnHvpcu_5-aK2A4uUyvuZVV_MJn4bIXMa20ks,835
 nucliadb/common/http_clients/auth.py,sha256=9A1k-H121W3lAFRl_XxGizcxUw_qw1STDZqJOC2Kpyw,2146
 nucliadb/common/http_clients/exceptions.py,sha256=47Y8OjkaGV_F18G07FpJhOzgWKUIexhlILyuVtICz8s,1100
 nucliadb/common/http_clients/processing.py,sha256=-J5Lxmlk4coboOWvYQ4gc88AIrvHzSV9bzVsedmslCQ,7155
 nucliadb/common/http_clients/pypi.py,sha256=VHIUjwJEJVntVUo_FRoXIo8sLmluy7sa9-iXSITcrMY,1540
 nucliadb/common/http_clients/utils.py,sha256=b7FCaOSf21UVE9OqDhBpWetxP2nguV_gKwBBb9dYifI,1551
 nucliadb/common/maindb/__init__.py,sha256=cp15ZcFnHvpcu_5-aK2A4uUyvuZVV_MJn4bIXMa20ks,835
 nucliadb/common/maindb/driver.py,sha256=ldk1vxo-fx9vmAr8nzqQ0v8Z1fc6K_xzhsYa0QTcdlA,3449
 nucliadb/common/maindb/exceptions.py,sha256=u6ZSQW6jk5QM_IL5XmQ_dF-vZ-JkuWEqZbNJ-S6FG_g,988
 nucliadb/common/maindb/local.py,sha256=E6rWm9QOXOdkk6is6Ut6AiUaW9pRr2UgS_eHyMp2e-s,6769
-nucliadb/common/maindb/pg.py,sha256=OkZOPcpEepDK9FHioLPDgOzOcmnbe4AWhmThyo-Yyjg,8391
+nucliadb/common/maindb/pg.py,sha256=ouQkD8o53LcFvjQr2KSBmZPHFi4dx0r29wOdSizlOfs,8673
 nucliadb/common/maindb/redis.py,sha256=fPvLuDDlxXUiGPsO936SaaopFhdvzD_HGXgSV8TneY4,6053
 nucliadb/common/maindb/tikv.py,sha256=7Jp3YLwmb-ZDb0v6TQupo8xtSeAPLde3th45QH424pc,15314
 nucliadb/common/maindb/utils.py,sha256=LmZL3pbGcUuCK8DFtOuVbM7K_kjhea0ofnuy95sXfzE,4167
 nucliadb/export_import/__init__.py,sha256=y-Is0Bxa8TMV6UiOW0deC_D3U465P65CQ5RjBjIWnow,932
-nucliadb/export_import/datamanager.py,sha256=Ndya8T3X74kGo38UcQB-iPmfvg8HHIQEatKBcGzIl8s,6171
+nucliadb/export_import/datamanager.py,sha256=sNq01FYRsanPbwO0UmPeAdMdb5J914wWo-_YPkCqW_8,6185
 nucliadb/export_import/exceptions.py,sha256=Dw8WqfG4r6MPJc5TPfbjMvCgXXWTcTOecGHRVU1h3kM,1949
 nucliadb/export_import/exporter.py,sha256=boXHZrH6UhnIPttHBjF0lHN0UT0OyQhPC1IEV6wAnwk,7116
 nucliadb/export_import/importer.py,sha256=kiZxziPo8ynQuO41mPmeUhVbV5w7iaFNzxlcNaKPcwA,4258
 nucliadb/export_import/models.py,sha256=VHetyHlofHH5yzcV5q6hN15zGKJTRAu7GOTNveN-tGA,2063
 nucliadb/export_import/tasks.py,sha256=HptUd322AmFDrlXqXcHLD3UYzaeHA54PevbvWxhqZjo,2571
-nucliadb/export_import/utils.py,sha256=EmujsB9DxLPu6cPdHf3lHn5hDSgHhaOo5zjdzErGBPU,19646
+nucliadb/export_import/utils.py,sha256=70CUrMbnKcO1IBF1oV6W7Sm60ybwgneaUklAL6NLq9E,19655
 nucliadb/ingest/__init__.py,sha256=fsw3C38VP50km3R-nHL775LNGPpJ4JxqXJ2Ib1f5SqE,1011
 nucliadb/ingest/app.py,sha256=g51GuMZ9oLuIn8YZ7EKglVlLmu114VSmWzqMCbKtXRE,7277
 nucliadb/ingest/cache.py,sha256=w7jMMzamOmQ7gwXna6Dqm6isRNBVv6l5BTBlTxaYWjE,1005
 nucliadb/ingest/partitions.py,sha256=xhonCO-gqNO-8TlitjcmchVrxCLi-99SyOWvX4va1lE,2484
 nucliadb/ingest/processing.py,sha256=5UWQ8H_rBgDEmRYsiAI5CC9JPA_StMxhzRU8QKSs4bs,19904
 nucliadb/ingest/py.typed,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-nucliadb/ingest/serialize.py,sha256=DM18fONnptJbUqSFQZl4kg33Q8S4GpJUqK432rzSHYU,20277
+nucliadb/ingest/serialize.py,sha256=ROCJZX0rtPx8skltubzN48es3mPSuxrI5mu_CfkdJOw,20291
 nucliadb/ingest/settings.py,sha256=VrOfSSwadDb2LRl0rwlJl5DSiDILj03KSD-n0Jh4yaE,3207
 nucliadb/ingest/utils.py,sha256=dyFEv9V38OlkrQdM8_Xgii3YmbsRqNUoZeYApe39kx0,2314
 nucliadb/ingest/consumer/__init__.py,sha256=cp15ZcFnHvpcu_5-aK2A4uUyvuZVV_MJn4bIXMa20ks,835
 nucliadb/ingest/consumer/auditing.py,sha256=P6a7HgEJVE5WBJuyL7Q2avuqLqQ5QE3VaxoifS3YT3k,6918
 nucliadb/ingest/consumer/consumer.py,sha256=bJgVt1G7RchZrHX-5ykG2uHfGNY_HEjsLE2ZsgAv8HA,12174
-nucliadb/ingest/consumer/materializer.py,sha256=Zoe7DEks14nRvXFSLiBMzF6yKMq1v2TABNtOo0PsT1Q,3945
+nucliadb/ingest/consumer/materializer.py,sha256=yN37qqXLwa4s2PuSNdgJTRKH7mFNhbexj2j7239iNg4,3934
 nucliadb/ingest/consumer/metrics.py,sha256=ji1l_4cKiHJthQd8YNem1ft4iMbw9KThmVvJmLcv3Xg,1075
-nucliadb/ingest/consumer/pull.py,sha256=DQ0_EOjMk4AdYqC1sSX4zVtF4IyrsWT-kaQbAjIs3H4,9543
+nucliadb/ingest/consumer/pull.py,sha256=pvD4Wn73wItyImmnoHADDISKYzI5K0XyUVtVmFJ0GvM,9546
 nucliadb/ingest/consumer/service.py,sha256=873H7IGwpJM7Nhmfzr0RMDSXF3uTSQ2ctkBpWo-IgwU,6871
 nucliadb/ingest/consumer/shard_creator.py,sha256=FmKQSOOC19fsr72qoJ5cbZhnU5t8XnD3nr2TBFXW_js,4331
 nucliadb/ingest/consumer/utils.py,sha256=6zWurmmhOmu80uk-fjUhJB1rrulxArlhaUWFLIY-2Jg,2656
 nucliadb/ingest/fields/__init__.py,sha256=cp15ZcFnHvpcu_5-aK2A4uUyvuZVV_MJn4bIXMa20ks,835
 nucliadb/ingest/fields/base.py,sha256=RBb_dYWwnbvPvsbWReDzJFaWWcisXkC9u7HNNWXlIno,17797
 nucliadb/ingest/fields/conversation.py,sha256=_fuGEnYOBhi9ppRFDJo9e8fgNg9Wn7Xfta69SmadaBk,7047
 nucliadb/ingest/fields/date.py,sha256=jXMWfdCv87oVySDQORXhMZ1Zvpw_aOpcrYAfUSnL3uA,1223
@@ -118,24 +118,24 @@
 nucliadb/ingest/fields/link.py,sha256=kwV3KxSn6bZNYBBHljMEN9qNXPlNv80guoKqQib8ivc,4212
 nucliadb/ingest/fields/text.py,sha256=qMMH76gN--Ag1fPZ1I5G9ZPAi4U0i9jbqlrpYc3cMxg,1319
 nucliadb/ingest/orm/__init__.py,sha256=cp15ZcFnHvpcu_5-aK2A4uUyvuZVV_MJn4bIXMa20ks,835
 nucliadb/ingest/orm/brain.py,sha256=SNn1QRqYApN6PGYMos185r7PEZ6UO-pDbH9Z7A9YhFA,28721
 nucliadb/ingest/orm/broker_message.py,sha256=NBANB8ODLwpU83JNhq5q8G-TiZNSiRKPQGmEsc17r6I,6954
 nucliadb/ingest/orm/entities.py,sha256=q027LfocE-KIqRNC1ZOSrrvt6x9NGrB25TZsOe0SyVk,15758
 nucliadb/ingest/orm/exceptions.py,sha256=Wv10JwvueWrSV0ExqSTFIq_mBXWz4rAelEdc1R5w0Q0,1326
-nucliadb/ingest/orm/knowledgebox.py,sha256=S111iRkfixYXqsqVTcvnos7dch7CF4U8BJaFnDiEnvs,16914
+nucliadb/ingest/orm/knowledgebox.py,sha256=5A2F9RgmHk9S06jzkApQCGTldaz8NZtr4iB2b5a5Uh8,16068
 nucliadb/ingest/orm/metrics.py,sha256=OkwMSPKLZcKba0ZTwtTiIxwBgaLMX5ydhGieKvi2y7E,1096
 nucliadb/ingest/orm/resource.py,sha256=hVqwvdOcOKec91D0Zs8Vs-P_ulTUekQs4XVAELtWhZk,54798
 nucliadb/ingest/orm/utils.py,sha256=A3_EsRw7Nub54qZPF08cv391caxpLQWJURR0_5qP9mU,2685
 nucliadb/ingest/orm/processor/__init__.py,sha256=SqX421XJs_g-sRNSzdv9EyWQGUUceSs6U4LllvUEzCA,27092
-nucliadb/ingest/orm/processor/auditing.py,sha256=M8YLnqEJMCvjYATqIRQS2KpJyhyxxoZvBfpxxppKGOI,5090
-nucliadb/ingest/orm/processor/sequence_manager.py,sha256=Mc9SA_NfzxTwovD5yGiAcdmen4pa-QNdsYcONIWeZPc,1690
+nucliadb/ingest/orm/processor/auditing.py,sha256=2CVeNX9LmJkCAl3SZw0AIt644iVk2tmOmbz5FtPCeUg,5104
+nucliadb/ingest/orm/processor/sequence_manager.py,sha256=uqEphtI1Ir_yk9jRl2gPf7BlzzXWovbARY5MNZSBI_8,1704
 nucliadb/ingest/service/__init__.py,sha256=C_lkkjoHm0hDT2fZjEN4mpwXtU4bWthB-vM5-28-MBM,2057
 nucliadb/ingest/service/exceptions.py,sha256=cp15ZcFnHvpcu_5-aK2A4uUyvuZVV_MJn4bIXMa20ks,835
-nucliadb/ingest/service/writer.py,sha256=UqEyHOOOMOrguybNNpG6G3DYS-zKFtldvo-VTUIA6fM,32883
+nucliadb/ingest/service/writer.py,sha256=UxdwO3TYi72IkXdppmOIGpvp1E6A-hMnm8D9d77mQdU,29886
 nucliadb/ingest/tests/__init__.py,sha256=cp15ZcFnHvpcu_5-aK2A4uUyvuZVV_MJn4bIXMa20ks,835
 nucliadb/ingest/tests/conftest.py,sha256=yTepuxodMXl5vEMTzFfgos9wdRnYfxPffZQDYm3Ej-E,1157
 nucliadb/ingest/tests/fixtures.py,sha256=FA62vAdJ_geh3V4wu3vnVaIE0PIct2f50Chdkr6wfgA,24111
 nucliadb/ingest/tests/vectors.py,sha256=CcNKx-E8LPpyvRyljbmb-Tn_wST9Juw2CBoogWrKiTk,62843
 nucliadb/ingest/tests/integration/__init__.py,sha256=cp15ZcFnHvpcu_5-aK2A4uUyvuZVV_MJn4bIXMa20ks,835
 nucliadb/ingest/tests/integration/consumer/__init__.py,sha256=itSI7dtTwFP55YMX4iK7JzdMHS5CQVUiB1XzQu4UBh8,833
 nucliadb/ingest/tests/integration/consumer/test_auditing.py,sha256=kUUrdaR-iDFjmkip025rpYP5v6x3MIXLWd_n_c8-DXY,2500
@@ -175,32 +175,32 @@
 nucliadb/migrator/migrator.py,sha256=HoxeJWzRK21yzTfowS72USJDCIe2SnVRS66TV_hSvHs,9370
 nucliadb/migrator/models.py,sha256=3PJkL2PGvKgIG0KIBv4H5XCsOVmwWMlRV3m0ntDj10Q,1145
 nucliadb/migrator/settings.py,sha256=jOUX0ZMunCXN8HpF9xXN0aunJYRhu4Vdr_ffjRIqwtw,1144
 nucliadb/migrator/utils.py,sha256=7Y2zJZWB2qM0PcmS5G20g5EEwSdRVeHyR4_1wWNbl6Q,2346
 nucliadb/models/__init__.py,sha256=cp15ZcFnHvpcu_5-aK2A4uUyvuZVV_MJn4bIXMa20ks,835
 nucliadb/models/responses.py,sha256=qnuOoc7TrVSUnpikfTwHLKez47_DE4mSFzpxrwtqijA,1599
 nucliadb/purge/__init__.py,sha256=IHnoGcbASPUQ74ewbPtHiOnUbRXfB92-aDH4sUYALTQ,6041
-nucliadb/purge/orphan_shards.py,sha256=tGFlF7-RLDHv2XPc5J_1lgBvBCM5UjUtUNUmpodGqBc,9364
+nucliadb/purge/orphan_shards.py,sha256=DoKn1OVL0xwGZXpD7w7hx6zrMSseVz2QZU__SLr4EaM,9367
 nucliadb/reader/__init__.py,sha256=TxsAOWhRnz9l8DuFy-Qfv0I5HrzrysaxtAzogg6FQB8,1328
 nucliadb/reader/app.py,sha256=dyvTCnVwXD3gVsk09tUB63N6hL-fS9q_S-AsI3zpFkk,3709
 nucliadb/reader/lifecycle.py,sha256=45NGAjNyi01Emi14Eh5GYBScS5N7yJbs2r1R2P-usSg,1366
 nucliadb/reader/openapi.py,sha256=ZwXYXZPYpxQL68HyWI310YnmMKJMzBUtYe-r9OSbN8I,1031
 nucliadb/reader/py.typed,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 nucliadb/reader/run.py,sha256=AR-iCnON3YVXgI5-KEgg99G4KAPN1BKXDg7nr4dgoDA,1447
 nucliadb/reader/api/__init__.py,sha256=c-UD29C0FVzQDGEvslebDCKtvnyEcAbiDd-3Q_QgGN4,872
 nucliadb/reader/api/models.py,sha256=dBDxZf_LnZFzKIKB_Oaj1B2pccAhrwviJn8KAhxJzwY,2458
 nucliadb/reader/api/v1/__init__.py,sha256=81AhxhYJcni8K_a5apWfL8Dnj4Mf_EznIsFse7jN-gQ,1110
 nucliadb/reader/api/v1/download.py,sha256=GH3lCZ4Wcs1wBu6P0PnLGe-F5QW0z9UVAlvIP_xyXrM,12457
-nucliadb/reader/api/v1/export_import.py,sha256=nBYEwFnKUJYsiXUlbfKIL_jI9Ec5UVZE-2fCbK1rfQk,6459
+nucliadb/reader/api/v1/export_import.py,sha256=x4VBNDFjnlY1nIt5kdq0eZTB_DeRzGzT8T7uB7wUhNU,6448
 nucliadb/reader/api/v1/knowledgebox.py,sha256=Pd71iqTVRgx5u_Gb2LegDTQ3gGTKbVLsAvgcZne5_lM,3641
 nucliadb/reader/api/v1/learning_collector.py,sha256=6XDrfEZffqPrFYGj9TDfWOS1wcy3n9DRu35aH6-2WRA,2099
 nucliadb/reader/api/v1/learning_config.py,sha256=T1bxwsNDnVaeW9lkO4WTO9RHjz6GhYCJwvS1_MNYTes,4472
 nucliadb/reader/api/v1/resource.py,sha256=DaJZh7T0aics-kB7tgSMUU79RFja4D1UBJy7dkxWnEo,13961
 nucliadb/reader/api/v1/router.py,sha256=eyNmEGSP9zHkCIG5XlAXl6sukq950B7gFT3X2peMtIE,1011
-nucliadb/reader/api/v1/services.py,sha256=OSQXi-QcuhS_LDzwzntiLgP16jIYwTn48iypdzYayTQ,12115
+nucliadb/reader/api/v1/services.py,sha256=6B1PJpwMUMOprljAWW1w3d3QlO-FBk2URmzpUpTLGL0,11902
 nucliadb/reader/reader/__init__.py,sha256=cp15ZcFnHvpcu_5-aK2A4uUyvuZVV_MJn4bIXMa20ks,835
 nucliadb/reader/reader/notifications.py,sha256=Hfs2QUguAKeMrH0oaG3e7eDBJSCumNMb1kuXk_DFEKU,7979
 nucliadb/reader/tests/__init__.py,sha256=cp15ZcFnHvpcu_5-aK2A4uUyvuZVV_MJn4bIXMa20ks,835
 nucliadb/reader/tests/conftest.py,sha256=RH5huJVfSZ9cQgzEWC_xViGbXUelZFuHmrOnWb-FpEU,1224
 nucliadb/reader/tests/fixtures.py,sha256=tOBBEksIzJ1sAG6Bodv11_VFstUMkbgtGlYPzon-W54,4355
 nucliadb/reader/tests/test_list_resources.py,sha256=yKsG6MLh4_cB7Yhov0OoBAVCJCXnpuQmT453R1oVQ6Q,2748
 nucliadb/reader/tests/test_reader_file_download.py,sha256=V_wLTRmSlYemSPLOBo3A_jhMBluro2sJiQwSsGGBx6I,10199
@@ -217,38 +217,38 @@
 nucliadb/search/utilities.py,sha256=9SsRDw0rJVXVoLBfF7rBb6q080h-thZc7u8uRcTiBeY,1037
 nucliadb/search/api/__init__.py,sha256=cp15ZcFnHvpcu_5-aK2A4uUyvuZVV_MJn4bIXMa20ks,835
 nucliadb/search/api/v1/__init__.py,sha256=FR4pbt1XyWQAS3TAiAhvOQb0kWSsZpmzL87JJMcAoMc,1298
 nucliadb/search/api/v1/ask.py,sha256=TcVSWwF9gcRlCCm3l3TUc8oUP2ruTWjgVhsG3tFKTdQ,3435
 nucliadb/search/api/v1/chat.py,sha256=N6EIh3MxwkUfZ0guXnrlMm4addVkw0tBCnZ7N1qpWOw,9514
 nucliadb/search/api/v1/feedback.py,sha256=SFXKzqgn31TDudUYPmp8845EBwLSJtWImG-7tTc9WQM,2668
 nucliadb/search/api/v1/find.py,sha256=fIm4hrCWCllFiPlTmMMqBCOaX9lo9py4q_4jUSdnQko,8795
-nucliadb/search/api/v1/knowledgebox.py,sha256=hQ0wdBlHJVTwiRZgVCeNVwW_6f2bay88Hs9JMHgnx9M,6938
+nucliadb/search/api/v1/knowledgebox.py,sha256=IQeDb1rPxNqhC7jLWbASdOF6WeJR5KEb6UT7TuPOTpQ,6941
 nucliadb/search/api/v1/predict_proxy.py,sha256=QrGzo0hKjtmyGZ6pjlJHYAh4hxwVUIOTcVcerRCw7eE,3047
 nucliadb/search/api/v1/router.py,sha256=mtT07rBZcVfpa49doaw9b1tj3sdi3qLH0gn9Io6NYM0,988
 nucliadb/search/api/v1/search.py,sha256=e693TQHuczf322zVEt0yfepeM55yXOCtMTddKJj860M,19262
 nucliadb/search/api/v1/suggest.py,sha256=3Mz34gxxTtyWG45CpfXQFJ54WS7cHUVwwz7oAtmtM28,5970
 nucliadb/search/api/v1/summarize.py,sha256=VAHJvE6V3xUgEBfqNKhgoxmDqCvh30RnrEIBVhMcNLU,2499
 nucliadb/search/api/v1/utils.py,sha256=5Ve-frn7LAE2jqAgB85F8RSeqxDlyA08--gS-AdOLS4,1434
 nucliadb/search/api/v1/resource/__init__.py,sha256=cp15ZcFnHvpcu_5-aK2A4uUyvuZVV_MJn4bIXMa20ks,835
-nucliadb/search/api/v1/resource/ask.py,sha256=ATrkB6SpcKvz2orsgdQdk50fMT5AhfGSJzknKndHktw,3866
-nucliadb/search/api/v1/resource/chat.py,sha256=J-lfvcMPCv-KuCw4KBqnAnIRP8TKuGEuTjww6hzdCas,5863
+nucliadb/search/api/v1/resource/ask.py,sha256=P-qD3UCc4qbH_1NhPC1bpVdF2J_Q-ItMUBvifyL105o,3869
+nucliadb/search/api/v1/resource/chat.py,sha256=NkJAkJuNyIcNsOc8wsbCsMf-NIVxDri01NSrkaK1Ofs,5866
 nucliadb/search/api/v1/resource/search.py,sha256=C6Do2x0dq0lUyUg67hFYxHMJ8xtaAtJj5yPnmrGTONo,5303
 nucliadb/search/requesters/__init__.py,sha256=itSI7dtTwFP55YMX4iK7JzdMHS5CQVUiB1XzQu4UBh8,833
 nucliadb/search/requesters/utils.py,sha256=P2OIPXs9klQ-Nnu7TjS3rVEp91Q3dCtf92mQa2StXdw,9111
 nucliadb/search/search/__init__.py,sha256=cp15ZcFnHvpcu_5-aK2A4uUyvuZVV_MJn4bIXMa20ks,835
 nucliadb/search/search/cache.py,sha256=86WwnknDYI00bd-kFf5MhN8TVFS2tfHzgobUHv_fAIA,2746
 nucliadb/search/search/exceptions.py,sha256=mbToQ-ghrv8ukLEv8S_-EZrgweWaIZZ5SIpoeuGDk6s,1154
 nucliadb/search/search/fetch.py,sha256=6S6s2s0JEP2QADDesbeN3XYPvTquMsTz9l0FKqQtSKU,5465
 nucliadb/search/search/filters.py,sha256=HpTpaDjKmUZWkp5xFFqKHz3TYdKEVBk4jWb2ssIYa5g,6513
 nucliadb/search/search/find.py,sha256=_cGdIfSqpaxm01SqTbcQCQJtadeiL71HB4zEIBj1dM4,4612
 nucliadb/search/search/find_merge.py,sha256=vhq14MFE7N9-9SNlg66LNUr6YAhR9cW22oDpmjvQhL0,17152
 nucliadb/search/search/merge.py,sha256=-srmB1gZEuMa9c2_hLTD1ihjJwDhdB6wnp9b7ljxuIM,21282
 nucliadb/search/search/metrics.py,sha256=4xQm4Q0_-R1bgMtnrbm-YaClEFR8HE6wDk9lunCrhjo,1130
 nucliadb/search/search/paragraphs.py,sha256=8TTii45JvQ7SXsV9Z9ipt5QpYk7ux6PnlOkjKPfYz4A,8698
-nucliadb/search/search/predict_proxy.py,sha256=aOq1AzXkUdHtEmXsec07ffuMKGjlMu-NaUxb_IKme6U,3026
+nucliadb/search/search/predict_proxy.py,sha256=xBlh6kjuQpWRq7KsBx4pEl2PtnwljjQIiYMaTWpcCSA,3015
 nucliadb/search/search/query.py,sha256=U5GL6z6sjViFcRiQfk_lRZizC3AM0EjkSWh3OY9wQxA,31093
 nucliadb/search/search/shards.py,sha256=0p_BWLEVrK87htqhavZ2ixA2l253FPQnre3RpThtZco,3018
 nucliadb/search/search/summarize.py,sha256=bjncFFBv1R9g4OyhQSlGHFq5cJ8UvR8KrMgeKc-1AMU,5101
 nucliadb/search/search/utils.py,sha256=Gzjr9rFdwRfOgyDzX1Slz8DbcXLvavo0124S8II9omw,2438
 nucliadb/search/search/chat/__init__.py,sha256=cp15ZcFnHvpcu_5-aK2A4uUyvuZVV_MJn4bIXMa20ks,835
 nucliadb/search/search/chat/ask.py,sha256=4yLOqeIJDKt5zVl78knppDqfgeMqZjRUEIiEbQxfDkM,16676
 nucliadb/search/search/chat/images.py,sha256=AjPgCJaCzu19ruUJcEVaG_bEUmqzB65EH0mduMbkzAE,2058
@@ -281,15 +281,15 @@
 nucliadb/search/tests/unit/search/test_query.py,sha256=W8JJqgpYc6r3ap9Yw2ZzVxlrVZDxTMKtLAuMPSK1mOw,5121
 nucliadb/search/tests/unit/search/requesters/__init__.py,sha256=itSI7dtTwFP55YMX4iK7JzdMHS5CQVUiB1XzQu4UBh8,833
 nucliadb/search/tests/unit/search/requesters/test_utils.py,sha256=aBMPou4VLx1UCcDQ_eF3ufn_fJJHOQ40SphKx9VXCDY,6455
 nucliadb/search/tests/unit/search/search/__init__.py,sha256=cp15ZcFnHvpcu_5-aK2A4uUyvuZVV_MJn4bIXMa20ks,835
 nucliadb/search/tests/unit/search/search/test_shards.py,sha256=XvGXSWf8g1Ap6dZsAdSidRjDIPlPRcTTGDtHVAJCEGo,1759
 nucliadb/search/tests/unit/search/search/test_utils.py,sha256=7JjO0NXJlv4tRtCYYU60SoxgVa3K6xNTDWGub5Mrwi4,2511
 nucliadb/standalone/__init__.py,sha256=cp15ZcFnHvpcu_5-aK2A4uUyvuZVV_MJn4bIXMa20ks,835
-nucliadb/standalone/api_router.py,sha256=DtB9uoMmT8NWjqZy-iEolHkM6sn-KzrykWVEmeTKM80,6746
+nucliadb/standalone/api_router.py,sha256=kCLzNcLi4mUWpgIhaTDZuTkumm9qlitC_IFRvuujHkA,6749
 nucliadb/standalone/app.py,sha256=AVojB5tQE3K2I9hPxHgd06At2ofyclJti4JS1g5_Y5c,5763
 nucliadb/standalone/auth.py,sha256=bglXXYH7F3TWR5d8qrJq0VgVYb63mQCJJU4vQy8hMdQ,7800
 nucliadb/standalone/config.py,sha256=Np6pIpOY7Yi5gLf73yLcdxSaMwZtJwWVlPzcEcCR4m8,5313
 nucliadb/standalone/introspect.py,sha256=KJ91JYGaxMJ62lNe6Ji9NFfyEyks6lVJcGTmqfPjtp0,6986
 nucliadb/standalone/lifecycle.py,sha256=6cCkiXwom7LppzKoG_vRuW5Ubw_YsLuVChHlCqnhts8,2488
 nucliadb/standalone/migrations.py,sha256=wmdxORbqIzs7Zo4240sssVjFt3csCWRyTntJVbVvKec,1980
 nucliadb/standalone/purge.py,sha256=FzyO3P3wIcBrvg3Apknim_jcol3Ku2Zi_YTHdaELwxU,1322
@@ -340,15 +340,15 @@
 nucliadb/tests/unit/test_purge.py,sha256=wxCRrBVAIs4tN1hQwUfbsIhkUV-r9CKE_wgmIyWF_kA,3649
 nucliadb/tests/unit/common/__init__.py,sha256=cp15ZcFnHvpcu_5-aK2A4uUyvuZVV_MJn4bIXMa20ks,835
 nucliadb/tests/unit/common/test_context.py,sha256=GmZlJtXsX4TTNLb49q_SnH0jADgBMSrGKgrc5zOyYH8,1268
 nucliadb/tests/unit/common/cluster/__init__.py,sha256=cp15ZcFnHvpcu_5-aK2A4uUyvuZVV_MJn4bIXMa20ks,835
 nucliadb/tests/unit/common/cluster/test_cluster.py,sha256=lO3IXRhXBsVQ7swHhPxKOCusnRsDyksIOSuvWOgDMM0,12240
 nucliadb/tests/unit/common/cluster/test_kb_shard_manager.py,sha256=N6aLQI3ZUwLdwLsMJ2hhnIAyGYTODLWYjJILQClaxLs,5387
 nucliadb/tests/unit/common/cluster/test_rebalance.py,sha256=L4T3mhz-Yj8UZGqeuY5nZ66QRdL3_4PNGF1NeL-kBkM,1428
-nucliadb/tests/unit/common/cluster/test_rollover.py,sha256=j0C-tKH9jwRThiN2DGmyRmskhag4C9pVZ7-0uATUQFI,9465
+nucliadb/tests/unit/common/cluster/test_rollover.py,sha256=jWc8JTlLAVAZlmI6A4K7jF1ctPEcvm6_95c8S31Gl2A,9609
 nucliadb/tests/unit/common/cluster/discovery/__init__.py,sha256=cp15ZcFnHvpcu_5-aK2A4uUyvuZVV_MJn4bIXMa20ks,835
 nucliadb/tests/unit/common/cluster/discovery/test_k8s.py,sha256=8rZ5yWiEXgLrMnWH4iX8Zrbw1upVqyM1EMFM2G0yOLo,5627
 nucliadb/tests/unit/common/cluster/standalone/__init__.py,sha256=itSI7dtTwFP55YMX4iK7JzdMHS5CQVUiB1XzQu4UBh8,833
 nucliadb/tests/unit/common/cluster/standalone/test_service.py,sha256=sg0wWlBZNtLo9pA3rIIv6BAbkRcXsgDV0JreCgjnTHo,3761
 nucliadb/tests/unit/common/cluster/standalone/test_utils.py,sha256=2UHgo366zBqgfm-o7GEzdG9PwzorCmfxxI9styaxo2c,2136
 nucliadb/tests/unit/common/maindb/__init__.py,sha256=itSI7dtTwFP55YMX4iK7JzdMHS5CQVUiB1XzQu4UBh8,833
 nucliadb/tests/unit/common/maindb/test_driver.py,sha256=Qx8iydiKuCT1U7ZI5L2N4bHCmAmtIArc86axcp5ApfA,3579
@@ -374,19 +374,19 @@
 nucliadb/train/app.py,sha256=3AucXVUiDFueskmw85nO22fu9YjRyZIU1yhGlh0jVOE,3530
 nucliadb/train/generator.py,sha256=zmoffpYvc6u3gk6cPXKcKPf0KKpMibu6xWnwDs143bQ,3800
 nucliadb/train/lifecycle.py,sha256=ZLqCl_IjFimon9pl3OJyF2UM4Jky_xsHuqilnrJj1as,1698
 nucliadb/train/models.py,sha256=BmgmMjDsu_1Ih5JDAqo6whhume90q0ASJcDP9dkMQm8,1198
 nucliadb/train/nodes.py,sha256=uYQFDh-PuL5_TmKcUjW6tZclag2azgefox4TWfeDvi4,5776
 nucliadb/train/py.typed,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 nucliadb/train/run.py,sha256=evz6CKVfJOzkbHMoaYz2mTMlKjJnNOb1O8zBBWMpeBw,1400
-nucliadb/train/servicer.py,sha256=b889xt0XiTOVpAPjK0AElJW3gJ7aV-55TQFbxdQe0MI,5926
+nucliadb/train/servicer.py,sha256=iMG7ZWDhbiBkJ35d0ybmbJ7pyWB1JSrP1Z33YkVhEw4,5750
 nucliadb/train/settings.py,sha256=eXe87TjqtGTa-bCKRPDIWdyb7qsaUW3VbLXV-zGBQZk,1415
 nucliadb/train/types.py,sha256=M3olA6vBosVs7L5QpzlxiFhuF3_vQhSkdlgClQzXjaQ,1496
 nucliadb/train/upload.py,sha256=Sz8KDXqFMD8reFw-8mb11il7Ab4onKcH0MPsZ1AbYUk,3265
-nucliadb/train/uploader.py,sha256=JEdZ6ozdFuKC_DmimljKnnH0gz2Nu-HxMFzjLa3gmkg,6420
+nucliadb/train/uploader.py,sha256=RFuBa7yRbahISkAz5I6ChNDXzVxaSuFIUGFeMVyJoQc,6395
 nucliadb/train/utils.py,sha256=Xoz7LjSWRfFNSHyZF-eK9DmWf9sgjyJXdYPppc3BE_c,3179
 nucliadb/train/api/__init__.py,sha256=cp15ZcFnHvpcu_5-aK2A4uUyvuZVV_MJn4bIXMa20ks,835
 nucliadb/train/api/utils.py,sha256=mvxHr3A3CCwvFXJyppm8KIi8yOwGxXhK-ADyDbZOuVo,1479
 nucliadb/train/api/v1/__init__.py,sha256=P4vCIv93r_Cq1WFDDNjy_Wg7zBkzx0S4euXwfPy1LA4,928
 nucliadb/train/api/v1/check.py,sha256=VLJRvkHG8fQGnIKu27tGTY1c7HBDrYQSn3tbIvnYmms,2071
 nucliadb/train/api/v1/router.py,sha256=ukdxn5q1oMar6NSPobgJczWsSxLCHw6DYKlb3zwCiSo,910
 nucliadb/train/api/v1/shards.py,sha256=4osVrNisomtTOJqY96yqn80S-BFZxFVbuDldOHZ9Wwo,1908
@@ -398,35 +398,35 @@
 nucliadb/train/generators/paragraph_streaming.py,sha256=U4d_vL_sOloFIM95UgDsWZd6tqEiWluyMRqOiFRhWGY,3590
 nucliadb/train/generators/question_answer_streaming.py,sha256=ME-rKB02xZ2JNbNEaBz8oN09FaEN_zbTQS-oOl33J5c,5372
 nucliadb/train/generators/sentence_classifier.py,sha256=K1UBebwyPngDy4pWjxZ8tTZyOo3M5WlizBLJ0DPMP1s,5160
 nucliadb/train/generators/token_classifier.py,sha256=G7pE49c63P7bQJGSnTxz_GlMYhlfebO-pjz32l8WeB4,10446
 nucliadb/train/generators/utils.py,sha256=I-P_KV4HdILOpaPK3cdKP0iT2QzBfSNvuMdewyiIqpg,3877
 nucliadb/train/tests/__init__.py,sha256=cp15ZcFnHvpcu_5-aK2A4uUyvuZVV_MJn4bIXMa20ks,835
 nucliadb/train/tests/conftest.py,sha256=8FfoA1iXscmNtHRXWDEGhMxLLqfjx3JUX3xrTaYXIAE,1125
-nucliadb/train/tests/fixtures.py,sha256=jUdgJIYaakSVfOQP2vDHA-SyGeh6Cl-Aml_Q9tnCmj4,11063
-nucliadb/train/tests/test_field_classification.py,sha256=rFhJKVJsPGLFTKMKuHMA9vWwtLrHixlC3DNg66Zx3vM,4598
+nucliadb/train/tests/fixtures.py,sha256=KE5VRainkPshQR1nWoLrBjWTVAKgZudMQiI4wE-gRp0,10995
+nucliadb/train/tests/test_field_classification.py,sha256=hm4pS8baWnyZrWu5uJdcLUKpu-WP4AiraE_VkXSSqPg,4571
 nucliadb/train/tests/test_get_entities.py,sha256=ndcEemTcITB70X_GxSIkUiAoNOnpTamfyPaXVtXmgKQ,2729
 nucliadb/train/tests/test_get_info.py,sha256=uWKFC8uDXsmdzUp0xgNpEEuf5Ge9dNPE5CSfdZSDz_o,1660
-nucliadb/train/tests/test_get_ontology.py,sha256=Xjr-eIYQLzNkqFU3nwANmDi4fwY09VymdikC3ibgM8A,1382
+nucliadb/train/tests/test_get_ontology.py,sha256=Gz8J0q20HeFEe7G81nnMIlZxuRamDBqdCmilPYCiHsk,1379
 nucliadb/train/tests/test_get_ontology_count.py,sha256=hyarvQOw5PyeYVJ7Z6v4I1Yagi0PwrEiIs615tsM4Z8,2201
 nucliadb/train/tests/test_image_classification.py,sha256=wegtn1V8ZS4HAkiQzOiQ-xs_W42DxG2xvB1NAofY7nQ,7669
 nucliadb/train/tests/test_list_fields.py,sha256=V6YS2ao09AiheI6GKaC9GVLUG_ypf-WrvId_mRdBJB8,1416
 nucliadb/train/tests/test_list_paragraphs.py,sha256=fvDh-vvgTj-XonTS8t9CDq0eDGgNl8iWw3E9OBmGK7c,2944
 nucliadb/train/tests/test_list_resources.py,sha256=QkrsRzRHAWHyJHEtSsrr0xOtrALtiUasSvoPHcjHsCc,1423
 nucliadb/train/tests/test_list_sentences.py,sha256=__4bq6Jmig-wr2LJQHjRZ8QxywNgc4EbDDtzeN0Gt7k,2947
 nucliadb/train/tests/test_paragraph_classification.py,sha256=_d2z8hxGBcdszBc4vIg-WyEnBR_QJQjhcVGyvsHBcuc,4645
 nucliadb/train/tests/test_paragraph_streaming.py,sha256=CMwGEDBQ3iwf7pldZfOBphFSYCvTLKPd1dDHgoHtslQ,4320
 nucliadb/train/tests/test_question_answer_streaming.py,sha256=URtFXd6sEy72Q1By5LtcwIPT5S_yQ0Ip8AjJPILUeDU,8751
 nucliadb/train/tests/test_sentence_classification.py,sha256=6cex9xJN1AGZhsVD1jG2JKYgZEmo09picNJkUrLjDDQ,5051
 nucliadb/train/tests/test_token_classification.py,sha256=fBS70sCKFWBjcaUDny9fg8qZgsQ5VtKBTPENFTgkHrk,5583
 nucliadb/train/tests/utils.py,sha256=J5UZoCz4Ss5b6SmZuyC7jJQlomQE8mDQ8E2OdYEV-gA,3324
 nucliadb/writer/__init__.py,sha256=HkfMuQR3CbbPU3g-A85Ibt8iwSTTADhLc0-pi3F3hvk,1328
 nucliadb/writer/app.py,sha256=Q55CmGR85wG5pjf_Ro-73QVWc7_wMpIt69xJSZ0kjCQ,4268
-nucliadb/writer/back_pressure.py,sha256=0aM0VRVpaBXArtFPekC8iCnIATwroQkFcYmN3OERgVA,19483
-nucliadb/writer/exceptions.py,sha256=2dMvuoF68v3BZuyzaBEsbG6gusQqwLFcn47qm1zNdTc,972
+nucliadb/writer/back_pressure.py,sha256=DWAlsdTJzWXCV1HuO6YisO-UWoGsmlNETxQqp4Y0qR0,19472
+nucliadb/writer/exceptions.py,sha256=-Z7LW--eid7PNeKFuzo9kAlbLEBMUosxE-UVIgGD3SA,929
 nucliadb/writer/lifecycle.py,sha256=gF9it0w98uBGCwzjs72e8mGi6H-qv_XAa2GGNBTOEDY,1953
 nucliadb/writer/openapi.py,sha256=thqCO1ht_RJgOkXs-aIsv8aXJrU5z8wo2n05l2_LqMs,1032
 nucliadb/writer/py.typed,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 nucliadb/writer/run.py,sha256=euVZ_rtHDXs-O1kB-Pt1Id8eft9CYVpWH3zJzEoEqls,1448
 nucliadb/writer/settings.py,sha256=EGY6ZKg-BTKD0xPRIam7EN_FxAQEU_eb5ywNCQOQEg0,3103
 nucliadb/writer/utilities.py,sha256=AZ5qEny1Xm0IDsFtH13oJa2usvJZK8f0FdgF1LrnLCw,1036
 nucliadb/writer/api/__init__.py,sha256=cp15ZcFnHvpcu_5-aK2A4uUyvuZVV_MJn4bIXMa20ks,835
@@ -434,28 +434,28 @@
 nucliadb/writer/api/v1/__init__.py,sha256=FVn7N9VJ6bsEoy4TRnkclr4Umd5hECiwPXVqRnJ8BME,1095
 nucliadb/writer/api/v1/export_import.py,sha256=9Gqxq1EAPOXCX80F2G7s0UVkvMV1Kgwo66o5sHn2KGY,6421
 nucliadb/writer/api/v1/field.py,sha256=Yi0F1IUin2TaQXyh9QDSwwzrqfjKw7nrAVbfnhl7z3o,24482
 nucliadb/writer/api/v1/knowledgebox.py,sha256=624Uv5_UHacWLv1p2YoMAR7oFPUlM9VgmiwsuJezqWk,5248
 nucliadb/writer/api/v1/learning_config.py,sha256=GaYaagjBrVG9ZxrWQyVQfqGMQV3tAJjqJ5CStaKhktU,2058
 nucliadb/writer/api/v1/resource.py,sha256=-pqZi7riP-EF-eGJsttko5PVA_-0I1oE5SuIxORTKB8,18628
 nucliadb/writer/api/v1/router.py,sha256=RjuoWLpZer6Kl2BW_wznpNo6XL3BOpdTGqXZCn3QrrQ,1034
-nucliadb/writer/api/v1/services.py,sha256=uK6XZnbw3zGT83SzPMFgQPLLU4IFrT3g-0_VOj2DXbA,10216
+nucliadb/writer/api/v1/services.py,sha256=YRmaNsQ1u8H9_j4177tbiOT3vlTySYXI_YIF66BjLfs,10485
 nucliadb/writer/api/v1/upload.py,sha256=6TZpT-_g4MdnKGxE6vWs0065HvwZjDPXFdUpEXgUlZ8,30985
 nucliadb/writer/layouts/__init__.py,sha256=Siod9W963CG5gJa20GSTw9VemAFgsMmJDbUspbrYAyE,1612
 nucliadb/writer/layouts/v1.py,sha256=Yc2idmfrpCS8js_XJByNWA_tmt2WeKoWvidLHoTPXoo,2115
 nucliadb/writer/resource/__init__.py,sha256=cp15ZcFnHvpcu_5-aK2A4uUyvuZVV_MJn4bIXMa20ks,835
 nucliadb/writer/resource/audit.py,sha256=SXPu_hdNBlm9uCSl666UQL7hzMx9zYVbBLT_U7ro8Gs,1425
 nucliadb/writer/resource/basic.py,sha256=eSWW6u6U3e0KjjdFwp9YQokojoDepl5vmJfbE2MQACM,10968
 nucliadb/writer/resource/field.py,sha256=woPN-1bIC6eMXtvggMuvcVwbNAGLpS7GIz8pkO9UNz4,16740
 nucliadb/writer/resource/origin.py,sha256=3Y2zVtG_v0U6uMbDhW9Yl7KKHKt5V3T5_v3iCpqdBEk,2022
 nucliadb/writer/tests/__init__.py,sha256=cp15ZcFnHvpcu_5-aK2A4uUyvuZVV_MJn4bIXMa20ks,835
 nucliadb/writer/tests/conftest.py,sha256=bmFKnuaqRqMCjtTp6c4V4R-qF59OPu0gW8-hp1TXFwk,1200
 nucliadb/writer/tests/fixtures.py,sha256=Ni66Iq-A6W8qqa6V6PwSzDq2BD9IINXlGexilVaDzPU,5971
 nucliadb/writer/tests/test_fields.py,sha256=fbzN0Bgu8HOLAqqYXO15JIqXN1bxr7mTTCTUuYhG85c,15472
-nucliadb/writer/tests/test_files.py,sha256=V-YB-ceSVCMmiVuXeH7BKl00GmC7t0ZyjUPAKqMr048,25999
+nucliadb/writer/tests/test_files.py,sha256=BsXeoGXV1bCw3CCnFr1lq7CduNVtbg9e-Jm3LRhDulY,25988
 nucliadb/writer/tests/test_knowledgebox.py,sha256=KPUGr4TsmHXSTfte40rY18ANUHaUYs_TD4DXCIlawt8,1729
 nucliadb/writer/tests/test_reprocess_file_field.py,sha256=MClPDagdcnpemIRpE_W7OeWTNRnYYK1xUm_BJOwRKdI,4400
 nucliadb/writer/tests/test_resources.py,sha256=Oqbby4QuiDZW1JLkIB68g6PK6gIt78KUjQnLdrySSGE,16857
 nucliadb/writer/tests/test_service.py,sha256=bfV1qQVL5fq6w9NznllqLN8LS3hxRYsBjT2bs_rHWV4,5120
 nucliadb/writer/tests/test_tus.py,sha256=Dy98EhBCcmDSXlNfoPiQnLElTi1KEdybjVk8MtIAlJw,6054
 nucliadb/writer/tests/utils.py,sha256=eSyyTCMERC-EzeBrBAurSIZCpqgH67wc1wHZ1KjO1DM,1287
 nucliadb/writer/tus/__init__.py,sha256=J6d-4FHwJ_2DxYGWRtX2RBoPETW-fmBQp-sgVChaOJY,5226
@@ -463,13 +463,13 @@
 nucliadb/writer/tus/exceptions.py,sha256=CmxYKnHXpXug25DYV4SpVAU47SGD-NVBd7pNTRbWHyk,2186
 nucliadb/writer/tus/gcs.py,sha256=WykJZicWKRYkVB5_Fkb_1cVLovAk86IVkEn1VgEDufc,14527
 nucliadb/writer/tus/local.py,sha256=lIOoGaylnsxPBYGskcmKSHv7MsvwIYFS4soDLey_KSs,5849
 nucliadb/writer/tus/pg.py,sha256=JUK_xKsyNcKAvWOch8gUMTc_e1evI_3aC6-Y5gMk2jw,4367
 nucliadb/writer/tus/s3.py,sha256=a9mfPtjBW3QaTYY2r6P7u_Y13V6mBefZjWgV4juZzgE,9069
 nucliadb/writer/tus/storage.py,sha256=8iBOjWIcY6PawQq_rmSiBKi0Gl6J6Q5ad6L-9nLCcJ4,4734
 nucliadb/writer/tus/utils.py,sha256=MSdVbRsRSZVdkaum69_0wku7X3p5wlZf4nr6E0GMKbw,2556
-nucliadb-4.0.3.post562.dist-info/METADATA,sha256=mPLIfu8KrVMLP8YC8FOi4kOQ-ikJHlok129GEzE-8C8,4474
-nucliadb-4.0.3.post562.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
-nucliadb-4.0.3.post562.dist-info/entry_points.txt,sha256=XqGfgFDuY3zXQc8ewXM2TRVjTModIq851zOsgrmaXx4,1268
-nucliadb-4.0.3.post562.dist-info/top_level.txt,sha256=hwYhTVnX7jkQ9gJCkVrbqEG1M4lT2F_iPQND1fCzF80,20
-nucliadb-4.0.3.post562.dist-info/zip-safe,sha256=AbpHGcgLb-kRsJGnwFEktk7uzpZOCcBY74-YBdrKVGs,1
-nucliadb-4.0.3.post562.dist-info/RECORD,,
+nucliadb-4.0.3.post563.dist-info/METADATA,sha256=IIls1efPFYVQ9yn47WsxRfBJKp6gHI25Avw5gPzVT44,4474
+nucliadb-4.0.3.post563.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
+nucliadb-4.0.3.post563.dist-info/entry_points.txt,sha256=XqGfgFDuY3zXQc8ewXM2TRVjTModIq851zOsgrmaXx4,1268
+nucliadb-4.0.3.post563.dist-info/top_level.txt,sha256=hwYhTVnX7jkQ9gJCkVrbqEG1M4lT2F_iPQND1fCzF80,20
+nucliadb-4.0.3.post563.dist-info/zip-safe,sha256=AbpHGcgLb-kRsJGnwFEktk7uzpZOCcBY74-YBdrKVGs,1
+nucliadb-4.0.3.post563.dist-info/RECORD,,
```

