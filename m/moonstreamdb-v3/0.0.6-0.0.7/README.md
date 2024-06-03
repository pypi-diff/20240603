# Comparing `tmp/moonstreamdb-v3-0.0.6.tar.gz` & `tmp/moonstreamdb-v3-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "moonstreamdb-v3-0.0.6.tar", last modified: Tue May 28 14:01:32 2024, max compression
+gzip compressed data, was "moonstreamdb-v3-0.0.7.tar", last modified: Mon Jun  3 14:59:06 2024, max compression
```

## Comparing `moonstreamdb-v3-0.0.6.tar` & `moonstreamdb-v3-0.0.7.tar`

### file list

```diff
@@ -1,33 +1,35 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 14:01:32.207919 moonstreamdb-v3-0.0.6/
--rw-r--r--   0 runner    (1001) docker     (127)      862 2024-05-28 14:01:32.207919 moonstreamdb-v3-0.0.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-28 14:01:16.000000 moonstreamdb-v3-0.0.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 14:01:32.203920 moonstreamdb-v3-0.0.6/moonstreamdb_v3.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      862 2024-05-28 14:01:31.000000 moonstreamdb-v3-0.0.6/moonstreamdb_v3.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1001 2024-05-28 14:01:32.000000 moonstreamdb-v3-0.0.6/moonstreamdb_v3.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-28 14:01:31.000000 moonstreamdb-v3-0.0.6/moonstreamdb_v3.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-28 14:01:23.000000 moonstreamdb-v3-0.0.6/moonstreamdb_v3.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      103 2024-05-28 14:01:31.000000 moonstreamdb-v3-0.0.6/moonstreamdb_v3.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-28 14:01:31.000000 moonstreamdb-v3-0.0.6/moonstreamdb_v3.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 14:01:32.203920 moonstreamdb-v3-0.0.6/moonstreamdbv3/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 14:01:16.000000 moonstreamdb-v3-0.0.6/moonstreamdbv3/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 14:01:32.203920 moonstreamdb-v3-0.0.6/moonstreamdbv3/alembic/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 14:01:16.000000 moonstreamdb-v3-0.0.6/moonstreamdbv3/alembic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3722 2024-05-28 14:01:16.000000 moonstreamdb-v3-0.0.6/moonstreamdbv3/alembic/env.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 14:01:32.207919 moonstreamdb-v3-0.0.6/moonstreamdbv3/alembic/versions/
--rw-r--r--   0 runner    (1001) docker     (127)    49749 2024-05-28 14:01:16.000000 moonstreamdb-v3-0.0.6/moonstreamdbv3/alembic/versions/994e614b5500_tables_initial_generation.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 14:01:16.000000 moonstreamdb-v3-0.0.6/moonstreamdbv3/alembic/versions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    15836 2024-05-28 14:01:16.000000 moonstreamdb-v3-0.0.6/moonstreamdbv3/alembic/versions/d2ceff33be47_tx_call_and_event_unique_indexes.py
--rw-r--r--   0 runner    (1001) docker     (127)    13956 2024-05-28 14:01:16.000000 moonstreamdb-v3-0.0.6/moonstreamdbv3/alembic/versions/e9e1b43f49e1_amoy_blast_and_apex_blockchains.py
--rw-r--r--   0 runner    (1001) docker     (127)     4109 2024-05-28 14:01:16.000000 moonstreamdb-v3-0.0.6/moonstreamdbv3/alembic/versions/e9f640a2b45b_arbitrum_one_blockchain.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 14:01:32.207919 moonstreamdb-v3-0.0.6/moonstreamdbv3/alembic_indexes/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 14:01:16.000000 moonstreamdb-v3-0.0.6/moonstreamdbv3/alembic_indexes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3117 2024-05-28 14:01:16.000000 moonstreamdb-v3-0.0.6/moonstreamdbv3/alembic_indexes/env.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 14:01:32.207919 moonstreamdb-v3-0.0.6/moonstreamdbv3/alembic_indexes/versions/
--rw-r--r--   0 runner    (1001) docker     (127)    16088 2024-05-28 14:01:16.000000 moonstreamdb-v3-0.0.6/moonstreamdbv3/alembic_indexes/versions/0ea24314c181_init_v3_index.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 14:01:16.000000 moonstreamdb-v3-0.0.6/moonstreamdbv3/alembic_indexes/versions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4548 2024-05-28 14:01:16.000000 moonstreamdb-v3-0.0.6/moonstreamdbv3/db.py
--rw-r--r--   0 runner    (1001) docker     (127)    21409 2024-05-28 14:01:16.000000 moonstreamdb-v3-0.0.6/moonstreamdbv3/models.py
--rw-r--r--   0 runner    (1001) docker     (127)     6683 2024-05-28 14:01:16.000000 moonstreamdb-v3-0.0.6/moonstreamdbv3/models_indexes.py
--rw-r--r--   0 runner    (1001) docker     (127)      234 2024-05-28 14:01:16.000000 moonstreamdb-v3-0.0.6/moonstreamdbv3/version.py
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-28 14:01:32.207919 moonstreamdb-v3-0.0.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1360 2024-05-28 14:01:16.000000 moonstreamdb-v3-0.0.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 14:59:06.568534 moonstreamdb-v3-0.0.7/
+-rw-r--r--   0 runner    (1001) docker     (127)      862 2024-06-03 14:59:06.568534 moonstreamdb-v3-0.0.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-06-03 14:58:44.000000 moonstreamdb-v3-0.0.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 14:59:06.564534 moonstreamdb-v3-0.0.7/moonstreamdb_v3.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      862 2024-06-03 14:59:05.000000 moonstreamdb-v3-0.0.7/moonstreamdb_v3.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1183 2024-06-03 14:59:06.000000 moonstreamdb-v3-0.0.7/moonstreamdb_v3.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-03 14:59:05.000000 moonstreamdb-v3-0.0.7/moonstreamdb_v3.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-03 14:58:55.000000 moonstreamdb-v3-0.0.7/moonstreamdb_v3.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      103 2024-06-03 14:59:05.000000 moonstreamdb-v3-0.0.7/moonstreamdb_v3.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-06-03 14:59:05.000000 moonstreamdb-v3-0.0.7/moonstreamdb_v3.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 14:59:06.568534 moonstreamdb-v3-0.0.7/moonstreamdbv3/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 14:58:44.000000 moonstreamdb-v3-0.0.7/moonstreamdbv3/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 14:59:06.568534 moonstreamdb-v3-0.0.7/moonstreamdbv3/alembic/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 14:58:44.000000 moonstreamdb-v3-0.0.7/moonstreamdbv3/alembic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3970 2024-06-03 14:58:44.000000 moonstreamdb-v3-0.0.7/moonstreamdbv3/alembic/env.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 14:59:06.568534 moonstreamdb-v3-0.0.7/moonstreamdbv3/alembic/versions/
+-rw-r--r--   0 runner    (1001) docker     (127)    49749 2024-06-03 14:58:44.000000 moonstreamdb-v3-0.0.7/moonstreamdbv3/alembic/versions/994e614b5500_tables_initial_generation.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13587 2024-06-03 14:58:44.000000 moonstreamdb-v3-0.0.7/moonstreamdbv3/alembic/versions/9ca39b11e12a_game7_orbit_and_mantle_blockchain_models.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 14:58:44.000000 moonstreamdb-v3-0.0.7/moonstreamdbv3/alembic/versions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15836 2024-06-03 14:58:44.000000 moonstreamdb-v3-0.0.7/moonstreamdbv3/alembic/versions/d2ceff33be47_tx_call_and_event_unique_indexes.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13956 2024-06-03 14:58:44.000000 moonstreamdb-v3-0.0.7/moonstreamdbv3/alembic/versions/e9e1b43f49e1_amoy_blast_and_apex_blockchains.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4109 2024-06-03 14:58:44.000000 moonstreamdb-v3-0.0.7/moonstreamdbv3/alembic/versions/e9f640a2b45b_arbitrum_one_blockchain.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 14:59:06.568534 moonstreamdb-v3-0.0.7/moonstreamdbv3/alembic_indexes/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 14:58:44.000000 moonstreamdb-v3-0.0.7/moonstreamdbv3/alembic_indexes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5181 2024-06-03 14:58:44.000000 moonstreamdb-v3-0.0.7/moonstreamdbv3/alembic_indexes/env.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 14:59:06.568534 moonstreamdb-v3-0.0.7/moonstreamdbv3/alembic_indexes/versions/
+-rw-r--r--   0 runner    (1001) docker     (127)    16088 2024-06-03 14:58:44.000000 moonstreamdb-v3-0.0.7/moonstreamdbv3/alembic_indexes/versions/0ea24314c181_init_v3_index.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 14:58:44.000000 moonstreamdb-v3-0.0.7/moonstreamdbv3/alembic_indexes/versions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    48649 2024-06-03 14:58:44.000000 moonstreamdb-v3-0.0.7/moonstreamdbv3/alembic_indexes/versions/a4ef4f9031e4_game7_orbit_arbitrum_xai_and_mantle_.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4548 2024-06-03 14:58:44.000000 moonstreamdb-v3-0.0.7/moonstreamdbv3/db.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24136 2024-06-03 14:58:44.000000 moonstreamdb-v3-0.0.7/moonstreamdbv3/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14696 2024-06-03 14:58:44.000000 moonstreamdb-v3-0.0.7/moonstreamdbv3/models_indexes.py
+-rw-r--r--   0 runner    (1001) docker     (127)      234 2024-06-03 14:58:44.000000 moonstreamdb-v3-0.0.7/moonstreamdbv3/version.py
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-06-03 14:59:06.568534 moonstreamdb-v3-0.0.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1360 2024-06-03 14:58:44.000000 moonstreamdb-v3-0.0.7/setup.py
```

### Comparing `moonstreamdb-v3-0.0.6/PKG-INFO` & `moonstreamdb-v3-0.0.7/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: moonstreamdb-v3
-Version: 0.0.6
+Version: 0.0.7
 Summary: Moonstream V3 database
 Home-page: https://github.com/bugout-dev/moonstream
 Author: Bugout.dev
 Author-email: engineers@bugout.dev
 License: Apache License 2.0
 Description: # moonstreamdb-v3
```

### Comparing `moonstreamdb-v3-0.0.6/moonstreamdb_v3.egg-info/PKG-INFO` & `moonstreamdb-v3-0.0.7/moonstreamdb_v3.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: moonstreamdb-v3
-Version: 0.0.6
+Version: 0.0.7
 Summary: Moonstream V3 database
 Home-page: https://github.com/bugout-dev/moonstream
 Author: Bugout.dev
 Author-email: engineers@bugout.dev
 License: Apache License 2.0
 Description: # moonstreamdb-v3
```

### Comparing `moonstreamdb-v3-0.0.6/moonstreamdb_v3.egg-info/SOURCES.txt` & `moonstreamdb-v3-0.0.7/moonstreamdb_v3.egg-info/SOURCES.txt`

 * *Files 22% similar despite different names*

```diff
@@ -10,15 +10,17 @@
 moonstreamdbv3/db.py
 moonstreamdbv3/models.py
 moonstreamdbv3/models_indexes.py
 moonstreamdbv3/version.py
 moonstreamdbv3/alembic/__init__.py
 moonstreamdbv3/alembic/env.py
 moonstreamdbv3/alembic/versions/994e614b5500_tables_initial_generation.py
+moonstreamdbv3/alembic/versions/9ca39b11e12a_game7_orbit_and_mantle_blockchain_models.py
 moonstreamdbv3/alembic/versions/__init__.py
 moonstreamdbv3/alembic/versions/d2ceff33be47_tx_call_and_event_unique_indexes.py
 moonstreamdbv3/alembic/versions/e9e1b43f49e1_amoy_blast_and_apex_blockchains.py
 moonstreamdbv3/alembic/versions/e9f640a2b45b_arbitrum_one_blockchain.py
 moonstreamdbv3/alembic_indexes/__init__.py
 moonstreamdbv3/alembic_indexes/env.py
 moonstreamdbv3/alembic_indexes/versions/0ea24314c181_init_v3_index.py
-moonstreamdbv3/alembic_indexes/versions/__init__.py
+moonstreamdbv3/alembic_indexes/versions/__init__.py
+moonstreamdbv3/alembic_indexes/versions/a4ef4f9031e4_game7_orbit_arbitrum_xai_and_mantle_.py
```

### Comparing `moonstreamdb-v3-0.0.6/moonstreamdbv3/alembic/env.py` & `moonstreamdb-v3-0.0.7/moonstreamdbv3/alembic/env.py`

 * *Files 7% similar despite different names*

```diff
@@ -35,23 +35,26 @@
     XDaiLabel,
     ZkSyncEraLabel,
     ZkSyncEraSepoliaLabel,
     BaseLabel,
     ArbitrumNovaLabel,
     ArbitrumOneLabel,
     ArbitrumSepoliaLabel,
+    Game7OrbitArbitrumSepoliaLabel,
     XaiLabel,
     XaiSepoliaLabel,
     AvalancheLabel,
     AvalancheFujiLabel,
     BlastLabel,
     BlastSepoliaLabel,
     ProofOfPlayApexLabel,
     StarknetLabel,
     StarknetSepoliaLabel,
+    MantleLabel,
+    MantleSepoliaLabel,
 )
 
 
 def include_symbol(tablename, schema):
     return tablename in {
         EthereumLabel.__tablename__,
         SepoliaLabel.__tablename__,
@@ -59,24 +62,28 @@
         MumbaiLabel.__tablename__,
         AmoyLabel.__tablename__,
         XDaiLabel.__tablename__,
         ZkSyncEraLabel.__tablename__,
         ZkSyncEraSepoliaLabel.__tablename__,
         BaseLabel.__tablename__,
         ArbitrumNovaLabel.__tablename__,
+        ArbitrumOneLabel.__tablename__,
         ArbitrumSepoliaLabel.__tablename__,
+        Game7OrbitArbitrumSepoliaLabel.__tablename__,
         XaiLabel.__tablename__,
         XaiSepoliaLabel.__tablename__,
         AvalancheLabel.__tablename__,
         AvalancheFujiLabel.__tablename__,
         BlastLabel.__tablename__,
         BlastSepoliaLabel.__tablename__,
         ProofOfPlayApexLabel.__tablename__,
         StarknetLabel.__tablename__,
         StarknetSepoliaLabel.__tablename__,
+        MantleLabel.__tablename__,
+        MantleSepoliaLabel.__tablename__,
     }
 
 
 def run_migrations_offline() -> None:
     """Run migrations in 'offline' mode.
 
     This configures the context with just a URL
```

### Comparing `moonstreamdb-v3-0.0.6/moonstreamdbv3/alembic/versions/994e614b5500_tables_initial_generation.py` & `moonstreamdb-v3-0.0.7/moonstreamdbv3/alembic/versions/994e614b5500_tables_initial_generation.py`

 * *Files identical despite different names*

### Comparing `moonstreamdb-v3-0.0.6/moonstreamdbv3/alembic/versions/d2ceff33be47_tx_call_and_event_unique_indexes.py` & `moonstreamdb-v3-0.0.7/moonstreamdbv3/alembic/versions/d2ceff33be47_tx_call_and_event_unique_indexes.py`

 * *Files identical despite different names*

### Comparing `moonstreamdb-v3-0.0.6/moonstreamdbv3/alembic/versions/e9e1b43f49e1_amoy_blast_and_apex_blockchains.py` & `moonstreamdb-v3-0.0.7/moonstreamdbv3/alembic/versions/e9e1b43f49e1_amoy_blast_and_apex_blockchains.py`

 * *Files identical despite different names*

### Comparing `moonstreamdb-v3-0.0.6/moonstreamdbv3/alembic/versions/e9f640a2b45b_arbitrum_one_blockchain.py` & `moonstreamdb-v3-0.0.7/moonstreamdbv3/alembic/versions/e9f640a2b45b_arbitrum_one_blockchain.py`

 * *Files identical despite different names*

### Comparing `moonstreamdb-v3-0.0.6/moonstreamdbv3/alembic_indexes/versions/0ea24314c181_init_v3_index.py` & `moonstreamdb-v3-0.0.7/moonstreamdbv3/alembic_indexes/versions/0ea24314c181_init_v3_index.py`

 * *Files identical despite different names*

### Comparing `moonstreamdb-v3-0.0.6/moonstreamdbv3/db.py` & `moonstreamdb-v3-0.0.7/moonstreamdbv3/db.py`

 * *Files identical despite different names*

### Comparing `moonstreamdb-v3-0.0.6/moonstreamdbv3/models.py` & `moonstreamdb-v3-0.0.7/moonstreamdbv3/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -497,14 +497,46 @@
             "log_index",
             unique=True,
             postgresql_where=text("label='seer' and label_type='event'"),
         ),
     )
 
 
+class Game7OrbitArbitrumSepoliaLabel(EvmBasedLabel):  # type: ignore
+    __tablename__ = "game7_orbit_arbitrum_sepolia_labels"
+
+    __table_args__ = (
+        Index(
+            "ix_g7o_arbitrum_sepolia_labels_addr_block_num",
+            "address",
+            "block_number",
+            unique=False,
+        ),
+        Index(
+            "ix_g7o_arbitrum_sepolia_labels_addr_block_ts",
+            "address",
+            "block_timestamp",
+            unique=False,
+        ),
+        Index(
+            "uk_g7o_arbitrum_sepolia_labels_tx_hash_tx_call",
+            "transaction_hash",
+            unique=True,
+            postgresql_where=text("label='seer' and label_type='tx_call'"),
+        ),
+        Index(
+            "uk_g7o_arbitrum_sepolia_labels_tx_hash_log_idx_evt",
+            "transaction_hash",
+            "log_index",
+            unique=True,
+            postgresql_where=text("label='seer' and label_type='event'"),
+        ),
+    )
+
+
 class XaiLabel(EvmBasedLabel):  # type: ignore
     __tablename__ = "xai_labels"
 
     __table_args__ = (
         Index(
             "ix_xai_labels_addr_block_num",
             "address",
@@ -783,7 +815,71 @@
             "uk_starknet_sepolia_labels_tx_hash_log_idx_evt",
             "transaction_hash",
             "log_index",
             unique=True,
             postgresql_where=text("label='seer' and label_type='event'"),
         ),
     )
+
+
+class MantleLabel(EvmBasedLabel):  # type: ignore
+    __tablename__ = "mantle_labels"
+
+    __table_args__ = (
+        Index(
+            "ix_mantle_labels_addr_block_num",
+            "address",
+            "block_number",
+            unique=False,
+        ),
+        Index(
+            "ix_mantle_labels_addr_block_ts",
+            "address",
+            "block_timestamp",
+            unique=False,
+        ),
+        Index(
+            "uk_mantle_labels_tx_hash_tx_call",
+            "transaction_hash",
+            unique=True,
+            postgresql_where=text("label='seer' and label_type='tx_call'"),
+        ),
+        Index(
+            "uk_mantle_labels_tx_hash_log_idx_evt",
+            "transaction_hash",
+            "log_index",
+            unique=True,
+            postgresql_where=text("label='seer' and label_type='event'"),
+        ),
+    )
+
+
+class MantleSepoliaLabel(EvmBasedLabel):  # type: ignore
+    __tablename__ = "mantle_sepolia_labels"
+
+    __table_args__ = (
+        Index(
+            "ix_mantle_sepolia_labels_addr_block_num",
+            "address",
+            "block_number",
+            unique=False,
+        ),
+        Index(
+            "ix_mantle_sepolia_labels_addr_block_ts",
+            "address",
+            "block_timestamp",
+            unique=False,
+        ),
+        Index(
+            "uk_mantle_sepolia_labels_tx_hash_tx_call",
+            "transaction_hash",
+            unique=True,
+            postgresql_where=text("label='seer' and label_type='tx_call'"),
+        ),
+        Index(
+            "uk_mantle_sepolia_labels_tx_hash_log_idx_evt",
+            "transaction_hash",
+            "log_index",
+            unique=True,
+            postgresql_where=text("label='seer' and label_type='event'"),
+        ),
+    )
```

### Comparing `moonstreamdb-v3-0.0.6/setup.py` & `moonstreamdb-v3-0.0.7/setup.py`

 * *Files identical despite different names*

